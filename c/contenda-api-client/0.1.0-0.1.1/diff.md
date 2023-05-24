# Comparing `tmp/contenda-api-client-0.1.0.tar.gz` & `tmp/contenda-api-client-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "contenda-api-client-0.1.0.tar", max compression
+gzip compressed data, was "contenda-api-client-0.1.1.tar", max compression
```

## Comparing `contenda-api-client-0.1.0.tar` & `contenda-api-client-0.1.1.tar`

### file list

```diff
@@ -1,63 +1,63 @@
--rw-r--r--   0        0        0     3807 2023-05-19 21:56:26.769345 contenda-api-client-0.1.0/README.md
--rw-r--r--   0        0        0      156 2023-05-19 21:56:31.681902 contenda-api-client-0.1.0/contenda_api_client/__init__.py
--rw-r--r--   0        0        0       47 2023-05-19 21:56:26.851278 contenda-api-client-0.1.0/contenda_api_client/api/__init__.py
--rw-r--r--   0        0        0        0 2023-05-19 21:56:26.892890 contenda-api-client-0.1.0/contenda_api_client/api/content_and_results/__init__.py
--rw-r--r--   0        0        0     6192 2023-05-19 21:56:31.724435 contenda-api-client-0.1.0/contenda_api_client/api/content_and_results/get_all_blog_images_api_v2_content_blog_blog_id_images_get.py
--rw-r--r--   0        0        0     7362 2023-05-19 21:56:31.740508 contenda-api-client-0.1.0/contenda_api_client/api/content_and_results/get_blog_result_document_api_v2_content_blog_blog_id_get.py
--rw-r--r--   0        0        0     5578 2023-05-19 21:56:31.732686 contenda-api-client-0.1.0/contenda_api_client/api/content_and_results/get_blog_result_markdown_api_v2_content_blog_blog_id_markdown_get.py
--rw-r--r--   0        0        0     5089 2023-05-19 21:56:31.726028 contenda-api-client-0.1.0/contenda_api_client/api/content_and_results/get_regeneration_feedback_options_api_v2_content_blog_segment_revision_feedback_options_get.py
--rw-r--r--   0        0        0     6009 2023-05-19 21:56:31.770114 contenda-api-client-0.1.0/contenda_api_client/api/content_and_results/get_segment_transcript_api_v2_content_blog_segment_segment_id_transcript_get.py
--rw-r--r--   0        0        0     5026 2023-05-19 21:56:31.773372 contenda-api-client-0.1.0/contenda_api_client/api/content_and_results/list_blogs_api_v2_content_blog_list_get.py
--rw-r--r--   0        0        0    14566 2023-05-19 21:56:31.848554 contenda-api-client-0.1.0/contenda_api_client/api/content_and_results/save_blog_result_document_api_v2_content_blog_blog_id_put.py
--rw-r--r--   0        0        0     9714 2023-05-19 21:56:31.774909 contenda-api-client-0.1.0/contenda_api_client/api/content_and_results/save_segment_revision_feedback_api_v2_content_blog_segment_revision_feedback_revision_id_put.py
--rw-r--r--   0        0        0        0 2023-05-19 21:56:26.902494 contenda-api-client-0.1.0/contenda_api_client/api/experimental/__init__.py
--rw-r--r--   0        0        0     6936 2023-05-19 21:56:31.779472 contenda-api-client-0.1.0/contenda_api_client/api/experimental/get_rss_feed_parsed_api_v2_blog_rss_feed_parsed_get.py
--rw-r--r--   0        0        0        0 2023-05-19 21:56:26.884036 contenda-api-client-0.1.0/contenda_api_client/api/identity/__init__.py
--rw-r--r--   0        0        0     6496 2023-05-19 21:56:31.794577 contenda-api-client-0.1.0/contenda_api_client/api/identity/get_token_endpoint_api_v2_identity_token_post.py
--rw-r--r--   0        0        0        0 2023-05-19 21:56:26.885947 contenda-api-client-0.1.0/contenda_api_client/api/jobs/__init__.py
--rw-r--r--   0        0        0     5835 2023-05-19 21:56:31.790541 contenda-api-client-0.1.0/contenda_api_client/api/jobs/get_job_api_v2_jobs_status_job_id_get.py
--rw-r--r--   0        0        0     4927 2023-05-19 21:56:31.820613 contenda-api-client-0.1.0/contenda_api_client/api/jobs/get_usage_api_v2_jobs_usage_limits_get.py
--rw-r--r--   0        0        0    24681 2023-05-19 21:56:31.818989 contenda-api-client-0.1.0/contenda_api_client/api/jobs/post_video_to_blog_job_api_v2_jobs_video_to_blog_post.py
--rw-r--r--   0        0        0        0 2023-05-19 21:56:26.885091 contenda-api-client-0.1.0/contenda_api_client/api/media/__init__.py
--rw-r--r--   0        0        0     4807 2023-05-19 21:56:31.857515 contenda-api-client-0.1.0/contenda_api_client/api/media/get_media_list_api_v2_media_list_get.py
--rw-r--r--   0        0        0        0 2023-05-19 21:56:26.862124 contenda-api-client-0.1.0/contenda_api_client/api/utility/__init__.py
--rw-r--r--   0        0        0     4421 2023-05-19 21:56:31.805440 contenda-api-client-0.1.0/contenda_api_client/api/utility/health_health_get.py
--rw-r--r--   0        0        0     2817 2023-05-19 21:56:31.799277 contenda-api-client-0.1.0/contenda_api_client/client.py
--rw-r--r--   0        0        0      470 2023-05-19 21:56:31.803998 contenda-api-client-0.1.0/contenda_api_client/errors.py
--rw-r--r--   0        0        0     4806 2023-05-19 21:56:28.506772 contenda-api-client-0.1.0/contenda_api_client/models/__init__.py
--rw-r--r--   0        0        0     2643 2023-05-19 21:56:31.849242 contenda-api-client-0.1.0/contenda_api_client/models/blog_entry.py
--rw-r--r--   0        0        0     2134 2023-05-19 21:56:31.830808 contenda-api-client-0.1.0/contenda_api_client/models/blog_image_response_model.py
--rw-r--r--   0        0        0      316 2023-05-19 21:56:28.521910 contenda-api-client-0.1.0/contenda_api_client/models/blog_segment_type.py
--rw-r--r--   0        0        0     2773 2023-05-19 21:56:31.829196 contenda-api-client-0.1.0/contenda_api_client/models/contenda_body_segment_save_request.py
--rw-r--r--   0        0        0     2496 2023-05-19 21:56:31.863534 contenda-api-client-0.1.0/contenda_api_client/models/contenda_code_segment_save_request.py
--rw-r--r--   0        0        0     2515 2023-05-19 21:56:31.868629 contenda-api-client-0.1.0/contenda_api_client/models/contenda_heading_segment_save_request.py
--rw-r--r--   0        0        0     2792 2023-05-19 21:56:31.856193 contenda-api-client-0.1.0/contenda_api_client/models/contenda_image_segment_save_request.py
--rw-r--r--   0        0        0     3902 2023-05-19 21:56:31.863604 contenda-api-client-0.1.0/contenda_api_client/models/document_generation_configuration.py
--rw-r--r--   0        0        0     1857 2023-05-19 21:56:31.858290 contenda-api-client-0.1.0/contenda_api_client/models/generate_access_token.py
--rw-r--r--   0        0        0     1709 2023-05-19 21:56:31.865173 contenda-api-client-0.1.0/contenda_api_client/models/get_blog_result_document_api_v2_content_blog_blog_id_get_response_get_blog_result_document_api_v2_content_blog_blog_id_get.py
--rw-r--r--   0        0        0     1473 2023-05-19 21:56:31.874303 contenda-api-client-0.1.0/contenda_api_client/models/get_job_api_v2_jobs_status_job_id_get_response_get_job_api_v2_jobs_status_job_id_get.py
--rw-r--r--   0        0        0     1653 2023-05-19 21:56:31.877256 contenda-api-client-0.1.0/contenda_api_client/models/get_rss_feed_parsed_api_v2_blog_rss_feed_parsed_get_response_get_rss_feed_parsed_api_v2_blog_rss_feed_parsed_get.py
--rw-r--r--   0        0        0     1581 2023-05-19 21:56:31.883252 contenda-api-client-0.1.0/contenda_api_client/models/get_token_endpoint_api_v2_identity_token_post_response_get_token_endpoint_api_v2_identity_token_post.py
--rw-r--r--   0        0        0     1297 2023-05-19 21:56:31.876594 contenda-api-client-0.1.0/contenda_api_client/models/health_health_get_response_health_health_get.py
--rw-r--r--   0        0        0     2131 2023-05-19 21:56:31.914855 contenda-api-client-0.1.0/contenda_api_client/models/http_validation_error.py
--rw-r--r--   0        0        0     4490 2023-05-19 21:56:31.914360 contenda-api-client-0.1.0/contenda_api_client/models/job_create_video_to_blog.py
--rw-r--r--   0        0        0     3706 2023-05-19 21:56:31.926521 contenda-api-client-0.1.0/contenda_api_client/models/media_item.py
--rw-r--r--   0        0        0     1669 2023-05-19 21:56:31.886071 contenda-api-client-0.1.0/contenda_api_client/models/post_video_to_blog_job_api_v2_jobs_video_to_blog_post_response_post_video_to_blog_job_api_v2_jobs_video_to_blog_post.py
--rw-r--r--   0        0        0      219 2023-05-19 21:56:28.504655 contenda-api-client-0.1.0/contenda_api_client/models/regeneration_fn_name.py
--rw-r--r--   0        0        0      287 2023-05-19 21:56:28.522631 contenda-api-client-0.1.0/contenda_api_client/models/regeneration_label.py
--rw-r--r--   0        0        0     1719 2023-05-19 21:56:31.942794 contenda-api-client-0.1.0/contenda_api_client/models/save_blog_result_document_api_v2_content_blog_blog_id_put_response_save_blog_result_document_api_v2_content_blog_blog_id_put.py
--rw-r--r--   0        0        0     2062 2023-05-19 21:56:31.906736 contenda-api-client-0.1.0/contenda_api_client/models/save_segment_revision_feedback_api_v2_content_blog_segment_revision_feedback_revision_id_put_response_save_segment_revision_feedback_api_v2_content_blog_segment_revision_feedback_revision_id_put.py
--rw-r--r--   0        0        0     5260 2023-05-19 21:56:31.931507 contenda-api-client-0.1.0/contenda_api_client/models/segment_configuration.py
--rw-r--r--   0        0        0     3249 2023-05-19 21:56:31.939448 contenda-api-client-0.1.0/contenda_api_client/models/segment_revision_feedback_request_model.py
--rw-r--r--   0        0        0     1877 2023-05-19 21:56:31.910544 contenda-api-client-0.1.0/contenda_api_client/models/transcript_line_response_model.py
--rw-r--r--   0        0        0     2511 2023-05-19 21:56:31.931221 contenda-api-client-0.1.0/contenda_api_client/models/usage_limits.py
--rw-r--r--   0        0        0     2493 2023-05-19 21:56:31.934114 contenda-api-client-0.1.0/contenda_api_client/models/user_body_segment_save_request.py
--rw-r--r--   0        0        0     2493 2023-05-19 21:56:31.940538 contenda-api-client-0.1.0/contenda_api_client/models/user_code_segment_save_request.py
--rw-r--r--   0        0        0     2520 2023-05-19 21:56:31.945357 contenda-api-client-0.1.0/contenda_api_client/models/user_heading_segment_save_request.py
--rw-r--r--   0        0        0     2091 2023-05-19 21:56:31.956899 contenda-api-client-0.1.0/contenda_api_client/models/validation_error.py
--rw-r--r--   0        0        0      180 2023-05-19 21:56:28.528164 contenda-api-client-0.1.0/contenda_api_client/models/video_to_blog_type.py
--rw-r--r--   0        0        0       25 2023-05-19 21:56:26.765799 contenda-api-client-0.1.0/contenda_api_client/py.typed
--rw-r--r--   0        0        0      993 2023-05-19 21:56:31.942156 contenda-api-client-0.1.0/contenda_api_client/types.py
--rw-r--r--   0        0        0      721 2023-05-24 15:39:40.972635 contenda-api-client-0.1.0/pyproject.toml
--rw-r--r--   0        0        0     4882 2023-05-24 15:40:27.896843 contenda-api-client-0.1.0/setup.py
--rw-r--r--   0        0        0     4363 2023-05-24 15:40:27.897092 contenda-api-client-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0     2007 2023-05-24 16:09:16.265809 contenda-api-client-0.1.1/README.md
+-rw-r--r--   0        0        0      156 2023-05-19 21:56:31.681902 contenda-api-client-0.1.1/contenda_api_client/__init__.py
+-rw-r--r--   0        0        0       47 2023-05-19 21:56:26.851278 contenda-api-client-0.1.1/contenda_api_client/api/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-19 21:56:26.892890 contenda-api-client-0.1.1/contenda_api_client/api/content_and_results/__init__.py
+-rw-r--r--   0        0        0     6192 2023-05-19 21:56:31.724435 contenda-api-client-0.1.1/contenda_api_client/api/content_and_results/get_all_blog_images_api_v2_content_blog_blog_id_images_get.py
+-rw-r--r--   0        0        0     7362 2023-05-19 21:56:31.740508 contenda-api-client-0.1.1/contenda_api_client/api/content_and_results/get_blog_result_document_api_v2_content_blog_blog_id_get.py
+-rw-r--r--   0        0        0     5578 2023-05-19 21:56:31.732686 contenda-api-client-0.1.1/contenda_api_client/api/content_and_results/get_blog_result_markdown_api_v2_content_blog_blog_id_markdown_get.py
+-rw-r--r--   0        0        0     5089 2023-05-19 21:56:31.726028 contenda-api-client-0.1.1/contenda_api_client/api/content_and_results/get_regeneration_feedback_options_api_v2_content_blog_segment_revision_feedback_options_get.py
+-rw-r--r--   0        0        0     6009 2023-05-19 21:56:31.770114 contenda-api-client-0.1.1/contenda_api_client/api/content_and_results/get_segment_transcript_api_v2_content_blog_segment_segment_id_transcript_get.py
+-rw-r--r--   0        0        0     5026 2023-05-19 21:56:31.773372 contenda-api-client-0.1.1/contenda_api_client/api/content_and_results/list_blogs_api_v2_content_blog_list_get.py
+-rw-r--r--   0        0        0    14566 2023-05-19 21:56:31.848554 contenda-api-client-0.1.1/contenda_api_client/api/content_and_results/save_blog_result_document_api_v2_content_blog_blog_id_put.py
+-rw-r--r--   0        0        0     9714 2023-05-19 21:56:31.774909 contenda-api-client-0.1.1/contenda_api_client/api/content_and_results/save_segment_revision_feedback_api_v2_content_blog_segment_revision_feedback_revision_id_put.py
+-rw-r--r--   0        0        0        0 2023-05-19 21:56:26.902494 contenda-api-client-0.1.1/contenda_api_client/api/experimental/__init__.py
+-rw-r--r--   0        0        0     6936 2023-05-19 21:56:31.779472 contenda-api-client-0.1.1/contenda_api_client/api/experimental/get_rss_feed_parsed_api_v2_blog_rss_feed_parsed_get.py
+-rw-r--r--   0        0        0        0 2023-05-19 21:56:26.884036 contenda-api-client-0.1.1/contenda_api_client/api/identity/__init__.py
+-rw-r--r--   0        0        0     6496 2023-05-19 21:56:31.794577 contenda-api-client-0.1.1/contenda_api_client/api/identity/get_token_endpoint_api_v2_identity_token_post.py
+-rw-r--r--   0        0        0        0 2023-05-19 21:56:26.885947 contenda-api-client-0.1.1/contenda_api_client/api/jobs/__init__.py
+-rw-r--r--   0        0        0     5835 2023-05-19 21:56:31.790541 contenda-api-client-0.1.1/contenda_api_client/api/jobs/get_job_api_v2_jobs_status_job_id_get.py
+-rw-r--r--   0        0        0     4927 2023-05-19 21:56:31.820613 contenda-api-client-0.1.1/contenda_api_client/api/jobs/get_usage_api_v2_jobs_usage_limits_get.py
+-rw-r--r--   0        0        0    24681 2023-05-19 21:56:31.818989 contenda-api-client-0.1.1/contenda_api_client/api/jobs/post_video_to_blog_job_api_v2_jobs_video_to_blog_post.py
+-rw-r--r--   0        0        0        0 2023-05-19 21:56:26.885091 contenda-api-client-0.1.1/contenda_api_client/api/media/__init__.py
+-rw-r--r--   0        0        0     4807 2023-05-19 21:56:31.857515 contenda-api-client-0.1.1/contenda_api_client/api/media/get_media_list_api_v2_media_list_get.py
+-rw-r--r--   0        0        0        0 2023-05-19 21:56:26.862124 contenda-api-client-0.1.1/contenda_api_client/api/utility/__init__.py
+-rw-r--r--   0        0        0     4421 2023-05-19 21:56:31.805440 contenda-api-client-0.1.1/contenda_api_client/api/utility/health_health_get.py
+-rw-r--r--   0        0        0     2817 2023-05-19 21:56:31.799277 contenda-api-client-0.1.1/contenda_api_client/client.py
+-rw-r--r--   0        0        0      470 2023-05-19 21:56:31.803998 contenda-api-client-0.1.1/contenda_api_client/errors.py
+-rw-r--r--   0        0        0     4806 2023-05-19 21:56:28.506772 contenda-api-client-0.1.1/contenda_api_client/models/__init__.py
+-rw-r--r--   0        0        0     2643 2023-05-19 21:56:31.849242 contenda-api-client-0.1.1/contenda_api_client/models/blog_entry.py
+-rw-r--r--   0        0        0     2134 2023-05-19 21:56:31.830808 contenda-api-client-0.1.1/contenda_api_client/models/blog_image_response_model.py
+-rw-r--r--   0        0        0      316 2023-05-19 21:56:28.521910 contenda-api-client-0.1.1/contenda_api_client/models/blog_segment_type.py
+-rw-r--r--   0        0        0     2773 2023-05-19 21:56:31.829196 contenda-api-client-0.1.1/contenda_api_client/models/contenda_body_segment_save_request.py
+-rw-r--r--   0        0        0     2496 2023-05-19 21:56:31.863534 contenda-api-client-0.1.1/contenda_api_client/models/contenda_code_segment_save_request.py
+-rw-r--r--   0        0        0     2515 2023-05-19 21:56:31.868629 contenda-api-client-0.1.1/contenda_api_client/models/contenda_heading_segment_save_request.py
+-rw-r--r--   0        0        0     2792 2023-05-19 21:56:31.856193 contenda-api-client-0.1.1/contenda_api_client/models/contenda_image_segment_save_request.py
+-rw-r--r--   0        0        0     3902 2023-05-19 21:56:31.863604 contenda-api-client-0.1.1/contenda_api_client/models/document_generation_configuration.py
+-rw-r--r--   0        0        0     1857 2023-05-19 21:56:31.858290 contenda-api-client-0.1.1/contenda_api_client/models/generate_access_token.py
+-rw-r--r--   0        0        0     1709 2023-05-19 21:56:31.865173 contenda-api-client-0.1.1/contenda_api_client/models/get_blog_result_document_api_v2_content_blog_blog_id_get_response_get_blog_result_document_api_v2_content_blog_blog_id_get.py
+-rw-r--r--   0        0        0     1473 2023-05-19 21:56:31.874303 contenda-api-client-0.1.1/contenda_api_client/models/get_job_api_v2_jobs_status_job_id_get_response_get_job_api_v2_jobs_status_job_id_get.py
+-rw-r--r--   0        0        0     1653 2023-05-19 21:56:31.877256 contenda-api-client-0.1.1/contenda_api_client/models/get_rss_feed_parsed_api_v2_blog_rss_feed_parsed_get_response_get_rss_feed_parsed_api_v2_blog_rss_feed_parsed_get.py
+-rw-r--r--   0        0        0     1581 2023-05-19 21:56:31.883252 contenda-api-client-0.1.1/contenda_api_client/models/get_token_endpoint_api_v2_identity_token_post_response_get_token_endpoint_api_v2_identity_token_post.py
+-rw-r--r--   0        0        0     1297 2023-05-19 21:56:31.876594 contenda-api-client-0.1.1/contenda_api_client/models/health_health_get_response_health_health_get.py
+-rw-r--r--   0        0        0     2131 2023-05-19 21:56:31.914855 contenda-api-client-0.1.1/contenda_api_client/models/http_validation_error.py
+-rw-r--r--   0        0        0     4490 2023-05-19 21:56:31.914360 contenda-api-client-0.1.1/contenda_api_client/models/job_create_video_to_blog.py
+-rw-r--r--   0        0        0     3706 2023-05-19 21:56:31.926521 contenda-api-client-0.1.1/contenda_api_client/models/media_item.py
+-rw-r--r--   0        0        0     1669 2023-05-19 21:56:31.886071 contenda-api-client-0.1.1/contenda_api_client/models/post_video_to_blog_job_api_v2_jobs_video_to_blog_post_response_post_video_to_blog_job_api_v2_jobs_video_to_blog_post.py
+-rw-r--r--   0        0        0      219 2023-05-19 21:56:28.504655 contenda-api-client-0.1.1/contenda_api_client/models/regeneration_fn_name.py
+-rw-r--r--   0        0        0      287 2023-05-19 21:56:28.522631 contenda-api-client-0.1.1/contenda_api_client/models/regeneration_label.py
+-rw-r--r--   0        0        0     1719 2023-05-19 21:56:31.942794 contenda-api-client-0.1.1/contenda_api_client/models/save_blog_result_document_api_v2_content_blog_blog_id_put_response_save_blog_result_document_api_v2_content_blog_blog_id_put.py
+-rw-r--r--   0        0        0     2062 2023-05-19 21:56:31.906736 contenda-api-client-0.1.1/contenda_api_client/models/save_segment_revision_feedback_api_v2_content_blog_segment_revision_feedback_revision_id_put_response_save_segment_revision_feedback_api_v2_content_blog_segment_revision_feedback_revision_id_put.py
+-rw-r--r--   0        0        0     5260 2023-05-19 21:56:31.931507 contenda-api-client-0.1.1/contenda_api_client/models/segment_configuration.py
+-rw-r--r--   0        0        0     3249 2023-05-19 21:56:31.939448 contenda-api-client-0.1.1/contenda_api_client/models/segment_revision_feedback_request_model.py
+-rw-r--r--   0        0        0     1877 2023-05-19 21:56:31.910544 contenda-api-client-0.1.1/contenda_api_client/models/transcript_line_response_model.py
+-rw-r--r--   0        0        0     2511 2023-05-19 21:56:31.931221 contenda-api-client-0.1.1/contenda_api_client/models/usage_limits.py
+-rw-r--r--   0        0        0     2493 2023-05-19 21:56:31.934114 contenda-api-client-0.1.1/contenda_api_client/models/user_body_segment_save_request.py
+-rw-r--r--   0        0        0     2493 2023-05-19 21:56:31.940538 contenda-api-client-0.1.1/contenda_api_client/models/user_code_segment_save_request.py
+-rw-r--r--   0        0        0     2520 2023-05-19 21:56:31.945357 contenda-api-client-0.1.1/contenda_api_client/models/user_heading_segment_save_request.py
+-rw-r--r--   0        0        0     2091 2023-05-19 21:56:31.956899 contenda-api-client-0.1.1/contenda_api_client/models/validation_error.py
+-rw-r--r--   0        0        0      180 2023-05-19 21:56:28.528164 contenda-api-client-0.1.1/contenda_api_client/models/video_to_blog_type.py
+-rw-r--r--   0        0        0       25 2023-05-19 21:56:26.765799 contenda-api-client-0.1.1/contenda_api_client/py.typed
+-rw-r--r--   0        0        0      993 2023-05-19 21:56:31.942156 contenda-api-client-0.1.1/contenda_api_client/types.py
+-rw-r--r--   0        0        0      721 2023-05-24 16:09:22.035731 contenda-api-client-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0     3041 2023-05-24 16:11:58.463177 contenda-api-client-0.1.1/setup.py
+-rw-r--r--   0        0        0     2563 2023-05-24 16:11:58.463375 contenda-api-client-0.1.1/PKG-INFO
```

### Comparing `contenda-api-client-0.1.0/contenda_api_client/api/content_and_results/get_all_blog_images_api_v2_content_blog_blog_id_images_get.py` & `contenda-api-client-0.1.1/contenda_api_client/api/content_and_results/get_all_blog_images_api_v2_content_blog_blog_id_images_get.py`

 * *Files identical despite different names*

### Comparing `contenda-api-client-0.1.0/contenda_api_client/api/content_and_results/get_blog_result_document_api_v2_content_blog_blog_id_get.py` & `contenda-api-client-0.1.1/contenda_api_client/api/content_and_results/get_blog_result_document_api_v2_content_blog_blog_id_get.py`

 * *Files identical despite different names*

### Comparing `contenda-api-client-0.1.0/contenda_api_client/api/content_and_results/get_blog_result_markdown_api_v2_content_blog_blog_id_markdown_get.py` & `contenda-api-client-0.1.1/contenda_api_client/api/content_and_results/get_blog_result_markdown_api_v2_content_blog_blog_id_markdown_get.py`

 * *Files identical despite different names*

### Comparing `contenda-api-client-0.1.0/contenda_api_client/api/content_and_results/get_regeneration_feedback_options_api_v2_content_blog_segment_revision_feedback_options_get.py` & `contenda-api-client-0.1.1/contenda_api_client/api/content_and_results/get_regeneration_feedback_options_api_v2_content_blog_segment_revision_feedback_options_get.py`

 * *Files identical despite different names*

### Comparing `contenda-api-client-0.1.0/contenda_api_client/api/content_and_results/get_segment_transcript_api_v2_content_blog_segment_segment_id_transcript_get.py` & `contenda-api-client-0.1.1/contenda_api_client/api/content_and_results/get_segment_transcript_api_v2_content_blog_segment_segment_id_transcript_get.py`

 * *Files identical despite different names*

### Comparing `contenda-api-client-0.1.0/contenda_api_client/api/content_and_results/list_blogs_api_v2_content_blog_list_get.py` & `contenda-api-client-0.1.1/contenda_api_client/api/content_and_results/list_blogs_api_v2_content_blog_list_get.py`

 * *Files identical despite different names*

### Comparing `contenda-api-client-0.1.0/contenda_api_client/api/content_and_results/save_blog_result_document_api_v2_content_blog_blog_id_put.py` & `contenda-api-client-0.1.1/contenda_api_client/api/content_and_results/save_blog_result_document_api_v2_content_blog_blog_id_put.py`

 * *Files identical despite different names*

### Comparing `contenda-api-client-0.1.0/contenda_api_client/api/content_and_results/save_segment_revision_feedback_api_v2_content_blog_segment_revision_feedback_revision_id_put.py` & `contenda-api-client-0.1.1/contenda_api_client/api/content_and_results/save_segment_revision_feedback_api_v2_content_blog_segment_revision_feedback_revision_id_put.py`

 * *Files identical despite different names*

### Comparing `contenda-api-client-0.1.0/contenda_api_client/api/experimental/get_rss_feed_parsed_api_v2_blog_rss_feed_parsed_get.py` & `contenda-api-client-0.1.1/contenda_api_client/api/experimental/get_rss_feed_parsed_api_v2_blog_rss_feed_parsed_get.py`

 * *Files identical despite different names*

### Comparing `contenda-api-client-0.1.0/contenda_api_client/api/identity/get_token_endpoint_api_v2_identity_token_post.py` & `contenda-api-client-0.1.1/contenda_api_client/api/identity/get_token_endpoint_api_v2_identity_token_post.py`

 * *Files identical despite different names*

### Comparing `contenda-api-client-0.1.0/contenda_api_client/api/jobs/get_job_api_v2_jobs_status_job_id_get.py` & `contenda-api-client-0.1.1/contenda_api_client/api/jobs/get_job_api_v2_jobs_status_job_id_get.py`

 * *Files identical despite different names*

### Comparing `contenda-api-client-0.1.0/contenda_api_client/api/jobs/get_usage_api_v2_jobs_usage_limits_get.py` & `contenda-api-client-0.1.1/contenda_api_client/api/jobs/get_usage_api_v2_jobs_usage_limits_get.py`

 * *Files identical despite different names*

### Comparing `contenda-api-client-0.1.0/contenda_api_client/api/jobs/post_video_to_blog_job_api_v2_jobs_video_to_blog_post.py` & `contenda-api-client-0.1.1/contenda_api_client/api/jobs/post_video_to_blog_job_api_v2_jobs_video_to_blog_post.py`

 * *Files identical despite different names*

### Comparing `contenda-api-client-0.1.0/contenda_api_client/api/media/get_media_list_api_v2_media_list_get.py` & `contenda-api-client-0.1.1/contenda_api_client/api/media/get_media_list_api_v2_media_list_get.py`

 * *Files identical despite different names*

### Comparing `contenda-api-client-0.1.0/contenda_api_client/api/utility/health_health_get.py` & `contenda-api-client-0.1.1/contenda_api_client/api/utility/health_health_get.py`

 * *Files identical despite different names*

### Comparing `contenda-api-client-0.1.0/contenda_api_client/client.py` & `contenda-api-client-0.1.1/contenda_api_client/client.py`

 * *Files identical despite different names*

### Comparing `contenda-api-client-0.1.0/contenda_api_client/models/__init__.py` & `contenda-api-client-0.1.1/contenda_api_client/models/__init__.py`

 * *Files identical despite different names*

### Comparing `contenda-api-client-0.1.0/contenda_api_client/models/blog_entry.py` & `contenda-api-client-0.1.1/contenda_api_client/models/blog_entry.py`

 * *Files identical despite different names*

### Comparing `contenda-api-client-0.1.0/contenda_api_client/models/blog_image_response_model.py` & `contenda-api-client-0.1.1/contenda_api_client/models/blog_image_response_model.py`

 * *Files identical despite different names*

### Comparing `contenda-api-client-0.1.0/contenda_api_client/models/contenda_body_segment_save_request.py` & `contenda-api-client-0.1.1/contenda_api_client/models/contenda_body_segment_save_request.py`

 * *Files identical despite different names*

### Comparing `contenda-api-client-0.1.0/contenda_api_client/models/contenda_code_segment_save_request.py` & `contenda-api-client-0.1.1/contenda_api_client/models/contenda_code_segment_save_request.py`

 * *Files identical despite different names*

### Comparing `contenda-api-client-0.1.0/contenda_api_client/models/contenda_heading_segment_save_request.py` & `contenda-api-client-0.1.1/contenda_api_client/models/contenda_heading_segment_save_request.py`

 * *Files identical despite different names*

### Comparing `contenda-api-client-0.1.0/contenda_api_client/models/contenda_image_segment_save_request.py` & `contenda-api-client-0.1.1/contenda_api_client/models/contenda_image_segment_save_request.py`

 * *Files identical despite different names*

### Comparing `contenda-api-client-0.1.0/contenda_api_client/models/document_generation_configuration.py` & `contenda-api-client-0.1.1/contenda_api_client/models/document_generation_configuration.py`

 * *Files identical despite different names*

### Comparing `contenda-api-client-0.1.0/contenda_api_client/models/generate_access_token.py` & `contenda-api-client-0.1.1/contenda_api_client/models/generate_access_token.py`

 * *Files identical despite different names*

### Comparing `contenda-api-client-0.1.0/contenda_api_client/models/get_blog_result_document_api_v2_content_blog_blog_id_get_response_get_blog_result_document_api_v2_content_blog_blog_id_get.py` & `contenda-api-client-0.1.1/contenda_api_client/models/get_blog_result_document_api_v2_content_blog_blog_id_get_response_get_blog_result_document_api_v2_content_blog_blog_id_get.py`

 * *Files identical despite different names*

### Comparing `contenda-api-client-0.1.0/contenda_api_client/models/get_job_api_v2_jobs_status_job_id_get_response_get_job_api_v2_jobs_status_job_id_get.py` & `contenda-api-client-0.1.1/contenda_api_client/models/get_job_api_v2_jobs_status_job_id_get_response_get_job_api_v2_jobs_status_job_id_get.py`

 * *Files identical despite different names*

### Comparing `contenda-api-client-0.1.0/contenda_api_client/models/get_rss_feed_parsed_api_v2_blog_rss_feed_parsed_get_response_get_rss_feed_parsed_api_v2_blog_rss_feed_parsed_get.py` & `contenda-api-client-0.1.1/contenda_api_client/models/get_rss_feed_parsed_api_v2_blog_rss_feed_parsed_get_response_get_rss_feed_parsed_api_v2_blog_rss_feed_parsed_get.py`

 * *Files identical despite different names*

### Comparing `contenda-api-client-0.1.0/contenda_api_client/models/get_token_endpoint_api_v2_identity_token_post_response_get_token_endpoint_api_v2_identity_token_post.py` & `contenda-api-client-0.1.1/contenda_api_client/models/get_token_endpoint_api_v2_identity_token_post_response_get_token_endpoint_api_v2_identity_token_post.py`

 * *Files identical despite different names*

### Comparing `contenda-api-client-0.1.0/contenda_api_client/models/health_health_get_response_health_health_get.py` & `contenda-api-client-0.1.1/contenda_api_client/models/health_health_get_response_health_health_get.py`

 * *Files identical despite different names*

### Comparing `contenda-api-client-0.1.0/contenda_api_client/models/http_validation_error.py` & `contenda-api-client-0.1.1/contenda_api_client/models/http_validation_error.py`

 * *Files identical despite different names*

### Comparing `contenda-api-client-0.1.0/contenda_api_client/models/job_create_video_to_blog.py` & `contenda-api-client-0.1.1/contenda_api_client/models/job_create_video_to_blog.py`

 * *Files identical despite different names*

### Comparing `contenda-api-client-0.1.0/contenda_api_client/models/media_item.py` & `contenda-api-client-0.1.1/contenda_api_client/models/media_item.py`

 * *Files identical despite different names*

### Comparing `contenda-api-client-0.1.0/contenda_api_client/models/post_video_to_blog_job_api_v2_jobs_video_to_blog_post_response_post_video_to_blog_job_api_v2_jobs_video_to_blog_post.py` & `contenda-api-client-0.1.1/contenda_api_client/models/post_video_to_blog_job_api_v2_jobs_video_to_blog_post_response_post_video_to_blog_job_api_v2_jobs_video_to_blog_post.py`

 * *Files identical despite different names*

### Comparing `contenda-api-client-0.1.0/contenda_api_client/models/save_blog_result_document_api_v2_content_blog_blog_id_put_response_save_blog_result_document_api_v2_content_blog_blog_id_put.py` & `contenda-api-client-0.1.1/contenda_api_client/models/save_blog_result_document_api_v2_content_blog_blog_id_put_response_save_blog_result_document_api_v2_content_blog_blog_id_put.py`

 * *Files identical despite different names*

### Comparing `contenda-api-client-0.1.0/contenda_api_client/models/save_segment_revision_feedback_api_v2_content_blog_segment_revision_feedback_revision_id_put_response_save_segment_revision_feedback_api_v2_content_blog_segment_revision_feedback_revision_id_put.py` & `contenda-api-client-0.1.1/contenda_api_client/models/save_segment_revision_feedback_api_v2_content_blog_segment_revision_feedback_revision_id_put_response_save_segment_revision_feedback_api_v2_content_blog_segment_revision_feedback_revision_id_put.py`

 * *Files identical despite different names*

### Comparing `contenda-api-client-0.1.0/contenda_api_client/models/segment_configuration.py` & `contenda-api-client-0.1.1/contenda_api_client/models/segment_configuration.py`

 * *Files identical despite different names*

### Comparing `contenda-api-client-0.1.0/contenda_api_client/models/segment_revision_feedback_request_model.py` & `contenda-api-client-0.1.1/contenda_api_client/models/segment_revision_feedback_request_model.py`

 * *Files identical despite different names*

### Comparing `contenda-api-client-0.1.0/contenda_api_client/models/transcript_line_response_model.py` & `contenda-api-client-0.1.1/contenda_api_client/models/transcript_line_response_model.py`

 * *Files identical despite different names*

### Comparing `contenda-api-client-0.1.0/contenda_api_client/models/usage_limits.py` & `contenda-api-client-0.1.1/contenda_api_client/models/usage_limits.py`

 * *Files identical despite different names*

### Comparing `contenda-api-client-0.1.0/contenda_api_client/models/user_body_segment_save_request.py` & `contenda-api-client-0.1.1/contenda_api_client/models/user_body_segment_save_request.py`

 * *Files identical despite different names*

### Comparing `contenda-api-client-0.1.0/contenda_api_client/models/user_code_segment_save_request.py` & `contenda-api-client-0.1.1/contenda_api_client/models/user_code_segment_save_request.py`

 * *Files identical despite different names*

### Comparing `contenda-api-client-0.1.0/contenda_api_client/models/user_heading_segment_save_request.py` & `contenda-api-client-0.1.1/contenda_api_client/models/user_heading_segment_save_request.py`

 * *Files identical despite different names*

### Comparing `contenda-api-client-0.1.0/contenda_api_client/models/validation_error.py` & `contenda-api-client-0.1.1/contenda_api_client/models/validation_error.py`

 * *Files identical despite different names*

### Comparing `contenda-api-client-0.1.0/contenda_api_client/types.py` & `contenda-api-client-0.1.1/contenda_api_client/types.py`

 * *Files identical despite different names*

### Comparing `contenda-api-client-0.1.0/pyproject.toml` & `contenda-api-client-0.1.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "contenda-api-client"
-version = "0.1.0"
+version = "0.1.1"
 description = "A client library for accessing Contenda API"
 
 authors = ["Lilly Chen <lilly@contenda.co>"]
 
 readme = "README.md"
 packages = [
     {include = "contenda_api_client"},
```

