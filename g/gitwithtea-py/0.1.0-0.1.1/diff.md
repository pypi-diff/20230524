# Comparing `tmp/gitwithtea_py-0.1.0.tar.gz` & `tmp/gitwithtea_py-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gitwithtea_py-0.1.0.tar", max compression
+gzip compressed data, was "gitwithtea_py-0.1.1.tar", max compression
```

## Comparing `gitwithtea_py-0.1.0.tar` & `gitwithtea_py-0.1.1.tar`

### file list

```diff
@@ -1,185 +1,185 @@
--rw-r--r--   0        0        0    64033 2023-05-24 13:56:05.378940 gitwithtea_py-0.1.0/README.md
--rw-r--r--   0        0        0    11991 2023-05-24 13:56:05.401940 gitwithtea_py-0.1.0/gitwithtea_py/__init__.py
--rw-r--r--   0        0        0      651 2023-05-24 13:56:05.817942 gitwithtea_py-0.1.0/gitwithtea_py/api/__init__.py
--rw-r--r--   0        0        0     8720 2023-05-24 13:56:05.555941 gitwithtea_py-0.1.0/gitwithtea_py/api/activitypub_api.py
--rw-r--r--   0        0        0    77872 2023-05-24 13:56:05.519940 gitwithtea_py-0.1.0/gitwithtea_py/api/admin_api.py
--rw-r--r--   0        0        0   322896 2023-05-24 13:56:05.555941 gitwithtea_py-0.1.0/gitwithtea_py/api/issue_api.py
--rw-r--r--   0        0        0    17886 2023-05-24 13:56:05.817942 gitwithtea_py-0.1.0/gitwithtea_py/api/miscellaneous_api.py
--rw-r--r--   0        0        0    35978 2023-05-24 13:56:05.520941 gitwithtea_py-0.1.0/gitwithtea_py/api/notification_api.py
--rw-r--r--   0        0        0   184878 2023-05-24 13:56:05.817942 gitwithtea_py-0.1.0/gitwithtea_py/api/organization_api.py
--rw-r--r--   0        0        0    22639 2023-05-24 13:56:05.519940 gitwithtea_py-0.1.0/gitwithtea_py/api/package_api.py
--rw-r--r--   0        0        0   703704 2023-05-24 13:56:06.572945 gitwithtea_py-0.1.0/gitwithtea_py/api/repository_api.py
--rw-r--r--   0        0        0    14488 2023-05-24 13:56:05.519940 gitwithtea_py-0.1.0/gitwithtea_py/api/settings_api.py
--rw-r--r--   0        0        0   200637 2023-05-24 13:56:05.520941 gitwithtea_py-0.1.0/gitwithtea_py/api/user_api.py
--rw-r--r--   0        0        0    25058 2023-05-24 13:56:05.401940 gitwithtea_py-0.1.0/gitwithtea_py/api_client.py
--rw-r--r--   0        0        0     9652 2023-05-24 13:56:05.401940 gitwithtea_py-0.1.0/gitwithtea_py/configuration.py
--rw-r--r--   0        0        0    11276 2023-05-24 13:56:05.519940 gitwithtea_py-0.1.0/gitwithtea_py/models/__init__.py
--rw-r--r--   0        0        0     5816 2023-05-24 13:56:05.519940 gitwithtea_py-0.1.0/gitwithtea_py/models/access_token.py
--rw-r--r--   0        0        0     3327 2023-05-24 13:56:05.434940 gitwithtea_py-0.1.0/gitwithtea_py/models/activity_pub.py
--rw-r--r--   0        0        0     3476 2023-05-24 13:56:05.519940 gitwithtea_py-0.1.0/gitwithtea_py/models/add_collaborator_option.py
--rw-r--r--   0        0        0     4941 2023-05-24 13:56:05.519940 gitwithtea_py-0.1.0/gitwithtea_py/models/add_time_option.py
--rw-r--r--   0        0        0     7109 2023-05-24 13:56:05.519940 gitwithtea_py-0.1.0/gitwithtea_py/models/annotated_tag.py
--rw-r--r--   0        0        0     4491 2023-05-24 13:56:05.434940 gitwithtea_py-0.1.0/gitwithtea_py/models/annotated_tag_object.py
--rw-r--r--   0        0        0     3840 2023-05-24 13:56:05.415940 gitwithtea_py-0.1.0/gitwithtea_py/models/api_error.py
--rw-r--r--   0        0        0     7286 2023-05-24 13:56:05.519940 gitwithtea_py-0.1.0/gitwithtea_py/models/attachment.py
--rw-r--r--   0        0        0     9705 2023-05-24 13:56:05.519940 gitwithtea_py-0.1.0/gitwithtea_py/models/branch.py
--rw-r--r--   0        0        0    26670 2023-05-24 13:56:05.467940 gitwithtea_py-0.1.0/gitwithtea_py/models/branch_protection.py
--rw-r--r--   0        0        0     8790 2023-05-24 13:56:05.519940 gitwithtea_py-0.1.0/gitwithtea_py/models/changed_file.py
--rw-r--r--   0        0        0     7351 2023-05-24 13:56:05.434940 gitwithtea_py-0.1.0/gitwithtea_py/models/combined_status.py
--rw-r--r--   0        0        0    10032 2023-05-24 13:56:05.434940 gitwithtea_py-0.1.0/gitwithtea_py/models/comment.py
--rw-r--r--   0        0        0     8749 2023-05-24 13:56:05.415940 gitwithtea_py-0.1.0/gitwithtea_py/models/commit.py
--rw-r--r--   0        0        0     3418 2023-05-24 13:56:05.467940 gitwithtea_py-0.1.0/gitwithtea_py/models/commit_affected_files.py
--rw-r--r--   0        0        0     4087 2023-05-24 13:56:05.519940 gitwithtea_py-0.1.0/gitwithtea_py/models/commit_date_options.py
--rw-r--r--   0        0        0     4430 2023-05-24 13:56:05.467940 gitwithtea_py-0.1.0/gitwithtea_py/models/commit_meta.py
--rw-r--r--   0        0        0     4632 2023-05-24 13:56:05.434940 gitwithtea_py-0.1.0/gitwithtea_py/models/commit_stats.py
--rw-r--r--   0        0        0     8566 2023-05-24 13:56:05.401940 gitwithtea_py-0.1.0/gitwithtea_py/models/commit_status.py
--rw-r--r--   0        0        0     2723 2023-05-24 13:56:05.434940 gitwithtea_py-0.1.0/gitwithtea_py/models/commit_status_state.py
--rw-r--r--   0        0        0     4434 2023-05-24 13:56:05.434940 gitwithtea_py-0.1.0/gitwithtea_py/models/commit_user.py
--rw-r--r--   0        0        0    13452 2023-05-24 13:56:05.434940 gitwithtea_py-0.1.0/gitwithtea_py/models/contents_response.py
--rw-r--r--   0        0        0     4183 2023-05-24 13:56:05.467940 gitwithtea_py-0.1.0/gitwithtea_py/models/create_access_token_option.py
--rw-r--r--   0        0        0    26378 2023-05-24 13:56:05.434940 gitwithtea_py-0.1.0/gitwithtea_py/models/create_branch_protection_option.py
--rw-r--r--   0        0        0     4785 2023-05-24 13:56:05.434940 gitwithtea_py-0.1.0/gitwithtea_py/models/create_branch_repo_option.py
--rw-r--r--   0        0        0     3468 2023-05-24 13:56:05.434940 gitwithtea_py-0.1.0/gitwithtea_py/models/create_email_option.py
--rw-r--r--   0        0        0     9181 2023-05-24 13:56:05.434940 gitwithtea_py-0.1.0/gitwithtea_py/models/create_file_options.py
--rw-r--r--   0        0        0     4314 2023-05-24 13:56:05.434940 gitwithtea_py-0.1.0/gitwithtea_py/models/create_fork_option.py
--rw-r--r--   0        0        0     4710 2023-05-24 13:56:05.519940 gitwithtea_py-0.1.0/gitwithtea_py/models/create_gpg_key_option.py
--rw-r--r--   0        0        0     7686 2023-05-24 13:56:05.434940 gitwithtea_py-0.1.0/gitwithtea_py/models/create_hook_option.py
--rw-r--r--   0        0        0     2748 2023-05-24 13:56:05.519940 gitwithtea_py-0.1.0/gitwithtea_py/models/create_hook_option_config.py
--rw-r--r--   0        0        0     3513 2023-05-24 13:56:05.435940 gitwithtea_py-0.1.0/gitwithtea_py/models/create_issue_comment_option.py
--rw-r--r--   0        0        0     8937 2023-05-24 13:56:05.434940 gitwithtea_py-0.1.0/gitwithtea_py/models/create_issue_option.py
--rw-r--r--   0        0        0     5185 2023-05-24 13:56:05.434940 gitwithtea_py-0.1.0/gitwithtea_py/models/create_key_option.py
--rw-r--r--   0        0        0     5635 2023-05-24 13:56:05.519940 gitwithtea_py-0.1.0/gitwithtea_py/models/create_label_option.py
--rw-r--r--   0        0        0     5768 2023-05-24 13:56:05.434940 gitwithtea_py-0.1.0/gitwithtea_py/models/create_milestone_option.py
--rw-r--r--   0        0        0     5236 2023-05-24 13:56:05.434940 gitwithtea_py-0.1.0/gitwithtea_py/models/create_o_auth2_application_options.py
--rw-r--r--   0        0        0     8730 2023-05-24 13:56:05.467940 gitwithtea_py-0.1.0/gitwithtea_py/models/create_org_option.py
--rw-r--r--   0        0        0     8813 2023-05-24 13:56:05.434940 gitwithtea_py-0.1.0/gitwithtea_py/models/create_pull_request_option.py
--rw-r--r--   0        0        0     5849 2023-05-24 13:56:05.519940 gitwithtea_py-0.1.0/gitwithtea_py/models/create_pull_review_comment.py
--rw-r--r--   0        0        0     5551 2023-05-24 13:56:05.407940 gitwithtea_py-0.1.0/gitwithtea_py/models/create_pull_review_options.py
--rw-r--r--   0        0        0     6756 2023-05-24 13:56:05.415940 gitwithtea_py-0.1.0/gitwithtea_py/models/create_push_mirror_option.py
--rw-r--r--   0        0        0     6963 2023-05-24 13:56:05.519940 gitwithtea_py-0.1.0/gitwithtea_py/models/create_release_option.py
--rw-r--r--   0        0        0    12125 2023-05-24 13:56:05.467940 gitwithtea_py-0.1.0/gitwithtea_py/models/create_repo_option.py
--rw-r--r--   0        0        0     5514 2023-05-24 13:56:05.519940 gitwithtea_py-0.1.0/gitwithtea_py/models/create_status_option.py
--rw-r--r--   0        0        0     4794 2023-05-24 13:56:05.401940 gitwithtea_py-0.1.0/gitwithtea_py/models/create_tag_option.py
--rw-r--r--   0        0        0     8517 2023-05-24 13:56:05.407940 gitwithtea_py-0.1.0/gitwithtea_py/models/create_team_option.py
--rw-r--r--   0        0        0    11370 2023-05-24 13:56:05.434940 gitwithtea_py-0.1.0/gitwithtea_py/models/create_user_option.py
--rw-r--r--   0        0        0     5234 2023-05-24 13:56:05.401940 gitwithtea_py-0.1.0/gitwithtea_py/models/create_wiki_page_options.py
--rw-r--r--   0        0        0     5613 2023-05-24 13:56:05.467940 gitwithtea_py-0.1.0/gitwithtea_py/models/cron.py
--rw-r--r--   0        0        0     3474 2023-05-24 13:56:05.434940 gitwithtea_py-0.1.0/gitwithtea_py/models/delete_email_option.py
--rw-r--r--   0        0        0     9131 2023-05-24 13:56:05.519940 gitwithtea_py-0.1.0/gitwithtea_py/models/delete_file_options.py
--rw-r--r--   0        0        0     8267 2023-05-24 13:56:05.434940 gitwithtea_py-0.1.0/gitwithtea_py/models/deploy_key.py
--rw-r--r--   0        0        0     4111 2023-05-24 13:56:05.519940 gitwithtea_py-0.1.0/gitwithtea_py/models/dismiss_pull_review_options.py
--rw-r--r--   0        0        0     3356 2023-05-24 13:56:05.519940 gitwithtea_py-0.1.0/gitwithtea_py/models/edit_attachment_options.py
--rw-r--r--   0        0        0    24600 2023-05-24 13:56:05.519940 gitwithtea_py-0.1.0/gitwithtea_py/models/edit_branch_protection_option.py
--rw-r--r--   0        0        0     3558 2023-05-24 13:56:05.519940 gitwithtea_py-0.1.0/gitwithtea_py/models/edit_deadline_option.py
--rw-r--r--   0        0        0     3380 2023-05-24 13:56:05.519940 gitwithtea_py-0.1.0/gitwithtea_py/models/edit_git_hook_option.py
--rw-r--r--   0        0        0     6307 2023-05-24 13:56:05.415940 gitwithtea_py-0.1.0/gitwithtea_py/models/edit_hook_option.py
--rw-r--r--   0        0        0     3495 2023-05-24 13:56:05.435940 gitwithtea_py-0.1.0/gitwithtea_py/models/edit_issue_comment_option.py
--rw-r--r--   0        0        0     8696 2023-05-24 13:56:05.519940 gitwithtea_py-0.1.0/gitwithtea_py/models/edit_issue_option.py
--rw-r--r--   0        0        0     5332 2023-05-24 13:56:05.467940 gitwithtea_py-0.1.0/gitwithtea_py/models/edit_label_option.py
--rw-r--r--   0        0        0     5388 2023-05-24 13:56:05.435940 gitwithtea_py-0.1.0/gitwithtea_py/models/edit_milestone_option.py
--rw-r--r--   0        0        0     7849 2023-05-24 13:56:05.519940 gitwithtea_py-0.1.0/gitwithtea_py/models/edit_org_option.py
--rw-r--r--   0        0        0    10523 2023-05-24 13:56:05.434940 gitwithtea_py-0.1.0/gitwithtea_py/models/edit_pull_request_option.py
--rw-r--r--   0        0        0     3389 2023-05-24 13:56:05.435940 gitwithtea_py-0.1.0/gitwithtea_py/models/edit_reaction_option.py
--rw-r--r--   0        0        0     6771 2023-05-24 13:56:05.435940 gitwithtea_py-0.1.0/gitwithtea_py/models/edit_release_option.py
--rw-r--r--   0        0        0    29858 2023-05-24 13:56:05.434940 gitwithtea_py-0.1.0/gitwithtea_py/models/edit_repo_option.py
--rw-r--r--   0        0        0     8451 2023-05-24 13:56:05.467940 gitwithtea_py-0.1.0/gitwithtea_py/models/edit_team_option.py
--rw-r--r--   0        0        0    16213 2023-05-24 13:56:05.519940 gitwithtea_py-0.1.0/gitwithtea_py/models/edit_user_option.py
--rw-r--r--   0        0        0     4476 2023-05-24 13:56:05.434940 gitwithtea_py-0.1.0/gitwithtea_py/models/email.py
--rw-r--r--   0        0        0     7439 2023-05-24 13:56:05.467940 gitwithtea_py-0.1.0/gitwithtea_py/models/external_tracker.py
--rw-r--r--   0        0        0     3623 2023-05-24 13:56:05.435940 gitwithtea_py-0.1.0/gitwithtea_py/models/external_wiki.py
--rw-r--r--   0        0        0     8614 2023-05-24 13:56:05.519940 gitwithtea_py-0.1.0/gitwithtea_py/models/file_commit_response.py
--rw-r--r--   0        0        0     4911 2023-05-24 13:56:05.434940 gitwithtea_py-0.1.0/gitwithtea_py/models/file_delete_response.py
--rw-r--r--   0        0        0     4513 2023-05-24 13:56:05.434940 gitwithtea_py-0.1.0/gitwithtea_py/models/file_links_response.py
--rw-r--r--   0        0        0     4839 2023-05-24 13:56:05.519940 gitwithtea_py-0.1.0/gitwithtea_py/models/file_response.py
--rw-r--r--   0        0        0     6472 2023-05-24 13:56:05.434940 gitwithtea_py-0.1.0/gitwithtea_py/models/general_api_settings.py
--rw-r--r--   0        0        0     5702 2023-05-24 13:56:05.467940 gitwithtea_py-0.1.0/gitwithtea_py/models/general_attachment_settings.py
--rw-r--r--   0        0        0     7901 2023-05-24 13:56:05.434940 gitwithtea_py-0.1.0/gitwithtea_py/models/general_repo_settings.py
--rw-r--r--   0        0        0     5170 2023-05-24 13:56:05.519940 gitwithtea_py-0.1.0/gitwithtea_py/models/general_ui_settings.py
--rw-r--r--   0        0        0    11819 2023-05-24 13:56:05.434940 gitwithtea_py-0.1.0/gitwithtea_py/models/generate_repo_option.py
--rw-r--r--   0        0        0     5758 2023-05-24 13:56:05.434940 gitwithtea_py-0.1.0/gitwithtea_py/models/git_blob_response.py
--rw-r--r--   0        0        0     6004 2023-05-24 13:56:05.434940 gitwithtea_py-0.1.0/gitwithtea_py/models/git_entry.py
--rw-r--r--   0        0        0     4507 2023-05-24 13:56:05.467940 gitwithtea_py-0.1.0/gitwithtea_py/models/git_hook.py
--rw-r--r--   0        0        0     4338 2023-05-24 13:56:05.434940 gitwithtea_py-0.1.0/gitwithtea_py/models/git_object.py
--rw-r--r--   0        0        0     6483 2023-05-24 13:56:05.467940 gitwithtea_py-0.1.0/gitwithtea_py/models/git_tree_response.py
--rw-r--r--   0        0        0    11491 2023-05-24 13:56:05.467940 gitwithtea_py-0.1.0/gitwithtea_py/models/gpg_key.py
--rw-r--r--   0        0        0     3942 2023-05-24 13:56:05.519940 gitwithtea_py-0.1.0/gitwithtea_py/models/gpg_key_email.py
--rw-r--r--   0        0        0     7742 2023-05-24 13:56:05.434940 gitwithtea_py-0.1.0/gitwithtea_py/models/hook.py
--rw-r--r--   0        0        0     3820 2023-05-24 13:56:05.435940 gitwithtea_py-0.1.0/gitwithtea_py/models/identity.py
--rw-r--r--   0        0        0     3901 2023-05-24 13:56:05.467940 gitwithtea_py-0.1.0/gitwithtea_py/models/inline_response200.py
--rw-r--r--   0        0        0     3914 2023-05-24 13:56:05.401940 gitwithtea_py-0.1.0/gitwithtea_py/models/inline_response2001.py
--rw-r--r--   0        0        0     6357 2023-05-24 13:56:05.434940 gitwithtea_py-0.1.0/gitwithtea_py/models/internal_tracker.py
--rw-r--r--   0        0        0    17917 2023-05-24 13:56:05.519940 gitwithtea_py-0.1.0/gitwithtea_py/models/issue.py
--rw-r--r--   0        0        0     3379 2023-05-24 13:56:05.467940 gitwithtea_py-0.1.0/gitwithtea_py/models/issue_deadline.py
--rw-r--r--   0        0        0     5397 2023-05-24 13:56:05.519940 gitwithtea_py-0.1.0/gitwithtea_py/models/issue_form_field.py
--rw-r--r--   0        0        0     2728 2023-05-24 13:56:05.434940 gitwithtea_py-0.1.0/gitwithtea_py/models/issue_form_field_type.py
--rw-r--r--   0        0        0     3458 2023-05-24 13:56:05.415940 gitwithtea_py-0.1.0/gitwithtea_py/models/issue_labels_option.py
--rw-r--r--   0        0        0     7670 2023-05-24 13:56:05.401940 gitwithtea_py-0.1.0/gitwithtea_py/models/issue_template.py
--rw-r--r--   0        0        0     2733 2023-05-24 13:56:05.401940 gitwithtea_py-0.1.0/gitwithtea_py/models/issue_template_labels.py
--rw-r--r--   0        0        0     6160 2023-05-24 13:56:05.434940 gitwithtea_py-0.1.0/gitwithtea_py/models/label.py
--rw-r--r--   0        0        0     5521 2023-05-24 13:56:05.434940 gitwithtea_py-0.1.0/gitwithtea_py/models/markdown_option.py
--rw-r--r--   0        0        0    10110 2023-05-24 13:56:05.434940 gitwithtea_py-0.1.0/gitwithtea_py/models/merge_pull_request_option.py
--rw-r--r--   0        0        0    17639 2023-05-24 13:56:05.467940 gitwithtea_py-0.1.0/gitwithtea_py/models/migrate_repo_options.py
--rw-r--r--   0        0        0     9251 2023-05-24 13:56:05.519940 gitwithtea_py-0.1.0/gitwithtea_py/models/milestone.py
--rw-r--r--   0        0        0     7442 2023-05-24 13:56:05.519940 gitwithtea_py-0.1.0/gitwithtea_py/models/node_info.py
--rw-r--r--   0        0        0     4080 2023-05-24 13:56:05.519940 gitwithtea_py-0.1.0/gitwithtea_py/models/node_info_services.py
--rw-r--r--   0        0        0     5350 2023-05-24 13:56:05.519940 gitwithtea_py-0.1.0/gitwithtea_py/models/node_info_software.py
--rw-r--r--   0        0        0     4849 2023-05-24 13:56:05.434940 gitwithtea_py-0.1.0/gitwithtea_py/models/node_info_usage.py
--rw-r--r--   0        0        0     4929 2023-05-24 13:56:05.519940 gitwithtea_py-0.1.0/gitwithtea_py/models/node_info_usage_users.py
--rw-r--r--   0        0        0     3857 2023-05-24 13:56:05.415940 gitwithtea_py-0.1.0/gitwithtea_py/models/note.py
--rw-r--r--   0        0        0     3300 2023-05-24 13:56:05.434940 gitwithtea_py-0.1.0/gitwithtea_py/models/notification_count.py
--rw-r--r--   0        0        0     7788 2023-05-24 13:56:05.407940 gitwithtea_py-0.1.0/gitwithtea_py/models/notification_subject.py
--rw-r--r--   0        0        0     7345 2023-05-24 13:56:05.434940 gitwithtea_py-0.1.0/gitwithtea_py/models/notification_thread.py
--rw-r--r--   0        0        0     2723 2023-05-24 13:56:05.415940 gitwithtea_py-0.1.0/gitwithtea_py/models/notify_subject_type.py
--rw-r--r--   0        0        0     7718 2023-05-24 13:56:05.519940 gitwithtea_py-0.1.0/gitwithtea_py/models/o_auth2_application.py
--rw-r--r--   0        0        0     9837 2023-05-24 13:56:05.435940 gitwithtea_py-0.1.0/gitwithtea_py/models/organization.py
--rw-r--r--   0        0        0     6553 2023-05-24 13:56:05.434940 gitwithtea_py-0.1.0/gitwithtea_py/models/organization_permissions.py
--rw-r--r--   0        0        0     7511 2023-05-24 13:56:05.519940 gitwithtea_py-0.1.0/gitwithtea_py/models/package.py
--rw-r--r--   0        0        0     6724 2023-05-24 13:56:05.434940 gitwithtea_py-0.1.0/gitwithtea_py/models/package_file.py
--rw-r--r--   0        0        0     9348 2023-05-24 13:56:05.519940 gitwithtea_py-0.1.0/gitwithtea_py/models/payload_commit.py
--rw-r--r--   0        0        0     6255 2023-05-24 13:56:05.519940 gitwithtea_py-0.1.0/gitwithtea_py/models/payload_commit_verification.py
--rw-r--r--   0        0        0     4618 2023-05-24 13:56:05.519940 gitwithtea_py-0.1.0/gitwithtea_py/models/payload_user.py
--rw-r--r--   0        0        0     4424 2023-05-24 13:56:05.434940 gitwithtea_py-0.1.0/gitwithtea_py/models/permission.py
--rw-r--r--   0        0        0     5644 2023-05-24 13:56:05.434940 gitwithtea_py-0.1.0/gitwithtea_py/models/pr_branch_info.py
--rw-r--r--   0        0        0     8169 2023-05-24 13:56:05.434940 gitwithtea_py-0.1.0/gitwithtea_py/models/public_key.py
--rw-r--r--   0        0        0    21781 2023-05-24 13:56:05.519940 gitwithtea_py-0.1.0/gitwithtea_py/models/pull_request.py
--rw-r--r--   0        0        0     4049 2023-05-24 13:56:05.519940 gitwithtea_py-0.1.0/gitwithtea_py/models/pull_request_meta.py
--rw-r--r--   0        0        0    11955 2023-05-24 13:56:05.519940 gitwithtea_py-0.1.0/gitwithtea_py/models/pull_review.py
--rw-r--r--   0        0        0    13494 2023-05-24 13:56:05.519940 gitwithtea_py-0.1.0/gitwithtea_py/models/pull_review_comment.py
--rw-r--r--   0        0        0     4484 2023-05-24 13:56:05.519940 gitwithtea_py-0.1.0/gitwithtea_py/models/pull_review_request_options.py
--rw-r--r--   0        0        0     8283 2023-05-24 13:56:05.467940 gitwithtea_py-0.1.0/gitwithtea_py/models/push_mirror.py
--rw-r--r--   0        0        0     4559 2023-05-24 13:56:05.434940 gitwithtea_py-0.1.0/gitwithtea_py/models/reaction.py
--rw-r--r--   0        0        0     4396 2023-05-24 13:56:05.415940 gitwithtea_py-0.1.0/gitwithtea_py/models/reference.py
--rw-r--r--   0        0        0    12226 2023-05-24 13:56:05.519940 gitwithtea_py-0.1.0/gitwithtea_py/models/release.py
--rw-r--r--   0        0        0     4890 2023-05-24 13:56:05.519940 gitwithtea_py-0.1.0/gitwithtea_py/models/repo_collaborator_permission.py
--rw-r--r--   0        0        0     6571 2023-05-24 13:56:05.435940 gitwithtea_py-0.1.0/gitwithtea_py/models/repo_commit.py
--rw-r--r--   0        0        0     3453 2023-05-24 13:56:05.407940 gitwithtea_py-0.1.0/gitwithtea_py/models/repo_topic_options.py
--rw-r--r--   0        0        0     4716 2023-05-24 13:56:05.434940 gitwithtea_py-0.1.0/gitwithtea_py/models/repo_transfer.py
--rw-r--r--   0        0        0    40869 2023-05-24 13:56:05.467940 gitwithtea_py-0.1.0/gitwithtea_py/models/repository.py
--rw-r--r--   0        0        0     5128 2023-05-24 13:56:05.434940 gitwithtea_py-0.1.0/gitwithtea_py/models/repository_meta.py
--rw-r--r--   0        0        0     2713 2023-05-24 13:56:05.401940 gitwithtea_py-0.1.0/gitwithtea_py/models/review_state_type.py
--rw-r--r--   0        0        0     3867 2023-05-24 13:56:05.417940 gitwithtea_py-0.1.0/gitwithtea_py/models/search_results.py
--rw-r--r--   0        0        0     3344 2023-05-24 13:56:05.434940 gitwithtea_py-0.1.0/gitwithtea_py/models/server_version.py
--rw-r--r--   0        0        0     2683 2023-05-24 13:56:05.467940 gitwithtea_py-0.1.0/gitwithtea_py/models/state_type.py
--rw-r--r--   0        0        0     7453 2023-05-24 13:56:05.519940 gitwithtea_py-0.1.0/gitwithtea_py/models/stop_watch.py
--rw-r--r--   0        0        0     4051 2023-05-24 13:56:05.435940 gitwithtea_py-0.1.0/gitwithtea_py/models/submit_pull_review_options.py
--rw-r--r--   0        0        0     6260 2023-05-24 13:56:05.407940 gitwithtea_py-0.1.0/gitwithtea_py/models/tag.py
--rw-r--r--   0        0        0     9245 2023-05-24 13:56:05.519940 gitwithtea_py-0.1.0/gitwithtea_py/models/team.py
--rw-r--r--   0        0        0     2683 2023-05-24 13:56:05.434940 gitwithtea_py-0.1.0/gitwithtea_py/models/time_stamp.py
--rw-r--r--   0        0        0    23587 2023-05-24 13:56:05.467940 gitwithtea_py-0.1.0/gitwithtea_py/models/timeline_comment.py
--rw-r--r--   0        0        0     3306 2023-05-24 13:56:05.434940 gitwithtea_py-0.1.0/gitwithtea_py/models/topic_name.py
--rw-r--r--   0        0        0     5958 2023-05-24 13:56:05.434940 gitwithtea_py-0.1.0/gitwithtea_py/models/topic_response.py
--rw-r--r--   0        0        0     7353 2023-05-24 13:56:05.424940 gitwithtea_py-0.1.0/gitwithtea_py/models/tracked_time.py
--rw-r--r--   0        0        0     4695 2023-05-24 13:56:05.467940 gitwithtea_py-0.1.0/gitwithtea_py/models/transfer_repo_option.py
--rw-r--r--   0        0        0    10978 2023-05-24 13:56:05.467940 gitwithtea_py-0.1.0/gitwithtea_py/models/update_file_options.py
--rw-r--r--   0        0        0    17141 2023-05-24 13:56:05.435940 gitwithtea_py-0.1.0/gitwithtea_py/models/user.py
--rw-r--r--   0        0        0     4189 2023-05-24 13:56:05.519940 gitwithtea_py-0.1.0/gitwithtea_py/models/user_heatmap_data.py
--rw-r--r--   0        0        0     8957 2023-05-24 13:56:05.435940 gitwithtea_py-0.1.0/gitwithtea_py/models/user_settings.py
--rw-r--r--   0        0        0     9244 2023-05-24 13:56:05.434940 gitwithtea_py-0.1.0/gitwithtea_py/models/user_settings_options.py
--rw-r--r--   0        0        0     6623 2023-05-24 13:56:05.467940 gitwithtea_py-0.1.0/gitwithtea_py/models/watch_info.py
--rw-r--r--   0        0        0     5166 2023-05-24 13:56:05.519940 gitwithtea_py-0.1.0/gitwithtea_py/models/wiki_commit.py
--rw-r--r--   0        0        0     3997 2023-05-24 13:56:05.434940 gitwithtea_py-0.1.0/gitwithtea_py/models/wiki_commit_list.py
--rw-r--r--   0        0        0     8049 2023-05-24 13:56:05.435940 gitwithtea_py-0.1.0/gitwithtea_py/models/wiki_page.py
--rw-r--r--   0        0        0     5411 2023-05-24 13:56:05.434940 gitwithtea_py-0.1.0/gitwithtea_py/models/wiki_page_meta_data.py
--rw-r--r--   0        0        0    13161 2023-05-24 10:44:24.000000 gitwithtea_py-0.1.0/gitwithtea_py/rest.py
--rw-r--r--   0        0        0     1361 2023-05-24 13:56:31.538058 gitwithtea_py-0.1.0/pyproject.toml
--rw-r--r--   0        0        0    65410 1970-01-01 00:00:00.000000 gitwithtea_py-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0    64033 2023-05-24 13:56:05.378940 gitwithtea_py-0.1.1/README.md
+-rw-r--r--   0        0        0    11991 2023-05-24 13:56:05.401940 gitwithtea_py-0.1.1/gitwithtea_py/__init__.py
+-rw-r--r--   0        0        0      651 2023-05-24 13:56:05.817942 gitwithtea_py-0.1.1/gitwithtea_py/api/__init__.py
+-rw-r--r--   0        0        0     8720 2023-05-24 13:56:05.555941 gitwithtea_py-0.1.1/gitwithtea_py/api/activitypub_api.py
+-rw-r--r--   0        0        0    77872 2023-05-24 13:56:05.519940 gitwithtea_py-0.1.1/gitwithtea_py/api/admin_api.py
+-rw-r--r--   0        0        0   322896 2023-05-24 13:56:05.555941 gitwithtea_py-0.1.1/gitwithtea_py/api/issue_api.py
+-rw-r--r--   0        0        0    17886 2023-05-24 13:56:05.817942 gitwithtea_py-0.1.1/gitwithtea_py/api/miscellaneous_api.py
+-rw-r--r--   0        0        0    35978 2023-05-24 13:56:05.520941 gitwithtea_py-0.1.1/gitwithtea_py/api/notification_api.py
+-rw-r--r--   0        0        0   184878 2023-05-24 13:56:05.817942 gitwithtea_py-0.1.1/gitwithtea_py/api/organization_api.py
+-rw-r--r--   0        0        0    22639 2023-05-24 13:56:05.519940 gitwithtea_py-0.1.1/gitwithtea_py/api/package_api.py
+-rw-r--r--   0        0        0   703704 2023-05-24 13:56:06.572945 gitwithtea_py-0.1.1/gitwithtea_py/api/repository_api.py
+-rw-r--r--   0        0        0    14488 2023-05-24 13:56:05.519940 gitwithtea_py-0.1.1/gitwithtea_py/api/settings_api.py
+-rw-r--r--   0        0        0   200637 2023-05-24 13:56:05.520941 gitwithtea_py-0.1.1/gitwithtea_py/api/user_api.py
+-rw-r--r--   0        0        0    25058 2023-05-24 13:56:05.401940 gitwithtea_py-0.1.1/gitwithtea_py/api_client.py
+-rw-r--r--   0        0        0     9652 2023-05-24 13:56:05.401940 gitwithtea_py-0.1.1/gitwithtea_py/configuration.py
+-rw-r--r--   0        0        0    11255 2023-05-24 14:10:54.472345 gitwithtea_py-0.1.1/gitwithtea_py/models/__init__.py
+-rw-r--r--   0        0        0     5816 2023-05-24 13:56:05.519940 gitwithtea_py-0.1.1/gitwithtea_py/models/access_token.py
+-rw-r--r--   0        0        0     3327 2023-05-24 13:56:05.434940 gitwithtea_py-0.1.1/gitwithtea_py/models/activity_pub.py
+-rw-r--r--   0        0        0     3476 2023-05-24 13:56:05.519940 gitwithtea_py-0.1.1/gitwithtea_py/models/add_collaborator_option.py
+-rw-r--r--   0        0        0     4941 2023-05-24 13:56:05.519940 gitwithtea_py-0.1.1/gitwithtea_py/models/add_time_option.py
+-rw-r--r--   0        0        0     7109 2023-05-24 13:56:05.519940 gitwithtea_py-0.1.1/gitwithtea_py/models/annotated_tag.py
+-rw-r--r--   0        0        0     4491 2023-05-24 13:56:05.434940 gitwithtea_py-0.1.1/gitwithtea_py/models/annotated_tag_object.py
+-rw-r--r--   0        0        0     3840 2023-05-24 13:56:05.415940 gitwithtea_py-0.1.1/gitwithtea_py/models/api_error.py
+-rw-r--r--   0        0        0     7286 2023-05-24 13:56:05.519940 gitwithtea_py-0.1.1/gitwithtea_py/models/attachment.py
+-rw-r--r--   0        0        0     9705 2023-05-24 13:56:05.519940 gitwithtea_py-0.1.1/gitwithtea_py/models/branch.py
+-rw-r--r--   0        0        0    26670 2023-05-24 13:56:05.467940 gitwithtea_py-0.1.1/gitwithtea_py/models/branch_protection.py
+-rw-r--r--   0        0        0     8790 2023-05-24 13:56:05.519940 gitwithtea_py-0.1.1/gitwithtea_py/models/changed_file.py
+-rw-r--r--   0        0        0     7351 2023-05-24 13:56:05.434940 gitwithtea_py-0.1.1/gitwithtea_py/models/combined_status.py
+-rw-r--r--   0        0        0    10032 2023-05-24 13:56:05.434940 gitwithtea_py-0.1.1/gitwithtea_py/models/comment.py
+-rw-r--r--   0        0        0     8749 2023-05-24 13:56:05.415940 gitwithtea_py-0.1.1/gitwithtea_py/models/commit.py
+-rw-r--r--   0        0        0     3418 2023-05-24 13:56:05.467940 gitwithtea_py-0.1.1/gitwithtea_py/models/commit_affected_files.py
+-rw-r--r--   0        0        0     4087 2023-05-24 13:56:05.519940 gitwithtea_py-0.1.1/gitwithtea_py/models/commit_date_options.py
+-rw-r--r--   0        0        0     4430 2023-05-24 13:56:05.467940 gitwithtea_py-0.1.1/gitwithtea_py/models/commit_meta.py
+-rw-r--r--   0        0        0     4632 2023-05-24 13:56:05.434940 gitwithtea_py-0.1.1/gitwithtea_py/models/commit_stats.py
+-rw-r--r--   0        0        0     8566 2023-05-24 13:56:05.401940 gitwithtea_py-0.1.1/gitwithtea_py/models/commit_status.py
+-rw-r--r--   0        0        0     2723 2023-05-24 13:56:05.434940 gitwithtea_py-0.1.1/gitwithtea_py/models/commit_status_state.py
+-rw-r--r--   0        0        0     4434 2023-05-24 13:56:05.434940 gitwithtea_py-0.1.1/gitwithtea_py/models/commit_user.py
+-rw-r--r--   0        0        0    13452 2023-05-24 13:56:05.434940 gitwithtea_py-0.1.1/gitwithtea_py/models/contents_response.py
+-rw-r--r--   0        0        0     4183 2023-05-24 13:56:05.467940 gitwithtea_py-0.1.1/gitwithtea_py/models/create_access_token_option.py
+-rw-r--r--   0        0        0    26378 2023-05-24 13:56:05.434940 gitwithtea_py-0.1.1/gitwithtea_py/models/create_branch_protection_option.py
+-rw-r--r--   0        0        0     4785 2023-05-24 13:56:05.434940 gitwithtea_py-0.1.1/gitwithtea_py/models/create_branch_repo_option.py
+-rw-r--r--   0        0        0     3468 2023-05-24 13:56:05.434940 gitwithtea_py-0.1.1/gitwithtea_py/models/create_email_option.py
+-rw-r--r--   0        0        0     9181 2023-05-24 13:56:05.434940 gitwithtea_py-0.1.1/gitwithtea_py/models/create_file_options.py
+-rw-r--r--   0        0        0     4314 2023-05-24 13:56:05.434940 gitwithtea_py-0.1.1/gitwithtea_py/models/create_fork_option.py
+-rw-r--r--   0        0        0     4710 2023-05-24 13:56:05.519940 gitwithtea_py-0.1.1/gitwithtea_py/models/create_gpg_key_option.py
+-rw-r--r--   0        0        0     7686 2023-05-24 13:56:05.434940 gitwithtea_py-0.1.1/gitwithtea_py/models/create_hook_option.py
+-rw-r--r--   0        0        0     2748 2023-05-24 13:56:05.519940 gitwithtea_py-0.1.1/gitwithtea_py/models/create_hook_option_config.py
+-rw-r--r--   0        0        0     3513 2023-05-24 13:56:05.435940 gitwithtea_py-0.1.1/gitwithtea_py/models/create_issue_comment_option.py
+-rw-r--r--   0        0        0     8937 2023-05-24 13:56:05.434940 gitwithtea_py-0.1.1/gitwithtea_py/models/create_issue_option.py
+-rw-r--r--   0        0        0     5185 2023-05-24 13:56:05.434940 gitwithtea_py-0.1.1/gitwithtea_py/models/create_key_option.py
+-rw-r--r--   0        0        0     5635 2023-05-24 13:56:05.519940 gitwithtea_py-0.1.1/gitwithtea_py/models/create_label_option.py
+-rw-r--r--   0        0        0     5768 2023-05-24 13:56:05.434940 gitwithtea_py-0.1.1/gitwithtea_py/models/create_milestone_option.py
+-rw-r--r--   0        0        0     5236 2023-05-24 13:56:05.434940 gitwithtea_py-0.1.1/gitwithtea_py/models/create_o_auth2_application_options.py
+-rw-r--r--   0        0        0     8730 2023-05-24 13:56:05.467940 gitwithtea_py-0.1.1/gitwithtea_py/models/create_org_option.py
+-rw-r--r--   0        0        0     8813 2023-05-24 13:56:05.434940 gitwithtea_py-0.1.1/gitwithtea_py/models/create_pull_request_option.py
+-rw-r--r--   0        0        0     5849 2023-05-24 13:56:05.519940 gitwithtea_py-0.1.1/gitwithtea_py/models/create_pull_review_comment.py
+-rw-r--r--   0        0        0     5551 2023-05-24 13:56:05.407940 gitwithtea_py-0.1.1/gitwithtea_py/models/create_pull_review_options.py
+-rw-r--r--   0        0        0     6756 2023-05-24 13:56:05.415940 gitwithtea_py-0.1.1/gitwithtea_py/models/create_push_mirror_option.py
+-rw-r--r--   0        0        0     6963 2023-05-24 13:56:05.519940 gitwithtea_py-0.1.1/gitwithtea_py/models/create_release_option.py
+-rw-r--r--   0        0        0    12125 2023-05-24 13:56:05.467940 gitwithtea_py-0.1.1/gitwithtea_py/models/create_repo_option.py
+-rw-r--r--   0        0        0     5514 2023-05-24 13:56:05.519940 gitwithtea_py-0.1.1/gitwithtea_py/models/create_status_option.py
+-rw-r--r--   0        0        0     4794 2023-05-24 13:56:05.401940 gitwithtea_py-0.1.1/gitwithtea_py/models/create_tag_option.py
+-rw-r--r--   0        0        0     8517 2023-05-24 13:56:05.407940 gitwithtea_py-0.1.1/gitwithtea_py/models/create_team_option.py
+-rw-r--r--   0        0        0    11370 2023-05-24 13:56:05.434940 gitwithtea_py-0.1.1/gitwithtea_py/models/create_user_option.py
+-rw-r--r--   0        0        0     5234 2023-05-24 13:56:05.401940 gitwithtea_py-0.1.1/gitwithtea_py/models/create_wiki_page_options.py
+-rw-r--r--   0        0        0     5613 2023-05-24 13:56:05.467940 gitwithtea_py-0.1.1/gitwithtea_py/models/cron.py
+-rw-r--r--   0        0        0     3474 2023-05-24 13:56:05.434940 gitwithtea_py-0.1.1/gitwithtea_py/models/delete_email_option.py
+-rw-r--r--   0        0        0     9131 2023-05-24 13:56:05.519940 gitwithtea_py-0.1.1/gitwithtea_py/models/delete_file_options.py
+-rw-r--r--   0        0        0     8267 2023-05-24 13:56:05.434940 gitwithtea_py-0.1.1/gitwithtea_py/models/deploy_key.py
+-rw-r--r--   0        0        0     4111 2023-05-24 13:56:05.519940 gitwithtea_py-0.1.1/gitwithtea_py/models/dismiss_pull_review_options.py
+-rw-r--r--   0        0        0     3356 2023-05-24 13:56:05.519940 gitwithtea_py-0.1.1/gitwithtea_py/models/edit_attachment_options.py
+-rw-r--r--   0        0        0    24600 2023-05-24 13:56:05.519940 gitwithtea_py-0.1.1/gitwithtea_py/models/edit_branch_protection_option.py
+-rw-r--r--   0        0        0     3558 2023-05-24 13:56:05.519940 gitwithtea_py-0.1.1/gitwithtea_py/models/edit_deadline_option.py
+-rw-r--r--   0        0        0     3380 2023-05-24 13:56:05.519940 gitwithtea_py-0.1.1/gitwithtea_py/models/edit_git_hook_option.py
+-rw-r--r--   0        0        0     6307 2023-05-24 13:56:05.415940 gitwithtea_py-0.1.1/gitwithtea_py/models/edit_hook_option.py
+-rw-r--r--   0        0        0     3495 2023-05-24 13:56:05.435940 gitwithtea_py-0.1.1/gitwithtea_py/models/edit_issue_comment_option.py
+-rw-r--r--   0        0        0     8696 2023-05-24 13:56:05.519940 gitwithtea_py-0.1.1/gitwithtea_py/models/edit_issue_option.py
+-rw-r--r--   0        0        0     5332 2023-05-24 13:56:05.467940 gitwithtea_py-0.1.1/gitwithtea_py/models/edit_label_option.py
+-rw-r--r--   0        0        0     5388 2023-05-24 13:56:05.435940 gitwithtea_py-0.1.1/gitwithtea_py/models/edit_milestone_option.py
+-rw-r--r--   0        0        0     7849 2023-05-24 13:56:05.519940 gitwithtea_py-0.1.1/gitwithtea_py/models/edit_org_option.py
+-rw-r--r--   0        0        0    10523 2023-05-24 13:56:05.434940 gitwithtea_py-0.1.1/gitwithtea_py/models/edit_pull_request_option.py
+-rw-r--r--   0        0        0     3389 2023-05-24 13:56:05.435940 gitwithtea_py-0.1.1/gitwithtea_py/models/edit_reaction_option.py
+-rw-r--r--   0        0        0     6771 2023-05-24 13:56:05.435940 gitwithtea_py-0.1.1/gitwithtea_py/models/edit_release_option.py
+-rw-r--r--   0        0        0    29858 2023-05-24 13:56:05.434940 gitwithtea_py-0.1.1/gitwithtea_py/models/edit_repo_option.py
+-rw-r--r--   0        0        0     8451 2023-05-24 13:56:05.467940 gitwithtea_py-0.1.1/gitwithtea_py/models/edit_team_option.py
+-rw-r--r--   0        0        0    16213 2023-05-24 13:56:05.519940 gitwithtea_py-0.1.1/gitwithtea_py/models/edit_user_option.py
+-rw-r--r--   0        0        0     4476 2023-05-24 13:56:05.434940 gitwithtea_py-0.1.1/gitwithtea_py/models/email.py
+-rw-r--r--   0        0        0     7439 2023-05-24 13:56:05.467940 gitwithtea_py-0.1.1/gitwithtea_py/models/external_tracker.py
+-rw-r--r--   0        0        0     3623 2023-05-24 13:56:05.435940 gitwithtea_py-0.1.1/gitwithtea_py/models/external_wiki.py
+-rw-r--r--   0        0        0     8614 2023-05-24 13:56:05.519940 gitwithtea_py-0.1.1/gitwithtea_py/models/file_commit_response.py
+-rw-r--r--   0        0        0     4911 2023-05-24 13:56:05.434940 gitwithtea_py-0.1.1/gitwithtea_py/models/file_delete_response.py
+-rw-r--r--   0        0        0     4513 2023-05-24 13:56:05.434940 gitwithtea_py-0.1.1/gitwithtea_py/models/file_links_response.py
+-rw-r--r--   0        0        0     4839 2023-05-24 13:56:05.519940 gitwithtea_py-0.1.1/gitwithtea_py/models/file_response.py
+-rw-r--r--   0        0        0     6472 2023-05-24 13:56:05.434940 gitwithtea_py-0.1.1/gitwithtea_py/models/general_api_settings.py
+-rw-r--r--   0        0        0     5702 2023-05-24 13:56:05.467940 gitwithtea_py-0.1.1/gitwithtea_py/models/general_attachment_settings.py
+-rw-r--r--   0        0        0     7901 2023-05-24 13:56:05.434940 gitwithtea_py-0.1.1/gitwithtea_py/models/general_repo_settings.py
+-rw-r--r--   0        0        0     5170 2023-05-24 13:56:05.519940 gitwithtea_py-0.1.1/gitwithtea_py/models/general_ui_settings.py
+-rw-r--r--   0        0        0    11819 2023-05-24 13:56:05.434940 gitwithtea_py-0.1.1/gitwithtea_py/models/generate_repo_option.py
+-rw-r--r--   0        0        0     5758 2023-05-24 13:56:05.434940 gitwithtea_py-0.1.1/gitwithtea_py/models/git_blob_response.py
+-rw-r--r--   0        0        0     6004 2023-05-24 13:56:05.434940 gitwithtea_py-0.1.1/gitwithtea_py/models/git_entry.py
+-rw-r--r--   0        0        0     4507 2023-05-24 13:56:05.467940 gitwithtea_py-0.1.1/gitwithtea_py/models/git_hook.py
+-rw-r--r--   0        0        0     4338 2023-05-24 13:56:05.434940 gitwithtea_py-0.1.1/gitwithtea_py/models/git_object.py
+-rw-r--r--   0        0        0     6483 2023-05-24 13:56:05.467940 gitwithtea_py-0.1.1/gitwithtea_py/models/git_tree_response.py
+-rw-r--r--   0        0        0    11491 2023-05-24 13:56:05.467940 gitwithtea_py-0.1.1/gitwithtea_py/models/gpg_key.py
+-rw-r--r--   0        0        0     3942 2023-05-24 13:56:05.519940 gitwithtea_py-0.1.1/gitwithtea_py/models/gpg_key_email.py
+-rw-r--r--   0        0        0     7742 2023-05-24 13:56:05.434940 gitwithtea_py-0.1.1/gitwithtea_py/models/hook.py
+-rw-r--r--   0        0        0     3820 2023-05-24 13:56:05.435940 gitwithtea_py-0.1.1/gitwithtea_py/models/identity.py
+-rw-r--r--   0        0        0     3901 2023-05-24 13:56:05.467940 gitwithtea_py-0.1.1/gitwithtea_py/models/inline_response200.py
+-rw-r--r--   0        0        0     3914 2023-05-24 13:56:05.401940 gitwithtea_py-0.1.1/gitwithtea_py/models/inline_response2001.py
+-rw-r--r--   0        0        0     6357 2023-05-24 13:56:05.434940 gitwithtea_py-0.1.1/gitwithtea_py/models/internal_tracker.py
+-rw-r--r--   0        0        0    17917 2023-05-24 13:56:05.519940 gitwithtea_py-0.1.1/gitwithtea_py/models/issue.py
+-rw-r--r--   0        0        0     3379 2023-05-24 13:56:05.467940 gitwithtea_py-0.1.1/gitwithtea_py/models/issue_deadline.py
+-rw-r--r--   0        0        0     5397 2023-05-24 13:56:05.519940 gitwithtea_py-0.1.1/gitwithtea_py/models/issue_form_field.py
+-rw-r--r--   0        0        0     2728 2023-05-24 13:56:05.434940 gitwithtea_py-0.1.1/gitwithtea_py/models/issue_form_field_type.py
+-rw-r--r--   0        0        0     3458 2023-05-24 13:56:05.415940 gitwithtea_py-0.1.1/gitwithtea_py/models/issue_labels_option.py
+-rw-r--r--   0        0        0     7670 2023-05-24 13:56:05.401940 gitwithtea_py-0.1.1/gitwithtea_py/models/issue_template.py
+-rw-r--r--   0        0        0     2733 2023-05-24 13:56:05.401940 gitwithtea_py-0.1.1/gitwithtea_py/models/issue_template_labels.py
+-rw-r--r--   0        0        0     6160 2023-05-24 13:56:05.434940 gitwithtea_py-0.1.1/gitwithtea_py/models/label.py
+-rw-r--r--   0        0        0     5521 2023-05-24 13:56:05.434940 gitwithtea_py-0.1.1/gitwithtea_py/models/markdown_option.py
+-rw-r--r--   0        0        0    10110 2023-05-24 13:56:05.434940 gitwithtea_py-0.1.1/gitwithtea_py/models/merge_pull_request_option.py
+-rw-r--r--   0        0        0    17639 2023-05-24 13:56:05.467940 gitwithtea_py-0.1.1/gitwithtea_py/models/migrate_repo_options.py
+-rw-r--r--   0        0        0     9251 2023-05-24 13:56:05.519940 gitwithtea_py-0.1.1/gitwithtea_py/models/milestone.py
+-rw-r--r--   0        0        0     7442 2023-05-24 13:56:05.519940 gitwithtea_py-0.1.1/gitwithtea_py/models/node_info.py
+-rw-r--r--   0        0        0     4080 2023-05-24 13:56:05.519940 gitwithtea_py-0.1.1/gitwithtea_py/models/node_info_services.py
+-rw-r--r--   0        0        0     5350 2023-05-24 13:56:05.519940 gitwithtea_py-0.1.1/gitwithtea_py/models/node_info_software.py
+-rw-r--r--   0        0        0     4849 2023-05-24 13:56:05.434940 gitwithtea_py-0.1.1/gitwithtea_py/models/node_info_usage.py
+-rw-r--r--   0        0        0     4929 2023-05-24 13:56:05.519940 gitwithtea_py-0.1.1/gitwithtea_py/models/node_info_usage_users.py
+-rw-r--r--   0        0        0     3857 2023-05-24 13:56:05.415940 gitwithtea_py-0.1.1/gitwithtea_py/models/note.py
+-rw-r--r--   0        0        0     3300 2023-05-24 13:56:05.434940 gitwithtea_py-0.1.1/gitwithtea_py/models/notification_count.py
+-rw-r--r--   0        0        0     7788 2023-05-24 13:56:05.407940 gitwithtea_py-0.1.1/gitwithtea_py/models/notification_subject.py
+-rw-r--r--   0        0        0     7345 2023-05-24 13:56:05.434940 gitwithtea_py-0.1.1/gitwithtea_py/models/notification_thread.py
+-rw-r--r--   0        0        0     2723 2023-05-24 13:56:05.415940 gitwithtea_py-0.1.1/gitwithtea_py/models/notify_subject_type.py
+-rw-r--r--   0        0        0     7718 2023-05-24 13:56:05.519940 gitwithtea_py-0.1.1/gitwithtea_py/models/o_auth2_application.py
+-rw-r--r--   0        0        0     9837 2023-05-24 13:56:05.435940 gitwithtea_py-0.1.1/gitwithtea_py/models/organization.py
+-rw-r--r--   0        0        0     6553 2023-05-24 13:56:05.434940 gitwithtea_py-0.1.1/gitwithtea_py/models/organization_permissions.py
+-rw-r--r--   0        0        0     7511 2023-05-24 13:56:05.519940 gitwithtea_py-0.1.1/gitwithtea_py/models/package.py
+-rw-r--r--   0        0        0     6724 2023-05-24 13:56:05.434940 gitwithtea_py-0.1.1/gitwithtea_py/models/package_file.py
+-rw-r--r--   0        0        0     9348 2023-05-24 13:56:05.519940 gitwithtea_py-0.1.1/gitwithtea_py/models/payload_commit.py
+-rw-r--r--   0        0        0     6255 2023-05-24 13:56:05.519940 gitwithtea_py-0.1.1/gitwithtea_py/models/payload_commit_verification.py
+-rw-r--r--   0        0        0     4618 2023-05-24 13:56:05.519940 gitwithtea_py-0.1.1/gitwithtea_py/models/payload_user.py
+-rw-r--r--   0        0        0     4424 2023-05-24 13:56:05.434940 gitwithtea_py-0.1.1/gitwithtea_py/models/permission.py
+-rw-r--r--   0        0        0     5644 2023-05-24 13:56:05.434940 gitwithtea_py-0.1.1/gitwithtea_py/models/pr_branch_info.py
+-rw-r--r--   0        0        0     8169 2023-05-24 13:56:05.434940 gitwithtea_py-0.1.1/gitwithtea_py/models/public_key.py
+-rw-r--r--   0        0        0    21781 2023-05-24 13:56:05.519940 gitwithtea_py-0.1.1/gitwithtea_py/models/pull_request.py
+-rw-r--r--   0        0        0     4049 2023-05-24 13:56:05.519940 gitwithtea_py-0.1.1/gitwithtea_py/models/pull_request_meta.py
+-rw-r--r--   0        0        0    11955 2023-05-24 13:56:05.519940 gitwithtea_py-0.1.1/gitwithtea_py/models/pull_review.py
+-rw-r--r--   0        0        0    13494 2023-05-24 13:56:05.519940 gitwithtea_py-0.1.1/gitwithtea_py/models/pull_review_comment.py
+-rw-r--r--   0        0        0     4484 2023-05-24 13:56:05.519940 gitwithtea_py-0.1.1/gitwithtea_py/models/pull_review_request_options.py
+-rw-r--r--   0        0        0     8283 2023-05-24 13:56:05.467940 gitwithtea_py-0.1.1/gitwithtea_py/models/push_mirror.py
+-rw-r--r--   0        0        0     4559 2023-05-24 13:56:05.434940 gitwithtea_py-0.1.1/gitwithtea_py/models/reaction.py
+-rw-r--r--   0        0        0     4396 2023-05-24 13:56:05.415940 gitwithtea_py-0.1.1/gitwithtea_py/models/reference.py
+-rw-r--r--   0        0        0    12226 2023-05-24 13:56:05.519940 gitwithtea_py-0.1.1/gitwithtea_py/models/release.py
+-rw-r--r--   0        0        0     4890 2023-05-24 13:56:05.519940 gitwithtea_py-0.1.1/gitwithtea_py/models/repo_collaborator_permission.py
+-rw-r--r--   0        0        0     6571 2023-05-24 13:56:05.435940 gitwithtea_py-0.1.1/gitwithtea_py/models/repo_commit.py
+-rw-r--r--   0        0        0     3453 2023-05-24 13:56:05.407940 gitwithtea_py-0.1.1/gitwithtea_py/models/repo_topic_options.py
+-rw-r--r--   0        0        0     4716 2023-05-24 13:56:05.434940 gitwithtea_py-0.1.1/gitwithtea_py/models/repo_transfer.py
+-rw-r--r--   0        0        0    40869 2023-05-24 13:56:05.467940 gitwithtea_py-0.1.1/gitwithtea_py/models/repository.py
+-rw-r--r--   0        0        0     5128 2023-05-24 13:56:05.434940 gitwithtea_py-0.1.1/gitwithtea_py/models/repository_meta.py
+-rw-r--r--   0        0        0     2713 2023-05-24 13:56:05.401940 gitwithtea_py-0.1.1/gitwithtea_py/models/review_state_type.py
+-rw-r--r--   0        0        0     3867 2023-05-24 13:56:05.417940 gitwithtea_py-0.1.1/gitwithtea_py/models/search_results.py
+-rw-r--r--   0        0        0     3344 2023-05-24 13:56:05.434940 gitwithtea_py-0.1.1/gitwithtea_py/models/server_version.py
+-rw-r--r--   0        0        0     2683 2023-05-24 13:56:05.467940 gitwithtea_py-0.1.1/gitwithtea_py/models/state_type.py
+-rw-r--r--   0        0        0     7453 2023-05-24 13:56:05.519940 gitwithtea_py-0.1.1/gitwithtea_py/models/stop_watch.py
+-rw-r--r--   0        0        0     4051 2023-05-24 13:56:05.435940 gitwithtea_py-0.1.1/gitwithtea_py/models/submit_pull_review_options.py
+-rw-r--r--   0        0        0     6260 2023-05-24 13:56:05.407940 gitwithtea_py-0.1.1/gitwithtea_py/models/tag.py
+-rw-r--r--   0        0        0     9245 2023-05-24 13:56:05.519940 gitwithtea_py-0.1.1/gitwithtea_py/models/team.py
+-rw-r--r--   0        0        0     2683 2023-05-24 13:56:05.434940 gitwithtea_py-0.1.1/gitwithtea_py/models/time_stamp.py
+-rw-r--r--   0        0        0    23587 2023-05-24 13:56:05.467940 gitwithtea_py-0.1.1/gitwithtea_py/models/timeline_comment.py
+-rw-r--r--   0        0        0     3306 2023-05-24 13:56:05.434940 gitwithtea_py-0.1.1/gitwithtea_py/models/topic_name.py
+-rw-r--r--   0        0        0     5958 2023-05-24 13:56:05.434940 gitwithtea_py-0.1.1/gitwithtea_py/models/topic_response.py
+-rw-r--r--   0        0        0     7353 2023-05-24 13:56:05.424940 gitwithtea_py-0.1.1/gitwithtea_py/models/tracked_time.py
+-rw-r--r--   0        0        0     4695 2023-05-24 13:56:05.467940 gitwithtea_py-0.1.1/gitwithtea_py/models/transfer_repo_option.py
+-rw-r--r--   0        0        0    10978 2023-05-24 13:56:05.467940 gitwithtea_py-0.1.1/gitwithtea_py/models/update_file_options.py
+-rw-r--r--   0        0        0    17141 2023-05-24 13:56:05.435940 gitwithtea_py-0.1.1/gitwithtea_py/models/user.py
+-rw-r--r--   0        0        0     4189 2023-05-24 13:56:05.519940 gitwithtea_py-0.1.1/gitwithtea_py/models/user_heatmap_data.py
+-rw-r--r--   0        0        0     8957 2023-05-24 13:56:05.435940 gitwithtea_py-0.1.1/gitwithtea_py/models/user_settings.py
+-rw-r--r--   0        0        0     9244 2023-05-24 13:56:05.434940 gitwithtea_py-0.1.1/gitwithtea_py/models/user_settings_options.py
+-rw-r--r--   0        0        0     6623 2023-05-24 13:56:05.467940 gitwithtea_py-0.1.1/gitwithtea_py/models/watch_info.py
+-rw-r--r--   0        0        0     5166 2023-05-24 13:56:05.519940 gitwithtea_py-0.1.1/gitwithtea_py/models/wiki_commit.py
+-rw-r--r--   0        0        0     3997 2023-05-24 13:56:05.434940 gitwithtea_py-0.1.1/gitwithtea_py/models/wiki_commit_list.py
+-rw-r--r--   0        0        0     8049 2023-05-24 13:56:05.435940 gitwithtea_py-0.1.1/gitwithtea_py/models/wiki_page.py
+-rw-r--r--   0        0        0     5411 2023-05-24 13:56:05.434940 gitwithtea_py-0.1.1/gitwithtea_py/models/wiki_page_meta_data.py
+-rw-r--r--   0        0        0    13161 2023-05-24 10:44:24.000000 gitwithtea_py-0.1.1/gitwithtea_py/rest.py
+-rw-r--r--   0        0        0     1359 2023-05-24 14:11:10.065398 gitwithtea_py-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0    65403 1970-01-01 00:00:00.000000 gitwithtea_py-0.1.1/PKG-INFO
```

### Comparing `gitwithtea_py-0.1.0/README.md` & `gitwithtea_py-0.1.1/README.md`

 * *Files identical despite different names*

### Comparing `gitwithtea_py-0.1.0/gitwithtea_py/__init__.py` & `gitwithtea_py-0.1.1/gitwithtea_py/__init__.py`

 * *Files identical despite different names*

### Comparing `gitwithtea_py-0.1.0/gitwithtea_py/api/__init__.py` & `gitwithtea_py-0.1.1/gitwithtea_py/api/__init__.py`

 * *Files identical despite different names*

### Comparing `gitwithtea_py-0.1.0/gitwithtea_py/api/activitypub_api.py` & `gitwithtea_py-0.1.1/gitwithtea_py/api/activitypub_api.py`

 * *Files identical despite different names*

### Comparing `gitwithtea_py-0.1.0/gitwithtea_py/api/admin_api.py` & `gitwithtea_py-0.1.1/gitwithtea_py/api/admin_api.py`

 * *Files identical despite different names*

### Comparing `gitwithtea_py-0.1.0/gitwithtea_py/api/issue_api.py` & `gitwithtea_py-0.1.1/gitwithtea_py/api/issue_api.py`

 * *Files identical despite different names*

### Comparing `gitwithtea_py-0.1.0/gitwithtea_py/api/miscellaneous_api.py` & `gitwithtea_py-0.1.1/gitwithtea_py/api/miscellaneous_api.py`

 * *Files identical despite different names*

### Comparing `gitwithtea_py-0.1.0/gitwithtea_py/api/notification_api.py` & `gitwithtea_py-0.1.1/gitwithtea_py/api/notification_api.py`

 * *Files identical despite different names*

### Comparing `gitwithtea_py-0.1.0/gitwithtea_py/api/organization_api.py` & `gitwithtea_py-0.1.1/gitwithtea_py/api/organization_api.py`

 * *Files identical despite different names*

### Comparing `gitwithtea_py-0.1.0/gitwithtea_py/api/package_api.py` & `gitwithtea_py-0.1.1/gitwithtea_py/api/package_api.py`

 * *Files identical despite different names*

### Comparing `gitwithtea_py-0.1.0/gitwithtea_py/api/repository_api.py` & `gitwithtea_py-0.1.1/gitwithtea_py/api/repository_api.py`

 * *Files identical despite different names*

### Comparing `gitwithtea_py-0.1.0/gitwithtea_py/api/settings_api.py` & `gitwithtea_py-0.1.1/gitwithtea_py/api/settings_api.py`

 * *Files identical despite different names*

### Comparing `gitwithtea_py-0.1.0/gitwithtea_py/api/user_api.py` & `gitwithtea_py-0.1.1/gitwithtea_py/api/user_api.py`

 * *Files identical despite different names*

### Comparing `gitwithtea_py-0.1.0/gitwithtea_py/api_client.py` & `gitwithtea_py-0.1.1/gitwithtea_py/api_client.py`

 * *Files identical despite different names*

### Comparing `gitwithtea_py-0.1.0/gitwithtea_py/configuration.py` & `gitwithtea_py-0.1.1/gitwithtea_py/configuration.py`

 * *Files identical despite different names*

### Comparing `gitwithtea_py-0.1.0/gitwithtea_py/models/__init__.py` & `gitwithtea_py-0.1.1/gitwithtea_py/models/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -57,15 +57,15 @@
 from gitwithtea_py.models.create_pull_review_comment import CreatePullReviewComment
 from gitwithtea_py.models.create_pull_review_options import CreatePullReviewOptions
 from gitwithtea_py.models.create_push_mirror_option import CreatePushMirrorOption
 from gitwithtea_py.models.create_release_option import CreateReleaseOption
 from gitwithtea_py.models.create_repo_option import CreateRepoOption
 from gitwithtea_py.models.create_status_option import CreateStatusOption
 from gitwithtea_py.models.create_tag_option import CreateTagOption
