# Comparing `tmp/fern_persona-0.0.2.tar.gz` & `tmp/fern_persona-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fern_persona-0.0.2.tar", max compression
+gzip compressed data, was "fern_persona-0.0.3.tar", max compression
```

## Comparing `fern_persona-0.0.2.tar` & `fern_persona-0.0.3.tar`

### file list

```diff
@@ -1,913 +1,913 @@
--rw-r--r--   0        0        0     1683 2023-05-23 16:50:24.961418 fern_persona-0.0.2/README.md
--rw-r--r--   0        0        0      374 2023-05-23 16:50:24.961418 fern_persona-0.0.2/pyproject.toml
--rw-r--r--   0        0        0    89351 2023-05-23 16:50:24.961418 fern_persona-0.0.2/src/persona/__init__.py
--rw-r--r--   0        0        0     9082 2023-05-23 16:50:24.961418 fern_persona-0.0.2/src/persona/client.py
--rw-r--r--   0        0        0      348 2023-05-23 16:50:24.961418 fern_persona-0.0.2/src/persona/core/__init__.py
--rw-r--r--   0        0        0      426 2023-05-23 16:50:24.961418 fern_persona-0.0.2/src/persona/core/api_error.py
--rw-r--r--   0        0        0     1047 2023-05-23 16:50:24.961418 fern_persona-0.0.2/src/persona/core/datetime_utils.py
--rw-r--r--   0        0        0     3710 2023-05-23 16:50:24.961418 fern_persona-0.0.2/src/persona/core/jsonable_encoder.py
--rw-r--r--   0        0        0      385 2023-05-23 16:50:24.961418 fern_persona-0.0.2/src/persona/core/remove_none_from_headers.py
--rw-r--r--   0        0        0      163 2023-05-23 16:50:24.961418 fern_persona-0.0.2/src/persona/environment.py
--rw-r--r--   0        0        0      355 2023-05-23 16:50:24.961418 fern_persona-0.0.2/src/persona/errors/__init__.py
--rw-r--r--   0        0        0      248 2023-05-23 16:50:24.961418 fern_persona-0.0.2/src/persona/errors/bad_request_error.py
--rw-r--r--   0        0        0      246 2023-05-23 16:50:24.961418 fern_persona-0.0.2/src/persona/errors/conflict_error.py
--rw-r--r--   0        0        0      246 2023-05-23 16:50:24.961418 fern_persona-0.0.2/src/persona/errors/not_found_error.py
--rw-r--r--   0        0        0      341 2023-05-23 16:50:24.961418 fern_persona-0.0.2/src/persona/errors/unprocessable_entity_error.py
--rw-r--r--   0        0        0        0 2023-05-23 16:50:24.961418 fern_persona-0.0.2/src/persona/py.typed
--rw-r--r--   0        0        0     1282 2023-05-23 16:50:24.961418 fern_persona-0.0.2/src/persona/resources/__init__.py
--rw-r--r--   0        0        0       65 2023-05-23 16:50:24.961418 fern_persona-0.0.2/src/persona/resources/accounts/__init__.py
--rw-r--r--   0        0        0    27071 2023-05-23 16:50:24.961418 fern_persona-0.0.2/src/persona/resources/accounts/client.py
--rw-r--r--   0        0        0       65 2023-05-23 16:50:24.961418 fern_persona-0.0.2/src/persona/resources/api_keys/__init__.py
--rw-r--r--   0        0        0    12850 2023-05-23 16:50:24.961418 fern_persona-0.0.2/src/persona/resources/api_keys/client.py
--rw-r--r--   0        0        0       65 2023-05-23 16:50:24.965418 fern_persona-0.0.2/src/persona/resources/api_logs/__init__.py
--rw-r--r--   0        0        0     4924 2023-05-23 16:50:24.965418 fern_persona-0.0.2/src/persona/resources/api_logs/client.py
--rw-r--r--   0        0        0       65 2023-05-23 16:50:24.965418 fern_persona-0.0.2/src/persona/resources/cases/__init__.py
--rw-r--r--   0        0        0    19144 2023-05-23 16:50:24.965418 fern_persona-0.0.2/src/persona/resources/cases/client.py
--rw-r--r--   0        0        0       65 2023-05-23 16:50:24.965418 fern_persona-0.0.2/src/persona/resources/database_verifications/__init__.py
--rw-r--r--   0        0        0     7986 2023-05-23 16:50:24.965418 fern_persona-0.0.2/src/persona/resources/database_verifications/client.py
--rw-r--r--   0        0        0       65 2023-05-23 16:50:24.965418 fern_persona-0.0.2/src/persona/resources/document_verifications/__init__.py
--rw-r--r--   0        0        0     8038 2023-05-23 16:50:24.965418 fern_persona-0.0.2/src/persona/resources/document_verifications/client.py
--rw-r--r--   0        0        0       65 2023-05-23 16:50:24.965418 fern_persona-0.0.2/src/persona/resources/documents/__init__.py
--rw-r--r--   0        0        0    11036 2023-05-23 16:50:24.965418 fern_persona-0.0.2/src/persona/resources/documents/client.py
--rw-r--r--   0        0        0       65 2023-05-23 16:50:24.965418 fern_persona-0.0.2/src/persona/resources/email_address_verifications/__init__.py
--rw-r--r--   0        0        0    11147 2023-05-23 16:50:24.965418 fern_persona-0.0.2/src/persona/resources/email_address_verifications/client.py
--rw-r--r--   0        0        0       65 2023-05-23 16:50:24.965418 fern_persona-0.0.2/src/persona/resources/events/__init__.py
--rw-r--r--   0        0        0     6189 2023-05-23 16:50:24.965418 fern_persona-0.0.2/src/persona/resources/events/client.py
--rw-r--r--   0        0        0       65 2023-05-23 16:50:24.965418 fern_persona-0.0.2/src/persona/resources/government_id_documents/__init__.py
--rw-r--r--   0        0        0     9367 2023-05-23 16:50:24.965418 fern_persona-0.0.2/src/persona/resources/government_id_documents/client.py
--rw-r--r--   0        0        0       65 2023-05-23 16:50:24.965418 fern_persona-0.0.2/src/persona/resources/government_id_verifications/__init__.py
--rw-r--r--   0        0        0    11578 2023-05-23 16:50:24.965418 fern_persona-0.0.2/src/persona/resources/government_id_verifications/client.py
--rw-r--r--   0        0        0       65 2023-05-23 16:50:24.965418 fern_persona-0.0.2/src/persona/resources/graph_queries/__init__.py
--rw-r--r--   0        0        0     4115 2023-05-23 16:50:24.965418 fern_persona-0.0.2/src/persona/resources/graph_queries/client.py
--rw-r--r--   0        0        0       65 2023-05-23 16:50:24.965418 fern_persona-0.0.2/src/persona/resources/importers/__init__.py
--rw-r--r--   0        0        0    23039 2023-05-23 16:50:24.965418 fern_persona-0.0.2/src/persona/resources/importers/client.py
--rw-r--r--   0        0        0       65 2023-05-23 16:50:24.965418 fern_persona-0.0.2/src/persona/resources/inquiries/__init__.py
--rw-r--r--   0        0        0    34666 2023-05-23 16:50:24.965418 fern_persona-0.0.2/src/persona/resources/inquiries/client.py
--rw-r--r--   0        0        0       65 2023-05-23 16:50:24.965418 fern_persona-0.0.2/src/persona/resources/list_items/__init__.py
--rw-r--r--   0        0        0    47166 2023-05-23 16:50:24.965418 fern_persona-0.0.2/src/persona/resources/list_items/client.py
--rw-r--r--   0        0        0       65 2023-05-23 16:50:24.965418 fern_persona-0.0.2/src/persona/resources/lists/__init__.py
--rw-r--r--   0        0        0    39214 2023-05-23 16:50:24.965418 fern_persona-0.0.2/src/persona/resources/lists/client.py
--rw-r--r--   0        0        0       65 2023-05-23 16:50:24.965418 fern_persona-0.0.2/src/persona/resources/phone_carrier_database_verifications/__init__.py
--rw-r--r--   0        0        0     9207 2023-05-23 16:50:24.965418 fern_persona-0.0.2/src/persona/resources/phone_carrier_database_verifications/client.py
--rw-r--r--   0        0        0       65 2023-05-23 16:50:24.965418 fern_persona-0.0.2/src/persona/resources/phone_number_verifications/__init__.py
--rw-r--r--   0        0        0    11061 2023-05-23 16:50:24.965418 fern_persona-0.0.2/src/persona/resources/phone_number_verifications/client.py
--rw-r--r--   0        0        0       65 2023-05-23 16:50:24.965418 fern_persona-0.0.2/src/persona/resources/print_verifications/__init__.py
--rw-r--r--   0        0        0     2140 2023-05-23 16:50:24.965418 fern_persona-0.0.2/src/persona/resources/print_verifications/client.py
--rw-r--r--   0        0        0       65 2023-05-23 16:50:24.965418 fern_persona-0.0.2/src/persona/resources/reports/__init__.py
--rw-r--r--   0        0        0    31595 2023-05-23 16:50:24.965418 fern_persona-0.0.2/src/persona/resources/reports/client.py
--rw-r--r--   0        0        0       65 2023-05-23 16:50:24.965418 fern_persona-0.0.2/src/persona/resources/selfie_verifications/__init__.py
--rw-r--r--   0        0        0     8611 2023-05-23 16:50:24.965418 fern_persona-0.0.2/src/persona/resources/selfie_verifications/client.py
--rw-r--r--   0        0        0       65 2023-05-23 16:50:24.965418 fern_persona-0.0.2/src/persona/resources/serpo_database_verifications/__init__.py
--rw-r--r--   0        0        0     8878 2023-05-23 16:50:24.965418 fern_persona-0.0.2/src/persona/resources/serpo_database_verifications/client.py
--rw-r--r--   0        0        0       65 2023-05-23 16:50:24.965418 fern_persona-0.0.2/src/persona/resources/tin_database_verifications/__init__.py
--rw-r--r--   0        0        0     9240 2023-05-23 16:50:24.965418 fern_persona-0.0.2/src/persona/resources/tin_database_verifications/client.py
--rw-r--r--   0        0        0       65 2023-05-23 16:50:24.965418 fern_persona-0.0.2/src/persona/resources/user_audit_logs/__init__.py
--rw-r--r--   0        0        0     5057 2023-05-23 16:50:24.965418 fern_persona-0.0.2/src/persona/resources/user_audit_logs/client.py
--rw-r--r--   0        0        0       65 2023-05-23 16:50:24.965418 fern_persona-0.0.2/src/persona/resources/verifications/__init__.py
--rw-r--r--   0        0        0     2302 2023-05-23 16:50:24.965418 fern_persona-0.0.2/src/persona/resources/verifications/client.py
--rw-r--r--   0        0        0       65 2023-05-23 16:50:24.965418 fern_persona-0.0.2/src/persona/resources/workflows/__init__.py
--rw-r--r--   0        0        0     3702 2023-05-23 16:50:24.965418 fern_persona-0.0.2/src/persona/resources/workflows/client.py
--rw-r--r--   0        0        0   141824 2023-05-23 16:50:24.965418 fern_persona-0.0.2/src/persona/types/__init__.py
--rw-r--r--   0        0        0      855 2023-05-23 16:50:24.965418 fern_persona-0.0.2/src/persona/types/add_a_tag_1_request_meta.py
--rw-r--r--   0        0        0      854 2023-05-23 16:50:24.965418 fern_persona-0.0.2/src/persona/types/add_a_tag_request_meta.py
--rw-r--r--   0        0        0      965 2023-05-23 16:50:24.965418 fern_persona-0.0.2/src/persona/types/add_persona_objects_request_meta.py
--rw-r--r--   0        0        0      879 2023-05-23 16:50:24.965418 fern_persona-0.0.2/src/persona/types/add_persona_objects_response.py
--rw-r--r--   0        0        0     1163 2023-05-23 16:50:24.965418 fern_persona-0.0.2/src/persona/types/add_persona_objects_response_data.py
--rw-r--r--   0        0        0     1835 2023-05-23 16:50:24.965418 fern_persona-0.0.2/src/persona/types/add_persona_objects_response_data_attributes.py
--rw-r--r--   0        0        0     1994 2023-05-23 16:50:24.965418 fern_persona-0.0.2/src/persona/types/add_persona_objects_response_data_relationships.py
--rw-r--r--   0        0        0      821 2023-05-23 16:50:24.965418 fern_persona-0.0.2/src/persona/types/add_persona_objects_response_data_relationships_accounts.py
--rw-r--r--   0        0        0      825 2023-05-23 16:50:24.965418 fern_persona-0.0.2/src/persona/types/add_persona_objects_response_data_relationships_case_comments.py
--rw-r--r--   0        0        0     1008 2023-05-23 16:50:24.965418 fern_persona-0.0.2/src/persona/types/add_persona_objects_response_data_relationships_case_template.py
--rw-r--r--   0        0        0      838 2023-05-23 16:50:24.965418 fern_persona-0.0.2/src/persona/types/add_persona_objects_response_data_relationships_case_template_data.py
--rw-r--r--   0        0        0     1021 2023-05-23 16:50:24.965418 fern_persona-0.0.2/src/persona/types/add_persona_objects_response_data_relationships_inquiries.py
--rw-r--r--   0        0        0      839 2023-05-23 16:50:24.969419 fern_persona-0.0.2/src/persona/types/add_persona_objects_response_data_relationships_inquiries_data_item.py
--rw-r--r--   0        0        0     1013 2023-05-23 16:50:24.969419 fern_persona-0.0.2/src/persona/types/add_persona_objects_response_data_relationships_reports.py
--rw-r--r--   0        0        0      837 2023-05-23 16:50:24.969419 fern_persona-0.0.2/src/persona/types/add_persona_objects_response_data_relationships_reports_data_item.py
--rw-r--r--   0        0        0      848 2023-05-23 16:50:24.969419 fern_persona-0.0.2/src/persona/types/approve_an_inquiry_request_meta.py
--rw-r--r--   0        0        0      875 2023-05-23 16:50:24.969419 fern_persona-0.0.2/src/persona/types/approve_an_inquiry_response.py
--rw-r--r--   0        0        0     1156 2023-05-23 16:50:24.969419 fern_persona-0.0.2/src/persona/types/approve_an_inquiry_response_data.py
--rw-r--r--   0        0        0     1196 2023-05-23 16:50:24.969419 fern_persona-0.0.2/src/persona/types/approve_an_inquiry_response_data_attributes.py
--rw-r--r--   0        0        0     1582 2023-05-23 16:50:24.969419 fern_persona-0.0.2/src/persona/types/approve_an_inquiry_response_data_relationships.py
--rw-r--r--   0        0        0      983 2023-05-23 16:50:24.969419 fern_persona-0.0.2/src/persona/types/approve_an_inquiry_response_data_relationships_account.py
--rw-r--r--   0        0        0      832 2023-05-23 16:50:24.969419 fern_persona-0.0.2/src/persona/types/approve_an_inquiry_response_data_relationships_account_data.py
--rw-r--r--   0        0        0      819 2023-05-23 16:50:24.969419 fern_persona-0.0.2/src/persona/types/approve_an_inquiry_response_data_relationships_reports.py
--rw-r--r--   0        0        0      987 2023-05-23 16:50:24.969419 fern_persona-0.0.2/src/persona/types/approve_an_inquiry_response_data_relationships_template.py
--rw-r--r--   0        0        0      833 2023-05-23 16:50:24.969419 fern_persona-0.0.2/src/persona/types/approve_an_inquiry_response_data_relationships_template_data.py
--rw-r--r--   0        0        0     1033 2023-05-23 16:50:24.969419 fern_persona-0.0.2/src/persona/types/approve_an_inquiry_response_data_relationships_verifications.py
--rw-r--r--   0        0        0      842 2023-05-23 16:50:24.969419 fern_persona-0.0.2/src/persona/types/approve_an_inquiry_response_data_relationships_verifications_data_item.py
--rw-r--r--   0        0        0      950 2023-05-23 16:50:24.969419 fern_persona-0.0.2/src/persona/types/archive_a_browser_fingerprint_list_item_response.py
--rw-r--r--   0        0        0     1306 2023-05-23 16:50:24.969419 fern_persona-0.0.2/src/persona/types/archive_a_browser_fingerprint_list_item_response_data.py
--rw-r--r--   0        0        0     1187 2023-05-23 16:50:24.969419 fern_persona-0.0.2/src/persona/types/archive_a_browser_fingerprint_list_item_response_data_attributes.py
--rw-r--r--   0        0        0     1041 2023-05-23 16:50:24.969419 fern_persona-0.0.2/src/persona/types/archive_a_browser_fingerprint_list_item_response_data_relationships.py
--rw-r--r--   0        0        0      824 2023-05-23 16:50:24.969419 fern_persona-0.0.2/src/persona/types/archive_a_browser_fingerprint_list_item_response_data_relationships_creator.py
--rw-r--r--   0        0        0      921 2023-05-23 16:50:24.969419 fern_persona-0.0.2/src/persona/types/archive_a_geolocation_list_item_response.py
--rw-r--r--   0        0        0     1246 2023-05-23 16:50:24.969419 fern_persona-0.0.2/src/persona/types/archive_a_geolocation_list_item_response_data.py
--rw-r--r--   0        0        0     1303 2023-05-23 16:50:24.969419 fern_persona-0.0.2/src/persona/types/archive_a_geolocation_list_item_response_data_attributes.py
--rw-r--r--   0        0        0     1012 2023-05-23 16:50:24.969419 fern_persona-0.0.2/src/persona/types/archive_a_geolocation_list_item_response_data_relationships.py
--rw-r--r--   0        0        0      817 2023-05-23 16:50:24.969419 fern_persona-0.0.2/src/persona/types/archive_a_geolocation_list_item_response_data_relationships_creator.py
--rw-r--r--   0        0        0      951 2023-05-23 16:50:24.969419 fern_persona-0.0.2/src/persona/types/archive_a_government_id_number_list_item_response.py
--rw-r--r--   0        0        0     1308 2023-05-23 16:50:24.969419 fern_persona-0.0.2/src/persona/types/archive_a_government_id_number_list_item_response_data.py
--rw-r--r--   0        0        0     1297 2023-05-23 16:50:24.969419 fern_persona-0.0.2/src/persona/types/archive_a_government_id_number_list_item_response_data_attributes.py
--rw-r--r--   0        0        0     1042 2023-05-23 16:50:24.969419 fern_persona-0.0.2/src/persona/types/archive_a_government_id_number_list_item_response_data_relationships.py
--rw-r--r--   0        0        0      824 2023-05-23 16:50:24.969419 fern_persona-0.0.2/src/persona/types/archive_a_government_id_number_list_item_response_data_relationships_creator.py
--rw-r--r--   0        0        0      739 2023-05-23 16:50:24.969419 fern_persona-0.0.2/src/persona/types/archive_a_list_response.py
--rw-r--r--   0        0        0      893 2023-05-23 16:50:24.969419 fern_persona-0.0.2/src/persona/types/archive_a_name_list_item_response.py
--rw-r--r--   0        0        0     1188 2023-05-23 16:50:24.969419 fern_persona-0.0.2/src/persona/types/archive_a_name_list_item_response_data.py
--rw-r--r--   0        0        0     1287 2023-05-23 16:50:24.969419 fern_persona-0.0.2/src/persona/types/archive_a_name_list_item_response_data_attributes.py
--rw-r--r--   0        0        0      984 2023-05-23 16:50:24.969419 fern_persona-0.0.2/src/persona/types/archive_a_name_list_item_response_data_relationships.py
--rw-r--r--   0        0        0      810 2023-05-23 16:50:24.969419 fern_persona-0.0.2/src/persona/types/archive_a_name_list_item_response_data_relationships_creator.py
--rw-r--r--   0        0        0      930 2023-05-23 16:50:24.969419 fern_persona-0.0.2/src/persona/types/archive_an_email_address_list_item_response.py
--rw-r--r--   0        0        0     1271 2023-05-23 16:50:24.969419 fern_persona-0.0.2/src/persona/types/archive_an_email_address_list_item_response_data.py
--rw-r--r--   0        0        0     1256 2023-05-23 16:50:24.969419 fern_persona-0.0.2/src/persona/types/archive_an_email_address_list_item_response_data_attributes.py
--rw-r--r--   0        0        0     1021 2023-05-23 16:50:24.969419 fern_persona-0.0.2/src/persona/types/archive_an_email_address_list_item_response_data_relationships.py
--rw-r--r--   0        0        0      819 2023-05-23 16:50:24.969419 fern_persona-0.0.2/src/persona/types/archive_an_email_address_list_item_response_data_relationships_creator.py
--rw-r--r--   0        0        0      956 2023-05-23 16:50:24.969419 fern_persona-0.0.2/src/persona/types/assign_a_case_request_meta.py
--rw-r--r--   0        0        0      855 2023-05-23 16:50:24.969419 fern_persona-0.0.2/src/persona/types/assign_a_case_response.py
--rw-r--r--   0        0        0     1121 2023-05-23 16:50:24.969419 fern_persona-0.0.2/src/persona/types/assign_a_case_response_data.py
--rw-r--r--   0        0        0     1836 2023-05-23 16:50:24.969419 fern_persona-0.0.2/src/persona/types/assign_a_case_response_data_attributes.py
--rw-r--r--   0        0        0     1871 2023-05-23 16:50:24.969419 fern_persona-0.0.2/src/persona/types/assign_a_case_response_data_relationships.py
--rw-r--r--   0        0        0      815 2023-05-23 16:50:24.969419 fern_persona-0.0.2/src/persona/types/assign_a_case_response_data_relationships_accounts.py
--rw-r--r--   0        0        0      819 2023-05-23 16:50:24.969419 fern_persona-0.0.2/src/persona/types/assign_a_case_response_data_relationships_case_comments.py
--rw-r--r--   0        0        0      984 2023-05-23 16:50:24.969419 fern_persona-0.0.2/src/persona/types/assign_a_case_response_data_relationships_case_template.py
--rw-r--r--   0        0        0      832 2023-05-23 16:50:24.969419 fern_persona-0.0.2/src/persona/types/assign_a_case_response_data_relationships_case_template_data.py
--rw-r--r--   0        0        0      997 2023-05-23 16:50:24.969419 fern_persona-0.0.2/src/persona/types/assign_a_case_response_data_relationships_inquiries.py
--rw-r--r--   0        0        0      833 2023-05-23 16:50:24.969419 fern_persona-0.0.2/src/persona/types/assign_a_case_response_data_relationships_inquiries_data_item.py
--rw-r--r--   0        0        0      989 2023-05-23 16:50:24.969419 fern_persona-0.0.2/src/persona/types/assign_a_case_response_data_relationships_reports.py
--rw-r--r--   0        0        0      831 2023-05-23 16:50:24.969419 fern_persona-0.0.2/src/persona/types/assign_a_case_response_data_relationships_reports_data_item.py
--rw-r--r--   0        0        0      999 2023-05-23 16:50:24.969419 fern_persona-0.0.2/src/persona/types/business_lookup_report_1_request_data.py
--rw-r--r--   0        0        0      954 2023-05-23 16:50:24.969419 fern_persona-0.0.2/src/persona/types/business_lookup_report_1_request_data_attributes.py
--rw-r--r--   0        0        0     1866 2023-05-23 16:50:24.969419 fern_persona-0.0.2/src/persona/types/business_lookup_report_1_request_data_attributes_query.py
--rw-r--r--   0        0        0      896 2023-05-23 16:50:24.969419 fern_persona-0.0.2/src/persona/types/business_lookup_report_1_response.py
--rw-r--r--   0        0        0      997 2023-05-23 16:50:24.969419 fern_persona-0.0.2/src/persona/types/business_lookup_report_1_response_data.py
--rw-r--r--   0        0        0     1506 2023-05-23 16:50:24.969419 fern_persona-0.0.2/src/persona/types/business_lookup_report_1_response_data_attributes.py
--rw-r--r--   0        0        0     1316 2023-05-23 16:50:24.969419 fern_persona-0.0.2/src/persona/types/business_lookup_report_1_response_data_attributes_query.py
--rw-r--r--   0        0        0     3441 2023-05-23 16:50:24.969419 fern_persona-0.0.2/src/persona/types/business_lookup_report_1_response_data_attributes_result_item.py
--rw-r--r--   0        0        0     1209 2023-05-23 16:50:24.969419 fern_persona-0.0.2/src/persona/types/business_lookup_report_1_response_data_attributes_result_item_addresses_item.py
--rw-r--r--   0        0        0     1069 2023-05-23 16:50:24.969419 fern_persona-0.0.2/src/persona/types/business_lookup_report_1_response_data_attributes_result_item_agent.py
--rw-r--r--   0        0        0     1208 2023-05-23 16:50:24.969419 fern_persona-0.0.2/src/persona/types/business_lookup_report_1_response_data_attributes_result_item_agent_address.py
--rw-r--r--   0        0        0      851 2023-05-23 16:50:24.969419 fern_persona-0.0.2/src/persona/types/business_lookup_report_1_response_data_attributes_result_item_identifiers_item.py
--rw-r--r--   0        0        0      973 2023-05-23 16:50:24.969419 fern_persona-0.0.2/src/persona/types/business_lookup_report_1_response_data_attributes_result_item_industry_codes_item.py
--rw-r--r--   0        0        0     1335 2023-05-23 16:50:24.969419 fern_persona-0.0.2/src/persona/types/business_lookup_report_1_response_data_attributes_result_item_officers_item.py
--rw-r--r--   0        0        0     1215 2023-05-23 16:50:24.969419 fern_persona-0.0.2/src/persona/types/business_lookup_report_1_response_data_attributes_result_item_officers_item_address.py
--rw-r--r--   0        0        0     1102 2023-05-23 16:50:24.969419 fern_persona-0.0.2/src/persona/types/business_lookup_report_1_response_data_attributes_result_item_registration.py
--rw-r--r--   0        0        0     1215 2023-05-23 16:50:24.969419 fern_persona-0.0.2/src/persona/types/business_lookup_report_1_response_data_attributes_result_item_registration_address.py
--rw-r--r--   0        0        0      979 2023-05-23 16:50:24.969419 fern_persona-0.0.2/src/persona/types/business_lookup_report_1_response_data_attributes_result_item_source.py
--rw-r--r--   0        0        0      988 2023-05-23 16:50:24.969419 fern_persona-0.0.2/src/persona/types/confirm_a_phone_number_verification_1_request_data.py
--rw-r--r--   0        0        0      890 2023-05-23 16:50:24.969419 fern_persona-0.0.2/src/persona/types/confirm_a_phone_number_verification_1_request_data_attributes.py
--rw-r--r--   0        0        0      942 2023-05-23 16:50:24.969419 fern_persona-0.0.2/src/persona/types/confirm_a_phone_number_verification_1_response.py
--rw-r--r--   0        0        0     1052 2023-05-23 16:50:24.969419 fern_persona-0.0.2/src/persona/types/confirm_a_phone_number_verification_1_response_data.py
--rw-r--r--   0        0        0     1778 2023-05-23 16:50:24.969419 fern_persona-0.0.2/src/persona/types/confirm_a_phone_number_verification_1_response_data_attributes.py
--rw-r--r--   0        0        0      781 2023-05-23 16:50:24.969419 fern_persona-0.0.2/src/persona/types/confirm_a_phone_number_verification_1_response_data_attributes_metadata.py
--rw-r--r--   0        0        0      983 2023-05-23 16:50:24.969419 fern_persona-0.0.2/src/persona/types/confirm_a_phone_number_verification_request_data.py
--rw-r--r--   0        0        0      889 2023-05-23 16:50:24.969419 fern_persona-0.0.2/src/persona/types/confirm_a_phone_number_verification_request_data_attributes.py
--rw-r--r--   0        0        0      937 2023-05-23 16:50:24.969419 fern_persona-0.0.2/src/persona/types/confirm_a_phone_number_verification_response.py
--rw-r--r--   0        0        0     1047 2023-05-23 16:50:24.969419 fern_persona-0.0.2/src/persona/types/confirm_a_phone_number_verification_response_data.py
--rw-r--r--   0        0        0     1849 2023-05-23 16:50:24.969419 fern_persona-0.0.2/src/persona/types/confirm_a_phone_number_verification_response_data_attributes.py
--rw-r--r--   0        0        0      780 2023-05-23 16:50:24.969419 fern_persona-0.0.2/src/persona/types/confirm_a_phone_number_verification_response_data_attributes_metadata.py
--rw-r--r--   0        0        0     1027 2023-05-23 16:50:24.969419 fern_persona-0.0.2/src/persona/types/consolidate_into_an_account_request_meta.py
--rw-r--r--   0        0        0      992 2023-05-23 16:50:24.969419 fern_persona-0.0.2/src/persona/types/create_a_browser_fingerprint_list_item_request_data.py
--rw-r--r--   0        0        0     1102 2023-05-23 16:50:24.969419 fern_persona-0.0.2/src/persona/types/create_a_browser_fingerprint_list_item_request_data_attributes.py
--rw-r--r--   0        0        0      946 2023-05-23 16:50:24.969419 fern_persona-0.0.2/src/persona/types/create_a_browser_fingerprint_list_item_response.py
--rw-r--r--   0        0        0     1299 2023-05-23 16:50:24.969419 fern_persona-0.0.2/src/persona/types/create_a_browser_fingerprint_list_item_response_data.py
--rw-r--r--   0        0        0     1193 2023-05-23 16:50:24.969419 fern_persona-0.0.2/src/persona/types/create_a_browser_fingerprint_list_item_response_data_attributes.py
--rw-r--r--   0        0        0     1037 2023-05-23 16:50:24.969419 fern_persona-0.0.2/src/persona/types/create_a_browser_fingerprint_list_item_response_data_relationships.py
--rw-r--r--   0        0        0      823 2023-05-23 16:50:24.969419 fern_persona-0.0.2/src/persona/types/create_a_browser_fingerprint_list_item_response_data_relationships_creator.py
--rw-r--r--   0        0        0      975 2023-05-23 16:50:24.969419 fern_persona-0.0.2/src/persona/types/create_a_browser_fingerprint_list_request_data.py
--rw-r--r--   0        0        0      854 2023-05-23 16:50:24.969419 fern_persona-0.0.2/src/persona/types/create_a_browser_fingerprint_list_request_data_attributes.py
--rw-r--r--   0        0        0      756 2023-05-23 16:50:24.969419 fern_persona-0.0.2/src/persona/types/create_a_browser_fingerprint_list_response.py
--rw-r--r--   0        0        0      892 2023-05-23 16:50:24.969419 fern_persona-0.0.2/src/persona/types/create_a_case_request_data.py
--rw-r--r--   0        0        0      938 2023-05-23 16:50:24.969419 fern_persona-0.0.2/src/persona/types/create_a_case_request_data_attributes.py
--rw-r--r--   0        0        0      972 2023-05-23 16:50:24.969419 fern_persona-0.0.2/src/persona/types/create_a_case_request_meta.py
--rw-r--r--   0        0        0     1013 2023-05-23 16:50:24.969419 fern_persona-0.0.2/src/persona/types/create_a_case_response.py
--rw-r--r--   0        0        0     1121 2023-05-23 16:50:24.969419 fern_persona-0.0.2/src/persona/types/create_a_case_response_data.py
--rw-r--r--   0        0        0     1857 2023-05-23 16:50:24.969419 fern_persona-0.0.2/src/persona/types/create_a_case_response_data_attributes.py
--rw-r--r--   0        0        0     1871 2023-05-23 16:50:24.969419 fern_persona-0.0.2/src/persona/types/create_a_case_response_data_relationships.py
--rw-r--r--   0        0        0      815 2023-05-23 16:50:24.969419 fern_persona-0.0.2/src/persona/types/create_a_case_response_data_relationships_accounts.py
--rw-r--r--   0        0        0      819 2023-05-23 16:50:24.969419 fern_persona-0.0.2/src/persona/types/create_a_case_response_data_relationships_case_comments.py
--rw-r--r--   0        0        0      984 2023-05-23 16:50:24.969419 fern_persona-0.0.2/src/persona/types/create_a_case_response_data_relationships_case_template.py
--rw-r--r--   0        0        0      832 2023-05-23 16:50:24.969419 fern_persona-0.0.2/src/persona/types/create_a_case_response_data_relationships_case_template_data.py
--rw-r--r--   0        0        0      997 2023-05-23 16:50:24.969419 fern_persona-0.0.2/src/persona/types/create_a_case_response_data_relationships_inquiries.py
--rw-r--r--   0        0        0      833 2023-05-23 16:50:24.969419 fern_persona-0.0.2/src/persona/types/create_a_case_response_data_relationships_inquiries_data_item.py
--rw-r--r--   0        0        0      814 2023-05-23 16:50:24.969419 fern_persona-0.0.2/src/persona/types/create_a_case_response_data_relationships_reports.py
--rw-r--r--   0        0        0     1179 2023-05-23 16:50:24.969419 fern_persona-0.0.2/src/persona/types/create_a_case_response_included_item.py
--rw-r--r--   0        0        0     1970 2023-05-23 16:50:24.969419 fern_persona-0.0.2/src/persona/types/create_a_case_response_included_item_attributes.py
--rw-r--r--   0        0        0      766 2023-05-23 16:50:24.969419 fern_persona-0.0.2/src/persona/types/create_a_case_response_included_item_attributes_fields.py
--rw-r--r--   0        0        0     2699 2023-05-23 16:50:24.969419 fern_persona-0.0.2/src/persona/types/create_a_case_response_included_item_relationships.py
--rw-r--r--   0        0        0      996 2023-05-23 16:50:24.969419 fern_persona-0.0.2/src/persona/types/create_a_case_response_included_item_relationships_account.py
--rw-r--r--   0        0        0      835 2023-05-23 16:50:24.969419 fern_persona-0.0.2/src/persona/types/create_a_case_response_included_item_relationships_account_data.py
--rw-r--r--   0        0        0     1030 2023-05-23 16:50:24.969419 fern_persona-0.0.2/src/persona/types/create_a_case_response_included_item_relationships_documents.py
--rw-r--r--   0        0        0      841 2023-05-23 16:50:24.969419 fern_persona-0.0.2/src/persona/types/create_a_case_response_included_item_relationships_documents_data_item.py
--rw-r--r--   0        0        0      824 2023-05-23 16:50:24.969419 fern_persona-0.0.2/src/persona/types/create_a_case_response_included_item_relationships_inquiry_template_version.py
--rw-r--r--   0        0        0      822 2023-05-23 16:50:24.969419 fern_persona-0.0.2/src/persona/types/create_a_case_response_included_item_relationships_reports.py
--rw-r--r--   0        0        0     1022 2023-05-23 16:50:24.969419 fern_persona-0.0.2/src/persona/types/create_a_case_response_included_item_relationships_selfies.py
--rw-r--r--   0        0        0      839 2023-05-23 16:50:24.969419 fern_persona-0.0.2/src/persona/types/create_a_case_response_included_item_relationships_selfies_data_item.py
--rw-r--r--   0        0        0     1026 2023-05-23 16:50:24.969419 fern_persona-0.0.2/src/persona/types/create_a_case_response_included_item_relationships_sessions.py
--rw-r--r--   0        0        0      840 2023-05-23 16:50:24.969419 fern_persona-0.0.2/src/persona/types/create_a_case_response_included_item_relationships_sessions_data_item.py
--rw-r--r--   0        0        0     1000 2023-05-23 16:50:24.969419 fern_persona-0.0.2/src/persona/types/create_a_case_response_included_item_relationships_template.py
--rw-r--r--   0        0        0      836 2023-05-23 16:50:24.969419 fern_persona-0.0.2/src/persona/types/create_a_case_response_included_item_relationships_template_data.py
--rw-r--r--   0        0        0     1046 2023-05-23 16:50:24.969419 fern_persona-0.0.2/src/persona/types/create_a_case_response_included_item_relationships_verifications.py
--rw-r--r--   0        0        0      845 2023-05-23 16:50:24.969419 fern_persona-0.0.2/src/persona/types/create_a_case_response_included_item_relationships_verifications_data_item.py
--rw-r--r--   0        0        0      921 2023-05-23 16:50:24.969419 fern_persona-0.0.2/src/persona/types/create_a_country_list_request_data.py
--rw-r--r--   0        0        0      843 2023-05-23 16:50:24.969419 fern_persona-0.0.2/src/persona/types/create_a_country_list_request_data_attributes.py
--rw-r--r--   0        0        0      745 2023-05-23 16:50:24.973419 fern_persona-0.0.2/src/persona/types/create_a_country_list_response.py
--rw-r--r--   0        0        0      934 2023-05-23 16:50:24.973419 fern_persona-0.0.2/src/persona/types/create_a_county_list_item_request_data.py
--rw-r--r--   0        0        0     1114 2023-05-23 16:50:24.973419 fern_persona-0.0.2/src/persona/types/create_a_county_list_item_request_data_attributes.py
--rw-r--r--   0        0        0      925 2023-05-23 16:50:24.973419 fern_persona-0.0.2/src/persona/types/create_a_database_verification_1_response.py
--rw-r--r--   0        0        0     1262 2023-05-23 16:50:24.973419 fern_persona-0.0.2/src/persona/types/create_a_database_verification_1_response_data.py
--rw-r--r--   0        0        0     1629 2023-05-23 16:50:24.973419 fern_persona-0.0.2/src/persona/types/create_a_database_verification_1_response_data_attributes.py
--rw-r--r--   0        0        0     1016 2023-05-23 16:50:24.973419 fern_persona-0.0.2/src/persona/types/create_a_database_verification_1_response_data_relationships.py
--rw-r--r--   0        0        0      818 2023-05-23 16:50:24.973419 fern_persona-0.0.2/src/persona/types/create_a_database_verification_1_response_data_relationships_inquiry.py
--rw-r--r--   0        0        0      920 2023-05-23 16:50:24.973419 fern_persona-0.0.2/src/persona/types/create_a_database_verification_response.py
--rw-r--r--   0        0        0     1244 2023-05-23 16:50:24.973419 fern_persona-0.0.2/src/persona/types/create_a_database_verification_response_data.py
--rw-r--r--   0        0        0     1649 2023-05-23 16:50:24.973419 fern_persona-0.0.2/src/persona/types/create_a_database_verification_response_data_attributes.py
--rw-r--r--   0        0        0     1011 2023-05-23 16:50:24.973419 fern_persona-0.0.2/src/persona/types/create_a_database_verification_response_data_relationships.py
--rw-r--r--   0        0        0      817 2023-05-23 16:50:24.973419 fern_persona-0.0.2/src/persona/types/create_a_database_verification_response_data_relationships_inquiry.py
--rw-r--r--   0        0        0      908 2023-05-23 16:50:24.973419 fern_persona-0.0.2/src/persona/types/create_a_document_request_data.py
--rw-r--r--   0        0        0      966 2023-05-23 16:50:24.973419 fern_persona-0.0.2/src/persona/types/create_a_document_request_data_attributes.py
--rw-r--r--   0        0        0      871 2023-05-23 16:50:24.973419 fern_persona-0.0.2/src/persona/types/create_a_document_response.py
--rw-r--r--   0        0        0     1149 2023-05-23 16:50:24.973419 fern_persona-0.0.2/src/persona/types/create_a_document_response_data.py
--rw-r--r--   0        0        0     1228 2023-05-23 16:50:24.973419 fern_persona-0.0.2/src/persona/types/create_a_document_response_data_attributes.py
--rw-r--r--   0        0        0      831 2023-05-23 16:50:24.973419 fern_persona-0.0.2/src/persona/types/create_a_document_response_data_attributes_files_item.py
--rw-r--r--   0        0        0      953 2023-05-23 16:50:24.973419 fern_persona-0.0.2/src/persona/types/create_a_document_response_data_relationships.py
--rw-r--r--   0        0        0      979 2023-05-23 16:50:24.973419 fern_persona-0.0.2/src/persona/types/create_a_document_response_data_relationships_inquiry.py
--rw-r--r--   0        0        0      831 2023-05-23 16:50:24.973419 fern_persona-0.0.2/src/persona/types/create_a_document_response_data_relationships_inquiry_data.py
--rw-r--r--   0        0        0      957 2023-05-23 16:50:24.973419 fern_persona-0.0.2/src/persona/types/create_a_document_verification_request_data.py
--rw-r--r--   0        0        0      978 2023-05-23 16:50:24.973419 fern_persona-0.0.2/src/persona/types/create_a_document_verification_request_data_attributes.py
--rw-r--r--   0        0        0      920 2023-05-23 16:50:24.973419 fern_persona-0.0.2/src/persona/types/create_a_document_verification_response.py
--rw-r--r--   0        0        0     1244 2023-05-23 16:50:24.973419 fern_persona-0.0.2/src/persona/types/create_a_document_verification_response_data.py
--rw-r--r--   0        0        0     1439 2023-05-23 16:50:24.973419 fern_persona-0.0.2/src/persona/types/create_a_document_verification_response_data_attributes.py
--rw-r--r--   0        0        0     1254 2023-05-23 16:50:24.973419 fern_persona-0.0.2/src/persona/types/create_a_document_verification_response_data_relationships.py
--rw-r--r--   0        0        0     1032 2023-05-23 16:50:24.973419 fern_persona-0.0.2/src/persona/types/create_a_document_verification_response_data_relationships_document.py
--rw-r--r--   0        0        0      844 2023-05-23 16:50:24.973419 fern_persona-0.0.2/src/persona/types/create_a_document_verification_response_data_relationships_document_data.py
--rw-r--r--   0        0        0     1028 2023-05-23 16:50:24.973419 fern_persona-0.0.2/src/persona/types/create_a_document_verification_response_data_relationships_inquiry.py
--rw-r--r--   0        0        0      843 2023-05-23 16:50:24.973419 fern_persona-0.0.2/src/persona/types/create_a_document_verification_response_data_relationships_inquiry_data.py
--rw-r--r--   0        0        0      926 2023-05-23 16:50:24.973419 fern_persona-0.0.2/src/persona/types/create_a_face_list_item_request_data.py
--rw-r--r--   0        0        0     1220 2023-05-23 16:50:24.973419 fern_persona-0.0.2/src/persona/types/create_a_face_list_item_request_data_attributes.py
--rw-r--r--   0        0        0      940 2023-05-23 16:50:24.973419 fern_persona-0.0.2/src/persona/types/create_a_face_list_item_request_data_attributes_face_photo.py
--rw-r--r--   0        0        0      909 2023-05-23 16:50:24.973419 fern_persona-0.0.2/src/persona/types/create_a_face_list_request_data.py
--rw-r--r--   0        0        0      840 2023-05-23 16:50:24.973419 fern_persona-0.0.2/src/persona/types/create_a_face_list_request_data_attributes.py
--rw-r--r--   0        0        0      742 2023-05-23 16:50:24.973419 fern_persona-0.0.2/src/persona/types/create_a_face_list_response.py
--rw-r--r--   0        0        0      954 2023-05-23 16:50:24.973419 fern_persona-0.0.2/src/persona/types/create_a_geolocation_list_item_request_data.py
--rw-r--r--   0        0        0     1401 2023-05-23 16:50:24.973419 fern_persona-0.0.2/src/persona/types/create_a_geolocation_list_item_request_data_attributes.py
--rw-r--r--   0        0        0      917 2023-05-23 16:50:24.973419 fern_persona-0.0.2/src/persona/types/create_a_geolocation_list_item_response.py
--rw-r--r--   0        0        0     1239 2023-05-23 16:50:24.973419 fern_persona-0.0.2/src/persona/types/create_a_geolocation_list_item_response_data.py
--rw-r--r--   0        0        0     1309 2023-05-23 16:50:24.973419 fern_persona-0.0.2/src/persona/types/create_a_geolocation_list_item_response_data_attributes.py
--rw-r--r--   0        0        0     1008 2023-05-23 16:50:24.973419 fern_persona-0.0.2/src/persona/types/create_a_geolocation_list_item_response_data_relationships.py
--rw-r--r--   0        0        0      816 2023-05-23 16:50:24.973419 fern_persona-0.0.2/src/persona/types/create_a_geolocation_list_item_response_data_relationships_creator.py
--rw-r--r--   0        0        0      937 2023-05-23 16:50:24.973419 fern_persona-0.0.2/src/persona/types/create_a_geolocation_list_request_data.py
--rw-r--r--   0        0        0      847 2023-05-23 16:50:24.973419 fern_persona-0.0.2/src/persona/types/create_a_geolocation_list_request_data_attributes.py
--rw-r--r--   0        0        0      749 2023-05-23 16:50:24.973419 fern_persona-0.0.2/src/persona/types/create_a_geolocation_list_response.py
--rw-r--r--   0        0        0      946 2023-05-23 16:50:24.973419 fern_persona-0.0.2/src/persona/types/create_a_gov_id_verification_request_data.py
--rw-r--r--   0        0        0     2143 2023-05-23 16:50:24.973419 fern_persona-0.0.2/src/persona/types/create_a_gov_id_verification_request_data_attributes.py
--rw-r--r--   0        0        0     1341 2023-05-23 16:50:24.973419 fern_persona-0.0.2/src/persona/types/create_a_gov_id_verification_request_data_attributes_back_photo.py
--rw-r--r--   0        0        0     1164 2023-05-23 16:50:24.973419 fern_persona-0.0.2/src/persona/types/create_a_gov_id_verification_request_data_attributes_back_photo_data.py
--rw-r--r--   0        0        0     1346 2023-05-23 16:50:24.973419 fern_persona-0.0.2/src/persona/types/create_a_gov_id_verification_request_data_attributes_front_photo.py
--rw-r--r--   0        0        0     1165 2023-05-23 16:50:24.973419 fern_persona-0.0.2/src/persona/types/create_a_gov_id_verification_request_data_attributes_front_photo_data.py
--rw-r--r--   0        0        0      909 2023-05-23 16:50:24.973419 fern_persona-0.0.2/src/persona/types/create_a_gov_id_verification_response.py
--rw-r--r--   0        0        0     1216 2023-05-23 16:50:24.973419 fern_persona-0.0.2/src/persona/types/create_a_gov_id_verification_response_data.py
--rw-r--r--   0        0        0     2562 2023-05-23 16:50:24.973419 fern_persona-0.0.2/src/persona/types/create_a_gov_id_verification_response_data_attributes.py
--rw-r--r--   0        0        0     1235 2023-05-23 16:50:24.973419 fern_persona-0.0.2/src/persona/types/create_a_gov_id_verification_response_data_relationships.py
--rw-r--r--   0        0        0     1021 2023-05-23 16:50:24.973419 fern_persona-0.0.2/src/persona/types/create_a_gov_id_verification_response_data_relationships_document.py
--rw-r--r--   0        0        0      841 2023-05-23 16:50:24.973419 fern_persona-0.0.2/src/persona/types/create_a_gov_id_verification_response_data_relationships_document_data.py
--rw-r--r--   0        0        0      814 2023-05-23 16:50:24.973419 fern_persona-0.0.2/src/persona/types/create_a_gov_id_verification_response_data_relationships_inquiry.py
--rw-r--r--   0        0        0      958 2023-05-23 16:50:24.973419 fern_persona-0.0.2/src/persona/types/create_a_government_id_document_request_data.py
--rw-r--r--   0        0        0     1767 2023-05-23 16:50:24.973419 fern_persona-0.0.2/src/persona/types/create_a_government_id_document_request_data_attributes.py
--rw-r--r--   0        0        0     1353 2023-05-23 16:50:24.973419 fern_persona-0.0.2/src/persona/types/create_a_government_id_document_request_data_attributes_back_photo.py
--rw-r--r--   0        0        0     1167 2023-05-23 16:50:24.973419 fern_persona-0.0.2/src/persona/types/create_a_government_id_document_request_data_attributes_back_photo_data.py
--rw-r--r--   0        0        0     1358 2023-05-23 16:50:24.973419 fern_persona-0.0.2/src/persona/types/create_a_government_id_document_request_data_attributes_front_photo.py
--rw-r--r--   0        0        0     1168 2023-05-23 16:50:24.973419 fern_persona-0.0.2/src/persona/types/create_a_government_id_document_request_data_attributes_front_photo_data.py
--rw-r--r--   0        0        0      921 2023-05-23 16:50:24.973419 fern_persona-0.0.2/src/persona/types/create_a_government_id_document_response.py
--rw-r--r--   0        0        0     1246 2023-05-23 16:50:24.977419 fern_persona-0.0.2/src/persona/types/create_a_government_id_document_response_data.py
--rw-r--r--   0        0        0     2186 2023-05-23 16:50:24.977419 fern_persona-0.0.2/src/persona/types/create_a_government_id_document_response_data_attributes.py
--rw-r--r--   0        0        0     1012 2023-05-23 16:50:24.977419 fern_persona-0.0.2/src/persona/types/create_a_government_id_document_response_data_relationships.py
--rw-r--r--   0        0        0     1029 2023-05-23 16:50:24.977419 fern_persona-0.0.2/src/persona/types/create_a_government_id_document_response_data_relationships_inquiry.py
--rw-r--r--   0        0        0      843 2023-05-23 16:50:24.977419 fern_persona-0.0.2/src/persona/types/create_a_government_id_document_response_data_relationships_inquiry_data.py
--rw-r--r--   0        0        0      993 2023-05-23 16:50:24.977419 fern_persona-0.0.2/src/persona/types/create_a_government_id_number_list_item_request_data.py
--rw-r--r--   0        0        0     1305 2023-05-23 16:50:24.977419 fern_persona-0.0.2/src/persona/types/create_a_government_id_number_list_item_request_data_attributes.py
--rw-r--r--   0        0        0      947 2023-05-23 16:50:24.977419 fern_persona-0.0.2/src/persona/types/create_a_government_id_number_list_item_response.py
--rw-r--r--   0        0        0     1301 2023-05-23 16:50:24.977419 fern_persona-0.0.2/src/persona/types/create_a_government_id_number_list_item_response_data.py
--rw-r--r--   0        0        0     1303 2023-05-23 16:50:24.977419 fern_persona-0.0.2/src/persona/types/create_a_government_id_number_list_item_response_data_attributes.py
--rw-r--r--   0        0        0     1038 2023-05-23 16:50:24.977419 fern_persona-0.0.2/src/persona/types/create_a_government_id_number_list_item_response_data_relationships.py
--rw-r--r--   0        0        0      823 2023-05-23 16:50:24.977419 fern_persona-0.0.2/src/persona/types/create_a_government_id_number_list_item_response_data_relationships_creator.py
--rw-r--r--   0        0        0      976 2023-05-23 16:50:24.977419 fern_persona-0.0.2/src/persona/types/create_a_government_id_number_list_request_data.py
--rw-r--r--   0        0        0      854 2023-05-23 16:50:24.977419 fern_persona-0.0.2/src/persona/types/create_a_government_id_number_list_request_data_attributes.py
--rw-r--r--   0        0        0      756 2023-05-23 16:50:24.977419 fern_persona-0.0.2/src/persona/types/create_a_government_id_number_list_response.py
--rw-r--r--   0        0        0      917 2023-05-23 16:50:24.977419 fern_persona-0.0.2/src/persona/types/create_a_graph_query_request_data.py
--rw-r--r--   0        0        0     1146 2023-05-23 16:50:24.977419 fern_persona-0.0.2/src/persona/types/create_a_graph_query_request_data_attributes.py
--rw-r--r--   0        0        0     1295 2023-05-23 16:50:24.977419 fern_persona-0.0.2/src/persona/types/create_a_graph_query_request_data_attributes_variable_map.py
--rw-r--r--   0        0        0      926 2023-05-23 16:50:24.977419 fern_persona-0.0.2/src/persona/types/create_a_name_list_item_request_data.py
--rw-r--r--   0        0        0     1266 2023-05-23 16:50:24.977419 fern_persona-0.0.2/src/persona/types/create_a_name_list_item_request_data_attributes.py
--rw-r--r--   0        0        0      889 2023-05-23 16:50:24.977419 fern_persona-0.0.2/src/persona/types/create_a_name_list_item_response.py
--rw-r--r--   0        0        0     1181 2023-05-23 16:50:24.977419 fern_persona-0.0.2/src/persona/types/create_a_name_list_item_response_data.py
--rw-r--r--   0        0        0     1293 2023-05-23 16:50:24.977419 fern_persona-0.0.2/src/persona/types/create_a_name_list_item_response_data_attributes.py
--rw-r--r--   0        0        0      980 2023-05-23 16:50:24.977419 fern_persona-0.0.2/src/persona/types/create_a_name_list_item_response_data_relationships.py
--rw-r--r--   0        0        0      809 2023-05-23 16:50:24.977419 fern_persona-0.0.2/src/persona/types/create_a_name_list_item_response_data_relationships_creator.py
--rw-r--r--   0        0        0      909 2023-05-23 16:50:24.977419 fern_persona-0.0.2/src/persona/types/create_a_name_list_request_data.py
--rw-r--r--   0        0        0     1098 2023-05-23 16:50:24.977419 fern_persona-0.0.2/src/persona/types/create_a_name_list_request_data_attributes.py
--rw-r--r--   0        0        0      742 2023-05-23 16:50:24.977419 fern_persona-0.0.2/src/persona/types/create_a_name_list_response.py
--rw-r--r--   0        0        0     2149 2023-05-23 16:50:24.977419 fern_persona-0.0.2/src/persona/types/create_a_phone_carrier_database_verification_request_attributes.py
--rw-r--r--   0        0        0      979 2023-05-23 16:50:24.977419 fern_persona-0.0.2/src/persona/types/create_a_phone_carrier_database_verification_response.py
--rw-r--r--   0        0        0     1341 2023-05-23 16:50:24.977419 fern_persona-0.0.2/src/persona/types/create_a_phone_carrier_database_verification_response_data.py
--rw-r--r--   0        0        0     1571 2023-05-23 16:50:24.977419 fern_persona-0.0.2/src/persona/types/create_a_phone_carrier_database_verification_response_data_attributes.py
--rw-r--r--   0        0        0     1061 2023-05-23 16:50:24.977419 fern_persona-0.0.2/src/persona/types/create_a_phone_carrier_database_verification_response_data_relationships.py
--rw-r--r--   0        0        0      829 2023-05-23 16:50:24.977419 fern_persona-0.0.2/src/persona/types/create_a_phone_carrier_database_verification_response_data_relationships_inquiry.py
--rw-r--r--   0        0        0      955 2023-05-23 16:50:24.977419 fern_persona-0.0.2/src/persona/types/create_a_phone_number_list_item_request_data.py
--rw-r--r--   0        0        0     1065 2023-05-23 16:50:24.977419 fern_persona-0.0.2/src/persona/types/create_a_phone_number_list_item_request_data_attributes.py
--rw-r--r--   0        0        0      938 2023-05-23 16:50:24.977419 fern_persona-0.0.2/src/persona/types/create_a_phone_number_list_request_data.py
--rw-r--r--   0        0        0      847 2023-05-23 16:50:24.977419 fern_persona-0.0.2/src/persona/types/create_a_phone_number_list_request_data_attributes.py
--rw-r--r--   0        0        0      749 2023-05-23 16:50:24.977419 fern_persona-0.0.2/src/persona/types/create_a_phone_number_list_response.py
--rw-r--r--   0        0        0      979 2023-05-23 16:50:24.977419 fern_persona-0.0.2/src/persona/types/create_a_phone_number_verification_request_data.py
--rw-r--r--   0        0        0     1485 2023-05-23 16:50:24.977419 fern_persona-0.0.2/src/persona/types/create_a_phone_number_verification_request_data_attributes.py
--rw-r--r--   0        0        0      933 2023-05-23 16:50:24.977419 fern_persona-0.0.2/src/persona/types/create_a_phone_number_verification_response.py
--rw-r--r--   0        0        0     1043 2023-05-23 16:50:24.977419 fern_persona-0.0.2/src/persona/types/create_a_phone_number_verification_response_data.py
--rw-r--r--   0        0        0     1845 2023-05-23 16:50:24.977419 fern_persona-0.0.2/src/persona/types/create_a_phone_number_verification_response_data_attributes.py
--rw-r--r--   0        0        0      779 2023-05-23 16:50:24.977419 fern_persona-0.0.2/src/persona/types/create_a_phone_number_verification_response_data_attributes_metadata.py
--rw-r--r--   0        0        0      900 2023-05-23 16:50:24.977419 fern_persona-0.0.2/src/persona/types/create_a_report_request_data.py
--rw-r--r--   0        0        0     2563 2023-05-23 16:50:24.977419 fern_persona-0.0.2/src/persona/types/create_a_report_request_data_attributes.py
--rw-r--r--   0        0        0      949 2023-05-23 16:50:24.977419 fern_persona-0.0.2/src/persona/types/create_a_selfie_verification_request_data.py
--rw-r--r--   0        0        0     2190 2023-05-23 16:50:24.977419 fern_persona-0.0.2/src/persona/types/create_a_selfie_verification_request_data_attributes.py
--rw-r--r--   0        0        0     1077 2023-05-23 16:50:24.977419 fern_persona-0.0.2/src/persona/types/create_a_selfie_verification_request_data_attributes_center_photo.py
--rw-r--r--   0        0        0      920 2023-05-23 16:50:24.977419 fern_persona-0.0.2/src/persona/types/create_a_selfie_verification_request_data_attributes_center_photo_data.py
--rw-r--r--   0        0        0     1067 2023-05-23 16:50:24.977419 fern_persona-0.0.2/src/persona/types/create_a_selfie_verification_request_data_attributes_left_photo.py
--rw-r--r--   0        0        0      918 2023-05-23 16:50:24.977419 fern_persona-0.0.2/src/persona/types/create_a_selfie_verification_request_data_attributes_left_photo_data.py
--rw-r--r--   0        0        0     1072 2023-05-23 16:50:24.977419 fern_persona-0.0.2/src/persona/types/create_a_selfie_verification_request_data_attributes_right_photo.py
--rw-r--r--   0        0        0      919 2023-05-23 16:50:24.977419 fern_persona-0.0.2/src/persona/types/create_a_selfie_verification_request_data_attributes_right_photo_data.py
--rw-r--r--   0        0        0      912 2023-05-23 16:50:24.977419 fern_persona-0.0.2/src/persona/types/create_a_selfie_verification_response.py
--rw-r--r--   0        0        0     1221 2023-05-23 16:50:24.977419 fern_persona-0.0.2/src/persona/types/create_a_selfie_verification_response_data.py
--rw-r--r--   0        0        0     2064 2023-05-23 16:50:24.977419 fern_persona-0.0.2/src/persona/types/create_a_selfie_verification_response_data_attributes.py
--rw-r--r--   0        0        0     1003 2023-05-23 16:50:24.977419 fern_persona-0.0.2/src/persona/types/create_a_selfie_verification_response_data_relationships.py
--rw-r--r--   0        0        0      815 2023-05-23 16:50:24.977419 fern_persona-0.0.2/src/persona/types/create_a_selfie_verification_response_data_relationships_inquiry.py
--rw-r--r--   0        0        0      769 2023-05-23 16:50:24.977419 fern_persona-0.0.2/src/persona/types/create_a_serpro_database_verification_request_attributes.py
--rw-r--r--   0        0        0      945 2023-05-23 16:50:24.977419 fern_persona-0.0.2/src/persona/types/create_a_serpro_database_verification_response.py
--rw-r--r--   0        0        0     1297 2023-05-23 16:50:24.977419 fern_persona-0.0.2/src/persona/types/create_a_serpro_database_verification_response_data.py
--rw-r--r--   0        0        0     1565 2023-05-23 16:50:24.977419 fern_persona-0.0.2/src/persona/types/create_a_serpro_database_verification_response_data_attributes.py
--rw-r--r--   0        0        0     1290 2023-05-23 16:50:24.977419 fern_persona-0.0.2/src/persona/types/create_a_serpro_database_verification_response_data_relationships.py
--rw-r--r--   0        0        0      823 2023-05-23 16:50:24.977419 fern_persona-0.0.2/src/persona/types/create_a_serpro_database_verification_response_data_relationships_inquiry.py
--rw-r--r--   0        0        0      822 2023-05-23 16:50:24.977419 fern_persona-0.0.2/src/persona/types/create_a_serpro_database_verification_response_data_relationships_selfie.py
--rw-r--r--   0        0        0      983 2023-05-23 16:50:24.977419 fern_persona-0.0.2/src/persona/types/create_a_tin_database_verifications_request_data.py
--rw-r--r--   0        0        0     1634 2023-05-23 16:50:24.977419 fern_persona-0.0.2/src/persona/types/create_a_tin_database_verifications_request_data_attributes.py
--rw-r--r--   0        0        0      937 2023-05-23 16:50:24.977419 fern_persona-0.0.2/src/persona/types/create_a_tin_database_verifications_response.py
--rw-r--r--   0        0        0     1283 2023-05-23 16:50:24.977419 fern_persona-0.0.2/src/persona/types/create_a_tin_database_verifications_response_data.py
--rw-r--r--   0        0        0     1563 2023-05-23 16:50:24.977419 fern_persona-0.0.2/src/persona/types/create_a_tin_database_verifications_response_data_attributes.py
--rw-r--r--   0        0        0     1028 2023-05-23 16:50:24.977419 fern_persona-0.0.2/src/persona/types/create_a_tin_database_verifications_response_data_relationships.py
--rw-r--r--   0        0        0      821 2023-05-23 16:50:24.977419 fern_persona-0.0.2/src/persona/types/create_a_tin_database_verifications_response_data_relationships_inquiry.py
--rw-r--r--   0        0        0     1126 2023-05-23 16:50:24.977419 fern_persona-0.0.2/src/persona/types/create_a_workflow_run_request_data.py
--rw-r--r--   0        0        0     1429 2023-05-23 16:50:24.977419 fern_persona-0.0.2/src/persona/types/create_a_workflow_run_request_data_attributes.py
--rw-r--r--   0        0        0      884 2023-05-23 16:50:24.977419 fern_persona-0.0.2/src/persona/types/create_a_workflow_run_response.py
--rw-r--r--   0        0        0     1172 2023-05-23 16:50:24.977419 fern_persona-0.0.2/src/persona/types/create_a_workflow_run_response_data.py
--rw-r--r--   0        0        0      998 2023-05-23 16:50:24.977419 fern_persona-0.0.2/src/persona/types/create_a_workflow_run_response_data_attributes.py
--rw-r--r--   0        0        0     1540 2023-05-23 16:50:24.977419 fern_persona-0.0.2/src/persona/types/create_a_workflow_run_response_data_relationships.py
--rw-r--r--   0        0        0      808 2023-05-23 16:50:24.977419 fern_persona-0.0.2/src/persona/types/create_a_workflow_run_response_data_relationships_creator.py
--rw-r--r--   0        0        0      996 2023-05-23 16:50:24.977419 fern_persona-0.0.2/src/persona/types/create_a_workflow_run_response_data_relationships_workflow.py
--rw-r--r--   0        0        0      835 2023-05-23 16:50:24.977419 fern_persona-0.0.2/src/persona/types/create_a_workflow_run_response_data_relationships_workflow_data.py
--rw-r--r--   0        0        0     1025 2023-05-23 16:50:24.977419 fern_persona-0.0.2/src/persona/types/create_a_workflow_run_response_data_relationships_workflow_version.py
--rw-r--r--   0        0        0      842 2023-05-23 16:50:24.977419 fern_persona-0.0.2/src/persona/types/create_a_workflow_run_response_data_relationships_workflow_version_data.py
--rw-r--r--   0        0        0      908 2023-05-23 16:50:24.977419 fern_persona-0.0.2/src/persona/types/create_an_account_request_data.py
--rw-r--r--   0        0        0     3575 2023-05-23 16:50:24.977419 fern_persona-0.0.2/src/persona/types/create_an_account_request_data_attributes.py
--rw-r--r--   0        0        0     1231 2023-05-23 16:50:24.977419 fern_persona-0.0.2/src/persona/types/create_an_account_request_data_attributes_selfie_photo.py
--rw-r--r--   0        0        0     1113 2023-05-23 16:50:24.977419 fern_persona-0.0.2/src/persona/types/create_an_account_request_data_attributes_selfie_photo_data.py
--rw-r--r--   0        0        0      871 2023-05-23 16:50:24.977419 fern_persona-0.0.2/src/persona/types/create_an_account_response.py
--rw-r--r--   0        0        0      972 2023-05-23 16:50:24.977419 fern_persona-0.0.2/src/persona/types/create_an_account_response_data.py
--rw-r--r--   0        0        0     1029 2023-05-23 16:50:24.977419 fern_persona-0.0.2/src/persona/types/create_an_account_response_data_attributes.py
--rw-r--r--   0        0        0      905 2023-05-23 16:50:24.977419 fern_persona-0.0.2/src/persona/types/create_an_api_key_request_data.py
--rw-r--r--   0        0        0     1804 2023-05-23 16:50:24.977419 fern_persona-0.0.2/src/persona/types/create_an_api_key_request_data_attributes.py
--rw-r--r--   0        0        0      868 2023-05-23 16:50:24.977419 fern_persona-0.0.2/src/persona/types/create_an_api_key_response.py
--rw-r--r--   0        0        0      969 2023-05-23 16:50:24.977419 fern_persona-0.0.2/src/persona/types/create_an_api_key_response_data.py
--rw-r--r--   0        0        0     1582 2023-05-23 16:50:24.977419 fern_persona-0.0.2/src/persona/types/create_an_api_key_response_data_attributes.py
--rw-r--r--   0        0        0      963 2023-05-23 16:50:24.977419 fern_persona-0.0.2/src/persona/types/create_an_email_address_list_item_request_data.py
--rw-r--r--   0        0        0     1228 2023-05-23 16:50:24.977419 fern_persona-0.0.2/src/persona/types/create_an_email_address_list_item_request_data_attributes.py
--rw-r--r--   0        0        0      926 2023-05-23 16:50:24.977419 fern_persona-0.0.2/src/persona/types/create_an_email_address_list_item_response.py
--rw-r--r--   0        0        0     1264 2023-05-23 16:50:24.977419 fern_persona-0.0.2/src/persona/types/create_an_email_address_list_item_response_data.py
--rw-r--r--   0        0        0     1262 2023-05-23 16:50:24.977419 fern_persona-0.0.2/src/persona/types/create_an_email_address_list_item_response_data_attributes.py
--rw-r--r--   0        0        0     1017 2023-05-23 16:50:24.977419 fern_persona-0.0.2/src/persona/types/create_an_email_address_list_item_response_data_relationships.py
--rw-r--r--   0        0        0      818 2023-05-23 16:50:24.977419 fern_persona-0.0.2/src/persona/types/create_an_email_address_list_item_response_data_relationships_creator.py
--rw-r--r--   0        0        0      946 2023-05-23 16:50:24.977419 fern_persona-0.0.2/src/persona/types/create_an_email_address_list_request_data.py
--rw-r--r--   0        0        0      849 2023-05-23 16:50:24.977419 fern_persona-0.0.2/src/persona/types/create_an_email_address_list_request_data_attributes.py
--rw-r--r--   0        0        0      751 2023-05-23 16:50:24.977419 fern_persona-0.0.2/src/persona/types/create_an_email_address_list_response.py
--rw-r--r--   0        0        0      987 2023-05-23 16:50:24.977419 fern_persona-0.0.2/src/persona/types/create_an_email_address_verification_request_data.py
--rw-r--r--   0        0        0     1487 2023-05-23 16:50:24.977419 fern_persona-0.0.2/src/persona/types/create_an_email_address_verification_request_data_attributes.py
--rw-r--r--   0        0        0      941 2023-05-23 16:50:24.977419 fern_persona-0.0.2/src/persona/types/create_an_email_address_verification_response.py
--rw-r--r--   0        0        0     1051 2023-05-23 16:50:24.977419 fern_persona-0.0.2/src/persona/types/create_an_email_address_verification_response_data.py
--rw-r--r--   0        0        0     1855 2023-05-23 16:50:24.977419 fern_persona-0.0.2/src/persona/types/create_an_email_address_verification_response_data_attributes.py
--rw-r--r--   0        0        0      781 2023-05-23 16:50:24.977419 fern_persona-0.0.2/src/persona/types/create_an_email_address_verification_response_data_attributes_metadata.py
--rw-r--r--   0        0        0      908 2023-05-23 16:50:24.977419 fern_persona-0.0.2/src/persona/types/create_an_inquiry_request_data.py
--rw-r--r--   0        0        0     3293 2023-05-23 16:50:24.977419 fern_persona-0.0.2/src/persona/types/create_an_inquiry_request_data_attributes.py
--rw-r--r--   0        0        0     2262 2023-05-23 16:50:24.977419 fern_persona-0.0.2/src/persona/types/create_an_inquiry_request_data_attributes_fields.py
--rw-r--r--   0        0        0      871 2023-05-23 16:50:24.977419 fern_persona-0.0.2/src/persona/types/create_an_inquiry_response.py
--rw-r--r--   0        0        0     1149 2023-05-23 16:50:24.977419 fern_persona-0.0.2/src/persona/types/create_an_inquiry_response_data.py
--rw-r--r--   0        0        0     1202 2023-05-23 16:50:24.977419 fern_persona-0.0.2/src/persona/types/create_an_inquiry_response_data_attributes.py
--rw-r--r--   0        0        0     1569 2023-05-23 16:50:24.977419 fern_persona-0.0.2/src/persona/types/create_an_inquiry_response_data_relationships.py
--rw-r--r--   0        0        0      979 2023-05-23 16:50:24.977419 fern_persona-0.0.2/src/persona/types/create_an_inquiry_response_data_relationships_account.py
--rw-r--r--   0        0        0      831 2023-05-23 16:50:24.977419 fern_persona-0.0.2/src/persona/types/create_an_inquiry_response_data_relationships_account_data.py
--rw-r--r--   0        0        0      818 2023-05-23 16:50:24.977419 fern_persona-0.0.2/src/persona/types/create_an_inquiry_response_data_relationships_reports.py
--rw-r--r--   0        0        0      983 2023-05-23 16:50:24.977419 fern_persona-0.0.2/src/persona/types/create_an_inquiry_response_data_relationships_template.py
--rw-r--r--   0        0        0      832 2023-05-23 16:50:24.977419 fern_persona-0.0.2/src/persona/types/create_an_inquiry_response_data_relationships_template_data.py
--rw-r--r--   0        0        0     1029 2023-05-23 16:50:24.977419 fern_persona-0.0.2/src/persona/types/create_an_inquiry_response_data_relationships_verifications.py
--rw-r--r--   0        0        0      841 2023-05-23 16:50:24.977419 fern_persona-0.0.2/src/persona/types/create_an_inquiry_response_data_relationships_verifications_data_item.py
--rw-r--r--   0        0        0      951 2023-05-23 16:50:24.977419 fern_persona-0.0.2/src/persona/types/create_an_ip_address_list_item_request_data.py
--rw-r--r--   0        0        0     1098 2023-05-23 16:50:24.981420 fern_persona-0.0.2/src/persona/types/create_an_ip_address_list_item_request_data_attributes.py
--rw-r--r--   0        0        0      934 2023-05-23 16:50:24.981420 fern_persona-0.0.2/src/persona/types/create_an_ip_address_list_request_data.py
--rw-r--r--   0        0        0      846 2023-05-23 16:50:24.981420 fern_persona-0.0.2/src/persona/types/create_an_ip_address_list_request_data_attributes.py
--rw-r--r--   0        0        0      748 2023-05-23 16:50:24.981420 fern_persona-0.0.2/src/persona/types/create_an_ip_address_list_response.py
--rw-r--r--   0        0        0      848 2023-05-23 16:50:24.981420 fern_persona-0.0.2/src/persona/types/decline_an_inquiry_request_meta.py
--rw-r--r--   0        0        0      875 2023-05-23 16:50:24.981420 fern_persona-0.0.2/src/persona/types/decline_an_inquiry_response.py
--rw-r--r--   0        0        0     1156 2023-05-23 16:50:24.981420 fern_persona-0.0.2/src/persona/types/decline_an_inquiry_response_data.py
--rw-r--r--   0        0        0     1196 2023-05-23 16:50:24.981420 fern_persona-0.0.2/src/persona/types/decline_an_inquiry_response_data_attributes.py
--rw-r--r--   0        0        0     1582 2023-05-23 16:50:24.981420 fern_persona-0.0.2/src/persona/types/decline_an_inquiry_response_data_relationships.py
--rw-r--r--   0        0        0      983 2023-05-23 16:50:24.981420 fern_persona-0.0.2/src/persona/types/decline_an_inquiry_response_data_relationships_account.py
--rw-r--r--   0        0        0      832 2023-05-23 16:50:24.981420 fern_persona-0.0.2/src/persona/types/decline_an_inquiry_response_data_relationships_account_data.py
--rw-r--r--   0        0        0      819 2023-05-23 16:50:24.981420 fern_persona-0.0.2/src/persona/types/decline_an_inquiry_response_data_relationships_reports.py
--rw-r--r--   0        0        0      987 2023-05-23 16:50:24.981420 fern_persona-0.0.2/src/persona/types/decline_an_inquiry_response_data_relationships_template.py
--rw-r--r--   0        0        0      833 2023-05-23 16:50:24.981420 fern_persona-0.0.2/src/persona/types/decline_an_inquiry_response_data_relationships_template_data.py
--rw-r--r--   0        0        0     1033 2023-05-23 16:50:24.981420 fern_persona-0.0.2/src/persona/types/decline_an_inquiry_response_data_relationships_verifications.py
--rw-r--r--   0        0        0      842 2023-05-23 16:50:24.981420 fern_persona-0.0.2/src/persona/types/decline_an_inquiry_response_data_relationships_verifications_data_item.py
--rw-r--r--   0        0        0      903 2023-05-23 16:50:24.981420 fern_persona-0.0.2/src/persona/types/dismiss_matches_request_data.py
--rw-r--r--   0        0        0     1622 2023-05-23 16:50:24.981420 fern_persona-0.0.2/src/persona/types/dismiss_matches_request_data_attributes.py
--rw-r--r--   0        0        0      780 2023-05-23 16:50:24.981420 fern_persona-0.0.2/src/persona/types/dismiss_matches_request_data_attributes_dismiss_type.py
--rw-r--r--   0        0        0      866 2023-05-23 16:50:24.981420 fern_persona-0.0.2/src/persona/types/dismiss_matches_response.py
--rw-r--r--   0        0        0     1140 2023-05-23 16:50:24.981420 fern_persona-0.0.2/src/persona/types/dismiss_matches_response_data.py
--rw-r--r--   0        0        0     1271 2023-05-23 16:50:24.981420 fern_persona-0.0.2/src/persona/types/dismiss_matches_response_data_attributes.py
--rw-r--r--   0        0        0     1467 2023-05-23 16:50:24.981420 fern_persona-0.0.2/src/persona/types/dismiss_matches_response_data_relationships.py
--rw-r--r--   0        0        0      804 2023-05-23 16:50:24.981420 fern_persona-0.0.2/src/persona/types/dismiss_matches_response_data_relationships_account.py
--rw-r--r--   0        0        0      804 2023-05-23 16:50:24.981420 fern_persona-0.0.2/src/persona/types/dismiss_matches_response_data_relationships_inquiry.py
--rw-r--r--   0        0        0     1003 2023-05-23 16:50:24.981420 fern_persona-0.0.2/src/persona/types/dismiss_matches_response_data_relationships_report_template.py
--rw-r--r--   0        0        0      837 2023-05-23 16:50:24.981420 fern_persona-0.0.2/src/persona/types/dismiss_matches_response_data_relationships_report_template_data.py
--rw-r--r--   0        0        0      959 2023-05-23 16:50:24.981420 fern_persona-0.0.2/src/persona/types/expire_an_api_key_request_meta.py
--rw-r--r--   0        0        0      868 2023-05-23 16:50:24.981420 fern_persona-0.0.2/src/persona/types/expire_an_api_key_response.py
--rw-r--r--   0        0        0      969 2023-05-23 16:50:24.981420 fern_persona-0.0.2/src/persona/types/expire_an_api_key_response_data.py
--rw-r--r--   0        0        0     1582 2023-05-23 16:50:24.981420 fern_persona-0.0.2/src/persona/types/expire_an_api_key_response_data_attributes.py
--rw-r--r--   0        0        0      871 2023-05-23 16:50:24.981420 fern_persona-0.0.2/src/persona/types/expire_an_inquiry_response.py
--rw-r--r--   0        0        0     1149 2023-05-23 16:50:24.981420 fern_persona-0.0.2/src/persona/types/expire_an_inquiry_response_data.py
--rw-r--r--   0        0        0     1195 2023-05-23 16:50:24.981420 fern_persona-0.0.2/src/persona/types/expire_an_inquiry_response_data_attributes.py
--rw-r--r--   0        0        0     1569 2023-05-23 16:50:24.981420 fern_persona-0.0.2/src/persona/types/expire_an_inquiry_response_data_relationships.py
--rw-r--r--   0        0        0      979 2023-05-23 16:50:24.981420 fern_persona-0.0.2/src/persona/types/expire_an_inquiry_response_data_relationships_account.py
--rw-r--r--   0        0        0      831 2023-05-23 16:50:24.981420 fern_persona-0.0.2/src/persona/types/expire_an_inquiry_response_data_relationships_account_data.py
--rw-r--r--   0        0        0      818 2023-05-23 16:50:24.981420 fern_persona-0.0.2/src/persona/types/expire_an_inquiry_response_data_relationships_reports.py
--rw-r--r--   0        0        0      983 2023-05-23 16:50:24.981420 fern_persona-0.0.2/src/persona/types/expire_an_inquiry_response_data_relationships_template.py
--rw-r--r--   0        0        0      832 2023-05-23 16:50:24.981420 fern_persona-0.0.2/src/persona/types/expire_an_inquiry_response_data_relationships_template_data.py
--rw-r--r--   0        0        0     1029 2023-05-23 16:50:24.981420 fern_persona-0.0.2/src/persona/types/expire_an_inquiry_response_data_relationships_verifications.py
--rw-r--r--   0        0        0      841 2023-05-23 16:50:24.981420 fern_persona-0.0.2/src/persona/types/expire_an_inquiry_response_data_relationships_verifications_data_item.py
--rw-r--r--   0        0        0      903 2023-05-23 16:50:24.981420 fern_persona-0.0.2/src/persona/types/generate_a_one_time_link_request_meta.py
--rw-r--r--   0        0        0     1038 2023-05-23 16:50:24.981420 fern_persona-0.0.2/src/persona/types/generate_a_one_time_link_response.py
--rw-r--r--   0        0        0     1188 2023-05-23 16:50:24.981420 fern_persona-0.0.2/src/persona/types/generate_a_one_time_link_response_data.py
--rw-r--r--   0        0        0     3746 2023-05-23 16:50:24.981420 fern_persona-0.0.2/src/persona/types/generate_a_one_time_link_response_data_attributes.py
--rw-r--r--   0        0        0     2163 2023-05-23 16:50:24.981420 fern_persona-0.0.2/src/persona/types/generate_a_one_time_link_response_data_attributes_behaviors.py
--rw-r--r--   0        0        0     4475 2023-05-23 16:50:24.981420 fern_persona-0.0.2/src/persona/types/generate_a_one_time_link_response_data_attributes_fields.py
--rw-r--r--   0        0        0      849 2023-05-23 16:50:24.981420 fern_persona-0.0.2/src/persona/types/generate_a_one_time_link_response_data_attributes_fields_address_city.py
--rw-r--r--   0        0        0      855 2023-05-23 16:50:24.981420 fern_persona-0.0.2/src/persona/types/generate_a_one_time_link_response_data_attributes_fields_address_postal_code.py
--rw-r--r--   0        0        0      852 2023-05-23 16:50:24.981420 fern_persona-0.0.2/src/persona/types/generate_a_one_time_link_response_data_attributes_fields_address_street_1.py
--rw-r--r--   0        0        0      852 2023-05-23 16:50:24.981420 fern_persona-0.0.2/src/persona/types/generate_a_one_time_link_response_data_attributes_fields_address_street_2.py
--rw-r--r--   0        0        0      856 2023-05-23 16:50:24.981420 fern_persona-0.0.2/src/persona/types/generate_a_one_time_link_response_data_attributes_fields_address_subdivision.py
--rw-r--r--   0        0        0      847 2023-05-23 16:50:24.981420 fern_persona-0.0.2/src/persona/types/generate_a_one_time_link_response_data_attributes_fields_birthdate.py
--rw-r--r--   0        0        0      850 2023-05-23 16:50:24.981420 fern_persona-0.0.2/src/persona/types/generate_a_one_time_link_response_data_attributes_fields_email_address.py
--rw-r--r--   0        0        0      858 2023-05-23 16:50:24.981420 fern_persona-0.0.2/src/persona/types/generate_a_one_time_link_response_data_attributes_fields_identification_number.py
--rw-r--r--   0        0        0      847 2023-05-23 16:50:24.981420 fern_persona-0.0.2/src/persona/types/generate_a_one_time_link_response_data_attributes_fields_name_first.py
--rw-r--r--   0        0        0      846 2023-05-23 16:50:24.981420 fern_persona-0.0.2/src/persona/types/generate_a_one_time_link_response_data_attributes_fields_name_last.py
--rw-r--r--   0        0        0      848 2023-05-23 16:50:24.981420 fern_persona-0.0.2/src/persona/types/generate_a_one_time_link_response_data_attributes_fields_name_middle.py
--rw-r--r--   0        0        0      849 2023-05-23 16:50:24.981420 fern_persona-0.0.2/src/persona/types/generate_a_one_time_link_response_data_attributes_fields_phone_number.py
--rw-r--r--   0        0        0     3265 2023-05-23 16:50:24.981420 fern_persona-0.0.2/src/persona/types/generate_a_one_time_link_response_data_relationships.py
--rw-r--r--   0        0        0     1001 2023-05-23 16:50:24.981420 fern_persona-0.0.2/src/persona/types/generate_a_one_time_link_response_data_relationships_account.py
--rw-r--r--   0        0        0      836 2023-05-23 16:50:24.981420 fern_persona-0.0.2/src/persona/types/generate_a_one_time_link_response_data_relationships_account_data.py
--rw-r--r--   0        0        0     1035 2023-05-23 16:50:24.981420 fern_persona-0.0.2/src/persona/types/generate_a_one_time_link_response_data_relationships_documents.py
--rw-r--r--   0        0        0      842 2023-05-23 16:50:24.981420 fern_persona-0.0.2/src/persona/types/generate_a_one_time_link_response_data_relationships_documents_data_item.py
--rw-r--r--   0        0        0     1034 2023-05-23 16:50:24.981420 fern_persona-0.0.2/src/persona/types/generate_a_one_time_link_response_data_relationships_inquiry_template.py
--rw-r--r--   0        0        0      844 2023-05-23 16:50:24.981420 fern_persona-0.0.2/src/persona/types/generate_a_one_time_link_response_data_relationships_inquiry_template_data.py
--rw-r--r--   0        0        0     1063 2023-05-23 16:50:24.981420 fern_persona-0.0.2/src/persona/types/generate_a_one_time_link_response_data_relationships_inquiry_template_version.py
--rw-r--r--   0        0        0      851 2023-05-23 16:50:24.981420 fern_persona-0.0.2/src/persona/types/generate_a_one_time_link_response_data_relationships_inquiry_template_version_data.py
--rw-r--r--   0        0        0      823 2023-05-23 16:50:24.981420 fern_persona-0.0.2/src/persona/types/generate_a_one_time_link_response_data_relationships_reports.py
--rw-r--r--   0        0        0      811 2023-05-23 16:50:24.981420 fern_persona-0.0.2/src/persona/types/generate_a_one_time_link_response_data_relationships_reviewer.py
--rw-r--r--   0        0        0      823 2023-05-23 16:50:24.981420 fern_persona-0.0.2/src/persona/types/generate_a_one_time_link_response_data_relationships_selfies.py
--rw-r--r--   0        0        0     1031 2023-05-23 16:50:24.981420 fern_persona-0.0.2/src/persona/types/generate_a_one_time_link_response_data_relationships_sessions.py
--rw-r--r--   0        0        0      841 2023-05-23 16:50:24.981420 fern_persona-0.0.2/src/persona/types/generate_a_one_time_link_response_data_relationships_sessions_data_item.py
--rw-r--r--   0        0        0      811 2023-05-23 16:50:24.981420 fern_persona-0.0.2/src/persona/types/generate_a_one_time_link_response_data_relationships_template.py
--rw-r--r--   0        0        0     1051 2023-05-23 16:50:24.981420 fern_persona-0.0.2/src/persona/types/generate_a_one_time_link_response_data_relationships_verifications.py
--rw-r--r--   0        0        0      846 2023-05-23 16:50:24.981420 fern_persona-0.0.2/src/persona/types/generate_a_one_time_link_response_data_relationships_verifications_data_item.py
--rw-r--r--   0        0        0      970 2023-05-23 16:50:24.981420 fern_persona-0.0.2/src/persona/types/generate_a_one_time_link_response_meta.py
--rw-r--r--   0        0        0      884 2023-05-23 16:50:24.981420 fern_persona-0.0.2/src/persona/types/import_an_account_request_data.py
--rw-r--r--   0        0        0      921 2023-05-23 16:50:24.981420 fern_persona-0.0.2/src/persona/types/import_an_account_request_data_file.py
--rw-r--r--   0        0        0      871 2023-05-23 16:50:24.981420 fern_persona-0.0.2/src/persona/types/import_an_account_response.py
--rw-r--r--   0        0        0      972 2023-05-23 16:50:24.981420 fern_persona-0.0.2/src/persona/types/import_an_account_response_data.py
--rw-r--r--   0        0        0     1241 2023-05-23 16:50:24.981420 fern_persona-0.0.2/src/persona/types/import_an_account_response_data_attributes.py
--rw-r--r--   0        0        0      941 2023-05-23 16:50:24.981420 fern_persona-0.0.2/src/persona/types/import_email_address_lists_request_data.py
--rw-r--r--   0        0        0     1072 2023-05-23 16:50:24.981420 fern_persona-0.0.2/src/persona/types/import_email_address_lists_request_data_attributes.py
--rw-r--r--   0        0        0      939 2023-05-23 16:50:24.981420 fern_persona-0.0.2/src/persona/types/import_email_address_lists_request_data_attributes_file.py
--rw-r--r--   0        0        0      904 2023-05-23 16:50:24.981420 fern_persona-0.0.2/src/persona/types/import_email_address_lists_response.py
--rw-r--r--   0        0        0     1005 2023-05-23 16:50:24.981420 fern_persona-0.0.2/src/persona/types/import_email_address_lists_response_data.py
--rw-r--r--   0        0        0     1249 2023-05-23 16:50:24.981420 fern_persona-0.0.2/src/persona/types/import_email_address_lists_response_data_attributes.py
--rw-r--r--   0        0        0      908 2023-05-23 16:50:24.981420 fern_persona-0.0.2/src/persona/types/import_face_lists_request_data.py
--rw-r--r--   0        0        0     1152 2023-05-23 16:50:24.981420 fern_persona-0.0.2/src/persona/types/import_face_lists_request_data_attributes.py
--rw-r--r--   0        0        0      941 2023-05-23 16:50:24.981420 fern_persona-0.0.2/src/persona/types/import_face_lists_request_data_attributes_image_files_item.py
--rw-r--r--   0        0        0      871 2023-05-23 16:50:24.981420 fern_persona-0.0.2/src/persona/types/import_face_lists_response.py
--rw-r--r--   0        0        0      972 2023-05-23 16:50:24.981420 fern_persona-0.0.2/src/persona/types/import_face_lists_response_data.py
--rw-r--r--   0        0        0     1241 2023-05-23 16:50:24.981420 fern_persona-0.0.2/src/persona/types/import_face_lists_response_data_attributes.py
--rw-r--r--   0        0        0      936 2023-05-23 16:50:24.981420 fern_persona-0.0.2/src/persona/types/import_geolocation_lists_request_data.py
--rw-r--r--   0        0        0     1067 2023-05-23 16:50:24.981420 fern_persona-0.0.2/src/persona/types/import_geolocation_lists_request_data_attributes.py
--rw-r--r--   0        0        0      938 2023-05-23 16:50:24.981420 fern_persona-0.0.2/src/persona/types/import_geolocation_lists_request_data_attributes_file.py
--rw-r--r--   0        0        0      899 2023-05-23 16:50:24.981420 fern_persona-0.0.2/src/persona/types/import_geolocation_lists_response.py
--rw-r--r--   0        0        0     1000 2023-05-23 16:50:24.981420 fern_persona-0.0.2/src/persona/types/import_geolocation_lists_response_data.py
--rw-r--r--   0        0        0     1248 2023-05-23 16:50:24.981420 fern_persona-0.0.2/src/persona/types/import_geolocation_lists_response_data_attributes.py
--rw-r--r--   0        0        0      975 2023-05-23 16:50:24.981420 fern_persona-0.0.2/src/persona/types/import_government_id_number_lists_request_data.py
--rw-r--r--   0        0        0     1106 2023-05-23 16:50:24.981420 fern_persona-0.0.2/src/persona/types/import_government_id_number_lists_request_data_attributes.py
--rw-r--r--   0        0        0      945 2023-05-23 16:50:24.981420 fern_persona-0.0.2/src/persona/types/import_government_id_number_lists_request_data_attributes_file.py
--rw-r--r--   0        0        0      929 2023-05-23 16:50:24.981420 fern_persona-0.0.2/src/persona/types/import_government_id_number_lists_response.py
--rw-r--r--   0        0        0     1039 2023-05-23 16:50:24.981420 fern_persona-0.0.2/src/persona/types/import_government_id_number_lists_response_data.py
--rw-r--r--   0        0        0     1255 2023-05-23 16:50:24.981420 fern_persona-0.0.2/src/persona/types/import_government_id_number_lists_response_data_attributes.py
--rw-r--r--   0        0        0      929 2023-05-23 16:50:24.981420 fern_persona-0.0.2/src/persona/types/import_ip_address_lists_request_data.py
--rw-r--r--   0        0        0     1060 2023-05-23 16:50:24.981420 fern_persona-0.0.2/src/persona/types/import_ip_address_lists_request_data_attributes.py
--rw-r--r--   0        0        0      936 2023-05-23 16:50:24.981420 fern_persona-0.0.2/src/persona/types/import_ip_address_lists_request_data_attributes_file.py
--rw-r--r--   0        0        0      892 2023-05-23 16:50:24.981420 fern_persona-0.0.2/src/persona/types/import_ip_address_lists_response.py
--rw-r--r--   0        0        0      993 2023-05-23 16:50:24.981420 fern_persona-0.0.2/src/persona/types/import_ip_address_lists_response_data.py
--rw-r--r--   0        0        0     1246 2023-05-23 16:50:24.981420 fern_persona-0.0.2/src/persona/types/import_ip_address_lists_response_data_attributes.py
--rw-r--r--   0        0        0      908 2023-05-23 16:50:24.981420 fern_persona-0.0.2/src/persona/types/import_name_lists_request_data.py
--rw-r--r--   0        0        0     1039 2023-05-23 16:50:24.981420 fern_persona-0.0.2/src/persona/types/import_name_lists_request_data_attributes.py
--rw-r--r--   0        0        0      931 2023-05-23 16:50:24.981420 fern_persona-0.0.2/src/persona/types/import_name_lists_request_data_attributes_file.py
--rw-r--r--   0        0        0      871 2023-05-23 16:50:24.981420 fern_persona-0.0.2/src/persona/types/import_name_lists_response.py
--rw-r--r--   0        0        0      972 2023-05-23 16:50:24.981420 fern_persona-0.0.2/src/persona/types/import_name_lists_response_data.py
--rw-r--r--   0        0        0     1241 2023-05-23 16:50:24.981420 fern_persona-0.0.2/src/persona/types/import_name_lists_response_data_attributes.py
--rw-r--r--   0        0        0      937 2023-05-23 16:50:24.981420 fern_persona-0.0.2/src/persona/types/import_phone_number_lists_request_data.py
--rw-r--r--   0        0        0     1068 2023-05-23 16:50:24.981420 fern_persona-0.0.2/src/persona/types/import_phone_number_lists_request_data_attributes.py
--rw-r--r--   0        0        0      938 2023-05-23 16:50:24.981420 fern_persona-0.0.2/src/persona/types/import_phone_number_lists_request_data_attributes_file.py
--rw-r--r--   0        0        0      900 2023-05-23 16:50:24.981420 fern_persona-0.0.2/src/persona/types/import_phone_number_lists_response.py
--rw-r--r--   0        0        0     1001 2023-05-23 16:50:24.981420 fern_persona-0.0.2/src/persona/types/import_phone_number_lists_response_data.py
--rw-r--r--   0        0        0     1248 2023-05-23 16:50:24.981420 fern_persona-0.0.2/src/persona/types/import_phone_number_lists_response_data_attributes.py
--rw-r--r--   0        0        0     1029 2023-05-23 16:50:24.981420 fern_persona-0.0.2/src/persona/types/list_all_accounts_response.py
--rw-r--r--   0        0        0      989 2023-05-23 16:50:24.981420 fern_persona-0.0.2/src/persona/types/list_all_accounts_response_data_item.py
--rw-r--r--   0        0        0     1040 2023-05-23 16:50:24.981420 fern_persona-0.0.2/src/persona/types/list_all_accounts_response_data_item_attributes.py
--rw-r--r--   0        0        0      817 2023-05-23 16:50:24.981420 fern_persona-0.0.2/src/persona/types/list_all_accounts_response_links.py
--rw-r--r--   0        0        0     1024 2023-05-23 16:50:24.981420 fern_persona-0.0.2/src/persona/types/list_all_api_keys_response.py
--rw-r--r--   0        0        0      986 2023-05-23 16:50:24.981420 fern_persona-0.0.2/src/persona/types/list_all_api_keys_response_data_item.py
--rw-r--r--   0        0        0     1554 2023-05-23 16:50:24.981420 fern_persona-0.0.2/src/persona/types/list_all_api_keys_response_data_item_attributes.py
--rw-r--r--   0        0        0      823 2023-05-23 16:50:24.981420 fern_persona-0.0.2/src/persona/types/list_all_api_keys_response_links.py
--rw-r--r--   0        0        0     1008 2023-05-23 16:50:24.981420 fern_persona-0.0.2/src/persona/types/list_all_cases_response.py
--rw-r--r--   0        0        0     1158 2023-05-23 16:50:24.981420 fern_persona-0.0.2/src/persona/types/list_all_cases_response_data_item.py
--rw-r--r--   0        0        0     1779 2023-05-23 16:50:24.981420 fern_persona-0.0.2/src/persona/types/list_all_cases_response_data_item_attributes.py
--rw-r--r--   0        0        0     1089 2023-05-23 16:50:24.981420 fern_persona-0.0.2/src/persona/types/list_all_cases_response_data_item_relationships.py
--rw-r--r--   0        0        0     1005 2023-05-23 16:50:24.981420 fern_persona-0.0.2/src/persona/types/list_all_cases_response_data_item_relationships_case_template.py
--rw-r--r--   0        0        0      837 2023-05-23 16:50:24.981420 fern_persona-0.0.2/src/persona/types/list_all_cases_response_data_item_relationships_case_template_data.py
--rw-r--r--   0        0        0      821 2023-05-23 16:50:24.981420 fern_persona-0.0.2/src/persona/types/list_all_cases_response_links.py
--rw-r--r--   0        0        0      740 2023-05-23 16:50:24.981420 fern_persona-0.0.2/src/persona/types/list_all_events_response.py
--rw-r--r--   0        0        0     1036 2023-05-23 16:50:24.981420 fern_persona-0.0.2/src/persona/types/list_all_inquiries_response.py
--rw-r--r--   0        0        0     1186 2023-05-23 16:50:24.985420 fern_persona-0.0.2/src/persona/types/list_all_inquiries_response_data_item.py
--rw-r--r--   0        0        0     1200 2023-05-23 16:50:24.985420 fern_persona-0.0.2/src/persona/types/list_all_inquiries_response_data_item_attributes.py
--rw-r--r--   0        0        0     1887 2023-05-23 16:50:24.985420 fern_persona-0.0.2/src/persona/types/list_all_inquiries_response_data_item_relationships.py
--rw-r--r--   0        0        0     1000 2023-05-23 16:50:24.985420 fern_persona-0.0.2/src/persona/types/list_all_inquiries_response_data_item_relationships_account.py
--rw-r--r--   0        0        0      836 2023-05-23 16:50:24.985420 fern_persona-0.0.2/src/persona/types/list_all_inquiries_response_data_item_relationships_account_data.py
--rw-r--r--   0        0        0      823 2023-05-23 16:50:24.985420 fern_persona-0.0.2/src/persona/types/list_all_inquiries_response_data_item_relationships_reports.py
--rw-r--r--   0        0        0     1030 2023-05-23 16:50:24.985420 fern_persona-0.0.2/src/persona/types/list_all_inquiries_response_data_item_relationships_sessions.py
--rw-r--r--   0        0        0      841 2023-05-23 16:50:24.985420 fern_persona-0.0.2/src/persona/types/list_all_inquiries_response_data_item_relationships_sessions_data_item.py
--rw-r--r--   0        0        0     1004 2023-05-23 16:50:24.985420 fern_persona-0.0.2/src/persona/types/list_all_inquiries_response_data_item_relationships_template.py
--rw-r--r--   0        0        0      837 2023-05-23 16:50:24.985420 fern_persona-0.0.2/src/persona/types/list_all_inquiries_response_data_item_relationships_template_data.py
--rw-r--r--   0        0        0     1050 2023-05-23 16:50:24.985420 fern_persona-0.0.2/src/persona/types/list_all_inquiries_response_data_item_relationships_verifications.py
--rw-r--r--   0        0        0      846 2023-05-23 16:50:24.985420 fern_persona-0.0.2/src/persona/types/list_all_inquiries_response_data_item_relationships_verifications_data_item.py
--rw-r--r--   0        0        0      818 2023-05-23 16:50:24.985420 fern_persona-0.0.2/src/persona/types/list_all_inquiries_response_links.py
--rw-r--r--   0        0        0      739 2023-05-23 16:50:24.985420 fern_persona-0.0.2/src/persona/types/list_all_lists_response.py
--rw-r--r--   0        0        0      863 2023-05-23 16:50:24.985420 fern_persona-0.0.2/src/persona/types/redact_a_report_response.py
--rw-r--r--   0        0        0      964 2023-05-23 16:50:24.985420 fern_persona-0.0.2/src/persona/types/redact_a_report_response_data.py
--rw-r--r--   0        0        0     1225 2023-05-23 16:50:24.985420 fern_persona-0.0.2/src/persona/types/redact_a_report_response_data_attributes.py
--rw-r--r--   0        0        0      871 2023-05-23 16:50:24.985420 fern_persona-0.0.2/src/persona/types/redact_an_account_response.py
--rw-r--r--   0        0        0      972 2023-05-23 16:50:24.985420 fern_persona-0.0.2/src/persona/types/redact_an_account_response_data.py
--rw-r--r--   0        0        0     1896 2023-05-23 16:50:24.985420 fern_persona-0.0.2/src/persona/types/redact_an_account_response_data_attributes.py
--rw-r--r--   0        0        0      871 2023-05-23 16:50:24.985420 fern_persona-0.0.2/src/persona/types/redact_an_inquiry_response.py
--rw-r--r--   0        0        0     1149 2023-05-23 16:50:24.985420 fern_persona-0.0.2/src/persona/types/redact_an_inquiry_response_data.py
--rw-r--r--   0        0        0     1195 2023-05-23 16:50:24.985420 fern_persona-0.0.2/src/persona/types/redact_an_inquiry_response_data_attributes.py
--rw-r--r--   0        0        0     1569 2023-05-23 16:50:24.985420 fern_persona-0.0.2/src/persona/types/redact_an_inquiry_response_data_relationships.py
--rw-r--r--   0        0        0      979 2023-05-23 16:50:24.985420 fern_persona-0.0.2/src/persona/types/redact_an_inquiry_response_data_relationships_account.py
--rw-r--r--   0        0        0      831 2023-05-23 16:50:24.985420 fern_persona-0.0.2/src/persona/types/redact_an_inquiry_response_data_relationships_account_data.py
--rw-r--r--   0        0        0      818 2023-05-23 16:50:24.985420 fern_persona-0.0.2/src/persona/types/redact_an_inquiry_response_data_relationships_reports.py
--rw-r--r--   0        0        0      983 2023-05-23 16:50:24.985420 fern_persona-0.0.2/src/persona/types/redact_an_inquiry_response_data_relationships_template.py
--rw-r--r--   0        0        0      832 2023-05-23 16:50:24.985420 fern_persona-0.0.2/src/persona/types/redact_an_inquiry_response_data_relationships_template_data.py
--rw-r--r--   0        0        0     1029 2023-05-23 16:50:24.985420 fern_persona-0.0.2/src/persona/types/redact_an_inquiry_response_data_relationships_verifications.py
--rw-r--r--   0        0        0      841 2023-05-23 16:50:24.985420 fern_persona-0.0.2/src/persona/types/redact_an_inquiry_response_data_relationships_verifications_data_item.py
--rw-r--r--   0        0        0      858 2023-05-23 16:50:24.985420 fern_persona-0.0.2/src/persona/types/remove_a_tag_1_request_meta.py
--rw-r--r--   0        0        0      857 2023-05-23 16:50:24.985420 fern_persona-0.0.2/src/persona/types/remove_a_tag_request_meta.py
--rw-r--r--   0        0        0      961 2023-05-23 16:50:24.985420 fern_persona-0.0.2/src/persona/types/report_action_pause_continuous_monitoring_response.py
--rw-r--r--   0        0        0     1325 2023-05-23 16:50:24.985420 fern_persona-0.0.2/src/persona/types/report_action_pause_continuous_monitoring_response_data.py
--rw-r--r--   0        0        0     1294 2023-05-23 16:50:24.985420 fern_persona-0.0.2/src/persona/types/report_action_pause_continuous_monitoring_response_data_attributes.py
--rw-r--r--   0        0        0     1724 2023-05-23 16:50:24.985420 fern_persona-0.0.2/src/persona/types/report_action_pause_continuous_monitoring_response_data_relationships.py
--rw-r--r--   0        0        0      827 2023-05-23 16:50:24.985420 fern_persona-0.0.2/src/persona/types/report_action_pause_continuous_monitoring_response_data_relationships_account.py
--rw-r--r--   0        0        0      827 2023-05-23 16:50:24.985420 fern_persona-0.0.2/src/persona/types/report_action_pause_continuous_monitoring_response_data_relationships_inquiry.py
--rw-r--r--   0        0        0     1098 2023-05-23 16:50:24.985420 fern_persona-0.0.2/src/persona/types/report_action_pause_continuous_monitoring_response_data_relationships_report_template.py
--rw-r--r--   0        0        0      860 2023-05-23 16:50:24.985420 fern_persona-0.0.2/src/persona/types/report_action_pause_continuous_monitoring_response_data_relationships_report_template_data.py
--rw-r--r--   0        0        0      905 2023-05-23 16:50:24.985420 fern_persona-0.0.2/src/persona/types/report_action_re_run_report_response.py
--rw-r--r--   0        0        0     1209 2023-05-23 16:50:24.985420 fern_persona-0.0.2/src/persona/types/report_action_re_run_report_response_data.py
--rw-r--r--   0        0        0     1280 2023-05-23 16:50:24.985420 fern_persona-0.0.2/src/persona/types/report_action_re_run_report_response_data_attributes.py
--rw-r--r--   0        0        0     1584 2023-05-23 16:50:24.985420 fern_persona-0.0.2/src/persona/types/report_action_re_run_report_response_data_relationships.py
--rw-r--r--   0        0        0      813 2023-05-23 16:50:24.985420 fern_persona-0.0.2/src/persona/types/report_action_re_run_report_response_data_relationships_account.py
--rw-r--r--   0        0        0      813 2023-05-23 16:50:24.985420 fern_persona-0.0.2/src/persona/types/report_action_re_run_report_response_data_relationships_inquiry.py
--rw-r--r--   0        0        0     1042 2023-05-23 16:50:24.985420 fern_persona-0.0.2/src/persona/types/report_action_re_run_report_response_data_relationships_report_template.py
--rw-r--r--   0        0        0      846 2023-05-23 16:50:24.985420 fern_persona-0.0.2/src/persona/types/report_action_re_run_report_response_data_relationships_report_template_data.py
--rw-r--r--   0        0        0      965 2023-05-23 16:50:24.985420 fern_persona-0.0.2/src/persona/types/report_action_resume_continuous_monitoring_response.py
--rw-r--r--   0        0        0     1332 2023-05-23 16:50:24.985420 fern_persona-0.0.2/src/persona/types/report_action_resume_continuous_monitoring_response_data.py
--rw-r--r--   0        0        0     1295 2023-05-23 16:50:24.985420 fern_persona-0.0.2/src/persona/types/report_action_resume_continuous_monitoring_response_data_attributes.py
--rw-r--r--   0        0        0     1734 2023-05-23 16:50:24.985420 fern_persona-0.0.2/src/persona/types/report_action_resume_continuous_monitoring_response_data_relationships.py
--rw-r--r--   0        0        0      828 2023-05-23 16:50:24.985420 fern_persona-0.0.2/src/persona/types/report_action_resume_continuous_monitoring_response_data_relationships_account.py
--rw-r--r--   0        0        0      828 2023-05-23 16:50:24.985420 fern_persona-0.0.2/src/persona/types/report_action_resume_continuous_monitoring_response_data_relationships_inquiry.py
--rw-r--r--   0        0        0     1102 2023-05-23 16:50:24.985420 fern_persona-0.0.2/src/persona/types/report_action_resume_continuous_monitoring_response_data_relationships_report_template.py
--rw-r--r--   0        0        0      861 2023-05-23 16:50:24.985420 fern_persona-0.0.2/src/persona/types/report_action_resume_continuous_monitoring_response_data_relationships_report_template_data.py
--rw-r--r--   0        0        0      861 2023-05-23 16:50:24.985420 fern_persona-0.0.2/src/persona/types/reports_add_a_tag_request_meta.py
--rw-r--r--   0        0        0      868 2023-05-23 16:50:24.985420 fern_persona-0.0.2/src/persona/types/reports_add_a_tag_response.py
--rw-r--r--   0        0        0     1144 2023-05-23 16:50:24.985420 fern_persona-0.0.2/src/persona/types/reports_add_a_tag_response_data.py
--rw-r--r--   0        0        0     1875 2023-05-23 16:50:24.985420 fern_persona-0.0.2/src/persona/types/reports_add_a_tag_response_data_attributes.py
--rw-r--r--   0        0        0     1473 2023-05-23 16:50:24.985420 fern_persona-0.0.2/src/persona/types/reports_add_a_tag_response_data_relationships.py
--rw-r--r--   0        0        0      804 2023-05-23 16:50:24.985420 fern_persona-0.0.2/src/persona/types/reports_add_a_tag_response_data_relationships_account.py
--rw-r--r--   0        0        0      804 2023-05-23 16:50:24.985420 fern_persona-0.0.2/src/persona/types/reports_add_a_tag_response_data_relationships_inquiry.py
--rw-r--r--   0        0        0     1005 2023-05-23 16:50:24.985420 fern_persona-0.0.2/src/persona/types/reports_add_a_tag_response_data_relationships_report_template.py
--rw-r--r--   0        0        0      837 2023-05-23 16:50:24.985420 fern_persona-0.0.2/src/persona/types/reports_add_a_tag_response_data_relationships_report_template_data.py
--rw-r--r--   0        0        0      864 2023-05-23 16:50:24.985420 fern_persona-0.0.2/src/persona/types/reports_remove_a_tag_request_meta.py
--rw-r--r--   0        0        0      880 2023-05-23 16:50:24.985420 fern_persona-0.0.2/src/persona/types/reports_remove_a_tag_response.py
--rw-r--r--   0        0        0     1165 2023-05-23 16:50:24.985420 fern_persona-0.0.2/src/persona/types/reports_remove_a_tag_response_data.py
--rw-r--r--   0        0        0     1878 2023-05-23 16:50:24.985420 fern_persona-0.0.2/src/persona/types/reports_remove_a_tag_response_data_attributes.py
--rw-r--r--   0        0        0     1503 2023-05-23 16:50:24.985420 fern_persona-0.0.2/src/persona/types/reports_remove_a_tag_response_data_relationships.py
--rw-r--r--   0        0        0      807 2023-05-23 16:50:24.985420 fern_persona-0.0.2/src/persona/types/reports_remove_a_tag_response_data_relationships_account.py
--rw-r--r--   0        0        0      807 2023-05-23 16:50:24.985420 fern_persona-0.0.2/src/persona/types/reports_remove_a_tag_response_data_relationships_inquiry.py
--rw-r--r--   0        0        0     1017 2023-05-23 16:50:24.985420 fern_persona-0.0.2/src/persona/types/reports_remove_a_tag_response_data_relationships_report_template.py
--rw-r--r--   0        0        0      840 2023-05-23 16:50:24.985420 fern_persona-0.0.2/src/persona/types/reports_remove_a_tag_response_data_relationships_report_template_data.py
--rw-r--r--   0        0        0      877 2023-05-23 16:50:24.985420 fern_persona-0.0.2/src/persona/types/reports_set_all_tags_request_meta.py
--rw-r--r--   0        0        0      880 2023-05-23 16:50:24.985420 fern_persona-0.0.2/src/persona/types/reports_set_all_tags_response.py
--rw-r--r--   0        0        0     1165 2023-05-23 16:50:24.985420 fern_persona-0.0.2/src/persona/types/reports_set_all_tags_response_data.py
--rw-r--r--   0        0        0     1878 2023-05-23 16:50:24.985420 fern_persona-0.0.2/src/persona/types/reports_set_all_tags_response_data_attributes.py
--rw-r--r--   0        0        0     1503 2023-05-23 16:50:24.985420 fern_persona-0.0.2/src/persona/types/reports_set_all_tags_response_data_relationships.py
--rw-r--r--   0        0        0      807 2023-05-23 16:50:24.985420 fern_persona-0.0.2/src/persona/types/reports_set_all_tags_response_data_relationships_account.py
--rw-r--r--   0        0        0      807 2023-05-23 16:50:24.985420 fern_persona-0.0.2/src/persona/types/reports_set_all_tags_response_data_relationships_inquiry.py
--rw-r--r--   0        0        0     1017 2023-05-23 16:50:24.985420 fern_persona-0.0.2/src/persona/types/reports_set_all_tags_response_data_relationships_report_template.py
--rw-r--r--   0        0        0      840 2023-05-23 16:50:24.985420 fern_persona-0.0.2/src/persona/types/reports_set_all_tags_response_data_relationships_report_template_data.py
--rw-r--r--   0        0        0      999 2023-05-23 16:50:24.985420 fern_persona-0.0.2/src/persona/types/resume_an_inquiry_response.py
--rw-r--r--   0        0        0     1149 2023-05-23 16:50:24.985420 fern_persona-0.0.2/src/persona/types/resume_an_inquiry_response_data.py
--rw-r--r--   0        0        0     1195 2023-05-23 16:50:24.985420 fern_persona-0.0.2/src/persona/types/resume_an_inquiry_response_data_attributes.py
--rw-r--r--   0        0        0     1569 2023-05-23 16:50:24.985420 fern_persona-0.0.2/src/persona/types/resume_an_inquiry_response_data_relationships.py
--rw-r--r--   0        0        0      979 2023-05-23 16:50:24.985420 fern_persona-0.0.2/src/persona/types/resume_an_inquiry_response_data_relationships_account.py
--rw-r--r--   0        0        0      831 2023-05-23 16:50:24.985420 fern_persona-0.0.2/src/persona/types/resume_an_inquiry_response_data_relationships_account_data.py
--rw-r--r--   0        0        0      818 2023-05-23 16:50:24.985420 fern_persona-0.0.2/src/persona/types/resume_an_inquiry_response_data_relationships_reports.py
--rw-r--r--   0        0        0      983 2023-05-23 16:50:24.985420 fern_persona-0.0.2/src/persona/types/resume_an_inquiry_response_data_relationships_template.py
--rw-r--r--   0        0        0      832 2023-05-23 16:50:24.985420 fern_persona-0.0.2/src/persona/types/resume_an_inquiry_response_data_relationships_template_data.py
--rw-r--r--   0        0        0     1029 2023-05-23 16:50:24.985420 fern_persona-0.0.2/src/persona/types/resume_an_inquiry_response_data_relationships_verifications.py
--rw-r--r--   0        0        0      841 2023-05-23 16:50:24.985420 fern_persona-0.0.2/src/persona/types/resume_an_inquiry_response_data_relationships_verifications_data_item.py
--rw-r--r--   0        0        0      873 2023-05-23 16:50:24.985420 fern_persona-0.0.2/src/persona/types/resume_an_inquiry_response_meta.py
--rw-r--r--   0        0        0      928 2023-05-23 16:50:24.985420 fern_persona-0.0.2/src/persona/types/retrieve_a_database_verification_response.py
--rw-r--r--   0        0        0     1267 2023-05-23 16:50:24.985420 fern_persona-0.0.2/src/persona/types/retrieve_a_database_verification_response_data.py
--rw-r--r--   0        0        0     1821 2023-05-23 16:50:24.985420 fern_persona-0.0.2/src/persona/types/retrieve_a_database_verification_response_data_attributes.py
--rw-r--r--   0        0        0     1164 2023-05-23 16:50:24.985420 fern_persona-0.0.2/src/persona/types/retrieve_a_database_verification_response_data_attributes_checks_item.py
--rw-r--r--   0        0        0      788 2023-05-23 16:50:24.985420 fern_persona-0.0.2/src/persona/types/retrieve_a_database_verification_response_data_attributes_checks_item_metadata.py
--rw-r--r--   0        0        0     1019 2023-05-23 16:50:24.985420 fern_persona-0.0.2/src/persona/types/retrieve_a_database_verification_response_data_relationships.py
--rw-r--r--   0        0        0      819 2023-05-23 16:50:24.985420 fern_persona-0.0.2/src/persona/types/retrieve_a_database_verification_response_data_relationships_inquiry.py
--rw-r--r--   0        0        0      879 2023-05-23 16:50:24.985420 fern_persona-0.0.2/src/persona/types/retrieve_a_document_response.py
--rw-r--r--   0        0        0     1163 2023-05-23 16:50:24.985420 fern_persona-0.0.2/src/persona/types/retrieve_a_document_response_data.py
--rw-r--r--   0        0        0     1309 2023-05-23 16:50:24.985420 fern_persona-0.0.2/src/persona/types/retrieve_a_document_response_data_attributes.py
--rw-r--r--   0        0        0      833 2023-05-23 16:50:24.985420 fern_persona-0.0.2/src/persona/types/retrieve_a_document_response_data_attributes_files_item.py
--rw-r--r--   0        0        0      961 2023-05-23 16:50:24.985420 fern_persona-0.0.2/src/persona/types/retrieve_a_document_response_data_relationships.py
--rw-r--r--   0        0        0      987 2023-05-23 16:50:24.985420 fern_persona-0.0.2/src/persona/types/retrieve_a_document_response_data_relationships_inquiry.py
--rw-r--r--   0        0        0      833 2023-05-23 16:50:24.985420 fern_persona-0.0.2/src/persona/types/retrieve_a_document_response_data_relationships_inquiry_data.py
--rw-r--r--   0        0        0      945 2023-05-23 16:50:24.985420 fern_persona-0.0.2/src/persona/types/retrieve_a_email_address_verification_response.py
--rw-r--r--   0        0        0     1297 2023-05-23 16:50:24.985420 fern_persona-0.0.2/src/persona/types/retrieve_a_email_address_verification_response_data.py
--rw-r--r--   0        0        0     1767 2023-05-23 16:50:24.985420 fern_persona-0.0.2/src/persona/types/retrieve_a_email_address_verification_response_data_attributes.py
--rw-r--r--   0        0        0      782 2023-05-23 16:50:24.985420 fern_persona-0.0.2/src/persona/types/retrieve_a_email_address_verification_response_data_attributes_metadata.py
--rw-r--r--   0        0        0     1036 2023-05-23 16:50:24.985420 fern_persona-0.0.2/src/persona/types/retrieve_a_email_address_verification_response_data_relationships.py
--rw-r--r--   0        0        0      823 2023-05-23 16:50:24.985420 fern_persona-0.0.2/src/persona/types/retrieve_a_email_address_verification_response_data_relationships_inquiry.py
--rw-r--r--   0        0        0      945 2023-05-23 16:50:24.985420 fern_persona-0.0.2/src/persona/types/retrieve_a_government_id_verification_response.py
--rw-r--r--   0        0        0     1297 2023-05-23 16:50:24.985420 fern_persona-0.0.2/src/persona/types/retrieve_a_government_id_verification_response_data.py
--rw-r--r--   0        0        0     3024 2023-05-23 16:50:24.985420 fern_persona-0.0.2/src/persona/types/retrieve_a_government_id_verification_response_data_attributes.py
--rw-r--r--   0        0        0     1181 2023-05-23 16:50:24.985420 fern_persona-0.0.2/src/persona/types/retrieve_a_government_id_verification_response_data_attributes_checks_item.py
--rw-r--r--   0        0        0      792 2023-05-23 16:50:24.985420 fern_persona-0.0.2/src/persona/types/retrieve_a_government_id_verification_response_data_attributes_checks_item_metadata.py
--rw-r--r--   0        0        0     1142 2023-05-23 16:50:24.985420 fern_persona-0.0.2/src/persona/types/retrieve_a_government_id_verification_response_data_attributes_photo_urls_item.py
--rw-r--r--   0        0        0     1298 2023-05-23 16:50:24.985420 fern_persona-0.0.2/src/persona/types/retrieve_a_government_id_verification_response_data_relationships.py
--rw-r--r--   0        0        0     1057 2023-05-23 16:50:24.985420 fern_persona-0.0.2/src/persona/types/retrieve_a_government_id_verification_response_data_relationships_document.py
--rw-r--r--   0        0        0      850 2023-05-23 16:50:24.985420 fern_persona-0.0.2/src/persona/types/retrieve_a_government_id_verification_response_data_relationships_document_data.py
--rw-r--r--   0        0        0      823 2023-05-23 16:50:24.985420 fern_persona-0.0.2/src/persona/types/retrieve_a_government_id_verification_response_data_relationships_inquiry.py
--rw-r--r--   0        0        0      740 2023-05-23 16:50:24.985420 fern_persona-0.0.2/src/persona/types/retrieve_a_list_response.py
--rw-r--r--   0        0        0      987 2023-05-23 16:50:24.985420 fern_persona-0.0.2/src/persona/types/retrieve_a_phone_carrier_database_verification_response.py
--rw-r--r--   0        0        0     1355 2023-05-23 16:50:24.985420 fern_persona-0.0.2/src/persona/types/retrieve_a_phone_carrier_database_verification_response_data.py
--rw-r--r--   0        0        0     1788 2023-05-23 16:50:24.985420 fern_persona-0.0.2/src/persona/types/retrieve_a_phone_carrier_database_verification_response_data_attributes.py
--rw-r--r--   0        0        0     1221 2023-05-23 16:50:24.985420 fern_persona-0.0.2/src/persona/types/retrieve_a_phone_carrier_database_verification_response_data_attributes_checks_item.py
--rw-r--r--   0        0        0     1001 2023-05-23 16:50:24.985420 fern_persona-0.0.2/src/persona/types/retrieve_a_phone_carrier_database_verification_response_data_attributes_checks_item_metadata.py
--rw-r--r--   0        0        0     1069 2023-05-23 16:50:24.985420 fern_persona-0.0.2/src/persona/types/retrieve_a_phone_carrier_database_verification_response_data_relationships.py
--rw-r--r--   0        0        0      831 2023-05-23 16:50:24.985420 fern_persona-0.0.2/src/persona/types/retrieve_a_phone_carrier_database_verification_response_data_relationships_inquiry.py
--rw-r--r--   0        0        0      941 2023-05-23 16:50:24.989421 fern_persona-0.0.2/src/persona/types/retrieve_a_phone_number_verification_response.py
--rw-r--r--   0        0        0     1290 2023-05-23 16:50:24.989421 fern_persona-0.0.2/src/persona/types/retrieve_a_phone_number_verification_response_data.py
--rw-r--r--   0        0        0     1839 2023-05-23 16:50:24.989421 fern_persona-0.0.2/src/persona/types/retrieve_a_phone_number_verification_response_data_attributes.py
--rw-r--r--   0        0        0      781 2023-05-23 16:50:24.989421 fern_persona-0.0.2/src/persona/types/retrieve_a_phone_number_verification_response_data_attributes_metadata.py
--rw-r--r--   0        0        0     1032 2023-05-23 16:50:24.989421 fern_persona-0.0.2/src/persona/types/retrieve_a_phone_number_verification_response_data_relationships.py
--rw-r--r--   0        0        0      822 2023-05-23 16:50:24.989421 fern_persona-0.0.2/src/persona/types/retrieve_a_phone_number_verification_response_data_relationships_inquiry.py
--rw-r--r--   0        0        0      871 2023-05-23 16:50:24.989421 fern_persona-0.0.2/src/persona/types/retrieve_a_report_response.py
--rw-r--r--   0        0        0      972 2023-05-23 16:50:24.989421 fern_persona-0.0.2/src/persona/types/retrieve_a_report_response_data.py
--rw-r--r--   0        0        0     1815 2023-05-23 16:50:24.989421 fern_persona-0.0.2/src/persona/types/retrieve_a_report_response_data_attributes.py
--rw-r--r--   0        0        0      920 2023-05-23 16:50:24.989421 fern_persona-0.0.2/src/persona/types/retrieve_a_selfie_verification_response.py
--rw-r--r--   0        0        0     1244 2023-05-23 16:50:24.989421 fern_persona-0.0.2/src/persona/types/retrieve_a_selfie_verification_response_data.py
--rw-r--r--   0        0        0     2216 2023-05-23 16:50:24.989421 fern_persona-0.0.2/src/persona/types/retrieve_a_selfie_verification_response_data_attributes.py
--rw-r--r--   0        0        0     1156 2023-05-23 16:50:24.989421 fern_persona-0.0.2/src/persona/types/retrieve_a_selfie_verification_response_data_attributes_checks_item.py
--rw-r--r--   0        0        0      786 2023-05-23 16:50:24.989421 fern_persona-0.0.2/src/persona/types/retrieve_a_selfie_verification_response_data_attributes_checks_item_metadata.py
--rw-r--r--   0        0        0     1011 2023-05-23 16:50:24.989421 fern_persona-0.0.2/src/persona/types/retrieve_a_selfie_verification_response_data_relationships.py
--rw-r--r--   0        0        0      817 2023-05-23 16:50:24.989421 fern_persona-0.0.2/src/persona/types/retrieve_a_selfie_verification_response_data_relationships_inquiry.py
--rw-r--r--   0        0        0      953 2023-05-23 16:50:24.989421 fern_persona-0.0.2/src/persona/types/retrieve_a_serpro_database_verification_response.py
--rw-r--r--   0        0        0     1311 2023-05-23 16:50:24.989421 fern_persona-0.0.2/src/persona/types/retrieve_a_serpro_database_verification_response_data.py
--rw-r--r--   0        0        0     1763 2023-05-23 16:50:24.989421 fern_persona-0.0.2/src/persona/types/retrieve_a_serpro_database_verification_response_data_attributes.py
--rw-r--r--   0        0        0     1196 2023-05-23 16:50:24.989421 fern_persona-0.0.2/src/persona/types/retrieve_a_serpro_database_verification_response_data_attributes_checks_item.py
--rw-r--r--   0        0        0      794 2023-05-23 16:50:24.989421 fern_persona-0.0.2/src/persona/types/retrieve_a_serpro_database_verification_response_data_attributes_checks_item_metadata.py
--rw-r--r--   0        0        0     1304 2023-05-23 16:50:24.989421 fern_persona-0.0.2/src/persona/types/retrieve_a_serpro_database_verification_response_data_relationships.py
--rw-r--r--   0        0        0      825 2023-05-23 16:50:24.989421 fern_persona-0.0.2/src/persona/types/retrieve_a_serpro_database_verification_response_data_relationships_inquiry.py
--rw-r--r--   0        0        0      824 2023-05-23 16:50:24.989421 fern_persona-0.0.2/src/persona/types/retrieve_a_serpro_database_verification_response_data_relationships_selfie.py
--rw-r--r--   0        0        0      945 2023-05-23 16:50:24.989421 fern_persona-0.0.2/src/persona/types/retrieve_a_tin_database_verifications_response.py
--rw-r--r--   0        0        0     1297 2023-05-23 16:50:24.989421 fern_persona-0.0.2/src/persona/types/retrieve_a_tin_database_verifications_response_data.py
--rw-r--r--   0        0        0     1755 2023-05-23 16:50:24.989421 fern_persona-0.0.2/src/persona/types/retrieve_a_tin_database_verifications_response_data_attributes.py
--rw-r--r--   0        0        0     1188 2023-05-23 16:50:24.989421 fern_persona-0.0.2/src/persona/types/retrieve_a_tin_database_verifications_response_data_attributes_checks_item.py
--rw-r--r--   0        0        0      792 2023-05-23 16:50:24.989421 fern_persona-0.0.2/src/persona/types/retrieve_a_tin_database_verifications_response_data_attributes_checks_item_metadata.py
--rw-r--r--   0        0        0     1036 2023-05-23 16:50:24.989421 fern_persona-0.0.2/src/persona/types/retrieve_a_tin_database_verifications_response_data_relationships.py
--rw-r--r--   0        0        0      823 2023-05-23 16:50:24.989421 fern_persona-0.0.2/src/persona/types/retrieve_a_tin_database_verifications_response_data_relationships_inquiry.py
--rw-r--r--   0        0        0      879 2023-05-23 16:50:24.989421 fern_persona-0.0.2/src/persona/types/retrieve_an_account_response.py
--rw-r--r--   0        0        0      980 2023-05-23 16:50:24.989421 fern_persona-0.0.2/src/persona/types/retrieve_an_account_response_data.py
--rw-r--r--   0        0        0     1031 2023-05-23 16:50:24.989421 fern_persona-0.0.2/src/persona/types/retrieve_an_account_response_data_attributes.py
--rw-r--r--   0        0        0      876 2023-05-23 16:50:24.989421 fern_persona-0.0.2/src/persona/types/retrieve_an_api_key_response.py
--rw-r--r--   0        0        0      977 2023-05-23 16:50:24.989421 fern_persona-0.0.2/src/persona/types/retrieve_an_api_key_response_data.py
--rw-r--r--   0        0        0     1584 2023-05-23 16:50:24.989421 fern_persona-0.0.2/src/persona/types/retrieve_an_api_key_response_data_attributes.py
--rw-r--r--   0        0        0      876 2023-05-23 16:50:24.989421 fern_persona-0.0.2/src/persona/types/retrieve_an_api_log_response.py
--rw-r--r--   0        0        0      977 2023-05-23 16:50:24.989421 fern_persona-0.0.2/src/persona/types/retrieve_an_api_log_response_data.py
--rw-r--r--   0        0        0     1258 2023-05-23 16:50:24.989421 fern_persona-0.0.2/src/persona/types/retrieve_an_api_log_response_data_attributes.py
--rw-r--r--   0        0        0     1733 2023-05-23 16:50:24.989421 fern_persona-0.0.2/src/persona/types/retrieve_an_api_log_response_data_attributes_request.py
--rw-r--r--   0        0        0     1018 2023-05-23 16:50:24.989421 fern_persona-0.0.2/src/persona/types/retrieve_an_api_log_response_data_attributes_request_get_params.py
--rw-r--r--   0        0        0      819 2023-05-23 16:50:24.989421 fern_persona-0.0.2/src/persona/types/retrieve_an_api_log_response_data_attributes_request_get_params_filter.py
--rw-r--r--   0        0        0      898 2023-05-23 16:50:24.989421 fern_persona-0.0.2/src/persona/types/retrieve_an_api_log_response_data_attributes_request_headers.py
--rw-r--r--   0        0        0      774 2023-05-23 16:50:24.989421 fern_persona-0.0.2/src/persona/types/retrieve_an_api_log_response_data_attributes_request_post_params.py
--rw-r--r--   0        0        0     1072 2023-05-23 16:50:24.989421 fern_persona-0.0.2/src/persona/types/retrieve_an_api_log_response_data_attributes_response.py
--rw-r--r--   0        0        0      893 2023-05-23 16:50:24.989421 fern_persona-0.0.2/src/persona/types/retrieve_an_api_log_response_data_attributes_response_headers.py
--rw-r--r--   0        0        0      742 2023-05-23 16:50:24.989421 fern_persona-0.0.2/src/persona/types/retrieve_an_event_response.py
--rw-r--r--   0        0        0      883 2023-05-23 16:50:24.989421 fern_persona-0.0.2/src/persona/types/retrieve_an_importer_response.py
--rw-r--r--   0        0        0      984 2023-05-23 16:50:24.989421 fern_persona-0.0.2/src/persona/types/retrieve_an_importer_response_data.py
--rw-r--r--   0        0        0     1244 2023-05-23 16:50:24.989421 fern_persona-0.0.2/src/persona/types/retrieve_an_importer_response_data_attributes.py
--rw-r--r--   0        0        0     1055 2023-05-23 16:50:24.989421 fern_persona-0.0.2/src/persona/types/retrieve_an_inquiry_response.py
--rw-r--r--   0        0        0     1163 2023-05-23 16:50:24.989421 fern_persona-0.0.2/src/persona/types/retrieve_an_inquiry_response_data.py
--rw-r--r--   0        0        0     2311 2023-05-23 16:50:24.989421 fern_persona-0.0.2/src/persona/types/retrieve_an_inquiry_response_data_attributes.py
--rw-r--r--   0        0        0     2068 2023-05-23 16:50:24.989421 fern_persona-0.0.2/src/persona/types/retrieve_an_inquiry_response_data_attributes_behaviours.py
--rw-r--r--   0        0        0     1364 2023-05-23 16:50:24.989421 fern_persona-0.0.2/src/persona/types/retrieve_an_inquiry_response_data_attributes_fields.py
--rw-r--r--   0        0        0      837 2023-05-23 16:50:24.989421 fern_persona-0.0.2/src/persona/types/retrieve_an_inquiry_response_data_attributes_fields_name_first.py
--rw-r--r--   0        0        0      836 2023-05-23 16:50:24.989421 fern_persona-0.0.2/src/persona/types/retrieve_an_inquiry_response_data_attributes_fields_name_last.py
--rw-r--r--   0        0        0     1798 2023-05-23 16:50:24.989421 fern_persona-0.0.2/src/persona/types/retrieve_an_inquiry_response_data_relationships.py
--rw-r--r--   0        0        0      987 2023-05-23 16:50:24.989421 fern_persona-0.0.2/src/persona/types/retrieve_an_inquiry_response_data_relationships_account.py
--rw-r--r--   0        0        0      833 2023-05-23 16:50:24.989421 fern_persona-0.0.2/src/persona/types/retrieve_an_inquiry_response_data_relationships_account_data.py
--rw-r--r--   0        0        0      820 2023-05-23 16:50:24.989421 fern_persona-0.0.2/src/persona/types/retrieve_an_inquiry_response_data_relationships_reports.py
--rw-r--r--   0        0        0     1017 2023-05-23 16:50:24.989421 fern_persona-0.0.2/src/persona/types/retrieve_an_inquiry_response_data_relationships_sessions.py
--rw-r--r--   0        0        0      838 2023-05-23 16:50:24.989421 fern_persona-0.0.2/src/persona/types/retrieve_an_inquiry_response_data_relationships_sessions_data_item.py
--rw-r--r--   0        0        0      991 2023-05-23 16:50:24.989421 fern_persona-0.0.2/src/persona/types/retrieve_an_inquiry_response_data_relationships_template.py
--rw-r--r--   0        0        0      834 2023-05-23 16:50:24.989421 fern_persona-0.0.2/src/persona/types/retrieve_an_inquiry_response_data_relationships_template_data.py
--rw-r--r--   0        0        0     1037 2023-05-23 16:50:24.989421 fern_persona-0.0.2/src/persona/types/retrieve_an_inquiry_response_data_relationships_verifications.py
--rw-r--r--   0        0        0      843 2023-05-23 16:50:24.989421 fern_persona-0.0.2/src/persona/types/retrieve_an_inquiry_response_data_relationships_verifications_data_item.py
--rw-r--r--   0        0        0     1013 2023-05-23 16:50:24.989421 fern_persona-0.0.2/src/persona/types/retrieve_an_inquiry_response_included_item.py
--rw-r--r--   0        0        0     1782 2023-05-23 16:50:24.989421 fern_persona-0.0.2/src/persona/types/retrieve_an_inquiry_response_included_item_attributes.py
--rw-r--r--   0        0        0      901 2023-05-23 16:50:24.989421 fern_persona-0.0.2/src/persona/types/retrieve_an_user_audit_log_response.py
--rw-r--r--   0        0        0     1002 2023-05-23 16:50:24.989421 fern_persona-0.0.2/src/persona/types/retrieve_an_user_audit_log_response_data.py
--rw-r--r--   0        0        0     1022 2023-05-23 16:50:24.989421 fern_persona-0.0.2/src/persona/types/retrieve_an_user_audit_log_response_data_attributes.py
--rw-r--r--   0        0        0     1018 2023-05-23 16:50:24.989421 fern_persona-0.0.2/src/persona/types/retrieve_case_response.py
--rw-r--r--   0        0        0     1126 2023-05-23 16:50:24.989421 fern_persona-0.0.2/src/persona/types/retrieve_case_response_data.py
--rw-r--r--   0        0        0     1775 2023-05-23 16:50:24.989421 fern_persona-0.0.2/src/persona/types/retrieve_case_response_data_attributes.py
--rw-r--r--   0        0        0     1882 2023-05-23 16:50:24.989421 fern_persona-0.0.2/src/persona/types/retrieve_case_response_data_relationships.py
--rw-r--r--   0        0        0      996 2023-05-23 16:50:24.989421 fern_persona-0.0.2/src/persona/types/retrieve_case_response_data_relationships_accounts.py
--rw-r--r--   0        0        0      833 2023-05-23 16:50:24.989421 fern_persona-0.0.2/src/persona/types/retrieve_case_response_data_relationships_accounts_data_item.py
--rw-r--r--   0        0        0     1013 2023-05-23 16:50:24.989421 fern_persona-0.0.2/src/persona/types/retrieve_case_response_data_relationships_case_comments.py
--rw-r--r--   0        0        0      837 2023-05-23 16:50:24.989421 fern_persona-0.0.2/src/persona/types/retrieve_case_response_data_relationships_case_comments_data_item.py
--rw-r--r--   0        0        0      987 2023-05-23 16:50:24.989421 fern_persona-0.0.2/src/persona/types/retrieve_case_response_data_relationships_case_template.py
--rw-r--r--   0        0        0      833 2023-05-23 16:50:24.989421 fern_persona-0.0.2/src/persona/types/retrieve_case_response_data_relationships_case_template_data.py
--rw-r--r--   0        0        0     1000 2023-05-23 16:50:24.989421 fern_persona-0.0.2/src/persona/types/retrieve_case_response_data_relationships_inquiries.py
--rw-r--r--   0        0        0      834 2023-05-23 16:50:24.989421 fern_persona-0.0.2/src/persona/types/retrieve_case_response_data_relationships_inquiries_data_item.py
--rw-r--r--   0        0        0      815 2023-05-23 16:50:24.989421 fern_persona-0.0.2/src/persona/types/retrieve_case_response_data_relationships_reports.py
--rw-r--r--   0        0        0      992 2023-05-23 16:50:24.989421 fern_persona-0.0.2/src/persona/types/retrieve_case_response_included_item.py
--rw-r--r--   0        0        0     1092 2023-05-23 16:50:24.989421 fern_persona-0.0.2/src/persona/types/retrieve_case_response_included_item_attributes.py
--rw-r--r--   0        0        0      892 2023-05-23 16:50:24.989421 fern_persona-0.0.2/src/persona/types/send_an_email_request_data.py
--rw-r--r--   0        0        0      876 2023-05-23 16:50:24.989421 fern_persona-0.0.2/src/persona/types/send_an_email_request_data_attributes.py
--rw-r--r--   0        0        0      855 2023-05-23 16:50:24.989421 fern_persona-0.0.2/src/persona/types/send_an_email_response.py
--rw-r--r--   0        0        0      956 2023-05-23 16:50:24.989421 fern_persona-0.0.2/src/persona/types/send_an_email_response_data.py
--rw-r--r--   0        0        0     1682 2023-05-23 16:50:24.989421 fern_persona-0.0.2/src/persona/types/send_an_email_response_data_attributes.py
--rw-r--r--   0        0        0      760 2023-05-23 16:50:24.989421 fern_persona-0.0.2/src/persona/types/send_an_email_response_data_attributes_metadata.py
--rw-r--r--   0        0        0      884 2023-05-23 16:50:24.989421 fern_persona-0.0.2/src/persona/types/send_an_sms_request_data.py
--rw-r--r--   0        0        0      874 2023-05-23 16:50:24.989421 fern_persona-0.0.2/src/persona/types/send_an_sms_request_data_attributes.py
--rw-r--r--   0        0        0      847 2023-05-23 16:50:24.989421 fern_persona-0.0.2/src/persona/types/send_an_sms_response.py
--rw-r--r--   0        0        0      948 2023-05-23 16:50:24.989421 fern_persona-0.0.2/src/persona/types/send_an_sms_response_data.py
--rw-r--r--   0        0        0     1750 2023-05-23 16:50:24.989421 fern_persona-0.0.2/src/persona/types/send_an_sms_response_data_attributes.py
--rw-r--r--   0        0        0      758 2023-05-23 16:50:24.989421 fern_persona-0.0.2/src/persona/types/send_an_sms_response_data_attributes_metadata.py
--rw-r--r--   0        0        0      871 2023-05-23 16:50:24.989421 fern_persona-0.0.2/src/persona/types/set_all_tags_1_request_meta.py
--rw-r--r--   0        0        0      870 2023-05-23 16:50:24.989421 fern_persona-0.0.2/src/persona/types/set_all_tags_request_meta.py
--rw-r--r--   0        0        0      781 2023-05-23 16:50:24.989421 fern_persona-0.0.2/src/persona/types/set_status_for_a_case_request_meta.py
--rw-r--r--   0        0        0      881 2023-05-23 16:50:24.989421 fern_persona-0.0.2/src/persona/types/set_status_for_a_case_response.py
--rw-r--r--   0        0        0     1167 2023-05-23 16:50:24.989421 fern_persona-0.0.2/src/persona/types/set_status_for_a_case_response_data.py
--rw-r--r--   0        0        0     1842 2023-05-23 16:50:24.989421 fern_persona-0.0.2/src/persona/types/set_status_for_a_case_response_data_attributes.py
--rw-r--r--   0        0        0     2013 2023-05-23 16:50:24.989421 fern_persona-0.0.2/src/persona/types/set_status_for_a_case_response_data_relationships.py
--rw-r--r--   0        0        0      821 2023-05-23 16:50:24.989421 fern_persona-0.0.2/src/persona/types/set_status_for_a_case_response_data_relationships_accounts.py
--rw-r--r--   0        0        0      825 2023-05-23 16:50:24.989421 fern_persona-0.0.2/src/persona/types/set_status_for_a_case_response_data_relationships_case_comments.py
--rw-r--r--   0        0        0     1010 2023-05-23 16:50:24.989421 fern_persona-0.0.2/src/persona/types/set_status_for_a_case_response_data_relationships_case_template.py
--rw-r--r--   0        0        0      838 2023-05-23 16:50:24.989421 fern_persona-0.0.2/src/persona/types/set_status_for_a_case_response_data_relationships_case_template_data.py
--rw-r--r--   0        0        0     1023 2023-05-23 16:50:24.989421 fern_persona-0.0.2/src/persona/types/set_status_for_a_case_response_data_relationships_inquiries.py
--rw-r--r--   0        0        0      839 2023-05-23 16:50:24.989421 fern_persona-0.0.2/src/persona/types/set_status_for_a_case_response_data_relationships_inquiries_data_item.py
--rw-r--r--   0        0        0     1015 2023-05-23 16:50:24.989421 fern_persona-0.0.2/src/persona/types/set_status_for_a_case_response_data_relationships_reports.py
--rw-r--r--   0        0        0      837 2023-05-23 16:50:24.989421 fern_persona-0.0.2/src/persona/types/set_status_for_a_case_response_data_relationships_reports_data_item.py
--rw-r--r--   0        0        0      871 2023-05-23 16:50:24.989421 fern_persona-0.0.2/src/persona/types/submit_a_document_response.py
--rw-r--r--   0        0        0     1149 2023-05-23 16:50:24.989421 fern_persona-0.0.2/src/persona/types/submit_a_document_response_data.py
--rw-r--r--   0        0        0     1228 2023-05-23 16:50:24.989421 fern_persona-0.0.2/src/persona/types/submit_a_document_response_data_attributes.py
--rw-r--r--   0        0        0      831 2023-05-23 16:50:24.989421 fern_persona-0.0.2/src/persona/types/submit_a_document_response_data_attributes_files_item.py
--rw-r--r--   0        0        0      953 2023-05-23 16:50:24.989421 fern_persona-0.0.2/src/persona/types/submit_a_document_response_data_relationships.py
--rw-r--r--   0        0        0      979 2023-05-23 16:50:24.989421 fern_persona-0.0.2/src/persona/types/submit_a_document_response_data_relationships_inquiry.py
--rw-r--r--   0        0        0      831 2023-05-23 16:50:24.989421 fern_persona-0.0.2/src/persona/types/submit_a_document_response_data_relationships_inquiry_data.py
--rw-r--r--   0        0        0      920 2023-05-23 16:50:24.989421 fern_persona-0.0.2/src/persona/types/submit_a_document_verification_response.py
--rw-r--r--   0        0        0     1244 2023-05-23 16:50:24.989421 fern_persona-0.0.2/src/persona/types/submit_a_document_verification_response_data.py
--rw-r--r--   0        0        0     1425 2023-05-23 16:50:24.989421 fern_persona-0.0.2/src/persona/types/submit_a_document_verification_response_data_attributes.py
--rw-r--r--   0        0        0     1254 2023-05-23 16:50:24.989421 fern_persona-0.0.2/src/persona/types/submit_a_document_verification_response_data_relationships.py
--rw-r--r--   0        0        0     1032 2023-05-23 16:50:24.989421 fern_persona-0.0.2/src/persona/types/submit_a_document_verification_response_data_relationships_document.py
--rw-r--r--   0        0        0      844 2023-05-23 16:50:24.989421 fern_persona-0.0.2/src/persona/types/submit_a_document_verification_response_data_relationships_document_data.py
--rw-r--r--   0        0        0     1028 2023-05-23 16:50:24.993421 fern_persona-0.0.2/src/persona/types/submit_a_document_verification_response_data_relationships_inquiry.py
--rw-r--r--   0        0        0      843 2023-05-23 16:50:24.993421 fern_persona-0.0.2/src/persona/types/submit_a_document_verification_response_data_relationships_inquiry_data.py
--rw-r--r--   0        0        0      921 2023-05-23 16:50:24.993421 fern_persona-0.0.2/src/persona/types/submit_a_government_id_document_response.py
--rw-r--r--   0        0        0     1246 2023-05-23 16:50:24.993421 fern_persona-0.0.2/src/persona/types/submit_a_government_id_document_response_data.py
--rw-r--r--   0        0        0     2186 2023-05-23 16:50:24.993421 fern_persona-0.0.2/src/persona/types/submit_a_government_id_document_response_data_attributes.py
--rw-r--r--   0        0        0     1012 2023-05-23 16:50:24.993421 fern_persona-0.0.2/src/persona/types/submit_a_government_id_document_response_data_relationships.py
--rw-r--r--   0        0        0     1029 2023-05-23 16:50:24.993421 fern_persona-0.0.2/src/persona/types/submit_a_government_id_document_response_data_relationships_inquiry.py
--rw-r--r--   0        0        0      843 2023-05-23 16:50:24.993421 fern_persona-0.0.2/src/persona/types/submit_a_government_id_document_response_data_relationships_inquiry_data.py
--rw-r--r--   0        0        0      937 2023-05-23 16:50:24.993421 fern_persona-0.0.2/src/persona/types/submit_a_government_id_verification_response.py
--rw-r--r--   0        0        0     1283 2023-05-23 16:50:24.993421 fern_persona-0.0.2/src/persona/types/submit_a_government_id_verification_response_data.py
--rw-r--r--   0        0        0     2555 2023-05-23 16:50:24.993421 fern_persona-0.0.2/src/persona/types/submit_a_government_id_verification_response_data_attributes.py
--rw-r--r--   0        0        0     1284 2023-05-23 16:50:24.993421 fern_persona-0.0.2/src/persona/types/submit_a_government_id_verification_response_data_relationships.py
--rw-r--r--   0        0        0     1049 2023-05-23 16:50:24.993421 fern_persona-0.0.2/src/persona/types/submit_a_government_id_verification_response_data_relationships_document.py
--rw-r--r--   0        0        0      848 2023-05-23 16:50:24.993421 fern_persona-0.0.2/src/persona/types/submit_a_government_id_verification_response_data_relationships_document_data.py
--rw-r--r--   0        0        0      821 2023-05-23 16:50:24.993421 fern_persona-0.0.2/src/persona/types/submit_a_government_id_verification_response_data_relationships_inquiry.py
--rw-r--r--   0        0        0      979 2023-05-23 16:50:24.993421 fern_persona-0.0.2/src/persona/types/submit_a_phone_carrier_database_verification_response.py
--rw-r--r--   0        0        0     1341 2023-05-23 16:50:24.993421 fern_persona-0.0.2/src/persona/types/submit_a_phone_carrier_database_verification_response_data.py
--rw-r--r--   0        0        0     1557 2023-05-23 16:50:24.993421 fern_persona-0.0.2/src/persona/types/submit_a_phone_carrier_database_verification_response_data_attributes.py
--rw-r--r--   0        0        0     1061 2023-05-23 16:50:24.993421 fern_persona-0.0.2/src/persona/types/submit_a_phone_carrier_database_verification_response_data_relationships.py
--rw-r--r--   0        0        0      829 2023-05-23 16:50:24.993421 fern_persona-0.0.2/src/persona/types/submit_a_phone_carrier_database_verification_response_data_relationships_inquiry.py
--rw-r--r--   0        0        0      912 2023-05-23 16:50:24.993421 fern_persona-0.0.2/src/persona/types/submit_a_selfie_verification_response.py
--rw-r--r--   0        0        0     1221 2023-05-23 16:50:24.993421 fern_persona-0.0.2/src/persona/types/submit_a_selfie_verification_response_data.py
--rw-r--r--   0        0        0     2043 2023-05-23 16:50:24.993421 fern_persona-0.0.2/src/persona/types/submit_a_selfie_verification_response_data_attributes.py
--rw-r--r--   0        0        0     1003 2023-05-23 16:50:24.993421 fern_persona-0.0.2/src/persona/types/submit_a_selfie_verification_response_data_relationships.py
--rw-r--r--   0        0        0      815 2023-05-23 16:50:24.993421 fern_persona-0.0.2/src/persona/types/submit_a_selfie_verification_response_data_relationships_inquiry.py
--rw-r--r--   0        0        0      945 2023-05-23 16:50:24.993421 fern_persona-0.0.2/src/persona/types/submit_a_serpro_database_verification_response.py
--rw-r--r--   0        0        0     1297 2023-05-23 16:50:24.993421 fern_persona-0.0.2/src/persona/types/submit_a_serpro_database_verification_response_data.py
--rw-r--r--   0        0        0     1551 2023-05-23 16:50:24.993421 fern_persona-0.0.2/src/persona/types/submit_a_serpro_database_verification_response_data_attributes.py
--rw-r--r--   0        0        0     1290 2023-05-23 16:50:24.993421 fern_persona-0.0.2/src/persona/types/submit_a_serpro_database_verification_response_data_relationships.py
--rw-r--r--   0        0        0      823 2023-05-23 16:50:24.993421 fern_persona-0.0.2/src/persona/types/submit_a_serpro_database_verification_response_data_relationships_inquiry.py
--rw-r--r--   0        0        0      822 2023-05-23 16:50:24.993421 fern_persona-0.0.2/src/persona/types/submit_a_serpro_database_verification_response_data_relationships_selfie.py
--rw-r--r--   0        0        0      937 2023-05-23 16:50:24.993421 fern_persona-0.0.2/src/persona/types/submit_a_tin_database_verifications_response.py
--rw-r--r--   0        0        0     1283 2023-05-23 16:50:24.993421 fern_persona-0.0.2/src/persona/types/submit_a_tin_database_verifications_response_data.py
--rw-r--r--   0        0        0     1549 2023-05-23 16:50:24.993421 fern_persona-0.0.2/src/persona/types/submit_a_tin_database_verifications_response_data_attributes.py
--rw-r--r--   0        0        0     1028 2023-05-23 16:50:24.993421 fern_persona-0.0.2/src/persona/types/submit_a_tin_database_verifications_response_data_relationships.py
--rw-r--r--   0        0        0      821 2023-05-23 16:50:24.993421 fern_persona-0.0.2/src/persona/types/submit_a_tin_database_verifications_response_data_relationships_inquiry.py
--rw-r--r--   0        0        0      925 2023-05-23 16:50:24.993421 fern_persona-0.0.2/src/persona/types/unprocessable_entity_error_body.py
--rw-r--r--   0        0        0      824 2023-05-23 16:50:24.993421 fern_persona-0.0.2/src/persona/types/unprocessable_entity_error_body_errors_item.py
--rw-r--r--   0        0        0      892 2023-05-23 16:50:24.993421 fern_persona-0.0.2/src/persona/types/update_a_case_request_data.py
--rw-r--r--   0        0        0     1128 2023-05-23 16:50:24.993421 fern_persona-0.0.2/src/persona/types/update_a_case_request_data_attributes.py
--rw-r--r--   0        0        0      943 2023-05-23 16:50:24.993421 fern_persona-0.0.2/src/persona/types/update_a_case_request_data_attributes_attachments_item.py
--rw-r--r--   0        0        0     1055 2023-05-23 16:50:24.993421 fern_persona-0.0.2/src/persona/types/update_a_case_request_data_attributes_fields.py
--rw-r--r--   0        0        0      855 2023-05-23 16:50:24.993421 fern_persona-0.0.2/src/persona/types/update_a_case_response.py
--rw-r--r--   0        0        0     1121 2023-05-23 16:50:24.993421 fern_persona-0.0.2/src/persona/types/update_a_case_response_data.py
--rw-r--r--   0        0        0     1836 2023-05-23 16:50:24.993421 fern_persona-0.0.2/src/persona/types/update_a_case_response_data_attributes.py
--rw-r--r--   0        0        0     1871 2023-05-23 16:50:24.993421 fern_persona-0.0.2/src/persona/types/update_a_case_response_data_relationships.py
--rw-r--r--   0        0        0      815 2023-05-23 16:50:24.993421 fern_persona-0.0.2/src/persona/types/update_a_case_response_data_relationships_accounts.py
--rw-r--r--   0        0        0      819 2023-05-23 16:50:24.993421 fern_persona-0.0.2/src/persona/types/update_a_case_response_data_relationships_case_comments.py
--rw-r--r--   0        0        0      984 2023-05-23 16:50:24.993421 fern_persona-0.0.2/src/persona/types/update_a_case_response_data_relationships_case_template.py
--rw-r--r--   0        0        0      832 2023-05-23 16:50:24.993421 fern_persona-0.0.2/src/persona/types/update_a_case_response_data_relationships_case_template_data.py
--rw-r--r--   0        0        0      997 2023-05-23 16:50:24.993421 fern_persona-0.0.2/src/persona/types/update_a_case_response_data_relationships_inquiries.py
--rw-r--r--   0        0        0      833 2023-05-23 16:50:24.993421 fern_persona-0.0.2/src/persona/types/update_a_case_response_data_relationships_inquiries_data_item.py
--rw-r--r--   0        0        0      989 2023-05-23 16:50:24.993421 fern_persona-0.0.2/src/persona/types/update_a_case_response_data_relationships_reports.py
--rw-r--r--   0        0        0      831 2023-05-23 16:50:24.993421 fern_persona-0.0.2/src/persona/types/update_a_case_response_data_relationships_reports_data_item.py
--rw-r--r--   0        0        0      908 2023-05-23 16:50:24.993421 fern_persona-0.0.2/src/persona/types/update_a_document_request_data.py
--rw-r--r--   0        0        0      894 2023-05-23 16:50:24.993421 fern_persona-0.0.2/src/persona/types/update_a_document_request_data_attributes.py
--rw-r--r--   0        0        0      871 2023-05-23 16:50:24.993421 fern_persona-0.0.2/src/persona/types/update_a_document_response.py
--rw-r--r--   0        0        0     1149 2023-05-23 16:50:24.993421 fern_persona-0.0.2/src/persona/types/update_a_document_response_data.py
--rw-r--r--   0        0        0     1228 2023-05-23 16:50:24.993421 fern_persona-0.0.2/src/persona/types/update_a_document_response_data_attributes.py
--rw-r--r--   0        0        0      831 2023-05-23 16:50:24.993421 fern_persona-0.0.2/src/persona/types/update_a_document_response_data_attributes_files_item.py
--rw-r--r--   0        0        0      953 2023-05-23 16:50:24.993421 fern_persona-0.0.2/src/persona/types/update_a_document_response_data_relationships.py
--rw-r--r--   0        0        0      979 2023-05-23 16:50:24.993421 fern_persona-0.0.2/src/persona/types/update_a_document_response_data_relationships_inquiry.py
--rw-r--r--   0        0        0      831 2023-05-23 16:50:24.993421 fern_persona-0.0.2/src/persona/types/update_a_document_response_data_relationships_inquiry_data.py
--rw-r--r--   0        0        0      958 2023-05-23 16:50:24.993421 fern_persona-0.0.2/src/persona/types/update_a_government_id_document_request_data.py
--rw-r--r--   0        0        0     1561 2023-05-23 16:50:24.993421 fern_persona-0.0.2/src/persona/types/update_a_government_id_document_request_data_attributes.py
--rw-r--r--   0        0        0     1353 2023-05-23 16:50:24.993421 fern_persona-0.0.2/src/persona/types/update_a_government_id_document_request_data_attributes_back_photo.py
--rw-r--r--   0        0        0     1167 2023-05-23 16:50:24.993421 fern_persona-0.0.2/src/persona/types/update_a_government_id_document_request_data_attributes_back_photo_data.py
--rw-r--r--   0        0        0     1358 2023-05-23 16:50:24.993421 fern_persona-0.0.2/src/persona/types/update_a_government_id_document_request_data_attributes_front_photo.py
--rw-r--r--   0        0        0     1168 2023-05-23 16:50:24.993421 fern_persona-0.0.2/src/persona/types/update_a_government_id_document_request_data_attributes_front_photo_data.py
--rw-r--r--   0        0        0      921 2023-05-23 16:50:24.993421 fern_persona-0.0.2/src/persona/types/update_a_government_id_document_response.py
--rw-r--r--   0        0        0     1246 2023-05-23 16:50:24.993421 fern_persona-0.0.2/src/persona/types/update_a_government_id_document_response_data.py
--rw-r--r--   0        0        0     2186 2023-05-23 16:50:24.993421 fern_persona-0.0.2/src/persona/types/update_a_government_id_document_response_data_attributes.py
--rw-r--r--   0        0        0     1012 2023-05-23 16:50:24.993421 fern_persona-0.0.2/src/persona/types/update_a_government_id_document_response_data_relationships.py
--rw-r--r--   0        0        0     1029 2023-05-23 16:50:24.993421 fern_persona-0.0.2/src/persona/types/update_a_government_id_document_response_data_relationships_inquiry.py
--rw-r--r--   0        0        0      843 2023-05-23 16:50:24.993421 fern_persona-0.0.2/src/persona/types/update_a_government_id_document_response_data_relationships_inquiry_data.py
--rw-r--r--   0        0        0      983 2023-05-23 16:50:24.993421 fern_persona-0.0.2/src/persona/types/update_a_government_id_verification_request_data.py
--rw-r--r--   0        0        0     1589 2023-05-23 16:50:24.993421 fern_persona-0.0.2/src/persona/types/update_a_government_id_verification_request_data_attributes.py
--rw-r--r--   0        0        0     1369 2023-05-23 16:50:24.993421 fern_persona-0.0.2/src/persona/types/update_a_government_id_verification_request_data_attributes_back_photo.py
--rw-r--r--   0        0        0     1171 2023-05-23 16:50:24.993421 fern_persona-0.0.2/src/persona/types/update_a_government_id_verification_request_data_attributes_back_photo_data.py
--rw-r--r--   0        0        0     1374 2023-05-23 16:50:24.993421 fern_persona-0.0.2/src/persona/types/update_a_government_id_verification_request_data_attributes_front_photo.py
--rw-r--r--   0        0        0     1172 2023-05-23 16:50:24.993421 fern_persona-0.0.2/src/persona/types/update_a_government_id_verification_request_data_attributes_front_photo_data.py
--rw-r--r--   0        0        0      937 2023-05-23 16:50:24.993421 fern_persona-0.0.2/src/persona/types/update_a_government_id_verification_response.py
--rw-r--r--   0        0        0     1283 2023-05-23 16:50:24.993421 fern_persona-0.0.2/src/persona/types/update_a_government_id_verification_response_data.py
--rw-r--r--   0        0        0     3080 2023-05-23 16:50:24.993421 fern_persona-0.0.2/src/persona/types/update_a_government_id_verification_response_data_attributes.py
--rw-r--r--   0        0        0     1028 2023-05-23 16:50:24.993421 fern_persona-0.0.2/src/persona/types/update_a_government_id_verification_response_data_relationships.py
--rw-r--r--   0        0        0     1045 2023-05-23 16:50:24.993421 fern_persona-0.0.2/src/persona/types/update_a_government_id_verification_response_data_relationships_inquiry.py
--rw-r--r--   0        0        0      847 2023-05-23 16:50:24.993421 fern_persona-0.0.2/src/persona/types/update_a_government_id_verification_response_data_relationships_inquiry_data.py
--rw-r--r--   0        0        0      908 2023-05-23 16:50:24.993421 fern_persona-0.0.2/src/persona/types/update_an_account_request_data.py
--rw-r--r--   0        0        0     3576 2023-05-23 16:50:24.993421 fern_persona-0.0.2/src/persona/types/update_an_account_request_data_attributes.py
--rw-r--r--   0        0        0     1231 2023-05-23 16:50:24.993421 fern_persona-0.0.2/src/persona/types/update_an_account_request_data_attributes_selfie_photo.py
--rw-r--r--   0        0        0     1113 2023-05-23 16:50:24.993421 fern_persona-0.0.2/src/persona/types/update_an_account_request_data_attributes_selfie_photo_data.py
--rw-r--r--   0        0        0      871 2023-05-23 16:50:24.993421 fern_persona-0.0.2/src/persona/types/update_an_account_response.py
--rw-r--r--   0        0        0      972 2023-05-23 16:50:24.993421 fern_persona-0.0.2/src/persona/types/update_an_account_response_data.py
--rw-r--r--   0        0        0     1080 2023-05-23 16:50:24.993421 fern_persona-0.0.2/src/persona/types/update_an_account_response_data_attributes.py
--rw-r--r--   0        0        0      905 2023-05-23 16:50:24.993421 fern_persona-0.0.2/src/persona/types/update_an_api_key_request_data.py
--rw-r--r--   0        0        0     1804 2023-05-23 16:50:24.993421 fern_persona-0.0.2/src/persona/types/update_an_api_key_request_data_attributes.py
--rw-r--r--   0        0        0      868 2023-05-23 16:50:24.993421 fern_persona-0.0.2/src/persona/types/update_an_api_key_response.py
--rw-r--r--   0        0        0      969 2023-05-23 16:50:24.993421 fern_persona-0.0.2/src/persona/types/update_an_api_key_response_data.py
--rw-r--r--   0        0        0     1589 2023-05-23 16:50:24.993421 fern_persona-0.0.2/src/persona/types/update_an_api_key_response_data_attributes.py
--rw-r--r--   0        0        0      908 2023-05-23 16:50:24.993421 fern_persona-0.0.2/src/persona/types/update_an_inquiry_request_data.py
--rw-r--r--   0        0        0     2047 2023-05-23 16:50:24.993421 fern_persona-0.0.2/src/persona/types/update_an_inquiry_request_data_attributes.py
--rw-r--r--   0        0        0     2192 1970-01-01 00:00:00.000000 fern_persona-0.0.2/PKG-INFO
+-rw-r--r--   0        0        0     1683 2023-05-24 17:37:53.873832 fern_persona-0.0.3/README.md
+-rw-r--r--   0        0        0      374 2023-05-24 17:37:53.873832 fern_persona-0.0.3/pyproject.toml
+-rw-r--r--   0        0        0    89351 2023-05-24 17:37:53.877832 fern_persona-0.0.3/src/persona/__init__.py
+-rw-r--r--   0        0        0     9082 2023-05-24 17:37:53.877832 fern_persona-0.0.3/src/persona/client.py
+-rw-r--r--   0        0        0      348 2023-05-24 17:37:53.877832 fern_persona-0.0.3/src/persona/core/__init__.py
+-rw-r--r--   0        0        0      426 2023-05-24 17:37:53.877832 fern_persona-0.0.3/src/persona/core/api_error.py
+-rw-r--r--   0        0        0     1047 2023-05-24 17:37:53.877832 fern_persona-0.0.3/src/persona/core/datetime_utils.py
+-rw-r--r--   0        0        0     3710 2023-05-24 17:37:53.877832 fern_persona-0.0.3/src/persona/core/jsonable_encoder.py
+-rw-r--r--   0        0        0      385 2023-05-24 17:37:53.877832 fern_persona-0.0.3/src/persona/core/remove_none_from_headers.py
+-rw-r--r--   0        0        0      163 2023-05-24 17:37:53.877832 fern_persona-0.0.3/src/persona/environment.py
+-rw-r--r--   0        0        0      355 2023-05-24 17:37:53.877832 fern_persona-0.0.3/src/persona/errors/__init__.py
+-rw-r--r--   0        0        0      248 2023-05-24 17:37:53.877832 fern_persona-0.0.3/src/persona/errors/bad_request_error.py
+-rw-r--r--   0        0        0      246 2023-05-24 17:37:53.877832 fern_persona-0.0.3/src/persona/errors/conflict_error.py
+-rw-r--r--   0        0        0      246 2023-05-24 17:37:53.877832 fern_persona-0.0.3/src/persona/errors/not_found_error.py
+-rw-r--r--   0        0        0      341 2023-05-24 17:37:53.877832 fern_persona-0.0.3/src/persona/errors/unprocessable_entity_error.py
+-rw-r--r--   0        0        0        0 2023-05-24 17:37:53.877832 fern_persona-0.0.3/src/persona/py.typed
+-rw-r--r--   0        0        0     1282 2023-05-24 17:37:53.877832 fern_persona-0.0.3/src/persona/resources/__init__.py
+-rw-r--r--   0        0        0       65 2023-05-24 17:37:53.877832 fern_persona-0.0.3/src/persona/resources/accounts/__init__.py
+-rw-r--r--   0        0        0    28009 2023-05-24 17:37:53.877832 fern_persona-0.0.3/src/persona/resources/accounts/client.py
+-rw-r--r--   0        0        0       65 2023-05-24 17:37:53.877832 fern_persona-0.0.3/src/persona/resources/api_keys/__init__.py
+-rw-r--r--   0        0        0    13048 2023-05-24 17:37:53.877832 fern_persona-0.0.3/src/persona/resources/api_keys/client.py
+-rw-r--r--   0        0        0       65 2023-05-24 17:37:53.877832 fern_persona-0.0.3/src/persona/resources/api_logs/__init__.py
+-rw-r--r--   0        0        0     5112 2023-05-24 17:37:53.877832 fern_persona-0.0.3/src/persona/resources/api_logs/client.py
+-rw-r--r--   0        0        0       65 2023-05-24 17:37:53.877832 fern_persona-0.0.3/src/persona/resources/cases/__init__.py
+-rw-r--r--   0        0        0    19462 2023-05-24 17:37:53.877832 fern_persona-0.0.3/src/persona/resources/cases/client.py
+-rw-r--r--   0        0        0       65 2023-05-24 17:37:53.877832 fern_persona-0.0.3/src/persona/resources/database_verifications/__init__.py
+-rw-r--r--   0        0        0     8290 2023-05-24 17:37:53.877832 fern_persona-0.0.3/src/persona/resources/database_verifications/client.py
+-rw-r--r--   0        0        0       65 2023-05-24 17:37:53.877832 fern_persona-0.0.3/src/persona/resources/document_verifications/__init__.py
+-rw-r--r--   0        0        0     8342 2023-05-24 17:37:53.877832 fern_persona-0.0.3/src/persona/resources/document_verifications/client.py
+-rw-r--r--   0        0        0       65 2023-05-24 17:37:53.877832 fern_persona-0.0.3/src/persona/resources/documents/__init__.py
+-rw-r--r--   0        0        0    11445 2023-05-24 17:37:53.877832 fern_persona-0.0.3/src/persona/resources/documents/client.py
+-rw-r--r--   0        0        0       65 2023-05-24 17:37:53.877832 fern_persona-0.0.3/src/persona/resources/email_address_verifications/__init__.py
+-rw-r--r--   0        0        0    11398 2023-05-24 17:37:53.877832 fern_persona-0.0.3/src/persona/resources/email_address_verifications/client.py
+-rw-r--r--   0        0        0       65 2023-05-24 17:37:53.877832 fern_persona-0.0.3/src/persona/resources/events/__init__.py
+-rw-r--r--   0        0        0     6377 2023-05-24 17:37:53.881832 fern_persona-0.0.3/src/persona/resources/events/client.py
+-rw-r--r--   0        0        0       65 2023-05-24 17:37:53.881832 fern_persona-0.0.3/src/persona/resources/government_id_documents/__init__.py
+-rw-r--r--   0        0        0     9682 2023-05-24 17:37:53.881832 fern_persona-0.0.3/src/persona/resources/government_id_documents/client.py
+-rw-r--r--   0        0        0       65 2023-05-24 17:37:53.881832 fern_persona-0.0.3/src/persona/resources/government_id_verifications/__init__.py
+-rw-r--r--   0        0        0    11987 2023-05-24 17:37:53.881832 fern_persona-0.0.3/src/persona/resources/government_id_verifications/client.py
+-rw-r--r--   0        0        0       65 2023-05-24 17:37:53.881832 fern_persona-0.0.3/src/persona/resources/graph_queries/__init__.py
+-rw-r--r--   0        0        0     4167 2023-05-24 17:37:53.881832 fern_persona-0.0.3/src/persona/resources/graph_queries/client.py
+-rw-r--r--   0        0        0       65 2023-05-24 17:37:53.881832 fern_persona-0.0.3/src/persona/resources/importers/__init__.py
+-rw-r--r--   0        0        0    23273 2023-05-24 17:37:53.881832 fern_persona-0.0.3/src/persona/resources/importers/client.py
+-rw-r--r--   0        0        0       65 2023-05-24 17:37:53.881832 fern_persona-0.0.3/src/persona/resources/inquiries/__init__.py
+-rw-r--r--   0        0        0    35976 2023-05-24 17:37:53.881832 fern_persona-0.0.3/src/persona/resources/inquiries/client.py
+-rw-r--r--   0        0        0       65 2023-05-24 17:37:53.881832 fern_persona-0.0.3/src/persona/resources/list_items/__init__.py
+-rw-r--r--   0        0        0    48951 2023-05-24 17:37:53.881832 fern_persona-0.0.3/src/persona/resources/list_items/client.py
+-rw-r--r--   0        0        0       65 2023-05-24 17:37:53.881832 fern_persona-0.0.3/src/persona/resources/lists/__init__.py
+-rw-r--r--   0        0        0    40557 2023-05-24 17:37:53.881832 fern_persona-0.0.3/src/persona/resources/lists/client.py
+-rw-r--r--   0        0        0       65 2023-05-24 17:37:53.881832 fern_persona-0.0.3/src/persona/resources/phone_carrier_database_verifications/__init__.py
+-rw-r--r--   0        0        0     9432 2023-05-24 17:37:53.881832 fern_persona-0.0.3/src/persona/resources/phone_carrier_database_verifications/client.py
+-rw-r--r--   0        0        0       65 2023-05-24 17:37:53.881832 fern_persona-0.0.3/src/persona/resources/phone_number_verifications/__init__.py
+-rw-r--r--   0        0        0    11312 2023-05-24 17:37:53.881832 fern_persona-0.0.3/src/persona/resources/phone_number_verifications/client.py
+-rw-r--r--   0        0        0       65 2023-05-24 17:37:53.881832 fern_persona-0.0.3/src/persona/resources/print_verifications/__init__.py
+-rw-r--r--   0        0        0     2166 2023-05-24 17:37:53.881832 fern_persona-0.0.3/src/persona/resources/print_verifications/client.py
+-rw-r--r--   0        0        0       65 2023-05-24 17:37:53.881832 fern_persona-0.0.3/src/persona/resources/reports/__init__.py
+-rw-r--r--   0        0        0    32521 2023-05-24 17:37:53.881832 fern_persona-0.0.3/src/persona/resources/reports/client.py
+-rw-r--r--   0        0        0       65 2023-05-24 17:37:53.881832 fern_persona-0.0.3/src/persona/resources/selfie_verifications/__init__.py
+-rw-r--r--   0        0        0     8915 2023-05-24 17:37:53.881832 fern_persona-0.0.3/src/persona/resources/selfie_verifications/client.py
+-rw-r--r--   0        0        0       65 2023-05-24 17:37:53.881832 fern_persona-0.0.3/src/persona/resources/serpo_database_verifications/__init__.py
+-rw-r--r--   0        0        0     9103 2023-05-24 17:37:53.881832 fern_persona-0.0.3/src/persona/resources/serpo_database_verifications/client.py
+-rw-r--r--   0        0        0       65 2023-05-24 17:37:53.881832 fern_persona-0.0.3/src/persona/resources/tin_database_verifications/__init__.py
+-rw-r--r--   0        0        0     9544 2023-05-24 17:37:53.881832 fern_persona-0.0.3/src/persona/resources/tin_database_verifications/client.py
+-rw-r--r--   0        0        0       65 2023-05-24 17:37:53.881832 fern_persona-0.0.3/src/persona/resources/user_audit_logs/__init__.py
+-rw-r--r--   0        0        0     5245 2023-05-24 17:37:53.881832 fern_persona-0.0.3/src/persona/resources/user_audit_logs/client.py
+-rw-r--r--   0        0        0       65 2023-05-24 17:37:53.881832 fern_persona-0.0.3/src/persona/resources/verifications/__init__.py
+-rw-r--r--   0        0        0     2396 2023-05-24 17:37:53.881832 fern_persona-0.0.3/src/persona/resources/verifications/client.py
+-rw-r--r--   0        0        0       65 2023-05-24 17:37:53.881832 fern_persona-0.0.3/src/persona/resources/workflows/__init__.py
+-rw-r--r--   0        0        0     3796 2023-05-24 17:37:53.881832 fern_persona-0.0.3/src/persona/resources/workflows/client.py
+-rw-r--r--   0        0        0   141824 2023-05-24 17:37:53.881832 fern_persona-0.0.3/src/persona/types/__init__.py
+-rw-r--r--   0        0        0      855 2023-05-24 17:37:53.881832 fern_persona-0.0.3/src/persona/types/add_a_tag_1_request_meta.py
+-rw-r--r--   0        0        0      854 2023-05-24 17:37:53.881832 fern_persona-0.0.3/src/persona/types/add_a_tag_request_meta.py
+-rw-r--r--   0        0        0      965 2023-05-24 17:37:53.881832 fern_persona-0.0.3/src/persona/types/add_persona_objects_request_meta.py
+-rw-r--r--   0        0        0      879 2023-05-24 17:37:53.881832 fern_persona-0.0.3/src/persona/types/add_persona_objects_response.py
+-rw-r--r--   0        0        0     1163 2023-05-24 17:37:53.885832 fern_persona-0.0.3/src/persona/types/add_persona_objects_response_data.py
+-rw-r--r--   0        0        0     1835 2023-05-24 17:37:53.885832 fern_persona-0.0.3/src/persona/types/add_persona_objects_response_data_attributes.py
+-rw-r--r--   0        0        0     1994 2023-05-24 17:37:53.885832 fern_persona-0.0.3/src/persona/types/add_persona_objects_response_data_relationships.py
+-rw-r--r--   0        0        0      821 2023-05-24 17:37:53.885832 fern_persona-0.0.3/src/persona/types/add_persona_objects_response_data_relationships_accounts.py
+-rw-r--r--   0        0        0      825 2023-05-24 17:37:53.885832 fern_persona-0.0.3/src/persona/types/add_persona_objects_response_data_relationships_case_comments.py
+-rw-r--r--   0        0        0     1008 2023-05-24 17:37:53.885832 fern_persona-0.0.3/src/persona/types/add_persona_objects_response_data_relationships_case_template.py
+-rw-r--r--   0        0        0      838 2023-05-24 17:37:53.885832 fern_persona-0.0.3/src/persona/types/add_persona_objects_response_data_relationships_case_template_data.py
+-rw-r--r--   0        0        0     1021 2023-05-24 17:37:53.885832 fern_persona-0.0.3/src/persona/types/add_persona_objects_response_data_relationships_inquiries.py
+-rw-r--r--   0        0        0      839 2023-05-24 17:37:53.885832 fern_persona-0.0.3/src/persona/types/add_persona_objects_response_data_relationships_inquiries_data_item.py
+-rw-r--r--   0        0        0     1013 2023-05-24 17:37:53.885832 fern_persona-0.0.3/src/persona/types/add_persona_objects_response_data_relationships_reports.py
+-rw-r--r--   0        0        0      837 2023-05-24 17:37:53.885832 fern_persona-0.0.3/src/persona/types/add_persona_objects_response_data_relationships_reports_data_item.py
+-rw-r--r--   0        0        0      848 2023-05-24 17:37:53.885832 fern_persona-0.0.3/src/persona/types/approve_an_inquiry_request_meta.py
+-rw-r--r--   0        0        0      875 2023-05-24 17:37:53.885832 fern_persona-0.0.3/src/persona/types/approve_an_inquiry_response.py
+-rw-r--r--   0        0        0     1156 2023-05-24 17:37:53.885832 fern_persona-0.0.3/src/persona/types/approve_an_inquiry_response_data.py
+-rw-r--r--   0        0        0     1196 2023-05-24 17:37:53.885832 fern_persona-0.0.3/src/persona/types/approve_an_inquiry_response_data_attributes.py
+-rw-r--r--   0        0        0     1582 2023-05-24 17:37:53.885832 fern_persona-0.0.3/src/persona/types/approve_an_inquiry_response_data_relationships.py
+-rw-r--r--   0        0        0      983 2023-05-24 17:37:53.885832 fern_persona-0.0.3/src/persona/types/approve_an_inquiry_response_data_relationships_account.py
+-rw-r--r--   0        0        0      832 2023-05-24 17:37:53.885832 fern_persona-0.0.3/src/persona/types/approve_an_inquiry_response_data_relationships_account_data.py
+-rw-r--r--   0        0        0      819 2023-05-24 17:37:53.885832 fern_persona-0.0.3/src/persona/types/approve_an_inquiry_response_data_relationships_reports.py
+-rw-r--r--   0        0        0      987 2023-05-24 17:37:53.885832 fern_persona-0.0.3/src/persona/types/approve_an_inquiry_response_data_relationships_template.py
+-rw-r--r--   0        0        0      833 2023-05-24 17:37:53.885832 fern_persona-0.0.3/src/persona/types/approve_an_inquiry_response_data_relationships_template_data.py
+-rw-r--r--   0        0        0     1033 2023-05-24 17:37:53.885832 fern_persona-0.0.3/src/persona/types/approve_an_inquiry_response_data_relationships_verifications.py
+-rw-r--r--   0        0        0      842 2023-05-24 17:37:53.885832 fern_persona-0.0.3/src/persona/types/approve_an_inquiry_response_data_relationships_verifications_data_item.py
+-rw-r--r--   0        0        0      950 2023-05-24 17:37:53.885832 fern_persona-0.0.3/src/persona/types/archive_a_browser_fingerprint_list_item_response.py
+-rw-r--r--   0        0        0     1306 2023-05-24 17:37:53.885832 fern_persona-0.0.3/src/persona/types/archive_a_browser_fingerprint_list_item_response_data.py
+-rw-r--r--   0        0        0     1187 2023-05-24 17:37:53.885832 fern_persona-0.0.3/src/persona/types/archive_a_browser_fingerprint_list_item_response_data_attributes.py
+-rw-r--r--   0        0        0     1041 2023-05-24 17:37:53.885832 fern_persona-0.0.3/src/persona/types/archive_a_browser_fingerprint_list_item_response_data_relationships.py
+-rw-r--r--   0        0        0      824 2023-05-24 17:37:53.885832 fern_persona-0.0.3/src/persona/types/archive_a_browser_fingerprint_list_item_response_data_relationships_creator.py
+-rw-r--r--   0        0        0      921 2023-05-24 17:37:53.885832 fern_persona-0.0.3/src/persona/types/archive_a_geolocation_list_item_response.py
+-rw-r--r--   0        0        0     1246 2023-05-24 17:37:53.885832 fern_persona-0.0.3/src/persona/types/archive_a_geolocation_list_item_response_data.py
+-rw-r--r--   0        0        0     1303 2023-05-24 17:37:53.885832 fern_persona-0.0.3/src/persona/types/archive_a_geolocation_list_item_response_data_attributes.py
+-rw-r--r--   0        0        0     1012 2023-05-24 17:37:53.885832 fern_persona-0.0.3/src/persona/types/archive_a_geolocation_list_item_response_data_relationships.py
+-rw-r--r--   0        0        0      817 2023-05-24 17:37:53.885832 fern_persona-0.0.3/src/persona/types/archive_a_geolocation_list_item_response_data_relationships_creator.py
+-rw-r--r--   0        0        0      951 2023-05-24 17:37:53.885832 fern_persona-0.0.3/src/persona/types/archive_a_government_id_number_list_item_response.py
+-rw-r--r--   0        0        0     1308 2023-05-24 17:37:53.885832 fern_persona-0.0.3/src/persona/types/archive_a_government_id_number_list_item_response_data.py
+-rw-r--r--   0        0        0     1297 2023-05-24 17:37:53.885832 fern_persona-0.0.3/src/persona/types/archive_a_government_id_number_list_item_response_data_attributes.py
+-rw-r--r--   0        0        0     1042 2023-05-24 17:37:53.885832 fern_persona-0.0.3/src/persona/types/archive_a_government_id_number_list_item_response_data_relationships.py
+-rw-r--r--   0        0        0      824 2023-05-24 17:37:53.885832 fern_persona-0.0.3/src/persona/types/archive_a_government_id_number_list_item_response_data_relationships_creator.py
+-rw-r--r--   0        0        0      739 2023-05-24 17:37:53.885832 fern_persona-0.0.3/src/persona/types/archive_a_list_response.py
+-rw-r--r--   0        0        0      893 2023-05-24 17:37:53.885832 fern_persona-0.0.3/src/persona/types/archive_a_name_list_item_response.py
+-rw-r--r--   0        0        0     1188 2023-05-24 17:37:53.885832 fern_persona-0.0.3/src/persona/types/archive_a_name_list_item_response_data.py
+-rw-r--r--   0        0        0     1287 2023-05-24 17:37:53.885832 fern_persona-0.0.3/src/persona/types/archive_a_name_list_item_response_data_attributes.py
+-rw-r--r--   0        0        0      984 2023-05-24 17:37:53.885832 fern_persona-0.0.3/src/persona/types/archive_a_name_list_item_response_data_relationships.py
+-rw-r--r--   0        0        0      810 2023-05-24 17:37:53.885832 fern_persona-0.0.3/src/persona/types/archive_a_name_list_item_response_data_relationships_creator.py
+-rw-r--r--   0        0        0      930 2023-05-24 17:37:53.885832 fern_persona-0.0.3/src/persona/types/archive_an_email_address_list_item_response.py
+-rw-r--r--   0        0        0     1271 2023-05-24 17:37:53.885832 fern_persona-0.0.3/src/persona/types/archive_an_email_address_list_item_response_data.py
+-rw-r--r--   0        0        0     1256 2023-05-24 17:37:53.885832 fern_persona-0.0.3/src/persona/types/archive_an_email_address_list_item_response_data_attributes.py
+-rw-r--r--   0        0        0     1021 2023-05-24 17:37:53.885832 fern_persona-0.0.3/src/persona/types/archive_an_email_address_list_item_response_data_relationships.py
+-rw-r--r--   0        0        0      819 2023-05-24 17:37:53.885832 fern_persona-0.0.3/src/persona/types/archive_an_email_address_list_item_response_data_relationships_creator.py
+-rw-r--r--   0        0        0      956 2023-05-24 17:37:53.885832 fern_persona-0.0.3/src/persona/types/assign_a_case_request_meta.py
+-rw-r--r--   0        0        0      855 2023-05-24 17:37:53.885832 fern_persona-0.0.3/src/persona/types/assign_a_case_response.py
+-rw-r--r--   0        0        0     1121 2023-05-24 17:37:53.885832 fern_persona-0.0.3/src/persona/types/assign_a_case_response_data.py
+-rw-r--r--   0        0        0     1836 2023-05-24 17:37:53.885832 fern_persona-0.0.3/src/persona/types/assign_a_case_response_data_attributes.py
+-rw-r--r--   0        0        0     1871 2023-05-24 17:37:53.885832 fern_persona-0.0.3/src/persona/types/assign_a_case_response_data_relationships.py
+-rw-r--r--   0        0        0      815 2023-05-24 17:37:53.885832 fern_persona-0.0.3/src/persona/types/assign_a_case_response_data_relationships_accounts.py
+-rw-r--r--   0        0        0      819 2023-05-24 17:37:53.885832 fern_persona-0.0.3/src/persona/types/assign_a_case_response_data_relationships_case_comments.py
+-rw-r--r--   0        0        0      984 2023-05-24 17:37:53.885832 fern_persona-0.0.3/src/persona/types/assign_a_case_response_data_relationships_case_template.py
+-rw-r--r--   0        0        0      832 2023-05-24 17:37:53.885832 fern_persona-0.0.3/src/persona/types/assign_a_case_response_data_relationships_case_template_data.py
+-rw-r--r--   0        0        0      997 2023-05-24 17:37:53.885832 fern_persona-0.0.3/src/persona/types/assign_a_case_response_data_relationships_inquiries.py
+-rw-r--r--   0        0        0      833 2023-05-24 17:37:53.885832 fern_persona-0.0.3/src/persona/types/assign_a_case_response_data_relationships_inquiries_data_item.py
+-rw-r--r--   0        0        0      989 2023-05-24 17:37:53.885832 fern_persona-0.0.3/src/persona/types/assign_a_case_response_data_relationships_reports.py
+-rw-r--r--   0        0        0      831 2023-05-24 17:37:53.885832 fern_persona-0.0.3/src/persona/types/assign_a_case_response_data_relationships_reports_data_item.py
+-rw-r--r--   0        0        0      999 2023-05-24 17:37:53.885832 fern_persona-0.0.3/src/persona/types/business_lookup_report_1_request_data.py
+-rw-r--r--   0        0        0      954 2023-05-24 17:37:53.885832 fern_persona-0.0.3/src/persona/types/business_lookup_report_1_request_data_attributes.py
+-rw-r--r--   0        0        0     1866 2023-05-24 17:37:53.885832 fern_persona-0.0.3/src/persona/types/business_lookup_report_1_request_data_attributes_query.py
+-rw-r--r--   0        0        0      896 2023-05-24 17:37:53.885832 fern_persona-0.0.3/src/persona/types/business_lookup_report_1_response.py
+-rw-r--r--   0        0        0      997 2023-05-24 17:37:53.885832 fern_persona-0.0.3/src/persona/types/business_lookup_report_1_response_data.py
+-rw-r--r--   0        0        0     1506 2023-05-24 17:37:53.885832 fern_persona-0.0.3/src/persona/types/business_lookup_report_1_response_data_attributes.py
+-rw-r--r--   0        0        0     1316 2023-05-24 17:37:53.885832 fern_persona-0.0.3/src/persona/types/business_lookup_report_1_response_data_attributes_query.py
+-rw-r--r--   0        0        0     3441 2023-05-24 17:37:53.885832 fern_persona-0.0.3/src/persona/types/business_lookup_report_1_response_data_attributes_result_item.py
+-rw-r--r--   0        0        0     1209 2023-05-24 17:37:53.885832 fern_persona-0.0.3/src/persona/types/business_lookup_report_1_response_data_attributes_result_item_addresses_item.py
+-rw-r--r--   0        0        0     1069 2023-05-24 17:37:53.885832 fern_persona-0.0.3/src/persona/types/business_lookup_report_1_response_data_attributes_result_item_agent.py
+-rw-r--r--   0        0        0     1208 2023-05-24 17:37:53.885832 fern_persona-0.0.3/src/persona/types/business_lookup_report_1_response_data_attributes_result_item_agent_address.py
+-rw-r--r--   0        0        0      851 2023-05-24 17:37:53.885832 fern_persona-0.0.3/src/persona/types/business_lookup_report_1_response_data_attributes_result_item_identifiers_item.py
+-rw-r--r--   0        0        0      973 2023-05-24 17:37:53.885832 fern_persona-0.0.3/src/persona/types/business_lookup_report_1_response_data_attributes_result_item_industry_codes_item.py
+-rw-r--r--   0        0        0     1335 2023-05-24 17:37:53.885832 fern_persona-0.0.3/src/persona/types/business_lookup_report_1_response_data_attributes_result_item_officers_item.py
+-rw-r--r--   0        0        0     1215 2023-05-24 17:37:53.885832 fern_persona-0.0.3/src/persona/types/business_lookup_report_1_response_data_attributes_result_item_officers_item_address.py
+-rw-r--r--   0        0        0     1102 2023-05-24 17:37:53.885832 fern_persona-0.0.3/src/persona/types/business_lookup_report_1_response_data_attributes_result_item_registration.py
+-rw-r--r--   0        0        0     1215 2023-05-24 17:37:53.885832 fern_persona-0.0.3/src/persona/types/business_lookup_report_1_response_data_attributes_result_item_registration_address.py
+-rw-r--r--   0        0        0      979 2023-05-24 17:37:53.885832 fern_persona-0.0.3/src/persona/types/business_lookup_report_1_response_data_attributes_result_item_source.py
+-rw-r--r--   0        0        0      988 2023-05-24 17:37:53.885832 fern_persona-0.0.3/src/persona/types/confirm_a_phone_number_verification_1_request_data.py
+-rw-r--r--   0        0        0      890 2023-05-24 17:37:53.885832 fern_persona-0.0.3/src/persona/types/confirm_a_phone_number_verification_1_request_data_attributes.py
+-rw-r--r--   0        0        0      942 2023-05-24 17:37:53.885832 fern_persona-0.0.3/src/persona/types/confirm_a_phone_number_verification_1_response.py
+-rw-r--r--   0        0        0     1052 2023-05-24 17:37:53.885832 fern_persona-0.0.3/src/persona/types/confirm_a_phone_number_verification_1_response_data.py
+-rw-r--r--   0        0        0     1778 2023-05-24 17:37:53.885832 fern_persona-0.0.3/src/persona/types/confirm_a_phone_number_verification_1_response_data_attributes.py
+-rw-r--r--   0        0        0      781 2023-05-24 17:37:53.885832 fern_persona-0.0.3/src/persona/types/confirm_a_phone_number_verification_1_response_data_attributes_metadata.py
+-rw-r--r--   0        0        0      983 2023-05-24 17:37:53.885832 fern_persona-0.0.3/src/persona/types/confirm_a_phone_number_verification_request_data.py
+-rw-r--r--   0        0        0      889 2023-05-24 17:37:53.885832 fern_persona-0.0.3/src/persona/types/confirm_a_phone_number_verification_request_data_attributes.py
+-rw-r--r--   0        0        0      937 2023-05-24 17:37:53.889832 fern_persona-0.0.3/src/persona/types/confirm_a_phone_number_verification_response.py
+-rw-r--r--   0        0        0     1047 2023-05-24 17:37:53.889832 fern_persona-0.0.3/src/persona/types/confirm_a_phone_number_verification_response_data.py
+-rw-r--r--   0        0        0     1849 2023-05-24 17:37:53.889832 fern_persona-0.0.3/src/persona/types/confirm_a_phone_number_verification_response_data_attributes.py
+-rw-r--r--   0        0        0      780 2023-05-24 17:37:53.889832 fern_persona-0.0.3/src/persona/types/confirm_a_phone_number_verification_response_data_attributes_metadata.py
+-rw-r--r--   0        0        0     1027 2023-05-24 17:37:53.889832 fern_persona-0.0.3/src/persona/types/consolidate_into_an_account_request_meta.py
+-rw-r--r--   0        0        0      992 2023-05-24 17:37:53.889832 fern_persona-0.0.3/src/persona/types/create_a_browser_fingerprint_list_item_request_data.py
+-rw-r--r--   0        0        0     1102 2023-05-24 17:37:53.889832 fern_persona-0.0.3/src/persona/types/create_a_browser_fingerprint_list_item_request_data_attributes.py
+-rw-r--r--   0        0        0      946 2023-05-24 17:37:53.889832 fern_persona-0.0.3/src/persona/types/create_a_browser_fingerprint_list_item_response.py
+-rw-r--r--   0        0        0     1299 2023-05-24 17:37:53.889832 fern_persona-0.0.3/src/persona/types/create_a_browser_fingerprint_list_item_response_data.py
+-rw-r--r--   0        0        0     1193 2023-05-24 17:37:53.889832 fern_persona-0.0.3/src/persona/types/create_a_browser_fingerprint_list_item_response_data_attributes.py
+-rw-r--r--   0        0        0     1037 2023-05-24 17:37:53.889832 fern_persona-0.0.3/src/persona/types/create_a_browser_fingerprint_list_item_response_data_relationships.py
+-rw-r--r--   0        0        0      823 2023-05-24 17:37:53.889832 fern_persona-0.0.3/src/persona/types/create_a_browser_fingerprint_list_item_response_data_relationships_creator.py
+-rw-r--r--   0        0        0      975 2023-05-24 17:37:53.889832 fern_persona-0.0.3/src/persona/types/create_a_browser_fingerprint_list_request_data.py
+-rw-r--r--   0        0        0      854 2023-05-24 17:37:53.889832 fern_persona-0.0.3/src/persona/types/create_a_browser_fingerprint_list_request_data_attributes.py
+-rw-r--r--   0        0        0      756 2023-05-24 17:37:53.889832 fern_persona-0.0.3/src/persona/types/create_a_browser_fingerprint_list_response.py
+-rw-r--r--   0        0        0      892 2023-05-24 17:37:53.889832 fern_persona-0.0.3/src/persona/types/create_a_case_request_data.py
+-rw-r--r--   0        0        0      938 2023-05-24 17:37:53.889832 fern_persona-0.0.3/src/persona/types/create_a_case_request_data_attributes.py
+-rw-r--r--   0        0        0      972 2023-05-24 17:37:53.889832 fern_persona-0.0.3/src/persona/types/create_a_case_request_meta.py
+-rw-r--r--   0        0        0     1013 2023-05-24 17:37:53.889832 fern_persona-0.0.3/src/persona/types/create_a_case_response.py
+-rw-r--r--   0        0        0     1121 2023-05-24 17:37:53.889832 fern_persona-0.0.3/src/persona/types/create_a_case_response_data.py
+-rw-r--r--   0        0        0     1857 2023-05-24 17:37:53.889832 fern_persona-0.0.3/src/persona/types/create_a_case_response_data_attributes.py
+-rw-r--r--   0        0        0     1871 2023-05-24 17:37:53.889832 fern_persona-0.0.3/src/persona/types/create_a_case_response_data_relationships.py
+-rw-r--r--   0        0        0      815 2023-05-24 17:37:53.889832 fern_persona-0.0.3/src/persona/types/create_a_case_response_data_relationships_accounts.py
+-rw-r--r--   0        0        0      819 2023-05-24 17:37:53.889832 fern_persona-0.0.3/src/persona/types/create_a_case_response_data_relationships_case_comments.py
+-rw-r--r--   0        0        0      984 2023-05-24 17:37:53.889832 fern_persona-0.0.3/src/persona/types/create_a_case_response_data_relationships_case_template.py
+-rw-r--r--   0        0        0      832 2023-05-24 17:37:53.889832 fern_persona-0.0.3/src/persona/types/create_a_case_response_data_relationships_case_template_data.py
+-rw-r--r--   0        0        0      997 2023-05-24 17:37:53.889832 fern_persona-0.0.3/src/persona/types/create_a_case_response_data_relationships_inquiries.py
+-rw-r--r--   0        0        0      833 2023-05-24 17:37:53.889832 fern_persona-0.0.3/src/persona/types/create_a_case_response_data_relationships_inquiries_data_item.py
+-rw-r--r--   0        0        0      814 2023-05-24 17:37:53.889832 fern_persona-0.0.3/src/persona/types/create_a_case_response_data_relationships_reports.py
+-rw-r--r--   0        0        0     1179 2023-05-24 17:37:53.889832 fern_persona-0.0.3/src/persona/types/create_a_case_response_included_item.py
+-rw-r--r--   0        0        0     1970 2023-05-24 17:37:53.889832 fern_persona-0.0.3/src/persona/types/create_a_case_response_included_item_attributes.py
+-rw-r--r--   0        0        0      766 2023-05-24 17:37:53.889832 fern_persona-0.0.3/src/persona/types/create_a_case_response_included_item_attributes_fields.py
+-rw-r--r--   0        0        0     2699 2023-05-24 17:37:53.889832 fern_persona-0.0.3/src/persona/types/create_a_case_response_included_item_relationships.py
+-rw-r--r--   0        0        0      996 2023-05-24 17:37:53.889832 fern_persona-0.0.3/src/persona/types/create_a_case_response_included_item_relationships_account.py
+-rw-r--r--   0        0        0      835 2023-05-24 17:37:53.889832 fern_persona-0.0.3/src/persona/types/create_a_case_response_included_item_relationships_account_data.py
+-rw-r--r--   0        0        0     1030 2023-05-24 17:37:53.889832 fern_persona-0.0.3/src/persona/types/create_a_case_response_included_item_relationships_documents.py
+-rw-r--r--   0        0        0      841 2023-05-24 17:37:53.889832 fern_persona-0.0.3/src/persona/types/create_a_case_response_included_item_relationships_documents_data_item.py
+-rw-r--r--   0        0        0      824 2023-05-24 17:37:53.889832 fern_persona-0.0.3/src/persona/types/create_a_case_response_included_item_relationships_inquiry_template_version.py
+-rw-r--r--   0        0        0      822 2023-05-24 17:37:53.889832 fern_persona-0.0.3/src/persona/types/create_a_case_response_included_item_relationships_reports.py
+-rw-r--r--   0        0        0     1022 2023-05-24 17:37:53.889832 fern_persona-0.0.3/src/persona/types/create_a_case_response_included_item_relationships_selfies.py
+-rw-r--r--   0        0        0      839 2023-05-24 17:37:53.889832 fern_persona-0.0.3/src/persona/types/create_a_case_response_included_item_relationships_selfies_data_item.py
+-rw-r--r--   0        0        0     1026 2023-05-24 17:37:53.889832 fern_persona-0.0.3/src/persona/types/create_a_case_response_included_item_relationships_sessions.py
+-rw-r--r--   0        0        0      840 2023-05-24 17:37:53.889832 fern_persona-0.0.3/src/persona/types/create_a_case_response_included_item_relationships_sessions_data_item.py
+-rw-r--r--   0        0        0     1000 2023-05-24 17:37:53.889832 fern_persona-0.0.3/src/persona/types/create_a_case_response_included_item_relationships_template.py
+-rw-r--r--   0        0        0      836 2023-05-24 17:37:53.889832 fern_persona-0.0.3/src/persona/types/create_a_case_response_included_item_relationships_template_data.py
+-rw-r--r--   0        0        0     1046 2023-05-24 17:37:53.889832 fern_persona-0.0.3/src/persona/types/create_a_case_response_included_item_relationships_verifications.py
+-rw-r--r--   0        0        0      845 2023-05-24 17:37:53.889832 fern_persona-0.0.3/src/persona/types/create_a_case_response_included_item_relationships_verifications_data_item.py
+-rw-r--r--   0        0        0      921 2023-05-24 17:37:53.889832 fern_persona-0.0.3/src/persona/types/create_a_country_list_request_data.py
+-rw-r--r--   0        0        0      843 2023-05-24 17:37:53.889832 fern_persona-0.0.3/src/persona/types/create_a_country_list_request_data_attributes.py
+-rw-r--r--   0        0        0      745 2023-05-24 17:37:53.889832 fern_persona-0.0.3/src/persona/types/create_a_country_list_response.py
+-rw-r--r--   0        0        0      934 2023-05-24 17:37:53.893832 fern_persona-0.0.3/src/persona/types/create_a_county_list_item_request_data.py
+-rw-r--r--   0        0        0     1114 2023-05-24 17:37:53.893832 fern_persona-0.0.3/src/persona/types/create_a_county_list_item_request_data_attributes.py
+-rw-r--r--   0        0        0      925 2023-05-24 17:37:53.893832 fern_persona-0.0.3/src/persona/types/create_a_database_verification_1_response.py
+-rw-r--r--   0        0        0     1262 2023-05-24 17:37:53.893832 fern_persona-0.0.3/src/persona/types/create_a_database_verification_1_response_data.py
+-rw-r--r--   0        0        0     1629 2023-05-24 17:37:53.893832 fern_persona-0.0.3/src/persona/types/create_a_database_verification_1_response_data_attributes.py
+-rw-r--r--   0        0        0     1016 2023-05-24 17:37:53.893832 fern_persona-0.0.3/src/persona/types/create_a_database_verification_1_response_data_relationships.py
+-rw-r--r--   0        0        0      818 2023-05-24 17:37:53.893832 fern_persona-0.0.3/src/persona/types/create_a_database_verification_1_response_data_relationships_inquiry.py
+-rw-r--r--   0        0        0      920 2023-05-24 17:37:53.893832 fern_persona-0.0.3/src/persona/types/create_a_database_verification_response.py
+-rw-r--r--   0        0        0     1244 2023-05-24 17:37:53.893832 fern_persona-0.0.3/src/persona/types/create_a_database_verification_response_data.py
+-rw-r--r--   0        0        0     1649 2023-05-24 17:37:53.893832 fern_persona-0.0.3/src/persona/types/create_a_database_verification_response_data_attributes.py
+-rw-r--r--   0        0        0     1011 2023-05-24 17:37:53.893832 fern_persona-0.0.3/src/persona/types/create_a_database_verification_response_data_relationships.py
+-rw-r--r--   0        0        0      817 2023-05-24 17:37:53.893832 fern_persona-0.0.3/src/persona/types/create_a_database_verification_response_data_relationships_inquiry.py
+-rw-r--r--   0        0        0      908 2023-05-24 17:37:53.893832 fern_persona-0.0.3/src/persona/types/create_a_document_request_data.py
+-rw-r--r--   0        0        0      966 2023-05-24 17:37:53.893832 fern_persona-0.0.3/src/persona/types/create_a_document_request_data_attributes.py
+-rw-r--r--   0        0        0      871 2023-05-24 17:37:53.893832 fern_persona-0.0.3/src/persona/types/create_a_document_response.py
+-rw-r--r--   0        0        0     1149 2023-05-24 17:37:53.893832 fern_persona-0.0.3/src/persona/types/create_a_document_response_data.py
+-rw-r--r--   0        0        0     1228 2023-05-24 17:37:53.893832 fern_persona-0.0.3/src/persona/types/create_a_document_response_data_attributes.py
+-rw-r--r--   0        0        0      831 2023-05-24 17:37:53.893832 fern_persona-0.0.3/src/persona/types/create_a_document_response_data_attributes_files_item.py
+-rw-r--r--   0        0        0      953 2023-05-24 17:37:53.893832 fern_persona-0.0.3/src/persona/types/create_a_document_response_data_relationships.py
+-rw-r--r--   0        0        0      979 2023-05-24 17:37:53.893832 fern_persona-0.0.3/src/persona/types/create_a_document_response_data_relationships_inquiry.py
+-rw-r--r--   0        0        0      831 2023-05-24 17:37:53.893832 fern_persona-0.0.3/src/persona/types/create_a_document_response_data_relationships_inquiry_data.py
+-rw-r--r--   0        0        0      957 2023-05-24 17:37:53.893832 fern_persona-0.0.3/src/persona/types/create_a_document_verification_request_data.py
+-rw-r--r--   0        0        0      978 2023-05-24 17:37:53.893832 fern_persona-0.0.3/src/persona/types/create_a_document_verification_request_data_attributes.py
+-rw-r--r--   0        0        0      920 2023-05-24 17:37:53.893832 fern_persona-0.0.3/src/persona/types/create_a_document_verification_response.py
+-rw-r--r--   0        0        0     1244 2023-05-24 17:37:53.893832 fern_persona-0.0.3/src/persona/types/create_a_document_verification_response_data.py
+-rw-r--r--   0        0        0     1439 2023-05-24 17:37:53.893832 fern_persona-0.0.3/src/persona/types/create_a_document_verification_response_data_attributes.py
+-rw-r--r--   0        0        0     1254 2023-05-24 17:37:53.893832 fern_persona-0.0.3/src/persona/types/create_a_document_verification_response_data_relationships.py
+-rw-r--r--   0        0        0     1032 2023-05-24 17:37:53.893832 fern_persona-0.0.3/src/persona/types/create_a_document_verification_response_data_relationships_document.py
+-rw-r--r--   0        0        0      844 2023-05-24 17:37:53.893832 fern_persona-0.0.3/src/persona/types/create_a_document_verification_response_data_relationships_document_data.py
+-rw-r--r--   0        0        0     1028 2023-05-24 17:37:53.893832 fern_persona-0.0.3/src/persona/types/create_a_document_verification_response_data_relationships_inquiry.py
+-rw-r--r--   0        0        0      843 2023-05-24 17:37:53.893832 fern_persona-0.0.3/src/persona/types/create_a_document_verification_response_data_relationships_inquiry_data.py
+-rw-r--r--   0        0        0      926 2023-05-24 17:37:53.893832 fern_persona-0.0.3/src/persona/types/create_a_face_list_item_request_data.py
+-rw-r--r--   0        0        0     1220 2023-05-24 17:37:53.893832 fern_persona-0.0.3/src/persona/types/create_a_face_list_item_request_data_attributes.py
+-rw-r--r--   0        0        0      940 2023-05-24 17:37:53.893832 fern_persona-0.0.3/src/persona/types/create_a_face_list_item_request_data_attributes_face_photo.py
+-rw-r--r--   0        0        0      909 2023-05-24 17:37:53.893832 fern_persona-0.0.3/src/persona/types/create_a_face_list_request_data.py
+-rw-r--r--   0        0        0      840 2023-05-24 17:37:53.893832 fern_persona-0.0.3/src/persona/types/create_a_face_list_request_data_attributes.py
+-rw-r--r--   0        0        0      742 2023-05-24 17:37:53.893832 fern_persona-0.0.3/src/persona/types/create_a_face_list_response.py
+-rw-r--r--   0        0        0      954 2023-05-24 17:37:53.893832 fern_persona-0.0.3/src/persona/types/create_a_geolocation_list_item_request_data.py
+-rw-r--r--   0        0        0     1401 2023-05-24 17:37:53.893832 fern_persona-0.0.3/src/persona/types/create_a_geolocation_list_item_request_data_attributes.py
+-rw-r--r--   0        0        0      917 2023-05-24 17:37:53.893832 fern_persona-0.0.3/src/persona/types/create_a_geolocation_list_item_response.py
+-rw-r--r--   0        0        0     1239 2023-05-24 17:37:53.893832 fern_persona-0.0.3/src/persona/types/create_a_geolocation_list_item_response_data.py
+-rw-r--r--   0        0        0     1309 2023-05-24 17:37:53.893832 fern_persona-0.0.3/src/persona/types/create_a_geolocation_list_item_response_data_attributes.py
+-rw-r--r--   0        0        0     1008 2023-05-24 17:37:53.893832 fern_persona-0.0.3/src/persona/types/create_a_geolocation_list_item_response_data_relationships.py
+-rw-r--r--   0        0        0      816 2023-05-24 17:37:53.893832 fern_persona-0.0.3/src/persona/types/create_a_geolocation_list_item_response_data_relationships_creator.py
+-rw-r--r--   0        0        0      937 2023-05-24 17:37:53.893832 fern_persona-0.0.3/src/persona/types/create_a_geolocation_list_request_data.py
+-rw-r--r--   0        0        0      847 2023-05-24 17:37:53.893832 fern_persona-0.0.3/src/persona/types/create_a_geolocation_list_request_data_attributes.py
+-rw-r--r--   0        0        0      749 2023-05-24 17:37:53.893832 fern_persona-0.0.3/src/persona/types/create_a_geolocation_list_response.py
+-rw-r--r--   0        0        0      946 2023-05-24 17:37:53.893832 fern_persona-0.0.3/src/persona/types/create_a_gov_id_verification_request_data.py
+-rw-r--r--   0        0        0     2143 2023-05-24 17:37:53.893832 fern_persona-0.0.3/src/persona/types/create_a_gov_id_verification_request_data_attributes.py
+-rw-r--r--   0        0        0     1341 2023-05-24 17:37:53.893832 fern_persona-0.0.3/src/persona/types/create_a_gov_id_verification_request_data_attributes_back_photo.py
+-rw-r--r--   0        0        0     1164 2023-05-24 17:37:53.893832 fern_persona-0.0.3/src/persona/types/create_a_gov_id_verification_request_data_attributes_back_photo_data.py
+-rw-r--r--   0        0        0     1346 2023-05-24 17:37:53.893832 fern_persona-0.0.3/src/persona/types/create_a_gov_id_verification_request_data_attributes_front_photo.py
+-rw-r--r--   0        0        0     1165 2023-05-24 17:37:53.893832 fern_persona-0.0.3/src/persona/types/create_a_gov_id_verification_request_data_attributes_front_photo_data.py
+-rw-r--r--   0        0        0      909 2023-05-24 17:37:53.893832 fern_persona-0.0.3/src/persona/types/create_a_gov_id_verification_response.py
+-rw-r--r--   0        0        0     1216 2023-05-24 17:37:53.893832 fern_persona-0.0.3/src/persona/types/create_a_gov_id_verification_response_data.py
+-rw-r--r--   0        0        0     2562 2023-05-24 17:37:53.893832 fern_persona-0.0.3/src/persona/types/create_a_gov_id_verification_response_data_attributes.py
+-rw-r--r--   0        0        0     1235 2023-05-24 17:37:53.893832 fern_persona-0.0.3/src/persona/types/create_a_gov_id_verification_response_data_relationships.py
+-rw-r--r--   0        0        0     1021 2023-05-24 17:37:53.893832 fern_persona-0.0.3/src/persona/types/create_a_gov_id_verification_response_data_relationships_document.py
+-rw-r--r--   0        0        0      841 2023-05-24 17:37:53.893832 fern_persona-0.0.3/src/persona/types/create_a_gov_id_verification_response_data_relationships_document_data.py
+-rw-r--r--   0        0        0      814 2023-05-24 17:37:53.893832 fern_persona-0.0.3/src/persona/types/create_a_gov_id_verification_response_data_relationships_inquiry.py
+-rw-r--r--   0        0        0      958 2023-05-24 17:37:53.893832 fern_persona-0.0.3/src/persona/types/create_a_government_id_document_request_data.py
+-rw-r--r--   0        0        0     1767 2023-05-24 17:37:53.893832 fern_persona-0.0.3/src/persona/types/create_a_government_id_document_request_data_attributes.py
+-rw-r--r--   0        0        0     1353 2023-05-24 17:37:53.893832 fern_persona-0.0.3/src/persona/types/create_a_government_id_document_request_data_attributes_back_photo.py
+-rw-r--r--   0        0        0     1167 2023-05-24 17:37:53.893832 fern_persona-0.0.3/src/persona/types/create_a_government_id_document_request_data_attributes_back_photo_data.py
+-rw-r--r--   0        0        0     1358 2023-05-24 17:37:53.893832 fern_persona-0.0.3/src/persona/types/create_a_government_id_document_request_data_attributes_front_photo.py
+-rw-r--r--   0        0        0     1168 2023-05-24 17:37:53.893832 fern_persona-0.0.3/src/persona/types/create_a_government_id_document_request_data_attributes_front_photo_data.py
+-rw-r--r--   0        0        0      921 2023-05-24 17:37:53.893832 fern_persona-0.0.3/src/persona/types/create_a_government_id_document_response.py
+-rw-r--r--   0        0        0     1246 2023-05-24 17:37:53.893832 fern_persona-0.0.3/src/persona/types/create_a_government_id_document_response_data.py
+-rw-r--r--   0        0        0     2186 2023-05-24 17:37:53.893832 fern_persona-0.0.3/src/persona/types/create_a_government_id_document_response_data_attributes.py
+-rw-r--r--   0        0        0     1012 2023-05-24 17:37:53.893832 fern_persona-0.0.3/src/persona/types/create_a_government_id_document_response_data_relationships.py
+-rw-r--r--   0        0        0     1029 2023-05-24 17:37:53.893832 fern_persona-0.0.3/src/persona/types/create_a_government_id_document_response_data_relationships_inquiry.py
+-rw-r--r--   0        0        0      843 2023-05-24 17:37:53.893832 fern_persona-0.0.3/src/persona/types/create_a_government_id_document_response_data_relationships_inquiry_data.py
+-rw-r--r--   0        0        0      993 2023-05-24 17:37:53.893832 fern_persona-0.0.3/src/persona/types/create_a_government_id_number_list_item_request_data.py
+-rw-r--r--   0        0        0     1305 2023-05-24 17:37:53.893832 fern_persona-0.0.3/src/persona/types/create_a_government_id_number_list_item_request_data_attributes.py
+-rw-r--r--   0        0        0      947 2023-05-24 17:37:53.893832 fern_persona-0.0.3/src/persona/types/create_a_government_id_number_list_item_response.py
+-rw-r--r--   0        0        0     1301 2023-05-24 17:37:53.893832 fern_persona-0.0.3/src/persona/types/create_a_government_id_number_list_item_response_data.py
+-rw-r--r--   0        0        0     1303 2023-05-24 17:37:53.893832 fern_persona-0.0.3/src/persona/types/create_a_government_id_number_list_item_response_data_attributes.py
+-rw-r--r--   0        0        0     1038 2023-05-24 17:37:53.893832 fern_persona-0.0.3/src/persona/types/create_a_government_id_number_list_item_response_data_relationships.py
+-rw-r--r--   0        0        0      823 2023-05-24 17:37:53.893832 fern_persona-0.0.3/src/persona/types/create_a_government_id_number_list_item_response_data_relationships_creator.py
+-rw-r--r--   0        0        0      976 2023-05-24 17:37:53.893832 fern_persona-0.0.3/src/persona/types/create_a_government_id_number_list_request_data.py
+-rw-r--r--   0        0        0      854 2023-05-24 17:37:53.893832 fern_persona-0.0.3/src/persona/types/create_a_government_id_number_list_request_data_attributes.py
+-rw-r--r--   0        0        0      756 2023-05-24 17:37:53.893832 fern_persona-0.0.3/src/persona/types/create_a_government_id_number_list_response.py
+-rw-r--r--   0        0        0      917 2023-05-24 17:37:53.893832 fern_persona-0.0.3/src/persona/types/create_a_graph_query_request_data.py
+-rw-r--r--   0        0        0     1146 2023-05-24 17:37:53.893832 fern_persona-0.0.3/src/persona/types/create_a_graph_query_request_data_attributes.py
+-rw-r--r--   0        0        0     1295 2023-05-24 17:37:53.893832 fern_persona-0.0.3/src/persona/types/create_a_graph_query_request_data_attributes_variable_map.py
+-rw-r--r--   0        0        0      926 2023-05-24 17:37:53.893832 fern_persona-0.0.3/src/persona/types/create_a_name_list_item_request_data.py
+-rw-r--r--   0        0        0     1266 2023-05-24 17:37:53.893832 fern_persona-0.0.3/src/persona/types/create_a_name_list_item_request_data_attributes.py
+-rw-r--r--   0        0        0      889 2023-05-24 17:37:53.893832 fern_persona-0.0.3/src/persona/types/create_a_name_list_item_response.py
+-rw-r--r--   0        0        0     1181 2023-05-24 17:37:53.893832 fern_persona-0.0.3/src/persona/types/create_a_name_list_item_response_data.py
+-rw-r--r--   0        0        0     1293 2023-05-24 17:37:53.893832 fern_persona-0.0.3/src/persona/types/create_a_name_list_item_response_data_attributes.py
+-rw-r--r--   0        0        0      980 2023-05-24 17:37:53.893832 fern_persona-0.0.3/src/persona/types/create_a_name_list_item_response_data_relationships.py
+-rw-r--r--   0        0        0      809 2023-05-24 17:37:53.893832 fern_persona-0.0.3/src/persona/types/create_a_name_list_item_response_data_relationships_creator.py
+-rw-r--r--   0        0        0      909 2023-05-24 17:37:53.897832 fern_persona-0.0.3/src/persona/types/create_a_name_list_request_data.py
+-rw-r--r--   0        0        0     1098 2023-05-24 17:37:53.897832 fern_persona-0.0.3/src/persona/types/create_a_name_list_request_data_attributes.py
+-rw-r--r--   0        0        0      742 2023-05-24 17:37:53.897832 fern_persona-0.0.3/src/persona/types/create_a_name_list_response.py
+-rw-r--r--   0        0        0     2149 2023-05-24 17:37:53.897832 fern_persona-0.0.3/src/persona/types/create_a_phone_carrier_database_verification_request_attributes.py
+-rw-r--r--   0        0        0      979 2023-05-24 17:37:53.897832 fern_persona-0.0.3/src/persona/types/create_a_phone_carrier_database_verification_response.py
+-rw-r--r--   0        0        0     1341 2023-05-24 17:37:53.897832 fern_persona-0.0.3/src/persona/types/create_a_phone_carrier_database_verification_response_data.py
+-rw-r--r--   0        0        0     1571 2023-05-24 17:37:53.897832 fern_persona-0.0.3/src/persona/types/create_a_phone_carrier_database_verification_response_data_attributes.py
+-rw-r--r--   0        0        0     1061 2023-05-24 17:37:53.897832 fern_persona-0.0.3/src/persona/types/create_a_phone_carrier_database_verification_response_data_relationships.py
+-rw-r--r--   0        0        0      829 2023-05-24 17:37:53.897832 fern_persona-0.0.3/src/persona/types/create_a_phone_carrier_database_verification_response_data_relationships_inquiry.py
+-rw-r--r--   0        0        0      955 2023-05-24 17:37:53.897832 fern_persona-0.0.3/src/persona/types/create_a_phone_number_list_item_request_data.py
+-rw-r--r--   0        0        0     1065 2023-05-24 17:37:53.897832 fern_persona-0.0.3/src/persona/types/create_a_phone_number_list_item_request_data_attributes.py
+-rw-r--r--   0        0        0      938 2023-05-24 17:37:53.897832 fern_persona-0.0.3/src/persona/types/create_a_phone_number_list_request_data.py
+-rw-r--r--   0        0        0      847 2023-05-24 17:37:53.897832 fern_persona-0.0.3/src/persona/types/create_a_phone_number_list_request_data_attributes.py
+-rw-r--r--   0        0        0      749 2023-05-24 17:37:53.897832 fern_persona-0.0.3/src/persona/types/create_a_phone_number_list_response.py
+-rw-r--r--   0        0        0      979 2023-05-24 17:37:53.897832 fern_persona-0.0.3/src/persona/types/create_a_phone_number_verification_request_data.py
+-rw-r--r--   0        0        0     1485 2023-05-24 17:37:53.897832 fern_persona-0.0.3/src/persona/types/create_a_phone_number_verification_request_data_attributes.py
+-rw-r--r--   0        0        0      933 2023-05-24 17:37:53.897832 fern_persona-0.0.3/src/persona/types/create_a_phone_number_verification_response.py
+-rw-r--r--   0        0        0     1043 2023-05-24 17:37:53.897832 fern_persona-0.0.3/src/persona/types/create_a_phone_number_verification_response_data.py
+-rw-r--r--   0        0        0     1845 2023-05-24 17:37:53.897832 fern_persona-0.0.3/src/persona/types/create_a_phone_number_verification_response_data_attributes.py
+-rw-r--r--   0        0        0      779 2023-05-24 17:37:53.897832 fern_persona-0.0.3/src/persona/types/create_a_phone_number_verification_response_data_attributes_metadata.py
+-rw-r--r--   0        0        0      900 2023-05-24 17:37:53.897832 fern_persona-0.0.3/src/persona/types/create_a_report_request_data.py
+-rw-r--r--   0        0        0     2563 2023-05-24 17:37:53.897832 fern_persona-0.0.3/src/persona/types/create_a_report_request_data_attributes.py
+-rw-r--r--   0        0        0      949 2023-05-24 17:37:53.897832 fern_persona-0.0.3/src/persona/types/create_a_selfie_verification_request_data.py
+-rw-r--r--   0        0        0     2190 2023-05-24 17:37:53.897832 fern_persona-0.0.3/src/persona/types/create_a_selfie_verification_request_data_attributes.py
+-rw-r--r--   0        0        0     1077 2023-05-24 17:37:53.897832 fern_persona-0.0.3/src/persona/types/create_a_selfie_verification_request_data_attributes_center_photo.py
+-rw-r--r--   0        0        0      920 2023-05-24 17:37:53.897832 fern_persona-0.0.3/src/persona/types/create_a_selfie_verification_request_data_attributes_center_photo_data.py
+-rw-r--r--   0        0        0     1067 2023-05-24 17:37:53.897832 fern_persona-0.0.3/src/persona/types/create_a_selfie_verification_request_data_attributes_left_photo.py
+-rw-r--r--   0        0        0      918 2023-05-24 17:37:53.897832 fern_persona-0.0.3/src/persona/types/create_a_selfie_verification_request_data_attributes_left_photo_data.py
+-rw-r--r--   0        0        0     1072 2023-05-24 17:37:53.897832 fern_persona-0.0.3/src/persona/types/create_a_selfie_verification_request_data_attributes_right_photo.py
+-rw-r--r--   0        0        0      919 2023-05-24 17:37:53.897832 fern_persona-0.0.3/src/persona/types/create_a_selfie_verification_request_data_attributes_right_photo_data.py
+-rw-r--r--   0        0        0      912 2023-05-24 17:37:53.897832 fern_persona-0.0.3/src/persona/types/create_a_selfie_verification_response.py
+-rw-r--r--   0        0        0     1221 2023-05-24 17:37:53.897832 fern_persona-0.0.3/src/persona/types/create_a_selfie_verification_response_data.py
+-rw-r--r--   0        0        0     2064 2023-05-24 17:37:53.897832 fern_persona-0.0.3/src/persona/types/create_a_selfie_verification_response_data_attributes.py
+-rw-r--r--   0        0        0     1003 2023-05-24 17:37:53.897832 fern_persona-0.0.3/src/persona/types/create_a_selfie_verification_response_data_relationships.py
+-rw-r--r--   0        0        0      815 2023-05-24 17:37:53.897832 fern_persona-0.0.3/src/persona/types/create_a_selfie_verification_response_data_relationships_inquiry.py
+-rw-r--r--   0        0        0      769 2023-05-24 17:37:53.897832 fern_persona-0.0.3/src/persona/types/create_a_serpro_database_verification_request_attributes.py
+-rw-r--r--   0        0        0      945 2023-05-24 17:37:53.897832 fern_persona-0.0.3/src/persona/types/create_a_serpro_database_verification_response.py
+-rw-r--r--   0        0        0     1297 2023-05-24 17:37:53.897832 fern_persona-0.0.3/src/persona/types/create_a_serpro_database_verification_response_data.py
+-rw-r--r--   0        0        0     1565 2023-05-24 17:37:53.897832 fern_persona-0.0.3/src/persona/types/create_a_serpro_database_verification_response_data_attributes.py
+-rw-r--r--   0        0        0     1290 2023-05-24 17:37:53.897832 fern_persona-0.0.3/src/persona/types/create_a_serpro_database_verification_response_data_relationships.py
+-rw-r--r--   0        0        0      823 2023-05-24 17:37:53.897832 fern_persona-0.0.3/src/persona/types/create_a_serpro_database_verification_response_data_relationships_inquiry.py
+-rw-r--r--   0        0        0      822 2023-05-24 17:37:53.897832 fern_persona-0.0.3/src/persona/types/create_a_serpro_database_verification_response_data_relationships_selfie.py
+-rw-r--r--   0        0        0      983 2023-05-24 17:37:53.897832 fern_persona-0.0.3/src/persona/types/create_a_tin_database_verifications_request_data.py
+-rw-r--r--   0        0        0     1634 2023-05-24 17:37:53.897832 fern_persona-0.0.3/src/persona/types/create_a_tin_database_verifications_request_data_attributes.py
+-rw-r--r--   0        0        0      937 2023-05-24 17:37:53.897832 fern_persona-0.0.3/src/persona/types/create_a_tin_database_verifications_response.py
+-rw-r--r--   0        0        0     1283 2023-05-24 17:37:53.897832 fern_persona-0.0.3/src/persona/types/create_a_tin_database_verifications_response_data.py
+-rw-r--r--   0        0        0     1563 2023-05-24 17:37:53.897832 fern_persona-0.0.3/src/persona/types/create_a_tin_database_verifications_response_data_attributes.py
+-rw-r--r--   0        0        0     1028 2023-05-24 17:37:53.897832 fern_persona-0.0.3/src/persona/types/create_a_tin_database_verifications_response_data_relationships.py
+-rw-r--r--   0        0        0      821 2023-05-24 17:37:53.897832 fern_persona-0.0.3/src/persona/types/create_a_tin_database_verifications_response_data_relationships_inquiry.py
+-rw-r--r--   0        0        0     1126 2023-05-24 17:37:53.897832 fern_persona-0.0.3/src/persona/types/create_a_workflow_run_request_data.py
+-rw-r--r--   0        0        0     1429 2023-05-24 17:37:53.897832 fern_persona-0.0.3/src/persona/types/create_a_workflow_run_request_data_attributes.py
+-rw-r--r--   0        0        0      884 2023-05-24 17:37:53.897832 fern_persona-0.0.3/src/persona/types/create_a_workflow_run_response.py
+-rw-r--r--   0        0        0     1172 2023-05-24 17:37:53.897832 fern_persona-0.0.3/src/persona/types/create_a_workflow_run_response_data.py
+-rw-r--r--   0        0        0      998 2023-05-24 17:37:53.897832 fern_persona-0.0.3/src/persona/types/create_a_workflow_run_response_data_attributes.py
+-rw-r--r--   0        0        0     1540 2023-05-24 17:37:53.897832 fern_persona-0.0.3/src/persona/types/create_a_workflow_run_response_data_relationships.py
+-rw-r--r--   0        0        0      808 2023-05-24 17:37:53.897832 fern_persona-0.0.3/src/persona/types/create_a_workflow_run_response_data_relationships_creator.py
+-rw-r--r--   0        0        0      996 2023-05-24 17:37:53.897832 fern_persona-0.0.3/src/persona/types/create_a_workflow_run_response_data_relationships_workflow.py
+-rw-r--r--   0        0        0      835 2023-05-24 17:37:53.897832 fern_persona-0.0.3/src/persona/types/create_a_workflow_run_response_data_relationships_workflow_data.py
+-rw-r--r--   0        0        0     1025 2023-05-24 17:37:53.897832 fern_persona-0.0.3/src/persona/types/create_a_workflow_run_response_data_relationships_workflow_version.py
+-rw-r--r--   0        0        0      842 2023-05-24 17:37:53.897832 fern_persona-0.0.3/src/persona/types/create_a_workflow_run_response_data_relationships_workflow_version_data.py
+-rw-r--r--   0        0        0      908 2023-05-24 17:37:53.897832 fern_persona-0.0.3/src/persona/types/create_an_account_request_data.py
+-rw-r--r--   0        0        0     3575 2023-05-24 17:37:53.897832 fern_persona-0.0.3/src/persona/types/create_an_account_request_data_attributes.py
+-rw-r--r--   0        0        0     1231 2023-05-24 17:37:53.897832 fern_persona-0.0.3/src/persona/types/create_an_account_request_data_attributes_selfie_photo.py
+-rw-r--r--   0        0        0     1113 2023-05-24 17:37:53.897832 fern_persona-0.0.3/src/persona/types/create_an_account_request_data_attributes_selfie_photo_data.py
+-rw-r--r--   0        0        0      871 2023-05-24 17:37:53.897832 fern_persona-0.0.3/src/persona/types/create_an_account_response.py
+-rw-r--r--   0        0        0      972 2023-05-24 17:37:53.897832 fern_persona-0.0.3/src/persona/types/create_an_account_response_data.py
+-rw-r--r--   0        0        0     1029 2023-05-24 17:37:53.897832 fern_persona-0.0.3/src/persona/types/create_an_account_response_data_attributes.py
+-rw-r--r--   0        0        0      905 2023-05-24 17:37:53.897832 fern_persona-0.0.3/src/persona/types/create_an_api_key_request_data.py
+-rw-r--r--   0        0        0     1804 2023-05-24 17:37:53.897832 fern_persona-0.0.3/src/persona/types/create_an_api_key_request_data_attributes.py
+-rw-r--r--   0        0        0      868 2023-05-24 17:37:53.897832 fern_persona-0.0.3/src/persona/types/create_an_api_key_response.py
+-rw-r--r--   0        0        0      969 2023-05-24 17:37:53.897832 fern_persona-0.0.3/src/persona/types/create_an_api_key_response_data.py
+-rw-r--r--   0        0        0     1582 2023-05-24 17:37:53.897832 fern_persona-0.0.3/src/persona/types/create_an_api_key_response_data_attributes.py
+-rw-r--r--   0        0        0      963 2023-05-24 17:37:53.897832 fern_persona-0.0.3/src/persona/types/create_an_email_address_list_item_request_data.py
+-rw-r--r--   0        0        0     1228 2023-05-24 17:37:53.897832 fern_persona-0.0.3/src/persona/types/create_an_email_address_list_item_request_data_attributes.py
+-rw-r--r--   0        0        0      926 2023-05-24 17:37:53.897832 fern_persona-0.0.3/src/persona/types/create_an_email_address_list_item_response.py
+-rw-r--r--   0        0        0     1264 2023-05-24 17:37:53.897832 fern_persona-0.0.3/src/persona/types/create_an_email_address_list_item_response_data.py
+-rw-r--r--   0        0        0     1262 2023-05-24 17:37:53.897832 fern_persona-0.0.3/src/persona/types/create_an_email_address_list_item_response_data_attributes.py
+-rw-r--r--   0        0        0     1017 2023-05-24 17:37:53.897832 fern_persona-0.0.3/src/persona/types/create_an_email_address_list_item_response_data_relationships.py
+-rw-r--r--   0        0        0      818 2023-05-24 17:37:53.897832 fern_persona-0.0.3/src/persona/types/create_an_email_address_list_item_response_data_relationships_creator.py
+-rw-r--r--   0        0        0      946 2023-05-24 17:37:53.897832 fern_persona-0.0.3/src/persona/types/create_an_email_address_list_request_data.py
+-rw-r--r--   0        0        0      849 2023-05-24 17:37:53.897832 fern_persona-0.0.3/src/persona/types/create_an_email_address_list_request_data_attributes.py
+-rw-r--r--   0        0        0      751 2023-05-24 17:37:53.897832 fern_persona-0.0.3/src/persona/types/create_an_email_address_list_response.py
+-rw-r--r--   0        0        0      987 2023-05-24 17:37:53.897832 fern_persona-0.0.3/src/persona/types/create_an_email_address_verification_request_data.py
+-rw-r--r--   0        0        0     1487 2023-05-24 17:37:53.897832 fern_persona-0.0.3/src/persona/types/create_an_email_address_verification_request_data_attributes.py
+-rw-r--r--   0        0        0      941 2023-05-24 17:37:53.897832 fern_persona-0.0.3/src/persona/types/create_an_email_address_verification_response.py
+-rw-r--r--   0        0        0     1051 2023-05-24 17:37:53.897832 fern_persona-0.0.3/src/persona/types/create_an_email_address_verification_response_data.py
+-rw-r--r--   0        0        0     1855 2023-05-24 17:37:53.897832 fern_persona-0.0.3/src/persona/types/create_an_email_address_verification_response_data_attributes.py
+-rw-r--r--   0        0        0      781 2023-05-24 17:37:53.897832 fern_persona-0.0.3/src/persona/types/create_an_email_address_verification_response_data_attributes_metadata.py
+-rw-r--r--   0        0        0      908 2023-05-24 17:37:53.897832 fern_persona-0.0.3/src/persona/types/create_an_inquiry_request_data.py
+-rw-r--r--   0        0        0     3293 2023-05-24 17:37:53.897832 fern_persona-0.0.3/src/persona/types/create_an_inquiry_request_data_attributes.py
+-rw-r--r--   0        0        0     2262 2023-05-24 17:37:53.897832 fern_persona-0.0.3/src/persona/types/create_an_inquiry_request_data_attributes_fields.py
+-rw-r--r--   0        0        0      871 2023-05-24 17:37:53.897832 fern_persona-0.0.3/src/persona/types/create_an_inquiry_response.py
+-rw-r--r--   0        0        0     1149 2023-05-24 17:37:53.897832 fern_persona-0.0.3/src/persona/types/create_an_inquiry_response_data.py
+-rw-r--r--   0        0        0     1202 2023-05-24 17:37:53.897832 fern_persona-0.0.3/src/persona/types/create_an_inquiry_response_data_attributes.py
+-rw-r--r--   0        0        0     1569 2023-05-24 17:37:53.897832 fern_persona-0.0.3/src/persona/types/create_an_inquiry_response_data_relationships.py
+-rw-r--r--   0        0        0      979 2023-05-24 17:37:53.897832 fern_persona-0.0.3/src/persona/types/create_an_inquiry_response_data_relationships_account.py
+-rw-r--r--   0        0        0      831 2023-05-24 17:37:53.897832 fern_persona-0.0.3/src/persona/types/create_an_inquiry_response_data_relationships_account_data.py
+-rw-r--r--   0        0        0      818 2023-05-24 17:37:53.901832 fern_persona-0.0.3/src/persona/types/create_an_inquiry_response_data_relationships_reports.py
+-rw-r--r--   0        0        0      983 2023-05-24 17:37:53.901832 fern_persona-0.0.3/src/persona/types/create_an_inquiry_response_data_relationships_template.py
+-rw-r--r--   0        0        0      832 2023-05-24 17:37:53.901832 fern_persona-0.0.3/src/persona/types/create_an_inquiry_response_data_relationships_template_data.py
+-rw-r--r--   0        0        0     1029 2023-05-24 17:37:53.901832 fern_persona-0.0.3/src/persona/types/create_an_inquiry_response_data_relationships_verifications.py
+-rw-r--r--   0        0        0      841 2023-05-24 17:37:53.901832 fern_persona-0.0.3/src/persona/types/create_an_inquiry_response_data_relationships_verifications_data_item.py
+-rw-r--r--   0        0        0      951 2023-05-24 17:37:53.901832 fern_persona-0.0.3/src/persona/types/create_an_ip_address_list_item_request_data.py
+-rw-r--r--   0        0        0     1098 2023-05-24 17:37:53.901832 fern_persona-0.0.3/src/persona/types/create_an_ip_address_list_item_request_data_attributes.py
+-rw-r--r--   0        0        0      934 2023-05-24 17:37:53.901832 fern_persona-0.0.3/src/persona/types/create_an_ip_address_list_request_data.py
+-rw-r--r--   0        0        0      846 2023-05-24 17:37:53.901832 fern_persona-0.0.3/src/persona/types/create_an_ip_address_list_request_data_attributes.py
+-rw-r--r--   0        0        0      748 2023-05-24 17:37:53.901832 fern_persona-0.0.3/src/persona/types/create_an_ip_address_list_response.py
+-rw-r--r--   0        0        0      848 2023-05-24 17:37:53.901832 fern_persona-0.0.3/src/persona/types/decline_an_inquiry_request_meta.py
+-rw-r--r--   0        0        0      875 2023-05-24 17:37:53.901832 fern_persona-0.0.3/src/persona/types/decline_an_inquiry_response.py
+-rw-r--r--   0        0        0     1156 2023-05-24 17:37:53.901832 fern_persona-0.0.3/src/persona/types/decline_an_inquiry_response_data.py
+-rw-r--r--   0        0        0     1196 2023-05-24 17:37:53.901832 fern_persona-0.0.3/src/persona/types/decline_an_inquiry_response_data_attributes.py
+-rw-r--r--   0        0        0     1582 2023-05-24 17:37:53.901832 fern_persona-0.0.3/src/persona/types/decline_an_inquiry_response_data_relationships.py
+-rw-r--r--   0        0        0      983 2023-05-24 17:37:53.901832 fern_persona-0.0.3/src/persona/types/decline_an_inquiry_response_data_relationships_account.py
+-rw-r--r--   0        0        0      832 2023-05-24 17:37:53.901832 fern_persona-0.0.3/src/persona/types/decline_an_inquiry_response_data_relationships_account_data.py
+-rw-r--r--   0        0        0      819 2023-05-24 17:37:53.901832 fern_persona-0.0.3/src/persona/types/decline_an_inquiry_response_data_relationships_reports.py
+-rw-r--r--   0        0        0      987 2023-05-24 17:37:53.901832 fern_persona-0.0.3/src/persona/types/decline_an_inquiry_response_data_relationships_template.py
+-rw-r--r--   0        0        0      833 2023-05-24 17:37:53.901832 fern_persona-0.0.3/src/persona/types/decline_an_inquiry_response_data_relationships_template_data.py
+-rw-r--r--   0        0        0     1033 2023-05-24 17:37:53.901832 fern_persona-0.0.3/src/persona/types/decline_an_inquiry_response_data_relationships_verifications.py
+-rw-r--r--   0        0        0      842 2023-05-24 17:37:53.901832 fern_persona-0.0.3/src/persona/types/decline_an_inquiry_response_data_relationships_verifications_data_item.py
+-rw-r--r--   0        0        0      903 2023-05-24 17:37:53.901832 fern_persona-0.0.3/src/persona/types/dismiss_matches_request_data.py
+-rw-r--r--   0        0        0     1622 2023-05-24 17:37:53.901832 fern_persona-0.0.3/src/persona/types/dismiss_matches_request_data_attributes.py
+-rw-r--r--   0        0        0      780 2023-05-24 17:37:53.901832 fern_persona-0.0.3/src/persona/types/dismiss_matches_request_data_attributes_dismiss_type.py
+-rw-r--r--   0        0        0      866 2023-05-24 17:37:53.901832 fern_persona-0.0.3/src/persona/types/dismiss_matches_response.py
+-rw-r--r--   0        0        0     1140 2023-05-24 17:37:53.901832 fern_persona-0.0.3/src/persona/types/dismiss_matches_response_data.py
+-rw-r--r--   0        0        0     1271 2023-05-24 17:37:53.901832 fern_persona-0.0.3/src/persona/types/dismiss_matches_response_data_attributes.py
+-rw-r--r--   0        0        0     1467 2023-05-24 17:37:53.901832 fern_persona-0.0.3/src/persona/types/dismiss_matches_response_data_relationships.py
+-rw-r--r--   0        0        0      804 2023-05-24 17:37:53.901832 fern_persona-0.0.3/src/persona/types/dismiss_matches_response_data_relationships_account.py
+-rw-r--r--   0        0        0      804 2023-05-24 17:37:53.901832 fern_persona-0.0.3/src/persona/types/dismiss_matches_response_data_relationships_inquiry.py
+-rw-r--r--   0        0        0     1003 2023-05-24 17:37:53.901832 fern_persona-0.0.3/src/persona/types/dismiss_matches_response_data_relationships_report_template.py
+-rw-r--r--   0        0        0      837 2023-05-24 17:37:53.901832 fern_persona-0.0.3/src/persona/types/dismiss_matches_response_data_relationships_report_template_data.py
+-rw-r--r--   0        0        0      959 2023-05-24 17:37:53.901832 fern_persona-0.0.3/src/persona/types/expire_an_api_key_request_meta.py
+-rw-r--r--   0        0        0      868 2023-05-24 17:37:53.901832 fern_persona-0.0.3/src/persona/types/expire_an_api_key_response.py
+-rw-r--r--   0        0        0      969 2023-05-24 17:37:53.901832 fern_persona-0.0.3/src/persona/types/expire_an_api_key_response_data.py
+-rw-r--r--   0        0        0     1582 2023-05-24 17:37:53.901832 fern_persona-0.0.3/src/persona/types/expire_an_api_key_response_data_attributes.py
+-rw-r--r--   0        0        0      871 2023-05-24 17:37:53.901832 fern_persona-0.0.3/src/persona/types/expire_an_inquiry_response.py
+-rw-r--r--   0        0        0     1149 2023-05-24 17:37:53.901832 fern_persona-0.0.3/src/persona/types/expire_an_inquiry_response_data.py
+-rw-r--r--   0        0        0     1195 2023-05-24 17:37:53.901832 fern_persona-0.0.3/src/persona/types/expire_an_inquiry_response_data_attributes.py
+-rw-r--r--   0        0        0     1569 2023-05-24 17:37:53.901832 fern_persona-0.0.3/src/persona/types/expire_an_inquiry_response_data_relationships.py
+-rw-r--r--   0        0        0      979 2023-05-24 17:37:53.901832 fern_persona-0.0.3/src/persona/types/expire_an_inquiry_response_data_relationships_account.py
+-rw-r--r--   0        0        0      831 2023-05-24 17:37:53.901832 fern_persona-0.0.3/src/persona/types/expire_an_inquiry_response_data_relationships_account_data.py
+-rw-r--r--   0        0        0      818 2023-05-24 17:37:53.901832 fern_persona-0.0.3/src/persona/types/expire_an_inquiry_response_data_relationships_reports.py
+-rw-r--r--   0        0        0      983 2023-05-24 17:37:53.901832 fern_persona-0.0.3/src/persona/types/expire_an_inquiry_response_data_relationships_template.py
+-rw-r--r--   0        0        0      832 2023-05-24 17:37:53.901832 fern_persona-0.0.3/src/persona/types/expire_an_inquiry_response_data_relationships_template_data.py
+-rw-r--r--   0        0        0     1029 2023-05-24 17:37:53.901832 fern_persona-0.0.3/src/persona/types/expire_an_inquiry_response_data_relationships_verifications.py
+-rw-r--r--   0        0        0      841 2023-05-24 17:37:53.901832 fern_persona-0.0.3/src/persona/types/expire_an_inquiry_response_data_relationships_verifications_data_item.py
+-rw-r--r--   0        0        0      903 2023-05-24 17:37:53.901832 fern_persona-0.0.3/src/persona/types/generate_a_one_time_link_request_meta.py
+-rw-r--r--   0        0        0     1038 2023-05-24 17:37:53.901832 fern_persona-0.0.3/src/persona/types/generate_a_one_time_link_response.py
+-rw-r--r--   0        0        0     1188 2023-05-24 17:37:53.901832 fern_persona-0.0.3/src/persona/types/generate_a_one_time_link_response_data.py
+-rw-r--r--   0        0        0     3746 2023-05-24 17:37:53.901832 fern_persona-0.0.3/src/persona/types/generate_a_one_time_link_response_data_attributes.py
+-rw-r--r--   0        0        0     2163 2023-05-24 17:37:53.901832 fern_persona-0.0.3/src/persona/types/generate_a_one_time_link_response_data_attributes_behaviors.py
+-rw-r--r--   0        0        0     4475 2023-05-24 17:37:53.901832 fern_persona-0.0.3/src/persona/types/generate_a_one_time_link_response_data_attributes_fields.py
+-rw-r--r--   0        0        0      849 2023-05-24 17:37:53.901832 fern_persona-0.0.3/src/persona/types/generate_a_one_time_link_response_data_attributes_fields_address_city.py
+-rw-r--r--   0        0        0      855 2023-05-24 17:37:53.901832 fern_persona-0.0.3/src/persona/types/generate_a_one_time_link_response_data_attributes_fields_address_postal_code.py
+-rw-r--r--   0        0        0      852 2023-05-24 17:37:53.901832 fern_persona-0.0.3/src/persona/types/generate_a_one_time_link_response_data_attributes_fields_address_street_1.py
+-rw-r--r--   0        0        0      852 2023-05-24 17:37:53.901832 fern_persona-0.0.3/src/persona/types/generate_a_one_time_link_response_data_attributes_fields_address_street_2.py
+-rw-r--r--   0        0        0      856 2023-05-24 17:37:53.901832 fern_persona-0.0.3/src/persona/types/generate_a_one_time_link_response_data_attributes_fields_address_subdivision.py
+-rw-r--r--   0        0        0      847 2023-05-24 17:37:53.901832 fern_persona-0.0.3/src/persona/types/generate_a_one_time_link_response_data_attributes_fields_birthdate.py
+-rw-r--r--   0        0        0      850 2023-05-24 17:37:53.901832 fern_persona-0.0.3/src/persona/types/generate_a_one_time_link_response_data_attributes_fields_email_address.py
+-rw-r--r--   0        0        0      858 2023-05-24 17:37:53.901832 fern_persona-0.0.3/src/persona/types/generate_a_one_time_link_response_data_attributes_fields_identification_number.py
+-rw-r--r--   0        0        0      847 2023-05-24 17:37:53.901832 fern_persona-0.0.3/src/persona/types/generate_a_one_time_link_response_data_attributes_fields_name_first.py
+-rw-r--r--   0        0        0      846 2023-05-24 17:37:53.901832 fern_persona-0.0.3/src/persona/types/generate_a_one_time_link_response_data_attributes_fields_name_last.py
+-rw-r--r--   0        0        0      848 2023-05-24 17:37:53.901832 fern_persona-0.0.3/src/persona/types/generate_a_one_time_link_response_data_attributes_fields_name_middle.py
+-rw-r--r--   0        0        0      849 2023-05-24 17:37:53.901832 fern_persona-0.0.3/src/persona/types/generate_a_one_time_link_response_data_attributes_fields_phone_number.py
+-rw-r--r--   0        0        0     3265 2023-05-24 17:37:53.901832 fern_persona-0.0.3/src/persona/types/generate_a_one_time_link_response_data_relationships.py
+-rw-r--r--   0        0        0     1001 2023-05-24 17:37:53.901832 fern_persona-0.0.3/src/persona/types/generate_a_one_time_link_response_data_relationships_account.py
+-rw-r--r--   0        0        0      836 2023-05-24 17:37:53.901832 fern_persona-0.0.3/src/persona/types/generate_a_one_time_link_response_data_relationships_account_data.py
+-rw-r--r--   0        0        0     1035 2023-05-24 17:37:53.901832 fern_persona-0.0.3/src/persona/types/generate_a_one_time_link_response_data_relationships_documents.py
+-rw-r--r--   0        0        0      842 2023-05-24 17:37:53.901832 fern_persona-0.0.3/src/persona/types/generate_a_one_time_link_response_data_relationships_documents_data_item.py
+-rw-r--r--   0        0        0     1034 2023-05-24 17:37:53.901832 fern_persona-0.0.3/src/persona/types/generate_a_one_time_link_response_data_relationships_inquiry_template.py
+-rw-r--r--   0        0        0      844 2023-05-24 17:37:53.901832 fern_persona-0.0.3/src/persona/types/generate_a_one_time_link_response_data_relationships_inquiry_template_data.py
+-rw-r--r--   0        0        0     1063 2023-05-24 17:37:53.901832 fern_persona-0.0.3/src/persona/types/generate_a_one_time_link_response_data_relationships_inquiry_template_version.py
+-rw-r--r--   0        0        0      851 2023-05-24 17:37:53.901832 fern_persona-0.0.3/src/persona/types/generate_a_one_time_link_response_data_relationships_inquiry_template_version_data.py
+-rw-r--r--   0        0        0      823 2023-05-24 17:37:53.901832 fern_persona-0.0.3/src/persona/types/generate_a_one_time_link_response_data_relationships_reports.py
+-rw-r--r--   0        0        0      811 2023-05-24 17:37:53.901832 fern_persona-0.0.3/src/persona/types/generate_a_one_time_link_response_data_relationships_reviewer.py
+-rw-r--r--   0        0        0      823 2023-05-24 17:37:53.901832 fern_persona-0.0.3/src/persona/types/generate_a_one_time_link_response_data_relationships_selfies.py
+-rw-r--r--   0        0        0     1031 2023-05-24 17:37:53.901832 fern_persona-0.0.3/src/persona/types/generate_a_one_time_link_response_data_relationships_sessions.py
+-rw-r--r--   0        0        0      841 2023-05-24 17:37:53.901832 fern_persona-0.0.3/src/persona/types/generate_a_one_time_link_response_data_relationships_sessions_data_item.py
+-rw-r--r--   0        0        0      811 2023-05-24 17:37:53.901832 fern_persona-0.0.3/src/persona/types/generate_a_one_time_link_response_data_relationships_template.py
+-rw-r--r--   0        0        0     1051 2023-05-24 17:37:53.901832 fern_persona-0.0.3/src/persona/types/generate_a_one_time_link_response_data_relationships_verifications.py
+-rw-r--r--   0        0        0      846 2023-05-24 17:37:53.901832 fern_persona-0.0.3/src/persona/types/generate_a_one_time_link_response_data_relationships_verifications_data_item.py
+-rw-r--r--   0        0        0      970 2023-05-24 17:37:53.901832 fern_persona-0.0.3/src/persona/types/generate_a_one_time_link_response_meta.py
+-rw-r--r--   0        0        0      884 2023-05-24 17:37:53.901832 fern_persona-0.0.3/src/persona/types/import_an_account_request_data.py
+-rw-r--r--   0        0        0      921 2023-05-24 17:37:53.901832 fern_persona-0.0.3/src/persona/types/import_an_account_request_data_file.py
+-rw-r--r--   0        0        0      871 2023-05-24 17:37:53.901832 fern_persona-0.0.3/src/persona/types/import_an_account_response.py
+-rw-r--r--   0        0        0      972 2023-05-24 17:37:53.901832 fern_persona-0.0.3/src/persona/types/import_an_account_response_data.py
+-rw-r--r--   0        0        0     1241 2023-05-24 17:37:53.901832 fern_persona-0.0.3/src/persona/types/import_an_account_response_data_attributes.py
+-rw-r--r--   0        0        0      941 2023-05-24 17:37:53.901832 fern_persona-0.0.3/src/persona/types/import_email_address_lists_request_data.py
+-rw-r--r--   0        0        0     1072 2023-05-24 17:37:53.901832 fern_persona-0.0.3/src/persona/types/import_email_address_lists_request_data_attributes.py
+-rw-r--r--   0        0        0      939 2023-05-24 17:37:53.901832 fern_persona-0.0.3/src/persona/types/import_email_address_lists_request_data_attributes_file.py
+-rw-r--r--   0        0        0      904 2023-05-24 17:37:53.901832 fern_persona-0.0.3/src/persona/types/import_email_address_lists_response.py
+-rw-r--r--   0        0        0     1005 2023-05-24 17:37:53.901832 fern_persona-0.0.3/src/persona/types/import_email_address_lists_response_data.py
+-rw-r--r--   0        0        0     1249 2023-05-24 17:37:53.901832 fern_persona-0.0.3/src/persona/types/import_email_address_lists_response_data_attributes.py
+-rw-r--r--   0        0        0      908 2023-05-24 17:37:53.901832 fern_persona-0.0.3/src/persona/types/import_face_lists_request_data.py
+-rw-r--r--   0        0        0     1152 2023-05-24 17:37:53.901832 fern_persona-0.0.3/src/persona/types/import_face_lists_request_data_attributes.py
+-rw-r--r--   0        0        0      941 2023-05-24 17:37:53.901832 fern_persona-0.0.3/src/persona/types/import_face_lists_request_data_attributes_image_files_item.py
+-rw-r--r--   0        0        0      871 2023-05-24 17:37:53.901832 fern_persona-0.0.3/src/persona/types/import_face_lists_response.py
+-rw-r--r--   0        0        0      972 2023-05-24 17:37:53.901832 fern_persona-0.0.3/src/persona/types/import_face_lists_response_data.py
+-rw-r--r--   0        0        0     1241 2023-05-24 17:37:53.901832 fern_persona-0.0.3/src/persona/types/import_face_lists_response_data_attributes.py
+-rw-r--r--   0        0        0      936 2023-05-24 17:37:53.901832 fern_persona-0.0.3/src/persona/types/import_geolocation_lists_request_data.py
+-rw-r--r--   0        0        0     1067 2023-05-24 17:37:53.901832 fern_persona-0.0.3/src/persona/types/import_geolocation_lists_request_data_attributes.py
+-rw-r--r--   0        0        0      938 2023-05-24 17:37:53.901832 fern_persona-0.0.3/src/persona/types/import_geolocation_lists_request_data_attributes_file.py
+-rw-r--r--   0        0        0      899 2023-05-24 17:37:53.901832 fern_persona-0.0.3/src/persona/types/import_geolocation_lists_response.py
+-rw-r--r--   0        0        0     1000 2023-05-24 17:37:53.901832 fern_persona-0.0.3/src/persona/types/import_geolocation_lists_response_data.py
+-rw-r--r--   0        0        0     1248 2023-05-24 17:37:53.901832 fern_persona-0.0.3/src/persona/types/import_geolocation_lists_response_data_attributes.py
+-rw-r--r--   0        0        0      975 2023-05-24 17:37:53.901832 fern_persona-0.0.3/src/persona/types/import_government_id_number_lists_request_data.py
+-rw-r--r--   0        0        0     1106 2023-05-24 17:37:53.901832 fern_persona-0.0.3/src/persona/types/import_government_id_number_lists_request_data_attributes.py
+-rw-r--r--   0        0        0      945 2023-05-24 17:37:53.901832 fern_persona-0.0.3/src/persona/types/import_government_id_number_lists_request_data_attributes_file.py
+-rw-r--r--   0        0        0      929 2023-05-24 17:37:53.901832 fern_persona-0.0.3/src/persona/types/import_government_id_number_lists_response.py
+-rw-r--r--   0        0        0     1039 2023-05-24 17:37:53.905832 fern_persona-0.0.3/src/persona/types/import_government_id_number_lists_response_data.py
+-rw-r--r--   0        0        0     1255 2023-05-24 17:37:53.905832 fern_persona-0.0.3/src/persona/types/import_government_id_number_lists_response_data_attributes.py
+-rw-r--r--   0        0        0      929 2023-05-24 17:37:53.905832 fern_persona-0.0.3/src/persona/types/import_ip_address_lists_request_data.py
+-rw-r--r--   0        0        0     1060 2023-05-24 17:37:53.905832 fern_persona-0.0.3/src/persona/types/import_ip_address_lists_request_data_attributes.py
+-rw-r--r--   0        0        0      936 2023-05-24 17:37:53.905832 fern_persona-0.0.3/src/persona/types/import_ip_address_lists_request_data_attributes_file.py
+-rw-r--r--   0        0        0      892 2023-05-24 17:37:53.905832 fern_persona-0.0.3/src/persona/types/import_ip_address_lists_response.py
+-rw-r--r--   0        0        0      993 2023-05-24 17:37:53.905832 fern_persona-0.0.3/src/persona/types/import_ip_address_lists_response_data.py
+-rw-r--r--   0        0        0     1246 2023-05-24 17:37:53.905832 fern_persona-0.0.3/src/persona/types/import_ip_address_lists_response_data_attributes.py
+-rw-r--r--   0        0        0      908 2023-05-24 17:37:53.905832 fern_persona-0.0.3/src/persona/types/import_name_lists_request_data.py
+-rw-r--r--   0        0        0     1039 2023-05-24 17:37:53.905832 fern_persona-0.0.3/src/persona/types/import_name_lists_request_data_attributes.py
+-rw-r--r--   0        0        0      931 2023-05-24 17:37:53.905832 fern_persona-0.0.3/src/persona/types/import_name_lists_request_data_attributes_file.py
+-rw-r--r--   0        0        0      871 2023-05-24 17:37:53.905832 fern_persona-0.0.3/src/persona/types/import_name_lists_response.py
+-rw-r--r--   0        0        0      972 2023-05-24 17:37:53.905832 fern_persona-0.0.3/src/persona/types/import_name_lists_response_data.py
+-rw-r--r--   0        0        0     1241 2023-05-24 17:37:53.905832 fern_persona-0.0.3/src/persona/types/import_name_lists_response_data_attributes.py
+-rw-r--r--   0        0        0      937 2023-05-24 17:37:53.905832 fern_persona-0.0.3/src/persona/types/import_phone_number_lists_request_data.py
+-rw-r--r--   0        0        0     1068 2023-05-24 17:37:53.905832 fern_persona-0.0.3/src/persona/types/import_phone_number_lists_request_data_attributes.py
+-rw-r--r--   0        0        0      938 2023-05-24 17:37:53.905832 fern_persona-0.0.3/src/persona/types/import_phone_number_lists_request_data_attributes_file.py
+-rw-r--r--   0        0        0      900 2023-05-24 17:37:53.905832 fern_persona-0.0.3/src/persona/types/import_phone_number_lists_response.py
+-rw-r--r--   0        0        0     1001 2023-05-24 17:37:53.905832 fern_persona-0.0.3/src/persona/types/import_phone_number_lists_response_data.py
+-rw-r--r--   0        0        0     1248 2023-05-24 17:37:53.905832 fern_persona-0.0.3/src/persona/types/import_phone_number_lists_response_data_attributes.py
+-rw-r--r--   0        0        0     1029 2023-05-24 17:37:53.905832 fern_persona-0.0.3/src/persona/types/list_all_accounts_response.py
+-rw-r--r--   0        0        0      989 2023-05-24 17:37:53.905832 fern_persona-0.0.3/src/persona/types/list_all_accounts_response_data_item.py
+-rw-r--r--   0        0        0     1040 2023-05-24 17:37:53.905832 fern_persona-0.0.3/src/persona/types/list_all_accounts_response_data_item_attributes.py
+-rw-r--r--   0        0        0      817 2023-05-24 17:37:53.905832 fern_persona-0.0.3/src/persona/types/list_all_accounts_response_links.py
+-rw-r--r--   0        0        0     1024 2023-05-24 17:37:53.905832 fern_persona-0.0.3/src/persona/types/list_all_api_keys_response.py
+-rw-r--r--   0        0        0      986 2023-05-24 17:37:53.905832 fern_persona-0.0.3/src/persona/types/list_all_api_keys_response_data_item.py
+-rw-r--r--   0        0        0     1554 2023-05-24 17:37:53.905832 fern_persona-0.0.3/src/persona/types/list_all_api_keys_response_data_item_attributes.py
+-rw-r--r--   0        0        0      823 2023-05-24 17:37:53.905832 fern_persona-0.0.3/src/persona/types/list_all_api_keys_response_links.py
+-rw-r--r--   0        0        0     1008 2023-05-24 17:37:53.905832 fern_persona-0.0.3/src/persona/types/list_all_cases_response.py
+-rw-r--r--   0        0        0     1158 2023-05-24 17:37:53.905832 fern_persona-0.0.3/src/persona/types/list_all_cases_response_data_item.py
+-rw-r--r--   0        0        0     1779 2023-05-24 17:37:53.905832 fern_persona-0.0.3/src/persona/types/list_all_cases_response_data_item_attributes.py
+-rw-r--r--   0        0        0     1089 2023-05-24 17:37:53.905832 fern_persona-0.0.3/src/persona/types/list_all_cases_response_data_item_relationships.py
+-rw-r--r--   0        0        0     1005 2023-05-24 17:37:53.905832 fern_persona-0.0.3/src/persona/types/list_all_cases_response_data_item_relationships_case_template.py
+-rw-r--r--   0        0        0      837 2023-05-24 17:37:53.905832 fern_persona-0.0.3/src/persona/types/list_all_cases_response_data_item_relationships_case_template_data.py
+-rw-r--r--   0        0        0      821 2023-05-24 17:37:53.905832 fern_persona-0.0.3/src/persona/types/list_all_cases_response_links.py
+-rw-r--r--   0        0        0      740 2023-05-24 17:37:53.905832 fern_persona-0.0.3/src/persona/types/list_all_events_response.py
+-rw-r--r--   0        0        0     1036 2023-05-24 17:37:53.905832 fern_persona-0.0.3/src/persona/types/list_all_inquiries_response.py
+-rw-r--r--   0        0        0     1186 2023-05-24 17:37:53.905832 fern_persona-0.0.3/src/persona/types/list_all_inquiries_response_data_item.py
+-rw-r--r--   0        0        0     1200 2023-05-24 17:37:53.905832 fern_persona-0.0.3/src/persona/types/list_all_inquiries_response_data_item_attributes.py
+-rw-r--r--   0        0        0     1887 2023-05-24 17:37:53.905832 fern_persona-0.0.3/src/persona/types/list_all_inquiries_response_data_item_relationships.py
+-rw-r--r--   0        0        0     1000 2023-05-24 17:37:53.905832 fern_persona-0.0.3/src/persona/types/list_all_inquiries_response_data_item_relationships_account.py
+-rw-r--r--   0        0        0      836 2023-05-24 17:37:53.905832 fern_persona-0.0.3/src/persona/types/list_all_inquiries_response_data_item_relationships_account_data.py
+-rw-r--r--   0        0        0      823 2023-05-24 17:37:53.905832 fern_persona-0.0.3/src/persona/types/list_all_inquiries_response_data_item_relationships_reports.py
+-rw-r--r--   0        0        0     1030 2023-05-24 17:37:53.905832 fern_persona-0.0.3/src/persona/types/list_all_inquiries_response_data_item_relationships_sessions.py
+-rw-r--r--   0        0        0      841 2023-05-24 17:37:53.905832 fern_persona-0.0.3/src/persona/types/list_all_inquiries_response_data_item_relationships_sessions_data_item.py
+-rw-r--r--   0        0        0     1004 2023-05-24 17:37:53.905832 fern_persona-0.0.3/src/persona/types/list_all_inquiries_response_data_item_relationships_template.py
+-rw-r--r--   0        0        0      837 2023-05-24 17:37:53.905832 fern_persona-0.0.3/src/persona/types/list_all_inquiries_response_data_item_relationships_template_data.py
+-rw-r--r--   0        0        0     1050 2023-05-24 17:37:53.905832 fern_persona-0.0.3/src/persona/types/list_all_inquiries_response_data_item_relationships_verifications.py
+-rw-r--r--   0        0        0      846 2023-05-24 17:37:53.905832 fern_persona-0.0.3/src/persona/types/list_all_inquiries_response_data_item_relationships_verifications_data_item.py
+-rw-r--r--   0        0        0      818 2023-05-24 17:37:53.905832 fern_persona-0.0.3/src/persona/types/list_all_inquiries_response_links.py
+-rw-r--r--   0        0        0      739 2023-05-24 17:37:53.905832 fern_persona-0.0.3/src/persona/types/list_all_lists_response.py
+-rw-r--r--   0        0        0      863 2023-05-24 17:37:53.905832 fern_persona-0.0.3/src/persona/types/redact_a_report_response.py
+-rw-r--r--   0        0        0      964 2023-05-24 17:37:53.905832 fern_persona-0.0.3/src/persona/types/redact_a_report_response_data.py
+-rw-r--r--   0        0        0     1225 2023-05-24 17:37:53.905832 fern_persona-0.0.3/src/persona/types/redact_a_report_response_data_attributes.py
+-rw-r--r--   0        0        0      871 2023-05-24 17:37:53.905832 fern_persona-0.0.3/src/persona/types/redact_an_account_response.py
+-rw-r--r--   0        0        0      972 2023-05-24 17:37:53.905832 fern_persona-0.0.3/src/persona/types/redact_an_account_response_data.py
+-rw-r--r--   0        0        0     1896 2023-05-24 17:37:53.905832 fern_persona-0.0.3/src/persona/types/redact_an_account_response_data_attributes.py
+-rw-r--r--   0        0        0      871 2023-05-24 17:37:53.905832 fern_persona-0.0.3/src/persona/types/redact_an_inquiry_response.py
+-rw-r--r--   0        0        0     1149 2023-05-24 17:37:53.905832 fern_persona-0.0.3/src/persona/types/redact_an_inquiry_response_data.py
+-rw-r--r--   0        0        0     1195 2023-05-24 17:37:53.905832 fern_persona-0.0.3/src/persona/types/redact_an_inquiry_response_data_attributes.py
+-rw-r--r--   0        0        0     1569 2023-05-24 17:37:53.905832 fern_persona-0.0.3/src/persona/types/redact_an_inquiry_response_data_relationships.py
+-rw-r--r--   0        0        0      979 2023-05-24 17:37:53.905832 fern_persona-0.0.3/src/persona/types/redact_an_inquiry_response_data_relationships_account.py
+-rw-r--r--   0        0        0      831 2023-05-24 17:37:53.905832 fern_persona-0.0.3/src/persona/types/redact_an_inquiry_response_data_relationships_account_data.py
+-rw-r--r--   0        0        0      818 2023-05-24 17:37:53.905832 fern_persona-0.0.3/src/persona/types/redact_an_inquiry_response_data_relationships_reports.py
+-rw-r--r--   0        0        0      983 2023-05-24 17:37:53.905832 fern_persona-0.0.3/src/persona/types/redact_an_inquiry_response_data_relationships_template.py
+-rw-r--r--   0        0        0      832 2023-05-24 17:37:53.905832 fern_persona-0.0.3/src/persona/types/redact_an_inquiry_response_data_relationships_template_data.py
+-rw-r--r--   0        0        0     1029 2023-05-24 17:37:53.905832 fern_persona-0.0.3/src/persona/types/redact_an_inquiry_response_data_relationships_verifications.py
+-rw-r--r--   0        0        0      841 2023-05-24 17:37:53.905832 fern_persona-0.0.3/src/persona/types/redact_an_inquiry_response_data_relationships_verifications_data_item.py
+-rw-r--r--   0        0        0      858 2023-05-24 17:37:53.905832 fern_persona-0.0.3/src/persona/types/remove_a_tag_1_request_meta.py
+-rw-r--r--   0        0        0      857 2023-05-24 17:37:53.905832 fern_persona-0.0.3/src/persona/types/remove_a_tag_request_meta.py
+-rw-r--r--   0        0        0      961 2023-05-24 17:37:53.905832 fern_persona-0.0.3/src/persona/types/report_action_pause_continuous_monitoring_response.py
+-rw-r--r--   0        0        0     1325 2023-05-24 17:37:53.905832 fern_persona-0.0.3/src/persona/types/report_action_pause_continuous_monitoring_response_data.py
+-rw-r--r--   0        0        0     1294 2023-05-24 17:37:53.905832 fern_persona-0.0.3/src/persona/types/report_action_pause_continuous_monitoring_response_data_attributes.py
+-rw-r--r--   0        0        0     1724 2023-05-24 17:37:53.905832 fern_persona-0.0.3/src/persona/types/report_action_pause_continuous_monitoring_response_data_relationships.py
+-rw-r--r--   0        0        0      827 2023-05-24 17:37:53.905832 fern_persona-0.0.3/src/persona/types/report_action_pause_continuous_monitoring_response_data_relationships_account.py
+-rw-r--r--   0        0        0      827 2023-05-24 17:37:53.905832 fern_persona-0.0.3/src/persona/types/report_action_pause_continuous_monitoring_response_data_relationships_inquiry.py
+-rw-r--r--   0        0        0     1098 2023-05-24 17:37:53.905832 fern_persona-0.0.3/src/persona/types/report_action_pause_continuous_monitoring_response_data_relationships_report_template.py
+-rw-r--r--   0        0        0      860 2023-05-24 17:37:53.905832 fern_persona-0.0.3/src/persona/types/report_action_pause_continuous_monitoring_response_data_relationships_report_template_data.py
+-rw-r--r--   0        0        0      905 2023-05-24 17:37:53.905832 fern_persona-0.0.3/src/persona/types/report_action_re_run_report_response.py
+-rw-r--r--   0        0        0     1209 2023-05-24 17:37:53.905832 fern_persona-0.0.3/src/persona/types/report_action_re_run_report_response_data.py
+-rw-r--r--   0        0        0     1280 2023-05-24 17:37:53.905832 fern_persona-0.0.3/src/persona/types/report_action_re_run_report_response_data_attributes.py
+-rw-r--r--   0        0        0     1584 2023-05-24 17:37:53.905832 fern_persona-0.0.3/src/persona/types/report_action_re_run_report_response_data_relationships.py
+-rw-r--r--   0        0        0      813 2023-05-24 17:37:53.905832 fern_persona-0.0.3/src/persona/types/report_action_re_run_report_response_data_relationships_account.py
+-rw-r--r--   0        0        0      813 2023-05-24 17:37:53.905832 fern_persona-0.0.3/src/persona/types/report_action_re_run_report_response_data_relationships_inquiry.py
+-rw-r--r--   0        0        0     1042 2023-05-24 17:37:53.905832 fern_persona-0.0.3/src/persona/types/report_action_re_run_report_response_data_relationships_report_template.py
+-rw-r--r--   0        0        0      846 2023-05-24 17:37:53.905832 fern_persona-0.0.3/src/persona/types/report_action_re_run_report_response_data_relationships_report_template_data.py
+-rw-r--r--   0        0        0      965 2023-05-24 17:37:53.905832 fern_persona-0.0.3/src/persona/types/report_action_resume_continuous_monitoring_response.py
+-rw-r--r--   0        0        0     1332 2023-05-24 17:37:53.905832 fern_persona-0.0.3/src/persona/types/report_action_resume_continuous_monitoring_response_data.py
+-rw-r--r--   0        0        0     1295 2023-05-24 17:37:53.905832 fern_persona-0.0.3/src/persona/types/report_action_resume_continuous_monitoring_response_data_attributes.py
+-rw-r--r--   0        0        0     1734 2023-05-24 17:37:53.905832 fern_persona-0.0.3/src/persona/types/report_action_resume_continuous_monitoring_response_data_relationships.py
+-rw-r--r--   0        0        0      828 2023-05-24 17:37:53.905832 fern_persona-0.0.3/src/persona/types/report_action_resume_continuous_monitoring_response_data_relationships_account.py
+-rw-r--r--   0        0        0      828 2023-05-24 17:37:53.905832 fern_persona-0.0.3/src/persona/types/report_action_resume_continuous_monitoring_response_data_relationships_inquiry.py
+-rw-r--r--   0        0        0     1102 2023-05-24 17:37:53.905832 fern_persona-0.0.3/src/persona/types/report_action_resume_continuous_monitoring_response_data_relationships_report_template.py
+-rw-r--r--   0        0        0      861 2023-05-24 17:37:53.905832 fern_persona-0.0.3/src/persona/types/report_action_resume_continuous_monitoring_response_data_relationships_report_template_data.py
+-rw-r--r--   0        0        0      861 2023-05-24 17:37:53.905832 fern_persona-0.0.3/src/persona/types/reports_add_a_tag_request_meta.py
+-rw-r--r--   0        0        0      868 2023-05-24 17:37:53.905832 fern_persona-0.0.3/src/persona/types/reports_add_a_tag_response.py
+-rw-r--r--   0        0        0     1144 2023-05-24 17:37:53.905832 fern_persona-0.0.3/src/persona/types/reports_add_a_tag_response_data.py
+-rw-r--r--   0        0        0     1875 2023-05-24 17:37:53.905832 fern_persona-0.0.3/src/persona/types/reports_add_a_tag_response_data_attributes.py
+-rw-r--r--   0        0        0     1473 2023-05-24 17:37:53.905832 fern_persona-0.0.3/src/persona/types/reports_add_a_tag_response_data_relationships.py
+-rw-r--r--   0        0        0      804 2023-05-24 17:37:53.905832 fern_persona-0.0.3/src/persona/types/reports_add_a_tag_response_data_relationships_account.py
+-rw-r--r--   0        0        0      804 2023-05-24 17:37:53.905832 fern_persona-0.0.3/src/persona/types/reports_add_a_tag_response_data_relationships_inquiry.py
+-rw-r--r--   0        0        0     1005 2023-05-24 17:37:53.905832 fern_persona-0.0.3/src/persona/types/reports_add_a_tag_response_data_relationships_report_template.py
+-rw-r--r--   0        0        0      837 2023-05-24 17:37:53.905832 fern_persona-0.0.3/src/persona/types/reports_add_a_tag_response_data_relationships_report_template_data.py
+-rw-r--r--   0        0        0      864 2023-05-24 17:37:53.905832 fern_persona-0.0.3/src/persona/types/reports_remove_a_tag_request_meta.py
+-rw-r--r--   0        0        0      880 2023-05-24 17:37:53.905832 fern_persona-0.0.3/src/persona/types/reports_remove_a_tag_response.py
+-rw-r--r--   0        0        0     1165 2023-05-24 17:37:53.905832 fern_persona-0.0.3/src/persona/types/reports_remove_a_tag_response_data.py
+-rw-r--r--   0        0        0     1878 2023-05-24 17:37:53.905832 fern_persona-0.0.3/src/persona/types/reports_remove_a_tag_response_data_attributes.py
+-rw-r--r--   0        0        0     1503 2023-05-24 17:37:53.905832 fern_persona-0.0.3/src/persona/types/reports_remove_a_tag_response_data_relationships.py
+-rw-r--r--   0        0        0      807 2023-05-24 17:37:53.905832 fern_persona-0.0.3/src/persona/types/reports_remove_a_tag_response_data_relationships_account.py
+-rw-r--r--   0        0        0      807 2023-05-24 17:37:53.905832 fern_persona-0.0.3/src/persona/types/reports_remove_a_tag_response_data_relationships_inquiry.py
+-rw-r--r--   0        0        0     1017 2023-05-24 17:37:53.905832 fern_persona-0.0.3/src/persona/types/reports_remove_a_tag_response_data_relationships_report_template.py
+-rw-r--r--   0        0        0      840 2023-05-24 17:37:53.909833 fern_persona-0.0.3/src/persona/types/reports_remove_a_tag_response_data_relationships_report_template_data.py
+-rw-r--r--   0        0        0      877 2023-05-24 17:37:53.909833 fern_persona-0.0.3/src/persona/types/reports_set_all_tags_request_meta.py
+-rw-r--r--   0        0        0      880 2023-05-24 17:37:53.909833 fern_persona-0.0.3/src/persona/types/reports_set_all_tags_response.py
+-rw-r--r--   0        0        0     1165 2023-05-24 17:37:53.909833 fern_persona-0.0.3/src/persona/types/reports_set_all_tags_response_data.py
+-rw-r--r--   0        0        0     1878 2023-05-24 17:37:53.909833 fern_persona-0.0.3/src/persona/types/reports_set_all_tags_response_data_attributes.py
+-rw-r--r--   0        0        0     1503 2023-05-24 17:37:53.909833 fern_persona-0.0.3/src/persona/types/reports_set_all_tags_response_data_relationships.py
+-rw-r--r--   0        0        0      807 2023-05-24 17:37:53.909833 fern_persona-0.0.3/src/persona/types/reports_set_all_tags_response_data_relationships_account.py
+-rw-r--r--   0        0        0      807 2023-05-24 17:37:53.909833 fern_persona-0.0.3/src/persona/types/reports_set_all_tags_response_data_relationships_inquiry.py
+-rw-r--r--   0        0        0     1017 2023-05-24 17:37:53.909833 fern_persona-0.0.3/src/persona/types/reports_set_all_tags_response_data_relationships_report_template.py
+-rw-r--r--   0        0        0      840 2023-05-24 17:37:53.909833 fern_persona-0.0.3/src/persona/types/reports_set_all_tags_response_data_relationships_report_template_data.py
+-rw-r--r--   0        0        0      999 2023-05-24 17:37:53.909833 fern_persona-0.0.3/src/persona/types/resume_an_inquiry_response.py
+-rw-r--r--   0        0        0     1149 2023-05-24 17:37:53.909833 fern_persona-0.0.3/src/persona/types/resume_an_inquiry_response_data.py
+-rw-r--r--   0        0        0     1195 2023-05-24 17:37:53.909833 fern_persona-0.0.3/src/persona/types/resume_an_inquiry_response_data_attributes.py
+-rw-r--r--   0        0        0     1569 2023-05-24 17:37:53.909833 fern_persona-0.0.3/src/persona/types/resume_an_inquiry_response_data_relationships.py
+-rw-r--r--   0        0        0      979 2023-05-24 17:37:53.909833 fern_persona-0.0.3/src/persona/types/resume_an_inquiry_response_data_relationships_account.py
+-rw-r--r--   0        0        0      831 2023-05-24 17:37:53.909833 fern_persona-0.0.3/src/persona/types/resume_an_inquiry_response_data_relationships_account_data.py
+-rw-r--r--   0        0        0      818 2023-05-24 17:37:53.909833 fern_persona-0.0.3/src/persona/types/resume_an_inquiry_response_data_relationships_reports.py
+-rw-r--r--   0        0        0      983 2023-05-24 17:37:53.909833 fern_persona-0.0.3/src/persona/types/resume_an_inquiry_response_data_relationships_template.py
+-rw-r--r--   0        0        0      832 2023-05-24 17:37:53.909833 fern_persona-0.0.3/src/persona/types/resume_an_inquiry_response_data_relationships_template_data.py
+-rw-r--r--   0        0        0     1029 2023-05-24 17:37:53.909833 fern_persona-0.0.3/src/persona/types/resume_an_inquiry_response_data_relationships_verifications.py
+-rw-r--r--   0        0        0      841 2023-05-24 17:37:53.909833 fern_persona-0.0.3/src/persona/types/resume_an_inquiry_response_data_relationships_verifications_data_item.py
+-rw-r--r--   0        0        0      873 2023-05-24 17:37:53.909833 fern_persona-0.0.3/src/persona/types/resume_an_inquiry_response_meta.py
+-rw-r--r--   0        0        0      928 2023-05-24 17:37:53.909833 fern_persona-0.0.3/src/persona/types/retrieve_a_database_verification_response.py
+-rw-r--r--   0        0        0     1267 2023-05-24 17:37:53.909833 fern_persona-0.0.3/src/persona/types/retrieve_a_database_verification_response_data.py
+-rw-r--r--   0        0        0     1821 2023-05-24 17:37:53.909833 fern_persona-0.0.3/src/persona/types/retrieve_a_database_verification_response_data_attributes.py
+-rw-r--r--   0        0        0     1164 2023-05-24 17:37:53.909833 fern_persona-0.0.3/src/persona/types/retrieve_a_database_verification_response_data_attributes_checks_item.py
+-rw-r--r--   0        0        0      788 2023-05-24 17:37:53.909833 fern_persona-0.0.3/src/persona/types/retrieve_a_database_verification_response_data_attributes_checks_item_metadata.py
+-rw-r--r--   0        0        0     1019 2023-05-24 17:37:53.909833 fern_persona-0.0.3/src/persona/types/retrieve_a_database_verification_response_data_relationships.py
+-rw-r--r--   0        0        0      819 2023-05-24 17:37:53.909833 fern_persona-0.0.3/src/persona/types/retrieve_a_database_verification_response_data_relationships_inquiry.py
+-rw-r--r--   0        0        0      879 2023-05-24 17:37:53.909833 fern_persona-0.0.3/src/persona/types/retrieve_a_document_response.py
+-rw-r--r--   0        0        0     1163 2023-05-24 17:37:53.909833 fern_persona-0.0.3/src/persona/types/retrieve_a_document_response_data.py
+-rw-r--r--   0        0        0     1309 2023-05-24 17:37:53.909833 fern_persona-0.0.3/src/persona/types/retrieve_a_document_response_data_attributes.py
+-rw-r--r--   0        0        0      833 2023-05-24 17:37:53.909833 fern_persona-0.0.3/src/persona/types/retrieve_a_document_response_data_attributes_files_item.py
+-rw-r--r--   0        0        0      961 2023-05-24 17:37:53.909833 fern_persona-0.0.3/src/persona/types/retrieve_a_document_response_data_relationships.py
+-rw-r--r--   0        0        0      987 2023-05-24 17:37:53.909833 fern_persona-0.0.3/src/persona/types/retrieve_a_document_response_data_relationships_inquiry.py
+-rw-r--r--   0        0        0      833 2023-05-24 17:37:53.909833 fern_persona-0.0.3/src/persona/types/retrieve_a_document_response_data_relationships_inquiry_data.py
+-rw-r--r--   0        0        0      945 2023-05-24 17:37:53.909833 fern_persona-0.0.3/src/persona/types/retrieve_a_email_address_verification_response.py
+-rw-r--r--   0        0        0     1297 2023-05-24 17:37:53.909833 fern_persona-0.0.3/src/persona/types/retrieve_a_email_address_verification_response_data.py
+-rw-r--r--   0        0        0     1767 2023-05-24 17:37:53.909833 fern_persona-0.0.3/src/persona/types/retrieve_a_email_address_verification_response_data_attributes.py
+-rw-r--r--   0        0        0      782 2023-05-24 17:37:53.909833 fern_persona-0.0.3/src/persona/types/retrieve_a_email_address_verification_response_data_attributes_metadata.py
+-rw-r--r--   0        0        0     1036 2023-05-24 17:37:53.909833 fern_persona-0.0.3/src/persona/types/retrieve_a_email_address_verification_response_data_relationships.py
+-rw-r--r--   0        0        0      823 2023-05-24 17:37:53.909833 fern_persona-0.0.3/src/persona/types/retrieve_a_email_address_verification_response_data_relationships_inquiry.py
+-rw-r--r--   0        0        0      945 2023-05-24 17:37:53.909833 fern_persona-0.0.3/src/persona/types/retrieve_a_government_id_verification_response.py
+-rw-r--r--   0        0        0     1297 2023-05-24 17:37:53.909833 fern_persona-0.0.3/src/persona/types/retrieve_a_government_id_verification_response_data.py
+-rw-r--r--   0        0        0     3024 2023-05-24 17:37:53.909833 fern_persona-0.0.3/src/persona/types/retrieve_a_government_id_verification_response_data_attributes.py
+-rw-r--r--   0        0        0     1181 2023-05-24 17:37:53.909833 fern_persona-0.0.3/src/persona/types/retrieve_a_government_id_verification_response_data_attributes_checks_item.py
+-rw-r--r--   0        0        0      792 2023-05-24 17:37:53.909833 fern_persona-0.0.3/src/persona/types/retrieve_a_government_id_verification_response_data_attributes_checks_item_metadata.py
+-rw-r--r--   0        0        0     1142 2023-05-24 17:37:53.909833 fern_persona-0.0.3/src/persona/types/retrieve_a_government_id_verification_response_data_attributes_photo_urls_item.py
+-rw-r--r--   0        0        0     1298 2023-05-24 17:37:53.909833 fern_persona-0.0.3/src/persona/types/retrieve_a_government_id_verification_response_data_relationships.py
+-rw-r--r--   0        0        0     1057 2023-05-24 17:37:53.909833 fern_persona-0.0.3/src/persona/types/retrieve_a_government_id_verification_response_data_relationships_document.py
+-rw-r--r--   0        0        0      850 2023-05-24 17:37:53.909833 fern_persona-0.0.3/src/persona/types/retrieve_a_government_id_verification_response_data_relationships_document_data.py
+-rw-r--r--   0        0        0      823 2023-05-24 17:37:53.909833 fern_persona-0.0.3/src/persona/types/retrieve_a_government_id_verification_response_data_relationships_inquiry.py
+-rw-r--r--   0        0        0      740 2023-05-24 17:37:53.909833 fern_persona-0.0.3/src/persona/types/retrieve_a_list_response.py
+-rw-r--r--   0        0        0      987 2023-05-24 17:37:53.909833 fern_persona-0.0.3/src/persona/types/retrieve_a_phone_carrier_database_verification_response.py
+-rw-r--r--   0        0        0     1355 2023-05-24 17:37:53.909833 fern_persona-0.0.3/src/persona/types/retrieve_a_phone_carrier_database_verification_response_data.py
+-rw-r--r--   0        0        0     1788 2023-05-24 17:37:53.909833 fern_persona-0.0.3/src/persona/types/retrieve_a_phone_carrier_database_verification_response_data_attributes.py
+-rw-r--r--   0        0        0     1221 2023-05-24 17:37:53.909833 fern_persona-0.0.3/src/persona/types/retrieve_a_phone_carrier_database_verification_response_data_attributes_checks_item.py
+-rw-r--r--   0        0        0     1001 2023-05-24 17:37:53.909833 fern_persona-0.0.3/src/persona/types/retrieve_a_phone_carrier_database_verification_response_data_attributes_checks_item_metadata.py
+-rw-r--r--   0        0        0     1069 2023-05-24 17:37:53.909833 fern_persona-0.0.3/src/persona/types/retrieve_a_phone_carrier_database_verification_response_data_relationships.py
+-rw-r--r--   0        0        0      831 2023-05-24 17:37:53.909833 fern_persona-0.0.3/src/persona/types/retrieve_a_phone_carrier_database_verification_response_data_relationships_inquiry.py
+-rw-r--r--   0        0        0      941 2023-05-24 17:37:53.909833 fern_persona-0.0.3/src/persona/types/retrieve_a_phone_number_verification_response.py
+-rw-r--r--   0        0        0     1290 2023-05-24 17:37:53.909833 fern_persona-0.0.3/src/persona/types/retrieve_a_phone_number_verification_response_data.py
+-rw-r--r--   0        0        0     1839 2023-05-24 17:37:53.909833 fern_persona-0.0.3/src/persona/types/retrieve_a_phone_number_verification_response_data_attributes.py
+-rw-r--r--   0        0        0      781 2023-05-24 17:37:53.909833 fern_persona-0.0.3/src/persona/types/retrieve_a_phone_number_verification_response_data_attributes_metadata.py
+-rw-r--r--   0        0        0     1032 2023-05-24 17:37:53.909833 fern_persona-0.0.3/src/persona/types/retrieve_a_phone_number_verification_response_data_relationships.py
+-rw-r--r--   0        0        0      822 2023-05-24 17:37:53.909833 fern_persona-0.0.3/src/persona/types/retrieve_a_phone_number_verification_response_data_relationships_inquiry.py
+-rw-r--r--   0        0        0      871 2023-05-24 17:37:53.909833 fern_persona-0.0.3/src/persona/types/retrieve_a_report_response.py
+-rw-r--r--   0        0        0      972 2023-05-24 17:37:53.909833 fern_persona-0.0.3/src/persona/types/retrieve_a_report_response_data.py
+-rw-r--r--   0        0        0     1815 2023-05-24 17:37:53.909833 fern_persona-0.0.3/src/persona/types/retrieve_a_report_response_data_attributes.py
+-rw-r--r--   0        0        0      920 2023-05-24 17:37:53.909833 fern_persona-0.0.3/src/persona/types/retrieve_a_selfie_verification_response.py
+-rw-r--r--   0        0        0     1244 2023-05-24 17:37:53.909833 fern_persona-0.0.3/src/persona/types/retrieve_a_selfie_verification_response_data.py
+-rw-r--r--   0        0        0     2216 2023-05-24 17:37:53.909833 fern_persona-0.0.3/src/persona/types/retrieve_a_selfie_verification_response_data_attributes.py
+-rw-r--r--   0        0        0     1156 2023-05-24 17:37:53.909833 fern_persona-0.0.3/src/persona/types/retrieve_a_selfie_verification_response_data_attributes_checks_item.py
+-rw-r--r--   0        0        0      786 2023-05-24 17:37:53.909833 fern_persona-0.0.3/src/persona/types/retrieve_a_selfie_verification_response_data_attributes_checks_item_metadata.py
+-rw-r--r--   0        0        0     1011 2023-05-24 17:37:53.909833 fern_persona-0.0.3/src/persona/types/retrieve_a_selfie_verification_response_data_relationships.py
+-rw-r--r--   0        0        0      817 2023-05-24 17:37:53.909833 fern_persona-0.0.3/src/persona/types/retrieve_a_selfie_verification_response_data_relationships_inquiry.py
+-rw-r--r--   0        0        0      953 2023-05-24 17:37:53.909833 fern_persona-0.0.3/src/persona/types/retrieve_a_serpro_database_verification_response.py
+-rw-r--r--   0        0        0     1311 2023-05-24 17:37:53.909833 fern_persona-0.0.3/src/persona/types/retrieve_a_serpro_database_verification_response_data.py
+-rw-r--r--   0        0        0     1763 2023-05-24 17:37:53.909833 fern_persona-0.0.3/src/persona/types/retrieve_a_serpro_database_verification_response_data_attributes.py
+-rw-r--r--   0        0        0     1196 2023-05-24 17:37:53.909833 fern_persona-0.0.3/src/persona/types/retrieve_a_serpro_database_verification_response_data_attributes_checks_item.py
+-rw-r--r--   0        0        0      794 2023-05-24 17:37:53.909833 fern_persona-0.0.3/src/persona/types/retrieve_a_serpro_database_verification_response_data_attributes_checks_item_metadata.py
+-rw-r--r--   0        0        0     1304 2023-05-24 17:37:53.909833 fern_persona-0.0.3/src/persona/types/retrieve_a_serpro_database_verification_response_data_relationships.py
+-rw-r--r--   0        0        0      825 2023-05-24 17:37:53.909833 fern_persona-0.0.3/src/persona/types/retrieve_a_serpro_database_verification_response_data_relationships_inquiry.py
+-rw-r--r--   0        0        0      824 2023-05-24 17:37:53.909833 fern_persona-0.0.3/src/persona/types/retrieve_a_serpro_database_verification_response_data_relationships_selfie.py
+-rw-r--r--   0        0        0      945 2023-05-24 17:37:53.909833 fern_persona-0.0.3/src/persona/types/retrieve_a_tin_database_verifications_response.py
+-rw-r--r--   0        0        0     1297 2023-05-24 17:37:53.909833 fern_persona-0.0.3/src/persona/types/retrieve_a_tin_database_verifications_response_data.py
+-rw-r--r--   0        0        0     1755 2023-05-24 17:37:53.909833 fern_persona-0.0.3/src/persona/types/retrieve_a_tin_database_verifications_response_data_attributes.py
+-rw-r--r--   0        0        0     1188 2023-05-24 17:37:53.909833 fern_persona-0.0.3/src/persona/types/retrieve_a_tin_database_verifications_response_data_attributes_checks_item.py
+-rw-r--r--   0        0        0      792 2023-05-24 17:37:53.909833 fern_persona-0.0.3/src/persona/types/retrieve_a_tin_database_verifications_response_data_attributes_checks_item_metadata.py
+-rw-r--r--   0        0        0     1036 2023-05-24 17:37:53.909833 fern_persona-0.0.3/src/persona/types/retrieve_a_tin_database_verifications_response_data_relationships.py
+-rw-r--r--   0        0        0      823 2023-05-24 17:37:53.909833 fern_persona-0.0.3/src/persona/types/retrieve_a_tin_database_verifications_response_data_relationships_inquiry.py
+-rw-r--r--   0        0        0      879 2023-05-24 17:37:53.909833 fern_persona-0.0.3/src/persona/types/retrieve_an_account_response.py
+-rw-r--r--   0        0        0      980 2023-05-24 17:37:53.909833 fern_persona-0.0.3/src/persona/types/retrieve_an_account_response_data.py
+-rw-r--r--   0        0        0     1031 2023-05-24 17:37:53.909833 fern_persona-0.0.3/src/persona/types/retrieve_an_account_response_data_attributes.py
+-rw-r--r--   0        0        0      876 2023-05-24 17:37:53.909833 fern_persona-0.0.3/src/persona/types/retrieve_an_api_key_response.py
+-rw-r--r--   0        0        0      977 2023-05-24 17:37:53.909833 fern_persona-0.0.3/src/persona/types/retrieve_an_api_key_response_data.py
+-rw-r--r--   0        0        0     1584 2023-05-24 17:37:53.909833 fern_persona-0.0.3/src/persona/types/retrieve_an_api_key_response_data_attributes.py
+-rw-r--r--   0        0        0      876 2023-05-24 17:37:53.909833 fern_persona-0.0.3/src/persona/types/retrieve_an_api_log_response.py
+-rw-r--r--   0        0        0      977 2023-05-24 17:37:53.909833 fern_persona-0.0.3/src/persona/types/retrieve_an_api_log_response_data.py
+-rw-r--r--   0        0        0     1258 2023-05-24 17:37:53.909833 fern_persona-0.0.3/src/persona/types/retrieve_an_api_log_response_data_attributes.py
+-rw-r--r--   0        0        0     1733 2023-05-24 17:37:53.909833 fern_persona-0.0.3/src/persona/types/retrieve_an_api_log_response_data_attributes_request.py
+-rw-r--r--   0        0        0     1018 2023-05-24 17:37:53.909833 fern_persona-0.0.3/src/persona/types/retrieve_an_api_log_response_data_attributes_request_get_params.py
+-rw-r--r--   0        0        0      819 2023-05-24 17:37:53.909833 fern_persona-0.0.3/src/persona/types/retrieve_an_api_log_response_data_attributes_request_get_params_filter.py
+-rw-r--r--   0        0        0      898 2023-05-24 17:37:53.909833 fern_persona-0.0.3/src/persona/types/retrieve_an_api_log_response_data_attributes_request_headers.py
+-rw-r--r--   0        0        0      774 2023-05-24 17:37:53.909833 fern_persona-0.0.3/src/persona/types/retrieve_an_api_log_response_data_attributes_request_post_params.py
+-rw-r--r--   0        0        0     1072 2023-05-24 17:37:53.909833 fern_persona-0.0.3/src/persona/types/retrieve_an_api_log_response_data_attributes_response.py
+-rw-r--r--   0        0        0      893 2023-05-24 17:37:53.909833 fern_persona-0.0.3/src/persona/types/retrieve_an_api_log_response_data_attributes_response_headers.py
+-rw-r--r--   0        0        0      742 2023-05-24 17:37:53.909833 fern_persona-0.0.3/src/persona/types/retrieve_an_event_response.py
+-rw-r--r--   0        0        0      883 2023-05-24 17:37:53.909833 fern_persona-0.0.3/src/persona/types/retrieve_an_importer_response.py
+-rw-r--r--   0        0        0      984 2023-05-24 17:37:53.909833 fern_persona-0.0.3/src/persona/types/retrieve_an_importer_response_data.py
+-rw-r--r--   0        0        0     1244 2023-05-24 17:37:53.909833 fern_persona-0.0.3/src/persona/types/retrieve_an_importer_response_data_attributes.py
+-rw-r--r--   0        0        0     1055 2023-05-24 17:37:53.909833 fern_persona-0.0.3/src/persona/types/retrieve_an_inquiry_response.py
+-rw-r--r--   0        0        0     1163 2023-05-24 17:37:53.909833 fern_persona-0.0.3/src/persona/types/retrieve_an_inquiry_response_data.py
+-rw-r--r--   0        0        0     2311 2023-05-24 17:37:53.909833 fern_persona-0.0.3/src/persona/types/retrieve_an_inquiry_response_data_attributes.py
+-rw-r--r--   0        0        0     2068 2023-05-24 17:37:53.909833 fern_persona-0.0.3/src/persona/types/retrieve_an_inquiry_response_data_attributes_behaviours.py
+-rw-r--r--   0        0        0     1364 2023-05-24 17:37:53.913833 fern_persona-0.0.3/src/persona/types/retrieve_an_inquiry_response_data_attributes_fields.py
+-rw-r--r--   0        0        0      837 2023-05-24 17:37:53.913833 fern_persona-0.0.3/src/persona/types/retrieve_an_inquiry_response_data_attributes_fields_name_first.py
+-rw-r--r--   0        0        0      836 2023-05-24 17:37:53.913833 fern_persona-0.0.3/src/persona/types/retrieve_an_inquiry_response_data_attributes_fields_name_last.py
+-rw-r--r--   0        0        0     1798 2023-05-24 17:37:53.913833 fern_persona-0.0.3/src/persona/types/retrieve_an_inquiry_response_data_relationships.py
+-rw-r--r--   0        0        0      987 2023-05-24 17:37:53.913833 fern_persona-0.0.3/src/persona/types/retrieve_an_inquiry_response_data_relationships_account.py
+-rw-r--r--   0        0        0      833 2023-05-24 17:37:53.913833 fern_persona-0.0.3/src/persona/types/retrieve_an_inquiry_response_data_relationships_account_data.py
+-rw-r--r--   0        0        0      820 2023-05-24 17:37:53.913833 fern_persona-0.0.3/src/persona/types/retrieve_an_inquiry_response_data_relationships_reports.py
+-rw-r--r--   0        0        0     1017 2023-05-24 17:37:53.913833 fern_persona-0.0.3/src/persona/types/retrieve_an_inquiry_response_data_relationships_sessions.py
+-rw-r--r--   0        0        0      838 2023-05-24 17:37:53.913833 fern_persona-0.0.3/src/persona/types/retrieve_an_inquiry_response_data_relationships_sessions_data_item.py
+-rw-r--r--   0        0        0      991 2023-05-24 17:37:53.913833 fern_persona-0.0.3/src/persona/types/retrieve_an_inquiry_response_data_relationships_template.py
+-rw-r--r--   0        0        0      834 2023-05-24 17:37:53.913833 fern_persona-0.0.3/src/persona/types/retrieve_an_inquiry_response_data_relationships_template_data.py
+-rw-r--r--   0        0        0     1037 2023-05-24 17:37:53.913833 fern_persona-0.0.3/src/persona/types/retrieve_an_inquiry_response_data_relationships_verifications.py
+-rw-r--r--   0        0        0      843 2023-05-24 17:37:53.913833 fern_persona-0.0.3/src/persona/types/retrieve_an_inquiry_response_data_relationships_verifications_data_item.py
+-rw-r--r--   0        0        0     1013 2023-05-24 17:37:53.913833 fern_persona-0.0.3/src/persona/types/retrieve_an_inquiry_response_included_item.py
+-rw-r--r--   0        0        0     1782 2023-05-24 17:37:53.913833 fern_persona-0.0.3/src/persona/types/retrieve_an_inquiry_response_included_item_attributes.py
+-rw-r--r--   0        0        0      901 2023-05-24 17:37:53.913833 fern_persona-0.0.3/src/persona/types/retrieve_an_user_audit_log_response.py
+-rw-r--r--   0        0        0     1002 2023-05-24 17:37:53.913833 fern_persona-0.0.3/src/persona/types/retrieve_an_user_audit_log_response_data.py
+-rw-r--r--   0        0        0     1022 2023-05-24 17:37:53.913833 fern_persona-0.0.3/src/persona/types/retrieve_an_user_audit_log_response_data_attributes.py
+-rw-r--r--   0        0        0     1018 2023-05-24 17:37:53.913833 fern_persona-0.0.3/src/persona/types/retrieve_case_response.py
+-rw-r--r--   0        0        0     1126 2023-05-24 17:37:53.913833 fern_persona-0.0.3/src/persona/types/retrieve_case_response_data.py
+-rw-r--r--   0        0        0     1775 2023-05-24 17:37:53.913833 fern_persona-0.0.3/src/persona/types/retrieve_case_response_data_attributes.py
+-rw-r--r--   0        0        0     1882 2023-05-24 17:37:53.913833 fern_persona-0.0.3/src/persona/types/retrieve_case_response_data_relationships.py
+-rw-r--r--   0        0        0      996 2023-05-24 17:37:53.913833 fern_persona-0.0.3/src/persona/types/retrieve_case_response_data_relationships_accounts.py
+-rw-r--r--   0        0        0      833 2023-05-24 17:37:53.913833 fern_persona-0.0.3/src/persona/types/retrieve_case_response_data_relationships_accounts_data_item.py
+-rw-r--r--   0        0        0     1013 2023-05-24 17:37:53.913833 fern_persona-0.0.3/src/persona/types/retrieve_case_response_data_relationships_case_comments.py
+-rw-r--r--   0        0        0      837 2023-05-24 17:37:53.913833 fern_persona-0.0.3/src/persona/types/retrieve_case_response_data_relationships_case_comments_data_item.py
+-rw-r--r--   0        0        0      987 2023-05-24 17:37:53.913833 fern_persona-0.0.3/src/persona/types/retrieve_case_response_data_relationships_case_template.py
+-rw-r--r--   0        0        0      833 2023-05-24 17:37:53.913833 fern_persona-0.0.3/src/persona/types/retrieve_case_response_data_relationships_case_template_data.py
+-rw-r--r--   0        0        0     1000 2023-05-24 17:37:53.913833 fern_persona-0.0.3/src/persona/types/retrieve_case_response_data_relationships_inquiries.py
+-rw-r--r--   0        0        0      834 2023-05-24 17:37:53.913833 fern_persona-0.0.3/src/persona/types/retrieve_case_response_data_relationships_inquiries_data_item.py
+-rw-r--r--   0        0        0      815 2023-05-24 17:37:53.913833 fern_persona-0.0.3/src/persona/types/retrieve_case_response_data_relationships_reports.py
+-rw-r--r--   0        0        0      992 2023-05-24 17:37:53.913833 fern_persona-0.0.3/src/persona/types/retrieve_case_response_included_item.py
+-rw-r--r--   0        0        0     1092 2023-05-24 17:37:53.913833 fern_persona-0.0.3/src/persona/types/retrieve_case_response_included_item_attributes.py
+-rw-r--r--   0        0        0      892 2023-05-24 17:37:53.913833 fern_persona-0.0.3/src/persona/types/send_an_email_request_data.py
+-rw-r--r--   0        0        0      876 2023-05-24 17:37:53.913833 fern_persona-0.0.3/src/persona/types/send_an_email_request_data_attributes.py
+-rw-r--r--   0        0        0      855 2023-05-24 17:37:53.913833 fern_persona-0.0.3/src/persona/types/send_an_email_response.py
+-rw-r--r--   0        0        0      956 2023-05-24 17:37:53.913833 fern_persona-0.0.3/src/persona/types/send_an_email_response_data.py
+-rw-r--r--   0        0        0     1682 2023-05-24 17:37:53.913833 fern_persona-0.0.3/src/persona/types/send_an_email_response_data_attributes.py
+-rw-r--r--   0        0        0      760 2023-05-24 17:37:53.913833 fern_persona-0.0.3/src/persona/types/send_an_email_response_data_attributes_metadata.py
+-rw-r--r--   0        0        0      884 2023-05-24 17:37:53.913833 fern_persona-0.0.3/src/persona/types/send_an_sms_request_data.py
+-rw-r--r--   0        0        0      874 2023-05-24 17:37:53.913833 fern_persona-0.0.3/src/persona/types/send_an_sms_request_data_attributes.py
+-rw-r--r--   0        0        0      847 2023-05-24 17:37:53.913833 fern_persona-0.0.3/src/persona/types/send_an_sms_response.py
+-rw-r--r--   0        0        0      948 2023-05-24 17:37:53.913833 fern_persona-0.0.3/src/persona/types/send_an_sms_response_data.py
+-rw-r--r--   0        0        0     1750 2023-05-24 17:37:53.913833 fern_persona-0.0.3/src/persona/types/send_an_sms_response_data_attributes.py
+-rw-r--r--   0        0        0      758 2023-05-24 17:37:53.913833 fern_persona-0.0.3/src/persona/types/send_an_sms_response_data_attributes_metadata.py
+-rw-r--r--   0        0        0      871 2023-05-24 17:37:53.913833 fern_persona-0.0.3/src/persona/types/set_all_tags_1_request_meta.py
+-rw-r--r--   0        0        0      870 2023-05-24 17:37:53.913833 fern_persona-0.0.3/src/persona/types/set_all_tags_request_meta.py
+-rw-r--r--   0        0        0      781 2023-05-24 17:37:53.913833 fern_persona-0.0.3/src/persona/types/set_status_for_a_case_request_meta.py
+-rw-r--r--   0        0        0      881 2023-05-24 17:37:53.913833 fern_persona-0.0.3/src/persona/types/set_status_for_a_case_response.py
+-rw-r--r--   0        0        0     1167 2023-05-24 17:37:53.913833 fern_persona-0.0.3/src/persona/types/set_status_for_a_case_response_data.py
+-rw-r--r--   0        0        0     1842 2023-05-24 17:37:53.913833 fern_persona-0.0.3/src/persona/types/set_status_for_a_case_response_data_attributes.py
+-rw-r--r--   0        0        0     2013 2023-05-24 17:37:53.913833 fern_persona-0.0.3/src/persona/types/set_status_for_a_case_response_data_relationships.py
+-rw-r--r--   0        0        0      821 2023-05-24 17:37:53.913833 fern_persona-0.0.3/src/persona/types/set_status_for_a_case_response_data_relationships_accounts.py
+-rw-r--r--   0        0        0      825 2023-05-24 17:37:53.913833 fern_persona-0.0.3/src/persona/types/set_status_for_a_case_response_data_relationships_case_comments.py
+-rw-r--r--   0        0        0     1010 2023-05-24 17:37:53.913833 fern_persona-0.0.3/src/persona/types/set_status_for_a_case_response_data_relationships_case_template.py
+-rw-r--r--   0        0        0      838 2023-05-24 17:37:53.913833 fern_persona-0.0.3/src/persona/types/set_status_for_a_case_response_data_relationships_case_template_data.py
+-rw-r--r--   0        0        0     1023 2023-05-24 17:37:53.913833 fern_persona-0.0.3/src/persona/types/set_status_for_a_case_response_data_relationships_inquiries.py
+-rw-r--r--   0        0        0      839 2023-05-24 17:37:53.913833 fern_persona-0.0.3/src/persona/types/set_status_for_a_case_response_data_relationships_inquiries_data_item.py
+-rw-r--r--   0        0        0     1015 2023-05-24 17:37:53.913833 fern_persona-0.0.3/src/persona/types/set_status_for_a_case_response_data_relationships_reports.py
+-rw-r--r--   0        0        0      837 2023-05-24 17:37:53.913833 fern_persona-0.0.3/src/persona/types/set_status_for_a_case_response_data_relationships_reports_data_item.py
+-rw-r--r--   0        0        0      871 2023-05-24 17:37:53.913833 fern_persona-0.0.3/src/persona/types/submit_a_document_response.py
+-rw-r--r--   0        0        0     1149 2023-05-24 17:37:53.913833 fern_persona-0.0.3/src/persona/types/submit_a_document_response_data.py
+-rw-r--r--   0        0        0     1228 2023-05-24 17:37:53.913833 fern_persona-0.0.3/src/persona/types/submit_a_document_response_data_attributes.py
+-rw-r--r--   0        0        0      831 2023-05-24 17:37:53.913833 fern_persona-0.0.3/src/persona/types/submit_a_document_response_data_attributes_files_item.py
+-rw-r--r--   0        0        0      953 2023-05-24 17:37:53.913833 fern_persona-0.0.3/src/persona/types/submit_a_document_response_data_relationships.py
+-rw-r--r--   0        0        0      979 2023-05-24 17:37:53.913833 fern_persona-0.0.3/src/persona/types/submit_a_document_response_data_relationships_inquiry.py
+-rw-r--r--   0        0        0      831 2023-05-24 17:37:53.913833 fern_persona-0.0.3/src/persona/types/submit_a_document_response_data_relationships_inquiry_data.py
+-rw-r--r--   0        0        0      920 2023-05-24 17:37:53.913833 fern_persona-0.0.3/src/persona/types/submit_a_document_verification_response.py
+-rw-r--r--   0        0        0     1244 2023-05-24 17:37:53.913833 fern_persona-0.0.3/src/persona/types/submit_a_document_verification_response_data.py
+-rw-r--r--   0        0        0     1425 2023-05-24 17:37:53.913833 fern_persona-0.0.3/src/persona/types/submit_a_document_verification_response_data_attributes.py
+-rw-r--r--   0        0        0     1254 2023-05-24 17:37:53.913833 fern_persona-0.0.3/src/persona/types/submit_a_document_verification_response_data_relationships.py
+-rw-r--r--   0        0        0     1032 2023-05-24 17:37:53.913833 fern_persona-0.0.3/src/persona/types/submit_a_document_verification_response_data_relationships_document.py
+-rw-r--r--   0        0        0      844 2023-05-24 17:37:53.913833 fern_persona-0.0.3/src/persona/types/submit_a_document_verification_response_data_relationships_document_data.py
+-rw-r--r--   0        0        0     1028 2023-05-24 17:37:53.913833 fern_persona-0.0.3/src/persona/types/submit_a_document_verification_response_data_relationships_inquiry.py
+-rw-r--r--   0        0        0      843 2023-05-24 17:37:53.913833 fern_persona-0.0.3/src/persona/types/submit_a_document_verification_response_data_relationships_inquiry_data.py
+-rw-r--r--   0        0        0      921 2023-05-24 17:37:53.913833 fern_persona-0.0.3/src/persona/types/submit_a_government_id_document_response.py
+-rw-r--r--   0        0        0     1246 2023-05-24 17:37:53.913833 fern_persona-0.0.3/src/persona/types/submit_a_government_id_document_response_data.py
+-rw-r--r--   0        0        0     2186 2023-05-24 17:37:53.913833 fern_persona-0.0.3/src/persona/types/submit_a_government_id_document_response_data_attributes.py
+-rw-r--r--   0        0        0     1012 2023-05-24 17:37:53.913833 fern_persona-0.0.3/src/persona/types/submit_a_government_id_document_response_data_relationships.py
+-rw-r--r--   0        0        0     1029 2023-05-24 17:37:53.913833 fern_persona-0.0.3/src/persona/types/submit_a_government_id_document_response_data_relationships_inquiry.py
+-rw-r--r--   0        0        0      843 2023-05-24 17:37:53.913833 fern_persona-0.0.3/src/persona/types/submit_a_government_id_document_response_data_relationships_inquiry_data.py
+-rw-r--r--   0        0        0      937 2023-05-24 17:37:53.913833 fern_persona-0.0.3/src/persona/types/submit_a_government_id_verification_response.py
+-rw-r--r--   0        0        0     1283 2023-05-24 17:37:53.913833 fern_persona-0.0.3/src/persona/types/submit_a_government_id_verification_response_data.py
+-rw-r--r--   0        0        0     2555 2023-05-24 17:37:53.913833 fern_persona-0.0.3/src/persona/types/submit_a_government_id_verification_response_data_attributes.py
+-rw-r--r--   0        0        0     1284 2023-05-24 17:37:53.913833 fern_persona-0.0.3/src/persona/types/submit_a_government_id_verification_response_data_relationships.py
+-rw-r--r--   0        0        0     1049 2023-05-24 17:37:53.913833 fern_persona-0.0.3/src/persona/types/submit_a_government_id_verification_response_data_relationships_document.py
+-rw-r--r--   0        0        0      848 2023-05-24 17:37:53.913833 fern_persona-0.0.3/src/persona/types/submit_a_government_id_verification_response_data_relationships_document_data.py
+-rw-r--r--   0        0        0      821 2023-05-24 17:37:53.913833 fern_persona-0.0.3/src/persona/types/submit_a_government_id_verification_response_data_relationships_inquiry.py
+-rw-r--r--   0        0        0      979 2023-05-24 17:37:53.913833 fern_persona-0.0.3/src/persona/types/submit_a_phone_carrier_database_verification_response.py
+-rw-r--r--   0        0        0     1341 2023-05-24 17:37:53.913833 fern_persona-0.0.3/src/persona/types/submit_a_phone_carrier_database_verification_response_data.py
+-rw-r--r--   0        0        0     1557 2023-05-24 17:37:53.913833 fern_persona-0.0.3/src/persona/types/submit_a_phone_carrier_database_verification_response_data_attributes.py
+-rw-r--r--   0        0        0     1061 2023-05-24 17:37:53.913833 fern_persona-0.0.3/src/persona/types/submit_a_phone_carrier_database_verification_response_data_relationships.py
+-rw-r--r--   0        0        0      829 2023-05-24 17:37:53.913833 fern_persona-0.0.3/src/persona/types/submit_a_phone_carrier_database_verification_response_data_relationships_inquiry.py
+-rw-r--r--   0        0        0      912 2023-05-24 17:37:53.913833 fern_persona-0.0.3/src/persona/types/submit_a_selfie_verification_response.py
+-rw-r--r--   0        0        0     1221 2023-05-24 17:37:53.913833 fern_persona-0.0.3/src/persona/types/submit_a_selfie_verification_response_data.py
+-rw-r--r--   0        0        0     2043 2023-05-24 17:37:53.913833 fern_persona-0.0.3/src/persona/types/submit_a_selfie_verification_response_data_attributes.py
+-rw-r--r--   0        0        0     1003 2023-05-24 17:37:53.913833 fern_persona-0.0.3/src/persona/types/submit_a_selfie_verification_response_data_relationships.py
+-rw-r--r--   0        0        0      815 2023-05-24 17:37:53.913833 fern_persona-0.0.3/src/persona/types/submit_a_selfie_verification_response_data_relationships_inquiry.py
+-rw-r--r--   0        0        0      945 2023-05-24 17:37:53.913833 fern_persona-0.0.3/src/persona/types/submit_a_serpro_database_verification_response.py
+-rw-r--r--   0        0        0     1297 2023-05-24 17:37:53.913833 fern_persona-0.0.3/src/persona/types/submit_a_serpro_database_verification_response_data.py
+-rw-r--r--   0        0        0     1551 2023-05-24 17:37:53.913833 fern_persona-0.0.3/src/persona/types/submit_a_serpro_database_verification_response_data_attributes.py
+-rw-r--r--   0        0        0     1290 2023-05-24 17:37:53.913833 fern_persona-0.0.3/src/persona/types/submit_a_serpro_database_verification_response_data_relationships.py
+-rw-r--r--   0        0        0      823 2023-05-24 17:37:53.913833 fern_persona-0.0.3/src/persona/types/submit_a_serpro_database_verification_response_data_relationships_inquiry.py
+-rw-r--r--   0        0        0      822 2023-05-24 17:37:53.913833 fern_persona-0.0.3/src/persona/types/submit_a_serpro_database_verification_response_data_relationships_selfie.py
+-rw-r--r--   0        0        0      937 2023-05-24 17:37:53.913833 fern_persona-0.0.3/src/persona/types/submit_a_tin_database_verifications_response.py
+-rw-r--r--   0        0        0     1283 2023-05-24 17:37:53.913833 fern_persona-0.0.3/src/persona/types/submit_a_tin_database_verifications_response_data.py
+-rw-r--r--   0        0        0     1549 2023-05-24 17:37:53.913833 fern_persona-0.0.3/src/persona/types/submit_a_tin_database_verifications_response_data_attributes.py
+-rw-r--r--   0        0        0     1028 2023-05-24 17:37:53.917832 fern_persona-0.0.3/src/persona/types/submit_a_tin_database_verifications_response_data_relationships.py
+-rw-r--r--   0        0        0      821 2023-05-24 17:37:53.917832 fern_persona-0.0.3/src/persona/types/submit_a_tin_database_verifications_response_data_relationships_inquiry.py
+-rw-r--r--   0        0        0      925 2023-05-24 17:37:53.917832 fern_persona-0.0.3/src/persona/types/unprocessable_entity_error_body.py
+-rw-r--r--   0        0        0      824 2023-05-24 17:37:53.917832 fern_persona-0.0.3/src/persona/types/unprocessable_entity_error_body_errors_item.py
+-rw-r--r--   0        0        0      892 2023-05-24 17:37:53.917832 fern_persona-0.0.3/src/persona/types/update_a_case_request_data.py
+-rw-r--r--   0        0        0     1128 2023-05-24 17:37:53.917832 fern_persona-0.0.3/src/persona/types/update_a_case_request_data_attributes.py
+-rw-r--r--   0        0        0      943 2023-05-24 17:37:53.917832 fern_persona-0.0.3/src/persona/types/update_a_case_request_data_attributes_attachments_item.py
+-rw-r--r--   0        0        0     1055 2023-05-24 17:37:53.917832 fern_persona-0.0.3/src/persona/types/update_a_case_request_data_attributes_fields.py
+-rw-r--r--   0        0        0      855 2023-05-24 17:37:53.917832 fern_persona-0.0.3/src/persona/types/update_a_case_response.py
+-rw-r--r--   0        0        0     1121 2023-05-24 17:37:53.917832 fern_persona-0.0.3/src/persona/types/update_a_case_response_data.py
+-rw-r--r--   0        0        0     1836 2023-05-24 17:37:53.917832 fern_persona-0.0.3/src/persona/types/update_a_case_response_data_attributes.py
+-rw-r--r--   0        0        0     1871 2023-05-24 17:37:53.917832 fern_persona-0.0.3/src/persona/types/update_a_case_response_data_relationships.py
+-rw-r--r--   0        0        0      815 2023-05-24 17:37:53.917832 fern_persona-0.0.3/src/persona/types/update_a_case_response_data_relationships_accounts.py
+-rw-r--r--   0        0        0      819 2023-05-24 17:37:53.917832 fern_persona-0.0.3/src/persona/types/update_a_case_response_data_relationships_case_comments.py
+-rw-r--r--   0        0        0      984 2023-05-24 17:37:53.917832 fern_persona-0.0.3/src/persona/types/update_a_case_response_data_relationships_case_template.py
+-rw-r--r--   0        0        0      832 2023-05-24 17:37:53.917832 fern_persona-0.0.3/src/persona/types/update_a_case_response_data_relationships_case_template_data.py
+-rw-r--r--   0        0        0      997 2023-05-24 17:37:53.917832 fern_persona-0.0.3/src/persona/types/update_a_case_response_data_relationships_inquiries.py
+-rw-r--r--   0        0        0      833 2023-05-24 17:37:53.917832 fern_persona-0.0.3/src/persona/types/update_a_case_response_data_relationships_inquiries_data_item.py
+-rw-r--r--   0        0        0      989 2023-05-24 17:37:53.917832 fern_persona-0.0.3/src/persona/types/update_a_case_response_data_relationships_reports.py
+-rw-r--r--   0        0        0      831 2023-05-24 17:37:53.917832 fern_persona-0.0.3/src/persona/types/update_a_case_response_data_relationships_reports_data_item.py
+-rw-r--r--   0        0        0      908 2023-05-24 17:37:53.917832 fern_persona-0.0.3/src/persona/types/update_a_document_request_data.py
+-rw-r--r--   0        0        0      894 2023-05-24 17:37:53.917832 fern_persona-0.0.3/src/persona/types/update_a_document_request_data_attributes.py
+-rw-r--r--   0        0        0      871 2023-05-24 17:37:53.917832 fern_persona-0.0.3/src/persona/types/update_a_document_response.py
+-rw-r--r--   0        0        0     1149 2023-05-24 17:37:53.917832 fern_persona-0.0.3/src/persona/types/update_a_document_response_data.py
+-rw-r--r--   0        0        0     1228 2023-05-24 17:37:53.917832 fern_persona-0.0.3/src/persona/types/update_a_document_response_data_attributes.py
+-rw-r--r--   0        0        0      831 2023-05-24 17:37:53.917832 fern_persona-0.0.3/src/persona/types/update_a_document_response_data_attributes_files_item.py
+-rw-r--r--   0        0        0      953 2023-05-24 17:37:53.917832 fern_persona-0.0.3/src/persona/types/update_a_document_response_data_relationships.py
+-rw-r--r--   0        0        0      979 2023-05-24 17:37:53.917832 fern_persona-0.0.3/src/persona/types/update_a_document_response_data_relationships_inquiry.py
+-rw-r--r--   0        0        0      831 2023-05-24 17:37:53.917832 fern_persona-0.0.3/src/persona/types/update_a_document_response_data_relationships_inquiry_data.py
+-rw-r--r--   0        0        0      958 2023-05-24 17:37:53.917832 fern_persona-0.0.3/src/persona/types/update_a_government_id_document_request_data.py
+-rw-r--r--   0        0        0     1561 2023-05-24 17:37:53.917832 fern_persona-0.0.3/src/persona/types/update_a_government_id_document_request_data_attributes.py
+-rw-r--r--   0        0        0     1353 2023-05-24 17:37:53.917832 fern_persona-0.0.3/src/persona/types/update_a_government_id_document_request_data_attributes_back_photo.py
+-rw-r--r--   0        0        0     1167 2023-05-24 17:37:53.917832 fern_persona-0.0.3/src/persona/types/update_a_government_id_document_request_data_attributes_back_photo_data.py
+-rw-r--r--   0        0        0     1358 2023-05-24 17:37:53.917832 fern_persona-0.0.3/src/persona/types/update_a_government_id_document_request_data_attributes_front_photo.py
+-rw-r--r--   0        0        0     1168 2023-05-24 17:37:53.917832 fern_persona-0.0.3/src/persona/types/update_a_government_id_document_request_data_attributes_front_photo_data.py
+-rw-r--r--   0        0        0      921 2023-05-24 17:37:53.917832 fern_persona-0.0.3/src/persona/types/update_a_government_id_document_response.py
+-rw-r--r--   0        0        0     1246 2023-05-24 17:37:53.917832 fern_persona-0.0.3/src/persona/types/update_a_government_id_document_response_data.py
+-rw-r--r--   0        0        0     2186 2023-05-24 17:37:53.917832 fern_persona-0.0.3/src/persona/types/update_a_government_id_document_response_data_attributes.py
+-rw-r--r--   0        0        0     1012 2023-05-24 17:37:53.917832 fern_persona-0.0.3/src/persona/types/update_a_government_id_document_response_data_relationships.py
+-rw-r--r--   0        0        0     1029 2023-05-24 17:37:53.917832 fern_persona-0.0.3/src/persona/types/update_a_government_id_document_response_data_relationships_inquiry.py
+-rw-r--r--   0        0        0      843 2023-05-24 17:37:53.917832 fern_persona-0.0.3/src/persona/types/update_a_government_id_document_response_data_relationships_inquiry_data.py
+-rw-r--r--   0        0        0      983 2023-05-24 17:37:53.917832 fern_persona-0.0.3/src/persona/types/update_a_government_id_verification_request_data.py
+-rw-r--r--   0        0        0     1589 2023-05-24 17:37:53.917832 fern_persona-0.0.3/src/persona/types/update_a_government_id_verification_request_data_attributes.py
+-rw-r--r--   0        0        0     1369 2023-05-24 17:37:53.917832 fern_persona-0.0.3/src/persona/types/update_a_government_id_verification_request_data_attributes_back_photo.py
+-rw-r--r--   0        0        0     1171 2023-05-24 17:37:53.917832 fern_persona-0.0.3/src/persona/types/update_a_government_id_verification_request_data_attributes_back_photo_data.py
+-rw-r--r--   0        0        0     1374 2023-05-24 17:37:53.917832 fern_persona-0.0.3/src/persona/types/update_a_government_id_verification_request_data_attributes_front_photo.py
+-rw-r--r--   0        0        0     1172 2023-05-24 17:37:53.917832 fern_persona-0.0.3/src/persona/types/update_a_government_id_verification_request_data_attributes_front_photo_data.py
+-rw-r--r--   0        0        0      937 2023-05-24 17:37:53.917832 fern_persona-0.0.3/src/persona/types/update_a_government_id_verification_response.py
+-rw-r--r--   0        0        0     1283 2023-05-24 17:37:53.917832 fern_persona-0.0.3/src/persona/types/update_a_government_id_verification_response_data.py
+-rw-r--r--   0        0        0     3080 2023-05-24 17:37:53.917832 fern_persona-0.0.3/src/persona/types/update_a_government_id_verification_response_data_attributes.py
+-rw-r--r--   0        0        0     1028 2023-05-24 17:37:53.917832 fern_persona-0.0.3/src/persona/types/update_a_government_id_verification_response_data_relationships.py
+-rw-r--r--   0        0        0     1045 2023-05-24 17:37:53.917832 fern_persona-0.0.3/src/persona/types/update_a_government_id_verification_response_data_relationships_inquiry.py
+-rw-r--r--   0        0        0      847 2023-05-24 17:37:53.917832 fern_persona-0.0.3/src/persona/types/update_a_government_id_verification_response_data_relationships_inquiry_data.py
+-rw-r--r--   0        0        0      908 2023-05-24 17:37:53.917832 fern_persona-0.0.3/src/persona/types/update_an_account_request_data.py
+-rw-r--r--   0        0        0     3576 2023-05-24 17:37:53.917832 fern_persona-0.0.3/src/persona/types/update_an_account_request_data_attributes.py
+-rw-r--r--   0        0        0     1231 2023-05-24 17:37:53.917832 fern_persona-0.0.3/src/persona/types/update_an_account_request_data_attributes_selfie_photo.py
+-rw-r--r--   0        0        0     1113 2023-05-24 17:37:53.917832 fern_persona-0.0.3/src/persona/types/update_an_account_request_data_attributes_selfie_photo_data.py
+-rw-r--r--   0        0        0      871 2023-05-24 17:37:53.917832 fern_persona-0.0.3/src/persona/types/update_an_account_response.py
+-rw-r--r--   0        0        0      972 2023-05-24 17:37:53.917832 fern_persona-0.0.3/src/persona/types/update_an_account_response_data.py
+-rw-r--r--   0        0        0     1080 2023-05-24 17:37:53.917832 fern_persona-0.0.3/src/persona/types/update_an_account_response_data_attributes.py
+-rw-r--r--   0        0        0      905 2023-05-24 17:37:53.917832 fern_persona-0.0.3/src/persona/types/update_an_api_key_request_data.py
+-rw-r--r--   0        0        0     1804 2023-05-24 17:37:53.917832 fern_persona-0.0.3/src/persona/types/update_an_api_key_request_data_attributes.py
+-rw-r--r--   0        0        0      868 2023-05-24 17:37:53.917832 fern_persona-0.0.3/src/persona/types/update_an_api_key_response.py
+-rw-r--r--   0        0        0      969 2023-05-24 17:37:53.917832 fern_persona-0.0.3/src/persona/types/update_an_api_key_response_data.py
+-rw-r--r--   0        0        0     1589 2023-05-24 17:37:53.917832 fern_persona-0.0.3/src/persona/types/update_an_api_key_response_data_attributes.py
+-rw-r--r--   0        0        0      908 2023-05-24 17:37:53.917832 fern_persona-0.0.3/src/persona/types/update_an_inquiry_request_data.py
+-rw-r--r--   0        0        0     2047 2023-05-24 17:37:53.917832 fern_persona-0.0.3/src/persona/types/update_an_inquiry_request_data_attributes.py
+-rw-r--r--   0        0        0     2192 1970-01-01 00:00:00.000000 fern_persona-0.0.3/PKG-INFO
```

### Comparing `fern_persona-0.0.2/README.md` & `fern_persona-0.0.3/README.md`

 * *Files identical despite different names*

### Comparing `fern_persona-0.0.2/src/persona/__init__.py` & `fern_persona-0.0.3/src/persona/__init__.py`

 * *Files identical despite different names*

### Comparing `fern_persona-0.0.2/src/persona/client.py` & `fern_persona-0.0.3/src/persona/client.py`

 * *Files identical despite different names*

### Comparing `fern_persona-0.0.2/src/persona/core/datetime_utils.py` & `fern_persona-0.0.3/src/persona/core/datetime_utils.py`

 * *Files identical despite different names*

### Comparing `fern_persona-0.0.2/src/persona/core/jsonable_encoder.py` & `fern_persona-0.0.3/src/persona/core/jsonable_encoder.py`

 * *Files identical despite different names*

### Comparing `fern_persona-0.0.2/src/persona/resources/__init__.py` & `fern_persona-0.0.3/src/persona/resources/__init__.py`

 * *Files identical despite different names*

### Comparing `fern_persona-0.0.2/src/persona/resources/accounts/client.py` & `fern_persona-0.0.3/src/persona/resources/accounts/client.py`

 * *Files 4% similar despite different names*

```diff
@@ -39,15 +39,17 @@
 
     def retrieve_an_account(
         self, account_id: str, *, key_inflection: typing.Optional[str] = None
     ) -> RetrieveAnAccountResponse:
         _response = httpx.request(
             "GET",
             urllib.parse.urljoin(f"{self._environment.value}/", f"accounts/{account_id}"),
-            headers=remove_none_from_headers({"Key-Inflection": key_inflection, "Authorization": self.api_key}),
+            headers=remove_none_from_headers(
+                {"Key-Inflection": key_inflection, "Authorization": f"Bearer  {self.api_key}"}
+            ),
             timeout=60,
         )
         if 200 <= _response.status_code < 300:
             return pydantic.parse_obj_as(RetrieveAnAccountResponse, _response.json())  # type: ignore
         if _response.status_code == 404:
             raise NotFoundError(pydantic.parse_obj_as(typing.Any, _response.json()))  # type: ignore
         try:
@@ -68,15 +70,19 @@
         if data is not OMIT:
             _request["data"] = data
         _response = httpx.request(
             "PATCH",
             urllib.parse.urljoin(f"{self._environment.value}/", f"accounts/{account_id}"),
             json=jsonable_encoder(_request),
             headers=remove_none_from_headers(
-                {"Key-Inflection": key_inflection, "Idempotency-Key": idempotency_key, "Authorization": self.api_key}
+                {
+                    "Key-Inflection": key_inflection,
+                    "Idempotency-Key": idempotency_key,
+                    "Authorization": f"Bearer  {self.api_key}",
+                }
             ),
             timeout=60,
         )
         if 200 <= _response.status_code < 300:
             return pydantic.parse_obj_as(UpdateAnAccountResponse, _response.json())  # type: ignore
         if _response.status_code == 409:
             raise ConflictError(pydantic.parse_obj_as(typing.Any, _response.json()))  # type: ignore
@@ -88,15 +94,17 @@
 
     def redact_an_account(
         self, account_id: str, *, persona_version: typing.Optional[str] = None
     ) -> RedactAnAccountResponse:
         _response = httpx.request(
             "DELETE",
             urllib.parse.urljoin(f"{self._environment.value}/", f"accounts/{account_id}"),
-            headers=remove_none_from_headers({"Persona-Version": persona_version, "Authorization": self.api_key}),
+            headers=remove_none_from_headers(
+                {"Persona-Version": persona_version, "Authorization": f"Bearer  {self.api_key}"}
+            ),
             timeout=60,
         )
         if 200 <= _response.status_code < 300:
             return pydantic.parse_obj_as(RedactAnAccountResponse, _response.json())  # type: ignore
         try:
             _response_json = _response.json()
         except JSONDecodeError:
@@ -117,15 +125,17 @@
             urllib.parse.urljoin(f"{self._environment.value}/", "accounts"),
             params={
                 "page[before]": page_before,
                 "page[after]": page_after,
                 "page[size]": page_size,
                 "filter[reference-id]": filter_reference_id,
             },
-            headers=remove_none_from_headers({"Key-Inflection": key_inflection, "Authorization": self.api_key}),
+            headers=remove_none_from_headers(
+                {"Key-Inflection": key_inflection, "Authorization": f"Bearer  {self.api_key}"}
+            ),
             timeout=60,
         )
         if 200 <= _response.status_code < 300:
             return pydantic.parse_obj_as(ListAllAccountsResponse, _response.json())  # type: ignore
         try:
             _response_json = _response.json()
         except JSONDecodeError:
@@ -143,15 +153,19 @@
         if data is not OMIT:
             _request["data"] = data
         _response = httpx.request(
             "POST",
             urllib.parse.urljoin(f"{self._environment.value}/", "accounts"),
             json=jsonable_encoder(_request),
             headers=remove_none_from_headers(
-                {"Key-Inflection": key_inflection, "Idempotency-Key": idempotency_key, "Authorization": self.api_key}
+                {
+                    "Key-Inflection": key_inflection,
+                    "Idempotency-Key": idempotency_key,
+                    "Authorization": f"Bearer  {self.api_key}",
+                }
             ),
             timeout=60,
         )
         if 200 <= _response.status_code < 300:
             return pydantic.parse_obj_as(CreateAnAccountResponse, _response.json())  # type: ignore
         if _response.status_code == 409:
             raise ConflictError(pydantic.parse_obj_as(typing.Any, _response.json()))  # type: ignore
@@ -173,15 +187,19 @@
         if meta is not OMIT:
             _request["meta"] = meta
         _response = httpx.request(
             "POST",
             urllib.parse.urljoin(f"{self._environment.value}/", f"accounts/{account_id}/consolidate"),
             json=jsonable_encoder(_request),
             headers=remove_none_from_headers(
-                {"Key-Inflection": key_inflection, "Idempotency-Key": idempotency_key, "Authorization": self.api_key}
+                {
+                    "Key-Inflection": key_inflection,
+                    "Idempotency-Key": idempotency_key,
+                    "Authorization": f"Bearer  {self.api_key}",
+                }
             ),
             timeout=60,
         )
         if 200 <= _response.status_code < 300:
             return
         if _response.status_code == 400:
             raise BadRequestError(pydantic.parse_obj_as(typing.Any, _response.json()))  # type: ignore
@@ -209,15 +227,19 @@
         if meta is not OMIT:
             _request["meta"] = meta
         _response = httpx.request(
             "POST",
             urllib.parse.urljoin(f"{self._environment.value}/", f"accounts/{account_id}/add-tag"),
             json=jsonable_encoder(_request),
             headers=remove_none_from_headers(
-                {"Key-Inflection": key_inflection, "Idempotency-Key": idempotency_key, "Authorization": self.api_key}
+                {
+                    "Key-Inflection": key_inflection,
+                    "Idempotency-Key": idempotency_key,
+                    "Authorization": f"Bearer  {self.api_key}",
+                }
             ),
             timeout=60,
         )
         if 200 <= _response.status_code < 300:
             return
         if _response.status_code == 400:
             raise BadRequestError(pydantic.parse_obj_as(typing.Any, _response.json()))  # type: ignore
@@ -239,15 +261,19 @@
         if meta is not OMIT:
             _request["meta"] = meta
         _response = httpx.request(
             "POST",
             urllib.parse.urljoin(f"{self._environment.value}/", f"accounts/{account_id}/remove-tag"),
             json=jsonable_encoder(_request),
             headers=remove_none_from_headers(
-                {"Key-Inflection": key_inflection, "Idempotency-Key": idempotency_key, "Authorization": self.api_key}
+                {
+                    "Key-Inflection": key_inflection,
+                    "Idempotency-Key": idempotency_key,
+                    "Authorization": f"Bearer  {self.api_key}",
+                }
             ),
             timeout=60,
         )
         if 200 <= _response.status_code < 300:
             return
         if _response.status_code == 400:
             raise BadRequestError(pydantic.parse_obj_as(typing.Any, _response.json()))  # type: ignore
@@ -269,15 +295,19 @@
         if meta is not OMIT:
             _request["meta"] = meta
         _response = httpx.request(
             "POST",
             urllib.parse.urljoin(f"{self._environment.value}/", f"accounts/{account_id}/set-tags"),
             json=jsonable_encoder(_request),
             headers=remove_none_from_headers(
-                {"Key-Inflection": key_inflection, "Idempotency-Key": idempotency_key, "Authorization": self.api_key}
+                {
+                    "Key-Inflection": key_inflection,
+                    "Idempotency-Key": idempotency_key,
+                    "Authorization": f"Bearer  {self.api_key}",
+                }
             ),
             timeout=60,
         )
         if 200 <= _response.status_code < 300:
             return
         if _response.status_code == 400:
             raise BadRequestError(pydantic.parse_obj_as(typing.Any, _response.json()))  # type: ignore
@@ -287,15 +317,15 @@
             raise ApiError(status_code=_response.status_code, body=_response.text)
         raise ApiError(status_code=_response.status_code, body=_response_json)
 
     def print_an_inquiry_pdf(self, inquiry_id: str) -> None:
         _response = httpx.request(
             "GET",
             urllib.parse.urljoin(f"{self._environment.value}/", f"inquiries/{inquiry_id}/print"),
-            headers=remove_none_from_headers({"Authorization": self.api_key}),
+            headers=remove_none_from_headers({"Authorization": f"Bearer  {self.api_key}"}),
             timeout=60,
         )
         if 200 <= _response.status_code < 300:
             return
         try:
             _response_json = _response.json()
         except JSONDecodeError:
@@ -311,15 +341,17 @@
     async def retrieve_an_account(
         self, account_id: str, *, key_inflection: typing.Optional[str] = None
     ) -> RetrieveAnAccountResponse:
         async with httpx.AsyncClient() as _client:
             _response = await _client.request(
                 "GET",
                 urllib.parse.urljoin(f"{self._environment.value}/", f"accounts/{account_id}"),
-                headers=remove_none_from_headers({"Key-Inflection": key_inflection, "Authorization": self.api_key}),
+                headers=remove_none_from_headers(
+                    {"Key-Inflection": key_inflection, "Authorization": f"Bearer  {self.api_key}"}
+                ),
                 timeout=60,
             )
         if 200 <= _response.status_code < 300:
             return pydantic.parse_obj_as(RetrieveAnAccountResponse, _response.json())  # type: ignore
         if _response.status_code == 404:
             raise NotFoundError(pydantic.parse_obj_as(typing.Any, _response.json()))  # type: ignore
         try:
@@ -344,15 +376,15 @@
                 "PATCH",
                 urllib.parse.urljoin(f"{self._environment.value}/", f"accounts/{account_id}"),
                 json=jsonable_encoder(_request),
                 headers=remove_none_from_headers(
                     {
                         "Key-Inflection": key_inflection,
                         "Idempotency-Key": idempotency_key,
-                        "Authorization": self.api_key,
+                        "Authorization": f"Bearer  {self.api_key}",
                     }
                 ),
                 timeout=60,
             )
         if 200 <= _response.status_code < 300:
             return pydantic.parse_obj_as(UpdateAnAccountResponse, _response.json())  # type: ignore
         if _response.status_code == 409:
@@ -366,15 +398,17 @@
     async def redact_an_account(
         self, account_id: str, *, persona_version: typing.Optional[str] = None
     ) -> RedactAnAccountResponse:
         async with httpx.AsyncClient() as _client:
             _response = await _client.request(
                 "DELETE",
                 urllib.parse.urljoin(f"{self._environment.value}/", f"accounts/{account_id}"),
-                headers=remove_none_from_headers({"Persona-Version": persona_version, "Authorization": self.api_key}),
+                headers=remove_none_from_headers(
+                    {"Persona-Version": persona_version, "Authorization": f"Bearer  {self.api_key}"}
+                ),
                 timeout=60,
             )
         if 200 <= _response.status_code < 300:
             return pydantic.parse_obj_as(RedactAnAccountResponse, _response.json())  # type: ignore
         try:
             _response_json = _response.json()
         except JSONDecodeError:
@@ -396,15 +430,17 @@
                 urllib.parse.urljoin(f"{self._environment.value}/", "accounts"),
                 params={
                     "page[before]": page_before,
                     "page[after]": page_after,
                     "page[size]": page_size,
                     "filter[reference-id]": filter_reference_id,
                 },
-                headers=remove_none_from_headers({"Key-Inflection": key_inflection, "Authorization": self.api_key}),
+                headers=remove_none_from_headers(
+                    {"Key-Inflection": key_inflection, "Authorization": f"Bearer  {self.api_key}"}
+                ),
                 timeout=60,
             )
         if 200 <= _response.status_code < 300:
             return pydantic.parse_obj_as(ListAllAccountsResponse, _response.json())  # type: ignore
         try:
             _response_json = _response.json()
         except JSONDecodeError:
@@ -426,15 +462,15 @@
                 "POST",
                 urllib.parse.urljoin(f"{self._environment.value}/", "accounts"),
                 json=jsonable_encoder(_request),
                 headers=remove_none_from_headers(
                     {
                         "Key-Inflection": key_inflection,
                         "Idempotency-Key": idempotency_key,
-                        "Authorization": self.api_key,
+                        "Authorization": f"Bearer  {self.api_key}",
                     }
                 ),
                 timeout=60,
             )
         if 200 <= _response.status_code < 300:
             return pydantic.parse_obj_as(CreateAnAccountResponse, _response.json())  # type: ignore
         if _response.status_code == 409:
@@ -461,15 +497,15 @@
                 "POST",
                 urllib.parse.urljoin(f"{self._environment.value}/", f"accounts/{account_id}/consolidate"),
                 json=jsonable_encoder(_request),
                 headers=remove_none_from_headers(
                     {
                         "Key-Inflection": key_inflection,
                         "Idempotency-Key": idempotency_key,
-                        "Authorization": self.api_key,
+                        "Authorization": f"Bearer  {self.api_key}",
                     }
                 ),
                 timeout=60,
             )
         if 200 <= _response.status_code < 300:
             return
         if _response.status_code == 400:
@@ -502,15 +538,15 @@
                 "POST",
                 urllib.parse.urljoin(f"{self._environment.value}/", f"accounts/{account_id}/add-tag"),
                 json=jsonable_encoder(_request),
                 headers=remove_none_from_headers(
                     {
                         "Key-Inflection": key_inflection,
                         "Idempotency-Key": idempotency_key,
-                        "Authorization": self.api_key,
+                        "Authorization": f"Bearer  {self.api_key}",
                     }
                 ),
                 timeout=60,
             )
         if 200 <= _response.status_code < 300:
             return
         if _response.status_code == 400:
@@ -537,15 +573,15 @@
                 "POST",
                 urllib.parse.urljoin(f"{self._environment.value}/", f"accounts/{account_id}/remove-tag"),
                 json=jsonable_encoder(_request),
                 headers=remove_none_from_headers(
                     {
                         "Key-Inflection": key_inflection,
                         "Idempotency-Key": idempotency_key,
-                        "Authorization": self.api_key,
+                        "Authorization": f"Bearer  {self.api_key}",
                     }
                 ),
                 timeout=60,
             )
         if 200 <= _response.status_code < 300:
             return
         if _response.status_code == 400:
@@ -572,15 +608,15 @@
                 "POST",
                 urllib.parse.urljoin(f"{self._environment.value}/", f"accounts/{account_id}/set-tags"),
                 json=jsonable_encoder(_request),
                 headers=remove_none_from_headers(
                     {
                         "Key-Inflection": key_inflection,
                         "Idempotency-Key": idempotency_key,
-                        "Authorization": self.api_key,
+                        "Authorization": f"Bearer  {self.api_key}",
                     }
                 ),
                 timeout=60,
             )
         if 200 <= _response.status_code < 300:
             return
         if _response.status_code == 400:
@@ -592,15 +628,15 @@
         raise ApiError(status_code=_response.status_code, body=_response_json)
 
     async def print_an_inquiry_pdf(self, inquiry_id: str) -> None:
         async with httpx.AsyncClient() as _client:
             _response = await _client.request(
                 "GET",
                 urllib.parse.urljoin(f"{self._environment.value}/", f"inquiries/{inquiry_id}/print"),
-                headers=remove_none_from_headers({"Authorization": self.api_key}),
+                headers=remove_none_from_headers({"Authorization": f"Bearer  {self.api_key}"}),
                 timeout=60,
             )
         if 200 <= _response.status_code < 300:
             return
         try:
             _response_json = _response.json()
         except JSONDecodeError:
```

### Comparing `fern_persona-0.0.2/src/persona/resources/api_keys/client.py` & `fern_persona-0.0.3/src/persona/resources/api_keys/client.py`

 * *Files 3% similar despite different names*

```diff
@@ -44,15 +44,17 @@
             urllib.parse.urljoin(f"{self._environment.value}/", "api-keys"),
             params={
                 "page[after]": page_after,
                 "page[before]": page_before,
                 "page[size]": page_size,
                 "filter[name]": filter_name,
             },
-            headers=remove_none_from_headers({"Key-Inflection": key_inflection, "Authorization": self.api_key}),
+            headers=remove_none_from_headers(
+                {"Key-Inflection": key_inflection, "Authorization": f"Bearer  {self.api_key}"}
+            ),
             timeout=60,
         )
         if 200 <= _response.status_code < 300:
             return pydantic.parse_obj_as(ListAllApiKeysResponse, _response.json())  # type: ignore
         try:
             _response_json = _response.json()
         except JSONDecodeError:
@@ -63,15 +65,15 @@
         _request: typing.Dict[str, typing.Any] = {}
         if data is not OMIT:
             _request["data"] = data
         _response = httpx.request(
             "POST",
             urllib.parse.urljoin(f"{self._environment.value}/", "api-keys"),
             json=jsonable_encoder(_request),
-            headers=remove_none_from_headers({"Authorization": self.api_key}),
+            headers=remove_none_from_headers({"Authorization": f"Bearer  {self.api_key}"}),
             timeout=60,
         )
         if 200 <= _response.status_code < 300:
             return pydantic.parse_obj_as(CreateAnApiKeyResponse, _response.json())  # type: ignore
         if _response.status_code == 400:
             raise BadRequestError(pydantic.parse_obj_as(typing.Any, _response.json()))  # type: ignore
         try:
@@ -86,15 +88,15 @@
         _request: typing.Dict[str, typing.Any] = {}
         if meta is not OMIT:
             _request["meta"] = meta
         _response = httpx.request(
             "POST",
             urllib.parse.urljoin(f"{self._environment.value}/", f"api-keys/{api_key_id}/expire"),
             json=jsonable_encoder(_request),
-            headers=remove_none_from_headers({"Authorization": self.api_key}),
+            headers=remove_none_from_headers({"Authorization": f"Bearer  {self.api_key}"}),
             timeout=60,
         )
         if 200 <= _response.status_code < 300:
             return pydantic.parse_obj_as(ExpireAnApiKeyResponse, _response.json())  # type: ignore
         if _response.status_code == 400:
             raise BadRequestError(pydantic.parse_obj_as(typing.Any, _response.json()))  # type: ignore
         try:
@@ -103,15 +105,15 @@
             raise ApiError(status_code=_response.status_code, body=_response.text)
         raise ApiError(status_code=_response.status_code, body=_response_json)
 
     def retrieve_an_api_key(self, api_key_id: str) -> RetrieveAnApiKeyResponse:
         _response = httpx.request(
             "GET",
             urllib.parse.urljoin(f"{self._environment.value}/", f"api-keys/{api_key_id}"),
-            headers=remove_none_from_headers({"Authorization": self.api_key}),
+            headers=remove_none_from_headers({"Authorization": f"Bearer  {self.api_key}"}),
             timeout=60,
         )
         if 200 <= _response.status_code < 300:
             return pydantic.parse_obj_as(RetrieveAnApiKeyResponse, _response.json())  # type: ignore
         if _response.status_code == 400:
             raise BadRequestError(pydantic.parse_obj_as(typing.Any, _response.json()))  # type: ignore
         try:
@@ -126,15 +128,15 @@
         _request: typing.Dict[str, typing.Any] = {}
         if data is not OMIT:
             _request["data"] = data
         _response = httpx.request(
             "PATCH",
             urllib.parse.urljoin(f"{self._environment.value}/", f"api-keys/{api_key_id}"),
             json=jsonable_encoder(_request),
-            headers=remove_none_from_headers({"Authorization": self.api_key}),
+            headers=remove_none_from_headers({"Authorization": f"Bearer  {self.api_key}"}),
             timeout=60,
         )
         if 200 <= _response.status_code < 300:
             return pydantic.parse_obj_as(UpdateAnApiKeyResponse, _response.json())  # type: ignore
         if _response.status_code == 400:
             raise BadRequestError(pydantic.parse_obj_as(typing.Any, _response.json()))  # type: ignore
         try:
@@ -164,15 +166,17 @@
                 urllib.parse.urljoin(f"{self._environment.value}/", "api-keys"),
                 params={
                     "page[after]": page_after,
                     "page[before]": page_before,
                     "page[size]": page_size,
                     "filter[name]": filter_name,
                 },
-                headers=remove_none_from_headers({"Key-Inflection": key_inflection, "Authorization": self.api_key}),
+                headers=remove_none_from_headers(
+                    {"Key-Inflection": key_inflection, "Authorization": f"Bearer  {self.api_key}"}
+                ),
                 timeout=60,
             )
         if 200 <= _response.status_code < 300:
             return pydantic.parse_obj_as(ListAllApiKeysResponse, _response.json())  # type: ignore
         try:
             _response_json = _response.json()
         except JSONDecodeError:
@@ -186,15 +190,15 @@
         if data is not OMIT:
             _request["data"] = data
         async with httpx.AsyncClient() as _client:
             _response = await _client.request(
                 "POST",
                 urllib.parse.urljoin(f"{self._environment.value}/", "api-keys"),
                 json=jsonable_encoder(_request),
-                headers=remove_none_from_headers({"Authorization": self.api_key}),
+                headers=remove_none_from_headers({"Authorization": f"Bearer  {self.api_key}"}),
                 timeout=60,
             )
         if 200 <= _response.status_code < 300:
             return pydantic.parse_obj_as(CreateAnApiKeyResponse, _response.json())  # type: ignore
         if _response.status_code == 400:
             raise BadRequestError(pydantic.parse_obj_as(typing.Any, _response.json()))  # type: ignore
         try:
@@ -210,15 +214,15 @@
         if meta is not OMIT:
             _request["meta"] = meta
         async with httpx.AsyncClient() as _client:
             _response = await _client.request(
                 "POST",
                 urllib.parse.urljoin(f"{self._environment.value}/", f"api-keys/{api_key_id}/expire"),
                 json=jsonable_encoder(_request),
-                headers=remove_none_from_headers({"Authorization": self.api_key}),
+                headers=remove_none_from_headers({"Authorization": f"Bearer  {self.api_key}"}),
                 timeout=60,
             )
         if 200 <= _response.status_code < 300:
             return pydantic.parse_obj_as(ExpireAnApiKeyResponse, _response.json())  # type: ignore
         if _response.status_code == 400:
             raise BadRequestError(pydantic.parse_obj_as(typing.Any, _response.json()))  # type: ignore
         try:
@@ -228,15 +232,15 @@
         raise ApiError(status_code=_response.status_code, body=_response_json)
 
     async def retrieve_an_api_key(self, api_key_id: str) -> RetrieveAnApiKeyResponse:
         async with httpx.AsyncClient() as _client:
             _response = await _client.request(
                 "GET",
                 urllib.parse.urljoin(f"{self._environment.value}/", f"api-keys/{api_key_id}"),
-                headers=remove_none_from_headers({"Authorization": self.api_key}),
+                headers=remove_none_from_headers({"Authorization": f"Bearer  {self.api_key}"}),
                 timeout=60,
             )
         if 200 <= _response.status_code < 300:
             return pydantic.parse_obj_as(RetrieveAnApiKeyResponse, _response.json())  # type: ignore
         if _response.status_code == 400:
             raise BadRequestError(pydantic.parse_obj_as(typing.Any, _response.json()))  # type: ignore
         try:
@@ -252,15 +256,15 @@
         if data is not OMIT:
             _request["data"] = data
         async with httpx.AsyncClient() as _client:
             _response = await _client.request(
                 "PATCH",
                 urllib.parse.urljoin(f"{self._environment.value}/", f"api-keys/{api_key_id}"),
                 json=jsonable_encoder(_request),
-                headers=remove_none_from_headers({"Authorization": self.api_key}),
+                headers=remove_none_from_headers({"Authorization": f"Bearer  {self.api_key}"}),
                 timeout=60,
             )
         if 200 <= _response.status_code < 300:
             return pydantic.parse_obj_as(UpdateAnApiKeyResponse, _response.json())  # type: ignore
         if _response.status_code == 400:
             raise BadRequestError(pydantic.parse_obj_as(typing.Any, _response.json()))  # type: ignore
         try:
```

### Comparing `fern_persona-0.0.2/src/persona/resources/api_logs/client.py` & `fern_persona-0.0.3/src/persona/resources/api_logs/client.py`

 * *Files 4% similar despite different names*

```diff
@@ -27,15 +27,17 @@
         page_size: typing.Optional[str] = None,
         key_inflection: typing.Optional[str] = None,
     ) -> None:
         _response = httpx.request(
             "GET",
             urllib.parse.urljoin(f"{self._environment.value}/", "api-logs"),
             params={"page[before]": page_before, "page[after]": page_after, "page[size]": page_size},
-            headers=remove_none_from_headers({"Key-Inflection": key_inflection, "Authorization": self.api_key}),
+            headers=remove_none_from_headers(
+                {"Key-Inflection": key_inflection, "Authorization": f"Bearer  {self.api_key}"}
+            ),
             timeout=60,
         )
         if 200 <= _response.status_code < 300:
             return
         try:
             _response_json = _response.json()
         except JSONDecodeError:
@@ -44,15 +46,17 @@
 
     def retrieve_an_api_log(
         self, api_log_id: str, *, key_inflection: typing.Optional[str] = None
     ) -> RetrieveAnApiLogResponse:
         _response = httpx.request(
             "GET",
             urllib.parse.urljoin(f"{self._environment.value}/", f"api-logs/{api_log_id}"),
-            headers=remove_none_from_headers({"Key-Inflection": key_inflection, "Authorization": self.api_key}),
+            headers=remove_none_from_headers(
+                {"Key-Inflection": key_inflection, "Authorization": f"Bearer  {self.api_key}"}
+            ),
             timeout=60,
         )
         if 200 <= _response.status_code < 300:
             return pydantic.parse_obj_as(RetrieveAnApiLogResponse, _response.json())  # type: ignore
         if _response.status_code == 404:
             raise NotFoundError(pydantic.parse_obj_as(typing.Any, _response.json()))  # type: ignore
         try:
@@ -76,15 +80,17 @@
         key_inflection: typing.Optional[str] = None,
     ) -> None:
         async with httpx.AsyncClient() as _client:
             _response = await _client.request(
                 "GET",
                 urllib.parse.urljoin(f"{self._environment.value}/", "api-logs"),
                 params={"page[before]": page_before, "page[after]": page_after, "page[size]": page_size},
-                headers=remove_none_from_headers({"Key-Inflection": key_inflection, "Authorization": self.api_key}),
+                headers=remove_none_from_headers(
+                    {"Key-Inflection": key_inflection, "Authorization": f"Bearer  {self.api_key}"}
+                ),
                 timeout=60,
             )
         if 200 <= _response.status_code < 300:
             return
         try:
             _response_json = _response.json()
         except JSONDecodeError:
@@ -94,15 +100,17 @@
     async def retrieve_an_api_log(
         self, api_log_id: str, *, key_inflection: typing.Optional[str] = None
     ) -> RetrieveAnApiLogResponse:
         async with httpx.AsyncClient() as _client:
             _response = await _client.request(
                 "GET",
                 urllib.parse.urljoin(f"{self._environment.value}/", f"api-logs/{api_log_id}"),
-                headers=remove_none_from_headers({"Key-Inflection": key_inflection, "Authorization": self.api_key}),
+                headers=remove_none_from_headers(
+                    {"Key-Inflection": key_inflection, "Authorization": f"Bearer  {self.api_key}"}
+                ),
                 timeout=60,
             )
         if 200 <= _response.status_code < 300:
             return pydantic.parse_obj_as(RetrieveAnApiLogResponse, _response.json())  # type: ignore
         if _response.status_code == 404:
             raise NotFoundError(pydantic.parse_obj_as(typing.Any, _response.json()))  # type: ignore
         try:
```

### Comparing `fern_persona-0.0.2/src/persona/resources/cases/client.py` & `fern_persona-0.0.3/src/persona/resources/cases/client.py`

 * *Files 3% similar despite different names*

```diff
@@ -59,15 +59,17 @@
                 "filter[status]": filter_status,
                 "filter[resolution]": filter_resolution,
                 "filter[case-template-id]": filter_case_template_id,
                 "filter[account-id]": filter_account_id,
                 "filter[inquiry-id]": filter_inquiry_id,
                 "filter[report-id]": filter_report_id,
             },
-            headers=remove_none_from_headers({"key-inflection": key_inflection, "Authorization": self.api_key}),
+            headers=remove_none_from_headers(
+                {"key-inflection": key_inflection, "Authorization": f"Bearer  {self.api_key}"}
+            ),
             timeout=60,
         )
         if 200 <= _response.status_code < 300:
             return pydantic.parse_obj_as(ListAllCasesResponse, _response.json())  # type: ignore
         if _response.status_code == 400:
             raise BadRequestError(pydantic.parse_obj_as(typing.Any, _response.json()))  # type: ignore
         try:
@@ -82,15 +84,15 @@
         _request: typing.Dict[str, typing.Any] = {"data": data}
         if meta is not OMIT:
             _request["meta"] = meta
         _response = httpx.request(
             "POST",
             urllib.parse.urljoin(f"{self._environment.value}/", "cases"),
             json=jsonable_encoder(_request),
-            headers=remove_none_from_headers({"Authorization": self.api_key}),
+            headers=remove_none_from_headers({"Authorization": f"Bearer  {self.api_key}"}),
             timeout=60,
         )
         if 200 <= _response.status_code < 300:
             return pydantic.parse_obj_as(CreateACaseResponse, _response.json())  # type: ignore
         if _response.status_code == 400:
             raise BadRequestError(pydantic.parse_obj_as(typing.Any, _response.json()))  # type: ignore
         try:
@@ -99,15 +101,17 @@
             raise ApiError(status_code=_response.status_code, body=_response.text)
         raise ApiError(status_code=_response.status_code, body=_response_json)
 
     def retrieve_case(self, case_id: str, *, key_inflection: typing.Optional[str] = None) -> RetrieveCaseResponse:
         _response = httpx.request(
             "GET",
             urllib.parse.urljoin(f"{self._environment.value}/", f"cases/{case_id}"),
-            headers=remove_none_from_headers({"key-inflection": key_inflection, "Authorization": self.api_key}),
+            headers=remove_none_from_headers(
+                {"key-inflection": key_inflection, "Authorization": f"Bearer  {self.api_key}"}
+            ),
             timeout=60,
         )
         if 200 <= _response.status_code < 300:
             return pydantic.parse_obj_as(RetrieveCaseResponse, _response.json())  # type: ignore
         if _response.status_code == 400:
             raise BadRequestError(pydantic.parse_obj_as(typing.Any, _response.json()))  # type: ignore
         try:
@@ -122,15 +126,15 @@
         _request: typing.Dict[str, typing.Any] = {}
         if data is not OMIT:
             _request["data"] = data
         _response = httpx.request(
             "PATCH",
             urllib.parse.urljoin(f"{self._environment.value}/", f"cases/{case_id}"),
             json=jsonable_encoder(_request),
-            headers=remove_none_from_headers({"Authorization": self.api_key}),
+            headers=remove_none_from_headers({"Authorization": f"Bearer  {self.api_key}"}),
             timeout=60,
         )
         if 200 <= _response.status_code < 300:
             return pydantic.parse_obj_as(UpdateACaseResponse, _response.json())  # type: ignore
         if _response.status_code == 400:
             raise BadRequestError(pydantic.parse_obj_as(typing.Any, _response.json()))  # type: ignore
         try:
@@ -145,15 +149,15 @@
         _request: typing.Dict[str, typing.Any] = {}
         if meta is not OMIT:
             _request["meta"] = meta
         _response = httpx.request(
             "POST",
             urllib.parse.urljoin(f"{self._environment.value}/", f"cases/{case_id}/add-objects"),
             json=jsonable_encoder(_request),
-            headers=remove_none_from_headers({"Authorization": self.api_key}),
+            headers=remove_none_from_headers({"Authorization": f"Bearer  {self.api_key}"}),
             timeout=60,
         )
         if 200 <= _response.status_code < 300:
             return pydantic.parse_obj_as(AddPersonaObjectsResponse, _response.json())  # type: ignore
         if _response.status_code == 400:
             raise BadRequestError(pydantic.parse_obj_as(typing.Any, _response.json()))  # type: ignore
         try:
@@ -163,15 +167,15 @@
         raise ApiError(status_code=_response.status_code, body=_response_json)
 
     def assign_a_case(self, case_id: str, *, meta: AssignACaseRequestMeta) -> AssignACaseResponse:
         _response = httpx.request(
             "POST",
             urllib.parse.urljoin(f"{self._environment.value}/", f"cases/{case_id}/assign"),
             json=jsonable_encoder({"meta": meta}),
-            headers=remove_none_from_headers({"Authorization": self.api_key}),
+            headers=remove_none_from_headers({"Authorization": f"Bearer  {self.api_key}"}),
             timeout=60,
         )
         if 200 <= _response.status_code < 300:
             return pydantic.parse_obj_as(AssignACaseResponse, _response.json())  # type: ignore
         if _response.status_code == 400:
             raise BadRequestError(pydantic.parse_obj_as(typing.Any, _response.json()))  # type: ignore
         try:
@@ -186,15 +190,15 @@
         _request: typing.Dict[str, typing.Any] = {}
         if meta is not OMIT:
             _request["meta"] = meta
         _response = httpx.request(
             "POST",
             urllib.parse.urljoin(f"{self._environment.value}/", f"cases/{case_id}/set-status"),
             json=jsonable_encoder(_request),
-            headers=remove_none_from_headers({"Authorization": self.api_key}),
+            headers=remove_none_from_headers({"Authorization": f"Bearer  {self.api_key}"}),
             timeout=60,
         )
         if 200 <= _response.status_code < 300:
             return pydantic.parse_obj_as(SetStatusForACaseResponse, _response.json())  # type: ignore
         if _response.status_code == 400:
             raise BadRequestError(pydantic.parse_obj_as(typing.Any, _response.json()))  # type: ignore
         try:
@@ -234,15 +238,17 @@
                     "filter[status]": filter_status,
                     "filter[resolution]": filter_resolution,
                     "filter[case-template-id]": filter_case_template_id,
                     "filter[account-id]": filter_account_id,
                     "filter[inquiry-id]": filter_inquiry_id,
                     "filter[report-id]": filter_report_id,
                 },
-                headers=remove_none_from_headers({"key-inflection": key_inflection, "Authorization": self.api_key}),
+                headers=remove_none_from_headers(
+                    {"key-inflection": key_inflection, "Authorization": f"Bearer  {self.api_key}"}
+                ),
                 timeout=60,
             )
         if 200 <= _response.status_code < 300:
             return pydantic.parse_obj_as(ListAllCasesResponse, _response.json())  # type: ignore
         if _response.status_code == 400:
             raise BadRequestError(pydantic.parse_obj_as(typing.Any, _response.json()))  # type: ignore
         try:
@@ -258,15 +264,15 @@
         if meta is not OMIT:
             _request["meta"] = meta
         async with httpx.AsyncClient() as _client:
             _response = await _client.request(
                 "POST",
                 urllib.parse.urljoin(f"{self._environment.value}/", "cases"),
                 json=jsonable_encoder(_request),
-                headers=remove_none_from_headers({"Authorization": self.api_key}),
+                headers=remove_none_from_headers({"Authorization": f"Bearer  {self.api_key}"}),
                 timeout=60,
             )
         if 200 <= _response.status_code < 300:
             return pydantic.parse_obj_as(CreateACaseResponse, _response.json())  # type: ignore
         if _response.status_code == 400:
             raise BadRequestError(pydantic.parse_obj_as(typing.Any, _response.json()))  # type: ignore
         try:
@@ -276,15 +282,17 @@
         raise ApiError(status_code=_response.status_code, body=_response_json)
 
     async def retrieve_case(self, case_id: str, *, key_inflection: typing.Optional[str] = None) -> RetrieveCaseResponse:
         async with httpx.AsyncClient() as _client:
             _response = await _client.request(
                 "GET",
                 urllib.parse.urljoin(f"{self._environment.value}/", f"cases/{case_id}"),
-                headers=remove_none_from_headers({"key-inflection": key_inflection, "Authorization": self.api_key}),
+                headers=remove_none_from_headers(
+                    {"key-inflection": key_inflection, "Authorization": f"Bearer  {self.api_key}"}
+                ),
                 timeout=60,
             )
         if 200 <= _response.status_code < 300:
             return pydantic.parse_obj_as(RetrieveCaseResponse, _response.json())  # type: ignore
         if _response.status_code == 400:
             raise BadRequestError(pydantic.parse_obj_as(typing.Any, _response.json()))  # type: ignore
         try:
@@ -300,15 +308,15 @@
         if data is not OMIT:
             _request["data"] = data
         async with httpx.AsyncClient() as _client:
             _response = await _client.request(
                 "PATCH",
                 urllib.parse.urljoin(f"{self._environment.value}/", f"cases/{case_id}"),
                 json=jsonable_encoder(_request),
-                headers=remove_none_from_headers({"Authorization": self.api_key}),
+                headers=remove_none_from_headers({"Authorization": f"Bearer  {self.api_key}"}),
                 timeout=60,
             )
         if 200 <= _response.status_code < 300:
             return pydantic.parse_obj_as(UpdateACaseResponse, _response.json())  # type: ignore
         if _response.status_code == 400:
             raise BadRequestError(pydantic.parse_obj_as(typing.Any, _response.json()))  # type: ignore
         try:
@@ -324,15 +332,15 @@
         if meta is not OMIT:
             _request["meta"] = meta
         async with httpx.AsyncClient() as _client:
             _response = await _client.request(
                 "POST",
                 urllib.parse.urljoin(f"{self._environment.value}/", f"cases/{case_id}/add-objects"),
                 json=jsonable_encoder(_request),
-                headers=remove_none_from_headers({"Authorization": self.api_key}),
+                headers=remove_none_from_headers({"Authorization": f"Bearer  {self.api_key}"}),
                 timeout=60,
             )
         if 200 <= _response.status_code < 300:
             return pydantic.parse_obj_as(AddPersonaObjectsResponse, _response.json())  # type: ignore
         if _response.status_code == 400:
             raise BadRequestError(pydantic.parse_obj_as(typing.Any, _response.json()))  # type: ignore
         try:
@@ -343,15 +351,15 @@
 
     async def assign_a_case(self, case_id: str, *, meta: AssignACaseRequestMeta) -> AssignACaseResponse:
         async with httpx.AsyncClient() as _client:
             _response = await _client.request(
                 "POST",
                 urllib.parse.urljoin(f"{self._environment.value}/", f"cases/{case_id}/assign"),
                 json=jsonable_encoder({"meta": meta}),
-                headers=remove_none_from_headers({"Authorization": self.api_key}),
+                headers=remove_none_from_headers({"Authorization": f"Bearer  {self.api_key}"}),
                 timeout=60,
             )
         if 200 <= _response.status_code < 300:
             return pydantic.parse_obj_as(AssignACaseResponse, _response.json())  # type: ignore
         if _response.status_code == 400:
             raise BadRequestError(pydantic.parse_obj_as(typing.Any, _response.json()))  # type: ignore
         try:
@@ -367,15 +375,15 @@
         if meta is not OMIT:
             _request["meta"] = meta
         async with httpx.AsyncClient() as _client:
             _response = await _client.request(
                 "POST",
                 urllib.parse.urljoin(f"{self._environment.value}/", f"cases/{case_id}/set-status"),
                 json=jsonable_encoder(_request),
-                headers=remove_none_from_headers({"Authorization": self.api_key}),
+                headers=remove_none_from_headers({"Authorization": f"Bearer  {self.api_key}"}),
                 timeout=60,
             )
         if 200 <= _response.status_code < 300:
             return pydantic.parse_obj_as(SetStatusForACaseResponse, _response.json())  # type: ignore
         if _response.status_code == 400:
             raise BadRequestError(pydantic.parse_obj_as(typing.Any, _response.json()))  # type: ignore
         try:
```

### Comparing `fern_persona-0.0.2/src/persona/resources/database_verifications/client.py` & `fern_persona-0.0.3/src/persona/resources/database_verifications/client.py`

 * *Files 7% similar despite different names*

```diff
@@ -30,15 +30,19 @@
         idempotency_key: typing.Optional[str] = None,
     ) -> CreateADatabaseVerificationResponse:
         _response = httpx.request(
             "POST",
             urllib.parse.urljoin(f"{self._environment.value}/", "verification/databases"),
             json=jsonable_encoder(request),
             headers=remove_none_from_headers(
-                {"Key-Inflection": key_inflection, "Idempotency-Key": idempotency_key, "Authorization": self.api_key}
+                {
+                    "Key-Inflection": key_inflection,
+                    "Idempotency-Key": idempotency_key,
+                    "Authorization": f"Bearer  {self.api_key}",
+                }
             ),
             timeout=60,
         )
         if 200 <= _response.status_code < 300:
             return pydantic.parse_obj_as(CreateADatabaseVerificationResponse, _response.json())  # type: ignore
         try:
             _response_json = _response.json()
@@ -53,15 +57,19 @@
         key_inflection: typing.Optional[str] = None,
         idempotency_key: typing.Optional[str] = None,
     ) -> CreateADatabaseVerification1Response:
         _response = httpx.request(
             "POST",
             urllib.parse.urljoin(f"{self._environment.value}/", f"verification/databases/{verification_id}/submit"),
             headers=remove_none_from_headers(
-                {"Key-Inflection": key_inflection, "Idempotency-Key": idempotency_key, "Authorization": self.api_key}
+                {
+                    "Key-Inflection": key_inflection,
+                    "Idempotency-Key": idempotency_key,
+                    "Authorization": f"Bearer  {self.api_key}",
+                }
             ),
             timeout=60,
         )
         if 200 <= _response.status_code < 300:
             return pydantic.parse_obj_as(CreateADatabaseVerification1Response, _response.json())  # type: ignore
         try:
             _response_json = _response.json()
@@ -71,15 +79,17 @@
 
     def retrieve_a_database_verification(
         self, verification_id: str, *, key_inflection: typing.Optional[str] = None
     ) -> RetrieveADatabaseVerificationResponse:
         _response = httpx.request(
             "GET",
             urllib.parse.urljoin(f"{self._environment.value}/", f"verification/databases/{verification_id}"),
-            headers=remove_none_from_headers({"Key-Inflection": key_inflection, "Authorization": self.api_key}),
+            headers=remove_none_from_headers(
+                {"Key-Inflection": key_inflection, "Authorization": f"Bearer  {self.api_key}"}
+            ),
             timeout=60,
         )
         if 200 <= _response.status_code < 300:
             return pydantic.parse_obj_as(RetrieveADatabaseVerificationResponse, _response.json())  # type: ignore
         if _response.status_code == 400:
             raise BadRequestError(pydantic.parse_obj_as(typing.Any, _response.json()))  # type: ignore
         try:
@@ -106,15 +116,15 @@
                 "POST",
                 urllib.parse.urljoin(f"{self._environment.value}/", "verification/databases"),
                 json=jsonable_encoder(request),
                 headers=remove_none_from_headers(
                     {
                         "Key-Inflection": key_inflection,
                         "Idempotency-Key": idempotency_key,
-                        "Authorization": self.api_key,
+                        "Authorization": f"Bearer  {self.api_key}",
                     }
                 ),
                 timeout=60,
             )
         if 200 <= _response.status_code < 300:
             return pydantic.parse_obj_as(CreateADatabaseVerificationResponse, _response.json())  # type: ignore
         try:
@@ -134,15 +144,15 @@
             _response = await _client.request(
                 "POST",
                 urllib.parse.urljoin(f"{self._environment.value}/", f"verification/databases/{verification_id}/submit"),
                 headers=remove_none_from_headers(
                     {
                         "Key-Inflection": key_inflection,
                         "Idempotency-Key": idempotency_key,
-                        "Authorization": self.api_key,
+                        "Authorization": f"Bearer  {self.api_key}",
                     }
                 ),
                 timeout=60,
             )
         if 200 <= _response.status_code < 300:
             return pydantic.parse_obj_as(CreateADatabaseVerification1Response, _response.json())  # type: ignore
         try:
@@ -154,15 +164,17 @@
     async def retrieve_a_database_verification(
         self, verification_id: str, *, key_inflection: typing.Optional[str] = None
     ) -> RetrieveADatabaseVerificationResponse:
         async with httpx.AsyncClient() as _client:
             _response = await _client.request(
                 "GET",
                 urllib.parse.urljoin(f"{self._environment.value}/", f"verification/databases/{verification_id}"),
-                headers=remove_none_from_headers({"Key-Inflection": key_inflection, "Authorization": self.api_key}),
+                headers=remove_none_from_headers(
+                    {"Key-Inflection": key_inflection, "Authorization": f"Bearer  {self.api_key}"}
+                ),
                 timeout=60,
             )
         if 200 <= _response.status_code < 300:
             return pydantic.parse_obj_as(RetrieveADatabaseVerificationResponse, _response.json())  # type: ignore
         if _response.status_code == 400:
             raise BadRequestError(pydantic.parse_obj_as(typing.Any, _response.json()))  # type: ignore
         try:
```

### Comparing `fern_persona-0.0.2/src/persona/resources/document_verifications/client.py` & `fern_persona-0.0.3/src/persona/resources/document_verifications/client.py`

 * *Files 3% similar despite different names*

```diff
@@ -30,15 +30,19 @@
         idempotency_key: typing.Optional[str] = None,
     ) -> CreateADocumentVerificationResponse:
         _response = httpx.request(
             "POST",
             urllib.parse.urljoin(f"{self._environment.value}/", "verification/documents"),
             json=jsonable_encoder({"data": data}),
             headers=remove_none_from_headers(
-                {"Key-Inflection": key_inflection, "Idempotency-Key": idempotency_key, "Authorization": self.api_key}
+                {
+                    "Key-Inflection": key_inflection,
+                    "Idempotency-Key": idempotency_key,
+                    "Authorization": f"Bearer  {self.api_key}",
+                }
             ),
             timeout=60,
         )
         if 200 <= _response.status_code < 300:
             return pydantic.parse_obj_as(CreateADocumentVerificationResponse, _response.json())  # type: ignore
         try:
             _response_json = _response.json()
@@ -53,15 +57,19 @@
         key_inflection: typing.Optional[str] = None,
         idempotency_key: typing.Optional[str] = None,
     ) -> SubmitADocumentVerificationResponse:
         _response = httpx.request(
             "POST",
             urllib.parse.urljoin(f"{self._environment.value}/", f"verification/documents/{verification_id}/submit"),
             headers=remove_none_from_headers(
-                {"Key-Inflection": key_inflection, "Idempotency-Key": idempotency_key, "Authorization": self.api_key}
+                {
+                    "Key-Inflection": key_inflection,
+                    "Idempotency-Key": idempotency_key,
+                    "Authorization": f"Bearer  {self.api_key}",
+                }
             ),
             timeout=60,
         )
         if 200 <= _response.status_code < 300:
             return pydantic.parse_obj_as(SubmitADocumentVerificationResponse, _response.json())  # type: ignore
         if _response.status_code == 400:
             raise BadRequestError(pydantic.parse_obj_as(typing.Any, _response.json()))  # type: ignore
@@ -73,15 +81,17 @@
 
     def retrieve_a_document_verification(
         self, verification_id: str, *, key_inflection: typing.Optional[str] = None
     ) -> None:
         _response = httpx.request(
             "GET",
             urllib.parse.urljoin(f"{self._environment.value}/", f"verification/documents/{verification_id}"),
-            headers=remove_none_from_headers({"Key-Inflection": key_inflection, "Authorization": self.api_key}),
+            headers=remove_none_from_headers(
+                {"Key-Inflection": key_inflection, "Authorization": f"Bearer  {self.api_key}"}
+            ),
             timeout=60,
         )
         if 200 <= _response.status_code < 300:
             return
         if _response.status_code == 400:
             raise BadRequestError(pydantic.parse_obj_as(typing.Any, _response.json()))  # type: ignore
         try:
@@ -108,15 +118,15 @@
                 "POST",
                 urllib.parse.urljoin(f"{self._environment.value}/", "verification/documents"),
                 json=jsonable_encoder({"data": data}),
                 headers=remove_none_from_headers(
                     {
                         "Key-Inflection": key_inflection,
                         "Idempotency-Key": idempotency_key,
-                        "Authorization": self.api_key,
+                        "Authorization": f"Bearer  {self.api_key}",
                     }
                 ),
                 timeout=60,
             )
         if 200 <= _response.status_code < 300:
             return pydantic.parse_obj_as(CreateADocumentVerificationResponse, _response.json())  # type: ignore
         try:
@@ -136,15 +146,15 @@
             _response = await _client.request(
                 "POST",
                 urllib.parse.urljoin(f"{self._environment.value}/", f"verification/documents/{verification_id}/submit"),
                 headers=remove_none_from_headers(
                     {
                         "Key-Inflection": key_inflection,
                         "Idempotency-Key": idempotency_key,
-                        "Authorization": self.api_key,
+                        "Authorization": f"Bearer  {self.api_key}",
                     }
                 ),
                 timeout=60,
             )
         if 200 <= _response.status_code < 300:
             return pydantic.parse_obj_as(SubmitADocumentVerificationResponse, _response.json())  # type: ignore
         if _response.status_code == 400:
@@ -158,15 +168,17 @@
     async def retrieve_a_document_verification(
         self, verification_id: str, *, key_inflection: typing.Optional[str] = None
     ) -> None:
         async with httpx.AsyncClient() as _client:
             _response = await _client.request(
                 "GET",
                 urllib.parse.urljoin(f"{self._environment.value}/", f"verification/documents/{verification_id}"),
-                headers=remove_none_from_headers({"Key-Inflection": key_inflection, "Authorization": self.api_key}),
+                headers=remove_none_from_headers(
+                    {"Key-Inflection": key_inflection, "Authorization": f"Bearer  {self.api_key}"}
+                ),
                 timeout=60,
             )
         if 200 <= _response.status_code < 300:
             return
         if _response.status_code == 400:
             raise BadRequestError(pydantic.parse_obj_as(typing.Any, _response.json()))  # type: ignore
         try:
```

### Comparing `fern_persona-0.0.2/src/persona/resources/documents/client.py` & `fern_persona-0.0.3/src/persona/resources/documents/client.py`

 * *Files 6% similar despite different names*

```diff
@@ -27,15 +27,17 @@
 
     def retrieve_a_document(
         self, document_id: str, *, key_inflection: typing.Optional[str] = None
     ) -> RetrieveADocumentResponse:
         _response = httpx.request(
             "GET",
             urllib.parse.urljoin(f"{self._environment.value}/", f"documents/{document_id}"),
-            headers=remove_none_from_headers({"Key-Inflection": key_inflection, "Authorization": self.api_key}),
+            headers=remove_none_from_headers(
+                {"Key-Inflection": key_inflection, "Authorization": f"Bearer  {self.api_key}"}
+            ),
             timeout=60,
         )
         if 200 <= _response.status_code < 300:
             return pydantic.parse_obj_as(RetrieveADocumentResponse, _response.json())  # type: ignore
         if _response.status_code == 400:
             raise BadRequestError(pydantic.parse_obj_as(typing.Any, _response.json()))  # type: ignore
         try:
@@ -52,15 +54,19 @@
         idempotency_key: typing.Optional[str] = None,
     ) -> CreateADocumentResponse:
         _response = httpx.request(
             "POST",
             urllib.parse.urljoin(f"{self._environment.value}/", "document/generics"),
             json=jsonable_encoder({"data": data}),
             headers=remove_none_from_headers(
-                {"Key-Inflection": key_inflection, "Idempotency-Key": idempotency_key, "Authorization": self.api_key}
+                {
+                    "Key-Inflection": key_inflection,
+                    "Idempotency-Key": idempotency_key,
+                    "Authorization": f"Bearer  {self.api_key}",
+                }
             ),
             timeout=60,
         )
         if 200 <= _response.status_code < 300:
             return pydantic.parse_obj_as(CreateADocumentResponse, _response.json())  # type: ignore
         if _response.status_code == 400:
             raise BadRequestError(pydantic.parse_obj_as(typing.Any, _response.json()))  # type: ignore
@@ -79,15 +85,19 @@
         idempotency_key: typing.Optional[str] = None,
     ) -> UpdateADocumentResponse:
         _response = httpx.request(
             "PATCH",
             urllib.parse.urljoin(f"{self._environment.value}/", f"document/generics/{document_id}"),
             json=jsonable_encoder({"data": data}),
             headers=remove_none_from_headers(
-                {"Key-Inflection": key_inflection, "Idempotency-Key": idempotency_key, "Authorization": self.api_key}
+                {
+                    "Key-Inflection": key_inflection,
+                    "Idempotency-Key": idempotency_key,
+                    "Authorization": f"Bearer  {self.api_key}",
+                }
             ),
             timeout=60,
         )
         if 200 <= _response.status_code < 300:
             return pydantic.parse_obj_as(UpdateADocumentResponse, _response.json())  # type: ignore
         if _response.status_code == 400:
             raise BadRequestError(pydantic.parse_obj_as(typing.Any, _response.json()))  # type: ignore
@@ -104,15 +114,19 @@
         key_inflection: typing.Optional[str] = None,
         idempotency_key: typing.Optional[str] = None,
     ) -> SubmitADocumentResponse:
         _response = httpx.request(
             "POST",
             urllib.parse.urljoin(f"{self._environment.value}/", f"document/generics/{document_id}/submit"),
             headers=remove_none_from_headers(
-                {"Key-Inflection": key_inflection, "Idempotency-Key": idempotency_key, "Authorization": self.api_key}
+                {
+                    "Key-Inflection": key_inflection,
+                    "Idempotency-Key": idempotency_key,
+                    "Authorization": f"Bearer  {self.api_key}",
+                }
             ),
             timeout=60,
         )
         if 200 <= _response.status_code < 300:
             return pydantic.parse_obj_as(SubmitADocumentResponse, _response.json())  # type: ignore
         if _response.status_code == 400:
             raise BadRequestError(pydantic.parse_obj_as(typing.Any, _response.json()))  # type: ignore
@@ -131,15 +145,17 @@
     async def retrieve_a_document(
         self, document_id: str, *, key_inflection: typing.Optional[str] = None
     ) -> RetrieveADocumentResponse:
         async with httpx.AsyncClient() as _client:
             _response = await _client.request(
                 "GET",
                 urllib.parse.urljoin(f"{self._environment.value}/", f"documents/{document_id}"),
-                headers=remove_none_from_headers({"Key-Inflection": key_inflection, "Authorization": self.api_key}),
+                headers=remove_none_from_headers(
+                    {"Key-Inflection": key_inflection, "Authorization": f"Bearer  {self.api_key}"}
+                ),
                 timeout=60,
             )
         if 200 <= _response.status_code < 300:
             return pydantic.parse_obj_as(RetrieveADocumentResponse, _response.json())  # type: ignore
         if _response.status_code == 400:
             raise BadRequestError(pydantic.parse_obj_as(typing.Any, _response.json()))  # type: ignore
         try:
@@ -160,15 +176,15 @@
                 "POST",
                 urllib.parse.urljoin(f"{self._environment.value}/", "document/generics"),
                 json=jsonable_encoder({"data": data}),
                 headers=remove_none_from_headers(
                     {
                         "Key-Inflection": key_inflection,
                         "Idempotency-Key": idempotency_key,
-                        "Authorization": self.api_key,
+                        "Authorization": f"Bearer  {self.api_key}",
                     }
                 ),
                 timeout=60,
             )
         if 200 <= _response.status_code < 300:
             return pydantic.parse_obj_as(CreateADocumentResponse, _response.json())  # type: ignore
         if _response.status_code == 400:
@@ -192,15 +208,15 @@
                 "PATCH",
                 urllib.parse.urljoin(f"{self._environment.value}/", f"document/generics/{document_id}"),
                 json=jsonable_encoder({"data": data}),
                 headers=remove_none_from_headers(
                     {
                         "Key-Inflection": key_inflection,
                         "Idempotency-Key": idempotency_key,
-                        "Authorization": self.api_key,
+                        "Authorization": f"Bearer  {self.api_key}",
                     }
                 ),
                 timeout=60,
             )
         if 200 <= _response.status_code < 300:
             return pydantic.parse_obj_as(UpdateADocumentResponse, _response.json())  # type: ignore
         if _response.status_code == 400:
@@ -222,15 +238,15 @@
             _response = await _client.request(
                 "POST",
                 urllib.parse.urljoin(f"{self._environment.value}/", f"document/generics/{document_id}/submit"),
                 headers=remove_none_from_headers(
                     {
                         "Key-Inflection": key_inflection,
                         "Idempotency-Key": idempotency_key,
-                        "Authorization": self.api_key,
+                        "Authorization": f"Bearer  {self.api_key}",
                     }
                 ),
                 timeout=60,
             )
         if 200 <= _response.status_code < 300:
             return pydantic.parse_obj_as(SubmitADocumentResponse, _response.json())  # type: ignore
         if _response.status_code == 400:
```

### Comparing `fern_persona-0.0.2/src/persona/resources/email_address_verifications/client.py` & `fern_persona-0.0.3/src/persona/resources/email_address_verifications/client.py`

 * *Files 3% similar despite different names*

```diff
@@ -37,15 +37,19 @@
         idempotency_key: typing.Optional[str] = None,
     ) -> CreateAnEmailAddressVerificationResponse:
         _response = httpx.request(
             "POST",
             urllib.parse.urljoin(f"{self._environment.value}/", "verification/email-addresses"),
             json=jsonable_encoder({"data": data}),
             headers=remove_none_from_headers(
-                {"Key-Inflection": key_inflection, "Idempotency-Key": idempotency_key, "Authorization": self.api_key}
+                {
+                    "Key-Inflection": key_inflection,
+                    "Idempotency-Key": idempotency_key,
+                    "Authorization": f"Bearer  {self.api_key}",
+                }
             ),
             timeout=60,
         )
         if 200 <= _response.status_code < 300:
             return pydantic.parse_obj_as(CreateAnEmailAddressVerificationResponse, _response.json())  # type: ignore
         try:
             _response_json = _response.json()
@@ -61,15 +65,15 @@
             _request["data"] = data
         _response = httpx.request(
             "POST",
             urllib.parse.urljoin(
                 f"{self._environment.value}/", f"verification/email-addresses/{verification_id}/send-confirmation-code"
             ),
             json=jsonable_encoder(_request),
-            headers=remove_none_from_headers({"Authorization": self.api_key}),
+            headers=remove_none_from_headers({"Authorization": f"Bearer  {self.api_key}"}),
             timeout=60,
         )
         if 200 <= _response.status_code < 300:
             return pydantic.parse_obj_as(SendAnEmailResponse, _response.json())  # type: ignore
         if _response.status_code == 400:
             raise BadRequestError(pydantic.parse_obj_as(typing.Any, _response.json()))  # type: ignore
         try:
@@ -83,15 +87,15 @@
     ) -> ConfirmAPhoneNumberVerification1Response:
         _response = httpx.request(
             "POST",
             urllib.parse.urljoin(
                 f"{self._environment.value}/", f"verification/email-addresses/{verification_id}/confirm"
             ),
             json=jsonable_encoder({"data": data}),
-            headers=remove_none_from_headers({"Authorization": self.api_key}),
+            headers=remove_none_from_headers({"Authorization": f"Bearer  {self.api_key}"}),
             timeout=60,
         )
         if 200 <= _response.status_code < 300:
             return pydantic.parse_obj_as(ConfirmAPhoneNumberVerification1Response, _response.json())  # type: ignore
         if _response.status_code == 400:
             raise BadRequestError(pydantic.parse_obj_as(typing.Any, _response.json()))  # type: ignore
         try:
@@ -102,15 +106,17 @@
 
     def retrieve_a_email_address_verification(
         self, verification_id: str, *, key_inflection: typing.Optional[str] = None
     ) -> RetrieveAEmailAddressVerificationResponse:
         _response = httpx.request(
             "GET",
             urllib.parse.urljoin(f"{self._environment.value}/", f"verification/email-address/{verification_id}"),
-            headers=remove_none_from_headers({"Key-Inflection": key_inflection, "Authorization": self.api_key}),
+            headers=remove_none_from_headers(
+                {"Key-Inflection": key_inflection, "Authorization": f"Bearer  {self.api_key}"}
+            ),
             timeout=60,
         )
         if 200 <= _response.status_code < 300:
             return pydantic.parse_obj_as(RetrieveAEmailAddressVerificationResponse, _response.json())  # type: ignore
         if _response.status_code == 400:
             raise BadRequestError(pydantic.parse_obj_as(typing.Any, _response.json()))  # type: ignore
         try:
@@ -137,15 +143,15 @@
                 "POST",
                 urllib.parse.urljoin(f"{self._environment.value}/", "verification/email-addresses"),
                 json=jsonable_encoder({"data": data}),
                 headers=remove_none_from_headers(
                     {
                         "Key-Inflection": key_inflection,
                         "Idempotency-Key": idempotency_key,
-                        "Authorization": self.api_key,
+                        "Authorization": f"Bearer  {self.api_key}",
                     }
                 ),
                 timeout=60,
             )
         if 200 <= _response.status_code < 300:
             return pydantic.parse_obj_as(CreateAnEmailAddressVerificationResponse, _response.json())  # type: ignore
         try:
@@ -164,15 +170,15 @@
             _response = await _client.request(
                 "POST",
                 urllib.parse.urljoin(
                     f"{self._environment.value}/",
                     f"verification/email-addresses/{verification_id}/send-confirmation-code",
                 ),
                 json=jsonable_encoder(_request),
-                headers=remove_none_from_headers({"Authorization": self.api_key}),
+                headers=remove_none_from_headers({"Authorization": f"Bearer  {self.api_key}"}),
                 timeout=60,
             )
         if 200 <= _response.status_code < 300:
             return pydantic.parse_obj_as(SendAnEmailResponse, _response.json())  # type: ignore
         if _response.status_code == 400:
             raise BadRequestError(pydantic.parse_obj_as(typing.Any, _response.json()))  # type: ignore
         try:
@@ -187,15 +193,15 @@
         async with httpx.AsyncClient() as _client:
             _response = await _client.request(
                 "POST",
                 urllib.parse.urljoin(
                     f"{self._environment.value}/", f"verification/email-addresses/{verification_id}/confirm"
                 ),
                 json=jsonable_encoder({"data": data}),
-                headers=remove_none_from_headers({"Authorization": self.api_key}),
+                headers=remove_none_from_headers({"Authorization": f"Bearer  {self.api_key}"}),
                 timeout=60,
             )
         if 200 <= _response.status_code < 300:
             return pydantic.parse_obj_as(ConfirmAPhoneNumberVerification1Response, _response.json())  # type: ignore
         if _response.status_code == 400:
             raise BadRequestError(pydantic.parse_obj_as(typing.Any, _response.json()))  # type: ignore
         try:
@@ -207,15 +213,17 @@
     async def retrieve_a_email_address_verification(
         self, verification_id: str, *, key_inflection: typing.Optional[str] = None
     ) -> RetrieveAEmailAddressVerificationResponse:
         async with httpx.AsyncClient() as _client:
             _response = await _client.request(
                 "GET",
                 urllib.parse.urljoin(f"{self._environment.value}/", f"verification/email-address/{verification_id}"),
-                headers=remove_none_from_headers({"Key-Inflection": key_inflection, "Authorization": self.api_key}),
+                headers=remove_none_from_headers(
+                    {"Key-Inflection": key_inflection, "Authorization": f"Bearer  {self.api_key}"}
+                ),
                 timeout=60,
             )
         if 200 <= _response.status_code < 300:
             return pydantic.parse_obj_as(RetrieveAEmailAddressVerificationResponse, _response.json())  # type: ignore
         if _response.status_code == 400:
             raise BadRequestError(pydantic.parse_obj_as(typing.Any, _response.json()))  # type: ignore
         try:
```

### Comparing `fern_persona-0.0.2/src/persona/resources/events/client.py` & `fern_persona-0.0.3/src/persona/resources/events/client.py`

 * *Files 9% similar despite different names*

```diff
@@ -38,15 +38,17 @@
                 "page[before]": page_before,
                 "page[after]": page_after,
                 "page[size]": page_size,
                 "filter[name]": filter_name,
                 "filter[object_id]": filter_object_id,
                 "filter[id]": filter_id,
             },
-            headers=remove_none_from_headers({"Key-Inflection": key_inflection, "Authorization": self.api_key}),
+            headers=remove_none_from_headers(
+                {"Key-Inflection": key_inflection, "Authorization": f"Bearer  {self.api_key}"}
+            ),
             timeout=60,
         )
         if 200 <= _response.status_code < 300:
             return pydantic.parse_obj_as(ListAllEventsResponse, _response.json())  # type: ignore
         if _response.status_code == 400:
             raise BadRequestError(pydantic.parse_obj_as(typing.Any, _response.json()))  # type: ignore
         try:
@@ -57,15 +59,17 @@
 
     def retrieve_an_event(
         self, event_id: str, *, key_inflection: typing.Optional[str] = None
     ) -> RetrieveAnEventResponse:
         _response = httpx.request(
             "GET",
             urllib.parse.urljoin(f"{self._environment.value}/", f"events/{event_id}"),
-            headers=remove_none_from_headers({"Key-Inflection": key_inflection, "Authorization": self.api_key}),
+            headers=remove_none_from_headers(
+                {"Key-Inflection": key_inflection, "Authorization": f"Bearer  {self.api_key}"}
+            ),
             timeout=60,
         )
         if 200 <= _response.status_code < 300:
             return pydantic.parse_obj_as(RetrieveAnEventResponse, _response.json())  # type: ignore
         if _response.status_code == 400:
             raise BadRequestError(pydantic.parse_obj_as(typing.Any, _response.json()))  # type: ignore
         try:
@@ -99,15 +103,17 @@
                     "page[before]": page_before,
                     "page[after]": page_after,
                     "page[size]": page_size,
                     "filter[name]": filter_name,
                     "filter[object_id]": filter_object_id,
                     "filter[id]": filter_id,
                 },
-                headers=remove_none_from_headers({"Key-Inflection": key_inflection, "Authorization": self.api_key}),
+                headers=remove_none_from_headers(
+                    {"Key-Inflection": key_inflection, "Authorization": f"Bearer  {self.api_key}"}
+                ),
                 timeout=60,
             )
         if 200 <= _response.status_code < 300:
             return pydantic.parse_obj_as(ListAllEventsResponse, _response.json())  # type: ignore
         if _response.status_code == 400:
             raise BadRequestError(pydantic.parse_obj_as(typing.Any, _response.json()))  # type: ignore
         try:
@@ -119,15 +125,17 @@
     async def retrieve_an_event(
         self, event_id: str, *, key_inflection: typing.Optional[str] = None
     ) -> RetrieveAnEventResponse:
         async with httpx.AsyncClient() as _client:
             _response = await _client.request(
                 "GET",
                 urllib.parse.urljoin(f"{self._environment.value}/", f"events/{event_id}"),
-                headers=remove_none_from_headers({"Key-Inflection": key_inflection, "Authorization": self.api_key}),
+                headers=remove_none_from_headers(
+                    {"Key-Inflection": key_inflection, "Authorization": f"Bearer  {self.api_key}"}
+                ),
                 timeout=60,
             )
         if 200 <= _response.status_code < 300:
             return pydantic.parse_obj_as(RetrieveAnEventResponse, _response.json())  # type: ignore
         if _response.status_code == 400:
             raise BadRequestError(pydantic.parse_obj_as(typing.Any, _response.json()))  # type: ignore
         try:
```

### Comparing `fern_persona-0.0.2/src/persona/resources/government_id_documents/client.py` & `fern_persona-0.0.3/src/persona/resources/government_id_documents/client.py`

 * *Files 4% similar despite different names*

```diff
@@ -32,15 +32,19 @@
         idempotency_key: typing.Optional[str] = None,
     ) -> CreateAGovernmentIdDocumentResponse:
         _response = httpx.request(
             "POST",
             urllib.parse.urljoin(f"{self._environment.value}/", "document/government-ids"),
             json=jsonable_encoder({"data": data}),
             headers=remove_none_from_headers(
-                {"Key-Inflection": key_inflection, "Idempotency-Key": idempotency_key, "Authorization": self.api_key}
+                {
+                    "Key-Inflection": key_inflection,
+                    "Idempotency-Key": idempotency_key,
+                    "Authorization": f"Bearer  {self.api_key}",
+                }
             ),
             timeout=60,
         )
         if 200 <= _response.status_code < 300:
             return pydantic.parse_obj_as(CreateAGovernmentIdDocumentResponse, _response.json())  # type: ignore
         if _response.status_code == 400:
             raise BadRequestError(pydantic.parse_obj_as(typing.Any, _response.json()))  # type: ignore
@@ -59,15 +63,19 @@
         idempotency_key: typing.Optional[str] = None,
     ) -> UpdateAGovernmentIdDocumentResponse:
         _response = httpx.request(
             "PATCH",
             urllib.parse.urljoin(f"{self._environment.value}/", f"document/government-ids/{document_id}"),
             json=jsonable_encoder({"data": data}),
             headers=remove_none_from_headers(
-                {"Key-Inflection": key_inflection, "Idempotency-Key": idempotency_key, "Authorization": self.api_key}
+                {
+                    "Key-Inflection": key_inflection,
+                    "Idempotency-Key": idempotency_key,
+                    "Authorization": f"Bearer  {self.api_key}",
+                }
             ),
             timeout=60,
         )
         if 200 <= _response.status_code < 300:
             return pydantic.parse_obj_as(UpdateAGovernmentIdDocumentResponse, _response.json())  # type: ignore
         if _response.status_code == 400:
             raise BadRequestError(pydantic.parse_obj_as(typing.Any, _response.json()))  # type: ignore
@@ -84,15 +92,19 @@
         key_inflection: typing.Optional[str] = None,
         idempotency_key: typing.Optional[str] = None,
     ) -> SubmitAGovernmentIdDocumentResponse:
         _response = httpx.request(
             "POST",
             urllib.parse.urljoin(f"{self._environment.value}/", f"document/government-ids/{document_id}/submit"),
             headers=remove_none_from_headers(
-                {"Key-Inflection": key_inflection, "Idempotency-Key": idempotency_key, "Authorization": self.api_key}
+                {
+                    "Key-Inflection": key_inflection,
+                    "Idempotency-Key": idempotency_key,
+                    "Authorization": f"Bearer  {self.api_key}",
+                }
             ),
             timeout=60,
         )
         if 200 <= _response.status_code < 300:
             return pydantic.parse_obj_as(SubmitAGovernmentIdDocumentResponse, _response.json())  # type: ignore
         if _response.status_code == 400:
             raise BadRequestError(pydantic.parse_obj_as(typing.Any, _response.json()))  # type: ignore
@@ -120,15 +132,15 @@
                 "POST",
                 urllib.parse.urljoin(f"{self._environment.value}/", "document/government-ids"),
                 json=jsonable_encoder({"data": data}),
                 headers=remove_none_from_headers(
                     {
                         "Key-Inflection": key_inflection,
                         "Idempotency-Key": idempotency_key,
-                        "Authorization": self.api_key,
+                        "Authorization": f"Bearer  {self.api_key}",
                     }
                 ),
                 timeout=60,
             )
         if 200 <= _response.status_code < 300:
             return pydantic.parse_obj_as(CreateAGovernmentIdDocumentResponse, _response.json())  # type: ignore
         if _response.status_code == 400:
@@ -152,15 +164,15 @@
                 "PATCH",
                 urllib.parse.urljoin(f"{self._environment.value}/", f"document/government-ids/{document_id}"),
                 json=jsonable_encoder({"data": data}),
                 headers=remove_none_from_headers(
                     {
                         "Key-Inflection": key_inflection,
                         "Idempotency-Key": idempotency_key,
-                        "Authorization": self.api_key,
+                        "Authorization": f"Bearer  {self.api_key}",
                     }
                 ),
                 timeout=60,
             )
         if 200 <= _response.status_code < 300:
             return pydantic.parse_obj_as(UpdateAGovernmentIdDocumentResponse, _response.json())  # type: ignore
         if _response.status_code == 400:
@@ -182,15 +194,15 @@
             _response = await _client.request(
                 "POST",
                 urllib.parse.urljoin(f"{self._environment.value}/", f"document/government-ids/{document_id}/submit"),
                 headers=remove_none_from_headers(
                     {
                         "Key-Inflection": key_inflection,
                         "Idempotency-Key": idempotency_key,
-                        "Authorization": self.api_key,
+                        "Authorization": f"Bearer  {self.api_key}",
                     }
                 ),
                 timeout=60,
             )
         if 200 <= _response.status_code < 300:
             return pydantic.parse_obj_as(SubmitAGovernmentIdDocumentResponse, _response.json())  # type: ignore
         if _response.status_code == 400:
```

### Comparing `fern_persona-0.0.2/src/persona/resources/government_id_verifications/client.py` & `fern_persona-0.0.3/src/persona/resources/government_id_verifications/client.py`

 * *Files 3% similar despite different names*

```diff
@@ -33,15 +33,19 @@
         idempotency_key: typing.Optional[str] = None,
     ) -> CreateAGovIdVerificationResponse:
         _response = httpx.request(
             "POST",
             urllib.parse.urljoin(f"{self._environment.value}/", "verification/government-ids"),
             json=jsonable_encoder({"data": data}),
             headers=remove_none_from_headers(
-                {"Key-Inflection": key_inflection, "Idempotency-Key": idempotency_key, "Authorization": self.api_key}
+                {
+                    "Key-Inflection": key_inflection,
+                    "Idempotency-Key": idempotency_key,
+                    "Authorization": f"Bearer  {self.api_key}",
+                }
             ),
             timeout=60,
         )
         if 200 <= _response.status_code < 300:
             return pydantic.parse_obj_as(CreateAGovIdVerificationResponse, _response.json())  # type: ignore
         try:
             _response_json = _response.json()
@@ -58,15 +62,19 @@
     ) -> SubmitAGovernmentIdVerificationResponse:
         _response = httpx.request(
             "POST",
             urllib.parse.urljoin(
                 f"{self._environment.value}/", f"verification/government-ids/{verification_id}/submit"
             ),
             headers=remove_none_from_headers(
-                {"Key-Inflection": key_inflection, "Idempotency-Key": idempotency_key, "Authorization": self.api_key}
+                {
+                    "Key-Inflection": key_inflection,
+                    "Idempotency-Key": idempotency_key,
+                    "Authorization": f"Bearer  {self.api_key}",
+                }
             ),
             timeout=60,
         )
         if 200 <= _response.status_code < 300:
             return pydantic.parse_obj_as(SubmitAGovernmentIdVerificationResponse, _response.json())  # type: ignore
         if _response.status_code == 400:
             raise BadRequestError(pydantic.parse_obj_as(typing.Any, _response.json()))  # type: ignore
@@ -85,15 +93,19 @@
         idempotency_key: typing.Optional[str] = None,
     ) -> UpdateAGovernmentIdVerificationResponse:
         _response = httpx.request(
             "PATCH",
             urllib.parse.urljoin(f"{self._environment.value}/", f"verifications/government-ids/{verification_id}"),
             json=jsonable_encoder({"data": data}),
             headers=remove_none_from_headers(
-                {"Key-Inflection": key_inflection, "Idempotency-Key": idempotency_key, "Authorization": self.api_key}
+                {
+                    "Key-Inflection": key_inflection,
+                    "Idempotency-Key": idempotency_key,
+                    "Authorization": f"Bearer  {self.api_key}",
+                }
             ),
             timeout=60,
         )
         if 200 <= _response.status_code < 300:
             return pydantic.parse_obj_as(UpdateAGovernmentIdVerificationResponse, _response.json())  # type: ignore
         if _response.status_code == 400:
             raise BadRequestError(pydantic.parse_obj_as(typing.Any, _response.json()))  # type: ignore
@@ -105,15 +117,17 @@
 
     def retrieve_a_government_id_verification(
         self, verification_id: str, *, key_inflection: typing.Optional[str] = None
     ) -> RetrieveAGovernmentIdVerificationResponse:
         _response = httpx.request(
             "GET",
             urllib.parse.urljoin(f"{self._environment.value}/", f"verification/government-ids/{verification_id}"),
-            headers=remove_none_from_headers({"Key-Inflection": key_inflection, "Authorization": self.api_key}),
+            headers=remove_none_from_headers(
+                {"Key-Inflection": key_inflection, "Authorization": f"Bearer  {self.api_key}"}
+            ),
             timeout=60,
         )
         if 200 <= _response.status_code < 300:
             return pydantic.parse_obj_as(RetrieveAGovernmentIdVerificationResponse, _response.json())  # type: ignore
         if _response.status_code == 400:
             raise BadRequestError(pydantic.parse_obj_as(typing.Any, _response.json()))  # type: ignore
         try:
@@ -140,15 +154,15 @@
                 "POST",
                 urllib.parse.urljoin(f"{self._environment.value}/", "verification/government-ids"),
                 json=jsonable_encoder({"data": data}),
                 headers=remove_none_from_headers(
                     {
                         "Key-Inflection": key_inflection,
                         "Idempotency-Key": idempotency_key,
-                        "Authorization": self.api_key,
+                        "Authorization": f"Bearer  {self.api_key}",
                     }
                 ),
                 timeout=60,
             )
         if 200 <= _response.status_code < 300:
             return pydantic.parse_obj_as(CreateAGovIdVerificationResponse, _response.json())  # type: ignore
         try:
@@ -170,15 +184,15 @@
                 urllib.parse.urljoin(
                     f"{self._environment.value}/", f"verification/government-ids/{verification_id}/submit"
                 ),
                 headers=remove_none_from_headers(
                     {
                         "Key-Inflection": key_inflection,
                         "Idempotency-Key": idempotency_key,
-                        "Authorization": self.api_key,
+                        "Authorization": f"Bearer  {self.api_key}",
                     }
                 ),
                 timeout=60,
             )
         if 200 <= _response.status_code < 300:
             return pydantic.parse_obj_as(SubmitAGovernmentIdVerificationResponse, _response.json())  # type: ignore
         if _response.status_code == 400:
@@ -202,15 +216,15 @@
                 "PATCH",
                 urllib.parse.urljoin(f"{self._environment.value}/", f"verifications/government-ids/{verification_id}"),
                 json=jsonable_encoder({"data": data}),
                 headers=remove_none_from_headers(
                     {
                         "Key-Inflection": key_inflection,
                         "Idempotency-Key": idempotency_key,
-                        "Authorization": self.api_key,
+                        "Authorization": f"Bearer  {self.api_key}",
                     }
                 ),
                 timeout=60,
             )
         if 200 <= _response.status_code < 300:
             return pydantic.parse_obj_as(UpdateAGovernmentIdVerificationResponse, _response.json())  # type: ignore
         if _response.status_code == 400:
@@ -224,15 +238,17 @@
     async def retrieve_a_government_id_verification(
         self, verification_id: str, *, key_inflection: typing.Optional[str] = None
     ) -> RetrieveAGovernmentIdVerificationResponse:
         async with httpx.AsyncClient() as _client:
             _response = await _client.request(
                 "GET",
                 urllib.parse.urljoin(f"{self._environment.value}/", f"verification/government-ids/{verification_id}"),
-                headers=remove_none_from_headers({"Key-Inflection": key_inflection, "Authorization": self.api_key}),
+                headers=remove_none_from_headers(
+                    {"Key-Inflection": key_inflection, "Authorization": f"Bearer  {self.api_key}"}
+                ),
                 timeout=60,
             )
         if 200 <= _response.status_code < 300:
             return pydantic.parse_obj_as(RetrieveAGovernmentIdVerificationResponse, _response.json())  # type: ignore
         if _response.status_code == 400:
             raise BadRequestError(pydantic.parse_obj_as(typing.Any, _response.json()))  # type: ignore
         try:
```

### Comparing `fern_persona-0.0.2/src/persona/resources/graph_queries/client.py` & `fern_persona-0.0.3/src/persona/resources/graph_queries/client.py`

 * *Files 2% similar despite different names*

```diff
@@ -20,15 +20,15 @@
         self._environment = environment
         self.api_key = api_key
 
     def retrieve_a_graph_query(self, graph_query_id: str) -> None:
         _response = httpx.request(
             "GET",
             urllib.parse.urljoin(f"{self._environment.value}/", f"graph-queries/{graph_query_id}"),
-            headers=remove_none_from_headers({"Authorization": self.api_key}),
+            headers=remove_none_from_headers({"Authorization": f"Bearer  {self.api_key}"}),
             timeout=60,
         )
         if 200 <= _response.status_code < 300:
             return
         try:
             _response_json = _response.json()
         except JSONDecodeError:
@@ -36,15 +36,15 @@
         raise ApiError(status_code=_response.status_code, body=_response_json)
 
     def create_a_graph_query(self, *, data: CreateAGraphQueryRequestData) -> None:
         _response = httpx.request(
             "POST",
             urllib.parse.urljoin(f"{self._environment.value}/", "graph-queries"),
             json=jsonable_encoder({"data": data}),
-            headers=remove_none_from_headers({"Authorization": self.api_key}),
+            headers=remove_none_from_headers({"Authorization": f"Bearer  {self.api_key}"}),
             timeout=60,
         )
         if 200 <= _response.status_code < 300:
             return
         if _response.status_code == 400:
             raise BadRequestError(pydantic.parse_obj_as(typing.Any, _response.json()))  # type: ignore
         try:
@@ -60,15 +60,15 @@
         self.api_key = api_key
 
     async def retrieve_a_graph_query(self, graph_query_id: str) -> None:
         async with httpx.AsyncClient() as _client:
             _response = await _client.request(
                 "GET",
                 urllib.parse.urljoin(f"{self._environment.value}/", f"graph-queries/{graph_query_id}"),
-                headers=remove_none_from_headers({"Authorization": self.api_key}),
+                headers=remove_none_from_headers({"Authorization": f"Bearer  {self.api_key}"}),
                 timeout=60,
             )
         if 200 <= _response.status_code < 300:
             return
         try:
             _response_json = _response.json()
         except JSONDecodeError:
@@ -77,15 +77,15 @@
 
     async def create_a_graph_query(self, *, data: CreateAGraphQueryRequestData) -> None:
         async with httpx.AsyncClient() as _client:
             _response = await _client.request(
                 "POST",
                 urllib.parse.urljoin(f"{self._environment.value}/", "graph-queries"),
                 json=jsonable_encoder({"data": data}),
-                headers=remove_none_from_headers({"Authorization": self.api_key}),
+                headers=remove_none_from_headers({"Authorization": f"Bearer  {self.api_key}"}),
                 timeout=60,
             )
         if 200 <= _response.status_code < 300:
             return
         if _response.status_code == 400:
             raise BadRequestError(pydantic.parse_obj_as(typing.Any, _response.json()))  # type: ignore
         try:
```

### Comparing `fern_persona-0.0.2/src/persona/resources/importers/client.py` & `fern_persona-0.0.3/src/persona/resources/importers/client.py`

 * *Files 11% similar despite different names*

```diff
@@ -39,15 +39,15 @@
         self._environment = environment
         self.api_key = api_key
 
     def retrieve_an_importer(self, importer_id: str) -> RetrieveAnImporterResponse:
         _response = httpx.request(
             "GET",
             urllib.parse.urljoin(f"{self._environment.value}/", f"importers/{importer_id}"),
-            headers=remove_none_from_headers({"Authorization": self.api_key}),
+            headers=remove_none_from_headers({"Authorization": f"Bearer  {self.api_key}"}),
             timeout=60,
         )
         if 200 <= _response.status_code < 300:
             return pydantic.parse_obj_as(RetrieveAnImporterResponse, _response.json())  # type: ignore
         if _response.status_code == 400:
             raise BadRequestError(pydantic.parse_obj_as(typing.Any, _response.json()))  # type: ignore
         try:
@@ -60,15 +60,15 @@
         _request: typing.Dict[str, typing.Any] = {}
         if data is not OMIT:
             _request["data"] = data
         _response = httpx.request(
             "POST",
             urllib.parse.urljoin(f"{self._environment.value}/", "importer/accounts"),
             json=jsonable_encoder(_request),
-            headers=remove_none_from_headers({"Authorization": self.api_key}),
+            headers=remove_none_from_headers({"Authorization": f"Bearer  {self.api_key}"}),
             timeout=60,
         )
         if 200 <= _response.status_code < 300:
             return pydantic.parse_obj_as(ImportAnAccountResponse, _response.json())  # type: ignore
         if _response.status_code == 400:
             raise BadRequestError(pydantic.parse_obj_as(typing.Any, _response.json()))  # type: ignore
         try:
@@ -83,15 +83,15 @@
         _request: typing.Dict[str, typing.Any] = {}
         if data is not OMIT:
             _request["data"] = data
         _response = httpx.request(
             "POST",
             urllib.parse.urljoin(f"{self._environment.value}/", "importer/list-item/email-addresses"),
             json=jsonable_encoder(_request),
-            headers=remove_none_from_headers({"Authorization": self.api_key}),
+            headers=remove_none_from_headers({"Authorization": f"Bearer  {self.api_key}"}),
             timeout=60,
         )
         if 200 <= _response.status_code < 300:
             return pydantic.parse_obj_as(ImportEmailAddressListsResponse, _response.json())  # type: ignore
         if _response.status_code == 400:
             raise BadRequestError(pydantic.parse_obj_as(typing.Any, _response.json()))  # type: ignore
         try:
@@ -106,15 +106,15 @@
         _request: typing.Dict[str, typing.Any] = {}
         if data is not OMIT:
             _request["data"] = data
         _response = httpx.request(
             "POST",
             urllib.parse.urljoin(f"{self._environment.value}/", "importer/list-item/geolocations"),
             json=jsonable_encoder(_request),
-            headers=remove_none_from_headers({"Authorization": self.api_key}),
+            headers=remove_none_from_headers({"Authorization": f"Bearer  {self.api_key}"}),
             timeout=60,
         )
         if 200 <= _response.status_code < 300:
             return pydantic.parse_obj_as(ImportGeolocationListsResponse, _response.json())  # type: ignore
         if _response.status_code == 400:
             raise BadRequestError(pydantic.parse_obj_as(typing.Any, _response.json()))  # type: ignore
         try:
@@ -129,15 +129,15 @@
         _request: typing.Dict[str, typing.Any] = {}
         if data is not OMIT:
             _request["data"] = data
         _response = httpx.request(
             "POST",
             urllib.parse.urljoin(f"{self._environment.value}/", "importer/list-item/government-id-numbers"),
             json=jsonable_encoder(_request),
-            headers=remove_none_from_headers({"Authorization": self.api_key}),
+            headers=remove_none_from_headers({"Authorization": f"Bearer  {self.api_key}"}),
             timeout=60,
         )
         if 200 <= _response.status_code < 300:
             return pydantic.parse_obj_as(ImportGovernmentIdNumberListsResponse, _response.json())  # type: ignore
         if _response.status_code == 400:
             raise BadRequestError(pydantic.parse_obj_as(typing.Any, _response.json()))  # type: ignore
         try:
@@ -152,15 +152,15 @@
         _request: typing.Dict[str, typing.Any] = {}
         if data is not OMIT:
             _request["data"] = data
         _response = httpx.request(
             "POST",
             urllib.parse.urljoin(f"{self._environment.value}/", "importer/list-item/ip-addresses"),
             json=jsonable_encoder(_request),
-            headers=remove_none_from_headers({"Authorization": self.api_key}),
+            headers=remove_none_from_headers({"Authorization": f"Bearer  {self.api_key}"}),
             timeout=60,
         )
         if 200 <= _response.status_code < 300:
             return pydantic.parse_obj_as(ImportIpAddressListsResponse, _response.json())  # type: ignore
         if _response.status_code == 400:
             raise BadRequestError(pydantic.parse_obj_as(typing.Any, _response.json()))  # type: ignore
         try:
@@ -173,15 +173,15 @@
         _request: typing.Dict[str, typing.Any] = {}
         if data is not OMIT:
             _request["data"] = data
         _response = httpx.request(
             "POST",
             urllib.parse.urljoin(f"{self._environment.value}/", "importer/list-item/names"),
             json=jsonable_encoder(_request),
-            headers=remove_none_from_headers({"Authorization": self.api_key}),
+            headers=remove_none_from_headers({"Authorization": f"Bearer  {self.api_key}"}),
             timeout=60,
         )
         if 200 <= _response.status_code < 300:
             return pydantic.parse_obj_as(ImportNameListsResponse, _response.json())  # type: ignore
         if _response.status_code == 400:
             raise BadRequestError(pydantic.parse_obj_as(typing.Any, _response.json()))  # type: ignore
         try:
@@ -196,15 +196,15 @@
         _request: typing.Dict[str, typing.Any] = {}
         if data is not OMIT:
             _request["data"] = data
         _response = httpx.request(
             "POST",
             urllib.parse.urljoin(f"{self._environment.value}/", "importer/list-item/phone-numbers"),
             json=jsonable_encoder(_request),
-            headers=remove_none_from_headers({"Authorization": self.api_key}),
+            headers=remove_none_from_headers({"Authorization": f"Bearer  {self.api_key}"}),
             timeout=60,
         )
         if 200 <= _response.status_code < 300:
             return pydantic.parse_obj_as(ImportPhoneNumberListsResponse, _response.json())  # type: ignore
         if _response.status_code == 400:
             raise BadRequestError(pydantic.parse_obj_as(typing.Any, _response.json()))  # type: ignore
         try:
@@ -217,15 +217,15 @@
         _request: typing.Dict[str, typing.Any] = {}
         if data is not OMIT:
             _request["data"] = data
         _response = httpx.request(
             "POST",
             urllib.parse.urljoin(f"{self._environment.value}/", "importer/list-item/faces"),
             json=jsonable_encoder(_request),
-            headers=remove_none_from_headers({"Authorization": self.api_key}),
+            headers=remove_none_from_headers({"Authorization": f"Bearer  {self.api_key}"}),
             timeout=60,
         )
         if 200 <= _response.status_code < 300:
             return pydantic.parse_obj_as(ImportFaceListsResponse, _response.json())  # type: ignore
         if _response.status_code == 400:
             raise BadRequestError(pydantic.parse_obj_as(typing.Any, _response.json()))  # type: ignore
         try:
@@ -241,15 +241,15 @@
         self.api_key = api_key
 
     async def retrieve_an_importer(self, importer_id: str) -> RetrieveAnImporterResponse:
         async with httpx.AsyncClient() as _client:
             _response = await _client.request(
                 "GET",
                 urllib.parse.urljoin(f"{self._environment.value}/", f"importers/{importer_id}"),
-                headers=remove_none_from_headers({"Authorization": self.api_key}),
+                headers=remove_none_from_headers({"Authorization": f"Bearer  {self.api_key}"}),
                 timeout=60,
             )
         if 200 <= _response.status_code < 300:
             return pydantic.parse_obj_as(RetrieveAnImporterResponse, _response.json())  # type: ignore
         if _response.status_code == 400:
             raise BadRequestError(pydantic.parse_obj_as(typing.Any, _response.json()))  # type: ignore
         try:
@@ -265,15 +265,15 @@
         if data is not OMIT:
             _request["data"] = data
         async with httpx.AsyncClient() as _client:
             _response = await _client.request(
                 "POST",
                 urllib.parse.urljoin(f"{self._environment.value}/", "importer/accounts"),
                 json=jsonable_encoder(_request),
-                headers=remove_none_from_headers({"Authorization": self.api_key}),
+                headers=remove_none_from_headers({"Authorization": f"Bearer  {self.api_key}"}),
                 timeout=60,
             )
         if 200 <= _response.status_code < 300:
             return pydantic.parse_obj_as(ImportAnAccountResponse, _response.json())  # type: ignore
         if _response.status_code == 400:
             raise BadRequestError(pydantic.parse_obj_as(typing.Any, _response.json()))  # type: ignore
         try:
@@ -289,15 +289,15 @@
         if data is not OMIT:
             _request["data"] = data
         async with httpx.AsyncClient() as _client:
             _response = await _client.request(
                 "POST",
                 urllib.parse.urljoin(f"{self._environment.value}/", "importer/list-item/email-addresses"),
                 json=jsonable_encoder(_request),
-                headers=remove_none_from_headers({"Authorization": self.api_key}),
+                headers=remove_none_from_headers({"Authorization": f"Bearer  {self.api_key}"}),
                 timeout=60,
             )
         if 200 <= _response.status_code < 300:
             return pydantic.parse_obj_as(ImportEmailAddressListsResponse, _response.json())  # type: ignore
         if _response.status_code == 400:
             raise BadRequestError(pydantic.parse_obj_as(typing.Any, _response.json()))  # type: ignore
         try:
@@ -313,15 +313,15 @@
         if data is not OMIT:
             _request["data"] = data
         async with httpx.AsyncClient() as _client:
             _response = await _client.request(
                 "POST",
                 urllib.parse.urljoin(f"{self._environment.value}/", "importer/list-item/geolocations"),
                 json=jsonable_encoder(_request),
-                headers=remove_none_from_headers({"Authorization": self.api_key}),
+                headers=remove_none_from_headers({"Authorization": f"Bearer  {self.api_key}"}),
                 timeout=60,
             )
         if 200 <= _response.status_code < 300:
             return pydantic.parse_obj_as(ImportGeolocationListsResponse, _response.json())  # type: ignore
         if _response.status_code == 400:
             raise BadRequestError(pydantic.parse_obj_as(typing.Any, _response.json()))  # type: ignore
         try:
@@ -337,15 +337,15 @@
         if data is not OMIT:
             _request["data"] = data
         async with httpx.AsyncClient() as _client:
             _response = await _client.request(
                 "POST",
                 urllib.parse.urljoin(f"{self._environment.value}/", "importer/list-item/government-id-numbers"),
                 json=jsonable_encoder(_request),
-                headers=remove_none_from_headers({"Authorization": self.api_key}),
+                headers=remove_none_from_headers({"Authorization": f"Bearer  {self.api_key}"}),
                 timeout=60,
             )
         if 200 <= _response.status_code < 300:
             return pydantic.parse_obj_as(ImportGovernmentIdNumberListsResponse, _response.json())  # type: ignore
         if _response.status_code == 400:
             raise BadRequestError(pydantic.parse_obj_as(typing.Any, _response.json()))  # type: ignore
         try:
@@ -361,15 +361,15 @@
         if data is not OMIT:
             _request["data"] = data
         async with httpx.AsyncClient() as _client:
             _response = await _client.request(
                 "POST",
                 urllib.parse.urljoin(f"{self._environment.value}/", "importer/list-item/ip-addresses"),
                 json=jsonable_encoder(_request),
-                headers=remove_none_from_headers({"Authorization": self.api_key}),
+                headers=remove_none_from_headers({"Authorization": f"Bearer  {self.api_key}"}),
                 timeout=60,
             )
         if 200 <= _response.status_code < 300:
             return pydantic.parse_obj_as(ImportIpAddressListsResponse, _response.json())  # type: ignore
         if _response.status_code == 400:
             raise BadRequestError(pydantic.parse_obj_as(typing.Any, _response.json()))  # type: ignore
         try:
@@ -385,15 +385,15 @@
         if data is not OMIT:
             _request["data"] = data
         async with httpx.AsyncClient() as _client:
             _response = await _client.request(
                 "POST",
                 urllib.parse.urljoin(f"{self._environment.value}/", "importer/list-item/names"),
                 json=jsonable_encoder(_request),
-                headers=remove_none_from_headers({"Authorization": self.api_key}),
+                headers=remove_none_from_headers({"Authorization": f"Bearer  {self.api_key}"}),
                 timeout=60,
             )
         if 200 <= _response.status_code < 300:
             return pydantic.parse_obj_as(ImportNameListsResponse, _response.json())  # type: ignore
         if _response.status_code == 400:
             raise BadRequestError(pydantic.parse_obj_as(typing.Any, _response.json()))  # type: ignore
         try:
@@ -409,15 +409,15 @@
         if data is not OMIT:
             _request["data"] = data
         async with httpx.AsyncClient() as _client:
             _response = await _client.request(
                 "POST",
                 urllib.parse.urljoin(f"{self._environment.value}/", "importer/list-item/phone-numbers"),
                 json=jsonable_encoder(_request),
-                headers=remove_none_from_headers({"Authorization": self.api_key}),
+                headers=remove_none_from_headers({"Authorization": f"Bearer  {self.api_key}"}),
                 timeout=60,
             )
         if 200 <= _response.status_code < 300:
             return pydantic.parse_obj_as(ImportPhoneNumberListsResponse, _response.json())  # type: ignore
         if _response.status_code == 400:
             raise BadRequestError(pydantic.parse_obj_as(typing.Any, _response.json()))  # type: ignore
         try:
@@ -433,15 +433,15 @@
         if data is not OMIT:
             _request["data"] = data
         async with httpx.AsyncClient() as _client:
             _response = await _client.request(
                 "POST",
                 urllib.parse.urljoin(f"{self._environment.value}/", "importer/list-item/faces"),
                 json=jsonable_encoder(_request),
-                headers=remove_none_from_headers({"Authorization": self.api_key}),
+                headers=remove_none_from_headers({"Authorization": f"Bearer  {self.api_key}"}),
                 timeout=60,
             )
         if 200 <= _response.status_code < 300:
             return pydantic.parse_obj_as(ImportFaceListsResponse, _response.json())  # type: ignore
         if _response.status_code == 400:
             raise BadRequestError(pydantic.parse_obj_as(typing.Any, _response.json()))  # type: ignore
         try:
```

### Comparing `fern_persona-0.0.2/src/persona/resources/inquiries/client.py` & `fern_persona-0.0.3/src/persona/resources/inquiries/client.py`

 * *Files 3% similar despite different names*

```diff
@@ -48,15 +48,19 @@
         key_inflection: typing.Optional[str] = None,
         idempotency_key: typing.Optional[str] = None,
     ) -> ResumeAnInquiryResponse:
         _response = httpx.request(
             "POST",
             urllib.parse.urljoin(f"{self._environment.value}/", f"inquiries/{inquiry_id}/resume"),
             headers=remove_none_from_headers(
-                {"Key-Inflection": key_inflection, "Idempotency-Key": idempotency_key, "Authorization": self.api_key}
+                {
+                    "Key-Inflection": key_inflection,
+                    "Idempotency-Key": idempotency_key,
+                    "Authorization": f"Bearer  {self.api_key}",
+                }
             ),
             timeout=60,
         )
         if 200 <= _response.status_code < 300:
             return pydantic.parse_obj_as(ResumeAnInquiryResponse, _response.json())  # type: ignore
         if _response.status_code == 404:
             raise NotFoundError(pydantic.parse_obj_as(typing.Any, _response.json()))  # type: ignore
@@ -68,15 +72,17 @@
 
     def retrieve_an_inquiry(
         self, inquiry_id: str, *, key_inflection: typing.Optional[str] = None
     ) -> RetrieveAnInquiryResponse:
         _response = httpx.request(
             "GET",
             urllib.parse.urljoin(f"{self._environment.value}/", f"inquiries/{inquiry_id}"),
-            headers=remove_none_from_headers({"Key-Inflection": key_inflection, "Authorization": self.api_key}),
+            headers=remove_none_from_headers(
+                {"Key-Inflection": key_inflection, "Authorization": f"Bearer  {self.api_key}"}
+            ),
             timeout=60,
         )
         if 200 <= _response.status_code < 300:
             return pydantic.parse_obj_as(RetrieveAnInquiryResponse, _response.json())  # type: ignore
         if _response.status_code == 404:
             raise NotFoundError(pydantic.parse_obj_as(typing.Any, _response.json()))  # type: ignore
         try:
@@ -88,15 +94,17 @@
     def update_an_inquiry(
         self, inquiry_id: str, *, data: UpdateAnInquiryRequestData, key_inflection: typing.Optional[str] = None
     ) -> None:
         _response = httpx.request(
             "PATCH",
             urllib.parse.urljoin(f"{self._environment.value}/", f"inquiries/{inquiry_id}"),
             json=jsonable_encoder({"data": data}),
-            headers=remove_none_from_headers({"Key-Inflection": key_inflection, "Authorization": self.api_key}),
+            headers=remove_none_from_headers(
+                {"Key-Inflection": key_inflection, "Authorization": f"Bearer  {self.api_key}"}
+            ),
             timeout=60,
         )
         if 200 <= _response.status_code < 300:
             return
         if _response.status_code == 404:
             raise NotFoundError(pydantic.parse_obj_as(typing.Any, _response.json()))  # type: ignore
         try:
@@ -107,15 +115,17 @@
 
     def redact_an_inquiry(
         self, inquiry_id: str, *, key_inflection: typing.Optional[str] = None
     ) -> RedactAnInquiryResponse:
         _response = httpx.request(
             "DELETE",
             urllib.parse.urljoin(f"{self._environment.value}/", f"inquiries/{inquiry_id}"),
-            headers=remove_none_from_headers({"Key-Inflection": key_inflection, "Authorization": self.api_key}),
+            headers=remove_none_from_headers(
+                {"Key-Inflection": key_inflection, "Authorization": f"Bearer  {self.api_key}"}
+            ),
             timeout=60,
         )
         if 200 <= _response.status_code < 300:
             return pydantic.parse_obj_as(RedactAnInquiryResponse, _response.json())  # type: ignore
         try:
             _response_json = _response.json()
         except JSONDecodeError:
@@ -134,15 +144,19 @@
         if meta is not OMIT:
             _request["meta"] = meta
         _response = httpx.request(
             "POST",
             urllib.parse.urljoin(f"{self._environment.value}/", f"inquiries/{inquiry_id}/approve"),
             json=jsonable_encoder(_request),
             headers=remove_none_from_headers(
-                {"Key-Inflection": key_inflection, "Idempotency-Key": idempotency_key, "Authorization": self.api_key}
+                {
+                    "Key-Inflection": key_inflection,
+                    "Idempotency-Key": idempotency_key,
+                    "Authorization": f"Bearer  {self.api_key}",
+                }
             ),
             timeout=60,
         )
         if 200 <= _response.status_code < 300:
             return pydantic.parse_obj_as(ApproveAnInquiryResponse, _response.json())  # type: ignore
         if _response.status_code == 409:
             raise ConflictError(pydantic.parse_obj_as(typing.Any, _response.json()))  # type: ignore
@@ -164,15 +178,19 @@
         if meta is not OMIT:
             _request["meta"] = meta
         _response = httpx.request(
             "POST",
             urllib.parse.urljoin(f"{self._environment.value}/", f"inquiries/{inquiry_id}/decline"),
             json=jsonable_encoder(_request),
             headers=remove_none_from_headers(
-                {"Key-Inflection": key_inflection, "Idempotency-Key": idempotency_key, "Authorization": self.api_key}
+                {
+                    "Key-Inflection": key_inflection,
+                    "Idempotency-Key": idempotency_key,
+                    "Authorization": f"Bearer  {self.api_key}",
+                }
             ),
             timeout=60,
         )
         if 200 <= _response.status_code < 300:
             return pydantic.parse_obj_as(DeclineAnInquiryResponse, _response.json())  # type: ignore
         if _response.status_code == 409:
             raise ConflictError(pydantic.parse_obj_as(typing.Any, _response.json()))  # type: ignore
@@ -198,15 +216,17 @@
             params={
                 "page[after]": page_after,
                 "page[before]": page_before,
                 "page[size]": page_size,
                 "filter[account-id]": filter_account_id,
                 "filter[reference-id]": filter_reference_id,
             },
-            headers=remove_none_from_headers({"Key-Inflection": key_inflection, "Authorization": self.api_key}),
+            headers=remove_none_from_headers(
+                {"Key-Inflection": key_inflection, "Authorization": f"Bearer  {self.api_key}"}
+            ),
             timeout=60,
         )
         if 200 <= _response.status_code < 300:
             return pydantic.parse_obj_as(ListAllInquiriesResponse, _response.json())  # type: ignore
         try:
             _response_json = _response.json()
         except JSONDecodeError:
@@ -221,15 +241,19 @@
         idempotency_key: typing.Optional[str] = None,
     ) -> CreateAnInquiryResponse:
         _response = httpx.request(
             "POST",
             urllib.parse.urljoin(f"{self._environment.value}/", "inquiries"),
             json=jsonable_encoder({"data": data}),
             headers=remove_none_from_headers(
-                {"Key-Inflection": key_inflection, "Idempotency-Key": idempotency_key, "Authorization": self.api_key}
+                {
+                    "Key-Inflection": key_inflection,
+                    "Idempotency-Key": idempotency_key,
+                    "Authorization": f"Bearer  {self.api_key}",
+                }
             ),
             timeout=60,
         )
         if 200 <= _response.status_code < 300:
             return pydantic.parse_obj_as(CreateAnInquiryResponse, _response.json())  # type: ignore
         if _response.status_code == 404:
             raise NotFoundError(pydantic.parse_obj_as(typing.Any, _response.json()))  # type: ignore
@@ -251,15 +275,19 @@
         if meta is not OMIT:
             _request["meta"] = meta
         _response = httpx.request(
             "POST",
             urllib.parse.urljoin(f"{self._environment.value}/", f"inquiries/{inquiry_id}/add-tag"),
             json=jsonable_encoder(_request),
             headers=remove_none_from_headers(
-                {"Key-Inflection": key_inflection, "Idempotency-Key": idempotency_key, "Authorization": self.api_key}
+                {
+                    "Key-Inflection": key_inflection,
+                    "Idempotency-Key": idempotency_key,
+                    "Authorization": f"Bearer  {self.api_key}",
+                }
             ),
             timeout=60,
         )
         if 200 <= _response.status_code < 300:
             return
         if _response.status_code == 400:
             raise BadRequestError(pydantic.parse_obj_as(typing.Any, _response.json()))  # type: ignore
@@ -281,15 +309,19 @@
         if meta is not OMIT:
             _request["meta"] = meta
         _response = httpx.request(
             "POST",
             urllib.parse.urljoin(f"{self._environment.value}/", f"inquiries/{inquiry_id}/remove-tag"),
             json=jsonable_encoder(_request),
             headers=remove_none_from_headers(
-                {"Key-Inflection": key_inflection, "Idempotency-Key": idempotency_key, "Authorization": self.api_key}
+                {
+                    "Key-Inflection": key_inflection,
+                    "Idempotency-Key": idempotency_key,
+                    "Authorization": f"Bearer  {self.api_key}",
+                }
             ),
             timeout=60,
         )
         if 200 <= _response.status_code < 300:
             return
         if _response.status_code == 400:
             raise BadRequestError(pydantic.parse_obj_as(typing.Any, _response.json()))  # type: ignore
@@ -311,15 +343,19 @@
         if meta is not OMIT:
             _request["meta"] = meta
         _response = httpx.request(
             "POST",
             urllib.parse.urljoin(f"{self._environment.value}/", f"inquiries/{inquiry_id}/set-tags"),
             json=jsonable_encoder(_request),
             headers=remove_none_from_headers(
-                {"Key-Inflection": key_inflection, "Idempotency-Key": idempotency_key, "Authorization": self.api_key}
+                {
+                    "Key-Inflection": key_inflection,
+                    "Idempotency-Key": idempotency_key,
+                    "Authorization": f"Bearer  {self.api_key}",
+                }
             ),
             timeout=60,
         )
         if 200 <= _response.status_code < 300:
             return
         if _response.status_code == 400:
             raise BadRequestError(pydantic.parse_obj_as(typing.Any, _response.json()))  # type: ignore
@@ -331,15 +367,17 @@
 
     def expire_an_inquiry(
         self, inquiry_id: str, *, key_inflection: typing.Optional[str] = None
     ) -> ExpireAnInquiryResponse:
         _response = httpx.request(
             "POST",
             urllib.parse.urljoin(f"{self._environment.value}/", f"inquiries/{inquiry_id}/expire"),
-            headers=remove_none_from_headers({"Key-Inflection": key_inflection, "Authorization": self.api_key}),
+            headers=remove_none_from_headers(
+                {"Key-Inflection": key_inflection, "Authorization": f"Bearer  {self.api_key}"}
+            ),
             timeout=60,
         )
         if 200 <= _response.status_code < 300:
             return pydantic.parse_obj_as(ExpireAnInquiryResponse, _response.json())  # type: ignore
         try:
             _response_json = _response.json()
         except JSONDecodeError:
@@ -358,15 +396,19 @@
         if meta is not OMIT:
             _request["meta"] = meta
         _response = httpx.request(
             "POST",
             urllib.parse.urljoin(f"{self._environment.value}/", f"inquiries/{inquiry_id}/generate-one-time-link"),
             json=jsonable_encoder(_request),
             headers=remove_none_from_headers(
-                {"Key-Inflection": key_inflection, "Idempotency-Key": idempotency_key, "Authorization": self.api_key}
+                {
+                    "Key-Inflection": key_inflection,
+                    "Idempotency-Key": idempotency_key,
+                    "Authorization": f"Bearer  {self.api_key}",
+                }
             ),
             timeout=60,
         )
         if 200 <= _response.status_code < 300:
             return pydantic.parse_obj_as(GenerateAOneTimeLinkResponse, _response.json())  # type: ignore
         if _response.status_code == 400:
             raise BadRequestError(pydantic.parse_obj_as(typing.Any, _response.json()))  # type: ignore
@@ -393,15 +435,15 @@
             _response = await _client.request(
                 "POST",
                 urllib.parse.urljoin(f"{self._environment.value}/", f"inquiries/{inquiry_id}/resume"),
                 headers=remove_none_from_headers(
                     {
                         "Key-Inflection": key_inflection,
                         "Idempotency-Key": idempotency_key,
-                        "Authorization": self.api_key,
+                        "Authorization": f"Bearer  {self.api_key}",
                     }
                 ),
                 timeout=60,
             )
         if 200 <= _response.status_code < 300:
             return pydantic.parse_obj_as(ResumeAnInquiryResponse, _response.json())  # type: ignore
         if _response.status_code == 404:
@@ -415,15 +457,17 @@
     async def retrieve_an_inquiry(
         self, inquiry_id: str, *, key_inflection: typing.Optional[str] = None
     ) -> RetrieveAnInquiryResponse:
         async with httpx.AsyncClient() as _client:
             _response = await _client.request(
                 "GET",
                 urllib.parse.urljoin(f"{self._environment.value}/", f"inquiries/{inquiry_id}"),
-                headers=remove_none_from_headers({"Key-Inflection": key_inflection, "Authorization": self.api_key}),
+                headers=remove_none_from_headers(
+                    {"Key-Inflection": key_inflection, "Authorization": f"Bearer  {self.api_key}"}
+                ),
                 timeout=60,
             )
         if 200 <= _response.status_code < 300:
             return pydantic.parse_obj_as(RetrieveAnInquiryResponse, _response.json())  # type: ignore
         if _response.status_code == 404:
             raise NotFoundError(pydantic.parse_obj_as(typing.Any, _response.json()))  # type: ignore
         try:
@@ -436,15 +480,17 @@
         self, inquiry_id: str, *, data: UpdateAnInquiryRequestData, key_inflection: typing.Optional[str] = None
     ) -> None:
         async with httpx.AsyncClient() as _client:
             _response = await _client.request(
                 "PATCH",
                 urllib.parse.urljoin(f"{self._environment.value}/", f"inquiries/{inquiry_id}"),
                 json=jsonable_encoder({"data": data}),
-                headers=remove_none_from_headers({"Key-Inflection": key_inflection, "Authorization": self.api_key}),
+                headers=remove_none_from_headers(
+                    {"Key-Inflection": key_inflection, "Authorization": f"Bearer  {self.api_key}"}
+                ),
                 timeout=60,
             )
         if 200 <= _response.status_code < 300:
             return
         if _response.status_code == 404:
             raise NotFoundError(pydantic.parse_obj_as(typing.Any, _response.json()))  # type: ignore
         try:
@@ -456,15 +502,17 @@
     async def redact_an_inquiry(
         self, inquiry_id: str, *, key_inflection: typing.Optional[str] = None
     ) -> RedactAnInquiryResponse:
         async with httpx.AsyncClient() as _client:
             _response = await _client.request(
                 "DELETE",
                 urllib.parse.urljoin(f"{self._environment.value}/", f"inquiries/{inquiry_id}"),
-                headers=remove_none_from_headers({"Key-Inflection": key_inflection, "Authorization": self.api_key}),
+                headers=remove_none_from_headers(
+                    {"Key-Inflection": key_inflection, "Authorization": f"Bearer  {self.api_key}"}
+                ),
                 timeout=60,
             )
         if 200 <= _response.status_code < 300:
             return pydantic.parse_obj_as(RedactAnInquiryResponse, _response.json())  # type: ignore
         try:
             _response_json = _response.json()
         except JSONDecodeError:
@@ -487,15 +535,15 @@
                 "POST",
                 urllib.parse.urljoin(f"{self._environment.value}/", f"inquiries/{inquiry_id}/approve"),
                 json=jsonable_encoder(_request),
                 headers=remove_none_from_headers(
                     {
                         "Key-Inflection": key_inflection,
                         "Idempotency-Key": idempotency_key,
-                        "Authorization": self.api_key,
+                        "Authorization": f"Bearer  {self.api_key}",
                     }
                 ),
                 timeout=60,
             )
         if 200 <= _response.status_code < 300:
             return pydantic.parse_obj_as(ApproveAnInquiryResponse, _response.json())  # type: ignore
         if _response.status_code == 409:
@@ -522,15 +570,15 @@
                 "POST",
                 urllib.parse.urljoin(f"{self._environment.value}/", f"inquiries/{inquiry_id}/decline"),
                 json=jsonable_encoder(_request),
                 headers=remove_none_from_headers(
                     {
                         "Key-Inflection": key_inflection,
                         "Idempotency-Key": idempotency_key,
-                        "Authorization": self.api_key,
+                        "Authorization": f"Bearer  {self.api_key}",
                     }
                 ),
                 timeout=60,
             )
         if 200 <= _response.status_code < 300:
             return pydantic.parse_obj_as(DeclineAnInquiryResponse, _response.json())  # type: ignore
         if _response.status_code == 409:
@@ -558,15 +606,17 @@
                 params={
                     "page[after]": page_after,
                     "page[before]": page_before,
                     "page[size]": page_size,
                     "filter[account-id]": filter_account_id,
                     "filter[reference-id]": filter_reference_id,
                 },
-                headers=remove_none_from_headers({"Key-Inflection": key_inflection, "Authorization": self.api_key}),
+                headers=remove_none_from_headers(
+                    {"Key-Inflection": key_inflection, "Authorization": f"Bearer  {self.api_key}"}
+                ),
                 timeout=60,
             )
         if 200 <= _response.status_code < 300:
             return pydantic.parse_obj_as(ListAllInquiriesResponse, _response.json())  # type: ignore
         try:
             _response_json = _response.json()
         except JSONDecodeError:
@@ -585,15 +635,15 @@
                 "POST",
                 urllib.parse.urljoin(f"{self._environment.value}/", "inquiries"),
                 json=jsonable_encoder({"data": data}),
                 headers=remove_none_from_headers(
                     {
                         "Key-Inflection": key_inflection,
                         "Idempotency-Key": idempotency_key,
-                        "Authorization": self.api_key,
+                        "Authorization": f"Bearer  {self.api_key}",
                     }
                 ),
                 timeout=60,
             )
         if 200 <= _response.status_code < 300:
             return pydantic.parse_obj_as(CreateAnInquiryResponse, _response.json())  # type: ignore
         if _response.status_code == 404:
@@ -620,15 +670,15 @@
                 "POST",
                 urllib.parse.urljoin(f"{self._environment.value}/", f"inquiries/{inquiry_id}/add-tag"),
                 json=jsonable_encoder(_request),
                 headers=remove_none_from_headers(
                     {
                         "Key-Inflection": key_inflection,
                         "Idempotency-Key": idempotency_key,
-                        "Authorization": self.api_key,
+                        "Authorization": f"Bearer  {self.api_key}",
                     }
                 ),
                 timeout=60,
             )
         if 200 <= _response.status_code < 300:
             return
         if _response.status_code == 400:
@@ -655,15 +705,15 @@
                 "POST",
                 urllib.parse.urljoin(f"{self._environment.value}/", f"inquiries/{inquiry_id}/remove-tag"),
                 json=jsonable_encoder(_request),
                 headers=remove_none_from_headers(
                     {
                         "Key-Inflection": key_inflection,
                         "Idempotency-Key": idempotency_key,
-                        "Authorization": self.api_key,
+                        "Authorization": f"Bearer  {self.api_key}",
                     }
                 ),
                 timeout=60,
             )
         if 200 <= _response.status_code < 300:
             return
         if _response.status_code == 400:
@@ -690,15 +740,15 @@
                 "POST",
                 urllib.parse.urljoin(f"{self._environment.value}/", f"inquiries/{inquiry_id}/set-tags"),
                 json=jsonable_encoder(_request),
                 headers=remove_none_from_headers(
                     {
                         "Key-Inflection": key_inflection,
                         "Idempotency-Key": idempotency_key,
-                        "Authorization": self.api_key,
+                        "Authorization": f"Bearer  {self.api_key}",
                     }
                 ),
                 timeout=60,
             )
         if 200 <= _response.status_code < 300:
             return
         if _response.status_code == 400:
@@ -712,15 +762,17 @@
     async def expire_an_inquiry(
         self, inquiry_id: str, *, key_inflection: typing.Optional[str] = None
     ) -> ExpireAnInquiryResponse:
         async with httpx.AsyncClient() as _client:
             _response = await _client.request(
                 "POST",
                 urllib.parse.urljoin(f"{self._environment.value}/", f"inquiries/{inquiry_id}/expire"),
-                headers=remove_none_from_headers({"Key-Inflection": key_inflection, "Authorization": self.api_key}),
+                headers=remove_none_from_headers(
+                    {"Key-Inflection": key_inflection, "Authorization": f"Bearer  {self.api_key}"}
+                ),
                 timeout=60,
             )
         if 200 <= _response.status_code < 300:
             return pydantic.parse_obj_as(ExpireAnInquiryResponse, _response.json())  # type: ignore
         try:
             _response_json = _response.json()
         except JSONDecodeError:
@@ -743,15 +795,15 @@
                 "POST",
                 urllib.parse.urljoin(f"{self._environment.value}/", f"inquiries/{inquiry_id}/generate-one-time-link"),
                 json=jsonable_encoder(_request),
                 headers=remove_none_from_headers(
                     {
                         "Key-Inflection": key_inflection,
                         "Idempotency-Key": idempotency_key,
-                        "Authorization": self.api_key,
+                        "Authorization": f"Bearer  {self.api_key}",
                     }
                 ),
                 timeout=60,
             )
         if 200 <= _response.status_code < 300:
             return pydantic.parse_obj_as(GenerateAOneTimeLinkResponse, _response.json())  # type: ignore
         if _response.status_code == 400:
```

### Comparing `fern_persona-0.0.2/src/persona/resources/list_items/client.py` & `fern_persona-0.0.3/src/persona/resources/list_items/client.py`

 * *Files 3% similar despite different names*

```diff
@@ -50,15 +50,19 @@
         if data is not OMIT:
             _request["data"] = data
         _response = httpx.request(
             "POST",
             urllib.parse.urljoin(f"{self._environment.value}/", "list-item/countries"),
             json=jsonable_encoder(_request),
             headers=remove_none_from_headers(
-                {"key-inflection": key_inflection, "idempotence-key": idempotence_key, "Authorization": self.api_key}
+                {
+                    "key-inflection": key_inflection,
+                    "idempotence-key": idempotence_key,
+                    "Authorization": f"Bearer  {self.api_key}",
+                }
             ),
             timeout=60,
         )
         if 200 <= _response.status_code < 300:
             return
         if _response.status_code == 400:
             raise BadRequestError(pydantic.parse_obj_as(typing.Any, _response.json()))  # type: ignore
@@ -79,15 +83,19 @@
         if data is not OMIT:
             _request["data"] = data
         _response = httpx.request(
             "POST",
             urllib.parse.urljoin(f"{self._environment.value}/", "list-item/email-addresses"),
             json=jsonable_encoder(_request),
             headers=remove_none_from_headers(
-                {"key-inflection": key_inflection, "idempotence-key": idempotence_key, "Authorization": self.api_key}
+                {
+                    "key-inflection": key_inflection,
+                    "idempotence-key": idempotence_key,
+                    "Authorization": f"Bearer  {self.api_key}",
+                }
             ),
             timeout=60,
         )
         if 200 <= _response.status_code < 300:
             return pydantic.parse_obj_as(CreateAnEmailAddressListItemResponse, _response.json())  # type: ignore
         if _response.status_code == 400:
             raise BadRequestError(pydantic.parse_obj_as(typing.Any, _response.json()))  # type: ignore
@@ -108,15 +116,19 @@
         if data is not OMIT:
             _request["data"] = data
         _response = httpx.request(
             "POST",
             urllib.parse.urljoin(f"{self._environment.value}/", "list-item/geolocations"),
             json=jsonable_encoder(_request),
             headers=remove_none_from_headers(
-                {"key-inflection": key_inflection, "idempotence-key": idempotence_key, "Authorization": self.api_key}
+                {
+                    "key-inflection": key_inflection,
+                    "idempotence-key": idempotence_key,
+                    "Authorization": f"Bearer  {self.api_key}",
+                }
             ),
             timeout=60,
         )
         if 200 <= _response.status_code < 300:
             return pydantic.parse_obj_as(CreateAGeolocationListItemResponse, _response.json())  # type: ignore
         if _response.status_code == 400:
             raise BadRequestError(pydantic.parse_obj_as(typing.Any, _response.json()))  # type: ignore
@@ -137,15 +149,19 @@
         if data is not OMIT:
             _request["data"] = data
         _response = httpx.request(
             "POST",
             urllib.parse.urljoin(f"{self._environment.value}/", "list-item/ip-addresses"),
             json=jsonable_encoder(_request),
             headers=remove_none_from_headers(
-                {"key-inflection": key_inflection, "idempotence-key": idempotence_key, "Authorization": self.api_key}
+                {
+                    "key-inflection": key_inflection,
+                    "idempotence-key": idempotence_key,
+                    "Authorization": f"Bearer  {self.api_key}",
+                }
             ),
             timeout=60,
         )
         if 200 <= _response.status_code < 300:
             return
         if _response.status_code == 400:
             raise BadRequestError(pydantic.parse_obj_as(typing.Any, _response.json()))  # type: ignore
@@ -166,15 +182,19 @@
         if data is not OMIT:
             _request["data"] = data
         _response = httpx.request(
             "POST",
             urllib.parse.urljoin(f"{self._environment.value}/", "list-item/government-id-numbers"),
             json=jsonable_encoder(_request),
             headers=remove_none_from_headers(
-                {"key-inflection": key_inflection, "idempotence-key": idempotence_key, "Authorization": self.api_key}
+                {
+                    "key-inflection": key_inflection,
+                    "idempotence-key": idempotence_key,
+                    "Authorization": f"Bearer  {self.api_key}",
+                }
             ),
             timeout=60,
         )
         if 200 <= _response.status_code < 300:
             return pydantic.parse_obj_as(CreateAGovernmentIdNumberListItemResponse, _response.json())  # type: ignore
         if _response.status_code == 400:
             raise BadRequestError(pydantic.parse_obj_as(typing.Any, _response.json()))  # type: ignore
@@ -195,15 +215,19 @@
         if data is not OMIT:
             _request["data"] = data
         _response = httpx.request(
             "POST",
             urllib.parse.urljoin(f"{self._environment.value}/", "list-item/names"),
             json=jsonable_encoder(_request),
             headers=remove_none_from_headers(
-                {"key-inflection": key_inflection, "idempotence-key": idempotence_key, "Authorization": self.api_key}
+                {
+                    "key-inflection": key_inflection,
+                    "idempotence-key": idempotence_key,
+                    "Authorization": f"Bearer  {self.api_key}",
+                }
             ),
             timeout=60,
         )
         if 200 <= _response.status_code < 300:
             return pydantic.parse_obj_as(CreateANameListItemResponse, _response.json())  # type: ignore
         if _response.status_code == 400:
             raise BadRequestError(pydantic.parse_obj_as(typing.Any, _response.json()))  # type: ignore
@@ -224,15 +248,19 @@
         if data is not OMIT:
             _request["data"] = data
         _response = httpx.request(
             "POST",
             urllib.parse.urljoin(f"{self._environment.value}/", "list-item/phone-numbers"),
             json=jsonable_encoder(_request),
             headers=remove_none_from_headers(
-                {"key-inflection": key_inflection, "idempotence-key": idempotence_key, "Authorization": self.api_key}
+                {
+                    "key-inflection": key_inflection,
+                    "idempotence-key": idempotence_key,
+                    "Authorization": f"Bearer  {self.api_key}",
+                }
             ),
             timeout=60,
         )
         if 200 <= _response.status_code < 300:
             return
         if _response.status_code == 400:
             raise BadRequestError(pydantic.parse_obj_as(typing.Any, _response.json()))  # type: ignore
@@ -249,15 +277,19 @@
         key_inflection: typing.Optional[str] = None,
         idempotence_key: typing.Optional[str] = None,
     ) -> ArchiveABrowserFingerprintListItemResponse:
         _response = httpx.request(
             "DELETE",
             urllib.parse.urljoin(f"{self._environment.value}/", f"list-item/browser-fingerprints/{list_item_id}"),
             headers=remove_none_from_headers(
-                {"key-inflection": key_inflection, "idempotence-key": idempotence_key, "Authorization": self.api_key}
+                {
+                    "key-inflection": key_inflection,
+                    "idempotence-key": idempotence_key,
+                    "Authorization": f"Bearer  {self.api_key}",
+                }
             ),
             timeout=60,
         )
         if 200 <= _response.status_code < 300:
             return pydantic.parse_obj_as(ArchiveABrowserFingerprintListItemResponse, _response.json())  # type: ignore
         if _response.status_code == 400:
             raise BadRequestError(pydantic.parse_obj_as(typing.Any, _response.json()))  # type: ignore
@@ -274,15 +306,19 @@
         key_inflection: typing.Optional[str] = None,
         idempotence_key: typing.Optional[str] = None,
     ) -> None:
         _response = httpx.request(
             "DELETE",
             urllib.parse.urljoin(f"{self._environment.value}/", f"list-item/countries/{list_item_id}"),
             headers=remove_none_from_headers(
-                {"key-inflection": key_inflection, "idempotence-key": idempotence_key, "Authorization": self.api_key}
+                {
+                    "key-inflection": key_inflection,
+                    "idempotence-key": idempotence_key,
+                    "Authorization": f"Bearer  {self.api_key}",
+                }
             ),
             timeout=60,
         )
         if 200 <= _response.status_code < 300:
             return
         if _response.status_code == 400:
             raise BadRequestError(pydantic.parse_obj_as(typing.Any, _response.json()))  # type: ignore
@@ -299,15 +335,19 @@
         key_inflection: typing.Optional[str] = None,
         idempotence_key: typing.Optional[str] = None,
     ) -> ArchiveAnEmailAddressListItemResponse:
         _response = httpx.request(
             "DELETE",
             urllib.parse.urljoin(f"{self._environment.value}/", f"list-item/email-addresses/{list_item_id}"),
             headers=remove_none_from_headers(
-                {"key-inflection": key_inflection, "idempotence-key": idempotence_key, "Authorization": self.api_key}
+                {
+                    "key-inflection": key_inflection,
+                    "idempotence-key": idempotence_key,
+                    "Authorization": f"Bearer  {self.api_key}",
+                }
             ),
             timeout=60,
         )
         if 200 <= _response.status_code < 300:
             return pydantic.parse_obj_as(ArchiveAnEmailAddressListItemResponse, _response.json())  # type: ignore
         if _response.status_code == 400:
             raise BadRequestError(pydantic.parse_obj_as(typing.Any, _response.json()))  # type: ignore
@@ -324,15 +364,19 @@
         key_inflection: typing.Optional[str] = None,
         idempotence_key: typing.Optional[str] = None,
     ) -> ArchiveAGeolocationListItemResponse:
         _response = httpx.request(
             "DELETE",
             urllib.parse.urljoin(f"{self._environment.value}/", f"list-item/geolocations/{list_item_id}"),
             headers=remove_none_from_headers(
-                {"key-inflection": key_inflection, "idempotence-key": idempotence_key, "Authorization": self.api_key}
+                {
+                    "key-inflection": key_inflection,
+                    "idempotence-key": idempotence_key,
+                    "Authorization": f"Bearer  {self.api_key}",
+                }
             ),
             timeout=60,
         )
         if 200 <= _response.status_code < 300:
             return pydantic.parse_obj_as(ArchiveAGeolocationListItemResponse, _response.json())  # type: ignore
         if _response.status_code == 400:
             raise BadRequestError(pydantic.parse_obj_as(typing.Any, _response.json()))  # type: ignore
@@ -349,15 +393,19 @@
         key_inflection: typing.Optional[str] = None,
         idempotence_key: typing.Optional[str] = None,
     ) -> ArchiveAGovernmentIdNumberListItemResponse:
         _response = httpx.request(
             "DELETE",
             urllib.parse.urljoin(f"{self._environment.value}/", f"list-item/government-id-numbers/{list_item_id}"),
             headers=remove_none_from_headers(
-                {"key-inflection": key_inflection, "idempotence-key": idempotence_key, "Authorization": self.api_key}
+                {
+                    "key-inflection": key_inflection,
+                    "idempotence-key": idempotence_key,
+                    "Authorization": f"Bearer  {self.api_key}",
+                }
             ),
             timeout=60,
         )
         if 200 <= _response.status_code < 300:
             return pydantic.parse_obj_as(ArchiveAGovernmentIdNumberListItemResponse, _response.json())  # type: ignore
         if _response.status_code == 400:
             raise BadRequestError(pydantic.parse_obj_as(typing.Any, _response.json()))  # type: ignore
@@ -374,15 +422,19 @@
         key_inflection: typing.Optional[str] = None,
         idempotence_key: typing.Optional[str] = None,
     ) -> None:
         _response = httpx.request(
             "DELETE",
             urllib.parse.urljoin(f"{self._environment.value}/", f"list-item/ip-addresses/{list_item_id}"),
             headers=remove_none_from_headers(
-                {"key-inflection": key_inflection, "idempotence-key": idempotence_key, "Authorization": self.api_key}
+                {
+                    "key-inflection": key_inflection,
+                    "idempotence-key": idempotence_key,
+                    "Authorization": f"Bearer  {self.api_key}",
+                }
             ),
             timeout=60,
         )
         if 200 <= _response.status_code < 300:
             return
         if _response.status_code == 400:
             raise BadRequestError(pydantic.parse_obj_as(typing.Any, _response.json()))  # type: ignore
@@ -399,15 +451,19 @@
         key_inflection: typing.Optional[str] = None,
         idempotence_key: typing.Optional[str] = None,
     ) -> ArchiveANameListItemResponse:
         _response = httpx.request(
             "DELETE",
             urllib.parse.urljoin(f"{self._environment.value}/", f"list-item/names/{list_item_id}"),
             headers=remove_none_from_headers(
-                {"key-inflection": key_inflection, "idempotence-key": idempotence_key, "Authorization": self.api_key}
+                {
+                    "key-inflection": key_inflection,
+                    "idempotence-key": idempotence_key,
+                    "Authorization": f"Bearer  {self.api_key}",
+                }
             ),
             timeout=60,
         )
         if 200 <= _response.status_code < 300:
             return pydantic.parse_obj_as(ArchiveANameListItemResponse, _response.json())  # type: ignore
         if _response.status_code == 400:
             raise BadRequestError(pydantic.parse_obj_as(typing.Any, _response.json()))  # type: ignore
@@ -424,15 +480,19 @@
         key_inflection: typing.Optional[str] = None,
         idempotence_key: typing.Optional[str] = None,
     ) -> None:
         _response = httpx.request(
             "DELETE",
             urllib.parse.urljoin(f"{self._environment.value}/", f"list-item/phone-numbers/{list_item_id}"),
             headers=remove_none_from_headers(
-                {"key-inflection": key_inflection, "idempotence-key": idempotence_key, "Authorization": self.api_key}
+                {
+                    "key-inflection": key_inflection,
+                    "idempotence-key": idempotence_key,
+                    "Authorization": f"Bearer  {self.api_key}",
+                }
             ),
             timeout=60,
         )
         if 200 <= _response.status_code < 300:
             return
         if _response.status_code == 400:
             raise BadRequestError(pydantic.parse_obj_as(typing.Any, _response.json()))  # type: ignore
@@ -453,15 +513,19 @@
         if data is not OMIT:
             _request["data"] = data
         _response = httpx.request(
             "POST",
             urllib.parse.urljoin(f"{self._environment.value}/", "list-item/faces"),
             json=jsonable_encoder(_request),
             headers=remove_none_from_headers(
-                {"key-inflection": key_inflection, "idempotence-key": idempotence_key, "Authorization": self.api_key}
+                {
+                    "key-inflection": key_inflection,
+                    "idempotence-key": idempotence_key,
+                    "Authorization": f"Bearer  {self.api_key}",
+                }
             ),
             timeout=60,
         )
         if 200 <= _response.status_code < 300:
             return
         if _response.status_code == 400:
             raise BadRequestError(pydantic.parse_obj_as(typing.Any, _response.json()))  # type: ignore
@@ -478,15 +542,19 @@
         key_inflection: typing.Optional[str] = None,
         idempotence_key: typing.Optional[str] = None,
     ) -> None:
         _response = httpx.request(
             "DELETE",
             urllib.parse.urljoin(f"{self._environment.value}/", f"list-item/faces/{list_item_id}"),
             headers=remove_none_from_headers(
-                {"key-inflection": key_inflection, "idempotence-key": idempotence_key, "Authorization": self.api_key}
+                {
+                    "key-inflection": key_inflection,
+                    "idempotence-key": idempotence_key,
+                    "Authorization": f"Bearer  {self.api_key}",
+                }
             ),
             timeout=60,
         )
         if 200 <= _response.status_code < 300:
             return
         if _response.status_code == 400:
             raise BadRequestError(pydantic.parse_obj_as(typing.Any, _response.json()))  # type: ignore
@@ -517,15 +585,15 @@
                 "POST",
                 urllib.parse.urljoin(f"{self._environment.value}/", "list-item/countries"),
                 json=jsonable_encoder(_request),
                 headers=remove_none_from_headers(
                     {
                         "key-inflection": key_inflection,
                         "idempotence-key": idempotence_key,
-                        "Authorization": self.api_key,
+                        "Authorization": f"Bearer  {self.api_key}",
                     }
                 ),
                 timeout=60,
             )
         if 200 <= _response.status_code < 300:
             return
         if _response.status_code == 400:
@@ -551,15 +619,15 @@
                 "POST",
                 urllib.parse.urljoin(f"{self._environment.value}/", "list-item/email-addresses"),
                 json=jsonable_encoder(_request),
                 headers=remove_none_from_headers(
                     {
                         "key-inflection": key_inflection,
                         "idempotence-key": idempotence_key,
-                        "Authorization": self.api_key,
+                        "Authorization": f"Bearer  {self.api_key}",
                     }
                 ),
                 timeout=60,
             )
         if 200 <= _response.status_code < 300:
             return pydantic.parse_obj_as(CreateAnEmailAddressListItemResponse, _response.json())  # type: ignore
         if _response.status_code == 400:
@@ -585,15 +653,15 @@
                 "POST",
                 urllib.parse.urljoin(f"{self._environment.value}/", "list-item/geolocations"),
                 json=jsonable_encoder(_request),
                 headers=remove_none_from_headers(
                     {
                         "key-inflection": key_inflection,
                         "idempotence-key": idempotence_key,
-                        "Authorization": self.api_key,
+                        "Authorization": f"Bearer  {self.api_key}",
                     }
                 ),
                 timeout=60,
             )
         if 200 <= _response.status_code < 300:
             return pydantic.parse_obj_as(CreateAGeolocationListItemResponse, _response.json())  # type: ignore
         if _response.status_code == 400:
@@ -619,15 +687,15 @@
                 "POST",
                 urllib.parse.urljoin(f"{self._environment.value}/", "list-item/ip-addresses"),
                 json=jsonable_encoder(_request),
                 headers=remove_none_from_headers(
                     {
                         "key-inflection": key_inflection,
                         "idempotence-key": idempotence_key,
-                        "Authorization": self.api_key,
+                        "Authorization": f"Bearer  {self.api_key}",
                     }
                 ),
                 timeout=60,
             )
         if 200 <= _response.status_code < 300:
             return
         if _response.status_code == 400:
@@ -653,15 +721,15 @@
                 "POST",
                 urllib.parse.urljoin(f"{self._environment.value}/", "list-item/government-id-numbers"),
                 json=jsonable_encoder(_request),
                 headers=remove_none_from_headers(
                     {
                         "key-inflection": key_inflection,
                         "idempotence-key": idempotence_key,
-                        "Authorization": self.api_key,
+                        "Authorization": f"Bearer  {self.api_key}",
                     }
                 ),
                 timeout=60,
             )
         if 200 <= _response.status_code < 300:
             return pydantic.parse_obj_as(CreateAGovernmentIdNumberListItemResponse, _response.json())  # type: ignore
         if _response.status_code == 400:
@@ -687,15 +755,15 @@
                 "POST",
                 urllib.parse.urljoin(f"{self._environment.value}/", "list-item/names"),
                 json=jsonable_encoder(_request),
                 headers=remove_none_from_headers(
                     {
                         "key-inflection": key_inflection,
                         "idempotence-key": idempotence_key,
-                        "Authorization": self.api_key,
+                        "Authorization": f"Bearer  {self.api_key}",
                     }
                 ),
                 timeout=60,
             )
         if 200 <= _response.status_code < 300:
             return pydantic.parse_obj_as(CreateANameListItemResponse, _response.json())  # type: ignore
         if _response.status_code == 400:
@@ -721,15 +789,15 @@
                 "POST",
                 urllib.parse.urljoin(f"{self._environment.value}/", "list-item/phone-numbers"),
                 json=jsonable_encoder(_request),
                 headers=remove_none_from_headers(
                     {
                         "key-inflection": key_inflection,
                         "idempotence-key": idempotence_key,
-                        "Authorization": self.api_key,
+                        "Authorization": f"Bearer  {self.api_key}",
                     }
                 ),
                 timeout=60,
             )
         if 200 <= _response.status_code < 300:
             return
         if _response.status_code == 400:
@@ -751,15 +819,15 @@
             _response = await _client.request(
                 "DELETE",
                 urllib.parse.urljoin(f"{self._environment.value}/", f"list-item/browser-fingerprints/{list_item_id}"),
                 headers=remove_none_from_headers(
                     {
                         "key-inflection": key_inflection,
                         "idempotence-key": idempotence_key,
-                        "Authorization": self.api_key,
+                        "Authorization": f"Bearer  {self.api_key}",
                     }
                 ),
                 timeout=60,
             )
         if 200 <= _response.status_code < 300:
             return pydantic.parse_obj_as(ArchiveABrowserFingerprintListItemResponse, _response.json())  # type: ignore
         if _response.status_code == 400:
@@ -781,15 +849,15 @@
             _response = await _client.request(
                 "DELETE",
                 urllib.parse.urljoin(f"{self._environment.value}/", f"list-item/countries/{list_item_id}"),
                 headers=remove_none_from_headers(
                     {
                         "key-inflection": key_inflection,
                         "idempotence-key": idempotence_key,
-                        "Authorization": self.api_key,
+                        "Authorization": f"Bearer  {self.api_key}",
                     }
                 ),
                 timeout=60,
             )
         if 200 <= _response.status_code < 300:
             return
         if _response.status_code == 400:
@@ -811,15 +879,15 @@
             _response = await _client.request(
                 "DELETE",
                 urllib.parse.urljoin(f"{self._environment.value}/", f"list-item/email-addresses/{list_item_id}"),
                 headers=remove_none_from_headers(
                     {
                         "key-inflection": key_inflection,
                         "idempotence-key": idempotence_key,
-                        "Authorization": self.api_key,
+                        "Authorization": f"Bearer  {self.api_key}",
                     }
                 ),
                 timeout=60,
             )
         if 200 <= _response.status_code < 300:
             return pydantic.parse_obj_as(ArchiveAnEmailAddressListItemResponse, _response.json())  # type: ignore
         if _response.status_code == 400:
@@ -841,15 +909,15 @@
             _response = await _client.request(
                 "DELETE",
                 urllib.parse.urljoin(f"{self._environment.value}/", f"list-item/geolocations/{list_item_id}"),
                 headers=remove_none_from_headers(
                     {
                         "key-inflection": key_inflection,
                         "idempotence-key": idempotence_key,
-                        "Authorization": self.api_key,
+                        "Authorization": f"Bearer  {self.api_key}",
                     }
                 ),
                 timeout=60,
             )
         if 200 <= _response.status_code < 300:
             return pydantic.parse_obj_as(ArchiveAGeolocationListItemResponse, _response.json())  # type: ignore
         if _response.status_code == 400:
@@ -871,15 +939,15 @@
             _response = await _client.request(
                 "DELETE",
                 urllib.parse.urljoin(f"{self._environment.value}/", f"list-item/government-id-numbers/{list_item_id}"),
                 headers=remove_none_from_headers(
                     {
                         "key-inflection": key_inflection,
                         "idempotence-key": idempotence_key,
-                        "Authorization": self.api_key,
+                        "Authorization": f"Bearer  {self.api_key}",
                     }
                 ),
                 timeout=60,
             )
         if 200 <= _response.status_code < 300:
             return pydantic.parse_obj_as(ArchiveAGovernmentIdNumberListItemResponse, _response.json())  # type: ignore
         if _response.status_code == 400:
@@ -901,15 +969,15 @@
             _response = await _client.request(
                 "DELETE",
                 urllib.parse.urljoin(f"{self._environment.value}/", f"list-item/ip-addresses/{list_item_id}"),
                 headers=remove_none_from_headers(
                     {
                         "key-inflection": key_inflection,
                         "idempotence-key": idempotence_key,
-                        "Authorization": self.api_key,
+                        "Authorization": f"Bearer  {self.api_key}",
                     }
                 ),
                 timeout=60,
             )
         if 200 <= _response.status_code < 300:
             return
         if _response.status_code == 400:
@@ -931,15 +999,15 @@
             _response = await _client.request(
                 "DELETE",
                 urllib.parse.urljoin(f"{self._environment.value}/", f"list-item/names/{list_item_id}"),
                 headers=remove_none_from_headers(
                     {
                         "key-inflection": key_inflection,
                         "idempotence-key": idempotence_key,
-                        "Authorization": self.api_key,
+                        "Authorization": f"Bearer  {self.api_key}",
                     }
                 ),
                 timeout=60,
             )
         if 200 <= _response.status_code < 300:
             return pydantic.parse_obj_as(ArchiveANameListItemResponse, _response.json())  # type: ignore
         if _response.status_code == 400:
@@ -961,15 +1029,15 @@
             _response = await _client.request(
                 "DELETE",
                 urllib.parse.urljoin(f"{self._environment.value}/", f"list-item/phone-numbers/{list_item_id}"),
                 headers=remove_none_from_headers(
                     {
                         "key-inflection": key_inflection,
                         "idempotence-key": idempotence_key,
-                        "Authorization": self.api_key,
+                        "Authorization": f"Bearer  {self.api_key}",
                     }
                 ),
                 timeout=60,
             )
         if 200 <= _response.status_code < 300:
             return
         if _response.status_code == 400:
@@ -995,15 +1063,15 @@
                 "POST",
                 urllib.parse.urljoin(f"{self._environment.value}/", "list-item/faces"),
                 json=jsonable_encoder(_request),
                 headers=remove_none_from_headers(
                     {
                         "key-inflection": key_inflection,
                         "idempotence-key": idempotence_key,
-                        "Authorization": self.api_key,
+                        "Authorization": f"Bearer  {self.api_key}",
                     }
                 ),
                 timeout=60,
             )
         if 200 <= _response.status_code < 300:
             return
         if _response.status_code == 400:
@@ -1025,15 +1093,15 @@
             _response = await _client.request(
                 "DELETE",
                 urllib.parse.urljoin(f"{self._environment.value}/", f"list-item/faces/{list_item_id}"),
                 headers=remove_none_from_headers(
                     {
                         "key-inflection": key_inflection,
                         "idempotence-key": idempotence_key,
-                        "Authorization": self.api_key,
+                        "Authorization": f"Bearer  {self.api_key}",
                     }
                 ),
                 timeout=60,
             )
         if 200 <= _response.status_code < 300:
             return
         if _response.status_code == 400:
```

### Comparing `fern_persona-0.0.2/src/persona/resources/lists/client.py` & `fern_persona-0.0.3/src/persona/resources/lists/client.py`

 * *Files 6% similar despite different names*

```diff
@@ -59,15 +59,17 @@
             urllib.parse.urljoin(f"{self._environment.value}/", "lists"),
             params={
                 "page[before]": page_before,
                 "page[after]": page_after,
                 "page[size]": page_size,
                 "filter[status]": filter_status,
             },
-            headers=remove_none_from_headers({"key-inflection": key_inflection, "Authorization": self.api_key}),
+            headers=remove_none_from_headers(
+                {"key-inflection": key_inflection, "Authorization": f"Bearer  {self.api_key}"}
+            ),
             timeout=60,
         )
         if 200 <= _response.status_code < 300:
             return pydantic.parse_obj_as(ListAllListsResponse, _response.json())  # type: ignore
         if _response.status_code == 400:
             raise BadRequestError(pydantic.parse_obj_as(typing.Any, _response.json()))  # type: ignore
         try:
@@ -76,15 +78,17 @@
             raise ApiError(status_code=_response.status_code, body=_response.text)
         raise ApiError(status_code=_response.status_code, body=_response_json)
 
     def retrieve_a_list(self, list_id: str, *, key_inflection: typing.Optional[str] = None) -> RetrieveAListResponse:
         _response = httpx.request(
             "GET",
             urllib.parse.urljoin(f"{self._environment.value}/", f"lists/{list_id}"),
-            headers=remove_none_from_headers({"key-inflection": key_inflection, "Authorization": self.api_key}),
+            headers=remove_none_from_headers(
+                {"key-inflection": key_inflection, "Authorization": f"Bearer  {self.api_key}"}
+            ),
             timeout=60,
         )
         if 200 <= _response.status_code < 300:
             return pydantic.parse_obj_as(RetrieveAListResponse, _response.json())  # type: ignore
         if _response.status_code == 400:
             raise BadRequestError(pydantic.parse_obj_as(typing.Any, _response.json()))  # type: ignore
         try:
@@ -96,15 +100,19 @@
     def archive_a_list(
         self, list_id: str, *, key_inflection: typing.Optional[str] = None, idempotency_key: typing.Optional[str] = None
     ) -> ArchiveAListResponse:
         _response = httpx.request(
             "DELETE",
             urllib.parse.urljoin(f"{self._environment.value}/", f"lists/{list_id}"),
             headers=remove_none_from_headers(
-                {"key-inflection": key_inflection, "idempotency-key": idempotency_key, "Authorization": self.api_key}
+                {
+                    "key-inflection": key_inflection,
+                    "idempotency-key": idempotency_key,
+                    "Authorization": f"Bearer  {self.api_key}",
+                }
             ),
             timeout=60,
         )
         if 200 <= _response.status_code < 300:
             return pydantic.parse_obj_as(ArchiveAListResponse, _response.json())  # type: ignore
         if _response.status_code == 400:
             raise BadRequestError(pydantic.parse_obj_as(typing.Any, _response.json()))  # type: ignore
@@ -125,15 +133,19 @@
         if data is not OMIT:
             _request["data"] = data
         _response = httpx.request(
             "POST",
             urllib.parse.urljoin(f"{self._environment.value}/", "list/browser-fingerprints"),
             json=jsonable_encoder(_request),
             headers=remove_none_from_headers(
-                {"key-inflection": key_inflection, "idempotency-key": idempotency_key, "Authorization": self.api_key}
+                {
+                    "key-inflection": key_inflection,
+                    "idempotency-key": idempotency_key,
+                    "Authorization": f"Bearer  {self.api_key}",
+                }
             ),
             timeout=60,
         )
         if 200 <= _response.status_code < 300:
             return pydantic.parse_obj_as(CreateABrowserFingerprintListResponse, _response.json())  # type: ignore
         if _response.status_code == 400:
             raise BadRequestError(pydantic.parse_obj_as(typing.Any, _response.json()))  # type: ignore
@@ -154,15 +166,19 @@
         if data is not OMIT:
             _request["data"] = data
         _response = httpx.request(
             "POST",
             urllib.parse.urljoin(f"{self._environment.value}/", "list/countries"),
             json=jsonable_encoder(_request),
             headers=remove_none_from_headers(
-                {"key-inflection": key_inflection, "idempotency-key": idempotency_key, "Authorization": self.api_key}
+                {
+                    "key-inflection": key_inflection,
+                    "idempotency-key": idempotency_key,
+                    "Authorization": f"Bearer  {self.api_key}",
+                }
             ),
             timeout=60,
         )
         if 200 <= _response.status_code < 300:
             return pydantic.parse_obj_as(CreateACountryListResponse, _response.json())  # type: ignore
         if _response.status_code == 400:
             raise BadRequestError(pydantic.parse_obj_as(typing.Any, _response.json()))  # type: ignore
@@ -183,15 +199,19 @@
         if data is not OMIT:
             _request["data"] = data
         _response = httpx.request(
             "POST",
             urllib.parse.urljoin(f"{self._environment.value}/", "list/email-addresses"),
             json=jsonable_encoder(_request),
             headers=remove_none_from_headers(
-                {"key-inflection": key_inflection, "idempotency-key": idempotency_key, "Authorization": self.api_key}
+                {
+                    "key-inflection": key_inflection,
+                    "idempotency-key": idempotency_key,
+                    "Authorization": f"Bearer  {self.api_key}",
+                }
             ),
             timeout=60,
         )
         if 200 <= _response.status_code < 300:
             return pydantic.parse_obj_as(CreateAnEmailAddressListResponse, _response.json())  # type: ignore
         if _response.status_code == 400:
             raise BadRequestError(pydantic.parse_obj_as(typing.Any, _response.json()))  # type: ignore
@@ -212,15 +232,19 @@
         if data is not OMIT:
             _request["data"] = data
         _response = httpx.request(
             "POST",
             urllib.parse.urljoin(f"{self._environment.value}/", "list/geolocations"),
             json=jsonable_encoder(_request),
             headers=remove_none_from_headers(
-                {"key-inflection": key_inflection, "idempotency-key": idempotency_key, "Authorization": self.api_key}
+                {
+                    "key-inflection": key_inflection,
+                    "idempotency-key": idempotency_key,
+                    "Authorization": f"Bearer  {self.api_key}",
+                }
             ),
             timeout=60,
         )
         if 200 <= _response.status_code < 300:
             return pydantic.parse_obj_as(CreateAGeolocationListResponse, _response.json())  # type: ignore
         if _response.status_code == 400:
             raise BadRequestError(pydantic.parse_obj_as(typing.Any, _response.json()))  # type: ignore
@@ -241,15 +265,19 @@
         if data is not OMIT:
             _request["data"] = data
         _response = httpx.request(
             "POST",
             urllib.parse.urljoin(f"{self._environment.value}/", "list/government-id-numbers"),
             json=jsonable_encoder(_request),
             headers=remove_none_from_headers(
-                {"key-inflection": key_inflection, "idempotency-key": idempotency_key, "Authorization": self.api_key}
+                {
+                    "key-inflection": key_inflection,
+                    "idempotency-key": idempotency_key,
+                    "Authorization": f"Bearer  {self.api_key}",
+                }
             ),
             timeout=60,
         )
         if 200 <= _response.status_code < 300:
             return pydantic.parse_obj_as(CreateAGovernmentIdNumberListResponse, _response.json())  # type: ignore
         if _response.status_code == 400:
             raise BadRequestError(pydantic.parse_obj_as(typing.Any, _response.json()))  # type: ignore
@@ -270,15 +298,19 @@
         if data is not OMIT:
             _request["data"] = data
         _response = httpx.request(
             "POST",
             urllib.parse.urljoin(f"{self._environment.value}/", "list/ip-addresses"),
             json=jsonable_encoder(_request),
             headers=remove_none_from_headers(
-                {"key-inflection": key_inflection, "idempotency-key": idempotency_key, "Authorization": self.api_key}
+                {
+                    "key-inflection": key_inflection,
+                    "idempotency-key": idempotency_key,
+                    "Authorization": f"Bearer  {self.api_key}",
+                }
             ),
             timeout=60,
         )
         if 200 <= _response.status_code < 300:
             return pydantic.parse_obj_as(CreateAnIpAddressListResponse, _response.json())  # type: ignore
         if _response.status_code == 400:
             raise BadRequestError(pydantic.parse_obj_as(typing.Any, _response.json()))  # type: ignore
@@ -299,15 +331,19 @@
         if data is not OMIT:
             _request["data"] = data
         _response = httpx.request(
             "POST",
             urllib.parse.urljoin(f"{self._environment.value}/", "list/names"),
             json=jsonable_encoder(_request),
             headers=remove_none_from_headers(
-                {"key-inflection": key_inflection, "idempotency-key": idempotency_key, "Authorization": self.api_key}
+                {
+                    "key-inflection": key_inflection,
+                    "idempotency-key": idempotency_key,
+                    "Authorization": f"Bearer  {self.api_key}",
+                }
             ),
             timeout=60,
         )
         if 200 <= _response.status_code < 300:
             return pydantic.parse_obj_as(CreateANameListResponse, _response.json())  # type: ignore
         if _response.status_code == 400:
             raise BadRequestError(pydantic.parse_obj_as(typing.Any, _response.json()))  # type: ignore
@@ -328,15 +364,19 @@
         if data is not OMIT:
             _request["data"] = data
         _response = httpx.request(
             "POST",
             urllib.parse.urljoin(f"{self._environment.value}/", "list/phone-numbers"),
             json=jsonable_encoder(_request),
             headers=remove_none_from_headers(
-                {"key-inflection": key_inflection, "idempotency-key": idempotency_key, "Authorization": self.api_key}
+                {
+                    "key-inflection": key_inflection,
+                    "idempotency-key": idempotency_key,
+                    "Authorization": f"Bearer  {self.api_key}",
+                }
             ),
             timeout=60,
         )
         if 200 <= _response.status_code < 300:
             return pydantic.parse_obj_as(CreateAPhoneNumberListResponse, _response.json())  # type: ignore
         if _response.status_code == 400:
             raise BadRequestError(pydantic.parse_obj_as(typing.Any, _response.json()))  # type: ignore
@@ -357,15 +397,19 @@
         if data is not OMIT:
             _request["data"] = data
         _response = httpx.request(
             "POST",
             urllib.parse.urljoin(f"{self._environment.value}/", "list-item/browser-fingerprints"),
             json=jsonable_encoder(_request),
             headers=remove_none_from_headers(
-                {"key-inflection": key_inflection, "idempotence-key": idempotence_key, "Authorization": self.api_key}
+                {
+                    "key-inflection": key_inflection,
+                    "idempotence-key": idempotence_key,
+                    "Authorization": f"Bearer  {self.api_key}",
+                }
             ),
             timeout=60,
         )
         if 200 <= _response.status_code < 300:
             return pydantic.parse_obj_as(CreateABrowserFingerprintListItemResponse, _response.json())  # type: ignore
         if _response.status_code == 400:
             raise BadRequestError(pydantic.parse_obj_as(typing.Any, _response.json()))  # type: ignore
@@ -386,15 +430,19 @@
         if data is not OMIT:
             _request["data"] = data
         _response = httpx.request(
             "POST",
             urllib.parse.urljoin(f"{self._environment.value}/", "list/faces"),
             json=jsonable_encoder(_request),
             headers=remove_none_from_headers(
-                {"key-inflection": key_inflection, "idempotency-key": idempotency_key, "Authorization": self.api_key}
+                {
+                    "key-inflection": key_inflection,
+                    "idempotency-key": idempotency_key,
+                    "Authorization": f"Bearer  {self.api_key}",
+                }
             ),
             timeout=60,
         )
         if 200 <= _response.status_code < 300:
             return pydantic.parse_obj_as(CreateAFaceListResponse, _response.json())  # type: ignore
         if _response.status_code == 400:
             raise BadRequestError(pydantic.parse_obj_as(typing.Any, _response.json()))  # type: ignore
@@ -425,15 +473,17 @@
                 urllib.parse.urljoin(f"{self._environment.value}/", "lists"),
                 params={
                     "page[before]": page_before,
                     "page[after]": page_after,
                     "page[size]": page_size,
                     "filter[status]": filter_status,
                 },
-                headers=remove_none_from_headers({"key-inflection": key_inflection, "Authorization": self.api_key}),
+                headers=remove_none_from_headers(
+                    {"key-inflection": key_inflection, "Authorization": f"Bearer  {self.api_key}"}
+                ),
                 timeout=60,
             )
         if 200 <= _response.status_code < 300:
             return pydantic.parse_obj_as(ListAllListsResponse, _response.json())  # type: ignore
         if _response.status_code == 400:
             raise BadRequestError(pydantic.parse_obj_as(typing.Any, _response.json()))  # type: ignore
         try:
@@ -445,15 +495,17 @@
     async def retrieve_a_list(
         self, list_id: str, *, key_inflection: typing.Optional[str] = None
     ) -> RetrieveAListResponse:
         async with httpx.AsyncClient() as _client:
             _response = await _client.request(
                 "GET",
                 urllib.parse.urljoin(f"{self._environment.value}/", f"lists/{list_id}"),
-                headers=remove_none_from_headers({"key-inflection": key_inflection, "Authorization": self.api_key}),
+                headers=remove_none_from_headers(
+                    {"key-inflection": key_inflection, "Authorization": f"Bearer  {self.api_key}"}
+                ),
                 timeout=60,
             )
         if 200 <= _response.status_code < 300:
             return pydantic.parse_obj_as(RetrieveAListResponse, _response.json())  # type: ignore
         if _response.status_code == 400:
             raise BadRequestError(pydantic.parse_obj_as(typing.Any, _response.json()))  # type: ignore
         try:
@@ -469,15 +521,15 @@
             _response = await _client.request(
                 "DELETE",
                 urllib.parse.urljoin(f"{self._environment.value}/", f"lists/{list_id}"),
                 headers=remove_none_from_headers(
                     {
                         "key-inflection": key_inflection,
                         "idempotency-key": idempotency_key,
-                        "Authorization": self.api_key,
+                        "Authorization": f"Bearer  {self.api_key}",
                     }
                 ),
                 timeout=60,
             )
         if 200 <= _response.status_code < 300:
             return pydantic.parse_obj_as(ArchiveAListResponse, _response.json())  # type: ignore
         if _response.status_code == 400:
@@ -503,15 +555,15 @@
                 "POST",
                 urllib.parse.urljoin(f"{self._environment.value}/", "list/browser-fingerprints"),
                 json=jsonable_encoder(_request),
                 headers=remove_none_from_headers(
                     {
                         "key-inflection": key_inflection,
                         "idempotency-key": idempotency_key,
-                        "Authorization": self.api_key,
+                        "Authorization": f"Bearer  {self.api_key}",
                     }
                 ),
                 timeout=60,
             )
         if 200 <= _response.status_code < 300:
             return pydantic.parse_obj_as(CreateABrowserFingerprintListResponse, _response.json())  # type: ignore
         if _response.status_code == 400:
@@ -537,15 +589,15 @@
                 "POST",
                 urllib.parse.urljoin(f"{self._environment.value}/", "list/countries"),
                 json=jsonable_encoder(_request),
                 headers=remove_none_from_headers(
                     {
                         "key-inflection": key_inflection,
                         "idempotency-key": idempotency_key,
-                        "Authorization": self.api_key,
+                        "Authorization": f"Bearer  {self.api_key}",
                     }
                 ),
                 timeout=60,
             )
         if 200 <= _response.status_code < 300:
             return pydantic.parse_obj_as(CreateACountryListResponse, _response.json())  # type: ignore
         if _response.status_code == 400:
@@ -571,15 +623,15 @@
                 "POST",
                 urllib.parse.urljoin(f"{self._environment.value}/", "list/email-addresses"),
                 json=jsonable_encoder(_request),
                 headers=remove_none_from_headers(
                     {
                         "key-inflection": key_inflection,
                         "idempotency-key": idempotency_key,
-                        "Authorization": self.api_key,
+                        "Authorization": f"Bearer  {self.api_key}",
                     }
                 ),
                 timeout=60,
             )
         if 200 <= _response.status_code < 300:
             return pydantic.parse_obj_as(CreateAnEmailAddressListResponse, _response.json())  # type: ignore
         if _response.status_code == 400:
@@ -605,15 +657,15 @@
                 "POST",
                 urllib.parse.urljoin(f"{self._environment.value}/", "list/geolocations"),
                 json=jsonable_encoder(_request),
                 headers=remove_none_from_headers(
                     {
                         "key-inflection": key_inflection,
                         "idempotency-key": idempotency_key,
-                        "Authorization": self.api_key,
+                        "Authorization": f"Bearer  {self.api_key}",
                     }
                 ),
                 timeout=60,
             )
         if 200 <= _response.status_code < 300:
             return pydantic.parse_obj_as(CreateAGeolocationListResponse, _response.json())  # type: ignore
         if _response.status_code == 400:
@@ -639,15 +691,15 @@
                 "POST",
                 urllib.parse.urljoin(f"{self._environment.value}/", "list/government-id-numbers"),
                 json=jsonable_encoder(_request),
                 headers=remove_none_from_headers(
                     {
                         "key-inflection": key_inflection,
                         "idempotency-key": idempotency_key,
-                        "Authorization": self.api_key,
+                        "Authorization": f"Bearer  {self.api_key}",
                     }
                 ),
                 timeout=60,
             )
         if 200 <= _response.status_code < 300:
             return pydantic.parse_obj_as(CreateAGovernmentIdNumberListResponse, _response.json())  # type: ignore
         if _response.status_code == 400:
@@ -673,15 +725,15 @@
                 "POST",
                 urllib.parse.urljoin(f"{self._environment.value}/", "list/ip-addresses"),
                 json=jsonable_encoder(_request),
                 headers=remove_none_from_headers(
                     {
                         "key-inflection": key_inflection,
                         "idempotency-key": idempotency_key,
-                        "Authorization": self.api_key,
+                        "Authorization": f"Bearer  {self.api_key}",
                     }
                 ),
                 timeout=60,
             )
         if 200 <= _response.status_code < 300:
             return pydantic.parse_obj_as(CreateAnIpAddressListResponse, _response.json())  # type: ignore
         if _response.status_code == 400:
@@ -707,15 +759,15 @@
                 "POST",
                 urllib.parse.urljoin(f"{self._environment.value}/", "list/names"),
                 json=jsonable_encoder(_request),
                 headers=remove_none_from_headers(
                     {
                         "key-inflection": key_inflection,
                         "idempotency-key": idempotency_key,
-                        "Authorization": self.api_key,
+                        "Authorization": f"Bearer  {self.api_key}",
                     }
                 ),
                 timeout=60,
             )
         if 200 <= _response.status_code < 300:
             return pydantic.parse_obj_as(CreateANameListResponse, _response.json())  # type: ignore
         if _response.status_code == 400:
@@ -741,15 +793,15 @@
                 "POST",
                 urllib.parse.urljoin(f"{self._environment.value}/", "list/phone-numbers"),
                 json=jsonable_encoder(_request),
                 headers=remove_none_from_headers(
                     {
                         "key-inflection": key_inflection,
                         "idempotency-key": idempotency_key,
-                        "Authorization": self.api_key,
+                        "Authorization": f"Bearer  {self.api_key}",
                     }
                 ),
                 timeout=60,
             )
         if 200 <= _response.status_code < 300:
             return pydantic.parse_obj_as(CreateAPhoneNumberListResponse, _response.json())  # type: ignore
         if _response.status_code == 400:
@@ -775,15 +827,15 @@
                 "POST",
                 urllib.parse.urljoin(f"{self._environment.value}/", "list-item/browser-fingerprints"),
                 json=jsonable_encoder(_request),
                 headers=remove_none_from_headers(
                     {
                         "key-inflection": key_inflection,
                         "idempotence-key": idempotence_key,
-                        "Authorization": self.api_key,
+                        "Authorization": f"Bearer  {self.api_key}",
                     }
                 ),
                 timeout=60,
             )
         if 200 <= _response.status_code < 300:
             return pydantic.parse_obj_as(CreateABrowserFingerprintListItemResponse, _response.json())  # type: ignore
         if _response.status_code == 400:
@@ -809,15 +861,15 @@
                 "POST",
                 urllib.parse.urljoin(f"{self._environment.value}/", "list/faces"),
                 json=jsonable_encoder(_request),
                 headers=remove_none_from_headers(
                     {
                         "key-inflection": key_inflection,
                         "idempotency-key": idempotency_key,
-                        "Authorization": self.api_key,
+                        "Authorization": f"Bearer  {self.api_key}",
                     }
                 ),
                 timeout=60,
             )
         if 200 <= _response.status_code < 300:
             return pydantic.parse_obj_as(CreateAFaceListResponse, _response.json())  # type: ignore
         if _response.status_code == 400:
```

### Comparing `fern_persona-0.0.2/src/persona/resources/phone_carrier_database_verifications/client.py` & `fern_persona-0.0.3/src/persona/resources/phone_carrier_database_verifications/client.py`

 * *Files 6% similar despite different names*

```diff
@@ -43,15 +43,19 @@
     ) -> SubmitAPhoneCarrierDatabaseVerificationResponse:
         _response = httpx.request(
             "POST",
             urllib.parse.urljoin(
                 f"{self._environment.value}/", f"verification/database-phone-carriers/{verification_id}/submit"
             ),
             headers=remove_none_from_headers(
-                {"Key-Inflection": key_inflection, "Idempotency-Key": idempotency_key, "Authorization": self.api_key}
+                {
+                    "Key-Inflection": key_inflection,
+                    "Idempotency-Key": idempotency_key,
+                    "Authorization": f"Bearer  {self.api_key}",
+                }
             ),
             timeout=60,
         )
         if 200 <= _response.status_code < 300:
             return pydantic.parse_obj_as(SubmitAPhoneCarrierDatabaseVerificationResponse, _response.json())  # type: ignore
         if _response.status_code == 400:
             raise BadRequestError(pydantic.parse_obj_as(typing.Any, _response.json()))  # type: ignore
@@ -67,15 +71,15 @@
         _request: typing.Dict[str, typing.Any] = {}
         if attributes is not OMIT:
             _request["attributes"] = attributes
         _response = httpx.request(
             "POST",
             urllib.parse.urljoin(f"{self._environment.value}/", "verification/database-phone-carriers"),
             json=jsonable_encoder(_request),
-            headers=remove_none_from_headers({"Authorization": self.api_key}),
+            headers=remove_none_from_headers({"Authorization": f"Bearer  {self.api_key}"}),
             timeout=60,
         )
         if 200 <= _response.status_code < 300:
             return pydantic.parse_obj_as(CreateAPhoneCarrierDatabaseVerificationResponse, _response.json())  # type: ignore
         if _response.status_code == 400:
             raise BadRequestError(pydantic.parse_obj_as(typing.Any, _response.json()))  # type: ignore
         try:
@@ -88,15 +92,17 @@
         self, verification_id: str, *, key_inflection: typing.Optional[str] = None
     ) -> RetrieveAPhoneCarrierDatabaseVerificationResponse:
         _response = httpx.request(
             "GET",
             urllib.parse.urljoin(
                 f"{self._environment.value}/", f"verification/database-phone-carriers/{verification_id}"
             ),
-            headers=remove_none_from_headers({"Key-Inflection": key_inflection, "Authorization": self.api_key}),
+            headers=remove_none_from_headers(
+                {"Key-Inflection": key_inflection, "Authorization": f"Bearer  {self.api_key}"}
+            ),
             timeout=60,
         )
         if 200 <= _response.status_code < 300:
             return pydantic.parse_obj_as(RetrieveAPhoneCarrierDatabaseVerificationResponse, _response.json())  # type: ignore
         if _response.status_code == 400:
             raise BadRequestError(pydantic.parse_obj_as(typing.Any, _response.json()))  # type: ignore
         try:
@@ -124,15 +130,15 @@
                 urllib.parse.urljoin(
                     f"{self._environment.value}/", f"verification/database-phone-carriers/{verification_id}/submit"
                 ),
                 headers=remove_none_from_headers(
                     {
                         "Key-Inflection": key_inflection,
                         "Idempotency-Key": idempotency_key,
-                        "Authorization": self.api_key,
+                        "Authorization": f"Bearer  {self.api_key}",
                     }
                 ),
                 timeout=60,
             )
         if 200 <= _response.status_code < 300:
             return pydantic.parse_obj_as(SubmitAPhoneCarrierDatabaseVerificationResponse, _response.json())  # type: ignore
         if _response.status_code == 400:
@@ -150,15 +156,15 @@
         if attributes is not OMIT:
             _request["attributes"] = attributes
         async with httpx.AsyncClient() as _client:
             _response = await _client.request(
                 "POST",
                 urllib.parse.urljoin(f"{self._environment.value}/", "verification/database-phone-carriers"),
                 json=jsonable_encoder(_request),
-                headers=remove_none_from_headers({"Authorization": self.api_key}),
+                headers=remove_none_from_headers({"Authorization": f"Bearer  {self.api_key}"}),
                 timeout=60,
             )
         if 200 <= _response.status_code < 300:
             return pydantic.parse_obj_as(CreateAPhoneCarrierDatabaseVerificationResponse, _response.json())  # type: ignore
         if _response.status_code == 400:
             raise BadRequestError(pydantic.parse_obj_as(typing.Any, _response.json()))  # type: ignore
         try:
@@ -172,15 +178,17 @@
     ) -> RetrieveAPhoneCarrierDatabaseVerificationResponse:
         async with httpx.AsyncClient() as _client:
             _response = await _client.request(
                 "GET",
                 urllib.parse.urljoin(
                     f"{self._environment.value}/", f"verification/database-phone-carriers/{verification_id}"
                 ),
-                headers=remove_none_from_headers({"Key-Inflection": key_inflection, "Authorization": self.api_key}),
+                headers=remove_none_from_headers(
+                    {"Key-Inflection": key_inflection, "Authorization": f"Bearer  {self.api_key}"}
+                ),
                 timeout=60,
             )
         if 200 <= _response.status_code < 300:
             return pydantic.parse_obj_as(RetrieveAPhoneCarrierDatabaseVerificationResponse, _response.json())  # type: ignore
         if _response.status_code == 400:
             raise BadRequestError(pydantic.parse_obj_as(typing.Any, _response.json()))  # type: ignore
         try:
```

### Comparing `fern_persona-0.0.2/src/persona/resources/phone_number_verifications/client.py` & `fern_persona-0.0.3/src/persona/resources/phone_number_verifications/client.py`

 * *Files 6% similar despite different names*

```diff
@@ -37,15 +37,19 @@
         idempotency_key: typing.Optional[str] = None,
     ) -> CreateAPhoneNumberVerificationResponse:
         _response = httpx.request(
             "POST",
             urllib.parse.urljoin(f"{self._environment.value}/", "verification/phone-numbers"),
             json=jsonable_encoder({"data": data}),
             headers=remove_none_from_headers(
-                {"Key-Inflection": key_inflection, "Idempotency-Key": idempotency_key, "Authorization": self.api_key}
+                {
+                    "Key-Inflection": key_inflection,
+                    "Idempotency-Key": idempotency_key,
+                    "Authorization": f"Bearer  {self.api_key}",
+                }
             ),
             timeout=60,
         )
         if 200 <= _response.status_code < 300:
             return pydantic.parse_obj_as(CreateAPhoneNumberVerificationResponse, _response.json())  # type: ignore
         try:
             _response_json = _response.json()
@@ -58,15 +62,15 @@
     ) -> ConfirmAPhoneNumberVerificationResponse:
         _response = httpx.request(
             "POST",
             urllib.parse.urljoin(
                 f"{self._environment.value}/", f"verification/phone-numbers/{verification_id}/confirm"
             ),
             json=jsonable_encoder({"data": data}),
-            headers=remove_none_from_headers({"Authorization": self.api_key}),
+            headers=remove_none_from_headers({"Authorization": f"Bearer  {self.api_key}"}),
             timeout=60,
         )
         if 200 <= _response.status_code < 300:
             return pydantic.parse_obj_as(ConfirmAPhoneNumberVerificationResponse, _response.json())  # type: ignore
         if _response.status_code == 400:
             raise BadRequestError(pydantic.parse_obj_as(typing.Any, _response.json()))  # type: ignore
         try:
@@ -77,15 +81,17 @@
 
     def retrieve_a_phone_number_verification(
         self, verification_id: str, *, key_inflection: typing.Optional[str] = None
     ) -> RetrieveAPhoneNumberVerificationResponse:
         _response = httpx.request(
             "GET",
             urllib.parse.urljoin(f"{self._environment.value}/", f"verification/phone-numbers/{verification_id}"),
-            headers=remove_none_from_headers({"Key-Inflection": key_inflection, "Authorization": self.api_key}),
+            headers=remove_none_from_headers(
+                {"Key-Inflection": key_inflection, "Authorization": f"Bearer  {self.api_key}"}
+            ),
             timeout=60,
         )
         if 200 <= _response.status_code < 300:
             return pydantic.parse_obj_as(RetrieveAPhoneNumberVerificationResponse, _response.json())  # type: ignore
         if _response.status_code == 400:
             raise BadRequestError(pydantic.parse_obj_as(typing.Any, _response.json()))  # type: ignore
         try:
@@ -102,15 +108,15 @@
             _request["data"] = data
         _response = httpx.request(
             "POST",
             urllib.parse.urljoin(
                 f"{self._environment.value}/", f"verification/phone-numbers/{verification_id}/send-confirmation-code"
             ),
             json=jsonable_encoder(_request),
-            headers=remove_none_from_headers({"Authorization": self.api_key}),
+            headers=remove_none_from_headers({"Authorization": f"Bearer  {self.api_key}"}),
             timeout=60,
         )
         if 200 <= _response.status_code < 300:
             return pydantic.parse_obj_as(SendAnSmsResponse, _response.json())  # type: ignore
         if _response.status_code == 400:
             raise BadRequestError(pydantic.parse_obj_as(typing.Any, _response.json()))  # type: ignore
         try:
@@ -137,15 +143,15 @@
                 "POST",
                 urllib.parse.urljoin(f"{self._environment.value}/", "verification/phone-numbers"),
                 json=jsonable_encoder({"data": data}),
                 headers=remove_none_from_headers(
                     {
                         "Key-Inflection": key_inflection,
                         "Idempotency-Key": idempotency_key,
-                        "Authorization": self.api_key,
+                        "Authorization": f"Bearer  {self.api_key}",
                     }
                 ),
                 timeout=60,
             )
         if 200 <= _response.status_code < 300:
             return pydantic.parse_obj_as(CreateAPhoneNumberVerificationResponse, _response.json())  # type: ignore
         try:
@@ -160,15 +166,15 @@
         async with httpx.AsyncClient() as _client:
             _response = await _client.request(
                 "POST",
                 urllib.parse.urljoin(
                     f"{self._environment.value}/", f"verification/phone-numbers/{verification_id}/confirm"
                 ),
                 json=jsonable_encoder({"data": data}),
-                headers=remove_none_from_headers({"Authorization": self.api_key}),
+                headers=remove_none_from_headers({"Authorization": f"Bearer  {self.api_key}"}),
                 timeout=60,
             )
         if 200 <= _response.status_code < 300:
             return pydantic.parse_obj_as(ConfirmAPhoneNumberVerificationResponse, _response.json())  # type: ignore
         if _response.status_code == 400:
             raise BadRequestError(pydantic.parse_obj_as(typing.Any, _response.json()))  # type: ignore
         try:
@@ -180,15 +186,17 @@
     async def retrieve_a_phone_number_verification(
         self, verification_id: str, *, key_inflection: typing.Optional[str] = None
     ) -> RetrieveAPhoneNumberVerificationResponse:
         async with httpx.AsyncClient() as _client:
             _response = await _client.request(
                 "GET",
                 urllib.parse.urljoin(f"{self._environment.value}/", f"verification/phone-numbers/{verification_id}"),
-                headers=remove_none_from_headers({"Key-Inflection": key_inflection, "Authorization": self.api_key}),
+                headers=remove_none_from_headers(
+                    {"Key-Inflection": key_inflection, "Authorization": f"Bearer  {self.api_key}"}
+                ),
                 timeout=60,
             )
         if 200 <= _response.status_code < 300:
             return pydantic.parse_obj_as(RetrieveAPhoneNumberVerificationResponse, _response.json())  # type: ignore
         if _response.status_code == 400:
             raise BadRequestError(pydantic.parse_obj_as(typing.Any, _response.json()))  # type: ignore
         try:
@@ -207,15 +215,15 @@
             _response = await _client.request(
                 "POST",
                 urllib.parse.urljoin(
                     f"{self._environment.value}/",
                     f"verification/phone-numbers/{verification_id}/send-confirmation-code",
                 ),
                 json=jsonable_encoder(_request),
-                headers=remove_none_from_headers({"Authorization": self.api_key}),
+                headers=remove_none_from_headers({"Authorization": f"Bearer  {self.api_key}"}),
                 timeout=60,
             )
         if 200 <= _response.status_code < 300:
             return pydantic.parse_obj_as(SendAnSmsResponse, _response.json())  # type: ignore
         if _response.status_code == 400:
             raise BadRequestError(pydantic.parse_obj_as(typing.Any, _response.json()))  # type: ignore
         try:
```

### Comparing `fern_persona-0.0.2/src/persona/resources/print_verifications/client.py` & `fern_persona-0.0.3/src/persona/resources/print_verifications/client.py`

 * *Files 2% similar despite different names*

```diff
@@ -15,15 +15,15 @@
         self._environment = environment
         self.api_key = api_key
 
     def print_a_verification_as_pdf(self, verification_id: str) -> None:
         _response = httpx.request(
             "GET",
             urllib.parse.urljoin(f"{self._environment.value}/", f"verifications/{verification_id}/print"),
-            headers=remove_none_from_headers({"Authorization": self.api_key}),
+            headers=remove_none_from_headers({"Authorization": f"Bearer  {self.api_key}"}),
             timeout=60,
         )
         if 200 <= _response.status_code < 300:
             return
         try:
             _response_json = _response.json()
         except JSONDecodeError:
@@ -37,15 +37,15 @@
         self.api_key = api_key
 
     async def print_a_verification_as_pdf(self, verification_id: str) -> None:
         async with httpx.AsyncClient() as _client:
             _response = await _client.request(
                 "GET",
                 urllib.parse.urljoin(f"{self._environment.value}/", f"verifications/{verification_id}/print"),
-                headers=remove_none_from_headers({"Authorization": self.api_key}),
+                headers=remove_none_from_headers({"Authorization": f"Bearer  {self.api_key}"}),
                 timeout=60,
             )
         if 200 <= _response.status_code < 300:
             return
         try:
             _response_json = _response.json()
         except JSONDecodeError:
```

### Comparing `fern_persona-0.0.2/src/persona/resources/reports/client.py` & `fern_persona-0.0.3/src/persona/resources/reports/client.py`

 * *Files 9% similar despite different names*

```diff
@@ -40,30 +40,34 @@
 
     def retrieve_a_report(
         self, report_id: str, *, key_inflection: typing.Optional[str] = None
     ) -> RetrieveAReportResponse:
         _response = httpx.request(
             "GET",
             urllib.parse.urljoin(f"{self._environment.value}/", f"reports/{report_id}"),
-            headers=remove_none_from_headers({"Key-Inflection": key_inflection, "Authorization": self.api_key}),
+            headers=remove_none_from_headers(
+                {"Key-Inflection": key_inflection, "Authorization": f"Bearer  {self.api_key}"}
+            ),
             timeout=60,
         )
         if 200 <= _response.status_code < 300:
             return pydantic.parse_obj_as(RetrieveAReportResponse, _response.json())  # type: ignore
         try:
             _response_json = _response.json()
         except JSONDecodeError:
             raise ApiError(status_code=_response.status_code, body=_response.text)
         raise ApiError(status_code=_response.status_code, body=_response_json)
 
     def redact_a_report(self, report_id: str, *, persona_version: typing.Optional[str] = None) -> RedactAReportResponse:
         _response = httpx.request(
             "DELETE",
             urllib.parse.urljoin(f"{self._environment.value}/", f"reports/{report_id}"),
-            headers=remove_none_from_headers({"Persona-Version": persona_version, "Authorization": self.api_key}),
+            headers=remove_none_from_headers(
+                {"Persona-Version": persona_version, "Authorization": f"Bearer  {self.api_key}"}
+            ),
             timeout=60,
         )
         if 200 <= _response.status_code < 300:
             return pydantic.parse_obj_as(RedactAReportResponse, _response.json())  # type: ignore
         try:
             _response_json = _response.json()
         except JSONDecodeError:
@@ -86,15 +90,17 @@
             params={
                 "page[before]": page_before,
                 "page[after]": page_after,
                 "page[size]": page_size,
                 "filter[reference-id]": filter_reference_id,
                 "filter[account-id]": filter_account_id,
             },
-            headers=remove_none_from_headers({"Key-Inflection": key_inflection, "Authorization": self.api_key}),
+            headers=remove_none_from_headers(
+                {"Key-Inflection": key_inflection, "Authorization": f"Bearer  {self.api_key}"}
+            ),
             timeout=60,
         )
         if 200 <= _response.status_code < 300:
             return
         if _response.status_code == 400:
             raise BadRequestError(pydantic.parse_obj_as(typing.Any, _response.json()))  # type: ignore
         try:
@@ -104,15 +110,17 @@
         raise ApiError(status_code=_response.status_code, body=_response_json)
 
     def create_a_report(self, *, data: CreateAReportRequestData, key_inflection: typing.Optional[str] = None) -> None:
         _response = httpx.request(
             "POST",
             urllib.parse.urljoin(f"{self._environment.value}/", "reports"),
             json=jsonable_encoder({"data": data}),
-            headers=remove_none_from_headers({"Key-Inflection": key_inflection, "Authorization": self.api_key}),
+            headers=remove_none_from_headers(
+                {"Key-Inflection": key_inflection, "Authorization": f"Bearer  {self.api_key}"}
+            ),
             timeout=60,
         )
         if 200 <= _response.status_code < 300:
             return
         if _response.status_code == 400:
             raise BadRequestError(pydantic.parse_obj_as(typing.Any, _response.json()))  # type: ignore
         try:
@@ -121,15 +129,15 @@
             raise ApiError(status_code=_response.status_code, body=_response.text)
         raise ApiError(status_code=_response.status_code, body=_response_json)
 
     def print_report_pdf(self, report_id: str) -> None:
         _response = httpx.request(
             "GET",
             urllib.parse.urljoin(f"{self._environment.value}/", f"reports/{report_id}/print"),
-            headers=remove_none_from_headers({"Authorization": self.api_key}),
+            headers=remove_none_from_headers({"Authorization": f"Bearer  {self.api_key}"}),
             timeout=60,
         )
         if 200 <= _response.status_code < 300:
             return
         try:
             _response_json = _response.json()
         except JSONDecodeError:
@@ -142,15 +150,15 @@
         _request: typing.Dict[str, typing.Any] = {}
         if data is not OMIT:
             _request["data"] = data
         _response = httpx.request(
             "POST",
             urllib.parse.urljoin(f"{self._environment.value}/", "reports/biz-lookup"),
             json=jsonable_encoder(_request),
-            headers=remove_none_from_headers({"Authorization": self.api_key}),
+            headers=remove_none_from_headers({"Authorization": f"Bearer  {self.api_key}"}),
             timeout=60,
         )
         if 200 <= _response.status_code < 300:
             return pydantic.parse_obj_as(BusinessLookupReport1Response, _response.json())  # type: ignore
         if _response.status_code == 400:
             raise BadRequestError(pydantic.parse_obj_as(typing.Any, _response.json()))  # type: ignore
         try:
@@ -171,15 +179,19 @@
         if meta is not OMIT:
             _request["meta"] = meta
         _response = httpx.request(
             "POST",
             urllib.parse.urljoin(f"{self._environment.value}/", f"reports/{report_id}/add-tag"),
             json=jsonable_encoder(_request),
             headers=remove_none_from_headers(
-                {"Key-Inflection": key_inflection, "Idempotency-Key": idempotency_key, "Authorization": self.api_key}
+                {
+                    "Key-Inflection": key_inflection,
+                    "Idempotency-Key": idempotency_key,
+                    "Authorization": f"Bearer  {self.api_key}",
+                }
             ),
             timeout=60,
         )
         if 200 <= _response.status_code < 300:
             return pydantic.parse_obj_as(ReportsAddATagResponse, _response.json())  # type: ignore
         if _response.status_code == 400:
             raise BadRequestError(pydantic.parse_obj_as(typing.Any, _response.json()))  # type: ignore
@@ -201,15 +213,19 @@
         if meta is not OMIT:
             _request["meta"] = meta
         _response = httpx.request(
             "POST",
             urllib.parse.urljoin(f"{self._environment.value}/", f"reports/{report_id}/remove-tag"),
             json=jsonable_encoder(_request),
             headers=remove_none_from_headers(
-                {"Key-Inflection": key_inflection, "Idempotency-Key": idempotency_key, "Authorization": self.api_key}
+                {
+                    "Key-Inflection": key_inflection,
+                    "Idempotency-Key": idempotency_key,
+                    "Authorization": f"Bearer  {self.api_key}",
+                }
             ),
             timeout=60,
         )
         if 200 <= _response.status_code < 300:
             return pydantic.parse_obj_as(ReportsRemoveATagResponse, _response.json())  # type: ignore
         if _response.status_code == 400:
             raise BadRequestError(pydantic.parse_obj_as(typing.Any, _response.json()))  # type: ignore
@@ -231,15 +247,19 @@
         if meta is not OMIT:
             _request["meta"] = meta
         _response = httpx.request(
             "POST",
             urllib.parse.urljoin(f"{self._environment.value}/", f"reports/{report_id}/set-tags"),
             json=jsonable_encoder(_request),
             headers=remove_none_from_headers(
-                {"Key-Inflection": key_inflection, "Idempotency-Key": idempotency_key, "Authorization": self.api_key}
+                {
+                    "Key-Inflection": key_inflection,
+                    "Idempotency-Key": idempotency_key,
+                    "Authorization": f"Bearer  {self.api_key}",
+                }
             ),
             timeout=60,
         )
         if 200 <= _response.status_code < 300:
             return pydantic.parse_obj_as(ReportsSetAllTagsResponse, _response.json())  # type: ignore
         if _response.status_code == 400:
             raise BadRequestError(pydantic.parse_obj_as(typing.Any, _response.json()))  # type: ignore
@@ -249,15 +269,15 @@
             raise ApiError(status_code=_response.status_code, body=_response.text)
         raise ApiError(status_code=_response.status_code, body=_response_json)
 
     def report_action_re_run_report(self, report_id: str) -> ReportActionReRunReportResponse:
         _response = httpx.request(
             "POST",
             urllib.parse.urljoin(f"{self._environment.value}/", f"reports/{report_id}/run"),
-            headers=remove_none_from_headers({"Authorization": self.api_key}),
+            headers=remove_none_from_headers({"Authorization": f"Bearer  {self.api_key}"}),
             timeout=60,
         )
         if 200 <= _response.status_code < 300:
             return pydantic.parse_obj_as(ReportActionReRunReportResponse, _response.json())  # type: ignore
         if _response.status_code == 400:
             raise BadRequestError(pydantic.parse_obj_as(typing.Any, _response.json()))  # type: ignore
         try:
@@ -275,15 +295,19 @@
         idempotency_key: typing.Optional[str] = None,
     ) -> DismissMatchesResponse:
         _response = httpx.request(
             "POST",
             urllib.parse.urljoin(f"{self._environment.value}/", f"reports/{report_id}/dismiss"),
             json=jsonable_encoder({"data": data}),
             headers=remove_none_from_headers(
-                {"Key-Inflection": key_inflection, "Idempotency-Key": idempotency_key, "Authorization": self.api_key}
+                {
+                    "Key-Inflection": key_inflection,
+                    "Idempotency-Key": idempotency_key,
+                    "Authorization": f"Bearer  {self.api_key}",
+                }
             ),
             timeout=60,
         )
         if 200 <= _response.status_code < 300:
             return pydantic.parse_obj_as(DismissMatchesResponse, _response.json())  # type: ignore
         if _response.status_code == 400:
             raise BadRequestError(pydantic.parse_obj_as(typing.Any, _response.json()))  # type: ignore
@@ -295,15 +319,15 @@
 
     def report_action_resume_continuous_monitoring(
         self, report_id: str
     ) -> ReportActionResumeContinuousMonitoringResponse:
         _response = httpx.request(
             "POST",
             urllib.parse.urljoin(f"{self._environment.value}/", f"reports/{report_id}/resume"),
-            headers=remove_none_from_headers({"Authorization": self.api_key}),
+            headers=remove_none_from_headers({"Authorization": f"Bearer  {self.api_key}"}),
             timeout=60,
         )
         if 200 <= _response.status_code < 300:
             return pydantic.parse_obj_as(ReportActionResumeContinuousMonitoringResponse, _response.json())  # type: ignore
         if _response.status_code == 400:
             raise BadRequestError(pydantic.parse_obj_as(typing.Any, _response.json()))  # type: ignore
         try:
@@ -314,15 +338,15 @@
 
     def report_action_pause_continuous_monitoring(
         self, report_id: str
     ) -> ReportActionPauseContinuousMonitoringResponse:
         _response = httpx.request(
             "POST",
             urllib.parse.urljoin(f"{self._environment.value}/", f"reports/{report_id}/pause"),
-            headers=remove_none_from_headers({"Authorization": self.api_key}),
+            headers=remove_none_from_headers({"Authorization": f"Bearer  {self.api_key}"}),
             timeout=60,
         )
         if 200 <= _response.status_code < 300:
             return pydantic.parse_obj_as(ReportActionPauseContinuousMonitoringResponse, _response.json())  # type: ignore
         if _response.status_code == 400:
             raise BadRequestError(pydantic.parse_obj_as(typing.Any, _response.json()))  # type: ignore
         try:
@@ -340,15 +364,17 @@
     async def retrieve_a_report(
         self, report_id: str, *, key_inflection: typing.Optional[str] = None
     ) -> RetrieveAReportResponse:
         async with httpx.AsyncClient() as _client:
             _response = await _client.request(
                 "GET",
                 urllib.parse.urljoin(f"{self._environment.value}/", f"reports/{report_id}"),
-                headers=remove_none_from_headers({"Key-Inflection": key_inflection, "Authorization": self.api_key}),
+                headers=remove_none_from_headers(
+                    {"Key-Inflection": key_inflection, "Authorization": f"Bearer  {self.api_key}"}
+                ),
                 timeout=60,
             )
         if 200 <= _response.status_code < 300:
             return pydantic.parse_obj_as(RetrieveAReportResponse, _response.json())  # type: ignore
         try:
             _response_json = _response.json()
         except JSONDecodeError:
@@ -358,15 +384,17 @@
     async def redact_a_report(
         self, report_id: str, *, persona_version: typing.Optional[str] = None
     ) -> RedactAReportResponse:
         async with httpx.AsyncClient() as _client:
             _response = await _client.request(
                 "DELETE",
                 urllib.parse.urljoin(f"{self._environment.value}/", f"reports/{report_id}"),
-                headers=remove_none_from_headers({"Persona-Version": persona_version, "Authorization": self.api_key}),
+                headers=remove_none_from_headers(
+                    {"Persona-Version": persona_version, "Authorization": f"Bearer  {self.api_key}"}
+                ),
                 timeout=60,
             )
         if 200 <= _response.status_code < 300:
             return pydantic.parse_obj_as(RedactAReportResponse, _response.json())  # type: ignore
         try:
             _response_json = _response.json()
         except JSONDecodeError:
@@ -390,15 +418,17 @@
                 params={
                     "page[before]": page_before,
                     "page[after]": page_after,
                     "page[size]": page_size,
                     "filter[reference-id]": filter_reference_id,
                     "filter[account-id]": filter_account_id,
                 },
-                headers=remove_none_from_headers({"Key-Inflection": key_inflection, "Authorization": self.api_key}),
+                headers=remove_none_from_headers(
+                    {"Key-Inflection": key_inflection, "Authorization": f"Bearer  {self.api_key}"}
+                ),
                 timeout=60,
             )
         if 200 <= _response.status_code < 300:
             return
         if _response.status_code == 400:
             raise BadRequestError(pydantic.parse_obj_as(typing.Any, _response.json()))  # type: ignore
         try:
@@ -411,15 +441,17 @@
         self, *, data: CreateAReportRequestData, key_inflection: typing.Optional[str] = None
     ) -> None:
         async with httpx.AsyncClient() as _client:
             _response = await _client.request(
                 "POST",
                 urllib.parse.urljoin(f"{self._environment.value}/", "reports"),
                 json=jsonable_encoder({"data": data}),
-                headers=remove_none_from_headers({"Key-Inflection": key_inflection, "Authorization": self.api_key}),
+                headers=remove_none_from_headers(
+                    {"Key-Inflection": key_inflection, "Authorization": f"Bearer  {self.api_key}"}
+                ),
                 timeout=60,
             )
         if 200 <= _response.status_code < 300:
             return
         if _response.status_code == 400:
             raise BadRequestError(pydantic.parse_obj_as(typing.Any, _response.json()))  # type: ignore
         try:
@@ -429,15 +461,15 @@
         raise ApiError(status_code=_response.status_code, body=_response_json)
 
     async def print_report_pdf(self, report_id: str) -> None:
         async with httpx.AsyncClient() as _client:
             _response = await _client.request(
                 "GET",
                 urllib.parse.urljoin(f"{self._environment.value}/", f"reports/{report_id}/print"),
-                headers=remove_none_from_headers({"Authorization": self.api_key}),
+                headers=remove_none_from_headers({"Authorization": f"Bearer  {self.api_key}"}),
                 timeout=60,
             )
         if 200 <= _response.status_code < 300:
             return
         try:
             _response_json = _response.json()
         except JSONDecodeError:
@@ -451,15 +483,15 @@
         if data is not OMIT:
             _request["data"] = data
         async with httpx.AsyncClient() as _client:
             _response = await _client.request(
                 "POST",
                 urllib.parse.urljoin(f"{self._environment.value}/", "reports/biz-lookup"),
                 json=jsonable_encoder(_request),
-                headers=remove_none_from_headers({"Authorization": self.api_key}),
+                headers=remove_none_from_headers({"Authorization": f"Bearer  {self.api_key}"}),
                 timeout=60,
             )
         if 200 <= _response.status_code < 300:
             return pydantic.parse_obj_as(BusinessLookupReport1Response, _response.json())  # type: ignore
         if _response.status_code == 400:
             raise BadRequestError(pydantic.parse_obj_as(typing.Any, _response.json()))  # type: ignore
         try:
@@ -484,15 +516,15 @@
                 "POST",
                 urllib.parse.urljoin(f"{self._environment.value}/", f"reports/{report_id}/add-tag"),
                 json=jsonable_encoder(_request),
                 headers=remove_none_from_headers(
                     {
                         "Key-Inflection": key_inflection,
                         "Idempotency-Key": idempotency_key,
-                        "Authorization": self.api_key,
+                        "Authorization": f"Bearer  {self.api_key}",
                     }
                 ),
                 timeout=60,
             )
         if 200 <= _response.status_code < 300:
             return pydantic.parse_obj_as(ReportsAddATagResponse, _response.json())  # type: ignore
         if _response.status_code == 400:
@@ -519,15 +551,15 @@
                 "POST",
                 urllib.parse.urljoin(f"{self._environment.value}/", f"reports/{report_id}/remove-tag"),
                 json=jsonable_encoder(_request),
                 headers=remove_none_from_headers(
                     {
                         "Key-Inflection": key_inflection,
                         "Idempotency-Key": idempotency_key,
-                        "Authorization": self.api_key,
+                        "Authorization": f"Bearer  {self.api_key}",
                     }
                 ),
                 timeout=60,
             )
         if 200 <= _response.status_code < 300:
             return pydantic.parse_obj_as(ReportsRemoveATagResponse, _response.json())  # type: ignore
         if _response.status_code == 400:
@@ -554,15 +586,15 @@
                 "POST",
                 urllib.parse.urljoin(f"{self._environment.value}/", f"reports/{report_id}/set-tags"),
                 json=jsonable_encoder(_request),
                 headers=remove_none_from_headers(
                     {
                         "Key-Inflection": key_inflection,
                         "Idempotency-Key": idempotency_key,
-                        "Authorization": self.api_key,
+                        "Authorization": f"Bearer  {self.api_key}",
                     }
                 ),
                 timeout=60,
             )
         if 200 <= _response.status_code < 300:
             return pydantic.parse_obj_as(ReportsSetAllTagsResponse, _response.json())  # type: ignore
         if _response.status_code == 400:
@@ -574,15 +606,15 @@
         raise ApiError(status_code=_response.status_code, body=_response_json)
 
     async def report_action_re_run_report(self, report_id: str) -> ReportActionReRunReportResponse:
         async with httpx.AsyncClient() as _client:
             _response = await _client.request(
                 "POST",
                 urllib.parse.urljoin(f"{self._environment.value}/", f"reports/{report_id}/run"),
-                headers=remove_none_from_headers({"Authorization": self.api_key}),
+                headers=remove_none_from_headers({"Authorization": f"Bearer  {self.api_key}"}),
                 timeout=60,
             )
         if 200 <= _response.status_code < 300:
             return pydantic.parse_obj_as(ReportActionReRunReportResponse, _response.json())  # type: ignore
         if _response.status_code == 400:
             raise BadRequestError(pydantic.parse_obj_as(typing.Any, _response.json()))  # type: ignore
         try:
@@ -604,15 +636,15 @@
                 "POST",
                 urllib.parse.urljoin(f"{self._environment.value}/", f"reports/{report_id}/dismiss"),
                 json=jsonable_encoder({"data": data}),
                 headers=remove_none_from_headers(
                     {
                         "Key-Inflection": key_inflection,
                         "Idempotency-Key": idempotency_key,
-                        "Authorization": self.api_key,
+                        "Authorization": f"Bearer  {self.api_key}",
                     }
                 ),
                 timeout=60,
             )
         if 200 <= _response.status_code < 300:
             return pydantic.parse_obj_as(DismissMatchesResponse, _response.json())  # type: ignore
         if _response.status_code == 400:
@@ -626,15 +658,15 @@
     async def report_action_resume_continuous_monitoring(
         self, report_id: str
     ) -> ReportActionResumeContinuousMonitoringResponse:
         async with httpx.AsyncClient() as _client:
             _response = await _client.request(
                 "POST",
                 urllib.parse.urljoin(f"{self._environment.value}/", f"reports/{report_id}/resume"),
-                headers=remove_none_from_headers({"Authorization": self.api_key}),
+                headers=remove_none_from_headers({"Authorization": f"Bearer  {self.api_key}"}),
                 timeout=60,
             )
         if 200 <= _response.status_code < 300:
             return pydantic.parse_obj_as(ReportActionResumeContinuousMonitoringResponse, _response.json())  # type: ignore
         if _response.status_code == 400:
             raise BadRequestError(pydantic.parse_obj_as(typing.Any, _response.json()))  # type: ignore
         try:
@@ -646,15 +678,15 @@
     async def report_action_pause_continuous_monitoring(
         self, report_id: str
     ) -> ReportActionPauseContinuousMonitoringResponse:
         async with httpx.AsyncClient() as _client:
             _response = await _client.request(
                 "POST",
                 urllib.parse.urljoin(f"{self._environment.value}/", f"reports/{report_id}/pause"),
-                headers=remove_none_from_headers({"Authorization": self.api_key}),
+                headers=remove_none_from_headers({"Authorization": f"Bearer  {self.api_key}"}),
                 timeout=60,
             )
         if 200 <= _response.status_code < 300:
             return pydantic.parse_obj_as(ReportActionPauseContinuousMonitoringResponse, _response.json())  # type: ignore
         if _response.status_code == 400:
             raise BadRequestError(pydantic.parse_obj_as(typing.Any, _response.json()))  # type: ignore
         try:
```

### Comparing `fern_persona-0.0.2/src/persona/resources/selfie_verifications/client.py` & `fern_persona-0.0.3/src/persona/resources/selfie_verifications/client.py`

 * *Files 3% similar despite different names*

```diff
@@ -31,15 +31,19 @@
         idempotency_key: typing.Optional[str] = None,
     ) -> CreateASelfieVerificationResponse:
         _response = httpx.request(
             "POST",
             urllib.parse.urljoin(f"{self._environment.value}/", "verification/selfies"),
             json=jsonable_encoder({"data": data}),
             headers=remove_none_from_headers(
-                {"Key-Inflection": key_inflection, "Idempotency-Key": idempotency_key, "Authorization": self.api_key}
+                {
+                    "Key-Inflection": key_inflection,
+                    "Idempotency-Key": idempotency_key,
+                    "Authorization": f"Bearer  {self.api_key}",
+                }
             ),
             timeout=60,
         )
         if 200 <= _response.status_code < 300:
             return pydantic.parse_obj_as(CreateASelfieVerificationResponse, _response.json())  # type: ignore
         if _response.status_code == 400:
             raise BadRequestError(pydantic.parse_obj_as(typing.Any, _response.json()))  # type: ignore
@@ -56,15 +60,19 @@
         key_inflection: typing.Optional[str] = None,
         idempotency_key: typing.Optional[str] = None,
     ) -> SubmitASelfieVerificationResponse:
         _response = httpx.request(
             "POST",
             urllib.parse.urljoin(f"{self._environment.value}/", f"verification/selfies/{verification_id}/submit"),
             headers=remove_none_from_headers(
-                {"Key-Inflection": key_inflection, "Idempotency-Key": idempotency_key, "Authorization": self.api_key}
+                {
+                    "Key-Inflection": key_inflection,
+                    "Idempotency-Key": idempotency_key,
+                    "Authorization": f"Bearer  {self.api_key}",
+                }
             ),
             timeout=60,
         )
         if 200 <= _response.status_code < 300:
             return pydantic.parse_obj_as(SubmitASelfieVerificationResponse, _response.json())  # type: ignore
         if _response.status_code == 400:
             raise BadRequestError(pydantic.parse_obj_as(typing.Any, _response.json()))  # type: ignore
@@ -76,15 +84,17 @@
 
     def retrieve_a_selfie_verification(
         self, verification_id: str, *, key_inflection: typing.Optional[str] = None
     ) -> RetrieveASelfieVerificationResponse:
         _response = httpx.request(
             "GET",
             urllib.parse.urljoin(f"{self._environment.value}/", f"verification/selfies/{verification_id}"),
-            headers=remove_none_from_headers({"Key-Inflection": key_inflection, "Authorization": self.api_key}),
+            headers=remove_none_from_headers(
+                {"Key-Inflection": key_inflection, "Authorization": f"Bearer  {self.api_key}"}
+            ),
             timeout=60,
         )
         if 200 <= _response.status_code < 300:
             return pydantic.parse_obj_as(RetrieveASelfieVerificationResponse, _response.json())  # type: ignore
         if _response.status_code == 400:
             raise BadRequestError(pydantic.parse_obj_as(typing.Any, _response.json()))  # type: ignore
         try:
@@ -111,15 +121,15 @@
                 "POST",
                 urllib.parse.urljoin(f"{self._environment.value}/", "verification/selfies"),
                 json=jsonable_encoder({"data": data}),
                 headers=remove_none_from_headers(
                     {
                         "Key-Inflection": key_inflection,
                         "Idempotency-Key": idempotency_key,
-                        "Authorization": self.api_key,
+                        "Authorization": f"Bearer  {self.api_key}",
                     }
                 ),
                 timeout=60,
             )
         if 200 <= _response.status_code < 300:
             return pydantic.parse_obj_as(CreateASelfieVerificationResponse, _response.json())  # type: ignore
         if _response.status_code == 400:
@@ -141,15 +151,15 @@
             _response = await _client.request(
                 "POST",
                 urllib.parse.urljoin(f"{self._environment.value}/", f"verification/selfies/{verification_id}/submit"),
                 headers=remove_none_from_headers(
                     {
                         "Key-Inflection": key_inflection,
                         "Idempotency-Key": idempotency_key,
-                        "Authorization": self.api_key,
+                        "Authorization": f"Bearer  {self.api_key}",
                     }
                 ),
                 timeout=60,
             )
         if 200 <= _response.status_code < 300:
             return pydantic.parse_obj_as(SubmitASelfieVerificationResponse, _response.json())  # type: ignore
         if _response.status_code == 400:
@@ -163,15 +173,17 @@
     async def retrieve_a_selfie_verification(
         self, verification_id: str, *, key_inflection: typing.Optional[str] = None
     ) -> RetrieveASelfieVerificationResponse:
         async with httpx.AsyncClient() as _client:
             _response = await _client.request(
                 "GET",
                 urllib.parse.urljoin(f"{self._environment.value}/", f"verification/selfies/{verification_id}"),
-                headers=remove_none_from_headers({"Key-Inflection": key_inflection, "Authorization": self.api_key}),
+                headers=remove_none_from_headers(
+                    {"Key-Inflection": key_inflection, "Authorization": f"Bearer  {self.api_key}"}
+                ),
                 timeout=60,
             )
         if 200 <= _response.status_code < 300:
             return pydantic.parse_obj_as(RetrieveASelfieVerificationResponse, _response.json())  # type: ignore
         if _response.status_code == 400:
             raise BadRequestError(pydantic.parse_obj_as(typing.Any, _response.json()))  # type: ignore
         try:
```

### Comparing `fern_persona-0.0.2/src/persona/resources/serpo_database_verifications/client.py` & `fern_persona-0.0.3/src/persona/resources/serpo_database_verifications/client.py`

 * *Files 6% similar despite different names*

```diff
@@ -34,15 +34,15 @@
         _request: typing.Dict[str, typing.Any] = {}
         if attributes is not OMIT:
             _request["attributes"] = attributes
         _response = httpx.request(
             "POST",
             urllib.parse.urljoin(f"{self._environment.value}/", "verification/database-serpros"),
             json=jsonable_encoder(_request),
-            headers=remove_none_from_headers({"Authorization": self.api_key}),
+            headers=remove_none_from_headers({"Authorization": f"Bearer  {self.api_key}"}),
             timeout=60,
         )
         if 200 <= _response.status_code < 300:
             return pydantic.parse_obj_as(CreateASerproDatabaseVerificationResponse, _response.json())  # type: ignore
         if _response.status_code == 400:
             raise BadRequestError(pydantic.parse_obj_as(typing.Any, _response.json()))  # type: ignore
         try:
@@ -60,15 +60,19 @@
     ) -> SubmitASerproDatabaseVerificationResponse:
         _response = httpx.request(
             "POST",
             urllib.parse.urljoin(
                 f"{self._environment.value}/", f"verification/database-serpros/{verification_id}/submit"
             ),
             headers=remove_none_from_headers(
-                {"Key-Inflection": key_inflection, "Idempotency-Key": idempotency_key, "Authorization": self.api_key}
+                {
+                    "Key-Inflection": key_inflection,
+                    "Idempotency-Key": idempotency_key,
+                    "Authorization": f"Bearer  {self.api_key}",
+                }
             ),
             timeout=60,
         )
         if 200 <= _response.status_code < 300:
             return pydantic.parse_obj_as(SubmitASerproDatabaseVerificationResponse, _response.json())  # type: ignore
         if _response.status_code == 400:
             raise BadRequestError(pydantic.parse_obj_as(typing.Any, _response.json()))  # type: ignore
@@ -80,15 +84,17 @@
 
     def retrieve_a_serpro_database_verification(
         self, verification_id: str, *, key_inflection: typing.Optional[str] = None
     ) -> RetrieveASerproDatabaseVerificationResponse:
         _response = httpx.request(
             "GET",
             urllib.parse.urljoin(f"{self._environment.value}/", f"verification/database-serpros/{verification_id}"),
-            headers=remove_none_from_headers({"Key-Inflection": key_inflection, "Authorization": self.api_key}),
+            headers=remove_none_from_headers(
+                {"Key-Inflection": key_inflection, "Authorization": f"Bearer  {self.api_key}"}
+            ),
             timeout=60,
         )
         if 200 <= _response.status_code < 300:
             return pydantic.parse_obj_as(RetrieveASerproDatabaseVerificationResponse, _response.json())  # type: ignore
         if _response.status_code == 400:
             raise BadRequestError(pydantic.parse_obj_as(typing.Any, _response.json()))  # type: ignore
         try:
@@ -110,15 +116,15 @@
         if attributes is not OMIT:
             _request["attributes"] = attributes
         async with httpx.AsyncClient() as _client:
             _response = await _client.request(
                 "POST",
                 urllib.parse.urljoin(f"{self._environment.value}/", "verification/database-serpros"),
                 json=jsonable_encoder(_request),
-                headers=remove_none_from_headers({"Authorization": self.api_key}),
+                headers=remove_none_from_headers({"Authorization": f"Bearer  {self.api_key}"}),
                 timeout=60,
             )
         if 200 <= _response.status_code < 300:
             return pydantic.parse_obj_as(CreateASerproDatabaseVerificationResponse, _response.json())  # type: ignore
         if _response.status_code == 400:
             raise BadRequestError(pydantic.parse_obj_as(typing.Any, _response.json()))  # type: ignore
         try:
@@ -140,15 +146,15 @@
                 urllib.parse.urljoin(
                     f"{self._environment.value}/", f"verification/database-serpros/{verification_id}/submit"
                 ),
                 headers=remove_none_from_headers(
                     {
                         "Key-Inflection": key_inflection,
                         "Idempotency-Key": idempotency_key,
-                        "Authorization": self.api_key,
+                        "Authorization": f"Bearer  {self.api_key}",
                     }
                 ),
                 timeout=60,
             )
         if 200 <= _response.status_code < 300:
             return pydantic.parse_obj_as(SubmitASerproDatabaseVerificationResponse, _response.json())  # type: ignore
         if _response.status_code == 400:
@@ -162,15 +168,17 @@
     async def retrieve_a_serpro_database_verification(
         self, verification_id: str, *, key_inflection: typing.Optional[str] = None
     ) -> RetrieveASerproDatabaseVerificationResponse:
         async with httpx.AsyncClient() as _client:
             _response = await _client.request(
                 "GET",
                 urllib.parse.urljoin(f"{self._environment.value}/", f"verification/database-serpros/{verification_id}"),
-                headers=remove_none_from_headers({"Key-Inflection": key_inflection, "Authorization": self.api_key}),
+                headers=remove_none_from_headers(
+                    {"Key-Inflection": key_inflection, "Authorization": f"Bearer  {self.api_key}"}
+                ),
                 timeout=60,
             )
         if 200 <= _response.status_code < 300:
             return pydantic.parse_obj_as(RetrieveASerproDatabaseVerificationResponse, _response.json())  # type: ignore
         if _response.status_code == 400:
             raise BadRequestError(pydantic.parse_obj_as(typing.Any, _response.json()))  # type: ignore
         try:
```

### Comparing `fern_persona-0.0.2/src/persona/resources/tin_database_verifications/client.py` & `fern_persona-0.0.3/src/persona/resources/tin_database_verifications/client.py`

 * *Files 2% similar despite different names*

```diff
@@ -37,15 +37,19 @@
         if data is not OMIT:
             _request["data"] = data
         _response = httpx.request(
             "POST",
             urllib.parse.urljoin(f"{self._environment.value}/", "verification/database-tins"),
             json=jsonable_encoder(_request),
             headers=remove_none_from_headers(
-                {"Key-Inflection": key_inflection, "Idempotency-Key": idempotency_key, "Authorization": self.api_key}
+                {
+                    "Key-Inflection": key_inflection,
+                    "Idempotency-Key": idempotency_key,
+                    "Authorization": f"Bearer  {self.api_key}",
+                }
             ),
             timeout=60,
         )
         if 200 <= _response.status_code < 300:
             return pydantic.parse_obj_as(CreateATinDatabaseVerificationsResponse, _response.json())  # type: ignore
         if _response.status_code == 400:
             raise BadRequestError(pydantic.parse_obj_as(typing.Any, _response.json()))  # type: ignore
@@ -62,15 +66,19 @@
         key_inflection: typing.Optional[str] = None,
         idempotency_key: typing.Optional[str] = None,
     ) -> SubmitATinDatabaseVerificationsResponse:
         _response = httpx.request(
             "POST",
             urllib.parse.urljoin(f"{self._environment.value}/", f"verification/database-tins/{verification_id}/submit"),
             headers=remove_none_from_headers(
-                {"Key-Inflection": key_inflection, "Idempotency-Key": idempotency_key, "Authorization": self.api_key}
+                {
+                    "Key-Inflection": key_inflection,
+                    "Idempotency-Key": idempotency_key,
+                    "Authorization": f"Bearer  {self.api_key}",
+                }
             ),
             timeout=60,
         )
         if 200 <= _response.status_code < 300:
             return pydantic.parse_obj_as(SubmitATinDatabaseVerificationsResponse, _response.json())  # type: ignore
         if _response.status_code == 400:
             raise BadRequestError(pydantic.parse_obj_as(typing.Any, _response.json()))  # type: ignore
@@ -82,15 +90,17 @@
 
     def retrieve_a_tin_database_verifications(
         self, verification_id: str, *, key_inflection: typing.Optional[str] = None
     ) -> RetrieveATinDatabaseVerificationsResponse:
         _response = httpx.request(
             "GET",
             urllib.parse.urljoin(f"{self._environment.value}/", f"verification/database-tins/{verification_id}"),
-            headers=remove_none_from_headers({"Key-Inflection": key_inflection, "Authorization": self.api_key}),
+            headers=remove_none_from_headers(
+                {"Key-Inflection": key_inflection, "Authorization": f"Bearer  {self.api_key}"}
+            ),
             timeout=60,
         )
         if 200 <= _response.status_code < 300:
             return pydantic.parse_obj_as(RetrieveATinDatabaseVerificationsResponse, _response.json())  # type: ignore
         if _response.status_code == 400:
             raise BadRequestError(pydantic.parse_obj_as(typing.Any, _response.json()))  # type: ignore
         try:
@@ -120,15 +130,15 @@
                 "POST",
                 urllib.parse.urljoin(f"{self._environment.value}/", "verification/database-tins"),
                 json=jsonable_encoder(_request),
                 headers=remove_none_from_headers(
                     {
                         "Key-Inflection": key_inflection,
                         "Idempotency-Key": idempotency_key,
-                        "Authorization": self.api_key,
+                        "Authorization": f"Bearer  {self.api_key}",
                     }
                 ),
                 timeout=60,
             )
         if 200 <= _response.status_code < 300:
             return pydantic.parse_obj_as(CreateATinDatabaseVerificationsResponse, _response.json())  # type: ignore
         if _response.status_code == 400:
@@ -152,15 +162,15 @@
                 urllib.parse.urljoin(
                     f"{self._environment.value}/", f"verification/database-tins/{verification_id}/submit"
                 ),
                 headers=remove_none_from_headers(
                     {
                         "Key-Inflection": key_inflection,
                         "Idempotency-Key": idempotency_key,
-                        "Authorization": self.api_key,
+                        "Authorization": f"Bearer  {self.api_key}",
                     }
                 ),
                 timeout=60,
             )
         if 200 <= _response.status_code < 300:
             return pydantic.parse_obj_as(SubmitATinDatabaseVerificationsResponse, _response.json())  # type: ignore
         if _response.status_code == 400:
@@ -174,15 +184,17 @@
     async def retrieve_a_tin_database_verifications(
         self, verification_id: str, *, key_inflection: typing.Optional[str] = None
     ) -> RetrieveATinDatabaseVerificationsResponse:
         async with httpx.AsyncClient() as _client:
             _response = await _client.request(
                 "GET",
                 urllib.parse.urljoin(f"{self._environment.value}/", f"verification/database-tins/{verification_id}"),
-                headers=remove_none_from_headers({"Key-Inflection": key_inflection, "Authorization": self.api_key}),
+                headers=remove_none_from_headers(
+                    {"Key-Inflection": key_inflection, "Authorization": f"Bearer  {self.api_key}"}
+                ),
                 timeout=60,
             )
         if 200 <= _response.status_code < 300:
             return pydantic.parse_obj_as(RetrieveATinDatabaseVerificationsResponse, _response.json())  # type: ignore
         if _response.status_code == 400:
             raise BadRequestError(pydantic.parse_obj_as(typing.Any, _response.json()))  # type: ignore
         try:
```

### Comparing `fern_persona-0.0.2/src/persona/resources/user_audit_logs/client.py` & `fern_persona-0.0.3/src/persona/resources/user_audit_logs/client.py`

 * *Files 3% similar despite different names*

```diff
@@ -27,15 +27,17 @@
         page_size: typing.Optional[str] = None,
         key_inflection: typing.Optional[str] = None,
     ) -> None:
         _response = httpx.request(
             "GET",
             urllib.parse.urljoin(f"{self._environment.value}/", "user-audit-logs"),
             params={"page[before]": page_before, "page[after]": page_after, "page[size]": page_size},
-            headers=remove_none_from_headers({"Key-Inflection": key_inflection, "Authorization": self.api_key}),
+            headers=remove_none_from_headers(
+                {"Key-Inflection": key_inflection, "Authorization": f"Bearer  {self.api_key}"}
+            ),
             timeout=60,
         )
         if 200 <= _response.status_code < 300:
             return
         try:
             _response_json = _response.json()
         except JSONDecodeError:
@@ -44,15 +46,17 @@
 
     def retrieve_an_user_audit_log(
         self, user_audit_log_id: str, *, key_inflection: typing.Optional[str] = None
     ) -> RetrieveAnUserAuditLogResponse:
         _response = httpx.request(
             "GET",
             urllib.parse.urljoin(f"{self._environment.value}/", f"user-audit-logs/{user_audit_log_id}"),
-            headers=remove_none_from_headers({"Key-Inflection": key_inflection, "Authorization": self.api_key}),
+            headers=remove_none_from_headers(
+                {"Key-Inflection": key_inflection, "Authorization": f"Bearer  {self.api_key}"}
+            ),
             timeout=60,
         )
         if 200 <= _response.status_code < 300:
             return pydantic.parse_obj_as(RetrieveAnUserAuditLogResponse, _response.json())  # type: ignore
         if _response.status_code == 404:
             raise NotFoundError(pydantic.parse_obj_as(typing.Any, _response.json()))  # type: ignore
         try:
@@ -76,15 +80,17 @@
         key_inflection: typing.Optional[str] = None,
     ) -> None:
         async with httpx.AsyncClient() as _client:
             _response = await _client.request(
                 "GET",
                 urllib.parse.urljoin(f"{self._environment.value}/", "user-audit-logs"),
                 params={"page[before]": page_before, "page[after]": page_after, "page[size]": page_size},
-                headers=remove_none_from_headers({"Key-Inflection": key_inflection, "Authorization": self.api_key}),
+                headers=remove_none_from_headers(
+                    {"Key-Inflection": key_inflection, "Authorization": f"Bearer  {self.api_key}"}
+                ),
                 timeout=60,
             )
         if 200 <= _response.status_code < 300:
             return
         try:
             _response_json = _response.json()
         except JSONDecodeError:
@@ -94,15 +100,17 @@
     async def retrieve_an_user_audit_log(
         self, user_audit_log_id: str, *, key_inflection: typing.Optional[str] = None
     ) -> RetrieveAnUserAuditLogResponse:
         async with httpx.AsyncClient() as _client:
             _response = await _client.request(
                 "GET",
                 urllib.parse.urljoin(f"{self._environment.value}/", f"user-audit-logs/{user_audit_log_id}"),
-                headers=remove_none_from_headers({"Key-Inflection": key_inflection, "Authorization": self.api_key}),
+                headers=remove_none_from_headers(
+                    {"Key-Inflection": key_inflection, "Authorization": f"Bearer  {self.api_key}"}
+                ),
                 timeout=60,
             )
         if 200 <= _response.status_code < 300:
             return pydantic.parse_obj_as(RetrieveAnUserAuditLogResponse, _response.json())  # type: ignore
         if _response.status_code == 404:
             raise NotFoundError(pydantic.parse_obj_as(typing.Any, _response.json()))  # type: ignore
         try:
```

### Comparing `fern_persona-0.0.2/src/persona/resources/verifications/client.py` & `fern_persona-0.0.3/src/persona/resources/verifications/client.py`

 * *Files 6% similar despite different names*

```diff
@@ -16,15 +16,17 @@
         self._environment = environment
         self.api_key = api_key
 
     def retrieve_a_verification(self, verification_id: str, *, key_inflection: typing.Optional[str] = None) -> None:
         _response = httpx.request(
             "GET",
             urllib.parse.urljoin(f"{self._environment.value}/", f"verifications/{verification_id}"),
-            headers=remove_none_from_headers({"Key-Inflection": key_inflection, "Authorization": self.api_key}),
+            headers=remove_none_from_headers(
+                {"Key-Inflection": key_inflection, "Authorization": f"Bearer  {self.api_key}"}
+            ),
             timeout=60,
         )
         if 200 <= _response.status_code < 300:
             return
         try:
             _response_json = _response.json()
         except JSONDecodeError:
@@ -40,15 +42,17 @@
     async def retrieve_a_verification(
         self, verification_id: str, *, key_inflection: typing.Optional[str] = None
     ) -> None:
         async with httpx.AsyncClient() as _client:
             _response = await _client.request(
                 "GET",
                 urllib.parse.urljoin(f"{self._environment.value}/", f"verifications/{verification_id}"),
-                headers=remove_none_from_headers({"Key-Inflection": key_inflection, "Authorization": self.api_key}),
+                headers=remove_none_from_headers(
+                    {"Key-Inflection": key_inflection, "Authorization": f"Bearer  {self.api_key}"}
+                ),
                 timeout=60,
             )
         if 200 <= _response.status_code < 300:
             return
         try:
             _response_json = _response.json()
         except JSONDecodeError:
```

### Comparing `fern_persona-0.0.2/src/persona/resources/workflows/client.py` & `fern_persona-0.0.3/src/persona/resources/workflows/client.py`

 * *Files 6% similar despite different names*

```diff
@@ -34,15 +34,17 @@
         _request: typing.Dict[str, typing.Any] = {}
         if data is not OMIT:
             _request["data"] = data
         _response = httpx.request(
             "POST",
             urllib.parse.urljoin(f"{self._environment.value}/", f"workflows/{workflow_id}/trigger"),
             json=jsonable_encoder(_request),
-            headers=remove_none_from_headers({"Key-Inflection": key_inflection, "Authorization": self.api_key}),
+            headers=remove_none_from_headers(
+                {"Key-Inflection": key_inflection, "Authorization": f"Bearer  {self.api_key}"}
+            ),
             timeout=60,
         )
         if 200 <= _response.status_code < 300:
             return pydantic.parse_obj_as(CreateAWorkflowRunResponse, _response.json())  # type: ignore
         if _response.status_code == 400:
             raise BadRequestError(pydantic.parse_obj_as(typing.Any, _response.json()))  # type: ignore
         try:
@@ -68,15 +70,17 @@
         if data is not OMIT:
             _request["data"] = data
         async with httpx.AsyncClient() as _client:
             _response = await _client.request(
                 "POST",
                 urllib.parse.urljoin(f"{self._environment.value}/", f"workflows/{workflow_id}/trigger"),
                 json=jsonable_encoder(_request),
-                headers=remove_none_from_headers({"Key-Inflection": key_inflection, "Authorization": self.api_key}),
+                headers=remove_none_from_headers(
+                    {"Key-Inflection": key_inflection, "Authorization": f"Bearer  {self.api_key}"}
+                ),
                 timeout=60,
             )
         if 200 <= _response.status_code < 300:
             return pydantic.parse_obj_as(CreateAWorkflowRunResponse, _response.json())  # type: ignore
         if _response.status_code == 400:
             raise BadRequestError(pydantic.parse_obj_as(typing.Any, _response.json()))  # type: ignore
         try:
```

### Comparing `fern_persona-0.0.2/src/persona/types/__init__.py` & `fern_persona-0.0.3/src/persona/types/__init__.py`

 * *Files identical despite different names*

### Comparing `fern_persona-0.0.2/src/persona/types/add_a_tag_1_request_meta.py` & `fern_persona-0.0.3/src/persona/types/add_a_tag_1_request_meta.py`

 * *Files identical despite different names*

### Comparing `fern_persona-0.0.2/src/persona/types/add_a_tag_request_meta.py` & `fern_persona-0.0.3/src/persona/types/add_a_tag_request_meta.py`

 * *Files identical despite different names*

### Comparing `fern_persona-0.0.2/src/persona/types/add_persona_objects_request_meta.py` & `fern_persona-0.0.3/src/persona/types/add_persona_objects_request_meta.py`

 * *Files identical despite different names*

### Comparing `fern_persona-0.0.2/src/persona/types/add_persona_objects_response.py` & `fern_persona-0.0.3/src/persona/types/add_persona_objects_response.py`

 * *Files identical despite different names*

### Comparing `fern_persona-0.0.2/src/persona/types/add_persona_objects_response_data.py` & `fern_persona-0.0.3/src/persona/types/add_persona_objects_response_data.py`

 * *Files identical despite different names*

### Comparing `fern_persona-0.0.2/src/persona/types/add_persona_objects_response_data_attributes.py` & `fern_persona-0.0.3/src/persona/types/add_persona_objects_response_data_attributes.py`

 * *Files identical despite different names*

### Comparing `fern_persona-0.0.2/src/persona/types/add_persona_objects_response_data_relationships.py` & `fern_persona-0.0.3/src/persona/types/add_persona_objects_response_data_relationships.py`

 * *Files identical despite different names*

### Comparing `fern_persona-0.0.2/src/persona/types/add_persona_objects_response_data_relationships_accounts.py` & `fern_persona-0.0.3/src/persona/types/add_persona_objects_response_data_relationships_accounts.py`

 * *Files identical despite different names*

### Comparing `fern_persona-0.0.2/src/persona/types/add_persona_objects_response_data_relationships_case_comments.py` & `fern_persona-0.0.3/src/persona/types/add_persona_objects_response_data_relationships_case_comments.py`

 * *Files identical despite different names*

### Comparing `fern_persona-0.0.2/src/persona/types/add_persona_objects_response_data_relationships_case_template.py` & `fern_persona-0.0.3/src/persona/types/add_persona_objects_response_data_relationships_case_template.py`

 * *Files identical despite different names*

### Comparing `fern_persona-0.0.2/src/persona/types/add_persona_objects_response_data_relationships_case_template_data.py` & `fern_persona-0.0.3/src/persona/types/add_persona_objects_response_data_relationships_case_template_data.py`

 * *Files identical despite different names*

### Comparing `fern_persona-0.0.2/src/persona/types/add_persona_objects_response_data_relationships_inquiries.py` & `fern_persona-0.0.3/src/persona/types/add_persona_objects_response_data_relationships_inquiries.py`

 * *Files identical despite different names*

### Comparing `fern_persona-0.0.2/src/persona/types/add_persona_objects_response_data_relationships_inquiries_data_item.py` & `fern_persona-0.0.3/src/persona/types/add_persona_objects_response_data_relationships_inquiries_data_item.py`

 * *Files identical despite different names*

### Comparing `fern_persona-0.0.2/src/persona/types/add_persona_objects_response_data_relationships_reports.py` & `fern_persona-0.0.3/src/persona/types/add_persona_objects_response_data_relationships_reports.py`

 * *Files identical despite different names*

### Comparing `fern_persona-0.0.2/src/persona/types/add_persona_objects_response_data_relationships_reports_data_item.py` & `fern_persona-0.0.3/src/persona/types/add_persona_objects_response_data_relationships_reports_data_item.py`

 * *Files identical despite different names*

### Comparing `fern_persona-0.0.2/src/persona/types/approve_an_inquiry_request_meta.py` & `fern_persona-0.0.3/src/persona/types/approve_an_inquiry_request_meta.py`

 * *Files identical despite different names*

### Comparing `fern_persona-0.0.2/src/persona/types/approve_an_inquiry_response.py` & `fern_persona-0.0.3/src/persona/types/approve_an_inquiry_response.py`

 * *Files identical despite different names*

### Comparing `fern_persona-0.0.2/src/persona/types/approve_an_inquiry_response_data.py` & `fern_persona-0.0.3/src/persona/types/approve_an_inquiry_response_data.py`

 * *Files identical despite different names*

### Comparing `fern_persona-0.0.2/src/persona/types/approve_an_inquiry_response_data_attributes.py` & `fern_persona-0.0.3/src/persona/types/approve_an_inquiry_response_data_attributes.py`

 * *Files identical despite different names*

### Comparing `fern_persona-0.0.2/src/persona/types/approve_an_inquiry_response_data_relationships.py` & `fern_persona-0.0.3/src/persona/types/approve_an_inquiry_response_data_relationships.py`

 * *Files identical despite different names*

### Comparing `fern_persona-0.0.2/src/persona/types/approve_an_inquiry_response_data_relationships_account.py` & `fern_persona-0.0.3/src/persona/types/approve_an_inquiry_response_data_relationships_account.py`

 * *Files identical despite different names*

### Comparing `fern_persona-0.0.2/src/persona/types/approve_an_inquiry_response_data_relationships_account_data.py` & `fern_persona-0.0.3/src/persona/types/approve_an_inquiry_response_data_relationships_account_data.py`

 * *Files identical despite different names*

### Comparing `fern_persona-0.0.2/src/persona/types/approve_an_inquiry_response_data_relationships_reports.py` & `fern_persona-0.0.3/src/persona/types/approve_an_inquiry_response_data_relationships_reports.py`

 * *Files identical despite different names*

### Comparing `fern_persona-0.0.2/src/persona/types/approve_an_inquiry_response_data_relationships_template.py` & `fern_persona-0.0.3/src/persona/types/approve_an_inquiry_response_data_relationships_template.py`

 * *Files identical despite different names*

### Comparing `fern_persona-0.0.2/src/persona/types/approve_an_inquiry_response_data_relationships_template_data.py` & `fern_persona-0.0.3/src/persona/types/approve_an_inquiry_response_data_relationships_template_data.py`

 * *Files identical despite different names*

### Comparing `fern_persona-0.0.2/src/persona/types/approve_an_inquiry_response_data_relationships_verifications.py` & `fern_persona-0.0.3/src/persona/types/approve_an_inquiry_response_data_relationships_verifications.py`

 * *Files identical despite different names*

### Comparing `fern_persona-0.0.2/src/persona/types/approve_an_inquiry_response_data_relationships_verifications_data_item.py` & `fern_persona-0.0.3/src/persona/types/approve_an_inquiry_response_data_relationships_verifications_data_item.py`

 * *Files identical despite different names*

### Comparing `fern_persona-0.0.2/src/persona/types/archive_a_browser_fingerprint_list_item_response.py` & `fern_persona-0.0.3/src/persona/types/archive_a_browser_fingerprint_list_item_response.py`

 * *Files identical despite different names*

### Comparing `fern_persona-0.0.2/src/persona/types/archive_a_browser_fingerprint_list_item_response_data.py` & `fern_persona-0.0.3/src/persona/types/archive_a_browser_fingerprint_list_item_response_data.py`

 * *Files identical despite different names*

### Comparing `fern_persona-0.0.2/src/persona/types/archive_a_browser_fingerprint_list_item_response_data_attributes.py` & `fern_persona-0.0.3/src/persona/types/archive_a_browser_fingerprint_list_item_response_data_attributes.py`

 * *Files identical despite different names*

### Comparing `fern_persona-0.0.2/src/persona/types/archive_a_browser_fingerprint_list_item_response_data_relationships.py` & `fern_persona-0.0.3/src/persona/types/archive_a_browser_fingerprint_list_item_response_data_relationships.py`

 * *Files identical despite different names*

### Comparing `fern_persona-0.0.2/src/persona/types/archive_a_browser_fingerprint_list_item_response_data_relationships_creator.py` & `fern_persona-0.0.3/src/persona/types/archive_a_browser_fingerprint_list_item_response_data_relationships_creator.py`

 * *Files identical despite different names*

### Comparing `fern_persona-0.0.2/src/persona/types/archive_a_geolocation_list_item_response.py` & `fern_persona-0.0.3/src/persona/types/archive_a_geolocation_list_item_response.py`

 * *Files identical despite different names*

### Comparing `fern_persona-0.0.2/src/persona/types/archive_a_geolocation_list_item_response_data.py` & `fern_persona-0.0.3/src/persona/types/archive_a_geolocation_list_item_response_data.py`

 * *Files identical despite different names*

### Comparing `fern_persona-0.0.2/src/persona/types/archive_a_geolocation_list_item_response_data_attributes.py` & `fern_persona-0.0.3/src/persona/types/archive_a_geolocation_list_item_response_data_attributes.py`

 * *Files identical despite different names*

### Comparing `fern_persona-0.0.2/src/persona/types/archive_a_geolocation_list_item_response_data_relationships.py` & `fern_persona-0.0.3/src/persona/types/archive_a_geolocation_list_item_response_data_relationships.py`

 * *Files identical despite different names*

### Comparing `fern_persona-0.0.2/src/persona/types/archive_a_geolocation_list_item_response_data_relationships_creator.py` & `fern_persona-0.0.3/src/persona/types/archive_a_geolocation_list_item_response_data_relationships_creator.py`

 * *Files identical despite different names*

### Comparing `fern_persona-0.0.2/src/persona/types/archive_a_government_id_number_list_item_response.py` & `fern_persona-0.0.3/src/persona/types/archive_a_government_id_number_list_item_response.py`

 * *Files identical despite different names*

### Comparing `fern_persona-0.0.2/src/persona/types/archive_a_government_id_number_list_item_response_data.py` & `fern_persona-0.0.3/src/persona/types/archive_a_government_id_number_list_item_response_data.py`

 * *Files identical despite different names*

### Comparing `fern_persona-0.0.2/src/persona/types/archive_a_government_id_number_list_item_response_data_attributes.py` & `fern_persona-0.0.3/src/persona/types/archive_a_government_id_number_list_item_response_data_attributes.py`

 * *Files identical despite different names*

### Comparing `fern_persona-0.0.2/src/persona/types/archive_a_government_id_number_list_item_response_data_relationships.py` & `fern_persona-0.0.3/src/persona/types/archive_a_government_id_number_list_item_response_data_relationships.py`

 * *Files identical despite different names*

### Comparing `fern_persona-0.0.2/src/persona/types/archive_a_government_id_number_list_item_response_data_relationships_creator.py` & `fern_persona-0.0.3/src/persona/types/archive_a_government_id_number_list_item_response_data_relationships_creator.py`

 * *Files identical despite different names*

### Comparing `fern_persona-0.0.2/src/persona/types/archive_a_list_response.py` & `fern_persona-0.0.3/src/persona/types/archive_a_list_response.py`

 * *Files identical despite different names*

### Comparing `fern_persona-0.0.2/src/persona/types/archive_a_name_list_item_response.py` & `fern_persona-0.0.3/src/persona/types/archive_a_name_list_item_response.py`

 * *Files identical despite different names*

### Comparing `fern_persona-0.0.2/src/persona/types/archive_a_name_list_item_response_data.py` & `fern_persona-0.0.3/src/persona/types/archive_a_name_list_item_response_data.py`

 * *Files identical despite different names*

### Comparing `fern_persona-0.0.2/src/persona/types/archive_a_name_list_item_response_data_attributes.py` & `fern_persona-0.0.3/src/persona/types/archive_a_name_list_item_response_data_attributes.py`

 * *Files identical despite different names*

### Comparing `fern_persona-0.0.2/src/persona/types/archive_a_name_list_item_response_data_relationships.py` & `fern_persona-0.0.3/src/persona/types/archive_a_name_list_item_response_data_relationships.py`

 * *Files identical despite different names*

### Comparing `fern_persona-0.0.2/src/persona/types/archive_a_name_list_item_response_data_relationships_creator.py` & `fern_persona-0.0.3/src/persona/types/archive_a_name_list_item_response_data_relationships_creator.py`

 * *Files identical despite different names*

### Comparing `fern_persona-0.0.2/src/persona/types/archive_an_email_address_list_item_response.py` & `fern_persona-0.0.3/src/persona/types/archive_an_email_address_list_item_response.py`

 * *Files identical despite different names*

### Comparing `fern_persona-0.0.2/src/persona/types/archive_an_email_address_list_item_response_data.py` & `fern_persona-0.0.3/src/persona/types/archive_an_email_address_list_item_response_data.py`

 * *Files identical despite different names*

### Comparing `fern_persona-0.0.2/src/persona/types/archive_an_email_address_list_item_response_data_attributes.py` & `fern_persona-0.0.3/src/persona/types/archive_an_email_address_list_item_response_data_attributes.py`

 * *Files identical despite different names*

### Comparing `fern_persona-0.0.2/src/persona/types/archive_an_email_address_list_item_response_data_relationships.py` & `fern_persona-0.0.3/src/persona/types/archive_an_email_address_list_item_response_data_relationships.py`

 * *Files identical despite different names*

### Comparing `fern_persona-0.0.2/src/persona/types/archive_an_email_address_list_item_response_data_relationships_creator.py` & `fern_persona-0.0.3/src/persona/types/archive_an_email_address_list_item_response_data_relationships_creator.py`

 * *Files identical despite different names*

### Comparing `fern_persona-0.0.2/src/persona/types/assign_a_case_request_meta.py` & `fern_persona-0.0.3/src/persona/types/assign_a_case_request_meta.py`

 * *Files identical despite different names*

### Comparing `fern_persona-0.0.2/src/persona/types/assign_a_case_response.py` & `fern_persona-0.0.3/src/persona/types/assign_a_case_response.py`

 * *Files identical despite different names*

### Comparing `fern_persona-0.0.2/src/persona/types/assign_a_case_response_data.py` & `fern_persona-0.0.3/src/persona/types/assign_a_case_response_data.py`

 * *Files identical despite different names*

### Comparing `fern_persona-0.0.2/src/persona/types/assign_a_case_response_data_attributes.py` & `fern_persona-0.0.3/src/persona/types/assign_a_case_response_data_attributes.py`

 * *Files identical despite different names*

### Comparing `fern_persona-0.0.2/src/persona/types/assign_a_case_response_data_relationships.py` & `fern_persona-0.0.3/src/persona/types/assign_a_case_response_data_relationships.py`

 * *Files identical despite different names*

### Comparing `fern_persona-0.0.2/src/persona/types/assign_a_case_response_data_relationships_accounts.py` & `fern_persona-0.0.3/src/persona/types/assign_a_case_response_data_relationships_accounts.py`

 * *Files identical despite different names*

### Comparing `fern_persona-0.0.2/src/persona/types/assign_a_case_response_data_relationships_case_comments.py` & `fern_persona-0.0.3/src/persona/types/assign_a_case_response_data_relationships_case_comments.py`

 * *Files identical despite different names*

### Comparing `fern_persona-0.0.2/src/persona/types/assign_a_case_response_data_relationships_case_template.py` & `fern_persona-0.0.3/src/persona/types/assign_a_case_response_data_relationships_case_template.py`

 * *Files identical despite different names*

### Comparing `fern_persona-0.0.2/src/persona/types/assign_a_case_response_data_relationships_case_template_data.py` & `fern_persona-0.0.3/src/persona/types/assign_a_case_response_data_relationships_case_template_data.py`

 * *Files identical despite different names*

### Comparing `fern_persona-0.0.2/src/persona/types/assign_a_case_response_data_relationships_inquiries.py` & `fern_persona-0.0.3/src/persona/types/assign_a_case_response_data_relationships_inquiries.py`

 * *Files identical despite different names*

### Comparing `fern_persona-0.0.2/src/persona/types/assign_a_case_response_data_relationships_inquiries_data_item.py` & `fern_persona-0.0.3/src/persona/types/assign_a_case_response_data_relationships_inquiries_data_item.py`

 * *Files identical despite different names*

### Comparing `fern_persona-0.0.2/src/persona/types/assign_a_case_response_data_relationships_reports.py` & `fern_persona-0.0.3/src/persona/types/assign_a_case_response_data_relationships_reports.py`

 * *Files identical despite different names*

### Comparing `fern_persona-0.0.2/src/persona/types/assign_a_case_response_data_relationships_reports_data_item.py` & `fern_persona-0.0.3/src/persona/types/assign_a_case_response_data_relationships_reports_data_item.py`

 * *Files identical despite different names*

### Comparing `fern_persona-0.0.2/src/persona/types/business_lookup_report_1_request_data.py` & `fern_persona-0.0.3/src/persona/types/business_lookup_report_1_request_data.py`

 * *Files identical despite different names*

### Comparing `fern_persona-0.0.2/src/persona/types/business_lookup_report_1_request_data_attributes.py` & `fern_persona-0.0.3/src/persona/types/business_lookup_report_1_request_data_attributes.py`

 * *Files identical despite different names*

### Comparing `fern_persona-0.0.2/src/persona/types/business_lookup_report_1_request_data_attributes_query.py` & `fern_persona-0.0.3/src/persona/types/business_lookup_report_1_request_data_attributes_query.py`

 * *Files identical despite different names*

### Comparing `fern_persona-0.0.2/src/persona/types/business_lookup_report_1_response.py` & `fern_persona-0.0.3/src/persona/types/business_lookup_report_1_response.py`

 * *Files identical despite different names*

### Comparing `fern_persona-0.0.2/src/persona/types/business_lookup_report_1_response_data.py` & `fern_persona-0.0.3/src/persona/types/business_lookup_report_1_response_data.py`

 * *Files identical despite different names*

### Comparing `fern_persona-0.0.2/src/persona/types/business_lookup_report_1_response_data_attributes.py` & `fern_persona-0.0.3/src/persona/types/business_lookup_report_1_response_data_attributes.py`

 * *Files identical despite different names*

### Comparing `fern_persona-0.0.2/src/persona/types/business_lookup_report_1_response_data_attributes_query.py` & `fern_persona-0.0.3/src/persona/types/business_lookup_report_1_response_data_attributes_query.py`

 * *Files identical despite different names*

### Comparing `fern_persona-0.0.2/src/persona/types/business_lookup_report_1_response_data_attributes_result_item.py` & `fern_persona-0.0.3/src/persona/types/business_lookup_report_1_response_data_attributes_result_item.py`

 * *Files identical despite different names*

### Comparing `fern_persona-0.0.2/src/persona/types/business_lookup_report_1_response_data_attributes_result_item_addresses_item.py` & `fern_persona-0.0.3/src/persona/types/business_lookup_report_1_response_data_attributes_result_item_addresses_item.py`

 * *Files identical despite different names*

### Comparing `fern_persona-0.0.2/src/persona/types/business_lookup_report_1_response_data_attributes_result_item_agent.py` & `fern_persona-0.0.3/src/persona/types/business_lookup_report_1_response_data_attributes_result_item_agent.py`

 * *Files identical despite different names*

### Comparing `fern_persona-0.0.2/src/persona/types/business_lookup_report_1_response_data_attributes_result_item_agent_address.py` & `fern_persona-0.0.3/src/persona/types/business_lookup_report_1_response_data_attributes_result_item_agent_address.py`

 * *Files identical despite different names*

### Comparing `fern_persona-0.0.2/src/persona/types/business_lookup_report_1_response_data_attributes_result_item_identifiers_item.py` & `fern_persona-0.0.3/src/persona/types/business_lookup_report_1_response_data_attributes_result_item_identifiers_item.py`

 * *Files identical despite different names*

### Comparing `fern_persona-0.0.2/src/persona/types/business_lookup_report_1_response_data_attributes_result_item_industry_codes_item.py` & `fern_persona-0.0.3/src/persona/types/business_lookup_report_1_response_data_attributes_result_item_industry_codes_item.py`

 * *Files identical despite different names*

### Comparing `fern_persona-0.0.2/src/persona/types/business_lookup_report_1_response_data_attributes_result_item_officers_item.py` & `fern_persona-0.0.3/src/persona/types/business_lookup_report_1_response_data_attributes_result_item_officers_item.py`

 * *Files identical despite different names*

### Comparing `fern_persona-0.0.2/src/persona/types/business_lookup_report_1_response_data_attributes_result_item_officers_item_address.py` & `fern_persona-0.0.3/src/persona/types/business_lookup_report_1_response_data_attributes_result_item_officers_item_address.py`

 * *Files identical despite different names*

### Comparing `fern_persona-0.0.2/src/persona/types/business_lookup_report_1_response_data_attributes_result_item_registration.py` & `fern_persona-0.0.3/src/persona/types/business_lookup_report_1_response_data_attributes_result_item_registration.py`

 * *Files identical despite different names*

### Comparing `fern_persona-0.0.2/src/persona/types/business_lookup_report_1_response_data_attributes_result_item_registration_address.py` & `fern_persona-0.0.3/src/persona/types/business_lookup_report_1_response_data_attributes_result_item_registration_address.py`

 * *Files identical despite different names*

### Comparing `fern_persona-0.0.2/src/persona/types/business_lookup_report_1_response_data_attributes_result_item_source.py` & `fern_persona-0.0.3/src/persona/types/business_lookup_report_1_response_data_attributes_result_item_source.py`

 * *Files identical despite different names*

### Comparing `fern_persona-0.0.2/src/persona/types/confirm_a_phone_number_verification_1_request_data.py` & `fern_persona-0.0.3/src/persona/types/confirm_a_phone_number_verification_1_request_data.py`

 * *Files identical despite different names*

### Comparing `fern_persona-0.0.2/src/persona/types/confirm_a_phone_number_verification_1_request_data_attributes.py` & `fern_persona-0.0.3/src/persona/types/confirm_a_phone_number_verification_1_request_data_attributes.py`

 * *Files identical despite different names*

### Comparing `fern_persona-0.0.2/src/persona/types/confirm_a_phone_number_verification_1_response.py` & `fern_persona-0.0.3/src/persona/types/confirm_a_phone_number_verification_1_response.py`

 * *Files identical despite different names*

### Comparing `fern_persona-0.0.2/src/persona/types/confirm_a_phone_number_verification_1_response_data.py` & `fern_persona-0.0.3/src/persona/types/confirm_a_phone_number_verification_1_response_data.py`

 * *Files identical despite different names*

### Comparing `fern_persona-0.0.2/src/persona/types/confirm_a_phone_number_verification_1_response_data_attributes.py` & `fern_persona-0.0.3/src/persona/types/confirm_a_phone_number_verification_1_response_data_attributes.py`

 * *Files identical despite different names*

### Comparing `fern_persona-0.0.2/src/persona/types/confirm_a_phone_number_verification_1_response_data_attributes_metadata.py` & `fern_persona-0.0.3/src/persona/types/confirm_a_phone_number_verification_1_response_data_attributes_metadata.py`

 * *Files identical despite different names*

### Comparing `fern_persona-0.0.2/src/persona/types/confirm_a_phone_number_verification_request_data.py` & `fern_persona-0.0.3/src/persona/types/confirm_a_phone_number_verification_request_data.py`

 * *Files identical despite different names*

### Comparing `fern_persona-0.0.2/src/persona/types/confirm_a_phone_number_verification_request_data_attributes.py` & `fern_persona-0.0.3/src/persona/types/confirm_a_phone_number_verification_request_data_attributes.py`

 * *Files identical despite different names*

### Comparing `fern_persona-0.0.2/src/persona/types/confirm_a_phone_number_verification_response.py` & `fern_persona-0.0.3/src/persona/types/confirm_a_phone_number_verification_response.py`

 * *Files identical despite different names*

### Comparing `fern_persona-0.0.2/src/persona/types/confirm_a_phone_number_verification_response_data.py` & `fern_persona-0.0.3/src/persona/types/confirm_a_phone_number_verification_response_data.py`

 * *Files identical despite different names*

### Comparing `fern_persona-0.0.2/src/persona/types/confirm_a_phone_number_verification_response_data_attributes.py` & `fern_persona-0.0.3/src/persona/types/confirm_a_phone_number_verification_response_data_attributes.py`

 * *Files identical despite different names*

### Comparing `fern_persona-0.0.2/src/persona/types/confirm_a_phone_number_verification_response_data_attributes_metadata.py` & `fern_persona-0.0.3/src/persona/types/confirm_a_phone_number_verification_response_data_attributes_metadata.py`

 * *Files identical despite different names*

### Comparing `fern_persona-0.0.2/src/persona/types/consolidate_into_an_account_request_meta.py` & `fern_persona-0.0.3/src/persona/types/consolidate_into_an_account_request_meta.py`

 * *Files identical despite different names*

### Comparing `fern_persona-0.0.2/src/persona/types/create_a_browser_fingerprint_list_item_request_data.py` & `fern_persona-0.0.3/src/persona/types/create_a_browser_fingerprint_list_item_request_data.py`

 * *Files identical despite different names*

### Comparing `fern_persona-0.0.2/src/persona/types/create_a_browser_fingerprint_list_item_request_data_attributes.py` & `fern_persona-0.0.3/src/persona/types/create_a_browser_fingerprint_list_item_request_data_attributes.py`

 * *Files identical despite different names*

### Comparing `fern_persona-0.0.2/src/persona/types/create_a_browser_fingerprint_list_item_response.py` & `fern_persona-0.0.3/src/persona/types/create_a_browser_fingerprint_list_item_response.py`

 * *Files identical despite different names*

### Comparing `fern_persona-0.0.2/src/persona/types/create_a_browser_fingerprint_list_item_response_data.py` & `fern_persona-0.0.3/src/persona/types/create_a_browser_fingerprint_list_item_response_data.py`

 * *Files identical despite different names*

### Comparing `fern_persona-0.0.2/src/persona/types/create_a_browser_fingerprint_list_item_response_data_attributes.py` & `fern_persona-0.0.3/src/persona/types/create_a_browser_fingerprint_list_item_response_data_attributes.py`

 * *Files identical despite different names*

### Comparing `fern_persona-0.0.2/src/persona/types/create_a_browser_fingerprint_list_item_response_data_relationships.py` & `fern_persona-0.0.3/src/persona/types/create_a_browser_fingerprint_list_item_response_data_relationships.py`

 * *Files identical despite different names*

### Comparing `fern_persona-0.0.2/src/persona/types/create_a_browser_fingerprint_list_item_response_data_relationships_creator.py` & `fern_persona-0.0.3/src/persona/types/create_a_browser_fingerprint_list_item_response_data_relationships_creator.py`

 * *Files identical despite different names*

### Comparing `fern_persona-0.0.2/src/persona/types/create_a_browser_fingerprint_list_request_data.py` & `fern_persona-0.0.3/src/persona/types/create_a_browser_fingerprint_list_request_data.py`

 * *Files identical despite different names*

### Comparing `fern_persona-0.0.2/src/persona/types/create_a_browser_fingerprint_list_request_data_attributes.py` & `fern_persona-0.0.3/src/persona/types/create_a_browser_fingerprint_list_request_data_attributes.py`

 * *Files identical despite different names*

### Comparing `fern_persona-0.0.2/src/persona/types/create_a_browser_fingerprint_list_response.py` & `fern_persona-0.0.3/src/persona/types/create_a_browser_fingerprint_list_response.py`

 * *Files identical despite different names*

### Comparing `fern_persona-0.0.2/src/persona/types/create_a_case_request_data.py` & `fern_persona-0.0.3/src/persona/types/create_a_case_request_data.py`

 * *Files identical despite different names*

### Comparing `fern_persona-0.0.2/src/persona/types/create_a_case_request_data_attributes.py` & `fern_persona-0.0.3/src/persona/types/create_a_case_request_data_attributes.py`

 * *Files identical despite different names*

### Comparing `fern_persona-0.0.2/src/persona/types/create_a_case_request_meta.py` & `fern_persona-0.0.3/src/persona/types/create_a_case_request_meta.py`

 * *Files identical despite different names*

### Comparing `fern_persona-0.0.2/src/persona/types/create_a_case_response.py` & `fern_persona-0.0.3/src/persona/types/create_a_case_response.py`

 * *Files identical despite different names*

### Comparing `fern_persona-0.0.2/src/persona/types/create_a_case_response_data.py` & `fern_persona-0.0.3/src/persona/types/create_a_case_response_data.py`

 * *Files identical despite different names*

### Comparing `fern_persona-0.0.2/src/persona/types/create_a_case_response_data_attributes.py` & `fern_persona-0.0.3/src/persona/types/create_a_case_response_data_attributes.py`

 * *Files identical despite different names*

### Comparing `fern_persona-0.0.2/src/persona/types/create_a_case_response_data_relationships.py` & `fern_persona-0.0.3/src/persona/types/create_a_case_response_data_relationships.py`

 * *Files identical despite different names*

### Comparing `fern_persona-0.0.2/src/persona/types/create_a_case_response_data_relationships_accounts.py` & `fern_persona-0.0.3/src/persona/types/create_a_case_response_data_relationships_accounts.py`

 * *Files identical despite different names*

### Comparing `fern_persona-0.0.2/src/persona/types/create_a_case_response_data_relationships_case_comments.py` & `fern_persona-0.0.3/src/persona/types/create_a_case_response_data_relationships_case_comments.py`

 * *Files identical despite different names*

### Comparing `fern_persona-0.0.2/src/persona/types/create_a_case_response_data_relationships_case_template.py` & `fern_persona-0.0.3/src/persona/types/create_a_case_response_data_relationships_case_template.py`

 * *Files identical despite different names*

### Comparing `fern_persona-0.0.2/src/persona/types/create_a_case_response_data_relationships_case_template_data.py` & `fern_persona-0.0.3/src/persona/types/create_a_case_response_data_relationships_case_template_data.py`

 * *Files identical despite different names*

### Comparing `fern_persona-0.0.2/src/persona/types/create_a_case_response_data_relationships_inquiries.py` & `fern_persona-0.0.3/src/persona/types/create_a_case_response_data_relationships_inquiries.py`

 * *Files identical despite different names*

### Comparing `fern_persona-0.0.2/src/persona/types/create_a_case_response_data_relationships_inquiries_data_item.py` & `fern_persona-0.0.3/src/persona/types/create_a_case_response_data_relationships_inquiries_data_item.py`

 * *Files identical despite different names*

### Comparing `fern_persona-0.0.2/src/persona/types/create_a_case_response_data_relationships_reports.py` & `fern_persona-0.0.3/src/persona/types/create_a_case_response_data_relationships_reports.py`

 * *Files identical despite different names*

### Comparing `fern_persona-0.0.2/src/persona/types/create_a_case_response_included_item.py` & `fern_persona-0.0.3/src/persona/types/create_a_case_response_included_item.py`

 * *Files identical despite different names*

### Comparing `fern_persona-0.0.2/src/persona/types/create_a_case_response_included_item_attributes.py` & `fern_persona-0.0.3/src/persona/types/create_a_case_response_included_item_attributes.py`

 * *Files identical despite different names*

### Comparing `fern_persona-0.0.2/src/persona/types/create_a_case_response_included_item_attributes_fields.py` & `fern_persona-0.0.3/src/persona/types/create_a_case_response_included_item_attributes_fields.py`

 * *Files identical despite different names*

### Comparing `fern_persona-0.0.2/src/persona/types/create_a_case_response_included_item_relationships.py` & `fern_persona-0.0.3/src/persona/types/create_a_case_response_included_item_relationships.py`

 * *Files identical despite different names*

### Comparing `fern_persona-0.0.2/src/persona/types/create_a_case_response_included_item_relationships_account.py` & `fern_persona-0.0.3/src/persona/types/create_a_case_response_included_item_relationships_account.py`

 * *Files identical despite different names*

### Comparing `fern_persona-0.0.2/src/persona/types/create_a_case_response_included_item_relationships_account_data.py` & `fern_persona-0.0.3/src/persona/types/create_a_case_response_included_item_relationships_account_data.py`

 * *Files identical despite different names*

### Comparing `fern_persona-0.0.2/src/persona/types/create_a_case_response_included_item_relationships_documents.py` & `fern_persona-0.0.3/src/persona/types/create_a_case_response_included_item_relationships_documents.py`

 * *Files identical despite different names*

### Comparing `fern_persona-0.0.2/src/persona/types/create_a_case_response_included_item_relationships_documents_data_item.py` & `fern_persona-0.0.3/src/persona/types/create_a_case_response_included_item_relationships_documents_data_item.py`

 * *Files identical despite different names*

### Comparing `fern_persona-0.0.2/src/persona/types/create_a_case_response_included_item_relationships_inquiry_template_version.py` & `fern_persona-0.0.3/src/persona/types/create_a_case_response_included_item_relationships_inquiry_template_version.py`

 * *Files identical despite different names*

### Comparing `fern_persona-0.0.2/src/persona/types/create_a_case_response_included_item_relationships_reports.py` & `fern_persona-0.0.3/src/persona/types/create_a_case_response_included_item_relationships_reports.py`

 * *Files identical despite different names*

### Comparing `fern_persona-0.0.2/src/persona/types/create_a_case_response_included_item_relationships_selfies.py` & `fern_persona-0.0.3/src/persona/types/create_a_case_response_included_item_relationships_selfies.py`

 * *Files identical despite different names*

### Comparing `fern_persona-0.0.2/src/persona/types/create_a_case_response_included_item_relationships_selfies_data_item.py` & `fern_persona-0.0.3/src/persona/types/create_a_case_response_included_item_relationships_selfies_data_item.py`

 * *Files identical despite different names*

### Comparing `fern_persona-0.0.2/src/persona/types/create_a_case_response_included_item_relationships_sessions.py` & `fern_persona-0.0.3/src/persona/types/create_a_case_response_included_item_relationships_sessions.py`

 * *Files identical despite different names*

### Comparing `fern_persona-0.0.2/src/persona/types/create_a_case_response_included_item_relationships_sessions_data_item.py` & `fern_persona-0.0.3/src/persona/types/create_a_case_response_included_item_relationships_sessions_data_item.py`

 * *Files identical despite different names*

### Comparing `fern_persona-0.0.2/src/persona/types/create_a_case_response_included_item_relationships_template.py` & `fern_persona-0.0.3/src/persona/types/create_a_case_response_included_item_relationships_template.py`

 * *Files identical despite different names*

### Comparing `fern_persona-0.0.2/src/persona/types/create_a_case_response_included_item_relationships_template_data.py` & `fern_persona-0.0.3/src/persona/types/create_a_case_response_included_item_relationships_template_data.py`

 * *Files identical despite different names*

### Comparing `fern_persona-0.0.2/src/persona/types/create_a_case_response_included_item_relationships_verifications.py` & `fern_persona-0.0.3/src/persona/types/create_a_case_response_included_item_relationships_verifications.py`

 * *Files identical despite different names*

### Comparing `fern_persona-0.0.2/src/persona/types/create_a_case_response_included_item_relationships_verifications_data_item.py` & `fern_persona-0.0.3/src/persona/types/create_a_case_response_included_item_relationships_verifications_data_item.py`

 * *Files identical despite different names*

### Comparing `fern_persona-0.0.2/src/persona/types/create_a_country_list_request_data.py` & `fern_persona-0.0.3/src/persona/types/create_a_country_list_request_data.py`

 * *Files identical despite different names*

### Comparing `fern_persona-0.0.2/src/persona/types/create_a_country_list_request_data_attributes.py` & `fern_persona-0.0.3/src/persona/types/create_a_country_list_request_data_attributes.py`

 * *Files identical despite different names*

### Comparing `fern_persona-0.0.2/src/persona/types/create_a_country_list_response.py` & `fern_persona-0.0.3/src/persona/types/create_a_country_list_response.py`

 * *Files identical despite different names*

### Comparing `fern_persona-0.0.2/src/persona/types/create_a_county_list_item_request_data.py` & `fern_persona-0.0.3/src/persona/types/create_a_county_list_item_request_data.py`

 * *Files identical despite different names*

### Comparing `fern_persona-0.0.2/src/persona/types/create_a_county_list_item_request_data_attributes.py` & `fern_persona-0.0.3/src/persona/types/create_a_county_list_item_request_data_attributes.py`

 * *Files identical despite different names*

### Comparing `fern_persona-0.0.2/src/persona/types/create_a_database_verification_1_response.py` & `fern_persona-0.0.3/src/persona/types/create_a_database_verification_1_response.py`

 * *Files identical despite different names*

### Comparing `fern_persona-0.0.2/src/persona/types/create_a_database_verification_1_response_data.py` & `fern_persona-0.0.3/src/persona/types/create_a_database_verification_1_response_data.py`

 * *Files identical despite different names*

### Comparing `fern_persona-0.0.2/src/persona/types/create_a_database_verification_1_response_data_attributes.py` & `fern_persona-0.0.3/src/persona/types/create_a_database_verification_1_response_data_attributes.py`

 * *Files identical despite different names*

### Comparing `fern_persona-0.0.2/src/persona/types/create_a_database_verification_1_response_data_relationships.py` & `fern_persona-0.0.3/src/persona/types/create_a_database_verification_1_response_data_relationships.py`

 * *Files identical despite different names*

### Comparing `fern_persona-0.0.2/src/persona/types/create_a_database_verification_1_response_data_relationships_inquiry.py` & `fern_persona-0.0.3/src/persona/types/create_a_database_verification_1_response_data_relationships_inquiry.py`

 * *Files identical despite different names*

### Comparing `fern_persona-0.0.2/src/persona/types/create_a_database_verification_response.py` & `fern_persona-0.0.3/src/persona/types/create_a_database_verification_response.py`

 * *Files identical despite different names*

### Comparing `fern_persona-0.0.2/src/persona/types/create_a_database_verification_response_data.py` & `fern_persona-0.0.3/src/persona/types/create_a_database_verification_response_data.py`

 * *Files identical despite different names*

### Comparing `fern_persona-0.0.2/src/persona/types/create_a_database_verification_response_data_attributes.py` & `fern_persona-0.0.3/src/persona/types/create_a_database_verification_response_data_attributes.py`

 * *Files identical despite different names*

### Comparing `fern_persona-0.0.2/src/persona/types/create_a_database_verification_response_data_relationships.py` & `fern_persona-0.0.3/src/persona/types/create_a_database_verification_response_data_relationships.py`

 * *Files identical despite different names*

### Comparing `fern_persona-0.0.2/src/persona/types/create_a_database_verification_response_data_relationships_inquiry.py` & `fern_persona-0.0.3/src/persona/types/create_a_database_verification_response_data_relationships_inquiry.py`

 * *Files identical despite different names*

### Comparing `fern_persona-0.0.2/src/persona/types/create_a_document_request_data.py` & `fern_persona-0.0.3/src/persona/types/create_a_document_request_data.py`

 * *Files identical despite different names*

### Comparing `fern_persona-0.0.2/src/persona/types/create_a_document_request_data_attributes.py` & `fern_persona-0.0.3/src/persona/types/create_a_document_request_data_attributes.py`

 * *Files identical despite different names*

### Comparing `fern_persona-0.0.2/src/persona/types/create_a_document_response.py` & `fern_persona-0.0.3/src/persona/types/create_a_document_response.py`

 * *Files identical despite different names*

### Comparing `fern_persona-0.0.2/src/persona/types/create_a_document_response_data.py` & `fern_persona-0.0.3/src/persona/types/create_a_document_response_data.py`

 * *Files identical despite different names*

### Comparing `fern_persona-0.0.2/src/persona/types/create_a_document_response_data_attributes.py` & `fern_persona-0.0.3/src/persona/types/create_a_document_response_data_attributes.py`

 * *Files identical despite different names*

### Comparing `fern_persona-0.0.2/src/persona/types/create_a_document_response_data_attributes_files_item.py` & `fern_persona-0.0.3/src/persona/types/create_a_document_response_data_attributes_files_item.py`

 * *Files identical despite different names*

### Comparing `fern_persona-0.0.2/src/persona/types/create_a_document_response_data_relationships.py` & `fern_persona-0.0.3/src/persona/types/create_a_document_response_data_relationships.py`

 * *Files identical despite different names*

### Comparing `fern_persona-0.0.2/src/persona/types/create_a_document_response_data_relationships_inquiry.py` & `fern_persona-0.0.3/src/persona/types/create_a_document_response_data_relationships_inquiry.py`

 * *Files identical despite different names*

### Comparing `fern_persona-0.0.2/src/persona/types/create_a_document_response_data_relationships_inquiry_data.py` & `fern_persona-0.0.3/src/persona/types/create_a_document_response_data_relationships_inquiry_data.py`

 * *Files identical despite different names*

### Comparing `fern_persona-0.0.2/src/persona/types/create_a_document_verification_request_data.py` & `fern_persona-0.0.3/src/persona/types/create_a_document_verification_request_data.py`

 * *Files identical despite different names*

### Comparing `fern_persona-0.0.2/src/persona/types/create_a_document_verification_request_data_attributes.py` & `fern_persona-0.0.3/src/persona/types/create_a_document_verification_request_data_attributes.py`

 * *Files identical despite different names*

### Comparing `fern_persona-0.0.2/src/persona/types/create_a_document_verification_response.py` & `fern_persona-0.0.3/src/persona/types/create_a_document_verification_response.py`

 * *Files identical despite different names*

### Comparing `fern_persona-0.0.2/src/persona/types/create_a_document_verification_response_data.py` & `fern_persona-0.0.3/src/persona/types/create_a_document_verification_response_data.py`

 * *Files identical despite different names*

### Comparing `fern_persona-0.0.2/src/persona/types/create_a_document_verification_response_data_attributes.py` & `fern_persona-0.0.3/src/persona/types/create_a_document_verification_response_data_attributes.py`

 * *Files identical despite different names*

### Comparing `fern_persona-0.0.2/src/persona/types/create_a_document_verification_response_data_relationships.py` & `fern_persona-0.0.3/src/persona/types/create_a_document_verification_response_data_relationships.py`

 * *Files identical despite different names*

### Comparing `fern_persona-0.0.2/src/persona/types/create_a_document_verification_response_data_relationships_document.py` & `fern_persona-0.0.3/src/persona/types/create_a_document_verification_response_data_relationships_document.py`

 * *Files identical despite different names*

### Comparing `fern_persona-0.0.2/src/persona/types/create_a_document_verification_response_data_relationships_document_data.py` & `fern_persona-0.0.3/src/persona/types/create_a_document_verification_response_data_relationships_document_data.py`

 * *Files identical despite different names*

### Comparing `fern_persona-0.0.2/src/persona/types/create_a_document_verification_response_data_relationships_inquiry.py` & `fern_persona-0.0.3/src/persona/types/create_a_document_verification_response_data_relationships_inquiry.py`

 * *Files identical despite different names*

### Comparing `fern_persona-0.0.2/src/persona/types/create_a_document_verification_response_data_relationships_inquiry_data.py` & `fern_persona-0.0.3/src/persona/types/create_a_document_verification_response_data_relationships_inquiry_data.py`

 * *Files identical despite different names*

### Comparing `fern_persona-0.0.2/src/persona/types/create_a_face_list_item_request_data.py` & `fern_persona-0.0.3/src/persona/types/create_a_face_list_item_request_data.py`

 * *Files identical despite different names*

### Comparing `fern_persona-0.0.2/src/persona/types/create_a_face_list_item_request_data_attributes.py` & `fern_persona-0.0.3/src/persona/types/create_a_face_list_item_request_data_attributes.py`

 * *Files identical despite different names*

### Comparing `fern_persona-0.0.2/src/persona/types/create_a_face_list_item_request_data_attributes_face_photo.py` & `fern_persona-0.0.3/src/persona/types/create_a_face_list_item_request_data_attributes_face_photo.py`

 * *Files identical despite different names*

### Comparing `fern_persona-0.0.2/src/persona/types/create_a_face_list_request_data.py` & `fern_persona-0.0.3/src/persona/types/create_a_face_list_request_data.py`

 * *Files identical despite different names*

### Comparing `fern_persona-0.0.2/src/persona/types/create_a_face_list_request_data_attributes.py` & `fern_persona-0.0.3/src/persona/types/create_a_face_list_request_data_attributes.py`

 * *Files identical despite different names*

### Comparing `fern_persona-0.0.2/src/persona/types/create_a_face_list_response.py` & `fern_persona-0.0.3/src/persona/types/create_a_face_list_response.py`

 * *Files identical despite different names*

### Comparing `fern_persona-0.0.2/src/persona/types/create_a_geolocation_list_item_request_data.py` & `fern_persona-0.0.3/src/persona/types/create_a_geolocation_list_item_request_data.py`

 * *Files identical despite different names*

### Comparing `fern_persona-0.0.2/src/persona/types/create_a_geolocation_list_item_request_data_attributes.py` & `fern_persona-0.0.3/src/persona/types/create_a_geolocation_list_item_request_data_attributes.py`

 * *Files identical despite different names*

### Comparing `fern_persona-0.0.2/src/persona/types/create_a_geolocation_list_item_response.py` & `fern_persona-0.0.3/src/persona/types/create_a_geolocation_list_item_response.py`

 * *Files identical despite different names*

### Comparing `fern_persona-0.0.2/src/persona/types/create_a_geolocation_list_item_response_data.py` & `fern_persona-0.0.3/src/persona/types/create_a_geolocation_list_item_response_data.py`

 * *Files identical despite different names*

### Comparing `fern_persona-0.0.2/src/persona/types/create_a_geolocation_list_item_response_data_attributes.py` & `fern_persona-0.0.3/src/persona/types/create_a_geolocation_list_item_response_data_attributes.py`

 * *Files identical despite different names*

### Comparing `fern_persona-0.0.2/src/persona/types/create_a_geolocation_list_item_response_data_relationships.py` & `fern_persona-0.0.3/src/persona/types/create_a_geolocation_list_item_response_data_relationships.py`

 * *Files identical despite different names*

### Comparing `fern_persona-0.0.2/src/persona/types/create_a_geolocation_list_item_response_data_relationships_creator.py` & `fern_persona-0.0.3/src/persona/types/create_a_geolocation_list_item_response_data_relationships_creator.py`

 * *Files identical despite different names*

### Comparing `fern_persona-0.0.2/src/persona/types/create_a_geolocation_list_request_data.py` & `fern_persona-0.0.3/src/persona/types/create_a_geolocation_list_request_data.py`

 * *Files identical despite different names*

### Comparing `fern_persona-0.0.2/src/persona/types/create_a_geolocation_list_request_data_attributes.py` & `fern_persona-0.0.3/src/persona/types/create_a_geolocation_list_request_data_attributes.py`

 * *Files identical despite different names*

### Comparing `fern_persona-0.0.2/src/persona/types/create_a_geolocation_list_response.py` & `fern_persona-0.0.3/src/persona/types/create_a_geolocation_list_response.py`

 * *Files identical despite different names*

### Comparing `fern_persona-0.0.2/src/persona/types/create_a_gov_id_verification_request_data.py` & `fern_persona-0.0.3/src/persona/types/create_a_gov_id_verification_request_data.py`

 * *Files identical despite different names*

### Comparing `fern_persona-0.0.2/src/persona/types/create_a_gov_id_verification_request_data_attributes.py` & `fern_persona-0.0.3/src/persona/types/create_a_gov_id_verification_request_data_attributes.py`

 * *Files identical despite different names*

### Comparing `fern_persona-0.0.2/src/persona/types/create_a_gov_id_verification_request_data_attributes_back_photo.py` & `fern_persona-0.0.3/src/persona/types/create_a_gov_id_verification_request_data_attributes_back_photo.py`

 * *Files identical despite different names*

### Comparing `fern_persona-0.0.2/src/persona/types/create_a_gov_id_verification_request_data_attributes_back_photo_data.py` & `fern_persona-0.0.3/src/persona/types/create_a_gov_id_verification_request_data_attributes_back_photo_data.py`

 * *Files identical despite different names*

### Comparing `fern_persona-0.0.2/src/persona/types/create_a_gov_id_verification_request_data_attributes_front_photo.py` & `fern_persona-0.0.3/src/persona/types/create_a_gov_id_verification_request_data_attributes_front_photo.py`

 * *Files identical despite different names*

### Comparing `fern_persona-0.0.2/src/persona/types/create_a_gov_id_verification_request_data_attributes_front_photo_data.py` & `fern_persona-0.0.3/src/persona/types/create_a_gov_id_verification_request_data_attributes_front_photo_data.py`

 * *Files identical despite different names*

### Comparing `fern_persona-0.0.2/src/persona/types/create_a_gov_id_verification_response.py` & `fern_persona-0.0.3/src/persona/types/create_a_gov_id_verification_response.py`

 * *Files identical despite different names*

### Comparing `fern_persona-0.0.2/src/persona/types/create_a_gov_id_verification_response_data.py` & `fern_persona-0.0.3/src/persona/types/create_a_gov_id_verification_response_data.py`

 * *Files identical despite different names*

### Comparing `fern_persona-0.0.2/src/persona/types/create_a_gov_id_verification_response_data_attributes.py` & `fern_persona-0.0.3/src/persona/types/create_a_gov_id_verification_response_data_attributes.py`

 * *Files identical despite different names*

### Comparing `fern_persona-0.0.2/src/persona/types/create_a_gov_id_verification_response_data_relationships.py` & `fern_persona-0.0.3/src/persona/types/create_a_gov_id_verification_response_data_relationships.py`

 * *Files identical despite different names*

### Comparing `fern_persona-0.0.2/src/persona/types/create_a_gov_id_verification_response_data_relationships_document.py` & `fern_persona-0.0.3/src/persona/types/create_a_gov_id_verification_response_data_relationships_document.py`

 * *Files identical despite different names*

### Comparing `fern_persona-0.0.2/src/persona/types/create_a_gov_id_verification_response_data_relationships_document_data.py` & `fern_persona-0.0.3/src/persona/types/create_a_gov_id_verification_response_data_relationships_document_data.py`

 * *Files identical despite different names*

### Comparing `fern_persona-0.0.2/src/persona/types/create_a_gov_id_verification_response_data_relationships_inquiry.py` & `fern_persona-0.0.3/src/persona/types/create_a_gov_id_verification_response_data_relationships_inquiry.py`

 * *Files identical despite different names*

### Comparing `fern_persona-0.0.2/src/persona/types/create_a_government_id_document_request_data.py` & `fern_persona-0.0.3/src/persona/types/create_a_government_id_document_request_data.py`

 * *Files identical despite different names*

### Comparing `fern_persona-0.0.2/src/persona/types/create_a_government_id_document_request_data_attributes.py` & `fern_persona-0.0.3/src/persona/types/create_a_government_id_document_request_data_attributes.py`

 * *Files identical despite different names*

### Comparing `fern_persona-0.0.2/src/persona/types/create_a_government_id_document_request_data_attributes_back_photo.py` & `fern_persona-0.0.3/src/persona/types/create_a_government_id_document_request_data_attributes_back_photo.py`

 * *Files identical despite different names*

### Comparing `fern_persona-0.0.2/src/persona/types/create_a_government_id_document_request_data_attributes_back_photo_data.py` & `fern_persona-0.0.3/src/persona/types/create_a_government_id_document_request_data_attributes_back_photo_data.py`

 * *Files identical despite different names*

### Comparing `fern_persona-0.0.2/src/persona/types/create_a_government_id_document_request_data_attributes_front_photo.py` & `fern_persona-0.0.3/src/persona/types/create_a_government_id_document_request_data_attributes_front_photo.py`

 * *Files identical despite different names*

### Comparing `fern_persona-0.0.2/src/persona/types/create_a_government_id_document_request_data_attributes_front_photo_data.py` & `fern_persona-0.0.3/src/persona/types/create_a_government_id_document_request_data_attributes_front_photo_data.py`

 * *Files identical despite different names*

### Comparing `fern_persona-0.0.2/src/persona/types/create_a_government_id_document_response.py` & `fern_persona-0.0.3/src/persona/types/create_a_government_id_document_response.py`

 * *Files identical despite different names*

### Comparing `fern_persona-0.0.2/src/persona/types/create_a_government_id_document_response_data.py` & `fern_persona-0.0.3/src/persona/types/create_a_government_id_document_response_data.py`

 * *Files identical despite different names*

### Comparing `fern_persona-0.0.2/src/persona/types/create_a_government_id_document_response_data_attributes.py` & `fern_persona-0.0.3/src/persona/types/create_a_government_id_document_response_data_attributes.py`

 * *Files identical despite different names*

### Comparing `fern_persona-0.0.2/src/persona/types/create_a_government_id_document_response_data_relationships.py` & `fern_persona-0.0.3/src/persona/types/create_a_government_id_document_response_data_relationships.py`

 * *Files identical despite different names*

### Comparing `fern_persona-0.0.2/src/persona/types/create_a_government_id_document_response_data_relationships_inquiry.py` & `fern_persona-0.0.3/src/persona/types/create_a_government_id_document_response_data_relationships_inquiry.py`

 * *Files identical despite different names*

### Comparing `fern_persona-0.0.2/src/persona/types/create_a_government_id_document_response_data_relationships_inquiry_data.py` & `fern_persona-0.0.3/src/persona/types/create_a_government_id_document_response_data_relationships_inquiry_data.py`

 * *Files identical despite different names*

### Comparing `fern_persona-0.0.2/src/persona/types/create_a_government_id_number_list_item_request_data.py` & `fern_persona-0.0.3/src/persona/types/create_a_government_id_number_list_item_request_data.py`

 * *Files identical despite different names*

### Comparing `fern_persona-0.0.2/src/persona/types/create_a_government_id_number_list_item_request_data_attributes.py` & `fern_persona-0.0.3/src/persona/types/create_a_government_id_number_list_item_request_data_attributes.py`

 * *Files identical despite different names*

### Comparing `fern_persona-0.0.2/src/persona/types/create_a_government_id_number_list_item_response.py` & `fern_persona-0.0.3/src/persona/types/create_a_government_id_number_list_item_response.py`

 * *Files identical despite different names*

### Comparing `fern_persona-0.0.2/src/persona/types/create_a_government_id_number_list_item_response_data.py` & `fern_persona-0.0.3/src/persona/types/create_a_government_id_number_list_item_response_data.py`

 * *Files identical despite different names*

### Comparing `fern_persona-0.0.2/src/persona/types/create_a_government_id_number_list_item_response_data_attributes.py` & `fern_persona-0.0.3/src/persona/types/create_a_government_id_number_list_item_response_data_attributes.py`

 * *Files identical despite different names*

### Comparing `fern_persona-0.0.2/src/persona/types/create_a_government_id_number_list_item_response_data_relationships.py` & `fern_persona-0.0.3/src/persona/types/create_a_government_id_number_list_item_response_data_relationships.py`

 * *Files identical despite different names*

### Comparing `fern_persona-0.0.2/src/persona/types/create_a_government_id_number_list_item_response_data_relationships_creator.py` & `fern_persona-0.0.3/src/persona/types/create_a_government_id_number_list_item_response_data_relationships_creator.py`

 * *Files identical despite different names*

### Comparing `fern_persona-0.0.2/src/persona/types/create_a_government_id_number_list_request_data.py` & `fern_persona-0.0.3/src/persona/types/create_a_government_id_number_list_request_data.py`

 * *Files identical despite different names*

### Comparing `fern_persona-0.0.2/src/persona/types/create_a_government_id_number_list_request_data_attributes.py` & `fern_persona-0.0.3/src/persona/types/create_a_government_id_number_list_request_data_attributes.py`

 * *Files identical despite different names*

### Comparing `fern_persona-0.0.2/src/persona/types/create_a_government_id_number_list_response.py` & `fern_persona-0.0.3/src/persona/types/create_a_government_id_number_list_response.py`

 * *Files identical despite different names*

### Comparing `fern_persona-0.0.2/src/persona/types/create_a_graph_query_request_data.py` & `fern_persona-0.0.3/src/persona/types/create_a_graph_query_request_data.py`

 * *Files identical despite different names*

### Comparing `fern_persona-0.0.2/src/persona/types/create_a_graph_query_request_data_attributes.py` & `fern_persona-0.0.3/src/persona/types/create_a_graph_query_request_data_attributes.py`

 * *Files identical despite different names*

### Comparing `fern_persona-0.0.2/src/persona/types/create_a_graph_query_request_data_attributes_variable_map.py` & `fern_persona-0.0.3/src/persona/types/create_a_graph_query_request_data_attributes_variable_map.py`

 * *Files identical despite different names*

### Comparing `fern_persona-0.0.2/src/persona/types/create_a_name_list_item_request_data.py` & `fern_persona-0.0.3/src/persona/types/create_a_name_list_item_request_data.py`

 * *Files identical despite different names*

### Comparing `fern_persona-0.0.2/src/persona/types/create_a_name_list_item_request_data_attributes.py` & `fern_persona-0.0.3/src/persona/types/create_a_name_list_item_request_data_attributes.py`

 * *Files identical despite different names*

### Comparing `fern_persona-0.0.2/src/persona/types/create_a_name_list_item_response.py` & `fern_persona-0.0.3/src/persona/types/create_a_name_list_item_response.py`

 * *Files identical despite different names*

### Comparing `fern_persona-0.0.2/src/persona/types/create_a_name_list_item_response_data.py` & `fern_persona-0.0.3/src/persona/types/create_a_name_list_item_response_data.py`

 * *Files identical despite different names*

### Comparing `fern_persona-0.0.2/src/persona/types/create_a_name_list_item_response_data_attributes.py` & `fern_persona-0.0.3/src/persona/types/create_a_name_list_item_response_data_attributes.py`

 * *Files identical despite different names*

### Comparing `fern_persona-0.0.2/src/persona/types/create_a_name_list_item_response_data_relationships.py` & `fern_persona-0.0.3/src/persona/types/create_a_name_list_item_response_data_relationships.py`

 * *Files identical despite different names*

### Comparing `fern_persona-0.0.2/src/persona/types/create_a_name_list_item_response_data_relationships_creator.py` & `fern_persona-0.0.3/src/persona/types/create_a_name_list_item_response_data_relationships_creator.py`

 * *Files identical despite different names*

### Comparing `fern_persona-0.0.2/src/persona/types/create_a_name_list_request_data.py` & `fern_persona-0.0.3/src/persona/types/create_a_name_list_request_data.py`

 * *Files identical despite different names*

### Comparing `fern_persona-0.0.2/src/persona/types/create_a_name_list_request_data_attributes.py` & `fern_persona-0.0.3/src/persona/types/create_a_name_list_request_data_attributes.py`

 * *Files identical despite different names*

### Comparing `fern_persona-0.0.2/src/persona/types/create_a_name_list_response.py` & `fern_persona-0.0.3/src/persona/types/create_a_name_list_response.py`

 * *Files identical despite different names*

### Comparing `fern_persona-0.0.2/src/persona/types/create_a_phone_carrier_database_verification_request_attributes.py` & `fern_persona-0.0.3/src/persona/types/create_a_phone_carrier_database_verification_request_attributes.py`

 * *Files identical despite different names*

### Comparing `fern_persona-0.0.2/src/persona/types/create_a_phone_carrier_database_verification_response.py` & `fern_persona-0.0.3/src/persona/types/create_a_phone_carrier_database_verification_response.py`

 * *Files identical despite different names*

### Comparing `fern_persona-0.0.2/src/persona/types/create_a_phone_carrier_database_verification_response_data.py` & `fern_persona-0.0.3/src/persona/types/create_a_phone_carrier_database_verification_response_data.py`

 * *Files identical despite different names*

### Comparing `fern_persona-0.0.2/src/persona/types/create_a_phone_carrier_database_verification_response_data_attributes.py` & `fern_persona-0.0.3/src/persona/types/create_a_phone_carrier_database_verification_response_data_attributes.py`

 * *Files identical despite different names*

### Comparing `fern_persona-0.0.2/src/persona/types/create_a_phone_carrier_database_verification_response_data_relationships.py` & `fern_persona-0.0.3/src/persona/types/create_a_phone_carrier_database_verification_response_data_relationships.py`

 * *Files identical despite different names*

### Comparing `fern_persona-0.0.2/src/persona/types/create_a_phone_carrier_database_verification_response_data_relationships_inquiry.py` & `fern_persona-0.0.3/src/persona/types/create_a_phone_carrier_database_verification_response_data_relationships_inquiry.py`

 * *Files identical despite different names*

### Comparing `fern_persona-0.0.2/src/persona/types/create_a_phone_number_list_item_request_data.py` & `fern_persona-0.0.3/src/persona/types/create_a_phone_number_list_item_request_data.py`

 * *Files identical despite different names*

### Comparing `fern_persona-0.0.2/src/persona/types/create_a_phone_number_list_item_request_data_attributes.py` & `fern_persona-0.0.3/src/persona/types/create_a_phone_number_list_item_request_data_attributes.py`

 * *Files identical despite different names*

### Comparing `fern_persona-0.0.2/src/persona/types/create_a_phone_number_list_request_data.py` & `fern_persona-0.0.3/src/persona/types/create_a_phone_number_list_request_data.py`

 * *Files identical despite different names*

### Comparing `fern_persona-0.0.2/src/persona/types/create_a_phone_number_list_request_data_attributes.py` & `fern_persona-0.0.3/src/persona/types/create_a_phone_number_list_request_data_attributes.py`

 * *Files identical despite different names*

### Comparing `fern_persona-0.0.2/src/persona/types/create_a_phone_number_list_response.py` & `fern_persona-0.0.3/src/persona/types/create_a_phone_number_list_response.py`

 * *Files identical despite different names*

### Comparing `fern_persona-0.0.2/src/persona/types/create_a_phone_number_verification_request_data.py` & `fern_persona-0.0.3/src/persona/types/create_a_phone_number_verification_request_data.py`

 * *Files identical despite different names*

### Comparing `fern_persona-0.0.2/src/persona/types/create_a_phone_number_verification_request_data_attributes.py` & `fern_persona-0.0.3/src/persona/types/create_a_phone_number_verification_request_data_attributes.py`

 * *Files identical despite different names*

### Comparing `fern_persona-0.0.2/src/persona/types/create_a_phone_number_verification_response.py` & `fern_persona-0.0.3/src/persona/types/create_a_phone_number_verification_response.py`

 * *Files identical despite different names*

### Comparing `fern_persona-0.0.2/src/persona/types/create_a_phone_number_verification_response_data.py` & `fern_persona-0.0.3/src/persona/types/create_a_phone_number_verification_response_data.py`

 * *Files identical despite different names*

### Comparing `fern_persona-0.0.2/src/persona/types/create_a_phone_number_verification_response_data_attributes.py` & `fern_persona-0.0.3/src/persona/types/create_a_phone_number_verification_response_data_attributes.py`

 * *Files identical despite different names*

### Comparing `fern_persona-0.0.2/src/persona/types/create_a_phone_number_verification_response_data_attributes_metadata.py` & `fern_persona-0.0.3/src/persona/types/create_a_phone_number_verification_response_data_attributes_metadata.py`

 * *Files identical despite different names*

### Comparing `fern_persona-0.0.2/src/persona/types/create_a_report_request_data.py` & `fern_persona-0.0.3/src/persona/types/create_a_report_request_data.py`

 * *Files identical despite different names*

### Comparing `fern_persona-0.0.2/src/persona/types/create_a_report_request_data_attributes.py` & `fern_persona-0.0.3/src/persona/types/create_a_report_request_data_attributes.py`

 * *Files identical despite different names*

### Comparing `fern_persona-0.0.2/src/persona/types/create_a_selfie_verification_request_data.py` & `fern_persona-0.0.3/src/persona/types/create_a_selfie_verification_request_data.py`

 * *Files identical despite different names*

### Comparing `fern_persona-0.0.2/src/persona/types/create_a_selfie_verification_request_data_attributes.py` & `fern_persona-0.0.3/src/persona/types/create_a_selfie_verification_request_data_attributes.py`

 * *Files identical despite different names*

### Comparing `fern_persona-0.0.2/src/persona/types/create_a_selfie_verification_request_data_attributes_center_photo.py` & `fern_persona-0.0.3/src/persona/types/create_a_selfie_verification_request_data_attributes_center_photo.py`

 * *Files identical despite different names*

### Comparing `fern_persona-0.0.2/src/persona/types/create_a_selfie_verification_request_data_attributes_center_photo_data.py` & `fern_persona-0.0.3/src/persona/types/create_a_selfie_verification_request_data_attributes_center_photo_data.py`

 * *Files identical despite different names*

### Comparing `fern_persona-0.0.2/src/persona/types/create_a_selfie_verification_request_data_attributes_left_photo.py` & `fern_persona-0.0.3/src/persona/types/create_a_selfie_verification_request_data_attributes_left_photo.py`

 * *Files identical despite different names*

### Comparing `fern_persona-0.0.2/src/persona/types/create_a_selfie_verification_request_data_attributes_left_photo_data.py` & `fern_persona-0.0.3/src/persona/types/create_a_selfie_verification_request_data_attributes_left_photo_data.py`

 * *Files identical despite different names*

### Comparing `fern_persona-0.0.2/src/persona/types/create_a_selfie_verification_request_data_attributes_right_photo.py` & `fern_persona-0.0.3/src/persona/types/create_a_selfie_verification_request_data_attributes_right_photo.py`

 * *Files identical despite different names*

### Comparing `fern_persona-0.0.2/src/persona/types/create_a_selfie_verification_request_data_attributes_right_photo_data.py` & `fern_persona-0.0.3/src/persona/types/create_a_selfie_verification_request_data_attributes_right_photo_data.py`

 * *Files identical despite different names*

### Comparing `fern_persona-0.0.2/src/persona/types/create_a_selfie_verification_response.py` & `fern_persona-0.0.3/src/persona/types/create_a_selfie_verification_response.py`

 * *Files identical despite different names*

### Comparing `fern_persona-0.0.2/src/persona/types/create_a_selfie_verification_response_data.py` & `fern_persona-0.0.3/src/persona/types/create_a_selfie_verification_response_data.py`

 * *Files identical despite different names*

### Comparing `fern_persona-0.0.2/src/persona/types/create_a_selfie_verification_response_data_attributes.py` & `fern_persona-0.0.3/src/persona/types/create_a_selfie_verification_response_data_attributes.py`

 * *Files identical despite different names*

### Comparing `fern_persona-0.0.2/src/persona/types/create_a_selfie_verification_response_data_relationships.py` & `fern_persona-0.0.3/src/persona/types/create_a_selfie_verification_response_data_relationships.py`

 * *Files identical despite different names*

### Comparing `fern_persona-0.0.2/src/persona/types/create_a_selfie_verification_response_data_relationships_inquiry.py` & `fern_persona-0.0.3/src/persona/types/create_a_selfie_verification_response_data_relationships_inquiry.py`

 * *Files identical despite different names*

### Comparing `fern_persona-0.0.2/src/persona/types/create_a_serpro_database_verification_request_attributes.py` & `fern_persona-0.0.3/src/persona/types/create_a_serpro_database_verification_request_attributes.py`

 * *Files identical despite different names*

### Comparing `fern_persona-0.0.2/src/persona/types/create_a_serpro_database_verification_response.py` & `fern_persona-0.0.3/src/persona/types/create_a_serpro_database_verification_response.py`

 * *Files identical despite different names*

### Comparing `fern_persona-0.0.2/src/persona/types/create_a_serpro_database_verification_response_data.py` & `fern_persona-0.0.3/src/persona/types/create_a_serpro_database_verification_response_data.py`

 * *Files identical despite different names*

### Comparing `fern_persona-0.0.2/src/persona/types/create_a_serpro_database_verification_response_data_attributes.py` & `fern_persona-0.0.3/src/persona/types/create_a_serpro_database_verification_response_data_attributes.py`

 * *Files identical despite different names*

### Comparing `fern_persona-0.0.2/src/persona/types/create_a_serpro_database_verification_response_data_relationships.py` & `fern_persona-0.0.3/src/persona/types/create_a_serpro_database_verification_response_data_relationships.py`

 * *Files identical despite different names*

### Comparing `fern_persona-0.0.2/src/persona/types/create_a_serpro_database_verification_response_data_relationships_inquiry.py` & `fern_persona-0.0.3/src/persona/types/create_a_serpro_database_verification_response_data_relationships_inquiry.py`

 * *Files identical despite different names*

### Comparing `fern_persona-0.0.2/src/persona/types/create_a_serpro_database_verification_response_data_relationships_selfie.py` & `fern_persona-0.0.3/src/persona/types/create_a_serpro_database_verification_response_data_relationships_selfie.py`

 * *Files identical despite different names*

### Comparing `fern_persona-0.0.2/src/persona/types/create_a_tin_database_verifications_request_data.py` & `fern_persona-0.0.3/src/persona/types/create_a_tin_database_verifications_request_data.py`

 * *Files identical despite different names*

### Comparing `fern_persona-0.0.2/src/persona/types/create_a_tin_database_verifications_request_data_attributes.py` & `fern_persona-0.0.3/src/persona/types/create_a_tin_database_verifications_request_data_attributes.py`

 * *Files identical despite different names*

### Comparing `fern_persona-0.0.2/src/persona/types/create_a_tin_database_verifications_response.py` & `fern_persona-0.0.3/src/persona/types/create_a_tin_database_verifications_response.py`

 * *Files identical despite different names*

### Comparing `fern_persona-0.0.2/src/persona/types/create_a_tin_database_verifications_response_data.py` & `fern_persona-0.0.3/src/persona/types/create_a_tin_database_verifications_response_data.py`

 * *Files identical despite different names*

### Comparing `fern_persona-0.0.2/src/persona/types/create_a_tin_database_verifications_response_data_attributes.py` & `fern_persona-0.0.3/src/persona/types/create_a_tin_database_verifications_response_data_attributes.py`

 * *Files identical despite different names*

### Comparing `fern_persona-0.0.2/src/persona/types/create_a_tin_database_verifications_response_data_relationships.py` & `fern_persona-0.0.3/src/persona/types/create_a_tin_database_verifications_response_data_relationships.py`

 * *Files identical despite different names*

### Comparing `fern_persona-0.0.2/src/persona/types/create_a_tin_database_verifications_response_data_relationships_inquiry.py` & `fern_persona-0.0.3/src/persona/types/create_a_tin_database_verifications_response_data_relationships_inquiry.py`

 * *Files identical despite different names*

### Comparing `fern_persona-0.0.2/src/persona/types/create_a_workflow_run_request_data.py` & `fern_persona-0.0.3/src/persona/types/create_a_workflow_run_request_data.py`

 * *Files identical despite different names*

### Comparing `fern_persona-0.0.2/src/persona/types/create_a_workflow_run_request_data_attributes.py` & `fern_persona-0.0.3/src/persona/types/create_a_workflow_run_request_data_attributes.py`

 * *Files identical despite different names*

### Comparing `fern_persona-0.0.2/src/persona/types/create_a_workflow_run_response.py` & `fern_persona-0.0.3/src/persona/types/create_a_workflow_run_response.py`

 * *Files identical despite different names*

### Comparing `fern_persona-0.0.2/src/persona/types/create_a_workflow_run_response_data.py` & `fern_persona-0.0.3/src/persona/types/create_a_workflow_run_response_data.py`

 * *Files identical despite different names*

### Comparing `fern_persona-0.0.2/src/persona/types/create_a_workflow_run_response_data_attributes.py` & `fern_persona-0.0.3/src/persona/types/create_a_workflow_run_response_data_attributes.py`

 * *Files identical despite different names*

### Comparing `fern_persona-0.0.2/src/persona/types/create_a_workflow_run_response_data_relationships.py` & `fern_persona-0.0.3/src/persona/types/create_a_workflow_run_response_data_relationships.py`

 * *Files identical despite different names*

### Comparing `fern_persona-0.0.2/src/persona/types/create_a_workflow_run_response_data_relationships_creator.py` & `fern_persona-0.0.3/src/persona/types/create_a_workflow_run_response_data_relationships_creator.py`

 * *Files identical despite different names*

### Comparing `fern_persona-0.0.2/src/persona/types/create_a_workflow_run_response_data_relationships_workflow.py` & `fern_persona-0.0.3/src/persona/types/create_a_workflow_run_response_data_relationships_workflow.py`

 * *Files identical despite different names*

### Comparing `fern_persona-0.0.2/src/persona/types/create_a_workflow_run_response_data_relationships_workflow_data.py` & `fern_persona-0.0.3/src/persona/types/create_a_workflow_run_response_data_relationships_workflow_data.py`

 * *Files identical despite different names*

### Comparing `fern_persona-0.0.2/src/persona/types/create_a_workflow_run_response_data_relationships_workflow_version.py` & `fern_persona-0.0.3/src/persona/types/create_a_workflow_run_response_data_relationships_workflow_version.py`

 * *Files identical despite different names*

### Comparing `fern_persona-0.0.2/src/persona/types/create_a_workflow_run_response_data_relationships_workflow_version_data.py` & `fern_persona-0.0.3/src/persona/types/create_a_workflow_run_response_data_relationships_workflow_version_data.py`

 * *Files identical despite different names*

### Comparing `fern_persona-0.0.2/src/persona/types/create_an_account_request_data.py` & `fern_persona-0.0.3/src/persona/types/create_an_account_request_data.py`

 * *Files identical despite different names*

### Comparing `fern_persona-0.0.2/src/persona/types/create_an_account_request_data_attributes.py` & `fern_persona-0.0.3/src/persona/types/create_an_account_request_data_attributes.py`

 * *Files identical despite different names*

### Comparing `fern_persona-0.0.2/src/persona/types/create_an_account_request_data_attributes_selfie_photo.py` & `fern_persona-0.0.3/src/persona/types/create_an_account_request_data_attributes_selfie_photo.py`

 * *Files identical despite different names*

### Comparing `fern_persona-0.0.2/src/persona/types/create_an_account_request_data_attributes_selfie_photo_data.py` & `fern_persona-0.0.3/src/persona/types/create_an_account_request_data_attributes_selfie_photo_data.py`

 * *Files identical despite different names*

### Comparing `fern_persona-0.0.2/src/persona/types/create_an_account_response.py` & `fern_persona-0.0.3/src/persona/types/create_an_account_response.py`

 * *Files identical despite different names*

### Comparing `fern_persona-0.0.2/src/persona/types/create_an_account_response_data.py` & `fern_persona-0.0.3/src/persona/types/create_an_account_response_data.py`

 * *Files identical despite different names*

### Comparing `fern_persona-0.0.2/src/persona/types/create_an_account_response_data_attributes.py` & `fern_persona-0.0.3/src/persona/types/create_an_account_response_data_attributes.py`

 * *Files identical despite different names*

### Comparing `fern_persona-0.0.2/src/persona/types/create_an_api_key_request_data.py` & `fern_persona-0.0.3/src/persona/types/create_an_api_key_request_data.py`

 * *Files identical despite different names*

### Comparing `fern_persona-0.0.2/src/persona/types/create_an_api_key_request_data_attributes.py` & `fern_persona-0.0.3/src/persona/types/create_an_api_key_request_data_attributes.py`

 * *Files identical despite different names*

### Comparing `fern_persona-0.0.2/src/persona/types/create_an_api_key_response.py` & `fern_persona-0.0.3/src/persona/types/create_an_api_key_response.py`

 * *Files identical despite different names*

### Comparing `fern_persona-0.0.2/src/persona/types/create_an_api_key_response_data.py` & `fern_persona-0.0.3/src/persona/types/create_an_api_key_response_data.py`

 * *Files identical despite different names*

### Comparing `fern_persona-0.0.2/src/persona/types/create_an_api_key_response_data_attributes.py` & `fern_persona-0.0.3/src/persona/types/create_an_api_key_response_data_attributes.py`

 * *Files identical despite different names*

### Comparing `fern_persona-0.0.2/src/persona/types/create_an_email_address_list_item_request_data.py` & `fern_persona-0.0.3/src/persona/types/create_an_email_address_list_item_request_data.py`

 * *Files identical despite different names*

### Comparing `fern_persona-0.0.2/src/persona/types/create_an_email_address_list_item_request_data_attributes.py` & `fern_persona-0.0.3/src/persona/types/create_an_email_address_list_item_request_data_attributes.py`

 * *Files identical despite different names*

### Comparing `fern_persona-0.0.2/src/persona/types/create_an_email_address_list_item_response.py` & `fern_persona-0.0.3/src/persona/types/create_an_email_address_list_item_response.py`

 * *Files identical despite different names*

### Comparing `fern_persona-0.0.2/src/persona/types/create_an_email_address_list_item_response_data.py` & `fern_persona-0.0.3/src/persona/types/create_an_email_address_list_item_response_data.py`

 * *Files identical despite different names*

### Comparing `fern_persona-0.0.2/src/persona/types/create_an_email_address_list_item_response_data_attributes.py` & `fern_persona-0.0.3/src/persona/types/create_an_email_address_list_item_response_data_attributes.py`

 * *Files identical despite different names*

### Comparing `fern_persona-0.0.2/src/persona/types/create_an_email_address_list_item_response_data_relationships.py` & `fern_persona-0.0.3/src/persona/types/create_an_email_address_list_item_response_data_relationships.py`

 * *Files identical despite different names*

### Comparing `fern_persona-0.0.2/src/persona/types/create_an_email_address_list_item_response_data_relationships_creator.py` & `fern_persona-0.0.3/src/persona/types/create_an_email_address_list_item_response_data_relationships_creator.py`

 * *Files identical despite different names*

### Comparing `fern_persona-0.0.2/src/persona/types/create_an_email_address_list_request_data.py` & `fern_persona-0.0.3/src/persona/types/create_an_email_address_list_request_data.py`

 * *Files identical despite different names*

### Comparing `fern_persona-0.0.2/src/persona/types/create_an_email_address_list_request_data_attributes.py` & `fern_persona-0.0.3/src/persona/types/create_an_email_address_list_request_data_attributes.py`

 * *Files identical despite different names*

### Comparing `fern_persona-0.0.2/src/persona/types/create_an_email_address_list_response.py` & `fern_persona-0.0.3/src/persona/types/create_an_email_address_list_response.py`

 * *Files identical despite different names*

### Comparing `fern_persona-0.0.2/src/persona/types/create_an_email_address_verification_request_data.py` & `fern_persona-0.0.3/src/persona/types/create_an_email_address_verification_request_data.py`

 * *Files identical despite different names*

### Comparing `fern_persona-0.0.2/src/persona/types/create_an_email_address_verification_request_data_attributes.py` & `fern_persona-0.0.3/src/persona/types/create_an_email_address_verification_request_data_attributes.py`

 * *Files identical despite different names*

### Comparing `fern_persona-0.0.2/src/persona/types/create_an_email_address_verification_response.py` & `fern_persona-0.0.3/src/persona/types/create_an_email_address_verification_response.py`

 * *Files identical despite different names*

### Comparing `fern_persona-0.0.2/src/persona/types/create_an_email_address_verification_response_data.py` & `fern_persona-0.0.3/src/persona/types/create_an_email_address_verification_response_data.py`

 * *Files identical despite different names*

### Comparing `fern_persona-0.0.2/src/persona/types/create_an_email_address_verification_response_data_attributes.py` & `fern_persona-0.0.3/src/persona/types/create_an_email_address_verification_response_data_attributes.py`

 * *Files identical despite different names*

### Comparing `fern_persona-0.0.2/src/persona/types/create_an_email_address_verification_response_data_attributes_metadata.py` & `fern_persona-0.0.3/src/persona/types/create_an_email_address_verification_response_data_attributes_metadata.py`

 * *Files identical despite different names*

### Comparing `fern_persona-0.0.2/src/persona/types/create_an_inquiry_request_data.py` & `fern_persona-0.0.3/src/persona/types/create_an_inquiry_request_data.py`

 * *Files identical despite different names*

### Comparing `fern_persona-0.0.2/src/persona/types/create_an_inquiry_request_data_attributes.py` & `fern_persona-0.0.3/src/persona/types/create_an_inquiry_request_data_attributes.py`

 * *Files identical despite different names*

### Comparing `fern_persona-0.0.2/src/persona/types/create_an_inquiry_request_data_attributes_fields.py` & `fern_persona-0.0.3/src/persona/types/create_an_inquiry_request_data_attributes_fields.py`

 * *Files identical despite different names*

### Comparing `fern_persona-0.0.2/src/persona/types/create_an_inquiry_response.py` & `fern_persona-0.0.3/src/persona/types/create_an_inquiry_response.py`

 * *Files identical despite different names*

### Comparing `fern_persona-0.0.2/src/persona/types/create_an_inquiry_response_data.py` & `fern_persona-0.0.3/src/persona/types/create_an_inquiry_response_data.py`

 * *Files identical despite different names*

### Comparing `fern_persona-0.0.2/src/persona/types/create_an_inquiry_response_data_attributes.py` & `fern_persona-0.0.3/src/persona/types/create_an_inquiry_response_data_attributes.py`

 * *Files identical despite different names*

### Comparing `fern_persona-0.0.2/src/persona/types/create_an_inquiry_response_data_relationships.py` & `fern_persona-0.0.3/src/persona/types/create_an_inquiry_response_data_relationships.py`

 * *Files identical despite different names*

### Comparing `fern_persona-0.0.2/src/persona/types/create_an_inquiry_response_data_relationships_account.py` & `fern_persona-0.0.3/src/persona/types/create_an_inquiry_response_data_relationships_account.py`

 * *Files identical despite different names*

### Comparing `fern_persona-0.0.2/src/persona/types/create_an_inquiry_response_data_relationships_account_data.py` & `fern_persona-0.0.3/src/persona/types/create_an_inquiry_response_data_relationships_account_data.py`

 * *Files identical despite different names*

### Comparing `fern_persona-0.0.2/src/persona/types/create_an_inquiry_response_data_relationships_reports.py` & `fern_persona-0.0.3/src/persona/types/create_an_inquiry_response_data_relationships_reports.py`

 * *Files identical despite different names*

### Comparing `fern_persona-0.0.2/src/persona/types/create_an_inquiry_response_data_relationships_template.py` & `fern_persona-0.0.3/src/persona/types/create_an_inquiry_response_data_relationships_template.py`

 * *Files identical despite different names*

### Comparing `fern_persona-0.0.2/src/persona/types/create_an_inquiry_response_data_relationships_template_data.py` & `fern_persona-0.0.3/src/persona/types/create_an_inquiry_response_data_relationships_template_data.py`

 * *Files identical despite different names*

### Comparing `fern_persona-0.0.2/src/persona/types/create_an_inquiry_response_data_relationships_verifications.py` & `fern_persona-0.0.3/src/persona/types/create_an_inquiry_response_data_relationships_verifications.py`

 * *Files identical despite different names*

### Comparing `fern_persona-0.0.2/src/persona/types/create_an_inquiry_response_data_relationships_verifications_data_item.py` & `fern_persona-0.0.3/src/persona/types/create_an_inquiry_response_data_relationships_verifications_data_item.py`

 * *Files identical despite different names*

### Comparing `fern_persona-0.0.2/src/persona/types/create_an_ip_address_list_item_request_data.py` & `fern_persona-0.0.3/src/persona/types/create_an_ip_address_list_item_request_data.py`

 * *Files identical despite different names*

### Comparing `fern_persona-0.0.2/src/persona/types/create_an_ip_address_list_item_request_data_attributes.py` & `fern_persona-0.0.3/src/persona/types/create_an_ip_address_list_item_request_data_attributes.py`

 * *Files identical despite different names*

### Comparing `fern_persona-0.0.2/src/persona/types/create_an_ip_address_list_request_data.py` & `fern_persona-0.0.3/src/persona/types/create_an_ip_address_list_request_data.py`

 * *Files identical despite different names*

### Comparing `fern_persona-0.0.2/src/persona/types/create_an_ip_address_list_request_data_attributes.py` & `fern_persona-0.0.3/src/persona/types/create_an_ip_address_list_request_data_attributes.py`

 * *Files identical despite different names*

### Comparing `fern_persona-0.0.2/src/persona/types/create_an_ip_address_list_response.py` & `fern_persona-0.0.3/src/persona/types/create_an_ip_address_list_response.py`

 * *Files identical despite different names*

### Comparing `fern_persona-0.0.2/src/persona/types/decline_an_inquiry_request_meta.py` & `fern_persona-0.0.3/src/persona/types/decline_an_inquiry_request_meta.py`

 * *Files identical despite different names*

### Comparing `fern_persona-0.0.2/src/persona/types/decline_an_inquiry_response.py` & `fern_persona-0.0.3/src/persona/types/decline_an_inquiry_response.py`

 * *Files identical despite different names*

### Comparing `fern_persona-0.0.2/src/persona/types/decline_an_inquiry_response_data.py` & `fern_persona-0.0.3/src/persona/types/decline_an_inquiry_response_data.py`

 * *Files identical despite different names*

### Comparing `fern_persona-0.0.2/src/persona/types/decline_an_inquiry_response_data_attributes.py` & `fern_persona-0.0.3/src/persona/types/decline_an_inquiry_response_data_attributes.py`

 * *Files identical despite different names*

### Comparing `fern_persona-0.0.2/src/persona/types/decline_an_inquiry_response_data_relationships.py` & `fern_persona-0.0.3/src/persona/types/decline_an_inquiry_response_data_relationships.py`

 * *Files identical despite different names*

### Comparing `fern_persona-0.0.2/src/persona/types/decline_an_inquiry_response_data_relationships_account.py` & `fern_persona-0.0.3/src/persona/types/decline_an_inquiry_response_data_relationships_account.py`

 * *Files identical despite different names*

### Comparing `fern_persona-0.0.2/src/persona/types/decline_an_inquiry_response_data_relationships_account_data.py` & `fern_persona-0.0.3/src/persona/types/decline_an_inquiry_response_data_relationships_account_data.py`

 * *Files identical despite different names*

### Comparing `fern_persona-0.0.2/src/persona/types/decline_an_inquiry_response_data_relationships_reports.py` & `fern_persona-0.0.3/src/persona/types/decline_an_inquiry_response_data_relationships_reports.py`

 * *Files identical despite different names*

### Comparing `fern_persona-0.0.2/src/persona/types/decline_an_inquiry_response_data_relationships_template.py` & `fern_persona-0.0.3/src/persona/types/decline_an_inquiry_response_data_relationships_template.py`

 * *Files identical despite different names*

### Comparing `fern_persona-0.0.2/src/persona/types/decline_an_inquiry_response_data_relationships_template_data.py` & `fern_persona-0.0.3/src/persona/types/decline_an_inquiry_response_data_relationships_template_data.py`

 * *Files identical despite different names*

### Comparing `fern_persona-0.0.2/src/persona/types/decline_an_inquiry_response_data_relationships_verifications.py` & `fern_persona-0.0.3/src/persona/types/decline_an_inquiry_response_data_relationships_verifications.py`

 * *Files identical despite different names*

### Comparing `fern_persona-0.0.2/src/persona/types/decline_an_inquiry_response_data_relationships_verifications_data_item.py` & `fern_persona-0.0.3/src/persona/types/decline_an_inquiry_response_data_relationships_verifications_data_item.py`

 * *Files identical despite different names*

### Comparing `fern_persona-0.0.2/src/persona/types/dismiss_matches_request_data.py` & `fern_persona-0.0.3/src/persona/types/dismiss_matches_request_data.py`

 * *Files identical despite different names*

### Comparing `fern_persona-0.0.2/src/persona/types/dismiss_matches_request_data_attributes.py` & `fern_persona-0.0.3/src/persona/types/dismiss_matches_request_data_attributes.py`

 * *Files identical despite different names*

### Comparing `fern_persona-0.0.2/src/persona/types/dismiss_matches_request_data_attributes_dismiss_type.py` & `fern_persona-0.0.3/src/persona/types/dismiss_matches_request_data_attributes_dismiss_type.py`

 * *Files identical despite different names*

### Comparing `fern_persona-0.0.2/src/persona/types/dismiss_matches_response.py` & `fern_persona-0.0.3/src/persona/types/dismiss_matches_response.py`

 * *Files identical despite different names*

### Comparing `fern_persona-0.0.2/src/persona/types/dismiss_matches_response_data.py` & `fern_persona-0.0.3/src/persona/types/dismiss_matches_response_data.py`

 * *Files identical despite different names*

### Comparing `fern_persona-0.0.2/src/persona/types/dismiss_matches_response_data_attributes.py` & `fern_persona-0.0.3/src/persona/types/dismiss_matches_response_data_attributes.py`

 * *Files identical despite different names*

### Comparing `fern_persona-0.0.2/src/persona/types/dismiss_matches_response_data_relationships.py` & `fern_persona-0.0.3/src/persona/types/dismiss_matches_response_data_relationships.py`

 * *Files identical despite different names*

### Comparing `fern_persona-0.0.2/src/persona/types/dismiss_matches_response_data_relationships_account.py` & `fern_persona-0.0.3/src/persona/types/dismiss_matches_response_data_relationships_account.py`

 * *Files identical despite different names*

### Comparing `fern_persona-0.0.2/src/persona/types/dismiss_matches_response_data_relationships_inquiry.py` & `fern_persona-0.0.3/src/persona/types/dismiss_matches_response_data_relationships_inquiry.py`

 * *Files identical despite different names*

### Comparing `fern_persona-0.0.2/src/persona/types/dismiss_matches_response_data_relationships_report_template.py` & `fern_persona-0.0.3/src/persona/types/dismiss_matches_response_data_relationships_report_template.py`

 * *Files identical despite different names*

### Comparing `fern_persona-0.0.2/src/persona/types/dismiss_matches_response_data_relationships_report_template_data.py` & `fern_persona-0.0.3/src/persona/types/dismiss_matches_response_data_relationships_report_template_data.py`

 * *Files identical despite different names*

### Comparing `fern_persona-0.0.2/src/persona/types/expire_an_api_key_request_meta.py` & `fern_persona-0.0.3/src/persona/types/expire_an_api_key_request_meta.py`

 * *Files identical despite different names*

### Comparing `fern_persona-0.0.2/src/persona/types/expire_an_api_key_response.py` & `fern_persona-0.0.3/src/persona/types/expire_an_api_key_response.py`

 * *Files identical despite different names*

### Comparing `fern_persona-0.0.2/src/persona/types/expire_an_api_key_response_data.py` & `fern_persona-0.0.3/src/persona/types/expire_an_api_key_response_data.py`

 * *Files identical despite different names*

### Comparing `fern_persona-0.0.2/src/persona/types/expire_an_api_key_response_data_attributes.py` & `fern_persona-0.0.3/src/persona/types/expire_an_api_key_response_data_attributes.py`

 * *Files identical despite different names*

### Comparing `fern_persona-0.0.2/src/persona/types/expire_an_inquiry_response.py` & `fern_persona-0.0.3/src/persona/types/expire_an_inquiry_response.py`

 * *Files identical despite different names*

### Comparing `fern_persona-0.0.2/src/persona/types/expire_an_inquiry_response_data.py` & `fern_persona-0.0.3/src/persona/types/expire_an_inquiry_response_data.py`

 * *Files identical despite different names*

### Comparing `fern_persona-0.0.2/src/persona/types/expire_an_inquiry_response_data_attributes.py` & `fern_persona-0.0.3/src/persona/types/expire_an_inquiry_response_data_attributes.py`

 * *Files identical despite different names*

### Comparing `fern_persona-0.0.2/src/persona/types/expire_an_inquiry_response_data_relationships.py` & `fern_persona-0.0.3/src/persona/types/expire_an_inquiry_response_data_relationships.py`

 * *Files identical despite different names*

### Comparing `fern_persona-0.0.2/src/persona/types/expire_an_inquiry_response_data_relationships_account.py` & `fern_persona-0.0.3/src/persona/types/expire_an_inquiry_response_data_relationships_account.py`

 * *Files identical despite different names*

### Comparing `fern_persona-0.0.2/src/persona/types/expire_an_inquiry_response_data_relationships_account_data.py` & `fern_persona-0.0.3/src/persona/types/expire_an_inquiry_response_data_relationships_account_data.py`

 * *Files identical despite different names*

### Comparing `fern_persona-0.0.2/src/persona/types/expire_an_inquiry_response_data_relationships_reports.py` & `fern_persona-0.0.3/src/persona/types/expire_an_inquiry_response_data_relationships_reports.py`

 * *Files identical despite different names*

### Comparing `fern_persona-0.0.2/src/persona/types/expire_an_inquiry_response_data_relationships_template.py` & `fern_persona-0.0.3/src/persona/types/expire_an_inquiry_response_data_relationships_template.py`

 * *Files identical despite different names*

### Comparing `fern_persona-0.0.2/src/persona/types/expire_an_inquiry_response_data_relationships_template_data.py` & `fern_persona-0.0.3/src/persona/types/expire_an_inquiry_response_data_relationships_template_data.py`

 * *Files identical despite different names*

### Comparing `fern_persona-0.0.2/src/persona/types/expire_an_inquiry_response_data_relationships_verifications.py` & `fern_persona-0.0.3/src/persona/types/expire_an_inquiry_response_data_relationships_verifications.py`

 * *Files identical despite different names*

### Comparing `fern_persona-0.0.2/src/persona/types/expire_an_inquiry_response_data_relationships_verifications_data_item.py` & `fern_persona-0.0.3/src/persona/types/expire_an_inquiry_response_data_relationships_verifications_data_item.py`

 * *Files identical despite different names*

### Comparing `fern_persona-0.0.2/src/persona/types/generate_a_one_time_link_request_meta.py` & `fern_persona-0.0.3/src/persona/types/generate_a_one_time_link_request_meta.py`

 * *Files identical despite different names*

### Comparing `fern_persona-0.0.2/src/persona/types/generate_a_one_time_link_response.py` & `fern_persona-0.0.3/src/persona/types/generate_a_one_time_link_response.py`

 * *Files identical despite different names*

### Comparing `fern_persona-0.0.2/src/persona/types/generate_a_one_time_link_response_data.py` & `fern_persona-0.0.3/src/persona/types/generate_a_one_time_link_response_data.py`

 * *Files identical despite different names*

### Comparing `fern_persona-0.0.2/src/persona/types/generate_a_one_time_link_response_data_attributes.py` & `fern_persona-0.0.3/src/persona/types/generate_a_one_time_link_response_data_attributes.py`

 * *Files identical despite different names*

### Comparing `fern_persona-0.0.2/src/persona/types/generate_a_one_time_link_response_data_attributes_behaviors.py` & `fern_persona-0.0.3/src/persona/types/generate_a_one_time_link_response_data_attributes_behaviors.py`

 * *Files identical despite different names*

### Comparing `fern_persona-0.0.2/src/persona/types/generate_a_one_time_link_response_data_attributes_fields.py` & `fern_persona-0.0.3/src/persona/types/generate_a_one_time_link_response_data_attributes_fields.py`

 * *Files identical despite different names*

### Comparing `fern_persona-0.0.2/src/persona/types/generate_a_one_time_link_response_data_attributes_fields_address_city.py` & `fern_persona-0.0.3/src/persona/types/generate_a_one_time_link_response_data_attributes_fields_address_city.py`

 * *Files identical despite different names*

### Comparing `fern_persona-0.0.2/src/persona/types/generate_a_one_time_link_response_data_attributes_fields_address_postal_code.py` & `fern_persona-0.0.3/src/persona/types/generate_a_one_time_link_response_data_attributes_fields_address_postal_code.py`

 * *Files identical despite different names*

### Comparing `fern_persona-0.0.2/src/persona/types/generate_a_one_time_link_response_data_attributes_fields_address_street_1.py` & `fern_persona-0.0.3/src/persona/types/generate_a_one_time_link_response_data_attributes_fields_address_street_1.py`

 * *Files identical despite different names*

### Comparing `fern_persona-0.0.2/src/persona/types/generate_a_one_time_link_response_data_attributes_fields_address_street_2.py` & `fern_persona-0.0.3/src/persona/types/generate_a_one_time_link_response_data_attributes_fields_address_street_2.py`

 * *Files identical despite different names*

### Comparing `fern_persona-0.0.2/src/persona/types/generate_a_one_time_link_response_data_attributes_fields_address_subdivision.py` & `fern_persona-0.0.3/src/persona/types/generate_a_one_time_link_response_data_attributes_fields_address_subdivision.py`

 * *Files identical despite different names*

### Comparing `fern_persona-0.0.2/src/persona/types/generate_a_one_time_link_response_data_attributes_fields_birthdate.py` & `fern_persona-0.0.3/src/persona/types/generate_a_one_time_link_response_data_attributes_fields_birthdate.py`

 * *Files identical despite different names*

### Comparing `fern_persona-0.0.2/src/persona/types/generate_a_one_time_link_response_data_attributes_fields_email_address.py` & `fern_persona-0.0.3/src/persona/types/generate_a_one_time_link_response_data_attributes_fields_email_address.py`

 * *Files identical despite different names*

### Comparing `fern_persona-0.0.2/src/persona/types/generate_a_one_time_link_response_data_attributes_fields_identification_number.py` & `fern_persona-0.0.3/src/persona/types/generate_a_one_time_link_response_data_attributes_fields_identification_number.py`

 * *Files identical despite different names*

### Comparing `fern_persona-0.0.2/src/persona/types/generate_a_one_time_link_response_data_attributes_fields_name_first.py` & `fern_persona-0.0.3/src/persona/types/generate_a_one_time_link_response_data_attributes_fields_name_first.py`

 * *Files identical despite different names*

### Comparing `fern_persona-0.0.2/src/persona/types/generate_a_one_time_link_response_data_attributes_fields_name_last.py` & `fern_persona-0.0.3/src/persona/types/generate_a_one_time_link_response_data_attributes_fields_name_last.py`

 * *Files identical despite different names*

### Comparing `fern_persona-0.0.2/src/persona/types/generate_a_one_time_link_response_data_attributes_fields_name_middle.py` & `fern_persona-0.0.3/src/persona/types/generate_a_one_time_link_response_data_attributes_fields_name_middle.py`

 * *Files identical despite different names*

### Comparing `fern_persona-0.0.2/src/persona/types/generate_a_one_time_link_response_data_attributes_fields_phone_number.py` & `fern_persona-0.0.3/src/persona/types/generate_a_one_time_link_response_data_attributes_fields_phone_number.py`

 * *Files identical despite different names*

### Comparing `fern_persona-0.0.2/src/persona/types/generate_a_one_time_link_response_data_relationships.py` & `fern_persona-0.0.3/src/persona/types/generate_a_one_time_link_response_data_relationships.py`

 * *Files identical despite different names*

### Comparing `fern_persona-0.0.2/src/persona/types/generate_a_one_time_link_response_data_relationships_account.py` & `fern_persona-0.0.3/src/persona/types/generate_a_one_time_link_response_data_relationships_account.py`

 * *Files identical despite different names*

### Comparing `fern_persona-0.0.2/src/persona/types/generate_a_one_time_link_response_data_relationships_account_data.py` & `fern_persona-0.0.3/src/persona/types/generate_a_one_time_link_response_data_relationships_account_data.py`

 * *Files identical despite different names*

### Comparing `fern_persona-0.0.2/src/persona/types/generate_a_one_time_link_response_data_relationships_documents.py` & `fern_persona-0.0.3/src/persona/types/generate_a_one_time_link_response_data_relationships_documents.py`

 * *Files identical despite different names*

### Comparing `fern_persona-0.0.2/src/persona/types/generate_a_one_time_link_response_data_relationships_documents_data_item.py` & `fern_persona-0.0.3/src/persona/types/generate_a_one_time_link_response_data_relationships_documents_data_item.py`

 * *Files identical despite different names*

### Comparing `fern_persona-0.0.2/src/persona/types/generate_a_one_time_link_response_data_relationships_inquiry_template.py` & `fern_persona-0.0.3/src/persona/types/generate_a_one_time_link_response_data_relationships_inquiry_template.py`

 * *Files identical despite different names*

### Comparing `fern_persona-0.0.2/src/persona/types/generate_a_one_time_link_response_data_relationships_inquiry_template_data.py` & `fern_persona-0.0.3/src/persona/types/generate_a_one_time_link_response_data_relationships_inquiry_template_data.py`

 * *Files identical despite different names*

### Comparing `fern_persona-0.0.2/src/persona/types/generate_a_one_time_link_response_data_relationships_inquiry_template_version.py` & `fern_persona-0.0.3/src/persona/types/generate_a_one_time_link_response_data_relationships_inquiry_template_version.py`

 * *Files identical despite different names*

### Comparing `fern_persona-0.0.2/src/persona/types/generate_a_one_time_link_response_data_relationships_inquiry_template_version_data.py` & `fern_persona-0.0.3/src/persona/types/generate_a_one_time_link_response_data_relationships_inquiry_template_version_data.py`

 * *Files identical despite different names*

### Comparing `fern_persona-0.0.2/src/persona/types/generate_a_one_time_link_response_data_relationships_reports.py` & `fern_persona-0.0.3/src/persona/types/generate_a_one_time_link_response_data_relationships_reports.py`

 * *Files identical despite different names*

### Comparing `fern_persona-0.0.2/src/persona/types/generate_a_one_time_link_response_data_relationships_reviewer.py` & `fern_persona-0.0.3/src/persona/types/generate_a_one_time_link_response_data_relationships_reviewer.py`

 * *Files identical despite different names*

### Comparing `fern_persona-0.0.2/src/persona/types/generate_a_one_time_link_response_data_relationships_selfies.py` & `fern_persona-0.0.3/src/persona/types/generate_a_one_time_link_response_data_relationships_selfies.py`

 * *Files identical despite different names*

### Comparing `fern_persona-0.0.2/src/persona/types/generate_a_one_time_link_response_data_relationships_sessions.py` & `fern_persona-0.0.3/src/persona/types/generate_a_one_time_link_response_data_relationships_sessions.py`

 * *Files identical despite different names*

### Comparing `fern_persona-0.0.2/src/persona/types/generate_a_one_time_link_response_data_relationships_sessions_data_item.py` & `fern_persona-0.0.3/src/persona/types/generate_a_one_time_link_response_data_relationships_sessions_data_item.py`

 * *Files identical despite different names*

### Comparing `fern_persona-0.0.2/src/persona/types/generate_a_one_time_link_response_data_relationships_template.py` & `fern_persona-0.0.3/src/persona/types/generate_a_one_time_link_response_data_relationships_template.py`

 * *Files identical despite different names*

### Comparing `fern_persona-0.0.2/src/persona/types/generate_a_one_time_link_response_data_relationships_verifications.py` & `fern_persona-0.0.3/src/persona/types/generate_a_one_time_link_response_data_relationships_verifications.py`

 * *Files identical despite different names*

### Comparing `fern_persona-0.0.2/src/persona/types/generate_a_one_time_link_response_data_relationships_verifications_data_item.py` & `fern_persona-0.0.3/src/persona/types/generate_a_one_time_link_response_data_relationships_verifications_data_item.py`

 * *Files identical despite different names*

### Comparing `fern_persona-0.0.2/src/persona/types/generate_a_one_time_link_response_meta.py` & `fern_persona-0.0.3/src/persona/types/generate_a_one_time_link_response_meta.py`

 * *Files identical despite different names*

### Comparing `fern_persona-0.0.2/src/persona/types/import_an_account_request_data.py` & `fern_persona-0.0.3/src/persona/types/import_an_account_request_data.py`

 * *Files identical despite different names*

### Comparing `fern_persona-0.0.2/src/persona/types/import_an_account_request_data_file.py` & `fern_persona-0.0.3/src/persona/types/import_an_account_request_data_file.py`

 * *Files identical despite different names*

### Comparing `fern_persona-0.0.2/src/persona/types/import_an_account_response.py` & `fern_persona-0.0.3/src/persona/types/import_an_account_response.py`

 * *Files identical despite different names*

### Comparing `fern_persona-0.0.2/src/persona/types/import_an_account_response_data.py` & `fern_persona-0.0.3/src/persona/types/import_an_account_response_data.py`

 * *Files identical despite different names*

### Comparing `fern_persona-0.0.2/src/persona/types/import_an_account_response_data_attributes.py` & `fern_persona-0.0.3/src/persona/types/import_an_account_response_data_attributes.py`

 * *Files identical despite different names*

### Comparing `fern_persona-0.0.2/src/persona/types/import_email_address_lists_request_data.py` & `fern_persona-0.0.3/src/persona/types/import_email_address_lists_request_data.py`

 * *Files identical despite different names*

### Comparing `fern_persona-0.0.2/src/persona/types/import_email_address_lists_request_data_attributes.py` & `fern_persona-0.0.3/src/persona/types/import_email_address_lists_request_data_attributes.py`

 * *Files identical despite different names*

### Comparing `fern_persona-0.0.2/src/persona/types/import_email_address_lists_request_data_attributes_file.py` & `fern_persona-0.0.3/src/persona/types/import_email_address_lists_request_data_attributes_file.py`

 * *Files identical despite different names*

### Comparing `fern_persona-0.0.2/src/persona/types/import_email_address_lists_response.py` & `fern_persona-0.0.3/src/persona/types/import_email_address_lists_response.py`

 * *Files identical despite different names*

### Comparing `fern_persona-0.0.2/src/persona/types/import_email_address_lists_response_data.py` & `fern_persona-0.0.3/src/persona/types/import_email_address_lists_response_data.py`

 * *Files identical despite different names*

### Comparing `fern_persona-0.0.2/src/persona/types/import_email_address_lists_response_data_attributes.py` & `fern_persona-0.0.3/src/persona/types/import_email_address_lists_response_data_attributes.py`

 * *Files identical despite different names*

### Comparing `fern_persona-0.0.2/src/persona/types/import_face_lists_request_data.py` & `fern_persona-0.0.3/src/persona/types/import_face_lists_request_data.py`

 * *Files identical despite different names*

### Comparing `fern_persona-0.0.2/src/persona/types/import_face_lists_request_data_attributes.py` & `fern_persona-0.0.3/src/persona/types/import_face_lists_request_data_attributes.py`

 * *Files identical despite different names*

### Comparing `fern_persona-0.0.2/src/persona/types/import_face_lists_request_data_attributes_image_files_item.py` & `fern_persona-0.0.3/src/persona/types/import_face_lists_request_data_attributes_image_files_item.py`

 * *Files identical despite different names*

### Comparing `fern_persona-0.0.2/src/persona/types/import_face_lists_response.py` & `fern_persona-0.0.3/src/persona/types/import_face_lists_response.py`

 * *Files identical despite different names*

### Comparing `fern_persona-0.0.2/src/persona/types/import_face_lists_response_data.py` & `fern_persona-0.0.3/src/persona/types/import_face_lists_response_data.py`

 * *Files identical despite different names*

### Comparing `fern_persona-0.0.2/src/persona/types/import_face_lists_response_data_attributes.py` & `fern_persona-0.0.3/src/persona/types/import_face_lists_response_data_attributes.py`

 * *Files identical despite different names*

### Comparing `fern_persona-0.0.2/src/persona/types/import_geolocation_lists_request_data.py` & `fern_persona-0.0.3/src/persona/types/import_geolocation_lists_request_data.py`

 * *Files identical despite different names*

### Comparing `fern_persona-0.0.2/src/persona/types/import_geolocation_lists_request_data_attributes.py` & `fern_persona-0.0.3/src/persona/types/import_geolocation_lists_request_data_attributes.py`

 * *Files identical despite different names*

### Comparing `fern_persona-0.0.2/src/persona/types/import_geolocation_lists_request_data_attributes_file.py` & `fern_persona-0.0.3/src/persona/types/import_geolocation_lists_request_data_attributes_file.py`

 * *Files identical despite different names*

### Comparing `fern_persona-0.0.2/src/persona/types/import_geolocation_lists_response.py` & `fern_persona-0.0.3/src/persona/types/import_geolocation_lists_response.py`

 * *Files identical despite different names*

### Comparing `fern_persona-0.0.2/src/persona/types/import_geolocation_lists_response_data.py` & `fern_persona-0.0.3/src/persona/types/import_geolocation_lists_response_data.py`

 * *Files identical despite different names*

### Comparing `fern_persona-0.0.2/src/persona/types/import_geolocation_lists_response_data_attributes.py` & `fern_persona-0.0.3/src/persona/types/import_geolocation_lists_response_data_attributes.py`

 * *Files identical despite different names*

### Comparing `fern_persona-0.0.2/src/persona/types/import_government_id_number_lists_request_data.py` & `fern_persona-0.0.3/src/persona/types/import_government_id_number_lists_request_data.py`

 * *Files identical despite different names*

### Comparing `fern_persona-0.0.2/src/persona/types/import_government_id_number_lists_request_data_attributes.py` & `fern_persona-0.0.3/src/persona/types/import_government_id_number_lists_request_data_attributes.py`

 * *Files identical despite different names*

### Comparing `fern_persona-0.0.2/src/persona/types/import_government_id_number_lists_request_data_attributes_file.py` & `fern_persona-0.0.3/src/persona/types/import_government_id_number_lists_request_data_attributes_file.py`

 * *Files identical despite different names*

### Comparing `fern_persona-0.0.2/src/persona/types/import_government_id_number_lists_response.py` & `fern_persona-0.0.3/src/persona/types/import_government_id_number_lists_response.py`

 * *Files identical despite different names*

### Comparing `fern_persona-0.0.2/src/persona/types/import_government_id_number_lists_response_data.py` & `fern_persona-0.0.3/src/persona/types/import_government_id_number_lists_response_data.py`

 * *Files identical despite different names*

### Comparing `fern_persona-0.0.2/src/persona/types/import_government_id_number_lists_response_data_attributes.py` & `fern_persona-0.0.3/src/persona/types/import_government_id_number_lists_response_data_attributes.py`

 * *Files identical despite different names*

### Comparing `fern_persona-0.0.2/src/persona/types/import_ip_address_lists_request_data.py` & `fern_persona-0.0.3/src/persona/types/import_ip_address_lists_request_data.py`

 * *Files identical despite different names*

### Comparing `fern_persona-0.0.2/src/persona/types/import_ip_address_lists_request_data_attributes.py` & `fern_persona-0.0.3/src/persona/types/import_ip_address_lists_request_data_attributes.py`

 * *Files identical despite different names*

### Comparing `fern_persona-0.0.2/src/persona/types/import_ip_address_lists_request_data_attributes_file.py` & `fern_persona-0.0.3/src/persona/types/import_ip_address_lists_request_data_attributes_file.py`

 * *Files identical despite different names*

### Comparing `fern_persona-0.0.2/src/persona/types/import_ip_address_lists_response.py` & `fern_persona-0.0.3/src/persona/types/import_ip_address_lists_response.py`

 * *Files identical despite different names*

### Comparing `fern_persona-0.0.2/src/persona/types/import_ip_address_lists_response_data.py` & `fern_persona-0.0.3/src/persona/types/import_ip_address_lists_response_data.py`

 * *Files identical despite different names*

### Comparing `fern_persona-0.0.2/src/persona/types/import_ip_address_lists_response_data_attributes.py` & `fern_persona-0.0.3/src/persona/types/import_ip_address_lists_response_data_attributes.py`

 * *Files identical despite different names*

### Comparing `fern_persona-0.0.2/src/persona/types/import_name_lists_request_data.py` & `fern_persona-0.0.3/src/persona/types/import_name_lists_request_data.py`

 * *Files identical despite different names*

### Comparing `fern_persona-0.0.2/src/persona/types/import_name_lists_request_data_attributes.py` & `fern_persona-0.0.3/src/persona/types/import_name_lists_request_data_attributes.py`

 * *Files identical despite different names*

### Comparing `fern_persona-0.0.2/src/persona/types/import_name_lists_request_data_attributes_file.py` & `fern_persona-0.0.3/src/persona/types/import_name_lists_request_data_attributes_file.py`

 * *Files identical despite different names*

### Comparing `fern_persona-0.0.2/src/persona/types/import_name_lists_response.py` & `fern_persona-0.0.3/src/persona/types/import_name_lists_response.py`

 * *Files identical despite different names*

### Comparing `fern_persona-0.0.2/src/persona/types/import_name_lists_response_data.py` & `fern_persona-0.0.3/src/persona/types/import_name_lists_response_data.py`

 * *Files identical despite different names*

### Comparing `fern_persona-0.0.2/src/persona/types/import_name_lists_response_data_attributes.py` & `fern_persona-0.0.3/src/persona/types/import_name_lists_response_data_attributes.py`

 * *Files identical despite different names*

### Comparing `fern_persona-0.0.2/src/persona/types/import_phone_number_lists_request_data.py` & `fern_persona-0.0.3/src/persona/types/import_phone_number_lists_request_data.py`

 * *Files identical despite different names*

### Comparing `fern_persona-0.0.2/src/persona/types/import_phone_number_lists_request_data_attributes.py` & `fern_persona-0.0.3/src/persona/types/import_phone_number_lists_request_data_attributes.py`

 * *Files identical despite different names*

### Comparing `fern_persona-0.0.2/src/persona/types/import_phone_number_lists_request_data_attributes_file.py` & `fern_persona-0.0.3/src/persona/types/import_phone_number_lists_request_data_attributes_file.py`

 * *Files identical despite different names*

### Comparing `fern_persona-0.0.2/src/persona/types/import_phone_number_lists_response.py` & `fern_persona-0.0.3/src/persona/types/import_phone_number_lists_response.py`

 * *Files identical despite different names*

### Comparing `fern_persona-0.0.2/src/persona/types/import_phone_number_lists_response_data.py` & `fern_persona-0.0.3/src/persona/types/import_phone_number_lists_response_data.py`

 * *Files identical despite different names*

### Comparing `fern_persona-0.0.2/src/persona/types/import_phone_number_lists_response_data_attributes.py` & `fern_persona-0.0.3/src/persona/types/import_phone_number_lists_response_data_attributes.py`

 * *Files identical despite different names*

### Comparing `fern_persona-0.0.2/src/persona/types/list_all_accounts_response.py` & `fern_persona-0.0.3/src/persona/types/list_all_accounts_response.py`

 * *Files identical despite different names*

### Comparing `fern_persona-0.0.2/src/persona/types/list_all_accounts_response_data_item.py` & `fern_persona-0.0.3/src/persona/types/list_all_accounts_response_data_item.py`

 * *Files identical despite different names*

### Comparing `fern_persona-0.0.2/src/persona/types/list_all_accounts_response_data_item_attributes.py` & `fern_persona-0.0.3/src/persona/types/list_all_accounts_response_data_item_attributes.py`

 * *Files identical despite different names*

### Comparing `fern_persona-0.0.2/src/persona/types/list_all_accounts_response_links.py` & `fern_persona-0.0.3/src/persona/types/list_all_accounts_response_links.py`

 * *Files identical despite different names*

### Comparing `fern_persona-0.0.2/src/persona/types/list_all_api_keys_response.py` & `fern_persona-0.0.3/src/persona/types/list_all_api_keys_response.py`

 * *Files identical despite different names*

### Comparing `fern_persona-0.0.2/src/persona/types/list_all_api_keys_response_data_item.py` & `fern_persona-0.0.3/src/persona/types/list_all_api_keys_response_data_item.py`

 * *Files identical despite different names*

### Comparing `fern_persona-0.0.2/src/persona/types/list_all_api_keys_response_data_item_attributes.py` & `fern_persona-0.0.3/src/persona/types/list_all_api_keys_response_data_item_attributes.py`

 * *Files identical despite different names*

### Comparing `fern_persona-0.0.2/src/persona/types/list_all_api_keys_response_links.py` & `fern_persona-0.0.3/src/persona/types/list_all_api_keys_response_links.py`

 * *Files identical despite different names*

### Comparing `fern_persona-0.0.2/src/persona/types/list_all_cases_response.py` & `fern_persona-0.0.3/src/persona/types/list_all_cases_response.py`

 * *Files identical despite different names*

### Comparing `fern_persona-0.0.2/src/persona/types/list_all_cases_response_data_item.py` & `fern_persona-0.0.3/src/persona/types/list_all_cases_response_data_item.py`

 * *Files identical despite different names*

### Comparing `fern_persona-0.0.2/src/persona/types/list_all_cases_response_data_item_attributes.py` & `fern_persona-0.0.3/src/persona/types/list_all_cases_response_data_item_attributes.py`

 * *Files identical despite different names*

### Comparing `fern_persona-0.0.2/src/persona/types/list_all_cases_response_data_item_relationships.py` & `fern_persona-0.0.3/src/persona/types/list_all_cases_response_data_item_relationships.py`

 * *Files identical despite different names*

### Comparing `fern_persona-0.0.2/src/persona/types/list_all_cases_response_data_item_relationships_case_template.py` & `fern_persona-0.0.3/src/persona/types/list_all_cases_response_data_item_relationships_case_template.py`

 * *Files identical despite different names*

### Comparing `fern_persona-0.0.2/src/persona/types/list_all_cases_response_data_item_relationships_case_template_data.py` & `fern_persona-0.0.3/src/persona/types/list_all_cases_response_data_item_relationships_case_template_data.py`

 * *Files identical despite different names*

### Comparing `fern_persona-0.0.2/src/persona/types/list_all_cases_response_links.py` & `fern_persona-0.0.3/src/persona/types/list_all_cases_response_links.py`

 * *Files identical despite different names*

### Comparing `fern_persona-0.0.2/src/persona/types/list_all_events_response.py` & `fern_persona-0.0.3/src/persona/types/list_all_events_response.py`

 * *Files identical despite different names*

### Comparing `fern_persona-0.0.2/src/persona/types/list_all_inquiries_response.py` & `fern_persona-0.0.3/src/persona/types/list_all_inquiries_response.py`

 * *Files identical despite different names*

### Comparing `fern_persona-0.0.2/src/persona/types/list_all_inquiries_response_data_item.py` & `fern_persona-0.0.3/src/persona/types/list_all_inquiries_response_data_item.py`

 * *Files identical despite different names*

### Comparing `fern_persona-0.0.2/src/persona/types/list_all_inquiries_response_data_item_attributes.py` & `fern_persona-0.0.3/src/persona/types/list_all_inquiries_response_data_item_attributes.py`

 * *Files identical despite different names*

### Comparing `fern_persona-0.0.2/src/persona/types/list_all_inquiries_response_data_item_relationships.py` & `fern_persona-0.0.3/src/persona/types/list_all_inquiries_response_data_item_relationships.py`

 * *Files identical despite different names*

### Comparing `fern_persona-0.0.2/src/persona/types/list_all_inquiries_response_data_item_relationships_account.py` & `fern_persona-0.0.3/src/persona/types/list_all_inquiries_response_data_item_relationships_account.py`

 * *Files identical despite different names*

### Comparing `fern_persona-0.0.2/src/persona/types/list_all_inquiries_response_data_item_relationships_account_data.py` & `fern_persona-0.0.3/src/persona/types/list_all_inquiries_response_data_item_relationships_account_data.py`

 * *Files identical despite different names*

### Comparing `fern_persona-0.0.2/src/persona/types/list_all_inquiries_response_data_item_relationships_reports.py` & `fern_persona-0.0.3/src/persona/types/list_all_inquiries_response_data_item_relationships_reports.py`

 * *Files identical despite different names*

### Comparing `fern_persona-0.0.2/src/persona/types/list_all_inquiries_response_data_item_relationships_sessions.py` & `fern_persona-0.0.3/src/persona/types/list_all_inquiries_response_data_item_relationships_sessions.py`

 * *Files identical despite different names*

### Comparing `fern_persona-0.0.2/src/persona/types/list_all_inquiries_response_data_item_relationships_sessions_data_item.py` & `fern_persona-0.0.3/src/persona/types/list_all_inquiries_response_data_item_relationships_sessions_data_item.py`

 * *Files identical despite different names*

### Comparing `fern_persona-0.0.2/src/persona/types/list_all_inquiries_response_data_item_relationships_template.py` & `fern_persona-0.0.3/src/persona/types/list_all_inquiries_response_data_item_relationships_template.py`

 * *Files identical despite different names*

### Comparing `fern_persona-0.0.2/src/persona/types/list_all_inquiries_response_data_item_relationships_template_data.py` & `fern_persona-0.0.3/src/persona/types/list_all_inquiries_response_data_item_relationships_template_data.py`

 * *Files identical despite different names*

### Comparing `fern_persona-0.0.2/src/persona/types/list_all_inquiries_response_data_item_relationships_verifications.py` & `fern_persona-0.0.3/src/persona/types/list_all_inquiries_response_data_item_relationships_verifications.py`

 * *Files identical despite different names*

### Comparing `fern_persona-0.0.2/src/persona/types/list_all_inquiries_response_data_item_relationships_verifications_data_item.py` & `fern_persona-0.0.3/src/persona/types/list_all_inquiries_response_data_item_relationships_verifications_data_item.py`

 * *Files identical despite different names*

### Comparing `fern_persona-0.0.2/src/persona/types/list_all_inquiries_response_links.py` & `fern_persona-0.0.3/src/persona/types/list_all_inquiries_response_links.py`

 * *Files identical despite different names*

### Comparing `fern_persona-0.0.2/src/persona/types/list_all_lists_response.py` & `fern_persona-0.0.3/src/persona/types/list_all_lists_response.py`

 * *Files identical despite different names*

### Comparing `fern_persona-0.0.2/src/persona/types/redact_a_report_response.py` & `fern_persona-0.0.3/src/persona/types/redact_a_report_response.py`

 * *Files identical despite different names*

### Comparing `fern_persona-0.0.2/src/persona/types/redact_a_report_response_data.py` & `fern_persona-0.0.3/src/persona/types/redact_a_report_response_data.py`

 * *Files identical despite different names*

### Comparing `fern_persona-0.0.2/src/persona/types/redact_a_report_response_data_attributes.py` & `fern_persona-0.0.3/src/persona/types/redact_a_report_response_data_attributes.py`

 * *Files identical despite different names*

### Comparing `fern_persona-0.0.2/src/persona/types/redact_an_account_response.py` & `fern_persona-0.0.3/src/persona/types/redact_an_account_response.py`

 * *Files identical despite different names*

### Comparing `fern_persona-0.0.2/src/persona/types/redact_an_account_response_data.py` & `fern_persona-0.0.3/src/persona/types/redact_an_account_response_data.py`

 * *Files identical despite different names*

### Comparing `fern_persona-0.0.2/src/persona/types/redact_an_account_response_data_attributes.py` & `fern_persona-0.0.3/src/persona/types/redact_an_account_response_data_attributes.py`

 * *Files identical despite different names*

### Comparing `fern_persona-0.0.2/src/persona/types/redact_an_inquiry_response.py` & `fern_persona-0.0.3/src/persona/types/redact_an_inquiry_response.py`

 * *Files identical despite different names*

### Comparing `fern_persona-0.0.2/src/persona/types/redact_an_inquiry_response_data.py` & `fern_persona-0.0.3/src/persona/types/redact_an_inquiry_response_data.py`

 * *Files identical despite different names*

### Comparing `fern_persona-0.0.2/src/persona/types/redact_an_inquiry_response_data_attributes.py` & `fern_persona-0.0.3/src/persona/types/redact_an_inquiry_response_data_attributes.py`

 * *Files identical despite different names*

### Comparing `fern_persona-0.0.2/src/persona/types/redact_an_inquiry_response_data_relationships.py` & `fern_persona-0.0.3/src/persona/types/redact_an_inquiry_response_data_relationships.py`

 * *Files identical despite different names*

### Comparing `fern_persona-0.0.2/src/persona/types/redact_an_inquiry_response_data_relationships_account.py` & `fern_persona-0.0.3/src/persona/types/redact_an_inquiry_response_data_relationships_account.py`

 * *Files identical despite different names*

### Comparing `fern_persona-0.0.2/src/persona/types/redact_an_inquiry_response_data_relationships_account_data.py` & `fern_persona-0.0.3/src/persona/types/redact_an_inquiry_response_data_relationships_account_data.py`

 * *Files identical despite different names*

### Comparing `fern_persona-0.0.2/src/persona/types/redact_an_inquiry_response_data_relationships_reports.py` & `fern_persona-0.0.3/src/persona/types/redact_an_inquiry_response_data_relationships_reports.py`

 * *Files identical despite different names*

### Comparing `fern_persona-0.0.2/src/persona/types/redact_an_inquiry_response_data_relationships_template.py` & `fern_persona-0.0.3/src/persona/types/redact_an_inquiry_response_data_relationships_template.py`

 * *Files identical despite different names*

### Comparing `fern_persona-0.0.2/src/persona/types/redact_an_inquiry_response_data_relationships_template_data.py` & `fern_persona-0.0.3/src/persona/types/redact_an_inquiry_response_data_relationships_template_data.py`

 * *Files identical despite different names*

### Comparing `fern_persona-0.0.2/src/persona/types/redact_an_inquiry_response_data_relationships_verifications.py` & `fern_persona-0.0.3/src/persona/types/redact_an_inquiry_response_data_relationships_verifications.py`

 * *Files identical despite different names*

### Comparing `fern_persona-0.0.2/src/persona/types/redact_an_inquiry_response_data_relationships_verifications_data_item.py` & `fern_persona-0.0.3/src/persona/types/redact_an_inquiry_response_data_relationships_verifications_data_item.py`

 * *Files identical despite different names*

### Comparing `fern_persona-0.0.2/src/persona/types/remove_a_tag_1_request_meta.py` & `fern_persona-0.0.3/src/persona/types/remove_a_tag_1_request_meta.py`

 * *Files identical despite different names*

### Comparing `fern_persona-0.0.2/src/persona/types/remove_a_tag_request_meta.py` & `fern_persona-0.0.3/src/persona/types/remove_a_tag_request_meta.py`

 * *Files identical despite different names*

### Comparing `fern_persona-0.0.2/src/persona/types/report_action_pause_continuous_monitoring_response.py` & `fern_persona-0.0.3/src/persona/types/report_action_pause_continuous_monitoring_response.py`

 * *Files identical despite different names*

### Comparing `fern_persona-0.0.2/src/persona/types/report_action_pause_continuous_monitoring_response_data.py` & `fern_persona-0.0.3/src/persona/types/report_action_pause_continuous_monitoring_response_data.py`

 * *Files identical despite different names*

### Comparing `fern_persona-0.0.2/src/persona/types/report_action_pause_continuous_monitoring_response_data_attributes.py` & `fern_persona-0.0.3/src/persona/types/report_action_pause_continuous_monitoring_response_data_attributes.py`

 * *Files identical despite different names*

### Comparing `fern_persona-0.0.2/src/persona/types/report_action_pause_continuous_monitoring_response_data_relationships.py` & `fern_persona-0.0.3/src/persona/types/report_action_pause_continuous_monitoring_response_data_relationships.py`

 * *Files identical despite different names*

### Comparing `fern_persona-0.0.2/src/persona/types/report_action_pause_continuous_monitoring_response_data_relationships_account.py` & `fern_persona-0.0.3/src/persona/types/report_action_pause_continuous_monitoring_response_data_relationships_account.py`

 * *Files identical despite different names*

### Comparing `fern_persona-0.0.2/src/persona/types/report_action_pause_continuous_monitoring_response_data_relationships_inquiry.py` & `fern_persona-0.0.3/src/persona/types/report_action_pause_continuous_monitoring_response_data_relationships_inquiry.py`

 * *Files identical despite different names*

### Comparing `fern_persona-0.0.2/src/persona/types/report_action_pause_continuous_monitoring_response_data_relationships_report_template.py` & `fern_persona-0.0.3/src/persona/types/report_action_pause_continuous_monitoring_response_data_relationships_report_template.py`

 * *Files identical despite different names*

### Comparing `fern_persona-0.0.2/src/persona/types/report_action_pause_continuous_monitoring_response_data_relationships_report_template_data.py` & `fern_persona-0.0.3/src/persona/types/report_action_pause_continuous_monitoring_response_data_relationships_report_template_data.py`

 * *Files identical despite different names*

### Comparing `fern_persona-0.0.2/src/persona/types/report_action_re_run_report_response.py` & `fern_persona-0.0.3/src/persona/types/report_action_re_run_report_response.py`

 * *Files identical despite different names*

### Comparing `fern_persona-0.0.2/src/persona/types/report_action_re_run_report_response_data.py` & `fern_persona-0.0.3/src/persona/types/report_action_re_run_report_response_data.py`

 * *Files identical despite different names*

### Comparing `fern_persona-0.0.2/src/persona/types/report_action_re_run_report_response_data_attributes.py` & `fern_persona-0.0.3/src/persona/types/report_action_re_run_report_response_data_attributes.py`

 * *Files identical despite different names*

### Comparing `fern_persona-0.0.2/src/persona/types/report_action_re_run_report_response_data_relationships.py` & `fern_persona-0.0.3/src/persona/types/report_action_re_run_report_response_data_relationships.py`

 * *Files identical despite different names*

### Comparing `fern_persona-0.0.2/src/persona/types/report_action_re_run_report_response_data_relationships_account.py` & `fern_persona-0.0.3/src/persona/types/report_action_re_run_report_response_data_relationships_account.py`

 * *Files identical despite different names*

### Comparing `fern_persona-0.0.2/src/persona/types/report_action_re_run_report_response_data_relationships_inquiry.py` & `fern_persona-0.0.3/src/persona/types/report_action_re_run_report_response_data_relationships_inquiry.py`

 * *Files identical despite different names*

### Comparing `fern_persona-0.0.2/src/persona/types/report_action_re_run_report_response_data_relationships_report_template.py` & `fern_persona-0.0.3/src/persona/types/report_action_re_run_report_response_data_relationships_report_template.py`

 * *Files identical despite different names*

### Comparing `fern_persona-0.0.2/src/persona/types/report_action_re_run_report_response_data_relationships_report_template_data.py` & `fern_persona-0.0.3/src/persona/types/report_action_re_run_report_response_data_relationships_report_template_data.py`

 * *Files identical despite different names*

### Comparing `fern_persona-0.0.2/src/persona/types/report_action_resume_continuous_monitoring_response.py` & `fern_persona-0.0.3/src/persona/types/report_action_resume_continuous_monitoring_response.py`

 * *Files identical despite different names*

### Comparing `fern_persona-0.0.2/src/persona/types/report_action_resume_continuous_monitoring_response_data.py` & `fern_persona-0.0.3/src/persona/types/report_action_resume_continuous_monitoring_response_data.py`

 * *Files identical despite different names*

### Comparing `fern_persona-0.0.2/src/persona/types/report_action_resume_continuous_monitoring_response_data_attributes.py` & `fern_persona-0.0.3/src/persona/types/report_action_resume_continuous_monitoring_response_data_attributes.py`

 * *Files identical despite different names*

### Comparing `fern_persona-0.0.2/src/persona/types/report_action_resume_continuous_monitoring_response_data_relationships.py` & `fern_persona-0.0.3/src/persona/types/report_action_resume_continuous_monitoring_response_data_relationships.py`

 * *Files identical despite different names*

### Comparing `fern_persona-0.0.2/src/persona/types/report_action_resume_continuous_monitoring_response_data_relationships_account.py` & `fern_persona-0.0.3/src/persona/types/report_action_resume_continuous_monitoring_response_data_relationships_account.py`

 * *Files identical despite different names*

### Comparing `fern_persona-0.0.2/src/persona/types/report_action_resume_continuous_monitoring_response_data_relationships_inquiry.py` & `fern_persona-0.0.3/src/persona/types/report_action_resume_continuous_monitoring_response_data_relationships_inquiry.py`

 * *Files identical despite different names*

### Comparing `fern_persona-0.0.2/src/persona/types/report_action_resume_continuous_monitoring_response_data_relationships_report_template.py` & `fern_persona-0.0.3/src/persona/types/report_action_resume_continuous_monitoring_response_data_relationships_report_template.py`

 * *Files identical despite different names*

### Comparing `fern_persona-0.0.2/src/persona/types/report_action_resume_continuous_monitoring_response_data_relationships_report_template_data.py` & `fern_persona-0.0.3/src/persona/types/report_action_resume_continuous_monitoring_response_data_relationships_report_template_data.py`

 * *Files identical despite different names*

### Comparing `fern_persona-0.0.2/src/persona/types/reports_add_a_tag_request_meta.py` & `fern_persona-0.0.3/src/persona/types/reports_add_a_tag_request_meta.py`

 * *Files identical despite different names*

### Comparing `fern_persona-0.0.2/src/persona/types/reports_add_a_tag_response.py` & `fern_persona-0.0.3/src/persona/types/reports_add_a_tag_response.py`

 * *Files identical despite different names*

### Comparing `fern_persona-0.0.2/src/persona/types/reports_add_a_tag_response_data.py` & `fern_persona-0.0.3/src/persona/types/reports_add_a_tag_response_data.py`

 * *Files identical despite different names*

### Comparing `fern_persona-0.0.2/src/persona/types/reports_add_a_tag_response_data_attributes.py` & `fern_persona-0.0.3/src/persona/types/reports_add_a_tag_response_data_attributes.py`

 * *Files identical despite different names*

### Comparing `fern_persona-0.0.2/src/persona/types/reports_add_a_tag_response_data_relationships.py` & `fern_persona-0.0.3/src/persona/types/reports_add_a_tag_response_data_relationships.py`

 * *Files identical despite different names*

### Comparing `fern_persona-0.0.2/src/persona/types/reports_add_a_tag_response_data_relationships_account.py` & `fern_persona-0.0.3/src/persona/types/reports_add_a_tag_response_data_relationships_account.py`

 * *Files identical despite different names*

### Comparing `fern_persona-0.0.2/src/persona/types/reports_add_a_tag_response_data_relationships_inquiry.py` & `fern_persona-0.0.3/src/persona/types/reports_add_a_tag_response_data_relationships_inquiry.py`

 * *Files identical despite different names*

### Comparing `fern_persona-0.0.2/src/persona/types/reports_add_a_tag_response_data_relationships_report_template.py` & `fern_persona-0.0.3/src/persona/types/reports_add_a_tag_response_data_relationships_report_template.py`

 * *Files identical despite different names*

### Comparing `fern_persona-0.0.2/src/persona/types/reports_add_a_tag_response_data_relationships_report_template_data.py` & `fern_persona-0.0.3/src/persona/types/reports_add_a_tag_response_data_relationships_report_template_data.py`

 * *Files identical despite different names*

### Comparing `fern_persona-0.0.2/src/persona/types/reports_remove_a_tag_request_meta.py` & `fern_persona-0.0.3/src/persona/types/reports_remove_a_tag_request_meta.py`

 * *Files identical despite different names*

### Comparing `fern_persona-0.0.2/src/persona/types/reports_remove_a_tag_response.py` & `fern_persona-0.0.3/src/persona/types/reports_remove_a_tag_response.py`

 * *Files identical despite different names*

### Comparing `fern_persona-0.0.2/src/persona/types/reports_remove_a_tag_response_data.py` & `fern_persona-0.0.3/src/persona/types/reports_remove_a_tag_response_data.py`

 * *Files identical despite different names*

### Comparing `fern_persona-0.0.2/src/persona/types/reports_remove_a_tag_response_data_attributes.py` & `fern_persona-0.0.3/src/persona/types/reports_remove_a_tag_response_data_attributes.py`

 * *Files identical despite different names*

### Comparing `fern_persona-0.0.2/src/persona/types/reports_remove_a_tag_response_data_relationships.py` & `fern_persona-0.0.3/src/persona/types/reports_remove_a_tag_response_data_relationships.py`

 * *Files identical despite different names*

### Comparing `fern_persona-0.0.2/src/persona/types/reports_remove_a_tag_response_data_relationships_account.py` & `fern_persona-0.0.3/src/persona/types/reports_remove_a_tag_response_data_relationships_account.py`

 * *Files identical despite different names*

### Comparing `fern_persona-0.0.2/src/persona/types/reports_remove_a_tag_response_data_relationships_inquiry.py` & `fern_persona-0.0.3/src/persona/types/reports_remove_a_tag_response_data_relationships_inquiry.py`

 * *Files identical despite different names*

### Comparing `fern_persona-0.0.2/src/persona/types/reports_remove_a_tag_response_data_relationships_report_template.py` & `fern_persona-0.0.3/src/persona/types/reports_remove_a_tag_response_data_relationships_report_template.py`

 * *Files identical despite different names*

### Comparing `fern_persona-0.0.2/src/persona/types/reports_remove_a_tag_response_data_relationships_report_template_data.py` & `fern_persona-0.0.3/src/persona/types/reports_remove_a_tag_response_data_relationships_report_template_data.py`

 * *Files identical despite different names*

### Comparing `fern_persona-0.0.2/src/persona/types/reports_set_all_tags_request_meta.py` & `fern_persona-0.0.3/src/persona/types/reports_set_all_tags_request_meta.py`

 * *Files identical despite different names*

### Comparing `fern_persona-0.0.2/src/persona/types/reports_set_all_tags_response.py` & `fern_persona-0.0.3/src/persona/types/reports_set_all_tags_response.py`

 * *Files identical despite different names*

### Comparing `fern_persona-0.0.2/src/persona/types/reports_set_all_tags_response_data.py` & `fern_persona-0.0.3/src/persona/types/reports_set_all_tags_response_data.py`

 * *Files identical despite different names*

### Comparing `fern_persona-0.0.2/src/persona/types/reports_set_all_tags_response_data_attributes.py` & `fern_persona-0.0.3/src/persona/types/reports_set_all_tags_response_data_attributes.py`

 * *Files identical despite different names*

### Comparing `fern_persona-0.0.2/src/persona/types/reports_set_all_tags_response_data_relationships.py` & `fern_persona-0.0.3/src/persona/types/reports_set_all_tags_response_data_relationships.py`

 * *Files identical despite different names*

### Comparing `fern_persona-0.0.2/src/persona/types/reports_set_all_tags_response_data_relationships_account.py` & `fern_persona-0.0.3/src/persona/types/reports_set_all_tags_response_data_relationships_account.py`

 * *Files identical despite different names*

### Comparing `fern_persona-0.0.2/src/persona/types/reports_set_all_tags_response_data_relationships_inquiry.py` & `fern_persona-0.0.3/src/persona/types/reports_set_all_tags_response_data_relationships_inquiry.py`

 * *Files identical despite different names*

### Comparing `fern_persona-0.0.2/src/persona/types/reports_set_all_tags_response_data_relationships_report_template.py` & `fern_persona-0.0.3/src/persona/types/reports_set_all_tags_response_data_relationships_report_template.py`

 * *Files identical despite different names*

### Comparing `fern_persona-0.0.2/src/persona/types/reports_set_all_tags_response_data_relationships_report_template_data.py` & `fern_persona-0.0.3/src/persona/types/reports_set_all_tags_response_data_relationships_report_template_data.py`

 * *Files identical despite different names*

### Comparing `fern_persona-0.0.2/src/persona/types/resume_an_inquiry_response.py` & `fern_persona-0.0.3/src/persona/types/resume_an_inquiry_response.py`

 * *Files identical despite different names*

### Comparing `fern_persona-0.0.2/src/persona/types/resume_an_inquiry_response_data.py` & `fern_persona-0.0.3/src/persona/types/resume_an_inquiry_response_data.py`

 * *Files identical despite different names*

### Comparing `fern_persona-0.0.2/src/persona/types/resume_an_inquiry_response_data_attributes.py` & `fern_persona-0.0.3/src/persona/types/resume_an_inquiry_response_data_attributes.py`

 * *Files identical despite different names*

### Comparing `fern_persona-0.0.2/src/persona/types/resume_an_inquiry_response_data_relationships.py` & `fern_persona-0.0.3/src/persona/types/resume_an_inquiry_response_data_relationships.py`

 * *Files identical despite different names*

### Comparing `fern_persona-0.0.2/src/persona/types/resume_an_inquiry_response_data_relationships_account.py` & `fern_persona-0.0.3/src/persona/types/resume_an_inquiry_response_data_relationships_account.py`

 * *Files identical despite different names*

### Comparing `fern_persona-0.0.2/src/persona/types/resume_an_inquiry_response_data_relationships_account_data.py` & `fern_persona-0.0.3/src/persona/types/resume_an_inquiry_response_data_relationships_account_data.py`

 * *Files identical despite different names*

### Comparing `fern_persona-0.0.2/src/persona/types/resume_an_inquiry_response_data_relationships_reports.py` & `fern_persona-0.0.3/src/persona/types/resume_an_inquiry_response_data_relationships_reports.py`

 * *Files identical despite different names*

### Comparing `fern_persona-0.0.2/src/persona/types/resume_an_inquiry_response_data_relationships_template.py` & `fern_persona-0.0.3/src/persona/types/resume_an_inquiry_response_data_relationships_template.py`

 * *Files identical despite different names*

### Comparing `fern_persona-0.0.2/src/persona/types/resume_an_inquiry_response_data_relationships_template_data.py` & `fern_persona-0.0.3/src/persona/types/resume_an_inquiry_response_data_relationships_template_data.py`

 * *Files identical despite different names*

### Comparing `fern_persona-0.0.2/src/persona/types/resume_an_inquiry_response_data_relationships_verifications.py` & `fern_persona-0.0.3/src/persona/types/resume_an_inquiry_response_data_relationships_verifications.py`

 * *Files identical despite different names*

### Comparing `fern_persona-0.0.2/src/persona/types/resume_an_inquiry_response_data_relationships_verifications_data_item.py` & `fern_persona-0.0.3/src/persona/types/resume_an_inquiry_response_data_relationships_verifications_data_item.py`

 * *Files identical despite different names*

### Comparing `fern_persona-0.0.2/src/persona/types/resume_an_inquiry_response_meta.py` & `fern_persona-0.0.3/src/persona/types/resume_an_inquiry_response_meta.py`

 * *Files identical despite different names*

### Comparing `fern_persona-0.0.2/src/persona/types/retrieve_a_database_verification_response.py` & `fern_persona-0.0.3/src/persona/types/retrieve_a_database_verification_response.py`

 * *Files identical despite different names*

### Comparing `fern_persona-0.0.2/src/persona/types/retrieve_a_database_verification_response_data.py` & `fern_persona-0.0.3/src/persona/types/retrieve_a_database_verification_response_data.py`

 * *Files identical despite different names*

### Comparing `fern_persona-0.0.2/src/persona/types/retrieve_a_database_verification_response_data_attributes.py` & `fern_persona-0.0.3/src/persona/types/retrieve_a_database_verification_response_data_attributes.py`

 * *Files identical despite different names*

### Comparing `fern_persona-0.0.2/src/persona/types/retrieve_a_database_verification_response_data_attributes_checks_item.py` & `fern_persona-0.0.3/src/persona/types/retrieve_a_database_verification_response_data_attributes_checks_item.py`

 * *Files identical despite different names*

### Comparing `fern_persona-0.0.2/src/persona/types/retrieve_a_database_verification_response_data_attributes_checks_item_metadata.py` & `fern_persona-0.0.3/src/persona/types/retrieve_a_database_verification_response_data_attributes_checks_item_metadata.py`

 * *Files identical despite different names*

### Comparing `fern_persona-0.0.2/src/persona/types/retrieve_a_database_verification_response_data_relationships.py` & `fern_persona-0.0.3/src/persona/types/retrieve_a_database_verification_response_data_relationships.py`

 * *Files identical despite different names*

### Comparing `fern_persona-0.0.2/src/persona/types/retrieve_a_database_verification_response_data_relationships_inquiry.py` & `fern_persona-0.0.3/src/persona/types/retrieve_a_database_verification_response_data_relationships_inquiry.py`

 * *Files identical despite different names*

### Comparing `fern_persona-0.0.2/src/persona/types/retrieve_a_document_response.py` & `fern_persona-0.0.3/src/persona/types/retrieve_a_document_response.py`

 * *Files identical despite different names*

### Comparing `fern_persona-0.0.2/src/persona/types/retrieve_a_document_response_data.py` & `fern_persona-0.0.3/src/persona/types/retrieve_a_document_response_data.py`

 * *Files identical despite different names*

### Comparing `fern_persona-0.0.2/src/persona/types/retrieve_a_document_response_data_attributes.py` & `fern_persona-0.0.3/src/persona/types/retrieve_a_document_response_data_attributes.py`

 * *Files identical despite different names*

### Comparing `fern_persona-0.0.2/src/persona/types/retrieve_a_document_response_data_attributes_files_item.py` & `fern_persona-0.0.3/src/persona/types/retrieve_a_document_response_data_attributes_files_item.py`

 * *Files identical despite different names*

### Comparing `fern_persona-0.0.2/src/persona/types/retrieve_a_document_response_data_relationships.py` & `fern_persona-0.0.3/src/persona/types/retrieve_a_document_response_data_relationships.py`

 * *Files identical despite different names*

### Comparing `fern_persona-0.0.2/src/persona/types/retrieve_a_document_response_data_relationships_inquiry.py` & `fern_persona-0.0.3/src/persona/types/retrieve_a_document_response_data_relationships_inquiry.py`

 * *Files identical despite different names*

### Comparing `fern_persona-0.0.2/src/persona/types/retrieve_a_document_response_data_relationships_inquiry_data.py` & `fern_persona-0.0.3/src/persona/types/retrieve_a_document_response_data_relationships_inquiry_data.py`

 * *Files identical despite different names*

### Comparing `fern_persona-0.0.2/src/persona/types/retrieve_a_email_address_verification_response.py` & `fern_persona-0.0.3/src/persona/types/retrieve_a_email_address_verification_response.py`

 * *Files identical despite different names*

### Comparing `fern_persona-0.0.2/src/persona/types/retrieve_a_email_address_verification_response_data.py` & `fern_persona-0.0.3/src/persona/types/retrieve_a_email_address_verification_response_data.py`

 * *Files identical despite different names*

### Comparing `fern_persona-0.0.2/src/persona/types/retrieve_a_email_address_verification_response_data_attributes.py` & `fern_persona-0.0.3/src/persona/types/retrieve_a_email_address_verification_response_data_attributes.py`

 * *Files identical despite different names*

### Comparing `fern_persona-0.0.2/src/persona/types/retrieve_a_email_address_verification_response_data_attributes_metadata.py` & `fern_persona-0.0.3/src/persona/types/retrieve_a_email_address_verification_response_data_attributes_metadata.py`

 * *Files identical despite different names*

### Comparing `fern_persona-0.0.2/src/persona/types/retrieve_a_email_address_verification_response_data_relationships.py` & `fern_persona-0.0.3/src/persona/types/retrieve_a_email_address_verification_response_data_relationships.py`

 * *Files identical despite different names*

### Comparing `fern_persona-0.0.2/src/persona/types/retrieve_a_email_address_verification_response_data_relationships_inquiry.py` & `fern_persona-0.0.3/src/persona/types/retrieve_a_email_address_verification_response_data_relationships_inquiry.py`

 * *Files identical despite different names*

### Comparing `fern_persona-0.0.2/src/persona/types/retrieve_a_government_id_verification_response.py` & `fern_persona-0.0.3/src/persona/types/retrieve_a_government_id_verification_response.py`

 * *Files identical despite different names*

### Comparing `fern_persona-0.0.2/src/persona/types/retrieve_a_government_id_verification_response_data.py` & `fern_persona-0.0.3/src/persona/types/retrieve_a_government_id_verification_response_data.py`

 * *Files identical despite different names*

### Comparing `fern_persona-0.0.2/src/persona/types/retrieve_a_government_id_verification_response_data_attributes.py` & `fern_persona-0.0.3/src/persona/types/retrieve_a_government_id_verification_response_data_attributes.py`

 * *Files identical despite different names*

### Comparing `fern_persona-0.0.2/src/persona/types/retrieve_a_government_id_verification_response_data_attributes_checks_item.py` & `fern_persona-0.0.3/src/persona/types/retrieve_a_government_id_verification_response_data_attributes_checks_item.py`

 * *Files identical despite different names*

### Comparing `fern_persona-0.0.2/src/persona/types/retrieve_a_government_id_verification_response_data_attributes_checks_item_metadata.py` & `fern_persona-0.0.3/src/persona/types/retrieve_a_government_id_verification_response_data_attributes_checks_item_metadata.py`

 * *Files identical despite different names*

### Comparing `fern_persona-0.0.2/src/persona/types/retrieve_a_government_id_verification_response_data_attributes_photo_urls_item.py` & `fern_persona-0.0.3/src/persona/types/retrieve_a_government_id_verification_response_data_attributes_photo_urls_item.py`

 * *Files identical despite different names*

### Comparing `fern_persona-0.0.2/src/persona/types/retrieve_a_government_id_verification_response_data_relationships.py` & `fern_persona-0.0.3/src/persona/types/retrieve_a_government_id_verification_response_data_relationships.py`

 * *Files identical despite different names*

### Comparing `fern_persona-0.0.2/src/persona/types/retrieve_a_government_id_verification_response_data_relationships_document.py` & `fern_persona-0.0.3/src/persona/types/retrieve_a_government_id_verification_response_data_relationships_document.py`

 * *Files identical despite different names*

### Comparing `fern_persona-0.0.2/src/persona/types/retrieve_a_government_id_verification_response_data_relationships_document_data.py` & `fern_persona-0.0.3/src/persona/types/retrieve_a_government_id_verification_response_data_relationships_document_data.py`

 * *Files identical despite different names*

### Comparing `fern_persona-0.0.2/src/persona/types/retrieve_a_government_id_verification_response_data_relationships_inquiry.py` & `fern_persona-0.0.3/src/persona/types/retrieve_a_government_id_verification_response_data_relationships_inquiry.py`

 * *Files identical despite different names*

### Comparing `fern_persona-0.0.2/src/persona/types/retrieve_a_list_response.py` & `fern_persona-0.0.3/src/persona/types/retrieve_a_list_response.py`

 * *Files identical despite different names*

### Comparing `fern_persona-0.0.2/src/persona/types/retrieve_a_phone_carrier_database_verification_response.py` & `fern_persona-0.0.3/src/persona/types/retrieve_a_phone_carrier_database_verification_response.py`

 * *Files identical despite different names*

### Comparing `fern_persona-0.0.2/src/persona/types/retrieve_a_phone_carrier_database_verification_response_data.py` & `fern_persona-0.0.3/src/persona/types/retrieve_a_phone_carrier_database_verification_response_data.py`

 * *Files identical despite different names*

### Comparing `fern_persona-0.0.2/src/persona/types/retrieve_a_phone_carrier_database_verification_response_data_attributes.py` & `fern_persona-0.0.3/src/persona/types/retrieve_a_phone_carrier_database_verification_response_data_attributes.py`

 * *Files identical despite different names*

### Comparing `fern_persona-0.0.2/src/persona/types/retrieve_a_phone_carrier_database_verification_response_data_attributes_checks_item.py` & `fern_persona-0.0.3/src/persona/types/retrieve_a_phone_carrier_database_verification_response_data_attributes_checks_item.py`

 * *Files identical despite different names*

### Comparing `fern_persona-0.0.2/src/persona/types/retrieve_a_phone_carrier_database_verification_response_data_attributes_checks_item_metadata.py` & `fern_persona-0.0.3/src/persona/types/retrieve_a_phone_carrier_database_verification_response_data_attributes_checks_item_metadata.py`

 * *Files identical despite different names*

### Comparing `fern_persona-0.0.2/src/persona/types/retrieve_a_phone_carrier_database_verification_response_data_relationships.py` & `fern_persona-0.0.3/src/persona/types/retrieve_a_phone_carrier_database_verification_response_data_relationships.py`

 * *Files identical despite different names*

### Comparing `fern_persona-0.0.2/src/persona/types/retrieve_a_phone_carrier_database_verification_response_data_relationships_inquiry.py` & `fern_persona-0.0.3/src/persona/types/retrieve_a_phone_carrier_database_verification_response_data_relationships_inquiry.py`

 * *Files identical despite different names*

### Comparing `fern_persona-0.0.2/src/persona/types/retrieve_a_phone_number_verification_response.py` & `fern_persona-0.0.3/src/persona/types/retrieve_a_phone_number_verification_response.py`

 * *Files identical despite different names*

### Comparing `fern_persona-0.0.2/src/persona/types/retrieve_a_phone_number_verification_response_data.py` & `fern_persona-0.0.3/src/persona/types/retrieve_a_phone_number_verification_response_data.py`

 * *Files identical despite different names*

### Comparing `fern_persona-0.0.2/src/persona/types/retrieve_a_phone_number_verification_response_data_attributes.py` & `fern_persona-0.0.3/src/persona/types/retrieve_a_phone_number_verification_response_data_attributes.py`

 * *Files identical despite different names*

### Comparing `fern_persona-0.0.2/src/persona/types/retrieve_a_phone_number_verification_response_data_attributes_metadata.py` & `fern_persona-0.0.3/src/persona/types/retrieve_a_phone_number_verification_response_data_attributes_metadata.py`

 * *Files identical despite different names*

### Comparing `fern_persona-0.0.2/src/persona/types/retrieve_a_phone_number_verification_response_data_relationships.py` & `fern_persona-0.0.3/src/persona/types/retrieve_a_phone_number_verification_response_data_relationships.py`

 * *Files identical despite different names*

### Comparing `fern_persona-0.0.2/src/persona/types/retrieve_a_phone_number_verification_response_data_relationships_inquiry.py` & `fern_persona-0.0.3/src/persona/types/retrieve_a_phone_number_verification_response_data_relationships_inquiry.py`

 * *Files identical despite different names*

### Comparing `fern_persona-0.0.2/src/persona/types/retrieve_a_report_response.py` & `fern_persona-0.0.3/src/persona/types/retrieve_a_report_response.py`

 * *Files identical despite different names*

### Comparing `fern_persona-0.0.2/src/persona/types/retrieve_a_report_response_data.py` & `fern_persona-0.0.3/src/persona/types/retrieve_a_report_response_data.py`

 * *Files identical despite different names*

### Comparing `fern_persona-0.0.2/src/persona/types/retrieve_a_report_response_data_attributes.py` & `fern_persona-0.0.3/src/persona/types/retrieve_a_report_response_data_attributes.py`

 * *Files identical despite different names*

### Comparing `fern_persona-0.0.2/src/persona/types/retrieve_a_selfie_verification_response.py` & `fern_persona-0.0.3/src/persona/types/retrieve_a_selfie_verification_response.py`

 * *Files identical despite different names*

### Comparing `fern_persona-0.0.2/src/persona/types/retrieve_a_selfie_verification_response_data.py` & `fern_persona-0.0.3/src/persona/types/retrieve_a_selfie_verification_response_data.py`

 * *Files identical despite different names*

### Comparing `fern_persona-0.0.2/src/persona/types/retrieve_a_selfie_verification_response_data_attributes.py` & `fern_persona-0.0.3/src/persona/types/retrieve_a_selfie_verification_response_data_attributes.py`

 * *Files identical despite different names*

### Comparing `fern_persona-0.0.2/src/persona/types/retrieve_a_selfie_verification_response_data_attributes_checks_item.py` & `fern_persona-0.0.3/src/persona/types/retrieve_a_selfie_verification_response_data_attributes_checks_item.py`

 * *Files identical despite different names*

### Comparing `fern_persona-0.0.2/src/persona/types/retrieve_a_selfie_verification_response_data_attributes_checks_item_metadata.py` & `fern_persona-0.0.3/src/persona/types/retrieve_a_selfie_verification_response_data_attributes_checks_item_metadata.py`

 * *Files identical despite different names*

### Comparing `fern_persona-0.0.2/src/persona/types/retrieve_a_selfie_verification_response_data_relationships.py` & `fern_persona-0.0.3/src/persona/types/retrieve_a_selfie_verification_response_data_relationships.py`

 * *Files identical despite different names*

### Comparing `fern_persona-0.0.2/src/persona/types/retrieve_a_selfie_verification_response_data_relationships_inquiry.py` & `fern_persona-0.0.3/src/persona/types/retrieve_a_selfie_verification_response_data_relationships_inquiry.py`

 * *Files identical despite different names*

### Comparing `fern_persona-0.0.2/src/persona/types/retrieve_a_serpro_database_verification_response.py` & `fern_persona-0.0.3/src/persona/types/retrieve_a_serpro_database_verification_response.py`

 * *Files identical despite different names*

### Comparing `fern_persona-0.0.2/src/persona/types/retrieve_a_serpro_database_verification_response_data.py` & `fern_persona-0.0.3/src/persona/types/retrieve_a_serpro_database_verification_response_data.py`

 * *Files identical despite different names*

### Comparing `fern_persona-0.0.2/src/persona/types/retrieve_a_serpro_database_verification_response_data_attributes.py` & `fern_persona-0.0.3/src/persona/types/retrieve_a_serpro_database_verification_response_data_attributes.py`

 * *Files identical despite different names*

### Comparing `fern_persona-0.0.2/src/persona/types/retrieve_a_serpro_database_verification_response_data_attributes_checks_item.py` & `fern_persona-0.0.3/src/persona/types/retrieve_a_serpro_database_verification_response_data_attributes_checks_item.py`

 * *Files identical despite different names*

### Comparing `fern_persona-0.0.2/src/persona/types/retrieve_a_serpro_database_verification_response_data_attributes_checks_item_metadata.py` & `fern_persona-0.0.3/src/persona/types/retrieve_a_serpro_database_verification_response_data_attributes_checks_item_metadata.py`

 * *Files identical despite different names*

### Comparing `fern_persona-0.0.2/src/persona/types/retrieve_a_serpro_database_verification_response_data_relationships.py` & `fern_persona-0.0.3/src/persona/types/retrieve_a_serpro_database_verification_response_data_relationships.py`

 * *Files identical despite different names*

### Comparing `fern_persona-0.0.2/src/persona/types/retrieve_a_serpro_database_verification_response_data_relationships_inquiry.py` & `fern_persona-0.0.3/src/persona/types/retrieve_a_serpro_database_verification_response_data_relationships_inquiry.py`

 * *Files identical despite different names*

### Comparing `fern_persona-0.0.2/src/persona/types/retrieve_a_serpro_database_verification_response_data_relationships_selfie.py` & `fern_persona-0.0.3/src/persona/types/retrieve_a_serpro_database_verification_response_data_relationships_selfie.py`

 * *Files identical despite different names*

### Comparing `fern_persona-0.0.2/src/persona/types/retrieve_a_tin_database_verifications_response.py` & `fern_persona-0.0.3/src/persona/types/retrieve_a_tin_database_verifications_response.py`

 * *Files identical despite different names*

### Comparing `fern_persona-0.0.2/src/persona/types/retrieve_a_tin_database_verifications_response_data.py` & `fern_persona-0.0.3/src/persona/types/retrieve_a_tin_database_verifications_response_data.py`

 * *Files identical despite different names*

### Comparing `fern_persona-0.0.2/src/persona/types/retrieve_a_tin_database_verifications_response_data_attributes.py` & `fern_persona-0.0.3/src/persona/types/retrieve_a_tin_database_verifications_response_data_attributes.py`

 * *Files identical despite different names*

### Comparing `fern_persona-0.0.2/src/persona/types/retrieve_a_tin_database_verifications_response_data_attributes_checks_item.py` & `fern_persona-0.0.3/src/persona/types/retrieve_a_tin_database_verifications_response_data_attributes_checks_item.py`

 * *Files identical despite different names*

### Comparing `fern_persona-0.0.2/src/persona/types/retrieve_a_tin_database_verifications_response_data_attributes_checks_item_metadata.py` & `fern_persona-0.0.3/src/persona/types/retrieve_a_tin_database_verifications_response_data_attributes_checks_item_metadata.py`

 * *Files identical despite different names*

### Comparing `fern_persona-0.0.2/src/persona/types/retrieve_a_tin_database_verifications_response_data_relationships.py` & `fern_persona-0.0.3/src/persona/types/retrieve_a_tin_database_verifications_response_data_relationships.py`

 * *Files identical despite different names*

### Comparing `fern_persona-0.0.2/src/persona/types/retrieve_a_tin_database_verifications_response_data_relationships_inquiry.py` & `fern_persona-0.0.3/src/persona/types/retrieve_a_tin_database_verifications_response_data_relationships_inquiry.py`

 * *Files identical despite different names*

### Comparing `fern_persona-0.0.2/src/persona/types/retrieve_an_account_response.py` & `fern_persona-0.0.3/src/persona/types/retrieve_an_account_response.py`

 * *Files identical despite different names*

### Comparing `fern_persona-0.0.2/src/persona/types/retrieve_an_account_response_data.py` & `fern_persona-0.0.3/src/persona/types/retrieve_an_account_response_data.py`

 * *Files identical despite different names*

### Comparing `fern_persona-0.0.2/src/persona/types/retrieve_an_account_response_data_attributes.py` & `fern_persona-0.0.3/src/persona/types/retrieve_an_account_response_data_attributes.py`

 * *Files identical despite different names*

### Comparing `fern_persona-0.0.2/src/persona/types/retrieve_an_api_key_response.py` & `fern_persona-0.0.3/src/persona/types/retrieve_an_api_key_response.py`

 * *Files identical despite different names*

### Comparing `fern_persona-0.0.2/src/persona/types/retrieve_an_api_key_response_data.py` & `fern_persona-0.0.3/src/persona/types/retrieve_an_api_key_response_data.py`

 * *Files identical despite different names*

### Comparing `fern_persona-0.0.2/src/persona/types/retrieve_an_api_key_response_data_attributes.py` & `fern_persona-0.0.3/src/persona/types/retrieve_an_api_key_response_data_attributes.py`

 * *Files identical despite different names*

### Comparing `fern_persona-0.0.2/src/persona/types/retrieve_an_api_log_response.py` & `fern_persona-0.0.3/src/persona/types/retrieve_an_api_log_response.py`

 * *Files identical despite different names*

### Comparing `fern_persona-0.0.2/src/persona/types/retrieve_an_api_log_response_data.py` & `fern_persona-0.0.3/src/persona/types/retrieve_an_api_log_response_data.py`

 * *Files identical despite different names*

### Comparing `fern_persona-0.0.2/src/persona/types/retrieve_an_api_log_response_data_attributes.py` & `fern_persona-0.0.3/src/persona/types/retrieve_an_api_log_response_data_attributes.py`

 * *Files identical despite different names*

### Comparing `fern_persona-0.0.2/src/persona/types/retrieve_an_api_log_response_data_attributes_request.py` & `fern_persona-0.0.3/src/persona/types/retrieve_an_api_log_response_data_attributes_request.py`

 * *Files identical despite different names*

### Comparing `fern_persona-0.0.2/src/persona/types/retrieve_an_api_log_response_data_attributes_request_get_params.py` & `fern_persona-0.0.3/src/persona/types/retrieve_an_api_log_response_data_attributes_request_get_params.py`

 * *Files identical despite different names*

### Comparing `fern_persona-0.0.2/src/persona/types/retrieve_an_api_log_response_data_attributes_request_get_params_filter.py` & `fern_persona-0.0.3/src/persona/types/retrieve_an_api_log_response_data_attributes_request_get_params_filter.py`

 * *Files identical despite different names*

### Comparing `fern_persona-0.0.2/src/persona/types/retrieve_an_api_log_response_data_attributes_request_headers.py` & `fern_persona-0.0.3/src/persona/types/retrieve_an_api_log_response_data_attributes_request_headers.py`

 * *Files identical despite different names*

### Comparing `fern_persona-0.0.2/src/persona/types/retrieve_an_api_log_response_data_attributes_request_post_params.py` & `fern_persona-0.0.3/src/persona/types/retrieve_an_api_log_response_data_attributes_request_post_params.py`

 * *Files identical despite different names*

### Comparing `fern_persona-0.0.2/src/persona/types/retrieve_an_api_log_response_data_attributes_response.py` & `fern_persona-0.0.3/src/persona/types/retrieve_an_api_log_response_data_attributes_response.py`

 * *Files identical despite different names*

### Comparing `fern_persona-0.0.2/src/persona/types/retrieve_an_api_log_response_data_attributes_response_headers.py` & `fern_persona-0.0.3/src/persona/types/retrieve_an_api_log_response_data_attributes_response_headers.py`

 * *Files identical despite different names*

### Comparing `fern_persona-0.0.2/src/persona/types/retrieve_an_event_response.py` & `fern_persona-0.0.3/src/persona/types/retrieve_an_event_response.py`

 * *Files identical despite different names*

### Comparing `fern_persona-0.0.2/src/persona/types/retrieve_an_importer_response.py` & `fern_persona-0.0.3/src/persona/types/retrieve_an_importer_response.py`

 * *Files identical despite different names*

### Comparing `fern_persona-0.0.2/src/persona/types/retrieve_an_importer_response_data.py` & `fern_persona-0.0.3/src/persona/types/retrieve_an_importer_response_data.py`

 * *Files identical despite different names*

### Comparing `fern_persona-0.0.2/src/persona/types/retrieve_an_importer_response_data_attributes.py` & `fern_persona-0.0.3/src/persona/types/retrieve_an_importer_response_data_attributes.py`

 * *Files identical despite different names*

### Comparing `fern_persona-0.0.2/src/persona/types/retrieve_an_inquiry_response.py` & `fern_persona-0.0.3/src/persona/types/retrieve_an_inquiry_response.py`

 * *Files identical despite different names*

### Comparing `fern_persona-0.0.2/src/persona/types/retrieve_an_inquiry_response_data.py` & `fern_persona-0.0.3/src/persona/types/retrieve_an_inquiry_response_data.py`

 * *Files identical despite different names*

### Comparing `fern_persona-0.0.2/src/persona/types/retrieve_an_inquiry_response_data_attributes.py` & `fern_persona-0.0.3/src/persona/types/retrieve_an_inquiry_response_data_attributes.py`

 * *Files identical despite different names*

### Comparing `fern_persona-0.0.2/src/persona/types/retrieve_an_inquiry_response_data_attributes_behaviours.py` & `fern_persona-0.0.3/src/persona/types/retrieve_an_inquiry_response_data_attributes_behaviours.py`

 * *Files identical despite different names*

### Comparing `fern_persona-0.0.2/src/persona/types/retrieve_an_inquiry_response_data_attributes_fields.py` & `fern_persona-0.0.3/src/persona/types/retrieve_an_inquiry_response_data_attributes_fields.py`

 * *Files identical despite different names*

### Comparing `fern_persona-0.0.2/src/persona/types/retrieve_an_inquiry_response_data_attributes_fields_name_first.py` & `fern_persona-0.0.3/src/persona/types/retrieve_an_inquiry_response_data_attributes_fields_name_first.py`

 * *Files identical despite different names*

### Comparing `fern_persona-0.0.2/src/persona/types/retrieve_an_inquiry_response_data_attributes_fields_name_last.py` & `fern_persona-0.0.3/src/persona/types/retrieve_an_inquiry_response_data_attributes_fields_name_last.py`

 * *Files identical despite different names*

### Comparing `fern_persona-0.0.2/src/persona/types/retrieve_an_inquiry_response_data_relationships.py` & `fern_persona-0.0.3/src/persona/types/retrieve_an_inquiry_response_data_relationships.py`

 * *Files identical despite different names*

### Comparing `fern_persona-0.0.2/src/persona/types/retrieve_an_inquiry_response_data_relationships_account.py` & `fern_persona-0.0.3/src/persona/types/retrieve_an_inquiry_response_data_relationships_account.py`

 * *Files identical despite different names*

### Comparing `fern_persona-0.0.2/src/persona/types/retrieve_an_inquiry_response_data_relationships_account_data.py` & `fern_persona-0.0.3/src/persona/types/retrieve_an_inquiry_response_data_relationships_account_data.py`

 * *Files identical despite different names*

### Comparing `fern_persona-0.0.2/src/persona/types/retrieve_an_inquiry_response_data_relationships_reports.py` & `fern_persona-0.0.3/src/persona/types/retrieve_an_inquiry_response_data_relationships_reports.py`

 * *Files identical despite different names*

### Comparing `fern_persona-0.0.2/src/persona/types/retrieve_an_inquiry_response_data_relationships_sessions.py` & `fern_persona-0.0.3/src/persona/types/retrieve_an_inquiry_response_data_relationships_sessions.py`

 * *Files identical despite different names*

### Comparing `fern_persona-0.0.2/src/persona/types/retrieve_an_inquiry_response_data_relationships_sessions_data_item.py` & `fern_persona-0.0.3/src/persona/types/retrieve_an_inquiry_response_data_relationships_sessions_data_item.py`

 * *Files identical despite different names*

### Comparing `fern_persona-0.0.2/src/persona/types/retrieve_an_inquiry_response_data_relationships_template.py` & `fern_persona-0.0.3/src/persona/types/retrieve_an_inquiry_response_data_relationships_template.py`

 * *Files identical despite different names*

### Comparing `fern_persona-0.0.2/src/persona/types/retrieve_an_inquiry_response_data_relationships_template_data.py` & `fern_persona-0.0.3/src/persona/types/retrieve_an_inquiry_response_data_relationships_template_data.py`

 * *Files identical despite different names*

### Comparing `fern_persona-0.0.2/src/persona/types/retrieve_an_inquiry_response_data_relationships_verifications.py` & `fern_persona-0.0.3/src/persona/types/retrieve_an_inquiry_response_data_relationships_verifications.py`

 * *Files identical despite different names*

### Comparing `fern_persona-0.0.2/src/persona/types/retrieve_an_inquiry_response_data_relationships_verifications_data_item.py` & `fern_persona-0.0.3/src/persona/types/retrieve_an_inquiry_response_data_relationships_verifications_data_item.py`

 * *Files identical despite different names*

### Comparing `fern_persona-0.0.2/src/persona/types/retrieve_an_inquiry_response_included_item.py` & `fern_persona-0.0.3/src/persona/types/retrieve_an_inquiry_response_included_item.py`

 * *Files identical despite different names*

### Comparing `fern_persona-0.0.2/src/persona/types/retrieve_an_inquiry_response_included_item_attributes.py` & `fern_persona-0.0.3/src/persona/types/retrieve_an_inquiry_response_included_item_attributes.py`

 * *Files identical despite different names*

### Comparing `fern_persona-0.0.2/src/persona/types/retrieve_an_user_audit_log_response.py` & `fern_persona-0.0.3/src/persona/types/retrieve_an_user_audit_log_response.py`

 * *Files identical despite different names*

### Comparing `fern_persona-0.0.2/src/persona/types/retrieve_an_user_audit_log_response_data.py` & `fern_persona-0.0.3/src/persona/types/retrieve_an_user_audit_log_response_data.py`

 * *Files identical despite different names*

### Comparing `fern_persona-0.0.2/src/persona/types/retrieve_an_user_audit_log_response_data_attributes.py` & `fern_persona-0.0.3/src/persona/types/retrieve_an_user_audit_log_response_data_attributes.py`

 * *Files identical despite different names*

### Comparing `fern_persona-0.0.2/src/persona/types/retrieve_case_response.py` & `fern_persona-0.0.3/src/persona/types/retrieve_case_response.py`

 * *Files identical despite different names*

### Comparing `fern_persona-0.0.2/src/persona/types/retrieve_case_response_data.py` & `fern_persona-0.0.3/src/persona/types/retrieve_case_response_data.py`

 * *Files identical despite different names*

### Comparing `fern_persona-0.0.2/src/persona/types/retrieve_case_response_data_attributes.py` & `fern_persona-0.0.3/src/persona/types/retrieve_case_response_data_attributes.py`

 * *Files identical despite different names*

### Comparing `fern_persona-0.0.2/src/persona/types/retrieve_case_response_data_relationships.py` & `fern_persona-0.0.3/src/persona/types/retrieve_case_response_data_relationships.py`

 * *Files identical despite different names*

### Comparing `fern_persona-0.0.2/src/persona/types/retrieve_case_response_data_relationships_accounts.py` & `fern_persona-0.0.3/src/persona/types/retrieve_case_response_data_relationships_accounts.py`

 * *Files identical despite different names*

### Comparing `fern_persona-0.0.2/src/persona/types/retrieve_case_response_data_relationships_accounts_data_item.py` & `fern_persona-0.0.3/src/persona/types/retrieve_case_response_data_relationships_accounts_data_item.py`

 * *Files identical despite different names*

### Comparing `fern_persona-0.0.2/src/persona/types/retrieve_case_response_data_relationships_case_comments.py` & `fern_persona-0.0.3/src/persona/types/retrieve_case_response_data_relationships_case_comments.py`

 * *Files identical despite different names*

### Comparing `fern_persona-0.0.2/src/persona/types/retrieve_case_response_data_relationships_case_comments_data_item.py` & `fern_persona-0.0.3/src/persona/types/retrieve_case_response_data_relationships_case_comments_data_item.py`

 * *Files identical despite different names*

### Comparing `fern_persona-0.0.2/src/persona/types/retrieve_case_response_data_relationships_case_template.py` & `fern_persona-0.0.3/src/persona/types/retrieve_case_response_data_relationships_case_template.py`

 * *Files identical despite different names*

### Comparing `fern_persona-0.0.2/src/persona/types/retrieve_case_response_data_relationships_case_template_data.py` & `fern_persona-0.0.3/src/persona/types/retrieve_case_response_data_relationships_case_template_data.py`

 * *Files identical despite different names*

### Comparing `fern_persona-0.0.2/src/persona/types/retrieve_case_response_data_relationships_inquiries.py` & `fern_persona-0.0.3/src/persona/types/retrieve_case_response_data_relationships_inquiries.py`

 * *Files identical despite different names*

### Comparing `fern_persona-0.0.2/src/persona/types/retrieve_case_response_data_relationships_inquiries_data_item.py` & `fern_persona-0.0.3/src/persona/types/retrieve_case_response_data_relationships_inquiries_data_item.py`

 * *Files identical despite different names*

### Comparing `fern_persona-0.0.2/src/persona/types/retrieve_case_response_data_relationships_reports.py` & `fern_persona-0.0.3/src/persona/types/retrieve_case_response_data_relationships_reports.py`

 * *Files identical despite different names*

### Comparing `fern_persona-0.0.2/src/persona/types/retrieve_case_response_included_item.py` & `fern_persona-0.0.3/src/persona/types/retrieve_case_response_included_item.py`

 * *Files identical despite different names*

### Comparing `fern_persona-0.0.2/src/persona/types/retrieve_case_response_included_item_attributes.py` & `fern_persona-0.0.3/src/persona/types/retrieve_case_response_included_item_attributes.py`

 * *Files identical despite different names*

### Comparing `fern_persona-0.0.2/src/persona/types/send_an_email_request_data.py` & `fern_persona-0.0.3/src/persona/types/send_an_email_request_data.py`

 * *Files identical despite different names*

### Comparing `fern_persona-0.0.2/src/persona/types/send_an_email_request_data_attributes.py` & `fern_persona-0.0.3/src/persona/types/send_an_email_request_data_attributes.py`

 * *Files identical despite different names*

### Comparing `fern_persona-0.0.2/src/persona/types/send_an_email_response.py` & `fern_persona-0.0.3/src/persona/types/send_an_email_response.py`

 * *Files identical despite different names*

### Comparing `fern_persona-0.0.2/src/persona/types/send_an_email_response_data.py` & `fern_persona-0.0.3/src/persona/types/send_an_email_response_data.py`

 * *Files identical despite different names*

### Comparing `fern_persona-0.0.2/src/persona/types/send_an_email_response_data_attributes.py` & `fern_persona-0.0.3/src/persona/types/send_an_email_response_data_attributes.py`

 * *Files identical despite different names*

### Comparing `fern_persona-0.0.2/src/persona/types/send_an_email_response_data_attributes_metadata.py` & `fern_persona-0.0.3/src/persona/types/send_an_email_response_data_attributes_metadata.py`

 * *Files identical despite different names*

### Comparing `fern_persona-0.0.2/src/persona/types/send_an_sms_request_data.py` & `fern_persona-0.0.3/src/persona/types/send_an_sms_request_data.py`

 * *Files identical despite different names*

### Comparing `fern_persona-0.0.2/src/persona/types/send_an_sms_request_data_attributes.py` & `fern_persona-0.0.3/src/persona/types/send_an_sms_request_data_attributes.py`

 * *Files identical despite different names*

### Comparing `fern_persona-0.0.2/src/persona/types/send_an_sms_response.py` & `fern_persona-0.0.3/src/persona/types/send_an_sms_response.py`

 * *Files identical despite different names*

### Comparing `fern_persona-0.0.2/src/persona/types/send_an_sms_response_data.py` & `fern_persona-0.0.3/src/persona/types/send_an_sms_response_data.py`

 * *Files identical despite different names*

### Comparing `fern_persona-0.0.2/src/persona/types/send_an_sms_response_data_attributes.py` & `fern_persona-0.0.3/src/persona/types/send_an_sms_response_data_attributes.py`

 * *Files identical despite different names*

### Comparing `fern_persona-0.0.2/src/persona/types/send_an_sms_response_data_attributes_metadata.py` & `fern_persona-0.0.3/src/persona/types/send_an_sms_response_data_attributes_metadata.py`

 * *Files identical despite different names*

### Comparing `fern_persona-0.0.2/src/persona/types/set_all_tags_1_request_meta.py` & `fern_persona-0.0.3/src/persona/types/set_all_tags_1_request_meta.py`

 * *Files identical despite different names*

### Comparing `fern_persona-0.0.2/src/persona/types/set_all_tags_request_meta.py` & `fern_persona-0.0.3/src/persona/types/set_all_tags_request_meta.py`

 * *Files identical despite different names*

### Comparing `fern_persona-0.0.2/src/persona/types/set_status_for_a_case_request_meta.py` & `fern_persona-0.0.3/src/persona/types/set_status_for_a_case_request_meta.py`

 * *Files identical despite different names*

### Comparing `fern_persona-0.0.2/src/persona/types/set_status_for_a_case_response.py` & `fern_persona-0.0.3/src/persona/types/set_status_for_a_case_response.py`

 * *Files identical despite different names*

### Comparing `fern_persona-0.0.2/src/persona/types/set_status_for_a_case_response_data.py` & `fern_persona-0.0.3/src/persona/types/set_status_for_a_case_response_data.py`

 * *Files identical despite different names*

### Comparing `fern_persona-0.0.2/src/persona/types/set_status_for_a_case_response_data_attributes.py` & `fern_persona-0.0.3/src/persona/types/set_status_for_a_case_response_data_attributes.py`

 * *Files identical despite different names*

### Comparing `fern_persona-0.0.2/src/persona/types/set_status_for_a_case_response_data_relationships.py` & `fern_persona-0.0.3/src/persona/types/set_status_for_a_case_response_data_relationships.py`

 * *Files identical despite different names*

### Comparing `fern_persona-0.0.2/src/persona/types/set_status_for_a_case_response_data_relationships_accounts.py` & `fern_persona-0.0.3/src/persona/types/set_status_for_a_case_response_data_relationships_accounts.py`

 * *Files identical despite different names*

### Comparing `fern_persona-0.0.2/src/persona/types/set_status_for_a_case_response_data_relationships_case_comments.py` & `fern_persona-0.0.3/src/persona/types/set_status_for_a_case_response_data_relationships_case_comments.py`

 * *Files identical despite different names*

### Comparing `fern_persona-0.0.2/src/persona/types/set_status_for_a_case_response_data_relationships_case_template.py` & `fern_persona-0.0.3/src/persona/types/set_status_for_a_case_response_data_relationships_case_template.py`

 * *Files identical despite different names*

### Comparing `fern_persona-0.0.2/src/persona/types/set_status_for_a_case_response_data_relationships_case_template_data.py` & `fern_persona-0.0.3/src/persona/types/set_status_for_a_case_response_data_relationships_case_template_data.py`

 * *Files identical despite different names*

### Comparing `fern_persona-0.0.2/src/persona/types/set_status_for_a_case_response_data_relationships_inquiries.py` & `fern_persona-0.0.3/src/persona/types/set_status_for_a_case_response_data_relationships_inquiries.py`

 * *Files identical despite different names*

### Comparing `fern_persona-0.0.2/src/persona/types/set_status_for_a_case_response_data_relationships_inquiries_data_item.py` & `fern_persona-0.0.3/src/persona/types/set_status_for_a_case_response_data_relationships_inquiries_data_item.py`

 * *Files identical despite different names*

### Comparing `fern_persona-0.0.2/src/persona/types/set_status_for_a_case_response_data_relationships_reports.py` & `fern_persona-0.0.3/src/persona/types/set_status_for_a_case_response_data_relationships_reports.py`

 * *Files identical despite different names*

### Comparing `fern_persona-0.0.2/src/persona/types/set_status_for_a_case_response_data_relationships_reports_data_item.py` & `fern_persona-0.0.3/src/persona/types/set_status_for_a_case_response_data_relationships_reports_data_item.py`

 * *Files identical despite different names*

### Comparing `fern_persona-0.0.2/src/persona/types/submit_a_document_response.py` & `fern_persona-0.0.3/src/persona/types/submit_a_document_response.py`

 * *Files identical despite different names*

### Comparing `fern_persona-0.0.2/src/persona/types/submit_a_document_response_data.py` & `fern_persona-0.0.3/src/persona/types/submit_a_document_response_data.py`

 * *Files identical despite different names*

### Comparing `fern_persona-0.0.2/src/persona/types/submit_a_document_response_data_attributes.py` & `fern_persona-0.0.3/src/persona/types/submit_a_document_response_data_attributes.py`

 * *Files identical despite different names*

### Comparing `fern_persona-0.0.2/src/persona/types/submit_a_document_response_data_attributes_files_item.py` & `fern_persona-0.0.3/src/persona/types/submit_a_document_response_data_attributes_files_item.py`

 * *Files identical despite different names*

### Comparing `fern_persona-0.0.2/src/persona/types/submit_a_document_response_data_relationships.py` & `fern_persona-0.0.3/src/persona/types/submit_a_document_response_data_relationships.py`

 * *Files identical despite different names*

### Comparing `fern_persona-0.0.2/src/persona/types/submit_a_document_response_data_relationships_inquiry.py` & `fern_persona-0.0.3/src/persona/types/submit_a_document_response_data_relationships_inquiry.py`

 * *Files identical despite different names*

### Comparing `fern_persona-0.0.2/src/persona/types/submit_a_document_response_data_relationships_inquiry_data.py` & `fern_persona-0.0.3/src/persona/types/submit_a_document_response_data_relationships_inquiry_data.py`

 * *Files identical despite different names*

### Comparing `fern_persona-0.0.2/src/persona/types/submit_a_document_verification_response.py` & `fern_persona-0.0.3/src/persona/types/submit_a_document_verification_response.py`

 * *Files identical despite different names*

### Comparing `fern_persona-0.0.2/src/persona/types/submit_a_document_verification_response_data.py` & `fern_persona-0.0.3/src/persona/types/submit_a_document_verification_response_data.py`

 * *Files identical despite different names*

### Comparing `fern_persona-0.0.2/src/persona/types/submit_a_document_verification_response_data_attributes.py` & `fern_persona-0.0.3/src/persona/types/submit_a_document_verification_response_data_attributes.py`

 * *Files identical despite different names*

### Comparing `fern_persona-0.0.2/src/persona/types/submit_a_document_verification_response_data_relationships.py` & `fern_persona-0.0.3/src/persona/types/submit_a_document_verification_response_data_relationships.py`

 * *Files identical despite different names*

### Comparing `fern_persona-0.0.2/src/persona/types/submit_a_document_verification_response_data_relationships_document.py` & `fern_persona-0.0.3/src/persona/types/submit_a_document_verification_response_data_relationships_document.py`

 * *Files identical despite different names*

### Comparing `fern_persona-0.0.2/src/persona/types/submit_a_document_verification_response_data_relationships_document_data.py` & `fern_persona-0.0.3/src/persona/types/submit_a_document_verification_response_data_relationships_document_data.py`

 * *Files identical despite different names*

### Comparing `fern_persona-0.0.2/src/persona/types/submit_a_document_verification_response_data_relationships_inquiry.py` & `fern_persona-0.0.3/src/persona/types/submit_a_document_verification_response_data_relationships_inquiry.py`

 * *Files identical despite different names*

### Comparing `fern_persona-0.0.2/src/persona/types/submit_a_document_verification_response_data_relationships_inquiry_data.py` & `fern_persona-0.0.3/src/persona/types/submit_a_document_verification_response_data_relationships_inquiry_data.py`

 * *Files identical despite different names*

### Comparing `fern_persona-0.0.2/src/persona/types/submit_a_government_id_document_response.py` & `fern_persona-0.0.3/src/persona/types/submit_a_government_id_document_response.py`

 * *Files identical despite different names*

### Comparing `fern_persona-0.0.2/src/persona/types/submit_a_government_id_document_response_data.py` & `fern_persona-0.0.3/src/persona/types/submit_a_government_id_document_response_data.py`

 * *Files identical despite different names*

### Comparing `fern_persona-0.0.2/src/persona/types/submit_a_government_id_document_response_data_attributes.py` & `fern_persona-0.0.3/src/persona/types/submit_a_government_id_document_response_data_attributes.py`

 * *Files identical despite different names*

### Comparing `fern_persona-0.0.2/src/persona/types/submit_a_government_id_document_response_data_relationships.py` & `fern_persona-0.0.3/src/persona/types/submit_a_government_id_document_response_data_relationships.py`

 * *Files identical despite different names*

### Comparing `fern_persona-0.0.2/src/persona/types/submit_a_government_id_document_response_data_relationships_inquiry.py` & `fern_persona-0.0.3/src/persona/types/submit_a_government_id_document_response_data_relationships_inquiry.py`

 * *Files identical despite different names*

### Comparing `fern_persona-0.0.2/src/persona/types/submit_a_government_id_document_response_data_relationships_inquiry_data.py` & `fern_persona-0.0.3/src/persona/types/submit_a_government_id_document_response_data_relationships_inquiry_data.py`

 * *Files identical despite different names*

### Comparing `fern_persona-0.0.2/src/persona/types/submit_a_government_id_verification_response.py` & `fern_persona-0.0.3/src/persona/types/submit_a_government_id_verification_response.py`

 * *Files identical despite different names*

### Comparing `fern_persona-0.0.2/src/persona/types/submit_a_government_id_verification_response_data.py` & `fern_persona-0.0.3/src/persona/types/submit_a_government_id_verification_response_data.py`

 * *Files identical despite different names*

### Comparing `fern_persona-0.0.2/src/persona/types/submit_a_government_id_verification_response_data_attributes.py` & `fern_persona-0.0.3/src/persona/types/submit_a_government_id_verification_response_data_attributes.py`

 * *Files identical despite different names*

### Comparing `fern_persona-0.0.2/src/persona/types/submit_a_government_id_verification_response_data_relationships.py` & `fern_persona-0.0.3/src/persona/types/submit_a_government_id_verification_response_data_relationships.py`

 * *Files identical despite different names*

### Comparing `fern_persona-0.0.2/src/persona/types/submit_a_government_id_verification_response_data_relationships_document.py` & `fern_persona-0.0.3/src/persona/types/submit_a_government_id_verification_response_data_relationships_document.py`

 * *Files identical despite different names*

### Comparing `fern_persona-0.0.2/src/persona/types/submit_a_government_id_verification_response_data_relationships_document_data.py` & `fern_persona-0.0.3/src/persona/types/submit_a_government_id_verification_response_data_relationships_document_data.py`

 * *Files identical despite different names*

### Comparing `fern_persona-0.0.2/src/persona/types/submit_a_government_id_verification_response_data_relationships_inquiry.py` & `fern_persona-0.0.3/src/persona/types/submit_a_government_id_verification_response_data_relationships_inquiry.py`

 * *Files identical despite different names*

### Comparing `fern_persona-0.0.2/src/persona/types/submit_a_phone_carrier_database_verification_response.py` & `fern_persona-0.0.3/src/persona/types/submit_a_phone_carrier_database_verification_response.py`

 * *Files identical despite different names*

### Comparing `fern_persona-0.0.2/src/persona/types/submit_a_phone_carrier_database_verification_response_data.py` & `fern_persona-0.0.3/src/persona/types/submit_a_phone_carrier_database_verification_response_data.py`

 * *Files identical despite different names*

### Comparing `fern_persona-0.0.2/src/persona/types/submit_a_phone_carrier_database_verification_response_data_attributes.py` & `fern_persona-0.0.3/src/persona/types/submit_a_phone_carrier_database_verification_response_data_attributes.py`

 * *Files identical despite different names*

### Comparing `fern_persona-0.0.2/src/persona/types/submit_a_phone_carrier_database_verification_response_data_relationships.py` & `fern_persona-0.0.3/src/persona/types/submit_a_phone_carrier_database_verification_response_data_relationships.py`

 * *Files identical despite different names*

### Comparing `fern_persona-0.0.2/src/persona/types/submit_a_phone_carrier_database_verification_response_data_relationships_inquiry.py` & `fern_persona-0.0.3/src/persona/types/submit_a_phone_carrier_database_verification_response_data_relationships_inquiry.py`

 * *Files identical despite different names*

### Comparing `fern_persona-0.0.2/src/persona/types/submit_a_selfie_verification_response.py` & `fern_persona-0.0.3/src/persona/types/submit_a_selfie_verification_response.py`

 * *Files identical despite different names*

### Comparing `fern_persona-0.0.2/src/persona/types/submit_a_selfie_verification_response_data.py` & `fern_persona-0.0.3/src/persona/types/submit_a_selfie_verification_response_data.py`

 * *Files identical despite different names*

### Comparing `fern_persona-0.0.2/src/persona/types/submit_a_selfie_verification_response_data_attributes.py` & `fern_persona-0.0.3/src/persona/types/submit_a_selfie_verification_response_data_attributes.py`

 * *Files identical despite different names*

### Comparing `fern_persona-0.0.2/src/persona/types/submit_a_selfie_verification_response_data_relationships.py` & `fern_persona-0.0.3/src/persona/types/submit_a_selfie_verification_response_data_relationships.py`

 * *Files identical despite different names*

### Comparing `fern_persona-0.0.2/src/persona/types/submit_a_selfie_verification_response_data_relationships_inquiry.py` & `fern_persona-0.0.3/src/persona/types/submit_a_selfie_verification_response_data_relationships_inquiry.py`

 * *Files identical despite different names*

### Comparing `fern_persona-0.0.2/src/persona/types/submit_a_serpro_database_verification_response.py` & `fern_persona-0.0.3/src/persona/types/submit_a_serpro_database_verification_response.py`

 * *Files identical despite different names*

### Comparing `fern_persona-0.0.2/src/persona/types/submit_a_serpro_database_verification_response_data.py` & `fern_persona-0.0.3/src/persona/types/submit_a_serpro_database_verification_response_data.py`

 * *Files identical despite different names*

### Comparing `fern_persona-0.0.2/src/persona/types/submit_a_serpro_database_verification_response_data_attributes.py` & `fern_persona-0.0.3/src/persona/types/submit_a_serpro_database_verification_response_data_attributes.py`

 * *Files identical despite different names*

### Comparing `fern_persona-0.0.2/src/persona/types/submit_a_serpro_database_verification_response_data_relationships.py` & `fern_persona-0.0.3/src/persona/types/submit_a_serpro_database_verification_response_data_relationships.py`

 * *Files identical despite different names*

### Comparing `fern_persona-0.0.2/src/persona/types/submit_a_serpro_database_verification_response_data_relationships_inquiry.py` & `fern_persona-0.0.3/src/persona/types/submit_a_serpro_database_verification_response_data_relationships_inquiry.py`

 * *Files identical despite different names*

### Comparing `fern_persona-0.0.2/src/persona/types/submit_a_serpro_database_verification_response_data_relationships_selfie.py` & `fern_persona-0.0.3/src/persona/types/submit_a_serpro_database_verification_response_data_relationships_selfie.py`

 * *Files identical despite different names*

### Comparing `fern_persona-0.0.2/src/persona/types/submit_a_tin_database_verifications_response.py` & `fern_persona-0.0.3/src/persona/types/submit_a_tin_database_verifications_response.py`

 * *Files identical despite different names*

### Comparing `fern_persona-0.0.2/src/persona/types/submit_a_tin_database_verifications_response_data.py` & `fern_persona-0.0.3/src/persona/types/submit_a_tin_database_verifications_response_data.py`

 * *Files identical despite different names*

### Comparing `fern_persona-0.0.2/src/persona/types/submit_a_tin_database_verifications_response_data_attributes.py` & `fern_persona-0.0.3/src/persona/types/submit_a_tin_database_verifications_response_data_attributes.py`

 * *Files identical despite different names*

### Comparing `fern_persona-0.0.2/src/persona/types/submit_a_tin_database_verifications_response_data_relationships.py` & `fern_persona-0.0.3/src/persona/types/submit_a_tin_database_verifications_response_data_relationships.py`

 * *Files identical despite different names*

### Comparing `fern_persona-0.0.2/src/persona/types/submit_a_tin_database_verifications_response_data_relationships_inquiry.py` & `fern_persona-0.0.3/src/persona/types/submit_a_tin_database_verifications_response_data_relationships_inquiry.py`

 * *Files identical despite different names*

### Comparing `fern_persona-0.0.2/src/persona/types/unprocessable_entity_error_body.py` & `fern_persona-0.0.3/src/persona/types/unprocessable_entity_error_body.py`

 * *Files identical despite different names*

### Comparing `fern_persona-0.0.2/src/persona/types/unprocessable_entity_error_body_errors_item.py` & `fern_persona-0.0.3/src/persona/types/unprocessable_entity_error_body_errors_item.py`

 * *Files identical despite different names*

### Comparing `fern_persona-0.0.2/src/persona/types/update_a_case_request_data.py` & `fern_persona-0.0.3/src/persona/types/update_a_case_request_data.py`

 * *Files identical despite different names*

### Comparing `fern_persona-0.0.2/src/persona/types/update_a_case_request_data_attributes.py` & `fern_persona-0.0.3/src/persona/types/update_a_case_request_data_attributes.py`

 * *Files identical despite different names*

### Comparing `fern_persona-0.0.2/src/persona/types/update_a_case_request_data_attributes_attachments_item.py` & `fern_persona-0.0.3/src/persona/types/update_a_case_request_data_attributes_attachments_item.py`

 * *Files identical despite different names*

### Comparing `fern_persona-0.0.2/src/persona/types/update_a_case_request_data_attributes_fields.py` & `fern_persona-0.0.3/src/persona/types/update_a_case_request_data_attributes_fields.py`

 * *Files identical despite different names*

### Comparing `fern_persona-0.0.2/src/persona/types/update_a_case_response.py` & `fern_persona-0.0.3/src/persona/types/update_a_case_response.py`

 * *Files identical despite different names*

### Comparing `fern_persona-0.0.2/src/persona/types/update_a_case_response_data.py` & `fern_persona-0.0.3/src/persona/types/update_a_case_response_data.py`

 * *Files identical despite different names*

### Comparing `fern_persona-0.0.2/src/persona/types/update_a_case_response_data_attributes.py` & `fern_persona-0.0.3/src/persona/types/update_a_case_response_data_attributes.py`

 * *Files identical despite different names*

### Comparing `fern_persona-0.0.2/src/persona/types/update_a_case_response_data_relationships.py` & `fern_persona-0.0.3/src/persona/types/update_a_case_response_data_relationships.py`

 * *Files identical despite different names*

### Comparing `fern_persona-0.0.2/src/persona/types/update_a_case_response_data_relationships_accounts.py` & `fern_persona-0.0.3/src/persona/types/update_a_case_response_data_relationships_accounts.py`

 * *Files identical despite different names*

### Comparing `fern_persona-0.0.2/src/persona/types/update_a_case_response_data_relationships_case_comments.py` & `fern_persona-0.0.3/src/persona/types/update_a_case_response_data_relationships_case_comments.py`

 * *Files identical despite different names*

### Comparing `fern_persona-0.0.2/src/persona/types/update_a_case_response_data_relationships_case_template.py` & `fern_persona-0.0.3/src/persona/types/update_a_case_response_data_relationships_case_template.py`

 * *Files identical despite different names*

### Comparing `fern_persona-0.0.2/src/persona/types/update_a_case_response_data_relationships_case_template_data.py` & `fern_persona-0.0.3/src/persona/types/update_a_case_response_data_relationships_case_template_data.py`

 * *Files identical despite different names*

### Comparing `fern_persona-0.0.2/src/persona/types/update_a_case_response_data_relationships_inquiries.py` & `fern_persona-0.0.3/src/persona/types/update_a_case_response_data_relationships_inquiries.py`

 * *Files identical despite different names*

### Comparing `fern_persona-0.0.2/src/persona/types/update_a_case_response_data_relationships_inquiries_data_item.py` & `fern_persona-0.0.3/src/persona/types/update_a_case_response_data_relationships_inquiries_data_item.py`

 * *Files identical despite different names*

### Comparing `fern_persona-0.0.2/src/persona/types/update_a_case_response_data_relationships_reports.py` & `fern_persona-0.0.3/src/persona/types/update_a_case_response_data_relationships_reports.py`

 * *Files identical despite different names*

### Comparing `fern_persona-0.0.2/src/persona/types/update_a_case_response_data_relationships_reports_data_item.py` & `fern_persona-0.0.3/src/persona/types/update_a_case_response_data_relationships_reports_data_item.py`

 * *Files identical despite different names*

### Comparing `fern_persona-0.0.2/src/persona/types/update_a_document_request_data.py` & `fern_persona-0.0.3/src/persona/types/update_a_document_request_data.py`

 * *Files identical despite different names*

### Comparing `fern_persona-0.0.2/src/persona/types/update_a_document_request_data_attributes.py` & `fern_persona-0.0.3/src/persona/types/update_a_document_request_data_attributes.py`

 * *Files identical despite different names*

### Comparing `fern_persona-0.0.2/src/persona/types/update_a_document_response.py` & `fern_persona-0.0.3/src/persona/types/update_a_document_response.py`

 * *Files identical despite different names*

### Comparing `fern_persona-0.0.2/src/persona/types/update_a_document_response_data.py` & `fern_persona-0.0.3/src/persona/types/update_a_document_response_data.py`

 * *Files identical despite different names*

### Comparing `fern_persona-0.0.2/src/persona/types/update_a_document_response_data_attributes.py` & `fern_persona-0.0.3/src/persona/types/update_a_document_response_data_attributes.py`

 * *Files identical despite different names*

### Comparing `fern_persona-0.0.2/src/persona/types/update_a_document_response_data_attributes_files_item.py` & `fern_persona-0.0.3/src/persona/types/update_a_document_response_data_attributes_files_item.py`

 * *Files identical despite different names*

### Comparing `fern_persona-0.0.2/src/persona/types/update_a_document_response_data_relationships.py` & `fern_persona-0.0.3/src/persona/types/update_a_document_response_data_relationships.py`

 * *Files identical despite different names*

### Comparing `fern_persona-0.0.2/src/persona/types/update_a_document_response_data_relationships_inquiry.py` & `fern_persona-0.0.3/src/persona/types/update_a_document_response_data_relationships_inquiry.py`

 * *Files identical despite different names*

### Comparing `fern_persona-0.0.2/src/persona/types/update_a_document_response_data_relationships_inquiry_data.py` & `fern_persona-0.0.3/src/persona/types/update_a_document_response_data_relationships_inquiry_data.py`

 * *Files identical despite different names*

### Comparing `fern_persona-0.0.2/src/persona/types/update_a_government_id_document_request_data.py` & `fern_persona-0.0.3/src/persona/types/update_a_government_id_document_request_data.py`

 * *Files identical despite different names*

### Comparing `fern_persona-0.0.2/src/persona/types/update_a_government_id_document_request_data_attributes.py` & `fern_persona-0.0.3/src/persona/types/update_a_government_id_document_request_data_attributes.py`

 * *Files identical despite different names*

### Comparing `fern_persona-0.0.2/src/persona/types/update_a_government_id_document_request_data_attributes_back_photo.py` & `fern_persona-0.0.3/src/persona/types/update_a_government_id_document_request_data_attributes_back_photo.py`

 * *Files identical despite different names*

### Comparing `fern_persona-0.0.2/src/persona/types/update_a_government_id_document_request_data_attributes_back_photo_data.py` & `fern_persona-0.0.3/src/persona/types/update_a_government_id_document_request_data_attributes_back_photo_data.py`

 * *Files identical despite different names*

### Comparing `fern_persona-0.0.2/src/persona/types/update_a_government_id_document_request_data_attributes_front_photo.py` & `fern_persona-0.0.3/src/persona/types/update_a_government_id_document_request_data_attributes_front_photo.py`

 * *Files identical despite different names*

### Comparing `fern_persona-0.0.2/src/persona/types/update_a_government_id_document_request_data_attributes_front_photo_data.py` & `fern_persona-0.0.3/src/persona/types/update_a_government_id_document_request_data_attributes_front_photo_data.py`

 * *Files identical despite different names*

### Comparing `fern_persona-0.0.2/src/persona/types/update_a_government_id_document_response.py` & `fern_persona-0.0.3/src/persona/types/update_a_government_id_document_response.py`

 * *Files identical despite different names*

### Comparing `fern_persona-0.0.2/src/persona/types/update_a_government_id_document_response_data.py` & `fern_persona-0.0.3/src/persona/types/update_a_government_id_document_response_data.py`

 * *Files identical despite different names*

### Comparing `fern_persona-0.0.2/src/persona/types/update_a_government_id_document_response_data_attributes.py` & `fern_persona-0.0.3/src/persona/types/update_a_government_id_document_response_data_attributes.py`

 * *Files identical despite different names*

### Comparing `fern_persona-0.0.2/src/persona/types/update_a_government_id_document_response_data_relationships.py` & `fern_persona-0.0.3/src/persona/types/update_a_government_id_document_response_data_relationships.py`

 * *Files identical despite different names*

### Comparing `fern_persona-0.0.2/src/persona/types/update_a_government_id_document_response_data_relationships_inquiry.py` & `fern_persona-0.0.3/src/persona/types/update_a_government_id_document_response_data_relationships_inquiry.py`

 * *Files identical despite different names*

### Comparing `fern_persona-0.0.2/src/persona/types/update_a_government_id_document_response_data_relationships_inquiry_data.py` & `fern_persona-0.0.3/src/persona/types/update_a_government_id_document_response_data_relationships_inquiry_data.py`

 * *Files identical despite different names*

### Comparing `fern_persona-0.0.2/src/persona/types/update_a_government_id_verification_request_data.py` & `fern_persona-0.0.3/src/persona/types/update_a_government_id_verification_request_data.py`

 * *Files identical despite different names*

### Comparing `fern_persona-0.0.2/src/persona/types/update_a_government_id_verification_request_data_attributes.py` & `fern_persona-0.0.3/src/persona/types/update_a_government_id_verification_request_data_attributes.py`

 * *Files identical despite different names*

### Comparing `fern_persona-0.0.2/src/persona/types/update_a_government_id_verification_request_data_attributes_back_photo.py` & `fern_persona-0.0.3/src/persona/types/update_a_government_id_verification_request_data_attributes_back_photo.py`

 * *Files identical despite different names*

### Comparing `fern_persona-0.0.2/src/persona/types/update_a_government_id_verification_request_data_attributes_back_photo_data.py` & `fern_persona-0.0.3/src/persona/types/update_a_government_id_verification_request_data_attributes_back_photo_data.py`

 * *Files identical despite different names*

### Comparing `fern_persona-0.0.2/src/persona/types/update_a_government_id_verification_request_data_attributes_front_photo.py` & `fern_persona-0.0.3/src/persona/types/update_a_government_id_verification_request_data_attributes_front_photo.py`

 * *Files identical despite different names*

### Comparing `fern_persona-0.0.2/src/persona/types/update_a_government_id_verification_request_data_attributes_front_photo_data.py` & `fern_persona-0.0.3/src/persona/types/update_a_government_id_verification_request_data_attributes_front_photo_data.py`

 * *Files identical despite different names*

### Comparing `fern_persona-0.0.2/src/persona/types/update_a_government_id_verification_response.py` & `fern_persona-0.0.3/src/persona/types/update_a_government_id_verification_response.py`

 * *Files identical despite different names*

### Comparing `fern_persona-0.0.2/src/persona/types/update_a_government_id_verification_response_data.py` & `fern_persona-0.0.3/src/persona/types/update_a_government_id_verification_response_data.py`

 * *Files identical despite different names*

### Comparing `fern_persona-0.0.2/src/persona/types/update_a_government_id_verification_response_data_attributes.py` & `fern_persona-0.0.3/src/persona/types/update_a_government_id_verification_response_data_attributes.py`

 * *Files identical despite different names*

### Comparing `fern_persona-0.0.2/src/persona/types/update_a_government_id_verification_response_data_relationships.py` & `fern_persona-0.0.3/src/persona/types/update_a_government_id_verification_response_data_relationships.py`

 * *Files identical despite different names*

### Comparing `fern_persona-0.0.2/src/persona/types/update_a_government_id_verification_response_data_relationships_inquiry.py` & `fern_persona-0.0.3/src/persona/types/update_a_government_id_verification_response_data_relationships_inquiry.py`

 * *Files identical despite different names*

### Comparing `fern_persona-0.0.2/src/persona/types/update_a_government_id_verification_response_data_relationships_inquiry_data.py` & `fern_persona-0.0.3/src/persona/types/update_a_government_id_verification_response_data_relationships_inquiry_data.py`

 * *Files identical despite different names*

### Comparing `fern_persona-0.0.2/src/persona/types/update_an_account_request_data.py` & `fern_persona-0.0.3/src/persona/types/update_an_account_request_data.py`

 * *Files identical despite different names*

### Comparing `fern_persona-0.0.2/src/persona/types/update_an_account_request_data_attributes.py` & `fern_persona-0.0.3/src/persona/types/update_an_account_request_data_attributes.py`

 * *Files identical despite different names*

### Comparing `fern_persona-0.0.2/src/persona/types/update_an_account_request_data_attributes_selfie_photo.py` & `fern_persona-0.0.3/src/persona/types/update_an_account_request_data_attributes_selfie_photo.py`

 * *Files identical despite different names*

### Comparing `fern_persona-0.0.2/src/persona/types/update_an_account_request_data_attributes_selfie_photo_data.py` & `fern_persona-0.0.3/src/persona/types/update_an_account_request_data_attributes_selfie_photo_data.py`

 * *Files identical despite different names*

### Comparing `fern_persona-0.0.2/src/persona/types/update_an_account_response.py` & `fern_persona-0.0.3/src/persona/types/update_an_account_response.py`

 * *Files identical despite different names*

### Comparing `fern_persona-0.0.2/src/persona/types/update_an_account_response_data.py` & `fern_persona-0.0.3/src/persona/types/update_an_account_response_data.py`

 * *Files identical despite different names*

### Comparing `fern_persona-0.0.2/src/persona/types/update_an_account_response_data_attributes.py` & `fern_persona-0.0.3/src/persona/types/update_an_account_response_data_attributes.py`

 * *Files identical despite different names*

### Comparing `fern_persona-0.0.2/src/persona/types/update_an_api_key_request_data.py` & `fern_persona-0.0.3/src/persona/types/update_an_api_key_request_data.py`

 * *Files identical despite different names*

### Comparing `fern_persona-0.0.2/src/persona/types/update_an_api_key_request_data_attributes.py` & `fern_persona-0.0.3/src/persona/types/update_an_api_key_request_data_attributes.py`

 * *Files identical despite different names*

### Comparing `fern_persona-0.0.2/src/persona/types/update_an_api_key_response.py` & `fern_persona-0.0.3/src/persona/types/update_an_api_key_response.py`

 * *Files identical despite different names*

### Comparing `fern_persona-0.0.2/src/persona/types/update_an_api_key_response_data.py` & `fern_persona-0.0.3/src/persona/types/update_an_api_key_response_data.py`

 * *Files identical despite different names*

### Comparing `fern_persona-0.0.2/src/persona/types/update_an_api_key_response_data_attributes.py` & `fern_persona-0.0.3/src/persona/types/update_an_api_key_response_data_attributes.py`

 * *Files identical despite different names*

### Comparing `fern_persona-0.0.2/src/persona/types/update_an_inquiry_request_data.py` & `fern_persona-0.0.3/src/persona/types/update_an_inquiry_request_data.py`

 * *Files identical despite different names*

### Comparing `fern_persona-0.0.2/src/persona/types/update_an_inquiry_request_data_attributes.py` & `fern_persona-0.0.3/src/persona/types/update_an_inquiry_request_data_attributes.py`

 * *Files identical despite different names*

### Comparing `fern_persona-0.0.2/PKG-INFO` & `fern_persona-0.0.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fern-persona
-Version: 0.0.2
+Version: 0.0.3
 Summary: 
 Requires-Python: >=3.7,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
```