-from gitwithtea_py.models.create_gitwithteam_option import CreateTeamOption
+from gitwithtea_py.models.create_team_option import CreateTeamOption
 from gitwithtea_py.models.create_user_option import CreateUserOption
 from gitwithtea_py.models.create_wiki_page_options import CreateWikiPageOptions
 from gitwithtea_py.models.cron import Cron
 from gitwithtea_py.models.delete_email_option import DeleteEmailOption
 from gitwithtea_py.models.delete_file_options import DeleteFileOptions
 from gitwithtea_py.models.deploy_key import DeployKey
 from gitwithtea_py.models.dismiss_pull_review_options import DismissPullReviewOptions
@@ -79,15 +79,15 @@
 from gitwithtea_py.models.edit_label_option import EditLabelOption
 from gitwithtea_py.models.edit_milestone_option import EditMilestoneOption
 from gitwithtea_py.models.edit_org_option import EditOrgOption
 from gitwithtea_py.models.edit_pull_request_option import EditPullRequestOption
 from gitwithtea_py.models.edit_reaction_option import EditReactionOption
 from gitwithtea_py.models.edit_release_option import EditReleaseOption
 from gitwithtea_py.models.edit_repo_option import EditRepoOption
-from gitwithtea_py.models.edit_gitwithteam_option import EditTeamOption
+from gitwithtea_py.models.edit_team_option import EditTeamOption
 from gitwithtea_py.models.edit_user_option import EditUserOption
 from gitwithtea_py.models.email import Email
 from gitwithtea_py.models.external_tracker import ExternalTracker
 from gitwithtea_py.models.external_wiki import ExternalWiki
 from gitwithtea_py.models.file_commit_response import FileCommitResponse
 from gitwithtea_py.models.file_delete_response import FileDeleteResponse
 from gitwithtea_py.models.file_links_response import FileLinksResponse
@@ -160,15 +160,15 @@
 from gitwithtea_py.models.review_state_type import ReviewStateType
 from gitwithtea_py.models.search_results import SearchResults
 from gitwithtea_py.models.server_version import ServerVersion
 from gitwithtea_py.models.state_type import StateType
 from gitwithtea_py.models.stop_watch import StopWatch
 from gitwithtea_py.models.submit_pull_review_options import SubmitPullReviewOptions
 from gitwithtea_py.models.tag import Tag
-from gitwithtea_py.models.gitwithteam import Team
+from gitwithtea_py.models.team import Team
 from gitwithtea_py.models.time_stamp import TimeStamp
 from gitwithtea_py.models.timeline_comment import TimelineComment
 from gitwithtea_py.models.topic_name import TopicName
 from gitwithtea_py.models.topic_response import TopicResponse
 from gitwithtea_py.models.tracked_time import TrackedTime
 from gitwithtea_py.models.transfer_repo_option import TransferRepoOption
 from gitwithtea_py.models.update_file_options import UpdateFileOptions
```

### Comparing `gitwithtea_py-0.1.0/gitwithtea_py/models/access_token.py` & `gitwithtea_py-0.1.1/gitwithtea_py/models/access_token.py`

 * *Files identical despite different names*

### Comparing `gitwithtea_py-0.1.0/gitwithtea_py/models/activity_pub.py` & `gitwithtea_py-0.1.1/gitwithtea_py/models/activity_pub.py`

 * *Files identical despite different names*

### Comparing `gitwithtea_py-0.1.0/gitwithtea_py/models/add_collaborator_option.py` & `gitwithtea_py-0.1.1/gitwithtea_py/models/add_collaborator_option.py`

 * *Files identical despite different names*

### Comparing `gitwithtea_py-0.1.0/gitwithtea_py/models/add_time_option.py` & `gitwithtea_py-0.1.1/gitwithtea_py/models/add_time_option.py`

 * *Files identical despite different names*

### Comparing `gitwithtea_py-0.1.0/gitwithtea_py/models/annotated_tag.py` & `gitwithtea_py-0.1.1/gitwithtea_py/models/annotated_tag.py`

 * *Files identical despite different names*

### Comparing `gitwithtea_py-0.1.0/gitwithtea_py/models/annotated_tag_object.py` & `gitwithtea_py-0.1.1/gitwithtea_py/models/annotated_tag_object.py`

 * *Files identical despite different names*

### Comparing `gitwithtea_py-0.1.0/gitwithtea_py/models/api_error.py` & `gitwithtea_py-0.1.1/gitwithtea_py/models/api_error.py`

 * *Files identical despite different names*

### Comparing `gitwithtea_py-0.1.0/gitwithtea_py/models/attachment.py` & `gitwithtea_py-0.1.1/gitwithtea_py/models/attachment.py`

 * *Files identical despite different names*

### Comparing `gitwithtea_py-0.1.0/gitwithtea_py/models/branch.py` & `gitwithtea_py-0.1.1/gitwithtea_py/models/branch.py`

 * *Files identical despite different names*

### Comparing `gitwithtea_py-0.1.0/gitwithtea_py/models/branch_protection.py` & `gitwithtea_py-0.1.1/gitwithtea_py/models/branch_protection.py`

 * *Files identical despite different names*

### Comparing `gitwithtea_py-0.1.0/gitwithtea_py/models/changed_file.py` & `gitwithtea_py-0.1.1/gitwithtea_py/models/changed_file.py`

 * *Files identical despite different names*

### Comparing `gitwithtea_py-0.1.0/gitwithtea_py/models/combined_status.py` & `gitwithtea_py-0.1.1/gitwithtea_py/models/combined_status.py`

 * *Files identical despite different names*

### Comparing `gitwithtea_py-0.1.0/gitwithtea_py/models/comment.py` & `gitwithtea_py-0.1.1/gitwithtea_py/models/comment.py`

 * *Files identical despite different names*

### Comparing `gitwithtea_py-0.1.0/gitwithtea_py/models/commit.py` & `gitwithtea_py-0.1.1/gitwithtea_py/models/commit.py`

 * *Files identical despite different names*

### Comparing `gitwithtea_py-0.1.0/gitwithtea_py/models/commit_affected_files.py` & `gitwithtea_py-0.1.1/gitwithtea_py/models/commit_affected_files.py`

 * *Files identical despite different names*

### Comparing `gitwithtea_py-0.1.0/gitwithtea_py/models/commit_date_options.py` & `gitwithtea_py-0.1.1/gitwithtea_py/models/commit_date_options.py`

 * *Files identical despite different names*

### Comparing `gitwithtea_py-0.1.0/gitwithtea_py/models/commit_meta.py` & `gitwithtea_py-0.1.1/gitwithtea_py/models/commit_meta.py`

 * *Files identical despite different names*

### Comparing `gitwithtea_py-0.1.0/gitwithtea_py/models/commit_stats.py` & `gitwithtea_py-0.1.1/gitwithtea_py/models/commit_stats.py`

 * *Files identical despite different names*

### Comparing `gitwithtea_py-0.1.0/gitwithtea_py/models/commit_status.py` & `gitwithtea_py-0.1.1/gitwithtea_py/models/commit_status.py`

 * *Files identical despite different names*

### Comparing `gitwithtea_py-0.1.0/gitwithtea_py/models/commit_status_state.py` & `gitwithtea_py-0.1.1/gitwithtea_py/models/commit_status_state.py`

 * *Files identical despite different names*

### Comparing `gitwithtea_py-0.1.0/gitwithtea_py/models/commit_user.py` & `gitwithtea_py-0.1.1/gitwithtea_py/models/commit_user.py`

 * *Files identical despite different names*

### Comparing `gitwithtea_py-0.1.0/gitwithtea_py/models/contents_response.py` & `gitwithtea_py-0.1.1/gitwithtea_py/models/contents_response.py`

 * *Files identical despite different names*

### Comparing `gitwithtea_py-0.1.0/gitwithtea_py/models/create_access_token_option.py` & `gitwithtea_py-0.1.1/gitwithtea_py/models/create_access_token_option.py`

 * *Files identical despite different names*

### Comparing `gitwithtea_py-0.1.0/gitwithtea_py/models/create_branch_protection_option.py` & `gitwithtea_py-0.1.1/gitwithtea_py/models/create_branch_protection_option.py`

 * *Files identical despite different names*

### Comparing `gitwithtea_py-0.1.0/gitwithtea_py/models/create_branch_repo_option.py` & `gitwithtea_py-0.1.1/gitwithtea_py/models/create_branch_repo_option.py`

 * *Files identical despite different names*

### Comparing `gitwithtea_py-0.1.0/gitwithtea_py/models/create_email_option.py` & `gitwithtea_py-0.1.1/gitwithtea_py/models/create_email_option.py`

 * *Files identical despite different names*

### Comparing `gitwithtea_py-0.1.0/gitwithtea_py/models/create_file_options.py` & `gitwithtea_py-0.1.1/gitwithtea_py/models/create_file_options.py`

 * *Files identical despite different names*

### Comparing `gitwithtea_py-0.1.0/gitwithtea_py/models/create_fork_option.py` & `gitwithtea_py-0.1.1/gitwithtea_py/models/create_fork_option.py`

 * *Files identical despite different names*

### Comparing `gitwithtea_py-0.1.0/gitwithtea_py/models/create_gpg_key_option.py` & `gitwithtea_py-0.1.1/gitwithtea_py/models/create_gpg_key_option.py`

 * *Files identical despite different names*

### Comparing `gitwithtea_py-0.1.0/gitwithtea_py/models/create_hook_option.py` & `gitwithtea_py-0.1.1/gitwithtea_py/models/create_hook_option.py`

 * *Files identical despite different names*

### Comparing `gitwithtea_py-0.1.0/gitwithtea_py/models/create_hook_option_config.py` & `gitwithtea_py-0.1.1/gitwithtea_py/models/create_hook_option_config.py`

 * *Files identical despite different names*

### Comparing `gitwithtea_py-0.1.0/gitwithtea_py/models/create_issue_comment_option.py` & `gitwithtea_py-0.1.1/gitwithtea_py/models/create_issue_comment_option.py`

 * *Files identical despite different names*

### Comparing `gitwithtea_py-0.1.0/gitwithtea_py/models/create_issue_option.py` & `gitwithtea_py-0.1.1/gitwithtea_py/models/create_issue_option.py`

 * *Files identical despite different names*

### Comparing `gitwithtea_py-0.1.0/gitwithtea_py/models/create_key_option.py` & `gitwithtea_py-0.1.1/gitwithtea_py/models/create_key_option.py`

 * *Files identical despite different names*

### Comparing `gitwithtea_py-0.1.0/gitwithtea_py/models/create_label_option.py` & `gitwithtea_py-0.1.1/gitwithtea_py/models/create_label_option.py`

 * *Files identical despite different names*

### Comparing `gitwithtea_py-0.1.0/gitwithtea_py/models/create_milestone_option.py` & `gitwithtea_py-0.1.1/gitwithtea_py/models/create_milestone_option.py`

 * *Files identical despite different names*

### Comparing `gitwithtea_py-0.1.0/gitwithtea_py/models/create_o_auth2_application_options.py` & `gitwithtea_py-0.1.1/gitwithtea_py/models/create_o_auth2_application_options.py`

 * *Files identical despite different names*

### Comparing `gitwithtea_py-0.1.0/gitwithtea_py/models/create_org_option.py` & `gitwithtea_py-0.1.1/gitwithtea_py/models/create_org_option.py`

 * *Files identical despite different names*

### Comparing `gitwithtea_py-0.1.0/gitwithtea_py/models/create_pull_request_option.py` & `gitwithtea_py-0.1.1/gitwithtea_py/models/create_pull_request_option.py`

 * *Files identical despite different names*

### Comparing `gitwithtea_py-0.1.0/gitwithtea_py/models/create_pull_review_comment.py` & `gitwithtea_py-0.1.1/gitwithtea_py/models/create_pull_review_comment.py`

 * *Files identical despite different names*

### Comparing `gitwithtea_py-0.1.0/gitwithtea_py/models/create_pull_review_options.py` & `gitwithtea_py-0.1.1/gitwithtea_py/models/create_pull_review_options.py`

 * *Files identical despite different names*

### Comparing `gitwithtea_py-0.1.0/gitwithtea_py/models/create_push_mirror_option.py` & `gitwithtea_py-0.1.1/gitwithtea_py/models/create_push_mirror_option.py`

 * *Files identical despite different names*

### Comparing `gitwithtea_py-0.1.0/gitwithtea_py/models/create_release_option.py` & `gitwithtea_py-0.1.1/gitwithtea_py/models/create_release_option.py`

 * *Files identical despite different names*

### Comparing `gitwithtea_py-0.1.0/gitwithtea_py/models/create_repo_option.py` & `gitwithtea_py-0.1.1/gitwithtea_py/models/create_repo_option.py`

 * *Files identical despite different names*

### Comparing `gitwithtea_py-0.1.0/gitwithtea_py/models/create_status_option.py` & `gitwithtea_py-0.1.1/gitwithtea_py/models/create_status_option.py`

 * *Files identical despite different names*

### Comparing `gitwithtea_py-0.1.0/gitwithtea_py/models/create_tag_option.py` & `gitwithtea_py-0.1.1/gitwithtea_py/models/create_tag_option.py`

 * *Files identical despite different names*

### Comparing `gitwithtea_py-0.1.0/gitwithtea_py/models/create_team_option.py` & `gitwithtea_py-0.1.1/gitwithtea_py/models/create_team_option.py`

 * *Files identical despite different names*

### Comparing `gitwithtea_py-0.1.0/gitwithtea_py/models/create_user_option.py` & `gitwithtea_py-0.1.1/gitwithtea_py/models/create_user_option.py`

 * *Files identical despite different names*

### Comparing `gitwithtea_py-0.1.0/gitwithtea_py/models/create_wiki_page_options.py` & `gitwithtea_py-0.1.1/gitwithtea_py/models/create_wiki_page_options.py`

 * *Files identical despite different names*

### Comparing `gitwithtea_py-0.1.0/gitwithtea_py/models/cron.py` & `gitwithtea_py-0.1.1/gitwithtea_py/models/cron.py`

 * *Files identical despite different names*

### Comparing `gitwithtea_py-0.1.0/gitwithtea_py/models/delete_email_option.py` & `gitwithtea_py-0.1.1/gitwithtea_py/models/delete_email_option.py`

 * *Files identical despite different names*

### Comparing `gitwithtea_py-0.1.0/gitwithtea_py/models/delete_file_options.py` & `gitwithtea_py-0.1.1/gitwithtea_py/models/delete_file_options.py`

 * *Files identical despite different names*

### Comparing `gitwithtea_py-0.1.0/gitwithtea_py/models/deploy_key.py` & `gitwithtea_py-0.1.1/gitwithtea_py/models/deploy_key.py`

 * *Files identical despite different names*

### Comparing `gitwithtea_py-0.1.0/gitwithtea_py/models/dismiss_pull_review_options.py` & `gitwithtea_py-0.1.1/gitwithtea_py/models/dismiss_pull_review_options.py`

 * *Files identical despite different names*

### Comparing `gitwithtea_py-0.1.0/gitwithtea_py/models/edit_attachment_options.py` & `gitwithtea_py-0.1.1/gitwithtea_py/models/edit_attachment_options.py`

 * *Files identical despite different names*

### Comparing `gitwithtea_py-0.1.0/gitwithtea_py/models/edit_branch_protection_option.py` & `gitwithtea_py-0.1.1/gitwithtea_py/models/edit_branch_protection_option.py`

 * *Files identical despite different names*

### Comparing `gitwithtea_py-0.1.0/gitwithtea_py/models/edit_deadline_option.py` & `gitwithtea_py-0.1.1/gitwithtea_py/models/edit_deadline_option.py`

 * *Files identical despite different names*

### Comparing `gitwithtea_py-0.1.0/gitwithtea_py/models/edit_git_hook_option.py` & `gitwithtea_py-0.1.1/gitwithtea_py/models/edit_git_hook_option.py`

 * *Files identical despite different names*

### Comparing `gitwithtea_py-0.1.0/gitwithtea_py/models/edit_hook_option.py` & `gitwithtea_py-0.1.1/gitwithtea_py/models/edit_hook_option.py`

 * *Files identical despite different names*

### Comparing `gitwithtea_py-0.1.0/gitwithtea_py/models/edit_issue_comment_option.py` & `gitwithtea_py-0.1.1/gitwithtea_py/models/edit_issue_comment_option.py`

 * *Files identical despite different names*

### Comparing `gitwithtea_py-0.1.0/gitwithtea_py/models/edit_issue_option.py` & `gitwithtea_py-0.1.1/gitwithtea_py/models/edit_issue_option.py`

 * *Files identical despite different names*

### Comparing `gitwithtea_py-0.1.0/gitwithtea_py/models/edit_label_option.py` & `gitwithtea_py-0.1.1/gitwithtea_py/models/edit_label_option.py`

 * *Files identical despite different names*

### Comparing `gitwithtea_py-0.1.0/gitwithtea_py/models/edit_milestone_option.py` & `gitwithtea_py-0.1.1/gitwithtea_py/models/edit_milestone_option.py`

 * *Files identical despite different names*

### Comparing `gitwithtea_py-0.1.0/gitwithtea_py/models/edit_org_option.py` & `gitwithtea_py-0.1.1/gitwithtea_py/models/edit_org_option.py`

 * *Files identical despite different names*

### Comparing `gitwithtea_py-0.1.0/gitwithtea_py/models/edit_pull_request_option.py` & `gitwithtea_py-0.1.1/gitwithtea_py/models/edit_pull_request_option.py`

 * *Files identical despite different names*

### Comparing `gitwithtea_py-0.1.0/gitwithtea_py/models/edit_reaction_option.py` & `gitwithtea_py-0.1.1/gitwithtea_py/models/edit_reaction_option.py`

 * *Files identical despite different names*

### Comparing `gitwithtea_py-0.1.0/gitwithtea_py/models/edit_release_option.py` & `gitwithtea_py-0.1.1/gitwithtea_py/models/edit_release_option.py`

 * *Files identical despite different names*

### Comparing `gitwithtea_py-0.1.0/gitwithtea_py/models/edit_repo_option.py` & `gitwithtea_py-0.1.1/gitwithtea_py/models/edit_repo_option.py`

 * *Files identical despite different names*

### Comparing `gitwithtea_py-0.1.0/gitwithtea_py/models/edit_team_option.py` & `gitwithtea_py-0.1.1/gitwithtea_py/models/edit_team_option.py`

 * *Files identical despite different names*

### Comparing `gitwithtea_py-0.1.0/gitwithtea_py/models/edit_user_option.py` & `gitwithtea_py-0.1.1/gitwithtea_py/models/edit_user_option.py`

 * *Files identical despite different names*

### Comparing `gitwithtea_py-0.1.0/gitwithtea_py/models/email.py` & `gitwithtea_py-0.1.1/gitwithtea_py/models/email.py`

 * *Files identical despite different names*

### Comparing `gitwithtea_py-0.1.0/gitwithtea_py/models/external_tracker.py` & `gitwithtea_py-0.1.1/gitwithtea_py/models/external_tracker.py`

 * *Files identical despite different names*

### Comparing `gitwithtea_py-0.1.0/gitwithtea_py/models/external_wiki.py` & `gitwithtea_py-0.1.1/gitwithtea_py/models/external_wiki.py`

 * *Files identical despite different names*

### Comparing `gitwithtea_py-0.1.0/gitwithtea_py/models/file_commit_response.py` & `gitwithtea_py-0.1.1/gitwithtea_py/models/file_commit_response.py`

 * *Files identical despite different names*

### Comparing `gitwithtea_py-0.1.0/gitwithtea_py/models/file_delete_response.py` & `gitwithtea_py-0.1.1/gitwithtea_py/models/file_delete_response.py`

 * *Files identical despite different names*

### Comparing `gitwithtea_py-0.1.0/gitwithtea_py/models/file_links_response.py` & `gitwithtea_py-0.1.1/gitwithtea_py/models/file_links_response.py`

 * *Files identical despite different names*

### Comparing `gitwithtea_py-0.1.0/gitwithtea_py/models/file_response.py` & `gitwithtea_py-0.1.1/gitwithtea_py/models/file_response.py`

 * *Files identical despite different names*

### Comparing `gitwithtea_py-0.1.0/gitwithtea_py/models/general_api_settings.py` & `gitwithtea_py-0.1.1/gitwithtea_py/models/general_api_settings.py`

 * *Files identical despite different names*

### Comparing `gitwithtea_py-0.1.0/gitwithtea_py/models/general_attachment_settings.py` & `gitwithtea_py-0.1.1/gitwithtea_py/models/general_attachment_settings.py`

 * *Files identical despite different names*

### Comparing `gitwithtea_py-0.1.0/gitwithtea_py/models/general_repo_settings.py` & `gitwithtea_py-0.1.1/gitwithtea_py/models/general_repo_settings.py`

 * *Files identical despite different names*

### Comparing `gitwithtea_py-0.1.0/gitwithtea_py/models/general_ui_settings.py` & `gitwithtea_py-0.1.1/gitwithtea_py/models/general_ui_settings.py`

 * *Files identical despite different names*

### Comparing `gitwithtea_py-0.1.0/gitwithtea_py/models/generate_repo_option.py` & `gitwithtea_py-0.1.1/gitwithtea_py/models/generate_repo_option.py`

 * *Files identical despite different names*

### Comparing `gitwithtea_py-0.1.0/gitwithtea_py/models/git_blob_response.py` & `gitwithtea_py-0.1.1/gitwithtea_py/models/git_blob_response.py`

 * *Files identical despite different names*

### Comparing `gitwithtea_py-0.1.0/gitwithtea_py/models/git_entry.py` & `gitwithtea_py-0.1.1/gitwithtea_py/models/git_entry.py`

 * *Files identical despite different names*

### Comparing `gitwithtea_py-0.1.0/gitwithtea_py/models/git_hook.py` & `gitwithtea_py-0.1.1/gitwithtea_py/models/git_hook.py`

 * *Files identical despite different names*

### Comparing `gitwithtea_py-0.1.0/gitwithtea_py/models/git_object.py` & `gitwithtea_py-0.1.1/gitwithtea_py/models/git_object.py`

 * *Files identical despite different names*

### Comparing `gitwithtea_py-0.1.0/gitwithtea_py/models/git_tree_response.py` & `gitwithtea_py-0.1.1/gitwithtea_py/models/git_tree_response.py`

 * *Files identical despite different names*

### Comparing `gitwithtea_py-0.1.0/gitwithtea_py/models/gpg_key.py` & `gitwithtea_py-0.1.1/gitwithtea_py/models/gpg_key.py`

 * *Files identical despite different names*

### Comparing `gitwithtea_py-0.1.0/gitwithtea_py/models/gpg_key_email.py` & `gitwithtea_py-0.1.1/gitwithtea_py/models/gpg_key_email.py`

 * *Files identical despite different names*

### Comparing `gitwithtea_py-0.1.0/gitwithtea_py/models/hook.py` & `gitwithtea_py-0.1.1/gitwithtea_py/models/hook.py`

 * *Files identical despite different names*

### Comparing `gitwithtea_py-0.1.0/gitwithtea_py/models/identity.py` & `gitwithtea_py-0.1.1/gitwithtea_py/models/identity.py`

 * *Files identical despite different names*

### Comparing `gitwithtea_py-0.1.0/gitwithtea_py/models/inline_response200.py` & `gitwithtea_py-0.1.1/gitwithtea_py/models/inline_response200.py`

 * *Files identical despite different names*

### Comparing `gitwithtea_py-0.1.0/gitwithtea_py/models/inline_response2001.py` & `gitwithtea_py-0.1.1/gitwithtea_py/models/inline_response2001.py`

 * *Files identical despite different names*

### Comparing `gitwithtea_py-0.1.0/gitwithtea_py/models/internal_tracker.py` & `gitwithtea_py-0.1.1/gitwithtea_py/models/internal_tracker.py`

 * *Files identical despite different names*

### Comparing `gitwithtea_py-0.1.0/gitwithtea_py/models/issue.py` & `gitwithtea_py-0.1.1/gitwithtea_py/models/issue.py`

 * *Files identical despite different names*

### Comparing `gitwithtea_py-0.1.0/gitwithtea_py/models/issue_deadline.py` & `gitwithtea_py-0.1.1/gitwithtea_py/models/issue_deadline.py`

 * *Files identical despite different names*

### Comparing `gitwithtea_py-0.1.0/gitwithtea_py/models/issue_form_field.py` & `gitwithtea_py-0.1.1/gitwithtea_py/models/issue_form_field.py`

 * *Files identical despite different names*

### Comparing `gitwithtea_py-0.1.0/gitwithtea_py/models/issue_form_field_type.py` & `gitwithtea_py-0.1.1/gitwithtea_py/models/issue_form_field_type.py`

 * *Files identical despite different names*

### Comparing `gitwithtea_py-0.1.0/gitwithtea_py/models/issue_labels_option.py` & `gitwithtea_py-0.1.1/gitwithtea_py/models/issue_labels_option.py`

 * *Files identical despite different names*

### Comparing `gitwithtea_py-0.1.0/gitwithtea_py/models/issue_template.py` & `gitwithtea_py-0.1.1/gitwithtea_py/models/issue_template.py`

 * *Files identical despite different names*

### Comparing `gitwithtea_py-0.1.0/gitwithtea_py/models/issue_template_labels.py` & `gitwithtea_py-0.1.1/gitwithtea_py/models/issue_template_labels.py`

 * *Files identical despite different names*

### Comparing `gitwithtea_py-0.1.0/gitwithtea_py/models/label.py` & `gitwithtea_py-0.1.1/gitwithtea_py/models/label.py`

 * *Files identical despite different names*

### Comparing `gitwithtea_py-0.1.0/gitwithtea_py/models/markdown_option.py` & `gitwithtea_py-0.1.1/gitwithtea_py/models/markdown_option.py`

 * *Files identical despite different names*

### Comparing `gitwithtea_py-0.1.0/gitwithtea_py/models/merge_pull_request_option.py` & `gitwithtea_py-0.1.1/gitwithtea_py/models/merge_pull_request_option.py`

 * *Files identical despite different names*

### Comparing `gitwithtea_py-0.1.0/gitwithtea_py/models/migrate_repo_options.py` & `gitwithtea_py-0.1.1/gitwithtea_py/models/migrate_repo_options.py`

 * *Files identical despite different names*

### Comparing `gitwithtea_py-0.1.0/gitwithtea_py/models/milestone.py` & `gitwithtea_py-0.1.1/gitwithtea_py/models/milestone.py`

 * *Files identical despite different names*

### Comparing `gitwithtea_py-0.1.0/gitwithtea_py/models/node_info.py` & `gitwithtea_py-0.1.1/gitwithtea_py/models/node_info.py`

 * *Files identical despite different names*

### Comparing `gitwithtea_py-0.1.0/gitwithtea_py/models/node_info_services.py` & `gitwithtea_py-0.1.1/gitwithtea_py/models/node_info_services.py`

 * *Files identical despite different names*

### Comparing `gitwithtea_py-0.1.0/gitwithtea_py/models/node_info_software.py` & `gitwithtea_py-0.1.1/gitwithtea_py/models/node_info_software.py`

 * *Files identical despite different names*

### Comparing `gitwithtea_py-0.1.0/gitwithtea_py/models/node_info_usage.py` & `gitwithtea_py-0.1.1/gitwithtea_py/models/node_info_usage.py`

 * *Files identical despite different names*

### Comparing `gitwithtea_py-0.1.0/gitwithtea_py/models/node_info_usage_users.py` & `gitwithtea_py-0.1.1/gitwithtea_py/models/node_info_usage_users.py`

 * *Files identical despite different names*

### Comparing `gitwithtea_py-0.1.0/gitwithtea_py/models/note.py` & `gitwithtea_py-0.1.1/gitwithtea_py/models/note.py`

 * *Files identical despite different names*

### Comparing `gitwithtea_py-0.1.0/gitwithtea_py/models/notification_count.py` & `gitwithtea_py-0.1.1/gitwithtea_py/models/notification_count.py`

 * *Files identical despite different names*

### Comparing `gitwithtea_py-0.1.0/gitwithtea_py/models/notification_subject.py` & `gitwithtea_py-0.1.1/gitwithtea_py/models/notification_subject.py`

 * *Files identical despite different names*

### Comparing `gitwithtea_py-0.1.0/gitwithtea_py/models/notification_thread.py` & `gitwithtea_py-0.1.1/gitwithtea_py/models/notification_thread.py`

 * *Files identical despite different names*

### Comparing `gitwithtea_py-0.1.0/gitwithtea_py/models/notify_subject_type.py` & `gitwithtea_py-0.1.1/gitwithtea_py/models/notify_subject_type.py`

 * *Files identical despite different names*

### Comparing `gitwithtea_py-0.1.0/gitwithtea_py/models/o_auth2_application.py` & `gitwithtea_py-0.1.1/gitwithtea_py/models/o_auth2_application.py`

 * *Files identical despite different names*

### Comparing `gitwithtea_py-0.1.0/gitwithtea_py/models/organization.py` & `gitwithtea_py-0.1.1/gitwithtea_py/models/organization.py`

 * *Files identical despite different names*

### Comparing `gitwithtea_py-0.1.0/gitwithtea_py/models/organization_permissions.py` & `gitwithtea_py-0.1.1/gitwithtea_py/models/organization_permissions.py`

 * *Files identical despite different names*

### Comparing `gitwithtea_py-0.1.0/gitwithtea_py/models/package.py` & `gitwithtea_py-0.1.1/gitwithtea_py/models/package.py`

 * *Files identical despite different names*

### Comparing `gitwithtea_py-0.1.0/gitwithtea_py/models/package_file.py` & `gitwithtea_py-0.1.1/gitwithtea_py/models/package_file.py`

 * *Files identical despite different names*

### Comparing `gitwithtea_py-0.1.0/gitwithtea_py/models/payload_commit.py` & `gitwithtea_py-0.1.1/gitwithtea_py/models/payload_commit.py`

 * *Files identical despite different names*

### Comparing `gitwithtea_py-0.1.0/gitwithtea_py/models/payload_commit_verification.py` & `gitwithtea_py-0.1.1/gitwithtea_py/models/payload_commit_verification.py`

 * *Files identical despite different names*

### Comparing `gitwithtea_py-0.1.0/gitwithtea_py/models/payload_user.py` & `gitwithtea_py-0.1.1/gitwithtea_py/models/payload_user.py`

 * *Files identical despite different names*

### Comparing `gitwithtea_py-0.1.0/gitwithtea_py/models/permission.py` & `gitwithtea_py-0.1.1/gitwithtea_py/models/permission.py`

 * *Files identical despite different names*

### Comparing `gitwithtea_py-0.1.0/gitwithtea_py/models/pr_branch_info.py` & `gitwithtea_py-0.1.1/gitwithtea_py/models/pr_branch_info.py`

 * *Files identical despite different names*

### Comparing `gitwithtea_py-0.1.0/gitwithtea_py/models/public_key.py` & `gitwithtea_py-0.1.1/gitwithtea_py/models/public_key.py`

 * *Files identical despite different names*

### Comparing `gitwithtea_py-0.1.0/gitwithtea_py/models/pull_request.py` & `gitwithtea_py-0.1.1/gitwithtea_py/models/pull_request.py`

 * *Files identical despite different names*

### Comparing `gitwithtea_py-0.1.0/gitwithtea_py/models/pull_request_meta.py` & `gitwithtea_py-0.1.1/gitwithtea_py/models/pull_request_meta.py`

 * *Files identical despite different names*

### Comparing `gitwithtea_py-0.1.0/gitwithtea_py/models/pull_review.py` & `gitwithtea_py-0.1.1/gitwithtea_py/models/pull_review.py`

 * *Files identical despite different names*

### Comparing `gitwithtea_py-0.1.0/gitwithtea_py/models/pull_review_comment.py` & `gitwithtea_py-0.1.1/gitwithtea_py/models/pull_review_comment.py`

 * *Files identical despite different names*

### Comparing `gitwithtea_py-0.1.0/gitwithtea_py/models/pull_review_request_options.py` & `gitwithtea_py-0.1.1/gitwithtea_py/models/pull_review_request_options.py`

 * *Files identical despite different names*

### Comparing `gitwithtea_py-0.1.0/gitwithtea_py/models/push_mirror.py` & `gitwithtea_py-0.1.1/gitwithtea_py/models/push_mirror.py`

 * *Files identical despite different names*

### Comparing `gitwithtea_py-0.1.0/gitwithtea_py/models/reaction.py` & `gitwithtea_py-0.1.1/gitwithtea_py/models/reaction.py`

 * *Files identical despite different names*

### Comparing `gitwithtea_py-0.1.0/gitwithtea_py/models/reference.py` & `gitwithtea_py-0.1.1/gitwithtea_py/models/reference.py`

 * *Files identical despite different names*

### Comparing `gitwithtea_py-0.1.0/gitwithtea_py/models/release.py` & `gitwithtea_py-0.1.1/gitwithtea_py/models/release.py`

 * *Files identical despite different names*

### Comparing `gitwithtea_py-0.1.0/gitwithtea_py/models/repo_collaborator_permission.py` & `gitwithtea_py-0.1.1/gitwithtea_py/models/repo_collaborator_permission.py`

 * *Files identical despite different names*

### Comparing `gitwithtea_py-0.1.0/gitwithtea_py/models/repo_commit.py` & `gitwithtea_py-0.1.1/gitwithtea_py/models/repo_commit.py`

 * *Files identical despite different names*

### Comparing `gitwithtea_py-0.1.0/gitwithtea_py/models/repo_topic_options.py` & `gitwithtea_py-0.1.1/gitwithtea_py/models/repo_topic_options.py`

 * *Files identical despite different names*

### Comparing `gitwithtea_py-0.1.0/gitwithtea_py/models/repo_transfer.py` & `gitwithtea_py-0.1.1/gitwithtea_py/models/repo_transfer.py`

 * *Files identical despite different names*

### Comparing `gitwithtea_py-0.1.0/gitwithtea_py/models/repository.py` & `gitwithtea_py-0.1.1/gitwithtea_py/models/repository.py`

 * *Files identical despite different names*

### Comparing `gitwithtea_py-0.1.0/gitwithtea_py/models/repository_meta.py` & `gitwithtea_py-0.1.1/gitwithtea_py/models/repository_meta.py`

 * *Files identical despite different names*

### Comparing `gitwithtea_py-0.1.0/gitwithtea_py/models/review_state_type.py` & `gitwithtea_py-0.1.1/gitwithtea_py/models/review_state_type.py`

 * *Files identical despite different names*

### Comparing `gitwithtea_py-0.1.0/gitwithtea_py/models/search_results.py` & `gitwithtea_py-0.1.1/gitwithtea_py/models/search_results.py`

 * *Files identical despite different names*

### Comparing `gitwithtea_py-0.1.0/gitwithtea_py/models/server_version.py` & `gitwithtea_py-0.1.1/gitwithtea_py/models/server_version.py`

 * *Files identical despite different names*

### Comparing `gitwithtea_py-0.1.0/gitwithtea_py/models/state_type.py` & `gitwithtea_py-0.1.1/gitwithtea_py/models/state_type.py`

 * *Files identical despite different names*

### Comparing `gitwithtea_py-0.1.0/gitwithtea_py/models/stop_watch.py` & `gitwithtea_py-0.1.1/gitwithtea_py/models/stop_watch.py`

 * *Files identical despite different names*

### Comparing `gitwithtea_py-0.1.0/gitwithtea_py/models/submit_pull_review_options.py` & `gitwithtea_py-0.1.1/gitwithtea_py/models/submit_pull_review_options.py`

 * *Files identical despite different names*

### Comparing `gitwithtea_py-0.1.0/gitwithtea_py/models/tag.py` & `gitwithtea_py-0.1.1/gitwithtea_py/models/tag.py`

 * *Files identical despite different names*

### Comparing `gitwithtea_py-0.1.0/gitwithtea_py/models/team.py` & `gitwithtea_py-0.1.1/gitwithtea_py/models/team.py`

 * *Files identical despite different names*

### Comparing `gitwithtea_py-0.1.0/gitwithtea_py/models/time_stamp.py` & `gitwithtea_py-0.1.1/gitwithtea_py/models/time_stamp.py`

 * *Files identical despite different names*

### Comparing `gitwithtea_py-0.1.0/gitwithtea_py/models/timeline_comment.py` & `gitwithtea_py-0.1.1/gitwithtea_py/models/timeline_comment.py`

 * *Files identical despite different names*

### Comparing `gitwithtea_py-0.1.0/gitwithtea_py/models/topic_name.py` & `gitwithtea_py-0.1.1/gitwithtea_py/models/topic_name.py`

 * *Files identical despite different names*

### Comparing `gitwithtea_py-0.1.0/gitwithtea_py/models/topic_response.py` & `gitwithtea_py-0.1.1/gitwithtea_py/models/topic_response.py`

 * *Files identical despite different names*

### Comparing `gitwithtea_py-0.1.0/gitwithtea_py/models/tracked_time.py` & `gitwithtea_py-0.1.1/gitwithtea_py/models/tracked_time.py`

 * *Files identical despite different names*

### Comparing `gitwithtea_py-0.1.0/gitwithtea_py/models/transfer_repo_option.py` & `gitwithtea_py-0.1.1/gitwithtea_py/models/transfer_repo_option.py`

 * *Files identical despite different names*

### Comparing `gitwithtea_py-0.1.0/gitwithtea_py/models/update_file_options.py` & `gitwithtea_py-0.1.1/gitwithtea_py/models/update_file_options.py`

 * *Files identical despite different names*

### Comparing `gitwithtea_py-0.1.0/gitwithtea_py/models/user.py` & `gitwithtea_py-0.1.1/gitwithtea_py/models/user.py`

 * *Files identical despite different names*

### Comparing `gitwithtea_py-0.1.0/gitwithtea_py/models/user_heatmap_data.py` & `gitwithtea_py-0.1.1/gitwithtea_py/models/user_heatmap_data.py`

 * *Files identical despite different names*

### Comparing `gitwithtea_py-0.1.0/gitwithtea_py/models/user_settings.py` & `gitwithtea_py-0.1.1/gitwithtea_py/models/user_settings.py`

 * *Files identical despite different names*

### Comparing `gitwithtea_py-0.1.0/gitwithtea_py/models/user_settings_options.py` & `gitwithtea_py-0.1.1/gitwithtea_py/models/user_settings_options.py`

 * *Files identical despite different names*

### Comparing `gitwithtea_py-0.1.0/gitwithtea_py/models/watch_info.py` & `gitwithtea_py-0.1.1/gitwithtea_py/models/watch_info.py`

 * *Files identical despite different names*

### Comparing `gitwithtea_py-0.1.0/gitwithtea_py/models/wiki_commit.py` & `gitwithtea_py-0.1.1/gitwithtea_py/models/wiki_commit.py`

 * *Files identical despite different names*

### Comparing `gitwithtea_py-0.1.0/gitwithtea_py/models/wiki_commit_list.py` & `gitwithtea_py-0.1.1/gitwithtea_py/models/wiki_commit_list.py`

 * *Files identical despite different names*

### Comparing `gitwithtea_py-0.1.0/gitwithtea_py/models/wiki_page.py` & `gitwithtea_py-0.1.1/gitwithtea_py/models/wiki_page.py`

 * *Files identical despite different names*

### Comparing `gitwithtea_py-0.1.0/gitwithtea_py/models/wiki_page_meta_data.py` & `gitwithtea_py-0.1.1/gitwithtea_py/models/wiki_page_meta_data.py`

 * *Files identical despite different names*

### Comparing `gitwithtea_py-0.1.0/gitwithtea_py/rest.py` & `gitwithtea_py-0.1.1/gitwithtea_py/rest.py`

 * *Files identical despite different names*

### Comparing `gitwithtea_py-0.1.0/pyproject.toml` & `gitwithtea_py-0.1.1/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 [tool.poetry]
 name = "gitwithtea-py"
-version = "0.1.0"
-description = "Gigitwithtea API wrapper in Python"
+version = "0.1.1"
+description = "Gitea API wrapper in Python"
 authors = ["0xMRTT <0xMRTT@proton.me>"]
 maintainers = ["0xMRTT <0xMRTT@proton.me>"]
 readme = "README.md"
 packages = [{include = "gitwithtea_py"}]
 license = "GPL-3.0-or-later"
 homepage = "https://codeberg.org/gitwithtea-py/gitwithtea_py"
 documentation = "https://codeberg.org/gitwithtea-py/gitwithtea_py"
@@ -34,10 +34,10 @@
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
 
 [[tool.poetry.source]]
 name = "codeberg"
-url = "https://codeberg.org/api/packages/Bavarder/pypi"
+url = "https://codeberg.org/api/packages/gitwithtea-py/pypi"
 default = false
 secondary = true
```

### Comparing `gitwithtea_py-0.1.0/PKG-INFO` & `gitwithtea_py-0.1.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: gitwithtea-py
-Version: 0.1.0
-Summary: Gigitwithtea API wrapper in Python
+Version: 0.1.1
+Summary: Gitea API wrapper in Python
 Home-page: https://codeberg.org/gitwithtea-py/gitwithtea_py
 License: GPL-3.0-or-later
 Keywords: gitea,tea,git,api,forgejo,python,swagger
 Author: 0xMRTT
 Author-email: 0xMRTT@proton.me
 Maintainer: 0xMRTT
 Maintainer-email: 0xMRTT@proton.me
```

