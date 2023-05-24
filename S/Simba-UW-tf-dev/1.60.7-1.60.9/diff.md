# Comparing `tmp/Simba-UW-tf-dev-1.60.7.tar.gz` & `tmp/Simba-UW-tf-dev-1.60.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/Simba-UW-tf-dev-1.60.7.tar", last modified: Tue May 23 16:26:59 2023, max compression
+gzip compressed data, was "dist/Simba-UW-tf-dev-1.60.9.tar", last modified: Wed May 24 15:39:16 2023, max compression
```

## Comparing `Simba-UW-tf-dev-1.60.7.tar` & `Simba-UW-tf-dev-1.60.9.tar`

### file list

```diff
@@ -1,503 +1,504 @@
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-23 16:26:59.000000 Simba-UW-tf-dev-1.60.7/
--rw-r--r--   0 simon      (501) staff       (20)      579 2023-05-23 16:26:59.000000 Simba-UW-tf-dev-1.60.7/PKG-INFO
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-23 16:26:58.000000 Simba-UW-tf-dev-1.60.7/simba/
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-23 16:26:59.000000 Simba-UW-tf-dev-1.60.7/simba/ui/
--rw-r--r--   0 simon      (501) staff       (20)     8196 2023-05-23 15:42:08.000000 Simba-UW-tf-dev-1.60.7/simba/ui/.DS_Store
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-23 16:26:59.000000 Simba-UW-tf-dev-1.60.7/simba/ui/pop_ups/
--rw-r--r--   0 simon      (501) staff       (20)     3463 2023-05-04 17:49:06.000000 Simba-UW-tf-dev-1.60.7/simba/ui/pop_ups/movement_analysis_time_bins_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)     1431 2023-04-29 18:36:18.000000 Simba-UW-tf-dev-1.60.7/simba/ui/pop_ups/csv_2_parquet_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)     2343 2023-05-17 20:47:45.000000 Simba-UW-tf-dev-1.60.7/simba/ui/pop_ups/quick_path_plot_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)     2332 2023-04-29 18:13:54.000000 Simba-UW-tf-dev-1.60.7/simba/ui/pop_ups/batch_preprocess_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)     8342 2023-05-14 15:52:16.000000 Simba-UW-tf-dev-1.60.7/simba/ui/pop_ups/heatmap_location_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)     9302 2023-05-04 15:16:51.000000 Simba-UW-tf-dev-1.60.7/simba/ui/pop_ups/clf_probability_plot_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)     6148 2023-05-23 15:42:32.000000 Simba-UW-tf-dev-1.60.7/simba/ui/pop_ups/.DS_Store
--rw-r--r--   0 simon      (501) staff       (20)     3143 2023-05-03 16:24:11.000000 Simba-UW-tf-dev-1.60.7/simba/ui/pop_ups/movement_analysis_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)     3657 2023-04-29 19:37:54.000000 Simba-UW-tf-dev-1.60.7/simba/ui/pop_ups/set_machine_model_parameters_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)     9471 2023-05-14 16:01:44.000000 Simba-UW-tf-dev-1.60.7/simba/ui/pop_ups/clf_plot_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)    15950 2023-05-20 12:10:35.000000 Simba-UW-tf-dev-1.60.7/simba/ui/pop_ups/path_plot_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)     3024 2023-04-29 16:24:52.000000 Simba-UW-tf-dev-1.60.7/simba/ui/pop_ups/smoothing_interpolation_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)     4798 2023-04-29 18:54:24.000000 Simba-UW-tf-dev-1.60.7/simba/ui/pop_ups/visualize_pose_in_dir_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)     3551 2023-05-03 16:20:49.000000 Simba-UW-tf-dev-1.60.7/simba/ui/pop_ups/roi_analysis_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)     5873 2023-04-29 16:24:52.000000 Simba-UW-tf-dev-1.60.7/simba/ui/pop_ups/outlier_settings_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)     8296 2023-04-29 18:36:18.000000 Simba-UW-tf-dev-1.60.7/simba/ui/pop_ups/gantt_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)     5726 2023-05-01 12:04:35.000000 Simba-UW-tf-dev-1.60.7/simba/ui/pop_ups/clf_validation_plot_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)     7532 2023-05-23 15:46:01.000000 Simba-UW-tf-dev-1.60.7/simba/ui/pop_ups/severity_analysis_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)     2779 2023-04-29 18:36:18.000000 Simba-UW-tf-dev-1.60.7/simba/ui/pop_ups/fsttc_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)     4052 2023-05-13 17:09:38.000000 Simba-UW-tf-dev-1.60.7/simba/ui/pop_ups/kleinberg_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)        0 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.60.7/simba/ui/pop_ups/__init__.py
--rw-r--r--   0 simon      (501) staff       (20)     7288 2023-04-29 15:00:50.000000 Simba-UW-tf-dev-1.60.7/simba/ui/pop_ups/directing_other_animals_plot_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)     5425 2023-05-14 16:11:59.000000 Simba-UW-tf-dev-1.60.7/simba/ui/pop_ups/pose_reorganizer_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)     2411 2023-05-03 16:35:10.000000 Simba-UW-tf-dev-1.60.7/simba/ui/pop_ups/append_roi_features_animals_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)     3251 2023-04-29 18:36:18.000000 Simba-UW-tf-dev-1.60.7/simba/ui/pop_ups/clf_by_timebins_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)     8673 2023-05-14 15:52:16.000000 Simba-UW-tf-dev-1.60.7/simba/ui/pop_ups/heatmap_clf_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)     7688 2023-04-29 15:00:50.000000 Simba-UW-tf-dev-1.60.7/simba/ui/pop_ups/data_plot_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)     7860 2023-05-14 16:01:44.000000 Simba-UW-tf-dev-1.60.7/simba/ui/pop_ups/roi_features_plot_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)     8363 2023-04-29 19:49:16.000000 Simba-UW-tf-dev-1.60.7/simba/ui/pop_ups/pup_retrieval_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)      579 2023-04-29 18:12:37.000000 Simba-UW-tf-dev-1.60.7/simba/ui/pop_ups/about_simba_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)     2544 2023-04-29 18:36:18.000000 Simba-UW-tf-dev-1.60.7/simba/ui/pop_ups/clf_descriptive_statistics_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)     6352 2023-05-17 13:58:48.000000 Simba-UW-tf-dev-1.60.7/simba/ui/pop_ups/roi_tracking_plot_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)     1468 2023-04-29 16:24:52.000000 Simba-UW-tf-dev-1.60.7/simba/ui/pop_ups/append_roi_features_bodypart_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)     5318 2023-04-29 19:01:32.000000 Simba-UW-tf-dev-1.60.7/simba/ui/pop_ups/clf_add_remove_print_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)    42478 2023-04-29 18:56:08.000000 Simba-UW-tf-dev-1.60.7/simba/ui/pop_ups/video_processing_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)     7535 2023-05-15 13:09:04.000000 Simba-UW-tf-dev-1.60.7/simba/ui/pop_ups/validation_plot_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)     5255 2023-05-04 18:22:44.000000 Simba-UW-tf-dev-1.60.7/simba/ui/pop_ups/clf_by_roi_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)     2840 2023-04-29 18:36:18.000000 Simba-UW-tf-dev-1.60.7/simba/ui/pop_ups/make_path_plot_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)     5406 2023-04-29 18:36:18.000000 Simba-UW-tf-dev-1.60.7/simba/ui/pop_ups/create_user_defined_pose_configuration_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)     1065 2023-04-29 16:24:52.000000 Simba-UW-tf-dev-1.60.7/simba/ui/pop_ups/archive_files_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)     4087 2023-05-14 16:11:59.000000 Simba-UW-tf-dev-1.60.7/simba/ui/pop_ups/pose_bp_drop_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)    10712 2023-04-29 15:00:50.000000 Simba-UW-tf-dev-1.60.7/simba/ui/pop_ups/distance_plot_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)     2567 2023-04-29 16:24:52.000000 Simba-UW-tf-dev-1.60.7/simba/ui/pop_ups/subset_feature_extractor_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)     3114 2023-04-29 18:36:18.000000 Simba-UW-tf-dev-1.60.7/simba/ui/pop_ups/third_party_annotator_appender_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)     3193 2023-05-04 18:50:54.000000 Simba-UW-tf-dev-1.60.7/simba/ui/pop_ups/roi_analysis_time_bins_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)    12869 2023-05-23 12:47:59.000000 Simba-UW-tf-dev-1.60.7/simba/ui/video_info_ui.py
--rw-r--r--   0 simon      (501) staff       (20)     6019 2023-05-16 16:45:46.000000 Simba-UW-tf-dev-1.60.7/simba/ui/user_defined_pose_creator.py
--rw-r--r--   0 simon      (501) staff       (20)        0 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.60.7/simba/ui/__init__.py
--rw-r--r--   0 simon      (501) staff       (20)    12602 2023-05-15 17:45:06.000000 Simba-UW-tf-dev-1.60.7/simba/ui/create_project_ui.py
--rw-r--r--   0 simon      (501) staff       (20)    10957 2023-05-04 14:03:25.000000 Simba-UW-tf-dev-1.60.7/simba/ui/tkinter_functions.py
--rw-r--r--   0 simon      (501) staff       (20)    34040 2023-05-15 17:45:06.000000 Simba-UW-tf-dev-1.60.7/simba/ui/machine_model_settings_ui.py
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-23 16:26:58.000000 Simba-UW-tf-dev-1.60.7/simba/blob_storage/
--rw-r--r--   0 simon      (501) staff       (20)     6148 2023-05-20 18:16:05.000000 Simba-UW-tf-dev-1.60.7/simba/blob_storage/.DS_Store
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-23 16:26:58.000000 Simba-UW-tf-dev-1.60.7/simba/labelling/
--rw-r--r--   0 simon      (501) staff       (20)     6148 2023-05-09 13:50:26.000000 Simba-UW-tf-dev-1.60.7/simba/labelling/.DS_Store
--rw-r--r--   0 simon      (501) staff       (20)        0 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.60.7/simba/labelling/__init__.py
--rw-r--r--   0 simon      (501) staff       (20)    20743 2023-05-14 23:21:08.000000 Simba-UW-tf-dev-1.60.7/simba/labelling/labelling_interface.py
--rw-r--r--   0 simon      (501) staff       (20)     3568 2023-05-19 11:18:49.000000 Simba-UW-tf-dev-1.60.7/simba/labelling/extract_labelled_frames.py
--rw-r--r--   0 simon      (501) staff       (20)    26536 2023-05-14 19:57:32.000000 Simba-UW-tf-dev-1.60.7/simba/labelling/labelling_advanced_interface.py
--rw-r--r--   0 simon      (501) staff       (20)     6629 2023-05-13 17:45:08.000000 Simba-UW-tf-dev-1.60.7/simba/labelling/play_annotation_video.py
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-23 16:26:59.000000 Simba-UW-tf-dev-1.60.7/simba/unsupervised/
--rw-r--r--   0 simon      (501) staff       (20)    11877 2023-05-17 14:59:39.000000 Simba-UW-tf-dev-1.60.7/simba/unsupervised/dbcv_calculator.py
--rw-r--r--   0 simon      (501) staff       (20)     3375 2023-05-02 18:14:28.000000 Simba-UW-tf-dev-1.60.7/simba/unsupervised/enums.py
--rw-r--r--   0 simon      (501) staff       (20)     6148 2023-05-20 18:15:51.000000 Simba-UW-tf-dev-1.60.7/simba/unsupervised/.DS_Store
--rw-r--r--   0 simon      (501) staff       (20)     8141 2023-05-17 15:03:51.000000 Simba-UW-tf-dev-1.60.7/simba/unsupervised/dataset_creator.py
--rw-r--r--   0 simon      (501) staff       (20)     5636 2023-05-17 15:03:51.000000 Simba-UW-tf-dev-1.60.7/simba/unsupervised/grid_search_visualizers.py
--rw-r--r--   0 simon      (501) staff       (20)     7310 2023-05-17 15:03:51.000000 Simba-UW-tf-dev-1.60.7/simba/unsupervised/data_extractor.py
--rw-r--r--   0 simon      (501) staff       (20)     9848 2023-05-17 15:03:51.000000 Simba-UW-tf-dev-1.60.7/simba/unsupervised/ui.py
--rw-r--r--   0 simon      (501) staff       (20)        0 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.60.7/simba/unsupervised/__init__.py
--rw-r--r--   0 simon      (501) staff       (20)     9851 2023-05-17 15:03:51.000000 Simba-UW-tf-dev-1.60.7/simba/unsupervised/umap_embedder.py
--rw-r--r--   0 simon      (501) staff       (20)    41323 2023-05-02 18:14:28.000000 Simba-UW-tf-dev-1.60.7/simba/unsupervised/pop_up_classes.py
--rw-r--r--   0 simon      (501) staff       (20)     2931 2023-05-17 14:54:38.000000 Simba-UW-tf-dev-1.60.7/simba/unsupervised/bout_aggregator.py
--rw-r--r--   0 simon      (501) staff       (20)    20846 2023-05-17 15:03:51.000000 Simba-UW-tf-dev-1.60.7/simba/unsupervised/cluster_statistics.py
--rw-r--r--   0 simon      (501) staff       (20)     2188 2023-04-18 23:25:29.000000 Simba-UW-tf-dev-1.60.7/simba/unsupervised/data_map.yaml
--rw-r--r--   0 simon      (501) staff       (20)    10288 2023-05-17 15:07:44.000000 Simba-UW-tf-dev-1.60.7/simba/unsupervised/hdbscan_clusterer.py
--rw-r--r--   0 simon      (501) staff       (20)     3937 2023-04-28 19:59:05.000000 Simba-UW-tf-dev-1.60.7/simba/unsupervised/tsne.py
--rw-r--r--   0 simon      (501) staff       (20)     6656 2023-05-17 15:03:51.000000 Simba-UW-tf-dev-1.60.7/simba/unsupervised/cluster_visualizer.py
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-23 16:26:58.000000 Simba-UW-tf-dev-1.60.7/simba/bounding_box_tools/
--rw-r--r--   0 simon      (501) staff       (20)     6148 2023-05-20 18:16:05.000000 Simba-UW-tf-dev-1.60.7/simba/bounding_box_tools/.DS_Store
--rw-r--r--   0 simon      (501) staff       (20)        0 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.60.7/simba/bounding_box_tools/__init__.py
--rw-r--r--   0 simon      (501) staff       (20)     7031 2023-05-14 18:13:04.000000 Simba-UW-tf-dev-1.60.7/simba/bounding_box_tools/agg_boundary_stats.py
--rw-r--r--   0 simon      (501) staff       (20)    23566 2023-05-14 18:29:41.000000 Simba-UW-tf-dev-1.60.7/simba/bounding_box_tools/boundary_menus.py
--rw-r--r--   0 simon      (501) staff       (20)     8497 2023-05-14 18:22:39.000000 Simba-UW-tf-dev-1.60.7/simba/bounding_box_tools/boundary_statistics.py
--rw-r--r--   0 simon      (501) staff       (20)     6376 2023-05-15 16:44:53.000000 Simba-UW-tf-dev-1.60.7/simba/bounding_box_tools/find_boundaries.py
--rw-r--r--   0 simon      (501) staff       (20)    11381 2023-05-15 16:44:53.000000 Simba-UW-tf-dev-1.60.7/simba/bounding_box_tools/visualize_boundaries.py
--rw-r--r--   0 simon      (501) staff       (20)    49156 2023-05-23 15:41:51.000000 Simba-UW-tf-dev-1.60.7/simba/.DS_Store
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-23 16:26:58.000000 Simba-UW-tf-dev-1.60.7/simba/feature_extractors/
--rw-r--r--   0 simon      (501) staff       (20)    42512 2023-05-15 00:05:22.000000 Simba-UW-tf-dev-1.60.7/simba/feature_extractors/feature_extractor_14bp.py
--rw-r--r--   0 simon      (501) staff       (20)    21482 2023-05-14 23:55:56.000000 Simba-UW-tf-dev-1.60.7/simba/feature_extractors/feature_extractor_7bp.py
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-23 16:26:58.000000 Simba-UW-tf-dev-1.60.7/simba/feature_extractors/misc/
--rw-r--r--   0 simon      (501) staff       (20)     1685 2023-04-14 17:52:01.000000 Simba-UW-tf-dev-1.60.7/simba/feature_extractors/misc/doctests.py
--rw-r--r--   0 simon      (501) staff       (20)    23850 2023-04-17 18:48:40.000000 Simba-UW-tf-dev-1.60.7/simba/feature_extractors/misc/fish_feature_extractor_2023_version_3.py
--rw-r--r--   0 simon      (501) staff       (20)     2732 2023-04-04 19:46:36.000000 Simba-UW-tf-dev-1.60.7/simba/feature_extractors/misc/read_in_mp.py
--rw-r--r--   0 simon      (501) staff       (20)     2460 2023-04-22 18:02:29.000000 Simba-UW-tf-dev-1.60.7/simba/feature_extractors/misc/peaks.py
--rw-r--r--   0 simon      (501) staff       (20)    14141 2023-03-15 17:20:08.000000 Simba-UW-tf-dev-1.60.7/simba/feature_extractors/misc/fish_feature_extractor_2022.py
--rw-r--r--   0 simon      (501) staff       (20)     2053 2023-04-04 03:00:41.000000 Simba-UW-tf-dev-1.60.7/simba/feature_extractors/misc/convex_hull_3_scratch_3.py
--rw-r--r--   0 simon      (501) staff       (20)     5762 2023-04-04 01:54:33.000000 Simba-UW-tf-dev-1.60.7/simba/feature_extractors/misc/convex_hull_scratch_1.py
--rw-r--r--   0 simon      (501) staff       (20)     6148 2023-03-14 19:36:02.000000 Simba-UW-tf-dev-1.60.7/simba/feature_extractors/misc/.DS_Store
--rw-r--r--   0 simon      (501) staff       (20)    21398 2023-04-16 17:03:37.000000 Simba-UW-tf-dev-1.60.7/simba/feature_extractors/misc/fish_feature_extractor_2023_version_2.py
--rw-r--r--   0 simon      (501) staff       (20)     7127 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.60.7/simba/feature_extractors/misc/egocentrical_aligner.py
--rw-r--r--   0 simon      (501) staff       (20)     1213 2023-04-11 20:12:47.000000 Simba-UW-tf-dev-1.60.7/simba/feature_extractors/misc/count_values_in_range.py
--rw-r--r--   0 simon      (501) staff       (20)     4708 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.60.7/simba/feature_extractors/misc/graph_creator.py
--rw-r--r--   0 simon      (501) staff       (20)     3954 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.60.7/simba/feature_extractors/misc/termite_rois.csv
--rw-r--r--   0 simon      (501) staff       (20)      732 2023-03-20 12:13:51.000000 Simba-UW-tf-dev-1.60.7/simba/feature_extractors/misc/mutual_exclusive.py
--rw-r--r--   0 simon      (501) staff       (20)     2841 2023-04-14 15:16:23.000000 Simba-UW-tf-dev-1.60.7/simba/feature_extractors/misc/video_color.py
--rw-r--r--   0 simon      (501) staff       (20)     1862 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.60.7/simba/feature_extractors/misc/graph_3d_plotter.py
--rw-r--r--   0 simon      (501) staff       (20)     5232 2023-04-13 14:05:29.000000 Simba-UW-tf-dev-1.60.7/simba/feature_extractors/misc/video_rotator.py
--rw-r--r--   0 simon      (501) staff       (20)     2692 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.60.7/simba/feature_extractors/misc/add_probability_cnt_features.py
--rw-r--r--   0 simon      (501) staff       (20)     1619 2023-04-08 20:02:08.000000 Simba-UW-tf-dev-1.60.7/simba/feature_extractors/misc/make_splash.py
--rw-r--r--   0 simon      (501) staff       (20)    30661 2023-05-19 20:46:44.000000 Simba-UW-tf-dev-1.60.7/simba/feature_extractors/misc/fish_feature_extractor_2023_version_5.py
--rw-r--r--   0 simon      (501) staff       (20)     1658 2023-04-22 19:16:28.000000 Simba-UW-tf-dev-1.60.7/simba/feature_extractors/misc/time_stamp_calculator.py
--rw-r--r--   0 simon      (501) staff       (20)     5232 2023-04-15 19:24:18.000000 Simba-UW-tf-dev-1.60.7/simba/feature_extractors/misc/video_rotator_mp.py
--rw-r--r--   0 simon      (501) staff       (20)    30661 2023-05-19 20:44:29.000000 Simba-UW-tf-dev-1.60.7/simba/feature_extractors/misc/fish_feature_extractor_2023_version_4.py
--rw-r--r--   0 simon      (501) staff       (20)     2058 2023-04-03 23:51:37.000000 Simba-UW-tf-dev-1.60.7/simba/feature_extractors/misc/convex_hull_scratch_2.py
--rw-r--r--   0 simon      (501) staff       (20)    27995 2023-05-15 00:05:22.000000 Simba-UW-tf-dev-1.60.7/simba/feature_extractors/feature_extractor_8bps_2_animals.py
--rw-r--r--   0 simon      (501) staff       (20)    10244 2023-05-19 20:03:28.000000 Simba-UW-tf-dev-1.60.7/simba/feature_extractors/.DS_Store
--rw-r--r--   0 simon      (501) staff       (20)     3864 2023-05-19 19:41:40.000000 Simba-UW-tf-dev-1.60.7/simba/feature_extractors/perimeter_jit.py
--rw-r--r--   0 simon      (501) staff       (20)    13579 2023-05-14 19:53:33.000000 Simba-UW-tf-dev-1.60.7/simba/feature_extractors/feature_subsets.py
--rw-r--r--   0 simon      (501) staff       (20)        0 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.60.7/simba/feature_extractors/__init__.py
--rw-r--r--   0 simon      (501) staff       (20)     8244 2023-05-21 16:28:49.000000 Simba-UW-tf-dev-1.60.7/simba/feature_extractors/feature_extractor_user_defined.py
--rw-r--r--   0 simon      (501) staff       (20)    46461 2023-05-15 00:03:36.000000 Simba-UW-tf-dev-1.60.7/simba/feature_extractors/feature_extractor_16bp.py
--rw-r--r--   0 simon      (501) staff       (20)    28259 2023-05-15 00:05:22.000000 Simba-UW-tf-dev-1.60.7/simba/feature_extractors/feature_extractor_9bp.py
--rw-r--r--   0 simon      (501) staff       (20)    23976 2023-05-15 00:01:21.000000 Simba-UW-tf-dev-1.60.7/simba/feature_extractors/feature_extractor_8bp.py
--rw-r--r--   0 simon      (501) staff       (20)    16880 2023-05-14 23:53:59.000000 Simba-UW-tf-dev-1.60.7/simba/feature_extractors/feature_extractor_4bp.py
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-23 16:26:58.000000 Simba-UW-tf-dev-1.60.7/simba/feature_extractors/.idea/
--rw-r--r--   0 simon      (501) staff       (20)      617 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.60.7/simba/feature_extractors/.idea/features_scripts.iml
--rw-r--r--   0 simon      (501) staff       (20)      138 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.60.7/simba/feature_extractors/.idea/encodings.xml
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-23 16:26:58.000000 Simba-UW-tf-dev-1.60.7/simba/feature_extractors/.idea/inspectionProfiles/
--rw-r--r--   0 simon      (501) staff       (20)      822 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.60.7/simba/feature_extractors/.idea/inspectionProfiles/Project_Default.xml
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-23 16:26:58.000000 Simba-UW-tf-dev-1.60.7/simba/feature_extractors/.idea/libraries/
--rw-r--r--   0 simon      (501) staff       (20)      128 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.60.7/simba/feature_extractors/.idea/libraries/R_User_Library.xml
--rw-r--r--   0 simon      (501) staff       (20)      273 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.60.7/simba/feature_extractors/.idea/.gitignore
--rw-r--r--   0 simon      (501) staff       (20)     8081 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.60.7/simba/feature_extractors/.idea/workspace.xml
--rw-r--r--   0 simon      (501) staff       (20)      291 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.60.7/simba/feature_extractors/.idea/modules.xml
--rw-r--r--   0 simon      (501) staff       (20)       23 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.60.7/simba/feature_extractors/.idea/.name
--rw-r--r--   0 simon      (501) staff       (20)      294 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.60.7/simba/feature_extractors/.idea/misc.xml
--rw-r--r--   0 simon      (501) staff       (20)    15434 2023-05-20 18:29:53.000000 Simba-UW-tf-dev-1.60.7/simba/requirements.txt
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-23 16:26:58.000000 Simba-UW-tf-dev-1.60.7/simba/mixins/
--rw-r--r--   0 simon      (501) staff       (20)     6148 2023-03-15 17:26:03.000000 Simba-UW-tf-dev-1.60.7/simba/mixins/.DS_Store
--rw-r--r--   0 simon      (501) staff       (20)    42134 2023-05-16 16:45:46.000000 Simba-UW-tf-dev-1.60.7/simba/mixins/pop_up_mixin.py
--rw-r--r--   0 simon      (501) staff       (20)    30127 2023-05-23 12:26:01.000000 Simba-UW-tf-dev-1.60.7/simba/mixins/config_reader.py
--rw-r--r--   0 simon      (501) staff       (20)        0 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.60.7/simba/mixins/__init__.py
--rw-r--r--   0 simon      (501) staff       (20)    18616 2023-05-17 19:39:33.000000 Simba-UW-tf-dev-1.60.7/simba/mixins/pose_importer_mixin.py
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-23 16:26:58.000000 Simba-UW-tf-dev-1.60.7/simba/mixins/__pycache__/
--rw-r--r--   0 simon      (501) staff       (20)     1223 2023-05-21 16:37:18.000000 Simba-UW-tf-dev-1.60.7/simba/mixins/__pycache__/feature_extraction_mixin.FeatureExtractionMixin.cdist-333.py36m.nbi
--rw-r--r--   0 simon      (501) staff       (20)     1118 2023-05-21 00:18:56.000000 Simba-UW-tf-dev-1.60.7/simba/mixins/__pycache__/feature_extraction_mixin.FeatureExtractionMixin.angle3pt-84.py36m.nbi
--rw-r--r--   0 simon      (501) staff       (20)    51809 2023-05-21 16:37:18.000000 Simba-UW-tf-dev-1.60.7/simba/mixins/__pycache__/feature_extraction_mixin.FeatureExtractionMixin.cdist-333.py36m.1.nbc
--rw-r--r--   0 simon      (501) staff       (20)    14188 2023-05-21 00:18:56.000000 Simba-UW-tf-dev-1.60.7/simba/mixins/__pycache__/feature_extraction_mixin.FeatureExtractionMixin.angle3pt-84.py36m.1.nbc
--rw-r--r--   0 simon      (501) staff       (20)    37100 2023-05-19 15:31:55.000000 Simba-UW-tf-dev-1.60.7/simba/mixins/feature_extraction_mixin.py
--rw-r--r--   0 simon      (501) staff       (20)    61873 2023-05-19 21:14:46.000000 Simba-UW-tf-dev-1.60.7/simba/mixins/plotting_mixin.py
--rw-r--r--   0 simon      (501) staff       (20)     6175 2023-05-02 18:14:28.000000 Simba-UW-tf-dev-1.60.7/simba/mixins/unsupervised_mixin.py
--rw-r--r--   0 simon      (501) staff       (20)    60756 2023-05-18 20:03:49.000000 Simba-UW-tf-dev-1.60.7/simba/mixins/train_model_mixin.py
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-23 16:26:59.000000 Simba-UW-tf-dev-1.60.7/simba/third_party_label_appenders/
--rw-r--r--   0 simon      (501) staff       (20)     6094 2023-05-21 17:39:19.000000 Simba-UW-tf-dev-1.60.7/simba/third_party_label_appenders/deepethogram_importer.py
--rw-r--r--   0 simon      (501) staff       (20)    10623 2023-05-21 18:42:05.000000 Simba-UW-tf-dev-1.60.7/simba/third_party_label_appenders/BORIS_appender.py
--rw-r--r--   0 simon      (501) staff       (20)     8998 2023-05-15 17:20:07.000000 Simba-UW-tf-dev-1.60.7/simba/third_party_label_appenders/observer_importer.py
--rw-r--r--   0 simon      (501) staff       (20)    17954 2023-05-21 15:57:11.000000 Simba-UW-tf-dev-1.60.7/simba/third_party_label_appenders/tools.py
--rw-r--r--   0 simon      (501) staff       (20)        0 2023-04-01 14:10:06.000000 Simba-UW-tf-dev-1.60.7/simba/third_party_label_appenders/__init__.py
--rw-r--r--   0 simon      (501) staff       (20)    18224 2023-05-15 17:20:07.000000 Simba-UW-tf-dev-1.60.7/simba/third_party_label_appenders/third_party_appender.py
--rw-r--r--   0 simon      (501) staff       (20)     8181 2023-05-21 17:19:25.000000 Simba-UW-tf-dev-1.60.7/simba/third_party_label_appenders/ethovision_import.py
--rw-r--r--   0 simon      (501) staff       (20)     6988 2023-05-21 17:31:04.000000 Simba-UW-tf-dev-1.60.7/simba/third_party_label_appenders/BENTO_appender.py
--rw-r--r--   0 simon      (501) staff       (20)     5239 2023-05-21 18:07:18.000000 Simba-UW-tf-dev-1.60.7/simba/third_party_label_appenders/solomon_importer.py
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-23 16:26:58.000000 Simba-UW-tf-dev-1.60.7/simba/cue_light_tools/
--rw-r--r--   0 simon      (501) staff       (20)     6148 2023-05-20 18:06:55.000000 Simba-UW-tf-dev-1.60.7/simba/cue_light_tools/.DS_Store
--rw-r--r--   0 simon      (501) staff       (20)     7652 2023-05-15 16:44:53.000000 Simba-UW-tf-dev-1.60.7/simba/cue_light_tools/cue_light_clf_statistics.py
--rw-r--r--   0 simon      (501) staff       (20)    12207 2023-05-15 16:44:53.000000 Simba-UW-tf-dev-1.60.7/simba/cue_light_tools/cue_light_analyzer.py
--rw-r--r--   0 simon      (501) staff       (20)    16690 2023-05-15 16:44:53.000000 Simba-UW-tf-dev-1.60.7/simba/cue_light_tools/cue_light_menues.py
--rw-r--r--   0 simon      (501) staff       (20)        0 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.60.7/simba/cue_light_tools/__init__.py
--rw-r--r--   0 simon      (501) staff       (20)     1879 2023-05-15 16:44:53.000000 Simba-UW-tf-dev-1.60.7/simba/cue_light_tools/cue_light_tools.py
--rw-r--r--   0 simon      (501) staff       (20)    15212 2023-05-16 18:48:44.000000 Simba-UW-tf-dev-1.60.7/simba/cue_light_tools/cue_light_visualizer.py
--rw-r--r--   0 simon      (501) staff       (20)    12650 2023-05-15 16:44:53.000000 Simba-UW-tf-dev-1.60.7/simba/cue_light_tools/cue_light_movement_statistics.py
--rw-r--r--   0 simon      (501) staff       (20)        0 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.60.7/simba/__init__.py
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-23 16:26:59.000000 Simba-UW-tf-dev-1.60.7/simba/utils/
--rw-r--r--   0 simon      (501) staff       (20)    11899 2023-05-15 12:44:10.000000 Simba-UW-tf-dev-1.60.7/simba/utils/config_creator.py
--rw-r--r--   0 simon      (501) staff       (20)    20972 2023-05-08 18:03:19.000000 Simba-UW-tf-dev-1.60.7/simba/utils/enums.py
--rw-r--r--   0 simon      (501) staff       (20)     8196 2023-05-20 18:15:51.000000 Simba-UW-tf-dev-1.60.7/simba/utils/.DS_Store
--rw-r--r--   0 simon      (501) staff       (20)     7365 2023-04-27 20:23:35.000000 Simba-UW-tf-dev-1.60.7/simba/utils/warnings.py
--rw-r--r--   0 simon      (501) staff       (20)     8800 2023-05-16 00:24:15.000000 Simba-UW-tf-dev-1.60.7/simba/utils/checks.py
--rw-r--r--   0 simon      (501) staff       (20)        0 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.60.7/simba/utils/__init__.py
--rw-r--r--   0 simon      (501) staff       (20)    41782 2023-05-21 17:06:37.000000 Simba-UW-tf-dev-1.60.7/simba/utils/read_write.py
--rw-r--r--   0 simon      (501) staff       (20)     8240 2023-05-15 14:49:42.000000 Simba-UW-tf-dev-1.60.7/simba/utils/lookups.py
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-23 16:26:59.000000 Simba-UW-tf-dev-1.60.7/simba/utils/cli/
--rw-r--r--   0 simon      (501) staff       (20)        0 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.60.7/simba/utils/cli/__init__.py
--rw-r--r--   0 simon      (501) staff       (20)     3227 2023-05-15 15:41:04.000000 Simba-UW-tf-dev-1.60.7/simba/utils/cli/cli_tools.py
--rw-r--r--   0 simon      (501) staff       (20)    14666 2023-04-28 19:59:06.000000 Simba-UW-tf-dev-1.60.7/simba/utils/errors.py
--rw-r--r--   0 simon      (501) staff       (20)    15392 2023-05-15 15:08:26.000000 Simba-UW-tf-dev-1.60.7/simba/utils/data.py
--rw-r--r--   0 simon      (501) staff       (20)     1615 2023-05-08 18:13:22.000000 Simba-UW-tf-dev-1.60.7/simba/utils/printing.py
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-23 16:26:59.000000 Simba-UW-tf-dev-1.60.7/simba/pose_processors/
--rw-r--r--   0 simon      (501) staff       (20)     8256 2023-05-15 16:58:05.000000 Simba-UW-tf-dev-1.60.7/simba/pose_processors/reorganize_keypoint.py
--rw-r--r--   0 simon      (501) staff       (20)     5167 2023-05-15 16:58:05.000000 Simba-UW-tf-dev-1.60.7/simba/pose_processors/remove_keypoints.py
--rw-r--r--   0 simon      (501) staff       (20)        0 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.60.7/simba/pose_processors/__init__.py
--rw-r--r--   0 simon      (501) staff       (20)     2656 2023-05-15 16:58:04.000000 Simba-UW-tf-dev-1.60.7/simba/pose_processors/pose_reset.py
--rw-r--r--   0 simon      (501) staff       (20)     5614 2023-05-04 15:35:50.000000 Simba-UW-tf-dev-1.60.7/simba/pose_processors/reverse_pose.py
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-23 16:26:58.000000 Simba-UW-tf-dev-1.60.7/simba/plotting/
--rw-r--r--   0 simon      (501) staff       (20)     9114 2023-05-15 17:45:06.000000 Simba-UW-tf-dev-1.60.7/simba/plotting/gantt_creator.py
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-23 16:26:58.000000 Simba-UW-tf-dev-1.60.7/simba/plotting/tools/
--rw-r--r--   0 simon      (501) staff       (20)     5388 2023-04-27 20:23:35.000000 Simba-UW-tf-dev-1.60.7/simba/plotting/tools/tkinter_tools.py
--rw-r--r--   0 simon      (501) staff       (20)    13144 2023-05-17 13:58:48.000000 Simba-UW-tf-dev-1.60.7/simba/plotting/ROI_plotter_mp.py
--rw-r--r--   0 simon      (501) staff       (20)     6148 2023-04-25 23:35:57.000000 Simba-UW-tf-dev-1.60.7/simba/plotting/.DS_Store
--rw-r--r--   0 simon      (501) staff       (20)    14568 2023-05-15 18:41:17.000000 Simba-UW-tf-dev-1.60.7/simba/plotting/shap_agg_stats_visualizer.py
--rw-r--r--   0 simon      (501) staff       (20)    10105 2023-05-15 17:45:06.000000 Simba-UW-tf-dev-1.60.7/simba/plotting/gantt_creator_mp.py
--rw-r--r--   0 simon      (501) staff       (20)    15730 2023-05-15 17:49:01.000000 Simba-UW-tf-dev-1.60.7/simba/plotting/heat_mapper_clf_mp.py
--rw-r--r--   0 simon      (501) staff       (20)     8731 2023-05-15 18:13:11.000000 Simba-UW-tf-dev-1.60.7/simba/plotting/probability_plot_creator.py
--rw-r--r--   0 simon      (501) staff       (20)    12484 2023-05-23 14:52:24.000000 Simba-UW-tf-dev-1.60.7/simba/plotting/plot_clf_results.py
--rw-r--r--   0 simon      (501) staff       (20)    14056 2023-05-17 14:20:24.000000 Simba-UW-tf-dev-1.60.7/simba/plotting/plot_clf_results_mp.py
--rw-r--r--   0 simon      (501) staff       (20)    16031 2023-05-15 18:13:11.000000 Simba-UW-tf-dev-1.60.7/simba/plotting/ROI_feature_visualizer.py
--rw-r--r--   0 simon      (501) staff       (20)    12770 2023-05-15 18:08:47.000000 Simba-UW-tf-dev-1.60.7/simba/plotting/heat_mapper_location.py
--rw-r--r--   0 simon      (501) staff       (20)    10100 2023-05-15 18:13:11.000000 Simba-UW-tf-dev-1.60.7/simba/plotting/probability_plot_creator_mp.py
--rw-r--r--   0 simon      (501) staff       (20)        0 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.60.7/simba/plotting/__init__.py
--rw-r--r--   0 simon      (501) staff       (20)     4881 2023-05-15 18:08:47.000000 Simba-UW-tf-dev-1.60.7/simba/plotting/interactive_probability_grapher.py
--rw-r--r--   0 simon      (501) staff       (20)     5812 2023-05-15 18:08:47.000000 Simba-UW-tf-dev-1.60.7/simba/plotting/plot_pose_in_dir.py
--rw-r--r--   0 simon      (501) staff       (20)    13770 2023-05-23 16:26:11.000000 Simba-UW-tf-dev-1.60.7/simba/plotting/single_run_model_validation_video.py
--rw-r--r--   0 simon      (501) staff       (20)    12790 2023-05-16 16:20:20.000000 Simba-UW-tf-dev-1.60.7/simba/plotting/frame_mergerer_ffmpeg.py
--rw-r--r--   0 simon      (501) staff       (20)     7915 2023-05-16 16:18:45.000000 Simba-UW-tf-dev-1.60.7/simba/plotting/Directing_animals_visualizer_mp.py
--rw-r--r--   0 simon      (501) staff       (20)    11219 2023-05-17 12:58:17.000000 Simba-UW-tf-dev-1.60.7/simba/plotting/clf_validator.py
--rw-r--r--   0 simon      (501) staff       (20)    15745 2023-05-20 12:16:06.000000 Simba-UW-tf-dev-1.60.7/simba/plotting/path_plotter_mp.py
--rw-r--r--   0 simon      (501) staff       (20)    11204 2023-05-15 18:33:52.000000 Simba-UW-tf-dev-1.60.7/simba/plotting/ROI_feature_visualizer_mp.py
--rw-r--r--   0 simon      (501) staff       (20)     8933 2023-05-16 16:18:45.000000 Simba-UW-tf-dev-1.60.7/simba/plotting/data_plotter.py
--rw-r--r--   0 simon      (501) staff       (20)    13471 2023-05-20 12:15:46.000000 Simba-UW-tf-dev-1.60.7/simba/plotting/path_plotter.py
--rw-r--r--   0 simon      (501) staff       (20)     6494 2023-05-17 20:55:17.000000 Simba-UW-tf-dev-1.60.7/simba/plotting/ez_lineplot.py
--rw-r--r--   0 simon      (501) staff       (20)    11491 2023-05-15 17:45:06.000000 Simba-UW-tf-dev-1.60.7/simba/plotting/distance_plotter_mp.py
--rw-r--r--   0 simon      (501) staff       (20)    15794 2023-05-17 13:58:48.000000 Simba-UW-tf-dev-1.60.7/simba/plotting/ROI_plotter.py
--rw-r--r--   0 simon      (501) staff       (20)    13163 2023-05-16 16:42:03.000000 Simba-UW-tf-dev-1.60.7/simba/plotting/heat_mapper_clf.py
--rw-r--r--   0 simon      (501) staff       (20)     9113 2023-05-14 23:44:34.000000 Simba-UW-tf-dev-1.60.7/simba/plotting/distance_plotter.py
--rw-r--r--   0 simon      (501) staff       (20)     9274 2023-05-23 16:26:19.000000 Simba-UW-tf-dev-1.60.7/simba/plotting/single_run_model_validation_video_mp.py
--rw-r--r--   0 simon      (501) staff       (20)     9926 2023-05-16 16:20:20.000000 Simba-UW-tf-dev-1.60.7/simba/plotting/Directing_animals_visualizer.py
--rw-r--r--   0 simon      (501) staff       (20)    16320 2023-05-15 18:08:47.000000 Simba-UW-tf-dev-1.60.7/simba/plotting/heat_mapper_location_mp.py
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-23 16:26:58.000000 Simba-UW-tf-dev-1.60.7/simba/dash_app/
--rw-r--r--   0 simon      (501) staff       (20)    49699 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.60.7/simba/dash_app/SimBA_dash_app.py
--rw-r--r--   0 simon      (501) staff       (20)     5029 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.60.7/simba/dash_app/run_dash_tkinter.py
--rw-r--r--   0 simon      (501) staff       (20)    24474 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.60.7/simba/dash_app/dash_app.py
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-23 16:26:58.000000 Simba-UW-tf-dev-1.60.7/simba/data_processors/
--rw-r--r--   0 simon      (501) staff       (20)     6501 2023-05-18 22:42:15.000000 Simba-UW-tf-dev-1.60.7/simba/data_processors/agg_clf_calculator.py
--rw-r--r--   0 simon      (501) staff       (20)    12401 2023-05-23 15:41:17.000000 Simba-UW-tf-dev-1.60.7/simba/data_processors/severity_bout_based_calculator.py
--rw-r--r--   0 simon      (501) staff       (20)    16259 2023-05-19 18:26:50.000000 Simba-UW-tf-dev-1.60.7/simba/data_processors/interpolation_smoothing.py
--rw-r--r--   0 simon      (501) staff       (20)     7828 2023-05-14 19:47:31.000000 Simba-UW-tf-dev-1.60.7/simba/data_processors/timebins_clf_calculator.py
--rw-r--r--   0 simon      (501) staff       (20)    12908 2023-05-18 13:34:46.000000 Simba-UW-tf-dev-1.60.7/simba/data_processors/fsttc_calculator.py
--rw-r--r--   0 simon      (501) staff       (20)        0 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.60.7/simba/data_processors/__init__.py
--rw-r--r--   0 simon      (501) staff       (20)     6306 2023-05-13 17:09:38.000000 Simba-UW-tf-dev-1.60.7/simba/data_processors/interpolate_pose.py
--rw-r--r--   0 simon      (501) staff       (20)     9646 2023-05-14 19:19:14.000000 Simba-UW-tf-dev-1.60.7/simba/data_processors/directing_other_animals_calculator.py
--rw-r--r--   0 simon      (501) staff       (20)     8550 2023-05-14 19:47:31.000000 Simba-UW-tf-dev-1.60.7/simba/data_processors/timebins_movement_calculator.py
--rw-r--r--   0 simon      (501) staff       (20)     4799 2023-05-17 17:23:16.000000 Simba-UW-tf-dev-1.60.7/simba/data_processors/severity_calculator.py
--rw-r--r--   0 simon      (501) staff       (20)    16980 2023-05-14 19:47:31.000000 Simba-UW-tf-dev-1.60.7/simba/data_processors/pup_retrieval_calculator.py
--rw-r--r--   0 simon      (501) staff       (20)     3143 2023-05-13 17:23:00.000000 Simba-UW-tf-dev-1.60.7/simba/data_processors/pybursts_calculator.py
--rw-r--r--   0 simon      (501) staff       (20)     7725 2023-05-23 14:26:19.000000 Simba-UW-tf-dev-1.60.7/simba/data_processors/severity_frame_based_calculator.py
--rw-r--r--   0 simon      (501) staff       (20)     9649 2023-05-18 13:48:41.000000 Simba-UW-tf-dev-1.60.7/simba/data_processors/kleinberg_calculator.py
--rw-r--r--   0 simon      (501) staff       (20)     8129 2023-05-18 13:31:03.000000 Simba-UW-tf-dev-1.60.7/simba/data_processors/movement_calculator.py
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-23 16:26:58.000000 Simba-UW-tf-dev-1.60.7/simba/pose_configurations_archive/
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-23 16:26:58.000000 Simba-UW-tf-dev-1.60.7/simba/pose_configurations_archive/pose_configurations_archive_1/
--rw-r--r--   0 simon      (501) staff       (20)    14340 2023-03-30 11:05:37.000000 Simba-UW-tf-dev-1.60.7/simba/pose_configurations_archive/pose_configurations_archive_1/.DS_Store
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-23 16:26:58.000000 Simba-UW-tf-dev-1.60.7/simba/pose_configurations_archive/pose_configurations_archive_1/bp_names/
--rw-r--r--   0 simon      (501) staff       (20)     6148 2023-03-16 13:26:00.000000 Simba-UW-tf-dev-1.60.7/simba/pose_configurations_archive/pose_configurations_archive_1/bp_names/.DS_Store
--rw-r--r--   0 simon      (501) staff       (20)     1334 2023-04-28 23:45:27.000000 Simba-UW-tf-dev-1.60.7/simba/pose_configurations_archive/pose_configurations_archive_1/bp_names/bp_names.csv
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-23 16:26:58.000000 Simba-UW-tf-dev-1.60.7/simba/pose_configurations_archive/pose_configurations_archive_1/no_animals/
--rw-r--r--   0 simon      (501) staff       (20)       26 2023-04-28 23:45:27.000000 Simba-UW-tf-dev-1.60.7/simba/pose_configurations_archive/pose_configurations_archive_1/no_animals/no_animals.csv
--rw-r--r--   0 simon      (501) staff       (20)     6148 2023-03-16 13:26:19.000000 Simba-UW-tf-dev-1.60.7/simba/pose_configurations_archive/pose_configurations_archive_1/no_animals/.DS_Store
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-23 16:26:58.000000 Simba-UW-tf-dev-1.60.7/simba/pose_configurations_archive/pose_configurations_archive_1/configuration_names/
--rw-r--r--   0 simon      (501) staff       (20)     6148 2023-03-16 13:26:14.000000 Simba-UW-tf-dev-1.60.7/simba/pose_configurations_archive/pose_configurations_archive_1/configuration_names/.DS_Store
--rw-r--r--   0 simon      (501) staff       (20)      282 2023-04-28 23:45:27.000000 Simba-UW-tf-dev-1.60.7/simba/pose_configurations_archive/pose_configurations_archive_1/configuration_names/pose_config_names.csv
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-23 16:26:58.000000 Simba-UW-tf-dev-1.60.7/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/
--rw-r--r--   0 simon      (501) staff       (20)     8196 2023-03-30 10:45:10.000000 Simba-UW-tf-dev-1.60.7/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/.DS_Store
--rw-r--r--   0 simon      (501) staff       (20)    39805 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.60.7/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/8.png
--rw-r--r--   0 simon      (501) staff       (20)    62501 2023-03-30 10:39:05.000000 Simba-UW-tf-dev-1.60.7/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/9.png
--rw-r--r--   0 simon      (501) staff       (20)     6172 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.60.7/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/12.png
--rw-r--r--   0 simon      (501) staff       (20)    11376 2023-04-28 23:45:27.000000 Simba-UW-tf-dev-1.60.7/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/13.png
--rw-r--r--   0 simon      (501) staff       (20)    69501 2023-03-30 10:44:04.000000 Simba-UW-tf-dev-1.60.7/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/11.png
--rw-r--r--   0 simon      (501) staff       (20)    69410 2023-03-30 10:40:01.000000 Simba-UW-tf-dev-1.60.7/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/10.png
--rw-r--r--   0 simon      (501) staff       (20)    16000 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.60.7/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/4.png
--rw-r--r--   0 simon      (501) staff       (20)    28150 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.60.7/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/5.png
--rw-r--r--   0 simon      (501) staff       (20)    31140 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.60.7/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/7.png
--rw-r--r--   0 simon      (501) staff       (20)    30634 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.60.7/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/6.png
--rw-r--r--   0 simon      (501) staff       (20)    15417 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.60.7/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/2.png
--rw-r--r--   0 simon      (501) staff       (20)    15786 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.60.7/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/3.png
--rw-r--r--   0 simon      (501) staff       (20)    18939 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.60.7/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/1.png
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-23 16:26:58.000000 Simba-UW-tf-dev-1.60.7/simba/model/
--rw-r--r--   0 simon      (501) staff       (20)    19026 2023-05-19 11:15:45.000000 Simba-UW-tf-dev-1.60.7/simba/model/train_rf.py
--rw-r--r--   0 simon      (501) staff       (20)     6148 2023-05-20 18:06:50.000000 Simba-UW-tf-dev-1.60.7/simba/model/.DS_Store
--rw-r--r--   0 simon      (501) staff       (20)     3315 2023-05-18 22:48:36.000000 Simba-UW-tf-dev-1.60.7/simba/model/inference_batch.py
--rw-r--r--   0 simon      (501) staff       (20)    18876 2023-05-18 22:48:36.000000 Simba-UW-tf-dev-1.60.7/simba/model/grid_search_rf.py
--rw-r--r--   0 simon      (501) staff       (20)     3363 2023-05-19 11:12:45.000000 Simba-UW-tf-dev-1.60.7/simba/model/inference_validation.py
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-23 16:26:59.000000 Simba-UW-tf-dev-1.60.7/simba/roi_tools/
--rw-r--r--   0 simon      (501) staff       (20)     5858 2023-05-15 17:20:07.000000 Simba-UW-tf-dev-1.60.7/simba/roi_tools/ROI_time_bin_calculator.py
--rw-r--r--   0 simon      (501) staff       (20)     1687 2023-05-15 17:20:07.000000 Simba-UW-tf-dev-1.60.7/simba/roi_tools/ROI_movement_analyzer.py
--rw-r--r--   0 simon      (501) staff       (20)     6148 2023-03-20 12:47:56.000000 Simba-UW-tf-dev-1.60.7/simba/roi_tools/.DS_Store
--rw-r--r--   0 simon      (501) staff       (20)    43119 2023-05-14 16:11:59.000000 Simba-UW-tf-dev-1.60.7/simba/roi_tools/ROI_define.py
--rw-r--r--   0 simon      (501) staff       (20)     4024 2023-05-16 13:21:43.000000 Simba-UW-tf-dev-1.60.7/simba/roi_tools/ROI_reset.py
--rw-r--r--   0 simon      (501) staff       (20)        0 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.60.7/simba/roi_tools/__init__.py
--rw-r--r--   0 simon      (501) staff       (20)    19901 2023-05-15 17:00:34.000000 Simba-UW-tf-dev-1.60.7/simba/roi_tools/ROI_analyzer.py
--rw-r--r--   0 simon      (501) staff       (20)    11608 2023-05-15 17:12:32.000000 Simba-UW-tf-dev-1.60.7/simba/roi_tools/ROI_feature_analyzer.py
--rw-r--r--   0 simon      (501) staff       (20)     3654 2023-04-29 19:01:32.000000 Simba-UW-tf-dev-1.60.7/simba/roi_tools/ROI_multiply.py
--rw-r--r--   0 simon      (501) staff       (20)      959 2023-05-15 17:20:07.000000 Simba-UW-tf-dev-1.60.7/simba/roi_tools/ROI_size_calculations.py
--rw-r--r--   0 simon      (501) staff       (20)     3505 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.60.7/simba/roi_tools/ROI_zoom.py
--rw-r--r--   0 simon      (501) staff       (20)    11556 2023-05-15 17:12:32.000000 Simba-UW-tf-dev-1.60.7/simba/roi_tools/ROI_directing_analyzer.py
--rw-r--r--   0 simon      (501) staff       (20)    10128 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.60.7/simba/roi_tools/ROI_move_shape.py
--rw-r--r--   0 simon      (501) staff       (20)     5079 2023-04-29 19:01:32.000000 Simba-UW-tf-dev-1.60.7/simba/roi_tools/ROI_menus.py
--rw-r--r--   0 simon      (501) staff       (20)    13742 2023-05-15 17:12:32.000000 Simba-UW-tf-dev-1.60.7/simba/roi_tools/ROI_clf_calculator.py
--rw-r--r--   0 simon      (501) staff       (20)    22688 2023-04-29 19:01:32.000000 Simba-UW-tf-dev-1.60.7/simba/roi_tools/ROI_image.py
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-23 16:26:59.000000 Simba-UW-tf-dev-1.60.7/simba/pose_importers/
--rw-r--r--   0 simon      (501) staff       (20)     8115 2023-05-14 18:03:14.000000 Simba-UW-tf-dev-1.60.7/simba/pose_importers/sleap_csv_importer.py
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-23 16:26:59.000000 Simba-UW-tf-dev-1.60.7/simba/pose_importers/misc/
--rw-r--r--   0 simon      (501) staff       (20)     6148 2023-05-09 17:42:38.000000 Simba-UW-tf-dev-1.60.7/simba/pose_importers/misc/.DS_Store
--rw-r--r--   0 simon      (501) staff       (20)     7943 2023-05-01 19:07:14.000000 Simba-UW-tf-dev-1.60.7/simba/pose_importers/misc/apt_trk_importer.py
--rw-r--r--   0 simon      (501) staff       (20)     2464 2023-04-27 19:42:17.000000 Simba-UW-tf-dev-1.60.7/simba/pose_importers/read_DANNCE_mat.py
--rw-r--r--   0 simon      (501) staff       (20)     6148 2023-05-09 17:45:51.000000 Simba-UW-tf-dev-1.60.7/simba/pose_importers/.DS_Store
--rw-r--r--   0 simon      (501) staff       (20)    12549 2023-05-17 20:32:56.000000 Simba-UW-tf-dev-1.60.7/simba/pose_importers/sleap_h5_importer.py
--rw-r--r--   0 simon      (501) staff       (20)     7322 2023-05-16 16:55:05.000000 Simba-UW-tf-dev-1.60.7/simba/pose_importers/madlc_importer.py
--rw-r--r--   0 simon      (501) staff       (20)        0 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.60.7/simba/pose_importers/__init__.py
--rw-r--r--   0 simon      (501) staff       (20)    12141 2023-05-16 18:48:44.000000 Simba-UW-tf-dev-1.60.7/simba/pose_importers/sleap_slp_importer.py
--rw-r--r--   0 simon      (501) staff       (20)     7931 2023-05-15 16:58:04.000000 Simba-UW-tf-dev-1.60.7/simba/pose_importers/import_mars.py
--rw-r--r--   0 simon      (501) staff       (20)     6978 2023-05-15 16:44:53.000000 Simba-UW-tf-dev-1.60.7/simba/pose_importers/dlc_importer_csv.py
--rw-r--r--   0 simon      (501) staff       (20)     8060 2023-04-28 19:20:42.000000 Simba-UW-tf-dev-1.60.7/simba/pose_importers/trk_importer.py
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-23 16:26:58.000000 Simba-UW-tf-dev-1.60.7/simba/pose_configurations/
--rw-r--r--   0 simon      (501) staff       (20)    14340 2023-05-14 23:57:00.000000 Simba-UW-tf-dev-1.60.7/simba/pose_configurations/.DS_Store
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-23 16:26:58.000000 Simba-UW-tf-dev-1.60.7/simba/pose_configurations/bp_names/
--rw-r--r--   0 simon      (501) staff       (20)     6148 2023-03-16 13:26:00.000000 Simba-UW-tf-dev-1.60.7/simba/pose_configurations/bp_names/.DS_Store
--rw-r--r--   0 simon      (501) staff       (20)     1316 2023-04-29 18:20:02.000000 Simba-UW-tf-dev-1.60.7/simba/pose_configurations/bp_names/bp_names.csv
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-23 16:26:58.000000 Simba-UW-tf-dev-1.60.7/simba/pose_configurations/no_animals/
--rw-r--r--   0 simon      (501) staff       (20)       24 2023-04-29 18:20:02.000000 Simba-UW-tf-dev-1.60.7/simba/pose_configurations/no_animals/no_animals.csv
--rw-r--r--   0 simon      (501) staff       (20)     6148 2023-03-16 13:26:19.000000 Simba-UW-tf-dev-1.60.7/simba/pose_configurations/no_animals/.DS_Store
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-23 16:26:58.000000 Simba-UW-tf-dev-1.60.7/simba/pose_configurations/configuration_names/
--rw-r--r--   0 simon      (501) staff       (20)     6148 2023-03-16 13:26:14.000000 Simba-UW-tf-dev-1.60.7/simba/pose_configurations/configuration_names/.DS_Store
--rw-r--r--   0 simon      (501) staff       (20)      267 2023-04-29 18:20:02.000000 Simba-UW-tf-dev-1.60.7/simba/pose_configurations/configuration_names/pose_config_names.csv
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-23 16:26:58.000000 Simba-UW-tf-dev-1.60.7/simba/pose_configurations/schematics/
--rw-r--r--   0 simon      (501) staff       (20)    39805 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.60.7/simba/pose_configurations/schematics/8.png
--rw-r--r--   0 simon      (501) staff       (20)    62501 2023-03-30 10:39:05.000000 Simba-UW-tf-dev-1.60.7/simba/pose_configurations/schematics/9.png
--rw-r--r--   0 simon      (501) staff       (20)     6172 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.60.7/simba/pose_configurations/schematics/12.png
--rw-r--r--   0 simon      (501) staff       (20)    69501 2023-03-30 10:44:04.000000 Simba-UW-tf-dev-1.60.7/simba/pose_configurations/schematics/11.png
--rw-r--r--   0 simon      (501) staff       (20)    69410 2023-03-30 10:40:01.000000 Simba-UW-tf-dev-1.60.7/simba/pose_configurations/schematics/10.png
--rw-r--r--   0 simon      (501) staff       (20)    16000 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.60.7/simba/pose_configurations/schematics/4.png
--rw-r--r--   0 simon      (501) staff       (20)    28150 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.60.7/simba/pose_configurations/schematics/5.png
--rw-r--r--   0 simon      (501) staff       (20)    31140 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.60.7/simba/pose_configurations/schematics/7.png
--rw-r--r--   0 simon      (501) staff       (20)    30634 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.60.7/simba/pose_configurations/schematics/6.png
--rw-r--r--   0 simon      (501) staff       (20)    15417 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.60.7/simba/pose_configurations/schematics/2.png
--rw-r--r--   0 simon      (501) staff       (20)    15786 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.60.7/simba/pose_configurations/schematics/3.png
--rw-r--r--   0 simon      (501) staff       (20)    18939 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.60.7/simba/pose_configurations/schematics/1.png
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-23 16:26:59.000000 Simba-UW-tf-dev-1.60.7/simba/video_processors/
--rw-r--r--   0 simon      (501) staff       (20)    45564 2023-05-14 17:15:40.000000 Simba-UW-tf-dev-1.60.7/simba/video_processors/video_processing.py
--rw-r--r--   0 simon      (501) staff       (20)     8196 2023-05-20 18:15:51.000000 Simba-UW-tf-dev-1.60.7/simba/video_processors/.DS_Store
--rw-r--r--   0 simon      (501) staff       (20)     7171 2023-04-27 19:42:17.000000 Simba-UW-tf-dev-1.60.7/simba/video_processors/px_to_mm.py
--rw-r--r--   0 simon      (501) staff       (20)    24648 2023-05-16 16:42:04.000000 Simba-UW-tf-dev-1.60.7/simba/video_processors/batch_process_menus.py
--rw-r--r--   0 simon      (501) staff       (20)     7333 2023-05-16 12:54:28.000000 Simba-UW-tf-dev-1.60.7/simba/video_processors/multi_cropper.py
--rw-r--r--   0 simon      (501) staff       (20)     2833 2023-04-27 20:23:35.000000 Simba-UW-tf-dev-1.60.7/simba/video_processors/extract_frames.py
--rw-r--r--   0 simon      (501) staff       (20)        0 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.60.7/simba/video_processors/__init__.py
--rw-r--r--   0 simon      (501) staff       (20)     8266 2023-05-08 18:19:00.000000 Simba-UW-tf-dev-1.60.7/simba/video_processors/calculate_px_dist.py
--rw-r--r--   0 simon      (501) staff       (20)     4695 2023-04-26 18:17:53.000000 Simba-UW-tf-dev-1.60.7/simba/video_processors/extract_seqframes.py
--rw-r--r--   0 simon      (501) staff       (20)    11087 2023-05-14 16:24:59.000000 Simba-UW-tf-dev-1.60.7/simba/video_processors/batch_process_create_ffmpeg_commands.py
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-23 16:26:58.000000 Simba-UW-tf-dev-1.60.7/simba/outlier_tools/
--rw-r--r--   0 simon      (501) staff       (20)     6525 2023-05-19 17:31:41.000000 Simba-UW-tf-dev-1.60.7/simba/outlier_tools/outlier_corrector_movement.py
--rw-r--r--   0 simon      (501) staff       (20)     6148 2023-05-08 20:25:20.000000 Simba-UW-tf-dev-1.60.7/simba/outlier_tools/.DS_Store
--rw-r--r--   0 simon      (501) staff       (20)        0 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.60.7/simba/outlier_tools/__init__.py
--rw-r--r--   0 simon      (501) staff       (20)     8160 2023-05-19 18:34:50.000000 Simba-UW-tf-dev-1.60.7/simba/outlier_tools/outlier_corrector_location.py
--rw-r--r--   0 simon      (501) staff       (20)     2696 2023-05-23 12:33:12.000000 Simba-UW-tf-dev-1.60.7/simba/outlier_tools/skip_outlier_correction.py
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-23 16:26:58.000000 Simba-UW-tf-dev-1.60.7/simba/outlier_tools/.idea/
--rw-r--r--   0 simon      (501) staff       (20)      617 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.60.7/simba/outlier_tools/.idea/outlier_scripts.iml
--rw-r--r--   0 simon      (501) staff       (20)      138 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.60.7/simba/outlier_tools/.idea/encodings.xml
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-23 16:26:58.000000 Simba-UW-tf-dev-1.60.7/simba/outlier_tools/.idea/inspectionProfiles/
--rw-r--r--   0 simon      (501) staff       (20)      668 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.60.7/simba/outlier_tools/.idea/inspectionProfiles/Project_Default.xml
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-23 16:26:58.000000 Simba-UW-tf-dev-1.60.7/simba/outlier_tools/.idea/libraries/
--rw-r--r--   0 simon      (501) staff       (20)      128 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.60.7/simba/outlier_tools/.idea/libraries/R_User_Library.xml
--rw-r--r--   0 simon      (501) staff       (20)     8102 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.60.7/simba/outlier_tools/.idea/workspace.xml
--rw-r--r--   0 simon      (501) staff       (20)      289 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.60.7/simba/outlier_tools/.idea/modules.xml
--rw-r--r--   0 simon      (501) staff       (20)      294 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.60.7/simba/outlier_tools/.idea/misc.xml
--rw-r--r--   0 simon      (501) staff       (20)    64855 2023-05-21 18:08:05.000000 Simba-UW-tf-dev-1.60.7/simba/SimBA.py
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-23 16:26:58.000000 Simba-UW-tf-dev-1.60.7/simba/assets/
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-23 16:26:58.000000 Simba-UW-tf-dev-1.60.7/simba/assets/unsupervised/
--rw-r--r--   0 simon      (501) staff       (20)     6148 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.60.7/simba/assets/unsupervised/.DS_Store
--rw-r--r--   0 simon      (501) staff       (20)   109483 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.60.7/simba/assets/unsupervised/model_names.parquet
--rw-r--r--   0 simon      (501) staff       (20)    14175 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.60.7/simba/assets/unsupervised/features.csv
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-23 16:26:58.000000 Simba-UW-tf-dev-1.60.7/simba/assets/shap/
--rw-r--r--   0 simon      (501) staff       (20)     1177 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.60.7/simba/assets/shap/down_arrow.jpg
--rw-r--r--   0 simon      (501) staff       (20)     1733 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.60.7/simba/assets/shap/intruder_shape.jpg
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-23 16:26:58.000000 Simba-UW-tf-dev-1.60.7/simba/assets/shap/feature_categories/
--rw-r--r--   0 simon      (501) staff       (20)      109 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.60.7/simba/assets/shap/feature_categories/.~lock.shap_feature_categories.csv#
--rw-r--r--   0 simon      (501) staff       (20)    17420 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.60.7/simba/assets/shap/feature_categories/shap_feature_categories.csv
--rw-r--r--   0 simon      (501) staff       (20)     8196 2023-04-10 20:37:13.000000 Simba-UW-tf-dev-1.60.7/simba/assets/shap/.DS_Store
--rw-r--r--   0 simon      (501) staff       (20)     1665 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.60.7/simba/assets/shap/resident_shape.jpg
--rw-r--r--   0 simon      (501) staff       (20)     2415 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.60.7/simba/assets/shap/resident_intruder_shape.jpg
--rw-r--r--   0 simon      (501) staff       (20)     2012 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.60.7/simba/assets/shap/animal_distances.jpg
--rw-r--r--   0 simon      (501) staff       (20)     4422 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.60.7/simba/assets/shap/baseline_scale.jpg
--rw-r--r--   0 simon      (501) staff       (20)   353824 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.60.7/simba/assets/shap/ubuntu.regular.ttf
--rw-r--r--   0 simon      (501) staff       (20)     6672 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.60.7/simba/assets/shap/side_scale.jpg
--rw-r--r--   0 simon      (501) staff       (20)   189004 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.60.7/simba/assets/shap/UbuntuMono-Regular.ttf
--rw-r--r--   0 simon      (501) staff       (20)     2737 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.60.7/simba/assets/shap/side_scale_5.jpg
--rw-r--r--   0 simon      (501) staff       (20)     1785 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.60.7/simba/assets/shap/intruder_movement.jpg
--rw-r--r--   0 simon      (501) staff       (20)     1435 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.60.7/simba/assets/shap/resident_movement.jpg
--rw-r--r--   0 simon      (501) staff       (20)     3134 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.60.7/simba/assets/shap/color_bar.jpg
--rw-r--r--   0 simon      (501) staff       (20)     2120 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.60.7/simba/assets/shap/resident_intruder_movement.jpg
--rw-r--r--   0 simon      (501) staff       (20)    16388 2023-05-15 20:24:40.000000 Simba-UW-tf-dev-1.60.7/simba/assets/.DS_Store
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-23 16:26:58.000000 Simba-UW-tf-dev-1.60.7/simba/assets/lookups/
--rw-r--r--   0 simon      (501) staff       (20)     6148 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.60.7/simba/assets/lookups/.DS_Store
--rw-r--r--   0 simon      (501) staff       (20)   270783 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.60.7/simba/assets/lookups/model_names.parquet
--rw-r--r--   0 simon      (501) staff       (20)     2987 2023-04-25 20:39:03.000000 Simba-UW-tf-dev-1.60.7/simba/assets/lookups/feature_extraction_headers.csv
--rw-r--r--   0 simon      (501) staff       (20)    14175 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.60.7/simba/assets/lookups/features.csv
--rw-r--r--   0 simon      (501) staff       (20)    14175 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.60.7/simba/assets/lookups/unsupervised_example_x.csv
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-23 16:26:58.000000 Simba-UW-tf-dev-1.60.7/simba/assets/stl/
--rw-r--r--   0 simon      (501) staff       (20)   551576 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.60.7/simba/assets/stl/operant_tray.stl
--rw-r--r--   0 simon      (501) staff       (20)    67647 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.60.7/simba/assets/stl/operant_lever.stl
--rw-r--r--   0 simon      (501) staff       (20)    92896 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.60.7/simba/assets/stl/operant_walls.stl
--rw-r--r--   0 simon      (501) staff       (20)  4759984 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.60.7/simba/assets/stl/grid_floor.stl
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-23 16:26:58.000000 Simba-UW-tf-dev-1.60.7/simba/assets/img/
--rw-r--r--   0 simon      (501) staff       (20)     6148 2023-04-10 23:20:37.000000 Simba-UW-tf-dev-1.60.7/simba/assets/img/.DS_Store
--rw-r--r--   0 simon      (501) staff       (20)   399272 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.60.7/simba/assets/img/about_me.png
--rw-r--r--   0 simon      (501) staff       (20)   117108 2023-04-10 23:06:31.000000 Simba-UW-tf-dev-1.60.7/simba/assets/img/splash.mp4
--rw-r--r--   0 simon      (501) staff       (20)   322242 2023-04-06 16:38:51.000000 Simba-UW-tf-dev-1.60.7/simba/assets/img/bg_2.png
--rw-r--r--   0 simon      (501) staff       (20)    69267 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.60.7/simba/assets/img/splash.pptx
--rw-r--r--   0 simon      (501) staff       (20)   204362 2023-04-06 15:01:45.000000 Simba-UW-tf-dev-1.60.7/simba/assets/img/bg.png
--rw-r--r--   0 simon      (501) staff       (20)   189004 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.60.7/simba/assets/UbuntuMono-Regular.ttf
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-23 16:26:58.000000 Simba-UW-tf-dev-1.60.7/simba/assets/icons/
--rw-r--r--   0 simon      (501) staff       (20)     1350 2023-03-17 17:59:27.000000 Simba-UW-tf-dev-1.60.7/simba/assets/icons/factory.png
--rw-r--r--   0 simon      (501) staff       (20)     1413 2023-03-21 13:03:06.000000 Simba-UW-tf-dev-1.60.7/simba/assets/icons/cluster.png
--rw-r--r--   0 simon      (501) staff       (20)     1340 2023-03-17 16:51:08.000000 Simba-UW-tf-dev-1.60.7/simba/assets/icons/load.png
--rw-r--r--   0 simon      (501) staff       (20)     4507 2023-03-20 14:13:48.000000 Simba-UW-tf-dev-1.60.7/simba/assets/icons/gif.png
--rw-rw-r--   0 simon      (501) staff       (20)     4566 2023-03-18 18:12:27.000000 Simba-UW-tf-dev-1.60.7/simba/assets/icons/pose.png
--rw-rw-r--   0 simon      (501) staff       (20)     1943 2023-03-18 18:14:10.000000 Simba-UW-tf-dev-1.60.7/simba/assets/icons/features.png
--rw-r--r--   0 simon      (501) staff       (20)     6148 2023-04-05 17:25:36.000000 Simba-UW-tf-dev-1.60.7/simba/assets/icons/.DS_Store
--rw-rw-r--   0 simon      (501) staff       (20)     4896 2023-03-17 19:17:29.000000 Simba-UW-tf-dev-1.60.7/simba/assets/icons/settings.png
--rw-r--r--   0 simon      (501) staff       (20)     2090 2023-04-22 15:14:17.000000 Simba-UW-tf-dev-1.60.7/simba/assets/icons/stopwatch.png
--rw-r--r--   0 simon      (501) staff       (20)     1252 2023-03-19 16:48:40.000000 Simba-UW-tf-dev-1.60.7/simba/assets/icons/link.png
--rw-r--r--   0 simon      (501) staff       (20)    14250 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.60.7/simba/assets/icons/dash_simba.css
--rw-r--r--   0 simon      (501) staff       (20)      917 2023-04-05 16:43:13.000000 Simba-UW-tf-dev-1.60.7/simba/assets/icons/documentation.png
--rw-r--r--   0 simon      (501) staff       (20)     4503 2023-03-20 14:08:00.000000 Simba-UW-tf-dev-1.60.7/simba/assets/icons/fps.png
--rw-r--r--   0 simon      (501) staff       (20)     1299 2023-03-21 13:02:07.000000 Simba-UW-tf-dev-1.60.7/simba/assets/icons/dimensionality_reduction.png
--rw-rw-r--   0 simon      (501) staff       (20)     4823 2023-03-17 19:03:29.000000 Simba-UW-tf-dev-1.60.7/simba/assets/icons/roi.png
--rw-r--r--   0 simon      (501) staff       (20)      920 2023-03-20 14:25:03.000000 Simba-UW-tf-dev-1.60.7/simba/assets/icons/superimpose.png
--rw-r--r--   0 simon      (501) staff       (20)     1136 2023-03-18 20:25:31.000000 Simba-UW-tf-dev-1.60.7/simba/assets/icons/label.png
--rw-r--r--   0 simon      (501) staff       (20)     1016 2023-03-20 14:28:47.000000 Simba-UW-tf-dev-1.60.7/simba/assets/icons/change.png
--rw-r--r--   0 simon      (501) staff       (20)     1124 2023-03-17 18:05:26.000000 Simba-UW-tf-dev-1.60.7/simba/assets/icons/crop.png
--rw-r--r--   0 simon      (501) staff       (20)     2146 2023-04-13 14:09:23.000000 Simba-UW-tf-dev-1.60.7/simba/assets/icons/rotate.png
--rw-r--r--   0 simon      (501) staff       (20)     1057 2023-03-20 14:03:42.000000 Simba-UW-tf-dev-1.60.7/simba/assets/icons/path.png
--rw-r--r--   0 simon      (501) staff       (20)      950 2023-03-17 18:07:33.000000 Simba-UW-tf-dev-1.60.7/simba/assets/icons/clip.png
--rw-r--r--   0 simon      (501) staff       (20)     2121 2023-04-04 14:37:43.000000 Simba-UW-tf-dev-1.60.7/simba/assets/icons/restart.png
--rw-rw-r--   0 simon      (501) staff       (20)     4653 2023-03-17 18:11:59.000000 Simba-UW-tf-dev-1.60.7/simba/assets/icons/calipher.png
--rw-r--r--   0 simon      (501) staff       (20)     1291 2023-03-21 20:16:55.000000 Simba-UW-tf-dev-1.60.7/simba/assets/icons/add_on.png
--rw-rw-r--   0 simon      (501) staff       (20)     4695 2023-03-17 17:57:16.000000 Simba-UW-tf-dev-1.60.7/simba/assets/icons/create.png
--rw-r--r--   0 simon      (501) staff       (20)    78182 2023-03-20 16:35:36.000000 Simba-UW-tf-dev-1.60.7/simba/assets/icons/SimBA_logo.ico
--rw-r--r--   0 simon      (501) staff       (20)     1067 2023-03-20 14:22:44.000000 Simba-UW-tf-dev-1.60.7/simba/assets/icons/print.png
--rw-rw-r--   0 simon      (501) staff       (20)     4653 2023-03-18 20:27:58.000000 Simba-UW-tf-dev-1.60.7/simba/assets/icons/clf.png
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-23 16:26:58.000000 Simba-UW-tf-dev-1.60.7/simba/assets/icons/concat_icons/
--rw-r--r--   0 simon      (501) staff       (20)     6027 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.60.7/simba/assets/icons/concat_icons/mosaic.png
--rw-r--r--   0 simon      (501) staff       (20)     5654 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.60.7/simba/assets/icons/concat_icons/vertical.png
--rw-r--r--   0 simon      (501) staff       (20)     5542 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.60.7/simba/assets/icons/concat_icons/horizontal.png
--rw-r--r--   0 simon      (501) staff       (20)     5939 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.60.7/simba/assets/icons/concat_icons/mixed_mosaic.png
--rw-r--r--   0 simon      (501) staff       (20)     2060 2023-03-20 14:26:12.000000 Simba-UW-tf-dev-1.60.7/simba/assets/icons/merge.png
--rw-r--r--   0 simon      (501) staff       (20)     1252 2023-04-07 11:25:59.000000 Simba-UW-tf-dev-1.60.7/simba/assets/icons/clean.png
--rw-------   0 simon      (501) staff       (20)     4725 2023-03-18 20:27:47.000000 Simba-UW-tf-dev-1.60.7/simba/assets/icons/clf_2.png
--rw-rw-r--   0 simon      (501) staff       (20)     4795 2023-03-17 18:10:10.000000 Simba-UW-tf-dev-1.60.7/simba/assets/icons/visualize.png
--rw-r--r--   0 simon      (501) staff       (20)     2142 2023-03-20 14:10:28.000000 Simba-UW-tf-dev-1.60.7/simba/assets/icons/concat.png
--rw-r--r--   0 simon      (501) staff       (20)     1474 2023-03-17 19:20:24.000000 Simba-UW-tf-dev-1.60.7/simba/assets/icons/boris.png
--rw-rw-r--   0 simon      (501) staff       (20)     4804 2023-03-19 16:43:01.000000 Simba-UW-tf-dev-1.60.7/simba/assets/icons/frames.png
--rw-r--r--   0 simon      (501) staff       (20)     2425 2023-03-19 16:44:55.000000 Simba-UW-tf-dev-1.60.7/simba/assets/icons/video.png
--rw-r--r--   0 simon      (501) staff       (20)     2089 2023-03-20 14:05:58.000000 Simba-UW-tf-dev-1.60.7/simba/assets/icons/sample.png
--rw-r--r--   0 simon      (501) staff       (20)     1471 2023-03-21 13:04:02.000000 Simba-UW-tf-dev-1.60.7/simba/assets/icons/metrics.png
--rw-r--r--   0 simon      (501) staff       (20)     4555 2023-03-20 14:21:02.000000 Simba-UW-tf-dev-1.60.7/simba/assets/icons/grey.png
--rw-r--r--   0 simon      (501) staff       (20)      930 2023-03-18 18:07:29.000000 Simba-UW-tf-dev-1.60.7/simba/assets/icons/exit.png
--rw-r--r--   0 simon      (501) staff       (20)     4751 2023-03-18 20:31:58.000000 Simba-UW-tf-dev-1.60.7/simba/assets/icons/outlier.png
--rw-r--r--   0 simon      (501) staff       (20)     4392 2023-03-20 14:16:15.000000 Simba-UW-tf-dev-1.60.7/simba/assets/icons/clahe.png
--rw-rw-r--   0 simon      (501) staff       (20)     4637 2023-03-17 19:03:55.000000 Simba-UW-tf-dev-1.60.7/simba/assets/icons/trash.png
--rw-r--r--   0 simon      (501) staff       (20)     1239 2023-03-19 16:51:21.000000 Simba-UW-tf-dev-1.60.7/simba/assets/icons/about.png
--rw-rw-r--   0 simon      (501) staff       (20)     4666 2023-03-17 18:01:21.000000 Simba-UW-tf-dev-1.60.7/simba/assets/icons/convert.png
--rw-r--r--   0 simon      (501) staff       (20)    93229 2023-03-20 16:01:42.000000 Simba-UW-tf-dev-1.60.7/simba/assets/icons/SimBA_logo.icns
--rw-r--r--   0 simon      (501) staff       (20)      991 2023-03-20 19:02:33.000000 Simba-UW-tf-dev-1.60.7/simba/assets/icons/reorganize.png
--rw-rw-r--   0 simon      (501) staff       (20)     4784 2023-03-17 18:50:35.000000 Simba-UW-tf-dev-1.60.7/simba/assets/icons/browse.png
--rw-r--r--   0 simon      (501) staff       (20)    30707 2023-03-20 16:33:38.000000 Simba-UW-tf-dev-1.60.7/simba/assets/icons/SimBA_logo.png
--rw-r--r--   0 simon      (501) staff       (20)     2293 2023-03-17 19:24:38.000000 Simba-UW-tf-dev-1.60.7/simba/assets/icons/ethovision.png
--rw-r--r--   0 simon      (501) staff       (20)     1018 2023-04-05 15:24:49.000000 Simba-UW-tf-dev-1.60.7/simba/assets/icons/close.png
--rw-r--r--   0 simon      (501) staff       (20)    13672 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.60.7/simba/assets/dash_simba_base.css
--rw-r--r--   0 simon      (501) staff       (20)    31812 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.60.7/simba/assets/TheGoldenLab.PNG
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-23 16:26:58.000000 Simba-UW-tf-dev-1.60.7/Simba_UW_tf_dev.egg-info/
--rw-rw-r--   0 simon      (501) staff       (20)      579 2023-05-23 16:26:58.000000 Simba-UW-tf-dev-1.60.7/Simba_UW_tf_dev.egg-info/PKG-INFO
--rw-rw-r--   0 simon      (501) staff       (20)    18405 2023-05-23 16:26:58.000000 Simba-UW-tf-dev-1.60.7/Simba_UW_tf_dev.egg-info/SOURCES.txt
--rw-rw-r--   0 simon      (501) staff       (20)       44 2023-05-23 16:26:58.000000 Simba-UW-tf-dev-1.60.7/Simba_UW_tf_dev.egg-info/entry_points.txt
--rw-rw-r--   0 simon      (501) staff       (20)      639 2023-05-23 16:26:58.000000 Simba-UW-tf-dev-1.60.7/Simba_UW_tf_dev.egg-info/requires.txt
--rw-rw-r--   0 simon      (501) staff       (20)       12 2023-05-23 16:26:58.000000 Simba-UW-tf-dev-1.60.7/Simba_UW_tf_dev.egg-info/top_level.txt
--rw-rw-r--   0 simon      (501) staff       (20)        1 2023-05-23 16:26:58.000000 Simba-UW-tf-dev-1.60.7/Simba_UW_tf_dev.egg-info/dependency_links.txt
--rw-rw-r--   0 simon      (501) staff       (20)     7652 2020-05-13 13:27:38.000000 Simba-UW-tf-dev-1.60.7/LICENSE.md
--rw-r--r--   0 simon      (501) staff       (20)       89 2023-05-20 17:55:56.000000 Simba-UW-tf-dev-1.60.7/pyproject.toml
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-23 16:26:59.000000 Simba-UW-tf-dev-1.60.7/tests/
--rw-r--r--   0 simon      (501) staff       (20)        0 2023-05-20 18:02:57.000000 Simba-UW-tf-dev-1.60.7/tests/__init__.py
--rw-r--r--   0 simon      (501) staff       (20)     1859 2023-05-21 16:40:19.000000 Simba-UW-tf-dev-1.60.7/tests/test_featurizers.py
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-23 16:26:59.000000 Simba-UW-tf-dev-1.60.7/tests/data/
--rw-r--r--   0 simon      (501) staff       (20)        0 2023-05-20 18:02:57.000000 Simba-UW-tf-dev-1.60.7/tests/data/__init__.py
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-23 16:26:59.000000 Simba-UW-tf-dev-1.60.7/tests/data/test_projects/
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-23 16:26:59.000000 Simba-UW-tf-dev-1.60.7/tests/data/test_projects/two_c57/
--rw-r--r--   0 simon      (501) staff       (20)        0 2023-05-20 18:02:57.000000 Simba-UW-tf-dev-1.60.7/tests/data/test_projects/two_c57/__init__.py
--rw-r--r--   0 simon      (501) staff       (20)        0 2023-05-20 18:02:57.000000 Simba-UW-tf-dev-1.60.7/tests/data/test_projects/__init__.py
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-23 16:26:59.000000 Simba-UW-tf-dev-1.60.7/tests/data/test_projects/mouse_open_field/
--rw-r--r--   0 simon      (501) staff       (20)        0 2023-05-20 18:02:57.000000 Simba-UW-tf-dev-1.60.7/tests/data/test_projects/mouse_open_field/__init__.py
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-23 16:26:59.000000 Simba-UW-tf-dev-1.60.7/tests/data/test_projects/zebrafish/
--rw-r--r--   0 simon      (501) staff       (20)        0 2023-05-20 18:02:57.000000 Simba-UW-tf-dev-1.60.7/tests/data/test_projects/zebrafish/__init__.py
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-23 16:26:59.000000 Simba-UW-tf-dev-1.60.7/tests/data/test_projects/zebrafish/feature_file/
--rw-rw-r--   0 simon      (501) staff       (20)        0 2020-08-11 16:11:18.000000 Simba-UW-tf-dev-1.60.7/tests/data/test_projects/zebrafish/feature_file/__init__.py
--rw-rw-r--   0 simon      (501) staff       (20)    14128 2022-04-11 08:07:36.000000 Simba-UW-tf-dev-1.60.7/tests/data/test_projects/zebrafish/feature_file/fish_feature_extraction_092221.py
--rw-r--r--   0 simon      (501) staff       (20)     3972 2023-05-21 18:23:01.000000 Simba-UW-tf-dev-1.60.7/tests/test_thirdparty_appenders.py
--rw-rw-r--   0 simon      (501) staff       (20)      136 2021-04-10 10:44:06.000000 Simba-UW-tf-dev-1.60.7/MANIFEST.in
--rw-rw-r--   0 simon      (501) staff       (20)     9598 2020-05-13 13:27:40.000000 Simba-UW-tf-dev-1.60.7/README.md
--rw-rw-r--   0 simon      (501) staff       (20)     1897 2023-05-23 16:25:27.000000 Simba-UW-tf-dev-1.60.7/setup.py
--rw-r--r--   0 simon      (501) staff       (20)       38 2023-05-23 16:26:59.000000 Simba-UW-tf-dev-1.60.7/setup.cfg
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-24 15:39:16.000000 Simba-UW-tf-dev-1.60.9/
+-rw-r--r--   0 simon      (501) staff       (20)      579 2023-05-24 15:39:16.000000 Simba-UW-tf-dev-1.60.9/PKG-INFO
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-24 15:39:15.000000 Simba-UW-tf-dev-1.60.9/simba/
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-24 15:39:15.000000 Simba-UW-tf-dev-1.60.9/simba/ui/
+-rw-r--r--   0 simon      (501) staff       (20)     8196 2023-05-23 17:02:30.000000 Simba-UW-tf-dev-1.60.9/simba/ui/.DS_Store
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-24 15:39:15.000000 Simba-UW-tf-dev-1.60.9/simba/ui/pop_ups/
+-rw-r--r--   0 simon      (501) staff       (20)     3463 2023-05-04 17:49:06.000000 Simba-UW-tf-dev-1.60.9/simba/ui/pop_ups/movement_analysis_time_bins_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)     1431 2023-04-29 18:36:18.000000 Simba-UW-tf-dev-1.60.9/simba/ui/pop_ups/csv_2_parquet_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)     2343 2023-05-17 20:47:45.000000 Simba-UW-tf-dev-1.60.9/simba/ui/pop_ups/quick_path_plot_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)     2332 2023-04-29 18:13:54.000000 Simba-UW-tf-dev-1.60.9/simba/ui/pop_ups/batch_preprocess_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)     8342 2023-05-14 15:52:16.000000 Simba-UW-tf-dev-1.60.9/simba/ui/pop_ups/heatmap_location_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)     9302 2023-05-04 15:16:51.000000 Simba-UW-tf-dev-1.60.9/simba/ui/pop_ups/clf_probability_plot_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)     6148 2023-05-23 15:42:32.000000 Simba-UW-tf-dev-1.60.9/simba/ui/pop_ups/.DS_Store
+-rw-r--r--   0 simon      (501) staff       (20)     3143 2023-05-03 16:24:11.000000 Simba-UW-tf-dev-1.60.9/simba/ui/pop_ups/movement_analysis_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)     3657 2023-04-29 19:37:54.000000 Simba-UW-tf-dev-1.60.9/simba/ui/pop_ups/set_machine_model_parameters_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)     9471 2023-05-14 16:01:44.000000 Simba-UW-tf-dev-1.60.9/simba/ui/pop_ups/clf_plot_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)    15950 2023-05-20 12:10:35.000000 Simba-UW-tf-dev-1.60.9/simba/ui/pop_ups/path_plot_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)     3024 2023-04-29 16:24:52.000000 Simba-UW-tf-dev-1.60.9/simba/ui/pop_ups/smoothing_interpolation_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)     4798 2023-04-29 18:54:24.000000 Simba-UW-tf-dev-1.60.9/simba/ui/pop_ups/visualize_pose_in_dir_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)     3551 2023-05-03 16:20:49.000000 Simba-UW-tf-dev-1.60.9/simba/ui/pop_ups/roi_analysis_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)     5873 2023-04-29 16:24:52.000000 Simba-UW-tf-dev-1.60.9/simba/ui/pop_ups/outlier_settings_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)     8296 2023-04-29 18:36:18.000000 Simba-UW-tf-dev-1.60.9/simba/ui/pop_ups/gantt_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)     5726 2023-05-01 12:04:35.000000 Simba-UW-tf-dev-1.60.9/simba/ui/pop_ups/clf_validation_plot_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)     7721 2023-05-24 15:18:33.000000 Simba-UW-tf-dev-1.60.9/simba/ui/pop_ups/severity_analysis_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)     2779 2023-04-29 18:36:18.000000 Simba-UW-tf-dev-1.60.9/simba/ui/pop_ups/fsttc_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)     4052 2023-05-13 17:09:38.000000 Simba-UW-tf-dev-1.60.9/simba/ui/pop_ups/kleinberg_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)        0 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.60.9/simba/ui/pop_ups/__init__.py
+-rw-r--r--   0 simon      (501) staff       (20)     7288 2023-04-29 15:00:50.000000 Simba-UW-tf-dev-1.60.9/simba/ui/pop_ups/directing_other_animals_plot_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)     5425 2023-05-14 16:11:59.000000 Simba-UW-tf-dev-1.60.9/simba/ui/pop_ups/pose_reorganizer_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)     2411 2023-05-03 16:35:10.000000 Simba-UW-tf-dev-1.60.9/simba/ui/pop_ups/append_roi_features_animals_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)     3251 2023-04-29 18:36:18.000000 Simba-UW-tf-dev-1.60.9/simba/ui/pop_ups/clf_by_timebins_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)     8673 2023-05-14 15:52:16.000000 Simba-UW-tf-dev-1.60.9/simba/ui/pop_ups/heatmap_clf_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)     7688 2023-04-29 15:00:50.000000 Simba-UW-tf-dev-1.60.9/simba/ui/pop_ups/data_plot_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)     7860 2023-05-14 16:01:44.000000 Simba-UW-tf-dev-1.60.9/simba/ui/pop_ups/roi_features_plot_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)     8363 2023-04-29 19:49:16.000000 Simba-UW-tf-dev-1.60.9/simba/ui/pop_ups/pup_retrieval_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)      579 2023-04-29 18:12:37.000000 Simba-UW-tf-dev-1.60.9/simba/ui/pop_ups/about_simba_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)     2544 2023-04-29 18:36:18.000000 Simba-UW-tf-dev-1.60.9/simba/ui/pop_ups/clf_descriptive_statistics_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)     6353 2023-05-24 15:31:12.000000 Simba-UW-tf-dev-1.60.9/simba/ui/pop_ups/roi_tracking_plot_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)     1468 2023-04-29 16:24:52.000000 Simba-UW-tf-dev-1.60.9/simba/ui/pop_ups/append_roi_features_bodypart_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)     5318 2023-04-29 19:01:32.000000 Simba-UW-tf-dev-1.60.9/simba/ui/pop_ups/clf_add_remove_print_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)    42478 2023-04-29 18:56:08.000000 Simba-UW-tf-dev-1.60.9/simba/ui/pop_ups/video_processing_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)     7535 2023-05-15 13:09:04.000000 Simba-UW-tf-dev-1.60.9/simba/ui/pop_ups/validation_plot_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)     5255 2023-05-04 18:22:44.000000 Simba-UW-tf-dev-1.60.9/simba/ui/pop_ups/clf_by_roi_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)     2840 2023-04-29 18:36:18.000000 Simba-UW-tf-dev-1.60.9/simba/ui/pop_ups/make_path_plot_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)     5406 2023-04-29 18:36:18.000000 Simba-UW-tf-dev-1.60.9/simba/ui/pop_ups/create_user_defined_pose_configuration_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)     1065 2023-04-29 16:24:52.000000 Simba-UW-tf-dev-1.60.9/simba/ui/pop_ups/archive_files_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)     4087 2023-05-14 16:11:59.000000 Simba-UW-tf-dev-1.60.9/simba/ui/pop_ups/pose_bp_drop_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)    10712 2023-04-29 15:00:50.000000 Simba-UW-tf-dev-1.60.9/simba/ui/pop_ups/distance_plot_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)     2567 2023-04-29 16:24:52.000000 Simba-UW-tf-dev-1.60.9/simba/ui/pop_ups/subset_feature_extractor_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)     3114 2023-04-29 18:36:18.000000 Simba-UW-tf-dev-1.60.9/simba/ui/pop_ups/third_party_annotator_appender_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)     3193 2023-05-04 18:50:54.000000 Simba-UW-tf-dev-1.60.9/simba/ui/pop_ups/roi_analysis_time_bins_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)    12869 2023-05-23 12:47:59.000000 Simba-UW-tf-dev-1.60.9/simba/ui/video_info_ui.py
+-rw-r--r--   0 simon      (501) staff       (20)     6019 2023-05-16 16:45:46.000000 Simba-UW-tf-dev-1.60.9/simba/ui/user_defined_pose_creator.py
+-rw-r--r--   0 simon      (501) staff       (20)        0 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.60.9/simba/ui/__init__.py
+-rw-r--r--   0 simon      (501) staff       (20)    12602 2023-05-15 17:45:06.000000 Simba-UW-tf-dev-1.60.9/simba/ui/create_project_ui.py
+-rw-r--r--   0 simon      (501) staff       (20)    10957 2023-05-04 14:03:25.000000 Simba-UW-tf-dev-1.60.9/simba/ui/tkinter_functions.py
+-rw-r--r--   0 simon      (501) staff       (20)    34040 2023-05-15 17:45:06.000000 Simba-UW-tf-dev-1.60.9/simba/ui/machine_model_settings_ui.py
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-24 15:39:15.000000 Simba-UW-tf-dev-1.60.9/simba/blob_storage/
+-rw-r--r--   0 simon      (501) staff       (20)     6148 2023-05-20 18:16:05.000000 Simba-UW-tf-dev-1.60.9/simba/blob_storage/.DS_Store
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-24 15:39:15.000000 Simba-UW-tf-dev-1.60.9/simba/labelling/
+-rw-r--r--   0 simon      (501) staff       (20)     6148 2023-05-09 13:50:26.000000 Simba-UW-tf-dev-1.60.9/simba/labelling/.DS_Store
+-rw-r--r--   0 simon      (501) staff       (20)        0 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.60.9/simba/labelling/__init__.py
+-rw-r--r--   0 simon      (501) staff       (20)    20743 2023-05-14 23:21:08.000000 Simba-UW-tf-dev-1.60.9/simba/labelling/labelling_interface.py
+-rw-r--r--   0 simon      (501) staff       (20)     3568 2023-05-19 11:18:49.000000 Simba-UW-tf-dev-1.60.9/simba/labelling/extract_labelled_frames.py
+-rw-r--r--   0 simon      (501) staff       (20)    26732 2023-05-24 15:19:10.000000 Simba-UW-tf-dev-1.60.9/simba/labelling/labelling_advanced_interface.py
+-rw-r--r--   0 simon      (501) staff       (20)     6629 2023-05-13 17:45:08.000000 Simba-UW-tf-dev-1.60.9/simba/labelling/play_annotation_video.py
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-24 15:39:16.000000 Simba-UW-tf-dev-1.60.9/simba/unsupervised/
+-rw-r--r--   0 simon      (501) staff       (20)    11877 2023-05-17 14:59:39.000000 Simba-UW-tf-dev-1.60.9/simba/unsupervised/dbcv_calculator.py
+-rw-r--r--   0 simon      (501) staff       (20)     3375 2023-05-02 18:14:28.000000 Simba-UW-tf-dev-1.60.9/simba/unsupervised/enums.py
+-rw-r--r--   0 simon      (501) staff       (20)     6148 2023-05-20 18:15:51.000000 Simba-UW-tf-dev-1.60.9/simba/unsupervised/.DS_Store
+-rw-r--r--   0 simon      (501) staff       (20)     8141 2023-05-17 15:03:51.000000 Simba-UW-tf-dev-1.60.9/simba/unsupervised/dataset_creator.py
+-rw-r--r--   0 simon      (501) staff       (20)     5636 2023-05-17 15:03:51.000000 Simba-UW-tf-dev-1.60.9/simba/unsupervised/grid_search_visualizers.py
+-rw-r--r--   0 simon      (501) staff       (20)     7310 2023-05-17 15:03:51.000000 Simba-UW-tf-dev-1.60.9/simba/unsupervised/data_extractor.py
+-rw-r--r--   0 simon      (501) staff       (20)     9848 2023-05-17 15:03:51.000000 Simba-UW-tf-dev-1.60.9/simba/unsupervised/ui.py
+-rw-r--r--   0 simon      (501) staff       (20)        0 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.60.9/simba/unsupervised/__init__.py
+-rw-r--r--   0 simon      (501) staff       (20)     9851 2023-05-17 15:03:51.000000 Simba-UW-tf-dev-1.60.9/simba/unsupervised/umap_embedder.py
+-rw-r--r--   0 simon      (501) staff       (20)    41323 2023-05-02 18:14:28.000000 Simba-UW-tf-dev-1.60.9/simba/unsupervised/pop_up_classes.py
+-rw-r--r--   0 simon      (501) staff       (20)     2931 2023-05-17 14:54:38.000000 Simba-UW-tf-dev-1.60.9/simba/unsupervised/bout_aggregator.py
+-rw-r--r--   0 simon      (501) staff       (20)    20846 2023-05-17 15:03:51.000000 Simba-UW-tf-dev-1.60.9/simba/unsupervised/cluster_statistics.py
+-rw-r--r--   0 simon      (501) staff       (20)     2188 2023-04-18 23:25:29.000000 Simba-UW-tf-dev-1.60.9/simba/unsupervised/data_map.yaml
+-rw-r--r--   0 simon      (501) staff       (20)    10288 2023-05-17 15:07:44.000000 Simba-UW-tf-dev-1.60.9/simba/unsupervised/hdbscan_clusterer.py
+-rw-r--r--   0 simon      (501) staff       (20)     3937 2023-04-28 19:59:05.000000 Simba-UW-tf-dev-1.60.9/simba/unsupervised/tsne.py
+-rw-r--r--   0 simon      (501) staff       (20)     6656 2023-05-17 15:03:51.000000 Simba-UW-tf-dev-1.60.9/simba/unsupervised/cluster_visualizer.py
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-24 15:39:15.000000 Simba-UW-tf-dev-1.60.9/simba/bounding_box_tools/
+-rw-r--r--   0 simon      (501) staff       (20)     6148 2023-05-20 18:16:05.000000 Simba-UW-tf-dev-1.60.9/simba/bounding_box_tools/.DS_Store
+-rw-r--r--   0 simon      (501) staff       (20)        0 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.60.9/simba/bounding_box_tools/__init__.py
+-rw-r--r--   0 simon      (501) staff       (20)     7031 2023-05-14 18:13:04.000000 Simba-UW-tf-dev-1.60.9/simba/bounding_box_tools/agg_boundary_stats.py
+-rw-r--r--   0 simon      (501) staff       (20)    23566 2023-05-14 18:29:41.000000 Simba-UW-tf-dev-1.60.9/simba/bounding_box_tools/boundary_menus.py
+-rw-r--r--   0 simon      (501) staff       (20)     8497 2023-05-14 18:22:39.000000 Simba-UW-tf-dev-1.60.9/simba/bounding_box_tools/boundary_statistics.py
+-rw-r--r--   0 simon      (501) staff       (20)     6376 2023-05-15 16:44:53.000000 Simba-UW-tf-dev-1.60.9/simba/bounding_box_tools/find_boundaries.py
+-rw-r--r--   0 simon      (501) staff       (20)    11381 2023-05-15 16:44:53.000000 Simba-UW-tf-dev-1.60.9/simba/bounding_box_tools/visualize_boundaries.py
+-rw-r--r--   0 simon      (501) staff       (20)    49156 2023-05-23 15:41:51.000000 Simba-UW-tf-dev-1.60.9/simba/.DS_Store
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-24 15:39:15.000000 Simba-UW-tf-dev-1.60.9/simba/feature_extractors/
+-rw-r--r--   0 simon      (501) staff       (20)    42512 2023-05-15 00:05:22.000000 Simba-UW-tf-dev-1.60.9/simba/feature_extractors/feature_extractor_14bp.py
+-rw-r--r--   0 simon      (501) staff       (20)    21482 2023-05-14 23:55:56.000000 Simba-UW-tf-dev-1.60.9/simba/feature_extractors/feature_extractor_7bp.py
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-24 15:39:15.000000 Simba-UW-tf-dev-1.60.9/simba/feature_extractors/misc/
+-rw-r--r--   0 simon      (501) staff       (20)     1685 2023-04-14 17:52:01.000000 Simba-UW-tf-dev-1.60.9/simba/feature_extractors/misc/doctests.py
+-rw-r--r--   0 simon      (501) staff       (20)    23850 2023-04-17 18:48:40.000000 Simba-UW-tf-dev-1.60.9/simba/feature_extractors/misc/fish_feature_extractor_2023_version_3.py
+-rw-r--r--   0 simon      (501) staff       (20)     2732 2023-04-04 19:46:36.000000 Simba-UW-tf-dev-1.60.9/simba/feature_extractors/misc/read_in_mp.py
+-rw-r--r--   0 simon      (501) staff       (20)     2460 2023-04-22 18:02:29.000000 Simba-UW-tf-dev-1.60.9/simba/feature_extractors/misc/peaks.py
+-rw-r--r--   0 simon      (501) staff       (20)    14141 2023-03-15 17:20:08.000000 Simba-UW-tf-dev-1.60.9/simba/feature_extractors/misc/fish_feature_extractor_2022.py
+-rw-r--r--   0 simon      (501) staff       (20)     2053 2023-04-04 03:00:41.000000 Simba-UW-tf-dev-1.60.9/simba/feature_extractors/misc/convex_hull_3_scratch_3.py
+-rw-r--r--   0 simon      (501) staff       (20)     5762 2023-04-04 01:54:33.000000 Simba-UW-tf-dev-1.60.9/simba/feature_extractors/misc/convex_hull_scratch_1.py
+-rw-r--r--   0 simon      (501) staff       (20)     6148 2023-03-14 19:36:02.000000 Simba-UW-tf-dev-1.60.9/simba/feature_extractors/misc/.DS_Store
+-rw-r--r--   0 simon      (501) staff       (20)    21398 2023-04-16 17:03:37.000000 Simba-UW-tf-dev-1.60.9/simba/feature_extractors/misc/fish_feature_extractor_2023_version_2.py
+-rw-r--r--   0 simon      (501) staff       (20)     7127 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.60.9/simba/feature_extractors/misc/egocentrical_aligner.py
+-rw-r--r--   0 simon      (501) staff       (20)     1213 2023-04-11 20:12:47.000000 Simba-UW-tf-dev-1.60.9/simba/feature_extractors/misc/count_values_in_range.py
+-rw-r--r--   0 simon      (501) staff       (20)     4708 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.60.9/simba/feature_extractors/misc/graph_creator.py
+-rw-r--r--   0 simon      (501) staff       (20)     3954 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.60.9/simba/feature_extractors/misc/termite_rois.csv
+-rw-r--r--   0 simon      (501) staff       (20)      732 2023-03-20 12:13:51.000000 Simba-UW-tf-dev-1.60.9/simba/feature_extractors/misc/mutual_exclusive.py
+-rw-r--r--   0 simon      (501) staff       (20)     2841 2023-04-14 15:16:23.000000 Simba-UW-tf-dev-1.60.9/simba/feature_extractors/misc/video_color.py
+-rw-r--r--   0 simon      (501) staff       (20)     1862 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.60.9/simba/feature_extractors/misc/graph_3d_plotter.py
+-rw-r--r--   0 simon      (501) staff       (20)     5232 2023-04-13 14:05:29.000000 Simba-UW-tf-dev-1.60.9/simba/feature_extractors/misc/video_rotator.py
+-rw-r--r--   0 simon      (501) staff       (20)     2692 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.60.9/simba/feature_extractors/misc/add_probability_cnt_features.py
+-rw-r--r--   0 simon      (501) staff       (20)     1619 2023-04-08 20:02:08.000000 Simba-UW-tf-dev-1.60.9/simba/feature_extractors/misc/make_splash.py
+-rw-r--r--   0 simon      (501) staff       (20)    30661 2023-05-19 20:46:44.000000 Simba-UW-tf-dev-1.60.9/simba/feature_extractors/misc/fish_feature_extractor_2023_version_5.py
+-rw-r--r--   0 simon      (501) staff       (20)     1658 2023-04-22 19:16:28.000000 Simba-UW-tf-dev-1.60.9/simba/feature_extractors/misc/time_stamp_calculator.py
+-rw-r--r--   0 simon      (501) staff       (20)     5232 2023-04-15 19:24:18.000000 Simba-UW-tf-dev-1.60.9/simba/feature_extractors/misc/video_rotator_mp.py
+-rw-r--r--   0 simon      (501) staff       (20)    30661 2023-05-19 20:44:29.000000 Simba-UW-tf-dev-1.60.9/simba/feature_extractors/misc/fish_feature_extractor_2023_version_4.py
+-rw-r--r--   0 simon      (501) staff       (20)     2058 2023-04-03 23:51:37.000000 Simba-UW-tf-dev-1.60.9/simba/feature_extractors/misc/convex_hull_scratch_2.py
+-rw-r--r--   0 simon      (501) staff       (20)    27995 2023-05-15 00:05:22.000000 Simba-UW-tf-dev-1.60.9/simba/feature_extractors/feature_extractor_8bps_2_animals.py
+-rw-r--r--   0 simon      (501) staff       (20)    10244 2023-05-19 20:03:28.000000 Simba-UW-tf-dev-1.60.9/simba/feature_extractors/.DS_Store
+-rw-r--r--   0 simon      (501) staff       (20)     3864 2023-05-19 19:41:40.000000 Simba-UW-tf-dev-1.60.9/simba/feature_extractors/perimeter_jit.py
+-rw-r--r--   0 simon      (501) staff       (20)    13579 2023-05-14 19:53:33.000000 Simba-UW-tf-dev-1.60.9/simba/feature_extractors/feature_subsets.py
+-rw-r--r--   0 simon      (501) staff       (20)        0 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.60.9/simba/feature_extractors/__init__.py
+-rw-r--r--   0 simon      (501) staff       (20)     8244 2023-05-21 16:28:49.000000 Simba-UW-tf-dev-1.60.9/simba/feature_extractors/feature_extractor_user_defined.py
+-rw-r--r--   0 simon      (501) staff       (20)    46461 2023-05-15 00:03:36.000000 Simba-UW-tf-dev-1.60.9/simba/feature_extractors/feature_extractor_16bp.py
+-rw-r--r--   0 simon      (501) staff       (20)    28259 2023-05-15 00:05:22.000000 Simba-UW-tf-dev-1.60.9/simba/feature_extractors/feature_extractor_9bp.py
+-rw-r--r--   0 simon      (501) staff       (20)    23976 2023-05-15 00:01:21.000000 Simba-UW-tf-dev-1.60.9/simba/feature_extractors/feature_extractor_8bp.py
+-rw-r--r--   0 simon      (501) staff       (20)    16880 2023-05-14 23:53:59.000000 Simba-UW-tf-dev-1.60.9/simba/feature_extractors/feature_extractor_4bp.py
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-24 15:39:15.000000 Simba-UW-tf-dev-1.60.9/simba/feature_extractors/.idea/
+-rw-r--r--   0 simon      (501) staff       (20)      617 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.60.9/simba/feature_extractors/.idea/features_scripts.iml
+-rw-r--r--   0 simon      (501) staff       (20)      138 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.60.9/simba/feature_extractors/.idea/encodings.xml
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-24 15:39:15.000000 Simba-UW-tf-dev-1.60.9/simba/feature_extractors/.idea/inspectionProfiles/
+-rw-r--r--   0 simon      (501) staff       (20)      822 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.60.9/simba/feature_extractors/.idea/inspectionProfiles/Project_Default.xml
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-24 15:39:15.000000 Simba-UW-tf-dev-1.60.9/simba/feature_extractors/.idea/libraries/
+-rw-r--r--   0 simon      (501) staff       (20)      128 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.60.9/simba/feature_extractors/.idea/libraries/R_User_Library.xml
+-rw-r--r--   0 simon      (501) staff       (20)      273 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.60.9/simba/feature_extractors/.idea/.gitignore
+-rw-r--r--   0 simon      (501) staff       (20)     8081 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.60.9/simba/feature_extractors/.idea/workspace.xml
+-rw-r--r--   0 simon      (501) staff       (20)      291 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.60.9/simba/feature_extractors/.idea/modules.xml
+-rw-r--r--   0 simon      (501) staff       (20)       23 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.60.9/simba/feature_extractors/.idea/.name
+-rw-r--r--   0 simon      (501) staff       (20)      294 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.60.9/simba/feature_extractors/.idea/misc.xml
+-rw-r--r--   0 simon      (501) staff       (20)    15434 2023-05-20 18:29:53.000000 Simba-UW-tf-dev-1.60.9/simba/requirements.txt
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-24 15:39:15.000000 Simba-UW-tf-dev-1.60.9/simba/mixins/
+-rw-r--r--   0 simon      (501) staff       (20)     6148 2023-03-15 17:26:03.000000 Simba-UW-tf-dev-1.60.9/simba/mixins/.DS_Store
+-rw-r--r--   0 simon      (501) staff       (20)    42134 2023-05-16 16:45:46.000000 Simba-UW-tf-dev-1.60.9/simba/mixins/pop_up_mixin.py
+-rw-r--r--   0 simon      (501) staff       (20)    30127 2023-05-23 12:26:01.000000 Simba-UW-tf-dev-1.60.9/simba/mixins/config_reader.py
+-rw-r--r--   0 simon      (501) staff       (20)        0 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.60.9/simba/mixins/__init__.py
+-rw-r--r--   0 simon      (501) staff       (20)    18616 2023-05-17 19:39:33.000000 Simba-UW-tf-dev-1.60.9/simba/mixins/pose_importer_mixin.py
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-24 15:39:15.000000 Simba-UW-tf-dev-1.60.9/simba/mixins/__pycache__/
+-rw-r--r--   0 simon      (501) staff       (20)     1223 2023-05-21 16:37:18.000000 Simba-UW-tf-dev-1.60.9/simba/mixins/__pycache__/feature_extraction_mixin.FeatureExtractionMixin.cdist-333.py36m.nbi
+-rw-r--r--   0 simon      (501) staff       (20)     1118 2023-05-21 00:18:56.000000 Simba-UW-tf-dev-1.60.9/simba/mixins/__pycache__/feature_extraction_mixin.FeatureExtractionMixin.angle3pt-84.py36m.nbi
+-rw-r--r--   0 simon      (501) staff       (20)    51809 2023-05-21 16:37:18.000000 Simba-UW-tf-dev-1.60.9/simba/mixins/__pycache__/feature_extraction_mixin.FeatureExtractionMixin.cdist-333.py36m.1.nbc
+-rw-r--r--   0 simon      (501) staff       (20)    14188 2023-05-21 00:18:56.000000 Simba-UW-tf-dev-1.60.9/simba/mixins/__pycache__/feature_extraction_mixin.FeatureExtractionMixin.angle3pt-84.py36m.1.nbc
+-rw-r--r--   0 simon      (501) staff       (20)    37100 2023-05-19 15:31:55.000000 Simba-UW-tf-dev-1.60.9/simba/mixins/feature_extraction_mixin.py
+-rw-r--r--   0 simon      (501) staff       (20)    61873 2023-05-19 21:14:46.000000 Simba-UW-tf-dev-1.60.9/simba/mixins/plotting_mixin.py
+-rw-r--r--   0 simon      (501) staff       (20)     6175 2023-05-02 18:14:28.000000 Simba-UW-tf-dev-1.60.9/simba/mixins/unsupervised_mixin.py
+-rw-r--r--   0 simon      (501) staff       (20)    60756 2023-05-18 20:03:49.000000 Simba-UW-tf-dev-1.60.9/simba/mixins/train_model_mixin.py
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-24 15:39:15.000000 Simba-UW-tf-dev-1.60.9/simba/third_party_label_appenders/
+-rw-r--r--   0 simon      (501) staff       (20)     6094 2023-05-21 17:39:19.000000 Simba-UW-tf-dev-1.60.9/simba/third_party_label_appenders/deepethogram_importer.py
+-rw-r--r--   0 simon      (501) staff       (20)    10623 2023-05-21 18:42:05.000000 Simba-UW-tf-dev-1.60.9/simba/third_party_label_appenders/BORIS_appender.py
+-rw-r--r--   0 simon      (501) staff       (20)     8998 2023-05-15 17:20:07.000000 Simba-UW-tf-dev-1.60.9/simba/third_party_label_appenders/observer_importer.py
+-rw-r--r--   0 simon      (501) staff       (20)    17954 2023-05-21 15:57:11.000000 Simba-UW-tf-dev-1.60.9/simba/third_party_label_appenders/tools.py
+-rw-r--r--   0 simon      (501) staff       (20)        0 2023-04-01 14:10:06.000000 Simba-UW-tf-dev-1.60.9/simba/third_party_label_appenders/__init__.py
+-rw-r--r--   0 simon      (501) staff       (20)    18214 2023-05-24 15:19:35.000000 Simba-UW-tf-dev-1.60.9/simba/third_party_label_appenders/third_party_appender.py
+-rw-r--r--   0 simon      (501) staff       (20)     8181 2023-05-21 17:19:25.000000 Simba-UW-tf-dev-1.60.9/simba/third_party_label_appenders/ethovision_import.py
+-rw-r--r--   0 simon      (501) staff       (20)     6988 2023-05-21 17:31:04.000000 Simba-UW-tf-dev-1.60.9/simba/third_party_label_appenders/BENTO_appender.py
+-rw-r--r--   0 simon      (501) staff       (20)     5239 2023-05-21 18:07:18.000000 Simba-UW-tf-dev-1.60.9/simba/third_party_label_appenders/solomon_importer.py
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-24 15:39:15.000000 Simba-UW-tf-dev-1.60.9/simba/cue_light_tools/
+-rw-r--r--   0 simon      (501) staff       (20)     6148 2023-05-20 18:06:55.000000 Simba-UW-tf-dev-1.60.9/simba/cue_light_tools/.DS_Store
+-rw-r--r--   0 simon      (501) staff       (20)     7652 2023-05-15 16:44:53.000000 Simba-UW-tf-dev-1.60.9/simba/cue_light_tools/cue_light_clf_statistics.py
+-rw-r--r--   0 simon      (501) staff       (20)    12207 2023-05-15 16:44:53.000000 Simba-UW-tf-dev-1.60.9/simba/cue_light_tools/cue_light_analyzer.py
+-rw-r--r--   0 simon      (501) staff       (20)    16690 2023-05-15 16:44:53.000000 Simba-UW-tf-dev-1.60.9/simba/cue_light_tools/cue_light_menues.py
+-rw-r--r--   0 simon      (501) staff       (20)        0 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.60.9/simba/cue_light_tools/__init__.py
+-rw-r--r--   0 simon      (501) staff       (20)     1879 2023-05-15 16:44:53.000000 Simba-UW-tf-dev-1.60.9/simba/cue_light_tools/cue_light_tools.py
+-rw-r--r--   0 simon      (501) staff       (20)    15212 2023-05-16 18:48:44.000000 Simba-UW-tf-dev-1.60.9/simba/cue_light_tools/cue_light_visualizer.py
+-rw-r--r--   0 simon      (501) staff       (20)    12650 2023-05-15 16:44:53.000000 Simba-UW-tf-dev-1.60.9/simba/cue_light_tools/cue_light_movement_statistics.py
+-rw-r--r--   0 simon      (501) staff       (20)        0 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.60.9/simba/__init__.py
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-24 15:39:16.000000 Simba-UW-tf-dev-1.60.9/simba/utils/
+-rw-r--r--   0 simon      (501) staff       (20)    11899 2023-05-15 12:44:10.000000 Simba-UW-tf-dev-1.60.9/simba/utils/config_creator.py
+-rw-r--r--   0 simon      (501) staff       (20)    20972 2023-05-08 18:03:19.000000 Simba-UW-tf-dev-1.60.9/simba/utils/enums.py
+-rw-r--r--   0 simon      (501) staff       (20)     8196 2023-05-20 18:15:51.000000 Simba-UW-tf-dev-1.60.9/simba/utils/.DS_Store
+-rw-r--r--   0 simon      (501) staff       (20)     7365 2023-04-27 20:23:35.000000 Simba-UW-tf-dev-1.60.9/simba/utils/warnings.py
+-rw-r--r--   0 simon      (501) staff       (20)     8800 2023-05-16 00:24:15.000000 Simba-UW-tf-dev-1.60.9/simba/utils/checks.py
+-rw-r--r--   0 simon      (501) staff       (20)        0 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.60.9/simba/utils/__init__.py
+-rw-r--r--   0 simon      (501) staff       (20)    41798 2023-05-24 15:36:33.000000 Simba-UW-tf-dev-1.60.9/simba/utils/read_write.py
+-rw-r--r--   0 simon      (501) staff       (20)     8240 2023-05-15 14:49:42.000000 Simba-UW-tf-dev-1.60.9/simba/utils/lookups.py
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-24 15:39:16.000000 Simba-UW-tf-dev-1.60.9/simba/utils/cli/
+-rw-r--r--   0 simon      (501) staff       (20)        0 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.60.9/simba/utils/cli/__init__.py
+-rw-r--r--   0 simon      (501) staff       (20)     3227 2023-05-15 15:41:04.000000 Simba-UW-tf-dev-1.60.9/simba/utils/cli/cli_tools.py
+-rw-r--r--   0 simon      (501) staff       (20)    14666 2023-04-28 19:59:06.000000 Simba-UW-tf-dev-1.60.9/simba/utils/errors.py
+-rw-r--r--   0 simon      (501) staff       (20)    17730 2023-05-24 15:37:54.000000 Simba-UW-tf-dev-1.60.9/simba/utils/data.py
+-rw-r--r--   0 simon      (501) staff       (20)     1615 2023-05-08 18:13:22.000000 Simba-UW-tf-dev-1.60.9/simba/utils/printing.py
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-24 15:39:15.000000 Simba-UW-tf-dev-1.60.9/simba/pose_processors/
+-rw-r--r--   0 simon      (501) staff       (20)     8256 2023-05-15 16:58:05.000000 Simba-UW-tf-dev-1.60.9/simba/pose_processors/reorganize_keypoint.py
+-rw-r--r--   0 simon      (501) staff       (20)     5167 2023-05-15 16:58:05.000000 Simba-UW-tf-dev-1.60.9/simba/pose_processors/remove_keypoints.py
+-rw-r--r--   0 simon      (501) staff       (20)        0 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.60.9/simba/pose_processors/__init__.py
+-rw-r--r--   0 simon      (501) staff       (20)     2656 2023-05-15 16:58:04.000000 Simba-UW-tf-dev-1.60.9/simba/pose_processors/pose_reset.py
+-rw-r--r--   0 simon      (501) staff       (20)     5614 2023-05-04 15:35:50.000000 Simba-UW-tf-dev-1.60.9/simba/pose_processors/reverse_pose.py
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-24 15:39:15.000000 Simba-UW-tf-dev-1.60.9/simba/plotting/
+-rw-r--r--   0 simon      (501) staff       (20)     9114 2023-05-15 17:45:06.000000 Simba-UW-tf-dev-1.60.9/simba/plotting/gantt_creator.py
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-24 15:39:15.000000 Simba-UW-tf-dev-1.60.9/simba/plotting/tools/
+-rw-r--r--   0 simon      (501) staff       (20)     5388 2023-04-27 20:23:35.000000 Simba-UW-tf-dev-1.60.9/simba/plotting/tools/tkinter_tools.py
+-rw-r--r--   0 simon      (501) staff       (20)    13008 2023-05-24 15:32:44.000000 Simba-UW-tf-dev-1.60.9/simba/plotting/ROI_plotter_mp.py
+-rw-r--r--   0 simon      (501) staff       (20)     6148 2023-04-25 23:35:57.000000 Simba-UW-tf-dev-1.60.9/simba/plotting/.DS_Store
+-rw-r--r--   0 simon      (501) staff       (20)    14568 2023-05-15 18:41:17.000000 Simba-UW-tf-dev-1.60.9/simba/plotting/shap_agg_stats_visualizer.py
+-rw-r--r--   0 simon      (501) staff       (20)    10105 2023-05-15 17:45:06.000000 Simba-UW-tf-dev-1.60.9/simba/plotting/gantt_creator_mp.py
+-rw-r--r--   0 simon      (501) staff       (20)    15730 2023-05-15 17:49:01.000000 Simba-UW-tf-dev-1.60.9/simba/plotting/heat_mapper_clf_mp.py
+-rw-r--r--   0 simon      (501) staff       (20)     8731 2023-05-15 18:13:11.000000 Simba-UW-tf-dev-1.60.9/simba/plotting/probability_plot_creator.py
+-rw-r--r--   0 simon      (501) staff       (20)    12484 2023-05-23 14:52:24.000000 Simba-UW-tf-dev-1.60.9/simba/plotting/plot_clf_results.py
+-rw-r--r--   0 simon      (501) staff       (20)    14056 2023-05-17 14:20:24.000000 Simba-UW-tf-dev-1.60.9/simba/plotting/plot_clf_results_mp.py
+-rw-r--r--   0 simon      (501) staff       (20)    16031 2023-05-15 18:13:11.000000 Simba-UW-tf-dev-1.60.9/simba/plotting/ROI_feature_visualizer.py
+-rw-r--r--   0 simon      (501) staff       (20)    12770 2023-05-15 18:08:47.000000 Simba-UW-tf-dev-1.60.9/simba/plotting/heat_mapper_location.py
+-rw-r--r--   0 simon      (501) staff       (20)    10100 2023-05-15 18:13:11.000000 Simba-UW-tf-dev-1.60.9/simba/plotting/probability_plot_creator_mp.py
+-rw-r--r--   0 simon      (501) staff       (20)        0 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.60.9/simba/plotting/__init__.py
+-rw-r--r--   0 simon      (501) staff       (20)     4881 2023-05-15 18:08:47.000000 Simba-UW-tf-dev-1.60.9/simba/plotting/interactive_probability_grapher.py
+-rw-r--r--   0 simon      (501) staff       (20)     5812 2023-05-15 18:08:47.000000 Simba-UW-tf-dev-1.60.9/simba/plotting/plot_pose_in_dir.py
+-rw-r--r--   0 simon      (501) staff       (20)    13770 2023-05-23 16:26:11.000000 Simba-UW-tf-dev-1.60.9/simba/plotting/single_run_model_validation_video.py
+-rw-r--r--   0 simon      (501) staff       (20)    12790 2023-05-16 16:20:20.000000 Simba-UW-tf-dev-1.60.9/simba/plotting/frame_mergerer_ffmpeg.py
+-rw-r--r--   0 simon      (501) staff       (20)     7915 2023-05-16 16:18:45.000000 Simba-UW-tf-dev-1.60.9/simba/plotting/Directing_animals_visualizer_mp.py
+-rw-r--r--   0 simon      (501) staff       (20)    11219 2023-05-17 12:58:17.000000 Simba-UW-tf-dev-1.60.9/simba/plotting/clf_validator.py
+-rw-r--r--   0 simon      (501) staff       (20)    15745 2023-05-20 12:16:06.000000 Simba-UW-tf-dev-1.60.9/simba/plotting/path_plotter_mp.py
+-rw-r--r--   0 simon      (501) staff       (20)    11203 2023-05-24 15:35:24.000000 Simba-UW-tf-dev-1.60.9/simba/plotting/ROI_feature_visualizer_mp.py
+-rw-r--r--   0 simon      (501) staff       (20)     8933 2023-05-16 16:18:45.000000 Simba-UW-tf-dev-1.60.9/simba/plotting/data_plotter.py
+-rw-r--r--   0 simon      (501) staff       (20)    13471 2023-05-20 12:15:46.000000 Simba-UW-tf-dev-1.60.9/simba/plotting/path_plotter.py
+-rw-r--r--   0 simon      (501) staff       (20)     6494 2023-05-17 20:55:17.000000 Simba-UW-tf-dev-1.60.9/simba/plotting/ez_lineplot.py
+-rw-r--r--   0 simon      (501) staff       (20)    11491 2023-05-15 17:45:06.000000 Simba-UW-tf-dev-1.60.9/simba/plotting/distance_plotter_mp.py
+-rw-r--r--   0 simon      (501) staff       (20)    15794 2023-05-17 13:58:48.000000 Simba-UW-tf-dev-1.60.9/simba/plotting/ROI_plotter.py
+-rw-r--r--   0 simon      (501) staff       (20)    13163 2023-05-16 16:42:03.000000 Simba-UW-tf-dev-1.60.9/simba/plotting/heat_mapper_clf.py
+-rw-r--r--   0 simon      (501) staff       (20)     9113 2023-05-14 23:44:34.000000 Simba-UW-tf-dev-1.60.9/simba/plotting/distance_plotter.py
+-rw-r--r--   0 simon      (501) staff       (20)     9274 2023-05-23 16:26:19.000000 Simba-UW-tf-dev-1.60.9/simba/plotting/single_run_model_validation_video_mp.py
+-rw-r--r--   0 simon      (501) staff       (20)     9926 2023-05-16 16:20:20.000000 Simba-UW-tf-dev-1.60.9/simba/plotting/Directing_animals_visualizer.py
+-rw-r--r--   0 simon      (501) staff       (20)    16320 2023-05-15 18:08:47.000000 Simba-UW-tf-dev-1.60.9/simba/plotting/heat_mapper_location_mp.py
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-24 15:39:15.000000 Simba-UW-tf-dev-1.60.9/simba/dash_app/
+-rw-r--r--   0 simon      (501) staff       (20)    49699 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.60.9/simba/dash_app/SimBA_dash_app.py
+-rw-r--r--   0 simon      (501) staff       (20)     5029 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.60.9/simba/dash_app/run_dash_tkinter.py
+-rw-r--r--   0 simon      (501) staff       (20)    24474 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.60.9/simba/dash_app/dash_app.py
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-24 15:39:15.000000 Simba-UW-tf-dev-1.60.9/simba/data_processors/
+-rw-r--r--   0 simon      (501) staff       (20)     6514 2023-05-24 15:15:38.000000 Simba-UW-tf-dev-1.60.9/simba/data_processors/agg_clf_calculator.py
+-rw-r--r--   0 simon      (501) staff       (20)    10782 2023-05-23 19:18:05.000000 Simba-UW-tf-dev-1.60.9/simba/data_processors/severity_bout_based_calculator.py
+-rw-r--r--   0 simon      (501) staff       (20)    16259 2023-05-19 18:26:50.000000 Simba-UW-tf-dev-1.60.9/simba/data_processors/interpolation_smoothing.py
+-rw-r--r--   0 simon      (501) staff       (20)     7828 2023-05-14 19:47:31.000000 Simba-UW-tf-dev-1.60.9/simba/data_processors/timebins_clf_calculator.py
+-rw-r--r--   0 simon      (501) staff       (20)    12938 2023-05-23 20:14:45.000000 Simba-UW-tf-dev-1.60.9/simba/data_processors/fsttc_calculator.py
+-rw-r--r--   0 simon      (501) staff       (20)        0 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.60.9/simba/data_processors/__init__.py
+-rw-r--r--   0 simon      (501) staff       (20)     6306 2023-05-13 17:09:38.000000 Simba-UW-tf-dev-1.60.9/simba/data_processors/interpolate_pose.py
+-rw-r--r--   0 simon      (501) staff       (20)     9646 2023-05-14 19:19:14.000000 Simba-UW-tf-dev-1.60.9/simba/data_processors/directing_other_animals_calculator.py
+-rw-r--r--   0 simon      (501) staff       (20)     8550 2023-05-14 19:47:31.000000 Simba-UW-tf-dev-1.60.9/simba/data_processors/timebins_movement_calculator.py
+-rw-r--r--   0 simon      (501) staff       (20)     4799 2023-05-17 17:23:16.000000 Simba-UW-tf-dev-1.60.9/simba/data_processors/severity_calculator.py
+-rw-r--r--   0 simon      (501) staff       (20)    16980 2023-05-14 19:47:31.000000 Simba-UW-tf-dev-1.60.9/simba/data_processors/pup_retrieval_calculator.py
+-rw-r--r--   0 simon      (501) staff       (20)     3143 2023-05-13 17:23:00.000000 Simba-UW-tf-dev-1.60.9/simba/data_processors/pybursts_calculator.py
+-rw-r--r--   0 simon      (501) staff       (20)    11410 2023-05-23 20:23:27.000000 Simba-UW-tf-dev-1.60.9/simba/data_processors/severity_frame_based_calculator.py
+-rw-r--r--   0 simon      (501) staff       (20)     9649 2023-05-18 13:48:41.000000 Simba-UW-tf-dev-1.60.9/simba/data_processors/kleinberg_calculator.py
+-rw-r--r--   0 simon      (501) staff       (20)     8129 2023-05-18 13:31:03.000000 Simba-UW-tf-dev-1.60.9/simba/data_processors/movement_calculator.py
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-24 15:39:15.000000 Simba-UW-tf-dev-1.60.9/simba/pose_configurations_archive/
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-24 15:39:15.000000 Simba-UW-tf-dev-1.60.9/simba/pose_configurations_archive/pose_configurations_archive_1/
+-rw-r--r--   0 simon      (501) staff       (20)    14340 2023-03-30 11:05:37.000000 Simba-UW-tf-dev-1.60.9/simba/pose_configurations_archive/pose_configurations_archive_1/.DS_Store
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-24 15:39:15.000000 Simba-UW-tf-dev-1.60.9/simba/pose_configurations_archive/pose_configurations_archive_1/bp_names/
+-rw-r--r--   0 simon      (501) staff       (20)     6148 2023-03-16 13:26:00.000000 Simba-UW-tf-dev-1.60.9/simba/pose_configurations_archive/pose_configurations_archive_1/bp_names/.DS_Store
+-rw-r--r--   0 simon      (501) staff       (20)     1334 2023-04-28 23:45:27.000000 Simba-UW-tf-dev-1.60.9/simba/pose_configurations_archive/pose_configurations_archive_1/bp_names/bp_names.csv
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-24 15:39:15.000000 Simba-UW-tf-dev-1.60.9/simba/pose_configurations_archive/pose_configurations_archive_1/no_animals/
+-rw-r--r--   0 simon      (501) staff       (20)       26 2023-04-28 23:45:27.000000 Simba-UW-tf-dev-1.60.9/simba/pose_configurations_archive/pose_configurations_archive_1/no_animals/no_animals.csv
+-rw-r--r--   0 simon      (501) staff       (20)     6148 2023-03-16 13:26:19.000000 Simba-UW-tf-dev-1.60.9/simba/pose_configurations_archive/pose_configurations_archive_1/no_animals/.DS_Store
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-24 15:39:15.000000 Simba-UW-tf-dev-1.60.9/simba/pose_configurations_archive/pose_configurations_archive_1/configuration_names/
+-rw-r--r--   0 simon      (501) staff       (20)     6148 2023-03-16 13:26:14.000000 Simba-UW-tf-dev-1.60.9/simba/pose_configurations_archive/pose_configurations_archive_1/configuration_names/.DS_Store
+-rw-r--r--   0 simon      (501) staff       (20)      282 2023-04-28 23:45:27.000000 Simba-UW-tf-dev-1.60.9/simba/pose_configurations_archive/pose_configurations_archive_1/configuration_names/pose_config_names.csv
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-24 15:39:15.000000 Simba-UW-tf-dev-1.60.9/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/
+-rw-r--r--   0 simon      (501) staff       (20)     8196 2023-03-30 10:45:10.000000 Simba-UW-tf-dev-1.60.9/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/.DS_Store
+-rw-r--r--   0 simon      (501) staff       (20)    39805 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.60.9/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/8.png
+-rw-r--r--   0 simon      (501) staff       (20)    62501 2023-03-30 10:39:05.000000 Simba-UW-tf-dev-1.60.9/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/9.png
+-rw-r--r--   0 simon      (501) staff       (20)     6172 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.60.9/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/12.png
+-rw-r--r--   0 simon      (501) staff       (20)    11376 2023-04-28 23:45:27.000000 Simba-UW-tf-dev-1.60.9/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/13.png
+-rw-r--r--   0 simon      (501) staff       (20)    69501 2023-03-30 10:44:04.000000 Simba-UW-tf-dev-1.60.9/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/11.png
+-rw-r--r--   0 simon      (501) staff       (20)    69410 2023-03-30 10:40:01.000000 Simba-UW-tf-dev-1.60.9/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/10.png
+-rw-r--r--   0 simon      (501) staff       (20)    16000 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.60.9/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/4.png
+-rw-r--r--   0 simon      (501) staff       (20)    28150 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.60.9/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/5.png
+-rw-r--r--   0 simon      (501) staff       (20)    31140 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.60.9/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/7.png
+-rw-r--r--   0 simon      (501) staff       (20)    30634 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.60.9/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/6.png
+-rw-r--r--   0 simon      (501) staff       (20)    15417 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.60.9/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/2.png
+-rw-r--r--   0 simon      (501) staff       (20)    15786 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.60.9/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/3.png
+-rw-r--r--   0 simon      (501) staff       (20)    18939 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.60.9/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/1.png
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-24 15:39:15.000000 Simba-UW-tf-dev-1.60.9/simba/model/
+-rw-r--r--   0 simon      (501) staff       (20)    19026 2023-05-19 11:15:45.000000 Simba-UW-tf-dev-1.60.9/simba/model/train_rf.py
+-rw-r--r--   0 simon      (501) staff       (20)     6148 2023-05-20 18:06:50.000000 Simba-UW-tf-dev-1.60.9/simba/model/.DS_Store
+-rw-r--r--   0 simon      (501) staff       (20)     3315 2023-05-18 22:48:36.000000 Simba-UW-tf-dev-1.60.9/simba/model/inference_batch.py
+-rw-r--r--   0 simon      (501) staff       (20)    18876 2023-05-18 22:48:36.000000 Simba-UW-tf-dev-1.60.9/simba/model/grid_search_rf.py
+-rw-r--r--   0 simon      (501) staff       (20)     3363 2023-05-19 11:12:45.000000 Simba-UW-tf-dev-1.60.9/simba/model/inference_validation.py
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-24 15:39:15.000000 Simba-UW-tf-dev-1.60.9/simba/roi_tools/
+-rw-r--r--   0 simon      (501) staff       (20)     5858 2023-05-15 17:20:07.000000 Simba-UW-tf-dev-1.60.9/simba/roi_tools/ROI_time_bin_calculator.py
+-rw-r--r--   0 simon      (501) staff       (20)     1687 2023-05-15 17:20:07.000000 Simba-UW-tf-dev-1.60.9/simba/roi_tools/ROI_movement_analyzer.py
+-rw-r--r--   0 simon      (501) staff       (20)     6148 2023-03-20 12:47:56.000000 Simba-UW-tf-dev-1.60.9/simba/roi_tools/.DS_Store
+-rw-r--r--   0 simon      (501) staff       (20)    43119 2023-05-14 16:11:59.000000 Simba-UW-tf-dev-1.60.9/simba/roi_tools/ROI_define.py
+-rw-r--r--   0 simon      (501) staff       (20)     4024 2023-05-16 13:21:43.000000 Simba-UW-tf-dev-1.60.9/simba/roi_tools/ROI_reset.py
+-rw-r--r--   0 simon      (501) staff       (20)        0 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.60.9/simba/roi_tools/__init__.py
+-rw-r--r--   0 simon      (501) staff       (20)    19901 2023-05-15 17:00:34.000000 Simba-UW-tf-dev-1.60.9/simba/roi_tools/ROI_analyzer.py
+-rw-r--r--   0 simon      (501) staff       (20)    11608 2023-05-15 17:12:32.000000 Simba-UW-tf-dev-1.60.9/simba/roi_tools/ROI_feature_analyzer.py
+-rw-r--r--   0 simon      (501) staff       (20)     3654 2023-04-29 19:01:32.000000 Simba-UW-tf-dev-1.60.9/simba/roi_tools/ROI_multiply.py
+-rw-r--r--   0 simon      (501) staff       (20)      959 2023-05-15 17:20:07.000000 Simba-UW-tf-dev-1.60.9/simba/roi_tools/ROI_size_calculations.py
+-rw-r--r--   0 simon      (501) staff       (20)     3505 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.60.9/simba/roi_tools/ROI_zoom.py
+-rw-r--r--   0 simon      (501) staff       (20)    11556 2023-05-15 17:12:32.000000 Simba-UW-tf-dev-1.60.9/simba/roi_tools/ROI_directing_analyzer.py
+-rw-r--r--   0 simon      (501) staff       (20)    10128 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.60.9/simba/roi_tools/ROI_move_shape.py
+-rw-r--r--   0 simon      (501) staff       (20)     5079 2023-04-29 19:01:32.000000 Simba-UW-tf-dev-1.60.9/simba/roi_tools/ROI_menus.py
+-rw-r--r--   0 simon      (501) staff       (20)    13742 2023-05-15 17:12:32.000000 Simba-UW-tf-dev-1.60.9/simba/roi_tools/ROI_clf_calculator.py
+-rw-r--r--   0 simon      (501) staff       (20)    22688 2023-04-29 19:01:32.000000 Simba-UW-tf-dev-1.60.9/simba/roi_tools/ROI_image.py
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-24 15:39:15.000000 Simba-UW-tf-dev-1.60.9/simba/pose_importers/
+-rw-r--r--   0 simon      (501) staff       (20)     8115 2023-05-14 18:03:14.000000 Simba-UW-tf-dev-1.60.9/simba/pose_importers/sleap_csv_importer.py
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-24 15:39:15.000000 Simba-UW-tf-dev-1.60.9/simba/pose_importers/misc/
+-rw-r--r--   0 simon      (501) staff       (20)     6148 2023-05-09 17:42:38.000000 Simba-UW-tf-dev-1.60.9/simba/pose_importers/misc/.DS_Store
+-rw-r--r--   0 simon      (501) staff       (20)     7943 2023-05-01 19:07:14.000000 Simba-UW-tf-dev-1.60.9/simba/pose_importers/misc/apt_trk_importer.py
+-rw-r--r--   0 simon      (501) staff       (20)     2464 2023-04-27 19:42:17.000000 Simba-UW-tf-dev-1.60.9/simba/pose_importers/read_DANNCE_mat.py
+-rw-r--r--   0 simon      (501) staff       (20)     6148 2023-05-09 17:45:51.000000 Simba-UW-tf-dev-1.60.9/simba/pose_importers/.DS_Store
+-rw-r--r--   0 simon      (501) staff       (20)    12549 2023-05-17 20:32:56.000000 Simba-UW-tf-dev-1.60.9/simba/pose_importers/sleap_h5_importer.py
+-rw-r--r--   0 simon      (501) staff       (20)     7322 2023-05-16 16:55:05.000000 Simba-UW-tf-dev-1.60.9/simba/pose_importers/madlc_importer.py
+-rw-r--r--   0 simon      (501) staff       (20)        0 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.60.9/simba/pose_importers/__init__.py
+-rw-r--r--   0 simon      (501) staff       (20)    12141 2023-05-16 18:48:44.000000 Simba-UW-tf-dev-1.60.9/simba/pose_importers/sleap_slp_importer.py
+-rw-r--r--   0 simon      (501) staff       (20)     7931 2023-05-15 16:58:04.000000 Simba-UW-tf-dev-1.60.9/simba/pose_importers/import_mars.py
+-rw-r--r--   0 simon      (501) staff       (20)     6978 2023-05-15 16:44:53.000000 Simba-UW-tf-dev-1.60.9/simba/pose_importers/dlc_importer_csv.py
+-rw-r--r--   0 simon      (501) staff       (20)     8060 2023-04-28 19:20:42.000000 Simba-UW-tf-dev-1.60.9/simba/pose_importers/trk_importer.py
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-24 15:39:15.000000 Simba-UW-tf-dev-1.60.9/simba/pose_configurations/
+-rw-r--r--   0 simon      (501) staff       (20)    14340 2023-05-14 23:57:00.000000 Simba-UW-tf-dev-1.60.9/simba/pose_configurations/.DS_Store
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-24 15:39:15.000000 Simba-UW-tf-dev-1.60.9/simba/pose_configurations/bp_names/
+-rw-r--r--   0 simon      (501) staff       (20)     6148 2023-03-16 13:26:00.000000 Simba-UW-tf-dev-1.60.9/simba/pose_configurations/bp_names/.DS_Store
+-rw-r--r--   0 simon      (501) staff       (20)     1316 2023-04-29 18:20:02.000000 Simba-UW-tf-dev-1.60.9/simba/pose_configurations/bp_names/bp_names.csv
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-24 15:39:15.000000 Simba-UW-tf-dev-1.60.9/simba/pose_configurations/no_animals/
+-rw-r--r--   0 simon      (501) staff       (20)       24 2023-04-29 18:20:02.000000 Simba-UW-tf-dev-1.60.9/simba/pose_configurations/no_animals/no_animals.csv
+-rw-r--r--   0 simon      (501) staff       (20)     6148 2023-03-16 13:26:19.000000 Simba-UW-tf-dev-1.60.9/simba/pose_configurations/no_animals/.DS_Store
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-24 15:39:15.000000 Simba-UW-tf-dev-1.60.9/simba/pose_configurations/configuration_names/
+-rw-r--r--   0 simon      (501) staff       (20)     6148 2023-03-16 13:26:14.000000 Simba-UW-tf-dev-1.60.9/simba/pose_configurations/configuration_names/.DS_Store
+-rw-r--r--   0 simon      (501) staff       (20)      267 2023-04-29 18:20:02.000000 Simba-UW-tf-dev-1.60.9/simba/pose_configurations/configuration_names/pose_config_names.csv
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-24 15:39:15.000000 Simba-UW-tf-dev-1.60.9/simba/pose_configurations/schematics/
+-rw-r--r--   0 simon      (501) staff       (20)    39805 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.60.9/simba/pose_configurations/schematics/8.png
+-rw-r--r--   0 simon      (501) staff       (20)    62501 2023-03-30 10:39:05.000000 Simba-UW-tf-dev-1.60.9/simba/pose_configurations/schematics/9.png
+-rw-r--r--   0 simon      (501) staff       (20)     6172 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.60.9/simba/pose_configurations/schematics/12.png
+-rw-r--r--   0 simon      (501) staff       (20)    69501 2023-03-30 10:44:04.000000 Simba-UW-tf-dev-1.60.9/simba/pose_configurations/schematics/11.png
+-rw-r--r--   0 simon      (501) staff       (20)    69410 2023-03-30 10:40:01.000000 Simba-UW-tf-dev-1.60.9/simba/pose_configurations/schematics/10.png
+-rw-r--r--   0 simon      (501) staff       (20)    16000 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.60.9/simba/pose_configurations/schematics/4.png
+-rw-r--r--   0 simon      (501) staff       (20)    28150 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.60.9/simba/pose_configurations/schematics/5.png
+-rw-r--r--   0 simon      (501) staff       (20)    31140 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.60.9/simba/pose_configurations/schematics/7.png
+-rw-r--r--   0 simon      (501) staff       (20)    30634 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.60.9/simba/pose_configurations/schematics/6.png
+-rw-r--r--   0 simon      (501) staff       (20)    15417 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.60.9/simba/pose_configurations/schematics/2.png
+-rw-r--r--   0 simon      (501) staff       (20)    15786 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.60.9/simba/pose_configurations/schematics/3.png
+-rw-r--r--   0 simon      (501) staff       (20)    18939 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.60.9/simba/pose_configurations/schematics/1.png
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-24 15:39:16.000000 Simba-UW-tf-dev-1.60.9/simba/video_processors/
+-rw-r--r--   0 simon      (501) staff       (20)    45564 2023-05-14 17:15:40.000000 Simba-UW-tf-dev-1.60.9/simba/video_processors/video_processing.py
+-rw-r--r--   0 simon      (501) staff       (20)     8196 2023-05-20 18:15:51.000000 Simba-UW-tf-dev-1.60.9/simba/video_processors/.DS_Store
+-rw-r--r--   0 simon      (501) staff       (20)     7171 2023-04-27 19:42:17.000000 Simba-UW-tf-dev-1.60.9/simba/video_processors/px_to_mm.py
+-rw-r--r--   0 simon      (501) staff       (20)    24648 2023-05-16 16:42:04.000000 Simba-UW-tf-dev-1.60.9/simba/video_processors/batch_process_menus.py
+-rw-r--r--   0 simon      (501) staff       (20)     7333 2023-05-16 12:54:28.000000 Simba-UW-tf-dev-1.60.9/simba/video_processors/multi_cropper.py
+-rw-r--r--   0 simon      (501) staff       (20)     2833 2023-04-27 20:23:35.000000 Simba-UW-tf-dev-1.60.9/simba/video_processors/extract_frames.py
+-rw-r--r--   0 simon      (501) staff       (20)        0 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.60.9/simba/video_processors/__init__.py
+-rw-r--r--   0 simon      (501) staff       (20)     8266 2023-05-08 18:19:00.000000 Simba-UW-tf-dev-1.60.9/simba/video_processors/calculate_px_dist.py
+-rw-r--r--   0 simon      (501) staff       (20)     4695 2023-04-26 18:17:53.000000 Simba-UW-tf-dev-1.60.9/simba/video_processors/extract_seqframes.py
+-rw-r--r--   0 simon      (501) staff       (20)    11087 2023-05-14 16:24:59.000000 Simba-UW-tf-dev-1.60.9/simba/video_processors/batch_process_create_ffmpeg_commands.py
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-24 15:39:15.000000 Simba-UW-tf-dev-1.60.9/simba/outlier_tools/
+-rw-r--r--   0 simon      (501) staff       (20)     6525 2023-05-19 17:31:41.000000 Simba-UW-tf-dev-1.60.9/simba/outlier_tools/outlier_corrector_movement.py
+-rw-r--r--   0 simon      (501) staff       (20)     6148 2023-05-08 20:25:20.000000 Simba-UW-tf-dev-1.60.9/simba/outlier_tools/.DS_Store
+-rw-r--r--   0 simon      (501) staff       (20)        0 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.60.9/simba/outlier_tools/__init__.py
+-rw-r--r--   0 simon      (501) staff       (20)     8160 2023-05-19 18:34:50.000000 Simba-UW-tf-dev-1.60.9/simba/outlier_tools/outlier_corrector_location.py
+-rw-r--r--   0 simon      (501) staff       (20)     2696 2023-05-23 12:33:12.000000 Simba-UW-tf-dev-1.60.9/simba/outlier_tools/skip_outlier_correction.py
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-24 15:39:15.000000 Simba-UW-tf-dev-1.60.9/simba/outlier_tools/.idea/
+-rw-r--r--   0 simon      (501) staff       (20)      617 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.60.9/simba/outlier_tools/.idea/outlier_scripts.iml
+-rw-r--r--   0 simon      (501) staff       (20)      138 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.60.9/simba/outlier_tools/.idea/encodings.xml
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-24 15:39:15.000000 Simba-UW-tf-dev-1.60.9/simba/outlier_tools/.idea/inspectionProfiles/
+-rw-r--r--   0 simon      (501) staff       (20)      668 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.60.9/simba/outlier_tools/.idea/inspectionProfiles/Project_Default.xml
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-24 15:39:15.000000 Simba-UW-tf-dev-1.60.9/simba/outlier_tools/.idea/libraries/
+-rw-r--r--   0 simon      (501) staff       (20)      128 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.60.9/simba/outlier_tools/.idea/libraries/R_User_Library.xml
+-rw-r--r--   0 simon      (501) staff       (20)     8102 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.60.9/simba/outlier_tools/.idea/workspace.xml
+-rw-r--r--   0 simon      (501) staff       (20)      289 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.60.9/simba/outlier_tools/.idea/modules.xml
+-rw-r--r--   0 simon      (501) staff       (20)      294 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.60.9/simba/outlier_tools/.idea/misc.xml
+-rw-r--r--   0 simon      (501) staff       (20)    64855 2023-05-21 18:08:05.000000 Simba-UW-tf-dev-1.60.9/simba/SimBA.py
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-24 15:39:15.000000 Simba-UW-tf-dev-1.60.9/simba/assets/
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-24 15:39:15.000000 Simba-UW-tf-dev-1.60.9/simba/assets/unsupervised/
+-rw-r--r--   0 simon      (501) staff       (20)     6148 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.60.9/simba/assets/unsupervised/.DS_Store
+-rw-r--r--   0 simon      (501) staff       (20)   109483 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.60.9/simba/assets/unsupervised/model_names.parquet
+-rw-r--r--   0 simon      (501) staff       (20)    14175 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.60.9/simba/assets/unsupervised/features.csv
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-24 15:39:15.000000 Simba-UW-tf-dev-1.60.9/simba/assets/shap/
+-rw-r--r--   0 simon      (501) staff       (20)     1177 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.60.9/simba/assets/shap/down_arrow.jpg
+-rw-r--r--   0 simon      (501) staff       (20)     1733 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.60.9/simba/assets/shap/intruder_shape.jpg
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-24 15:39:15.000000 Simba-UW-tf-dev-1.60.9/simba/assets/shap/feature_categories/
+-rw-r--r--   0 simon      (501) staff       (20)      109 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.60.9/simba/assets/shap/feature_categories/.~lock.shap_feature_categories.csv#
+-rw-r--r--   0 simon      (501) staff       (20)    17420 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.60.9/simba/assets/shap/feature_categories/shap_feature_categories.csv
+-rw-r--r--   0 simon      (501) staff       (20)     8196 2023-04-10 20:37:13.000000 Simba-UW-tf-dev-1.60.9/simba/assets/shap/.DS_Store
+-rw-r--r--   0 simon      (501) staff       (20)     1665 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.60.9/simba/assets/shap/resident_shape.jpg
+-rw-r--r--   0 simon      (501) staff       (20)     2415 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.60.9/simba/assets/shap/resident_intruder_shape.jpg
+-rw-r--r--   0 simon      (501) staff       (20)     2012 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.60.9/simba/assets/shap/animal_distances.jpg
+-rw-r--r--   0 simon      (501) staff       (20)     4422 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.60.9/simba/assets/shap/baseline_scale.jpg
+-rw-r--r--   0 simon      (501) staff       (20)   353824 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.60.9/simba/assets/shap/ubuntu.regular.ttf
+-rw-r--r--   0 simon      (501) staff       (20)     6672 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.60.9/simba/assets/shap/side_scale.jpg
+-rw-r--r--   0 simon      (501) staff       (20)   189004 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.60.9/simba/assets/shap/UbuntuMono-Regular.ttf
+-rw-r--r--   0 simon      (501) staff       (20)     2737 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.60.9/simba/assets/shap/side_scale_5.jpg
+-rw-r--r--   0 simon      (501) staff       (20)     1785 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.60.9/simba/assets/shap/intruder_movement.jpg
+-rw-r--r--   0 simon      (501) staff       (20)     1435 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.60.9/simba/assets/shap/resident_movement.jpg
+-rw-r--r--   0 simon      (501) staff       (20)     3134 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.60.9/simba/assets/shap/color_bar.jpg
+-rw-r--r--   0 simon      (501) staff       (20)     2120 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.60.9/simba/assets/shap/resident_intruder_movement.jpg
+-rw-r--r--   0 simon      (501) staff       (20)    16388 2023-05-15 20:24:40.000000 Simba-UW-tf-dev-1.60.9/simba/assets/.DS_Store
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-24 15:39:15.000000 Simba-UW-tf-dev-1.60.9/simba/assets/lookups/
+-rw-r--r--   0 simon      (501) staff       (20)     6148 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.60.9/simba/assets/lookups/.DS_Store
+-rw-r--r--   0 simon      (501) staff       (20)   270783 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.60.9/simba/assets/lookups/model_names.parquet
+-rw-r--r--   0 simon      (501) staff       (20)     2987 2023-04-25 20:39:03.000000 Simba-UW-tf-dev-1.60.9/simba/assets/lookups/feature_extraction_headers.csv
+-rw-r--r--   0 simon      (501) staff       (20)    14175 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.60.9/simba/assets/lookups/features.csv
+-rw-r--r--   0 simon      (501) staff       (20)    14175 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.60.9/simba/assets/lookups/unsupervised_example_x.csv
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-24 15:39:15.000000 Simba-UW-tf-dev-1.60.9/simba/assets/stl/
+-rw-r--r--   0 simon      (501) staff       (20)   551576 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.60.9/simba/assets/stl/operant_tray.stl
+-rw-r--r--   0 simon      (501) staff       (20)    67647 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.60.9/simba/assets/stl/operant_lever.stl
+-rw-r--r--   0 simon      (501) staff       (20)    92896 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.60.9/simba/assets/stl/operant_walls.stl
+-rw-r--r--   0 simon      (501) staff       (20)  4759984 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.60.9/simba/assets/stl/grid_floor.stl
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-24 15:39:15.000000 Simba-UW-tf-dev-1.60.9/simba/assets/img/
+-rw-r--r--   0 simon      (501) staff       (20)     6148 2023-04-10 23:20:37.000000 Simba-UW-tf-dev-1.60.9/simba/assets/img/.DS_Store
+-rw-r--r--   0 simon      (501) staff       (20)   399272 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.60.9/simba/assets/img/about_me.png
+-rw-r--r--   0 simon      (501) staff       (20)   117108 2023-04-10 23:06:31.000000 Simba-UW-tf-dev-1.60.9/simba/assets/img/splash.mp4
+-rw-r--r--   0 simon      (501) staff       (20)   322242 2023-04-06 16:38:51.000000 Simba-UW-tf-dev-1.60.9/simba/assets/img/bg_2.png
+-rw-r--r--   0 simon      (501) staff       (20)    69267 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.60.9/simba/assets/img/splash.pptx
+-rw-r--r--   0 simon      (501) staff       (20)   204362 2023-04-06 15:01:45.000000 Simba-UW-tf-dev-1.60.9/simba/assets/img/bg.png
+-rw-r--r--   0 simon      (501) staff       (20)   189004 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.60.9/simba/assets/UbuntuMono-Regular.ttf
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-24 15:39:15.000000 Simba-UW-tf-dev-1.60.9/simba/assets/icons/
+-rw-r--r--   0 simon      (501) staff       (20)     1350 2023-03-17 17:59:27.000000 Simba-UW-tf-dev-1.60.9/simba/assets/icons/factory.png
+-rw-r--r--   0 simon      (501) staff       (20)     1413 2023-03-21 13:03:06.000000 Simba-UW-tf-dev-1.60.9/simba/assets/icons/cluster.png
+-rw-r--r--   0 simon      (501) staff       (20)     1340 2023-03-17 16:51:08.000000 Simba-UW-tf-dev-1.60.9/simba/assets/icons/load.png
+-rw-r--r--   0 simon      (501) staff       (20)     4507 2023-03-20 14:13:48.000000 Simba-UW-tf-dev-1.60.9/simba/assets/icons/gif.png
+-rw-rw-r--   0 simon      (501) staff       (20)     4566 2023-03-18 18:12:27.000000 Simba-UW-tf-dev-1.60.9/simba/assets/icons/pose.png
+-rw-rw-r--   0 simon      (501) staff       (20)     1943 2023-03-18 18:14:10.000000 Simba-UW-tf-dev-1.60.9/simba/assets/icons/features.png
+-rw-r--r--   0 simon      (501) staff       (20)     6148 2023-04-05 17:25:36.000000 Simba-UW-tf-dev-1.60.9/simba/assets/icons/.DS_Store
+-rw-rw-r--   0 simon      (501) staff       (20)     4896 2023-03-17 19:17:29.000000 Simba-UW-tf-dev-1.60.9/simba/assets/icons/settings.png
+-rw-r--r--   0 simon      (501) staff       (20)     2090 2023-04-22 15:14:17.000000 Simba-UW-tf-dev-1.60.9/simba/assets/icons/stopwatch.png
+-rw-r--r--   0 simon      (501) staff       (20)     1252 2023-03-19 16:48:40.000000 Simba-UW-tf-dev-1.60.9/simba/assets/icons/link.png
+-rw-r--r--   0 simon      (501) staff       (20)    14250 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.60.9/simba/assets/icons/dash_simba.css
+-rw-r--r--   0 simon      (501) staff       (20)      917 2023-04-05 16:43:13.000000 Simba-UW-tf-dev-1.60.9/simba/assets/icons/documentation.png
+-rw-r--r--   0 simon      (501) staff       (20)     4503 2023-03-20 14:08:00.000000 Simba-UW-tf-dev-1.60.9/simba/assets/icons/fps.png
+-rw-r--r--   0 simon      (501) staff       (20)     1299 2023-03-21 13:02:07.000000 Simba-UW-tf-dev-1.60.9/simba/assets/icons/dimensionality_reduction.png
+-rw-rw-r--   0 simon      (501) staff       (20)     4823 2023-03-17 19:03:29.000000 Simba-UW-tf-dev-1.60.9/simba/assets/icons/roi.png
+-rw-r--r--   0 simon      (501) staff       (20)      920 2023-03-20 14:25:03.000000 Simba-UW-tf-dev-1.60.9/simba/assets/icons/superimpose.png
+-rw-r--r--   0 simon      (501) staff       (20)     1136 2023-03-18 20:25:31.000000 Simba-UW-tf-dev-1.60.9/simba/assets/icons/label.png
+-rw-r--r--   0 simon      (501) staff       (20)     1016 2023-03-20 14:28:47.000000 Simba-UW-tf-dev-1.60.9/simba/assets/icons/change.png
+-rw-r--r--   0 simon      (501) staff       (20)     1124 2023-03-17 18:05:26.000000 Simba-UW-tf-dev-1.60.9/simba/assets/icons/crop.png
+-rw-r--r--   0 simon      (501) staff       (20)     2146 2023-04-13 14:09:23.000000 Simba-UW-tf-dev-1.60.9/simba/assets/icons/rotate.png
+-rw-r--r--   0 simon      (501) staff       (20)     1057 2023-03-20 14:03:42.000000 Simba-UW-tf-dev-1.60.9/simba/assets/icons/path.png
+-rw-r--r--   0 simon      (501) staff       (20)      950 2023-03-17 18:07:33.000000 Simba-UW-tf-dev-1.60.9/simba/assets/icons/clip.png
+-rw-r--r--   0 simon      (501) staff       (20)     2121 2023-04-04 14:37:43.000000 Simba-UW-tf-dev-1.60.9/simba/assets/icons/restart.png
+-rw-rw-r--   0 simon      (501) staff       (20)     4653 2023-03-17 18:11:59.000000 Simba-UW-tf-dev-1.60.9/simba/assets/icons/calipher.png
+-rw-r--r--   0 simon      (501) staff       (20)     1291 2023-03-21 20:16:55.000000 Simba-UW-tf-dev-1.60.9/simba/assets/icons/add_on.png
+-rw-rw-r--   0 simon      (501) staff       (20)     4695 2023-03-17 17:57:16.000000 Simba-UW-tf-dev-1.60.9/simba/assets/icons/create.png
+-rw-r--r--   0 simon      (501) staff       (20)    78182 2023-03-20 16:35:36.000000 Simba-UW-tf-dev-1.60.9/simba/assets/icons/SimBA_logo.ico
+-rw-r--r--   0 simon      (501) staff       (20)     1067 2023-03-20 14:22:44.000000 Simba-UW-tf-dev-1.60.9/simba/assets/icons/print.png
+-rw-rw-r--   0 simon      (501) staff       (20)     4653 2023-03-18 20:27:58.000000 Simba-UW-tf-dev-1.60.9/simba/assets/icons/clf.png
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-24 15:39:15.000000 Simba-UW-tf-dev-1.60.9/simba/assets/icons/concat_icons/
+-rw-r--r--   0 simon      (501) staff       (20)     6027 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.60.9/simba/assets/icons/concat_icons/mosaic.png
+-rw-r--r--   0 simon      (501) staff       (20)     5654 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.60.9/simba/assets/icons/concat_icons/vertical.png
+-rw-r--r--   0 simon      (501) staff       (20)     5542 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.60.9/simba/assets/icons/concat_icons/horizontal.png
+-rw-r--r--   0 simon      (501) staff       (20)     5939 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.60.9/simba/assets/icons/concat_icons/mixed_mosaic.png
+-rw-r--r--   0 simon      (501) staff       (20)     2060 2023-03-20 14:26:12.000000 Simba-UW-tf-dev-1.60.9/simba/assets/icons/merge.png
+-rw-r--r--   0 simon      (501) staff       (20)     1252 2023-04-07 11:25:59.000000 Simba-UW-tf-dev-1.60.9/simba/assets/icons/clean.png
+-rw-------   0 simon      (501) staff       (20)     4725 2023-03-18 20:27:47.000000 Simba-UW-tf-dev-1.60.9/simba/assets/icons/clf_2.png
+-rw-rw-r--   0 simon      (501) staff       (20)     4795 2023-03-17 18:10:10.000000 Simba-UW-tf-dev-1.60.9/simba/assets/icons/visualize.png
+-rw-r--r--   0 simon      (501) staff       (20)     2142 2023-03-20 14:10:28.000000 Simba-UW-tf-dev-1.60.9/simba/assets/icons/concat.png
+-rw-r--r--   0 simon      (501) staff       (20)     1474 2023-03-17 19:20:24.000000 Simba-UW-tf-dev-1.60.9/simba/assets/icons/boris.png
+-rw-rw-r--   0 simon      (501) staff       (20)     4804 2023-03-19 16:43:01.000000 Simba-UW-tf-dev-1.60.9/simba/assets/icons/frames.png
+-rw-r--r--   0 simon      (501) staff       (20)     2425 2023-03-19 16:44:55.000000 Simba-UW-tf-dev-1.60.9/simba/assets/icons/video.png
+-rw-r--r--   0 simon      (501) staff       (20)     2089 2023-03-20 14:05:58.000000 Simba-UW-tf-dev-1.60.9/simba/assets/icons/sample.png
+-rw-r--r--   0 simon      (501) staff       (20)     1471 2023-03-21 13:04:02.000000 Simba-UW-tf-dev-1.60.9/simba/assets/icons/metrics.png
+-rw-r--r--   0 simon      (501) staff       (20)     4555 2023-03-20 14:21:02.000000 Simba-UW-tf-dev-1.60.9/simba/assets/icons/grey.png
+-rw-r--r--   0 simon      (501) staff       (20)      930 2023-03-18 18:07:29.000000 Simba-UW-tf-dev-1.60.9/simba/assets/icons/exit.png
+-rw-r--r--   0 simon      (501) staff       (20)     4751 2023-03-18 20:31:58.000000 Simba-UW-tf-dev-1.60.9/simba/assets/icons/outlier.png
+-rw-r--r--   0 simon      (501) staff       (20)     4392 2023-03-20 14:16:15.000000 Simba-UW-tf-dev-1.60.9/simba/assets/icons/clahe.png
+-rw-rw-r--   0 simon      (501) staff       (20)     4637 2023-03-17 19:03:55.000000 Simba-UW-tf-dev-1.60.9/simba/assets/icons/trash.png
+-rw-r--r--   0 simon      (501) staff       (20)     1239 2023-03-19 16:51:21.000000 Simba-UW-tf-dev-1.60.9/simba/assets/icons/about.png
+-rw-rw-r--   0 simon      (501) staff       (20)     4666 2023-03-17 18:01:21.000000 Simba-UW-tf-dev-1.60.9/simba/assets/icons/convert.png
+-rw-r--r--   0 simon      (501) staff       (20)    93229 2023-03-20 16:01:42.000000 Simba-UW-tf-dev-1.60.9/simba/assets/icons/SimBA_logo.icns
+-rw-r--r--   0 simon      (501) staff       (20)      991 2023-03-20 19:02:33.000000 Simba-UW-tf-dev-1.60.9/simba/assets/icons/reorganize.png
+-rw-rw-r--   0 simon      (501) staff       (20)     4784 2023-03-17 18:50:35.000000 Simba-UW-tf-dev-1.60.9/simba/assets/icons/browse.png
+-rw-r--r--   0 simon      (501) staff       (20)    30707 2023-03-20 16:33:38.000000 Simba-UW-tf-dev-1.60.9/simba/assets/icons/SimBA_logo.png
+-rw-r--r--   0 simon      (501) staff       (20)     2293 2023-03-17 19:24:38.000000 Simba-UW-tf-dev-1.60.9/simba/assets/icons/ethovision.png
+-rw-r--r--   0 simon      (501) staff       (20)     1018 2023-04-05 15:24:49.000000 Simba-UW-tf-dev-1.60.9/simba/assets/icons/close.png
+-rw-r--r--   0 simon      (501) staff       (20)    13672 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.60.9/simba/assets/dash_simba_base.css
+-rw-r--r--   0 simon      (501) staff       (20)    31812 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.60.9/simba/assets/TheGoldenLab.PNG
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-24 15:39:15.000000 Simba-UW-tf-dev-1.60.9/Simba_UW_tf_dev.egg-info/
+-rw-rw-r--   0 simon      (501) staff       (20)      579 2023-05-24 15:39:15.000000 Simba-UW-tf-dev-1.60.9/Simba_UW_tf_dev.egg-info/PKG-INFO
+-rw-rw-r--   0 simon      (501) staff       (20)    18435 2023-05-24 15:39:15.000000 Simba-UW-tf-dev-1.60.9/Simba_UW_tf_dev.egg-info/SOURCES.txt
+-rw-rw-r--   0 simon      (501) staff       (20)       44 2023-05-24 15:39:15.000000 Simba-UW-tf-dev-1.60.9/Simba_UW_tf_dev.egg-info/entry_points.txt
+-rw-rw-r--   0 simon      (501) staff       (20)      639 2023-05-24 15:39:15.000000 Simba-UW-tf-dev-1.60.9/Simba_UW_tf_dev.egg-info/requires.txt
+-rw-rw-r--   0 simon      (501) staff       (20)       12 2023-05-24 15:39:15.000000 Simba-UW-tf-dev-1.60.9/Simba_UW_tf_dev.egg-info/top_level.txt
+-rw-rw-r--   0 simon      (501) staff       (20)        1 2023-05-24 15:39:15.000000 Simba-UW-tf-dev-1.60.9/Simba_UW_tf_dev.egg-info/dependency_links.txt
+-rw-rw-r--   0 simon      (501) staff       (20)     7652 2020-05-13 13:27:38.000000 Simba-UW-tf-dev-1.60.9/LICENSE.md
+-rw-r--r--   0 simon      (501) staff       (20)       89 2023-05-20 17:55:56.000000 Simba-UW-tf-dev-1.60.9/pyproject.toml
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-24 15:39:16.000000 Simba-UW-tf-dev-1.60.9/tests/
+-rw-r--r--   0 simon      (501) staff       (20)     1723 2023-05-23 20:16:59.000000 Simba-UW-tf-dev-1.60.9/tests/test_data_processors.py
+-rw-r--r--   0 simon      (501) staff       (20)        0 2023-05-20 18:02:57.000000 Simba-UW-tf-dev-1.60.9/tests/__init__.py
+-rw-r--r--   0 simon      (501) staff       (20)     1859 2023-05-21 16:40:19.000000 Simba-UW-tf-dev-1.60.9/tests/test_featurizers.py
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-24 15:39:16.000000 Simba-UW-tf-dev-1.60.9/tests/data/
+-rw-r--r--   0 simon      (501) staff       (20)        0 2023-05-20 18:02:57.000000 Simba-UW-tf-dev-1.60.9/tests/data/__init__.py
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-24 15:39:16.000000 Simba-UW-tf-dev-1.60.9/tests/data/test_projects/
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-24 15:39:16.000000 Simba-UW-tf-dev-1.60.9/tests/data/test_projects/two_c57/
+-rw-r--r--   0 simon      (501) staff       (20)        0 2023-05-20 18:02:57.000000 Simba-UW-tf-dev-1.60.9/tests/data/test_projects/two_c57/__init__.py
+-rw-r--r--   0 simon      (501) staff       (20)        0 2023-05-20 18:02:57.000000 Simba-UW-tf-dev-1.60.9/tests/data/test_projects/__init__.py
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-24 15:39:16.000000 Simba-UW-tf-dev-1.60.9/tests/data/test_projects/mouse_open_field/
+-rw-r--r--   0 simon      (501) staff       (20)        0 2023-05-20 18:02:57.000000 Simba-UW-tf-dev-1.60.9/tests/data/test_projects/mouse_open_field/__init__.py
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-24 15:39:16.000000 Simba-UW-tf-dev-1.60.9/tests/data/test_projects/zebrafish/
+-rw-r--r--   0 simon      (501) staff       (20)        0 2023-05-20 18:02:57.000000 Simba-UW-tf-dev-1.60.9/tests/data/test_projects/zebrafish/__init__.py
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-24 15:39:16.000000 Simba-UW-tf-dev-1.60.9/tests/data/test_projects/zebrafish/feature_file/
+-rw-rw-r--   0 simon      (501) staff       (20)        0 2020-08-11 16:11:18.000000 Simba-UW-tf-dev-1.60.9/tests/data/test_projects/zebrafish/feature_file/__init__.py
+-rw-rw-r--   0 simon      (501) staff       (20)    14128 2022-04-11 08:07:36.000000 Simba-UW-tf-dev-1.60.9/tests/data/test_projects/zebrafish/feature_file/fish_feature_extraction_092221.py
+-rw-r--r--   0 simon      (501) staff       (20)     3972 2023-05-21 18:23:01.000000 Simba-UW-tf-dev-1.60.9/tests/test_thirdparty_appenders.py
+-rw-rw-r--   0 simon      (501) staff       (20)      136 2021-04-10 10:44:06.000000 Simba-UW-tf-dev-1.60.9/MANIFEST.in
+-rw-rw-r--   0 simon      (501) staff       (20)     9598 2020-05-13 13:27:40.000000 Simba-UW-tf-dev-1.60.9/README.md
+-rw-rw-r--   0 simon      (501) staff       (20)     1897 2023-05-24 15:39:09.000000 Simba-UW-tf-dev-1.60.9/setup.py
+-rw-r--r--   0 simon      (501) staff       (20)       38 2023-05-24 15:39:16.000000 Simba-UW-tf-dev-1.60.9/setup.cfg
```

### Comparing `Simba-UW-tf-dev-1.60.7/PKG-INFO` & `Simba-UW-tf-dev-1.60.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Simba-UW-tf-dev
-Version: 1.60.7
+Version: 1.60.9
 Summary: Toolkit for computer classification of complex social behaviors in experimental animals
 Home-page: https://github.com/sgoldenlab/simba
 Author: Simon Nilsson, Jia Jie Choong, Sophia Hwang
 Author-email: sronilsson@gmail.com
 License: GNU Lesser General Public License v3 (LGPLv3)
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

### Comparing `Simba-UW-tf-dev-1.60.7/simba/ui/.DS_Store` & `Simba-UW-tf-dev-1.60.9/simba/ui/.DS_Store`

 * *Files 18% similar despite different names*

```diff
@@ -281,99 +281,99 @@
 00001180: 7c7d 7e9a 0000 0000 0000 0101 0000 0000  |}~.............
 00001190: 0000 000f 0000 0000 0000 0000 0000 0000  ................
 000011a0: 0000 009b 0000 0007 0070 006f 0070 005f  .........p.o.p._
 000011b0: 0075 0070 0073 6c67 3153 636f 6d70 0000  .u.p.slg1Scomp..
 000011c0: 0000 0007 3ca2 0000 0007 0070 006f 0070  ....<......p.o.p
 000011d0: 005f 0075 0070 0073 6c73 7643 626c 6f62  ._.u.p.slsvCblob
 000011e0: 0000 02bb 6270 6c69 7374 3030 da01 0203  ....bplist00....
-000011f0: 0405 0607 0809 0a0b 0c0d 1848 494a 4b4c  ...........HIJKL
-00001200: 0c5f 1012 7669 6577 4f70 7469 6f6e 7356  ._..viewOptionsV
-00001210: 6572 7369 6f6e 5f10 0f73 686f 7749 636f  ersion_..showIco
-00001220: 6e50 7265 7669 6577 5763 6f6c 756d 6e73  nPreviewWcolumns
-00001230: 5f10 1163 616c 6375 6c61 7465 416c 6c53  _..calculateAllS
-00001240: 697a 6573 5f10 0f73 6372 6f6c 6c50 6f73  izes_..scrollPos
-00001250: 6974 696f 6e59 5874 6578 7453 697a 655f  itionYXtextSize_
-00001260: 100f 7363 726f 6c6c 506f 7369 7469 6f6e  ..scrollPosition
-00001270: 585a 736f 7274 436f 6c75 6d6e 5869 636f  XZsortColumnXico
-00001280: 6e53 697a 655f 1010 7573 6552 656c 6174  nSize_..useRelat
-00001290: 6976 6544 6174 6573 1001 09ab 0e17 1c21  iveDates.......!
-000012a0: 252a 2f34 393e 43d4 0f10 1112 1314 0c0c  %*/49>C.........
-000012b0: 5a69 6465 6e74 6966 6965 7255 7769 6474  ZidentifierUwidt
-000012c0: 6859 6173 6365 6e64 696e 6757 7669 7369  hYascendingWvisi
-000012d0: 626c 6554 6e61 6d65 1101 c709 09d4 1210  bleTname........
-000012e0: 110f 1819 181b 0810 2308 5875 6269 7175  ........#.Xubiqu
-000012f0: 6974 79d4 0f10 1112 1d1e 180c 5c64 6174  ity.........\dat
-00001300: 654d 6f64 6966 6965 6410 b508 09d4 0f10  eModified.......
-00001310: 1112 221e 1818 5b64 6174 6543 7265 6174  .."...[dateCreat
-00001320: 6564 0808 d40f 1011 1226 2718 0c54 7369  ed.......&'..Tsi
-00001330: 7a65 1061 0809 d40f 1011 122b 2c0c 0c54  ze.a.......+,..T
-00001340: 6b69 6e64 1073 0909 d40f 1011 1230 310c  kind.s.......01.
-00001350: 1855 6c61 6265 6c10 6409 08d4 0f10 1112  .Ulabel.d.......
-00001360: 3536 0c18 5776 6572 7369 6f6e 104b 0908  56..Wversion.K..
-00001370: d40f 1011 123a 3b0c 1858 636f 6d6d 656e  .....:;..Xcommen
-00001380: 7473 1101 2c09 08d4 0f10 1112 3f40 1818  ts..,.......?@..
-00001390: 5e64 6174 654c 6173 744f 7065 6e65 6410  ^dateLastOpened.
-000013a0: c808 08d4 1210 110f 181e 1846 0808 5964  ...........F..Yd
-000013b0: 6174 6541 6464 6564 0823 4074 d000 0000  ateAdded.#@t....
-000013c0: 0000 2340 2800 0000 0000 0023 0000 0000  ..#@(......#....
-000013d0: 0000 0000 546e 616d 6523 4030 0000 0000  ....Tname#@0....
-000013e0: 0000 0900 0800 1d00 3200 4400 4c00 6000  ........2.D.L.`.
-000013f0: 7200 7b00 8d00 9800 a100 b400 b600 b700  r.{.............
-00001400: c300 cc00 d700 dd00 e700 ef00 f400 f700  ................
-00001410: f800 f901 0201 0301 0501 0601 0f01 1801  ................
-00001420: 2501 2701 2801 2901 3201 3e01 3f01 4001  %.'.(.).2.>.?.@.
-00001430: 4901 4e01 5001 5101 5201 5b01 6001 6201  I.N.P.Q.R.[.`.b.
-00001440: 6301 6401 6d01 7301 7501 7601 7701 8001  c.d.m.s.u.v.w...
-00001450: 8801 8a01 8b01 8c01 9501 9e01 a101 a201  ................
-00001460: a301 ac01 bb01 bd01 be01 bf01 c801 c901  ................
-00001470: ca01 d401 d501 de01 e701 f001 f501 fe00  ................
+000011f0: 0405 0607 0809 0a0b 0c0d 1848 494a 4b0c  ...........HIJK.
+00001200: 4d58 6963 6f6e 5369 7a65 5f10 0f73 686f  MXiconSize_..sho
+00001210: 7749 636f 6e50 7265 7669 6577 5763 6f6c  wIconPreviewWcol
+00001220: 756d 6e73 5f10 1163 616c 6375 6c61 7465  umns_..calculate
+00001230: 416c 6c53 697a 6573 5f10 0f73 6372 6f6c  AllSizes_..scrol
+00001240: 6c50 6f73 6974 696f 6e59 5874 6578 7453  lPositionYXtextS
+00001250: 697a 655f 100f 7363 726f 6c6c 506f 7369  ize_..scrollPosi
+00001260: 7469 6f6e 585a 736f 7274 436f 6c75 6d6e  tionXZsortColumn
+00001270: 5f10 1075 7365 5265 6c61 7469 7665 4461  _..useRelativeDa
+00001280: 7465 735f 1012 7669 6577 4f70 7469 6f6e  tes_..viewOption
+00001290: 7356 6572 7369 6f6e 2340 3000 0000 0000  sVersion#@0.....
+000012a0: 0009 ab0e 171c 2125 2a2f 3439 3e43 d40f  ......!%*/49>C..
+000012b0: 1011 1213 140c 0c5a 6964 656e 7469 6669  .......Zidentifi
+000012c0: 6572 5577 6964 7468 5961 7363 656e 6469  erUwidthYascendi
+000012d0: 6e67 5776 6973 6962 6c65 546e 616d 6511  ngWvisibleTname.
+000012e0: 01c7 0909 d412 1011 0f18 1918 1b08 1023  ...............#
+000012f0: 0858 7562 6971 7569 7479 d40f 1011 121d  .Xubiquity......
+00001300: 1e18 0c5c 6461 7465 4d6f 6469 6669 6564  ...\dateModified
+00001310: 10b5 0809 d40f 1011 1222 1e18 185b 6461  ........."...[da
+00001320: 7465 4372 6561 7465 6408 08d4 0f10 1112  teCreated.......
+00001330: 2627 180c 5473 697a 6510 6108 09d4 0f10  &'..Tsize.a.....
+00001340: 1112 2b2c 0c0c 546b 696e 6410 7309 09d4  ..+,..Tkind.s...
+00001350: 0f10 1112 3031 0c18 556c 6162 656c 1064  ....01..Ulabel.d
+00001360: 0908 d40f 1011 1235 360c 1857 7665 7273  .......56..Wvers
+00001370: 696f 6e10 4b09 08d4 0f10 1112 3a3b 0c18  ion.K.......:;..
+00001380: 5863 6f6d 6d65 6e74 7311 012c 0908 d40f  Xcomments..,....
+00001390: 1011 123f 4018 185e 6461 7465 4c61 7374  ...?@..^dateLast
+000013a0: 4f70 656e 6564 10c8 0808 d412 1011 0f18  Opened..........
+000013b0: 1e18 4608 0859 6461 7465 4164 6465 6408  ..F..YdateAdded.
+000013c0: 2340 73a0 0000 0000 0023 4028 0000 0000  #@s......#@(....
+000013d0: 0000 2300 0000 0000 0000 0054 6e61 6d65  ..#........Tname
+000013e0: 0910 0100 0800 1d00 2600 3800 4000 5400  ........&.8.@.T.
+000013f0: 6600 6f00 8100 8c00 9f00 b400 bd00 be00  f.o.............
+00001400: ca00 d300 de00 e400 ee00 f600 fb00 fe00  ................
+00001410: ff01 0001 0901 0a01 0c01 0d01 1601 1f01  ................
+00001420: 2c01 2e01 2f01 3001 3901 4501 4601 4701  ,.../.0.9.E.F.G.
+00001430: 5001 5501 5701 5801 5901 6201 6701 6901  P.U.W.X.Y.b.g.i.
+00001440: 6a01 6b01 7401 7a01 7c01 7d01 7e01 8701  j.k.t.z.|.}.~...
+00001450: 8f01 9101 9201 9301 9c01 a501 a801 a901  ................
+00001460: aa01 b301 c201 c401 c501 c601 cf01 d001  ................
+00001470: d101 db01 dc01 e501 ee01 f701 fc01 fd00  ................
 00001480: 0000 0000 0002 0100 0000 0000 0000 4e00  ..............N.
 00001490: 0000 0000 0000 0000 0000 0000 0001 ff00  ................
 000014a0: 0000 0700 7000 6f00 7000 5f00 7500 7000  ....p.o.p._.u.p.
 000014b0: 736c 7376 7062 6c6f 6200 0002 a062 706c  slsvpblob....bpl
 000014c0: 6973 7430 30da 0102 0304 0506 0708 090a  ist00...........
-000014d0: 0b0c 0d1c 4748 494a 4b0c 5f10 1276 6965  ....GHIJK._..vie
-000014e0: 774f 7074 696f 6e73 5665 7273 696f 6e5f  wOptionsVersion_
-000014f0: 100f 7368 6f77 4963 6f6e 5072 6576 6965  ..showIconPrevie
-00001500: 7757 636f 6c75 6d6e 735f 1011 6361 6c63  wWcolumns_..calc
-00001510: 756c 6174 6541 6c6c 5369 7a65 735f 100f  ulateAllSizes_..
-00001520: 7363 726f 6c6c 506f 7369 7469 6f6e 5958  scrollPositionYX
-00001530: 7465 7874 5369 7a65 5f10 0f73 6372 6f6c  textSize_..scrol
-00001540: 6c50 6f73 6974 696f 6e58 5a73 6f72 7443  lPositionXZsortC
-00001550: 6f6c 756d 6e58 6963 6f6e 5369 7a65 5f10  olumnXiconSize_.
-00001560: 1075 7365 5265 6c61 7469 7665 4461 7465  .useRelativeDate
-00001570: 7310 0109 d90e 0f10 1112 1314 1516 1720  s.............. 
-00001580: 2529 2d32 373c 4158 636f 6d6d 656e 7473  %)-27<AXcomments
-00001590: 5e64 6174 654c 6173 744f 7065 6e65 645c  ^dateLastOpened\
-000015a0: 6461 7465 4d6f 6469 6669 6564 5b64 6174  dateModified[dat
-000015b0: 6543 7265 6174 6564 5473 697a 6555 6c61  eCreatedTsizeUla
-000015c0: 6265 6c54 6b69 6e64 5776 6572 7369 6f6e  belTkindWversion
-000015d0: 546e 616d 65d4 1819 1a1b 1c1d 0c1f 5776  Tname.........Wv
-000015e0: 6973 6962 6c65 5577 6964 7468 5961 7363  isibleUwidthYasc
-000015f0: 656e 6469 6e67 5569 6e64 6578 0811 012c  endingUindex...,
-00001600: 0910 07d4 1819 1a1b 1c22 1c24 0810 c808  .........".$....
-00001610: 1008 d418 191a 1b0c 271c 0b09 10b5 08d4  ........'.......
-00001620: 1819 1a1b 1c27 1c2c 0808 1002 d418 191a  .....'.,........
-00001630: 1b0c 2f1c 3109 1061 0810 03d4 1819 1a1b  ../.1..a........
-00001640: 1c34 0c36 0810 6409 1005 d418 191a 1b0c  .4.6..d.........
-00001650: 390c 3b09 1073 0910 04d4 1819 1a1b 1c3e  9.;..s.........>
-00001660: 0c40 0810 4b09 1006 d418 191a 1b0c 430c  .@..K.........C.
-00001670: 4509 1101 c709 1000 0823 4074 d000 0000  E........#@t....
-00001680: 0000 2340 2800 0000 0000 0023 0000 0000  ..#@(......#....
-00001690: 0000 0000 546e 616d 6523 4030 0000 0000  ....Tname#@0....
-000016a0: 0000 0900 0800 1d00 3200 4400 4c00 6000  ........2.D.L.`.
-000016b0: 7200 7b00 8d00 9800 a100 b400 b600 b700  r.{.............
-000016c0: ca00 d300 e200 ef00 fb01 0001 0601 0b01  ................
-000016d0: 1301 1801 2101 2901 2f01 3901 3f01 4001  ....!.)./.9.?.@.
-000016e0: 4301 4401 4601 4f01 5001 5201 5301 5501  C.D.F.O.P.R.S.U.
-000016f0: 5e01 5f01 6101 6201 6b01 6c01 6d01 6f01  ^._.a.b.k.l.m.o.
-00001700: 7801 7901 7b01 7c01 7e01 8701 8801 8a01  x.y.{.|.~.......
-00001710: 8b01 8d01 9601 9701 9901 9a01 9c01 a501  ................
-00001720: a601 a801 a901 ab01 b401 b501 b801 b901  ................
-00001730: bb01 bc01 c501 ce01 d701 dc01 e500 0000  ................
+000014d0: 0b0c 0d1c 4849 4a4b 0c29 5869 636f 6e53  ....HIJK.)XiconS
+000014e0: 697a 655f 100f 7368 6f77 4963 6f6e 5072  ize_..showIconPr
+000014f0: 6576 6965 7757 636f 6c75 6d6e 735f 1011  eviewWcolumns_..
+00001500: 6361 6c63 756c 6174 6541 6c6c 5369 7a65  calculateAllSize
+00001510: 735f 100f 7363 726f 6c6c 506f 7369 7469  s_..scrollPositi
+00001520: 6f6e 5958 7465 7874 5369 7a65 5f10 0f73  onYXtextSize_..s
+00001530: 6372 6f6c 6c50 6f73 6974 696f 6e58 5a73  crollPositionXZs
+00001540: 6f72 7443 6f6c 756d 6e5f 1010 7573 6552  ortColumn_..useR
+00001550: 656c 6174 6976 6544 6174 6573 5f10 1276  elativeDates_..v
+00001560: 6965 774f 7074 696f 6e73 5665 7273 696f  iewOptionsVersio
+00001570: 6e23 4030 0000 0000 0000 09d9 0e0f 1011  n#@0............
+00001580: 1213 1415 1617 2025 2a2e 3338 3d42 5863  ...... %*.38=BXc
+00001590: 6f6d 6d65 6e74 735e 6461 7465 4c61 7374  omments^dateLast
+000015a0: 4f70 656e 6564 5c64 6174 654d 6f64 6966  Opened\dateModif
+000015b0: 6965 645b 6461 7465 4372 6561 7465 6454  ied[dateCreatedT
+000015c0: 7369 7a65 556c 6162 656c 546b 696e 6457  sizeUlabelTkindW
+000015d0: 7665 7273 696f 6e54 6e61 6d65 d418 191a  versionTname....
+000015e0: 1b1c 1d0c 1f57 7669 7369 626c 6555 7769  .....WvisibleUwi
+000015f0: 6474 6859 6173 6365 6e64 696e 6755 696e  dthYascendingUin
+00001600: 6465 7808 1101 2c09 1007 d418 191a 1b1c  dex...,.........
+00001610: 221c 2408 10c8 0810 08d4 1819 1a1b 0c27  ".$............'
+00001620: 1c29 0910 b508 1001 d418 191a 1b1c 271c  .)............'.
+00001630: 2d08 0810 02d4 1819 1a1b 0c30 1c32 0910  -..........0.2..
+00001640: 6108 1003 d418 191a 1b1c 350c 3708 1064  a.........5.7..d
+00001650: 0910 05d4 1819 1a1b 0c3a 0c3c 0910 7309  .........:.<..s.
+00001660: 1004 d418 191a 1b1c 3f0c 4108 104b 0910  ........?.A..K..
+00001670: 06d4 1819 1a1b 0c44 0c46 0911 01c7 0910  .......D.F......
+00001680: 0008 2340 73a0 0000 0000 0023 4028 0000  ..#@s......#@(..
+00001690: 0000 0000 2300 0000 0000 0000 0054 6e61  ....#........Tna
+000016a0: 6d65 0900 0800 1d00 2600 3800 4000 5400  me......&.8.@.T.
+000016b0: 6600 6f00 8100 8c00 9f00 b400 bd00 be00  f.o.............
+000016c0: d100 da00 e900 f601 0201 0701 0d01 1201  ................
+000016d0: 1a01 1f01 2801 3001 3601 4001 4601 4701  ....(.0.6.@.F.G.
+000016e0: 4a01 4b01 4d01 5601 5701 5901 5a01 5c01  J.K.M.V.W.Y.Z.\.
+000016f0: 6501 6601 6801 6901 6b01 7401 7501 7601  e.f.h.i.k.t.u.v.
+00001700: 7801 8101 8201 8401 8501 8701 9001 9101  x...............
+00001710: 9301 9401 9601 9f01 a001 a201 a301 a501  ................
+00001720: ae01 af01 b101 b201 b401 bd01 be01 c101  ................
+00001730: c201 c401 c501 ce01 d701 e001 e500 0000  ................
 00001740: 0000 0002 0100 0000 0000 0000 4d00 0000  ............M...
 00001750: 0000 0000 0000 0000 0000 0001 e600 0000  ................
 00001760: 0700 7000 6f00 7000 5f00 7500 7000 736d  ..p.o.p._.u.p.sm
 00001770: 6f44 4462 6c6f 6200 0000 080e 96d0 4582  oDDblob.......E.
 00001780: 0ec5 4100 0000 0700 7000 6f00 7000 5f00  ..A.....p.o.p._.
 00001790: 7500 7000 736d 6f64 4462 6c6f 6200 0000  u.p.smodDblob...
 000017a0: 080e 96d0 4582 0ec5 4100 0000 0700 7000  ....E...A.....p.
@@ -457,51 +457,51 @@
 00001c80: 0000 0000 0100 0100 0000 0000 0100 0200  ................
 00001c90: 0000 0000 0100 0400 0000 0000 0100 0800  ................
 00001ca0: 0000 0000 0100 1000 0000 0000 0100 2000  .............. .
 00001cb0: 0000 0000 0100 4000 0000 0000 0100 8000  ......@.........
 00001cc0: 0000 0000 0101 0000 0000 0000 0102 0000  ................
 00001cd0: 0000 0000 0104 0000 0000 0000 0108 0000  ................
 00001ce0: 0000 0000 0110 0000 0000 0000 0120 0000  ............. ..
-00001cf0: 0000 0000 0140 0000 0000 0000 0076 6965  .....@.......vie
-00001d00: 7757 636f 6c75 6d6e 735f 1011 6361 6c63  wWcolumns_..calc
-00001d10: 756c 6174 6541 6c6c 5369 7a65 735f 100f  ulateAllSizes_..
-00001d20: 7363 726f 6c6c 506f 7369 7469 6f6e 5958  scrollPositionYX
-00001d30: 7465 7874 5369 7a65 5f10 0f73 6372 6f6c  textSize_..scrol
-00001d40: 6c50 6f73 6974 696f 6e58 5a73 6f72 7443  lPositionXZsortC
-00001d50: 6f6c 756d 6e58 6963 6f6e 5369 7a65 5f10  olumnXiconSize_.
-00001d60: 1075 7365 5265 6c61 7469 7665 4461 7465  .useRelativeDate
-00001d70: 7310 0109 d90e 0f10 1112 1314 1516 1720  s.............. 
-00001d80: 2529 2d32 373c 4158 636f 6d6d 656e 7473  %)-27<AXcomments
-00001d90: 5e64 6174 654c 6173 744f 7065 6e65 645c  ^dateLastOpened\
-00001da0: 6461 7465 4d6f 6469 6669 6564 5b64 6174  dateModified[dat
-00001db0: 6543 7265 6174 6564 5473 697a 6555 6c61  eCreatedTsizeUla
-00001dc0: 6265 6c54 6b69 6e64 5776 6572 7369 6f6e  belTkindWversion
-00001dd0: 546e 616d 65d4 1819 1a1b 1c1d 0c1f 5776  Tname.........Wv
-00001de0: 6973 6962 6c65 5577 6964 7468 5961 7363  isibleUwidthYasc
-00001df0: 656e 6469 6e67 5569 6e64 6578 0811 012c  endingUindex...,
-00001e00: 0910 07d4 1819 1a1b 1c22 1c24 0810 c808  .........".$....
-00001e10: 1008 d418 191a 1b0c 271c 0b09 10b5 08d4  ........'.......
-00001e20: 1819 1a1b 1c27 1c2c 0808 1002 d418 191a  .....'.,........
-00001e30: 1b0c 2f1c 3109 1061 0810 03d4 1819 1a1b  ../.1..a........
-00001e40: 1c34 0c36 0810 6409 1005 d418 191a 1b0c  .4.6..d.........
-00001e50: 390c 3b09 1073 0910 04d4 1819 1a1b 1c3e  9.;..s.........>
-00001e60: 0c40 0810 4b09 1006 d418 191a 1b0c 430c  .@..K.........C.
-00001e70: 4509 1101 c709 1000 0823 4074 d000 0000  E........#@t....
-00001e80: 0000 2340 2800 0000 0000 0023 0000 0000  ..#@(......#....
-00001e90: 0000 0000 546e 616d 6523 4030 0000 0000  ....Tname#@0....
-00001ea0: 0000 0900 0800 1d00 3200 4400 4c00 6000  ........2.D.L.`.
-00001eb0: 7200 7b00 8d00 9800 a100 b400 b600 b700  r.{.............
-00001ec0: ca00 d300 e200 ef00 fb01 0001 0601 0b01  ................
-00001ed0: 1301 1801 2101 2901 2f01 3901 3f01 4001  ....!.)./.9.?.@.
-00001ee0: 4301 4401 4601 4f01 5001 5201 5301 5501  C.D.F.O.P.R.S.U.
-00001ef0: 5e01 5f01 6101 6201 6b01 6c01 6d01 6f01  ^._.a.b.k.l.m.o.
-00001f00: 7801 7901 7b01 7c01 7e01 8701 8801 8a01  x.y.{.|.~.......
-00001f10: 8b01 8d01 9601 9701 9901 9a01 9c01 a501  ................
-00001f20: a601 a801 a901 ab01 b401 b501 b801 b901  ................
-00001f30: bb01 bc01 c501 ce01 d701 dc01 e500 0000  ................
+00001cf0: 0000 0000 0140 0000 0000 0000 005f 1011  .....@......._..
+00001d00: 6361 6c63 756c 6174 6541 6c6c 5369 7a65  calculateAllSize
+00001d10: 735f 100f 7363 726f 6c6c 506f 7369 7469  s_..scrollPositi
+00001d20: 6f6e 5958 7465 7874 5369 7a65 5f10 0f73  onYXtextSize_..s
+00001d30: 6372 6f6c 6c50 6f73 6974 696f 6e58 5a73  crollPositionXZs
+00001d40: 6f72 7443 6f6c 756d 6e5f 1010 7573 6552  ortColumn_..useR
+00001d50: 656c 6174 6976 6544 6174 6573 5f10 1276  elativeDates_..v
+00001d60: 6965 774f 7074 696f 6e73 5665 7273 696f  iewOptionsVersio
+00001d70: 6e23 4030 0000 0000 0000 09d9 0e0f 1011  n#@0............
+00001d80: 1213 1415 1617 2025 2a2e 3338 3d42 5863  ...... %*.38=BXc
+00001d90: 6f6d 6d65 6e74 735e 6461 7465 4c61 7374  omments^dateLast
+00001da0: 4f70 656e 6564 5c64 6174 654d 6f64 6966  Opened\dateModif
+00001db0: 6965 645b 6461 7465 4372 6561 7465 6454  ied[dateCreatedT
+00001dc0: 7369 7a65 556c 6162 656c 546b 696e 6457  sizeUlabelTkindW
+00001dd0: 7665 7273 696f 6e54 6e61 6d65 d418 191a  versionTname....
+00001de0: 1b1c 1d0c 1f57 7669 7369 626c 6555 7769  .....WvisibleUwi
+00001df0: 6474 6859 6173 6365 6e64 696e 6755 696e  dthYascendingUin
+00001e00: 6465 7808 1101 2c09 1007 d418 191a 1b1c  dex...,.........
+00001e10: 221c 2408 10c8 0810 08d4 1819 1a1b 0c27  ".$............'
+00001e20: 1c29 0910 b508 1001 d418 191a 1b1c 271c  .)............'.
+00001e30: 2d08 0810 02d4 1819 1a1b 0c30 1c32 0910  -..........0.2..
+00001e40: 6108 1003 d418 191a 1b1c 350c 3708 1064  a.........5.7..d
+00001e50: 0910 05d4 1819 1a1b 0c3a 0c3c 0910 7309  .........:.<..s.
+00001e60: 1004 d418 191a 1b1c 3f0c 4108 104b 0910  ........?.A..K..
+00001e70: 06d4 1819 1a1b 0c44 0c46 0911 01c7 0910  .......D.F......
+00001e80: 0008 2340 73a0 0000 0000 0023 4028 0000  ..#@s......#@(..
+00001e90: 0000 0000 2300 0000 0000 0000 0054 6e61  ....#........Tna
+00001ea0: 6d65 0900 0800 1d00 2600 3800 4000 5400  me......&.8.@.T.
+00001eb0: 6600 6f00 8100 8c00 9f00 b400 bd00 be00  f.o.............
+00001ec0: d100 da00 e900 f601 0201 0701 0d01 1201  ................
+00001ed0: 1a01 1f01 2801 3001 3601 4001 4601 4701  ....(.0.6.@.F.G.
+00001ee0: 4a01 4b01 4d01 5601 5701 5901 5a01 5c01  J.K.M.V.W.Y.Z.\.
+00001ef0: 6501 6601 6801 6901 6b01 7401 7501 7601  e.f.h.i.k.t.u.v.
+00001f00: 7801 8101 8201 8401 8501 8701 9001 9101  x...............
+00001f10: 9301 9401 9601 9f01 a001 a201 a301 a501  ................
+00001f20: ae01 af01 b101 b201 b401 bd01 be01 c101  ................
+00001f30: c201 c401 c501 ce01 d701 e001 e500 0000  ................
 00001f40: 0000 0002 0100 0000 0000 0000 4d00 0000  ............M...
 00001f50: 0000 0000 0000 0000 0000 0001 e600 0000  ................
 00001f60: 0700 7000 6f00 7000 5f00 7500 7000 736d  ..p.o.p._.u.p.sm
 00001f70: 6f44 4462 6c6f 6200 0000 080e 96d0 4582  oDDblob.......E.
 00001f80: 0ec5 4100 0000 0700 7000 6f00 7000 5f00  ..A.....p.o.p._.
 00001f90: 7500 7000 736d 6f64 4462 6c6f 6200 0000  u.p.smodDblob...
 00001fa0: 080e 96d0 4582 0ec5 4100 0000 0700 7000  ....E...A.....p.
```

### Comparing `Simba-UW-tf-dev-1.60.7/simba/ui/pop_ups/movement_analysis_time_bins_pop_up.py` & `Simba-UW-tf-dev-1.60.9/simba/ui/pop_ups/movement_analysis_time_bins_pop_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.60.7/simba/ui/pop_ups/csv_2_parquet_pop_up.py` & `Simba-UW-tf-dev-1.60.9/simba/ui/pop_ups/csv_2_parquet_pop_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.60.7/simba/ui/pop_ups/quick_path_plot_pop_up.py` & `Simba-UW-tf-dev-1.60.9/simba/ui/pop_ups/quick_path_plot_pop_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.60.7/simba/ui/pop_ups/batch_preprocess_pop_up.py` & `Simba-UW-tf-dev-1.60.9/simba/ui/pop_ups/batch_preprocess_pop_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.60.7/simba/ui/pop_ups/heatmap_location_pop_up.py` & `Simba-UW-tf-dev-1.60.9/simba/ui/pop_ups/heatmap_location_pop_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.60.7/simba/ui/pop_ups/clf_probability_plot_pop_up.py` & `Simba-UW-tf-dev-1.60.9/simba/ui/pop_ups/clf_probability_plot_pop_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.60.7/simba/ui/pop_ups/.DS_Store` & `Simba-UW-tf-dev-1.60.9/simba/ui/pop_ups/.DS_Store`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.60.7/simba/ui/pop_ups/movement_analysis_pop_up.py` & `Simba-UW-tf-dev-1.60.9/simba/ui/pop_ups/movement_analysis_pop_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.60.7/simba/ui/pop_ups/set_machine_model_parameters_pop_up.py` & `Simba-UW-tf-dev-1.60.9/simba/ui/pop_ups/set_machine_model_parameters_pop_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.60.7/simba/ui/pop_ups/clf_plot_pop_up.py` & `Simba-UW-tf-dev-1.60.9/simba/ui/pop_ups/clf_plot_pop_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.60.7/simba/ui/pop_ups/path_plot_pop_up.py` & `Simba-UW-tf-dev-1.60.9/simba/ui/pop_ups/path_plot_pop_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.60.7/simba/ui/pop_ups/smoothing_interpolation_pop_up.py` & `Simba-UW-tf-dev-1.60.9/simba/ui/pop_ups/smoothing_interpolation_pop_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.60.7/simba/ui/pop_ups/visualize_pose_in_dir_pop_up.py` & `Simba-UW-tf-dev-1.60.9/simba/ui/pop_ups/visualize_pose_in_dir_pop_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.60.7/simba/ui/pop_ups/roi_analysis_pop_up.py` & `Simba-UW-tf-dev-1.60.9/simba/ui/pop_ups/roi_analysis_pop_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.60.7/simba/ui/pop_ups/outlier_settings_pop_up.py` & `Simba-UW-tf-dev-1.60.9/simba/ui/pop_ups/outlier_settings_pop_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.60.7/simba/ui/pop_ups/gantt_pop_up.py` & `Simba-UW-tf-dev-1.60.9/simba/ui/pop_ups/gantt_pop_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.60.7/simba/ui/pop_ups/clf_validation_plot_pop_up.py` & `Simba-UW-tf-dev-1.60.9/simba/ui/pop_ups/clf_validation_plot_pop_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.60.7/simba/ui/pop_ups/severity_analysis_pop_up.py` & `Simba-UW-tf-dev-1.60.9/simba/ui/pop_ups/severity_analysis_pop_up.py`

 * *Files 8% similar despite different names*

```diff
@@ -23,65 +23,68 @@
         self.clip_cnt_options.insert(0, 'ALL CLIPS')
         self.frame_cnt_var = BooleanVar(value=False)
         self.seconds_cnt_var = BooleanVar(value=False)
         self.settings_frm = CreateLabelFrameWithIcon(parent=self.main_frm, header='SETTINGS', icon_name=Keys.DOCUMENTATION.value, icon_link=Links.ANALYZE_ML_RESULTS.value)
         self.clf_dropdown = DropDownMenu(self.settings_frm, 'CLASSIFIER:', self.clf_names, '25')
         self.clf_dropdown.setChoices(self.clf_names[0])
         self.brackets_dropdown = DropDownMenu(self.settings_frm, 'BRACKETS:', list(range(1,21)), '25')
+        self.bracket_type_dropdown = DropDownMenu(self.settings_frm, 'BRACKET TYPE: ', ['QUANTIZE', 'QUANTILE'], '25')
         self.brackets_dropdown.setChoices(10)
+        self.bracket_type_dropdown.setChoices('QUANTIZE')
         self.animal_dropdown = DropDownMenu(self.settings_frm, 'ANIMALS', self.multi_animal_id_list, '25')
         self.animal_dropdown.setChoices(self.multi_animal_id_list[0])
         self.bouts_vs_frames_dropdown = DropDownMenu(self.settings_frm, 'DATA TYPE: ', ['BOUTS', 'FRAMES'], '25', com=self.show_settings)
         self.bouts_vs_frames_dropdown.setChoices('FRAMES')
         self.normalization_type_dropdown = DropDownMenu(self.settings_frm, 'MOVEMENT NORMALIZATION TYPE: ', ['ALL VIDEOS', 'SINGLE VIDEOS'], '25')
         self.normalization_type_dropdown.setChoices('ALL VIDEOS')
         self.save_bracket_cut_off_points_var = BooleanVar(value=True)
         self.savet_brackets_info_cb = Checkbutton(self.settings_frm, text='Save bracket definitions', variable=self.save_bracket_cut_off_points_var)
         self.further_settings_frm = LabelFrame(self.main_frm, text='Further settings', font=Formats.LABELFRAME_HEADER_FORMAT.value, pady=5, padx=5, fg='black')
         run_frm = LabelFrame(self.main_frm, text='RUN', font=Formats.LABELFRAME_HEADER_FORMAT.value, pady=5, padx=5, fg='black')
         run_btn = Button(run_frm, text='RUN SEVERITY ANALYSIS', command= lambda: self.run())
         self.settings_frm.grid(row=0, column=0, sticky=NW)
         self.clf_dropdown.grid(row=0, column=0, sticky=NW)
         self.brackets_dropdown.grid(row=1, column=0, sticky=NW)
-        self.animal_dropdown.grid(row=2, column=0, sticky=NW)
-        self.bouts_vs_frames_dropdown.grid(row=3, column=0, sticky=NW)
-        self.normalization_type_dropdown.grid(row=4, column=0, sticky=NW)
-        self.savet_brackets_info_cb.grid(row=5, column=0, sticky=NW)
+        self.bracket_type_dropdown.grid(row=2, column=0, sticky=NW)
+        self.animal_dropdown.grid(row=3, column=0, sticky=NW)
+        self.bouts_vs_frames_dropdown.grid(row=4, column=0, sticky=NW)
+        self.normalization_type_dropdown.grid(row=5, column=0, sticky=NW)
+        self.savet_brackets_info_cb.grid(row=6, column=0, sticky=NW)
         self.further_settings_frm.grid(row=2, column=0, sticky=NW)
         run_frm.grid(row=3, column=0, sticky=NW)
         run_btn.grid(row=0, column=0, sticky=NW)
+        self.show_settings(self.bouts_vs_frames_dropdown.getChoices())
         self.main_frm.mainloop()
 
     def show_settings(self, setting):
         for w in self.further_settings_frm.winfo_children():
             w.destroy()
+
+        self.further_settings_frm.grid()
+        self.visualize_var = BooleanVar(value=False)
+        self.show_pose_var = BooleanVar(value=False)
+        self.visualize_cb = Checkbutton(self.further_settings_frm, text='Visualize', variable=self.visualize_var, command=self.enable_visualization_options)
+        self.show_pose_cb = Checkbutton(self.further_settings_frm, text='Show pose-estimated locations', variable=self.show_pose_var)
+        self.video_speed_dropdown = DropDownMenu(self.further_settings_frm, 'Video speed:', [float(i) / 10 for i in range(1, 21)], '25')
+        self.video_speed_dropdown.setChoices(1.0)
+        self.number_of_clips_dropdown = DropDownMenu(self.further_settings_frm, 'Clip count:', self.clip_cnt_options, '25')
+        self.show_pose_cb.config(state=DISABLED)
+        self.video_speed_dropdown.disable()
+        self.number_of_clips_dropdown.disable()
+        self.visualize_cb.grid(row=0, column=0, sticky=NW)
+        self.show_pose_cb.grid(row=1, column=0, sticky=NW)
+        self.video_speed_dropdown.grid(row=2, column=0, sticky=NW)
+        self.number_of_clips_dropdown.grid(row=3, column=0, sticky=NW)
+        self.number_of_clips_dropdown.setChoices('ALL CLIPS')
+
         if setting == 'FRAMES':
-            self.further_settings_frm.grid()
             self.frame_cnt_cb = Checkbutton(self.further_settings_frm, text='FRAME COUNT', variable=self.frame_cnt_var)
             self.seconds_cnt_cb = Checkbutton(self.further_settings_frm, text='SECONDS', variable=self.seconds_cnt_var)
-            self.frame_cnt_cb.grid(row=0, column=0, sticky=NW)
-            self.seconds_cnt_cb.grid(row=1, column=0, sticky=NW)
-
-        if setting == 'BOUTS':
-            self.further_settings_frm.grid()
-            self.visualize_var = BooleanVar(value=False)
-            self.show_pose_var = BooleanVar(value=False)
-            self.visualize_cb = Checkbutton(self.further_settings_frm, text='Visualize', variable=self.visualize_var, command=self.enable_visualization_options)
-            self.show_pose_cb = Checkbutton(self.further_settings_frm, text='Show pose-estimated locations', variable=self.show_pose_var)
-            self.video_speed_dropdown = DropDownMenu(self.further_settings_frm, 'Video speed:', [float(i) / 10 for i in range(1, 21)], '25')
-            self.video_speed_dropdown.setChoices(1.0)
-            self.number_of_clips_dropdown = DropDownMenu(self.further_settings_frm, 'Clip count:', self.clip_cnt_options, '25')
-            self.show_pose_cb.config(state=DISABLED)
-            self.video_speed_dropdown.disable()
-            self.number_of_clips_dropdown.disable()
-            self.visualize_cb.grid(row=0, column=0, sticky=NW)
-            self.show_pose_cb.grid(row=1, column=0, sticky=NW)
-            self.video_speed_dropdown.grid(row=2, column=0, sticky=NW)
-            self.number_of_clips_dropdown.grid(row=3, column=0, sticky=NW)
-            self.number_of_clips_dropdown.setChoices('ALL CLIPS')
+            self.frame_cnt_cb.grid(row=4, column=0, sticky=NW)
+            self.seconds_cnt_cb.grid(row=5, column=0, sticky=NW)
 
     def enable_visualization_options(self):
         if self.visualize_var.get():
             self.show_pose_cb.config(state=NORMAL)
             self.video_speed_dropdown.enable()
             self.number_of_clips_dropdown.enable()
         else:
@@ -91,33 +94,32 @@
 
     def run(self):
         if self.animal_dropdown.getChoices() == 'ALL ANIMALS':
             animals = self.multi_animal_id_list[1:]
         else:
             animals = [self.animal_dropdown.getChoices()]
         settings = {'brackets': int(self.brackets_dropdown.getChoices()),
+                    'bracket_type': self.bracket_type_dropdown.getChoices(),
                     'clf': self.clf_dropdown.getChoices(),
                     'animals': animals,
                     'save_bin_definitions': self.save_bracket_cut_off_points_var.get(),
                     'normalization': self.normalization_type_dropdown.getChoices()}
+        settings['visualize'] = self.visualize_var.get()
+        settings['video_speed'] = float(self.video_speed_dropdown.getChoices())
+        settings['visualize_event_cnt'] = self.number_of_clips_dropdown.getChoices()
+        settings['show_pose'] = self.show_pose_var.get()
         if self.bouts_vs_frames_dropdown.getChoices() == 'FRAMES':
             settings['frames'] = self.frame_cnt_var.get()
             settings['time'] = self.seconds_cnt_var.get()
             if (not self.seconds_cnt_var.get()) and (not self.frame_cnt_var.get()):
                 raise NoSpecifiedOutputError(msg='SIMBA ERROR: Please select frames and/or time output metrics')
-        else:
-            settings['visualize'] = self.visualize_var.get()
-            settings['video_speed'] = float(self.video_speed_dropdown.getChoices())
-            settings['visualize_event_cnt'] = self.number_of_clips_dropdown.getChoices()
-            settings['show_pose'] = self.show_pose_var.get()
 
         if self.bouts_vs_frames_dropdown.getChoices() == 'FRAMES':
             severity_calculator = SeverityFrameCalculator(config_path=self.config_path,
                                                           settings=settings)
         else:
             severity_calculator = SeverityBoutCalculator(config_path=self.config_path,
                                                           settings=settings)
 
         severity_calculator.run()
-        severity_calculator.save()
 
 #_ = AnalyzeSeverityPopUp(config_path='/Users/simon/Desktop/envs/troubleshooting/two_black_animals_14bp/project_folder/project_config.ini')
```

### Comparing `Simba-UW-tf-dev-1.60.7/simba/ui/pop_ups/fsttc_pop_up.py` & `Simba-UW-tf-dev-1.60.9/simba/ui/pop_ups/fsttc_pop_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.60.7/simba/ui/pop_ups/kleinberg_pop_up.py` & `Simba-UW-tf-dev-1.60.9/simba/ui/pop_ups/kleinberg_pop_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.60.7/simba/ui/pop_ups/directing_other_animals_plot_pop_up.py` & `Simba-UW-tf-dev-1.60.9/simba/ui/pop_ups/directing_other_animals_plot_pop_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.60.7/simba/ui/pop_ups/pose_reorganizer_pop_up.py` & `Simba-UW-tf-dev-1.60.9/simba/ui/pop_ups/pose_reorganizer_pop_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.60.7/simba/ui/pop_ups/append_roi_features_animals_pop_up.py` & `Simba-UW-tf-dev-1.60.9/simba/ui/pop_ups/append_roi_features_animals_pop_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.60.7/simba/ui/pop_ups/clf_by_timebins_pop_up.py` & `Simba-UW-tf-dev-1.60.9/simba/ui/pop_ups/clf_by_timebins_pop_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.60.7/simba/ui/pop_ups/heatmap_clf_pop_up.py` & `Simba-UW-tf-dev-1.60.9/simba/ui/pop_ups/heatmap_clf_pop_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.60.7/simba/ui/pop_ups/data_plot_pop_up.py` & `Simba-UW-tf-dev-1.60.9/simba/ui/pop_ups/data_plot_pop_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.60.7/simba/ui/pop_ups/roi_features_plot_pop_up.py` & `Simba-UW-tf-dev-1.60.9/simba/ui/pop_ups/roi_features_plot_pop_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.60.7/simba/ui/pop_ups/pup_retrieval_pop_up.py` & `Simba-UW-tf-dev-1.60.9/simba/ui/pop_ups/pup_retrieval_pop_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.60.7/simba/ui/pop_ups/about_simba_pop_up.py` & `Simba-UW-tf-dev-1.60.9/simba/ui/pop_ups/about_simba_pop_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.60.7/simba/ui/pop_ups/clf_descriptive_statistics_pop_up.py` & `Simba-UW-tf-dev-1.60.9/simba/ui/pop_ups/clf_descriptive_statistics_pop_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.60.7/simba/ui/pop_ups/roi_tracking_plot_pop_up.py` & `Simba-UW-tf-dev-1.60.9/simba/ui/pop_ups/roi_tracking_plot_pop_up.py`

 * *Files 1% similar despite different names*

```diff
@@ -84,14 +84,15 @@
             with open(self.config_path, 'w') as f:
                 self.config.write(f)
             for video in videos:
                 roi_plotter = ROIPlot(ini_path=self.config_path, video_path=video, style_attr=style_attr)
                 roi_plotter.insert_data()
                 roi_plotter_multiprocessor = multiprocessing.Process(target=roi_plotter.visualize_ROI_data())
                 roi_plotter_multiprocessor.start()
+
         else:
             with open(self.config_path, 'w') as f:
                 self.config.write(f)
             core_cnt = self.multiprocess_dropdown.getChoices()
             for video in videos:
                 roi_plotter = ROIPlotMultiprocess(ini_path=self.config_path, video_path=video, core_cnt=int(core_cnt), style_attr=style_attr)
                 roi_plotter.run()
```

### Comparing `Simba-UW-tf-dev-1.60.7/simba/ui/pop_ups/append_roi_features_bodypart_pop_up.py` & `Simba-UW-tf-dev-1.60.9/simba/ui/pop_ups/append_roi_features_bodypart_pop_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.60.7/simba/ui/pop_ups/clf_add_remove_print_pop_up.py` & `Simba-UW-tf-dev-1.60.9/simba/ui/pop_ups/clf_add_remove_print_pop_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.60.7/simba/ui/pop_ups/video_processing_pop_up.py` & `Simba-UW-tf-dev-1.60.9/simba/ui/pop_ups/video_processing_pop_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.60.7/simba/ui/pop_ups/validation_plot_pop_up.py` & `Simba-UW-tf-dev-1.60.9/simba/ui/pop_ups/validation_plot_pop_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.60.7/simba/ui/pop_ups/clf_by_roi_pop_up.py` & `Simba-UW-tf-dev-1.60.9/simba/ui/pop_ups/clf_by_roi_pop_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.60.7/simba/ui/pop_ups/make_path_plot_pop_up.py` & `Simba-UW-tf-dev-1.60.9/simba/ui/pop_ups/make_path_plot_pop_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.60.7/simba/ui/pop_ups/create_user_defined_pose_configuration_pop_up.py` & `Simba-UW-tf-dev-1.60.9/simba/ui/pop_ups/create_user_defined_pose_configuration_pop_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.60.7/simba/ui/pop_ups/archive_files_pop_up.py` & `Simba-UW-tf-dev-1.60.9/simba/ui/pop_ups/archive_files_pop_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.60.7/simba/ui/pop_ups/pose_bp_drop_pop_up.py` & `Simba-UW-tf-dev-1.60.9/simba/ui/pop_ups/pose_bp_drop_pop_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.60.7/simba/ui/pop_ups/distance_plot_pop_up.py` & `Simba-UW-tf-dev-1.60.9/simba/ui/pop_ups/distance_plot_pop_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.60.7/simba/ui/pop_ups/subset_feature_extractor_pop_up.py` & `Simba-UW-tf-dev-1.60.9/simba/ui/pop_ups/subset_feature_extractor_pop_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.60.7/simba/ui/pop_ups/third_party_annotator_appender_pop_up.py` & `Simba-UW-tf-dev-1.60.9/simba/ui/pop_ups/third_party_annotator_appender_pop_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.60.7/simba/ui/pop_ups/roi_analysis_time_bins_pop_up.py` & `Simba-UW-tf-dev-1.60.9/simba/ui/pop_ups/roi_analysis_time_bins_pop_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.60.7/simba/ui/video_info_ui.py` & `Simba-UW-tf-dev-1.60.9/simba/ui/video_info_ui.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.60.7/simba/ui/user_defined_pose_creator.py` & `Simba-UW-tf-dev-1.60.9/simba/ui/user_defined_pose_creator.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.60.7/simba/ui/create_project_ui.py` & `Simba-UW-tf-dev-1.60.9/simba/ui/create_project_ui.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.60.7/simba/ui/tkinter_functions.py` & `Simba-UW-tf-dev-1.60.9/simba/ui/tkinter_functions.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.60.7/simba/ui/machine_model_settings_ui.py` & `Simba-UW-tf-dev-1.60.9/simba/ui/machine_model_settings_ui.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.60.7/simba/blob_storage/.DS_Store` & `Simba-UW-tf-dev-1.60.9/simba/blob_storage/.DS_Store`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.60.7/simba/labelling/.DS_Store` & `Simba-UW-tf-dev-1.60.9/simba/labelling/.DS_Store`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.60.7/simba/labelling/labelling_interface.py` & `Simba-UW-tf-dev-1.60.9/simba/labelling/labelling_interface.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.60.7/simba/labelling/extract_labelled_frames.py` & `Simba-UW-tf-dev-1.60.9/simba/labelling/extract_labelled_frames.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.60.7/simba/labelling/labelling_advanced_interface.py` & `Simba-UW-tf-dev-1.60.9/simba/labelling/labelling_advanced_interface.py`

 * *Files 3% similar despite different names*

```diff
@@ -12,14 +12,15 @@
 from simba.utils.checks import check_int, check_file_exist_and_readable
 from simba.utils.read_write import (read_config_entry,
                                     get_video_meta_data,
                                     get_fn_ext,
                                     read_df,
                                     write_df,
                                     get_all_clf_names)
+from simba.utils.enums import Formats
 from simba.utils.errors import FrameRangeError, AdvancedLabellingError
 from simba.utils.printing import stdout_success
 from simba.mixins.config_reader import ConfigReader
 
 class AdvancedLabellingInterface(ConfigReader):
     """
     Launch advanced labelling (annotation) interface in SimBA.
@@ -56,20 +57,21 @@
         self.max_frm_no = max(self.frame_lst)
         self.target_lst = get_all_clf_names(config=self.config, target_cnt=self.clf_cnt)
         self.max_frm_size = 1080, 650
         self.main_window = Toplevel()
         if continuing:
             check_file_exist_and_readable(file_path=self.targets_inserted_file_path)
             check_file_exist_and_readable(file_path=self.features_extracted_file_path)
-            self.data_df = read_df(self.targets_inserted_file_path, self.file_type)
+            if self.file_type == Formats.CSV.value:
+                self.data_df = pd.read_csv(self.targets_inserted_file_path).set_index('Unnamed: 0')[self.target_lst]
+                self.data_df.index.name = None
+            if self.file_type == Formats.PARQUET.value:
+                self.data_df = pd.read_parquet(self.targets_inserted_file_path)[self.target_lst]
             self.data_df_features = read_df(self.features_extracted_file_path, self.file_type)
-            missing_idx = self.data_df_features.index.difference(self.data_df.index)
-            if len(missing_idx) > 0:
-                self.data_df_features = self.data_df_features.iloc[self.data_df_features.index.difference(self.data_df.index)]
-                self.data_df = pd.concat([self.data_df, self.data_df_features], axis=0).sort_index()
+            self.data_df = self.data_df_features.join(self.data_df)
             self.main_window.title('SIMBA ANNOTATION INTERFACE (CONTINUING ANNOTATIONS)')
             try:
                 self.frm_no = read_config_entry(self.config, 'Last annotated frames', self.video_name.lower(), data_type='int')
             except ValueError:
                 pass
         else:
             check_file_exist_and_readable(file_path=self.features_extracted_file_path)
@@ -99,23 +101,23 @@
         self.jump_size.set(0)
         self.jump_back = Button(self.jump_frame, text="<<",command=lambda: self.advance_frame(int(self.change_frm_box.get()) - self.jump_size.get()))
         self.jump_forward = Button(self.jump_frame, text=">>", command=lambda: self.advance_frame(int(self.change_frm_box.get()) + self.jump_size.get()))
 
         self.folder.grid(row=0, column=1, sticky=N)
         self.buttons_frm.grid(row=1, column=0)
         self.change_frm_box.grid(row=0, column=1)
-        self.forward_btn.grid(row=1, column=3, sticky=E, padx=self.padding)
         self.last_present_forward_btn.grid(row=1, column=0, sticky=W, padx=self.padding)
         self.last_absent_forward_btn.grid(row=1, column=1, sticky=W, padx=self.padding)
         self.backward_max_btn.grid(row=1, column=2, sticky=W, padx=self.padding)
         self.backward_btn.grid(row=1, column=3, sticky=W, padx=self.padding)
         self.change_frm_box.grid(row=1, column=4)
-        self.forward_max_btn.grid(row=1, column=5, sticky=W, padx=self.padding)
-        self.next_absent_forward_btn.grid(row=1, column=6, sticky=W, padx=self.padding)
-        self.next_present_forward_btn.grid(row=1, column=7, sticky=W, padx=self.padding)
+        self.forward_btn.grid(row=1, column=5, sticky=E, padx=self.padding)
+        self.forward_max_btn.grid(row=1, column=6, sticky=W, padx=self.padding)
+        self.next_absent_forward_btn.grid(row=1, column=7, sticky=W, padx=self.padding)
+        self.next_present_forward_btn.grid(row=1, column=8, sticky=W, padx=self.padding)
 
         self.select_frm_btn.grid(row=2, column=4, sticky=N)
         self.jump_frame.grid(row=2, column=0)
         self.jump.grid(row=0, column=0, sticky=W)
         self.jump_size.grid(row=0, column=1, sticky=W)
         self.jump_back.grid(row=0, column=2, sticky=E)
         self.jump_forward.grid(row=0, column=3, sticky=W)
@@ -247,26 +249,26 @@
     def update_frame_from_video(self):
         f = open(os.path.join(os.path.dirname(self.config_path), 'labelling_info.txt'), 'r+')
         os.fsync(f.fileno())
         vid_frame_no = int(f.readline())
         self.advance_frame(new_frm_number=vid_frame_no)
         f.close()
 
-    def read_frm(self, frm_number=None):
+    def read_frm(self, frm_number: int):
         self.cap.set(1, frm_number)
         _, self.current_frm_npy = self.cap.read()
         self.current_frm_npy = cv2.cvtColor(self.current_frm_npy, cv2.COLOR_RGB2BGR)
         self.current_frm_pil = Image.fromarray(self.current_frm_npy)
         self.current_frm_pil.thumbnail(self.max_frm_size, Image.ANTIALIAS)
         self.current_frm_pil = ImageTk.PhotoImage(master=self.main_window, image=self.current_frm_pil)
         self.video_frame = Label(self.main_window, image=self.current_frm_pil)
         self.video_frame.image = self.current_frm_pil
         self.video_frame.grid(row=0, column=0)
 
-    def advance_frame(self, new_frm_number: int=None, keep_prior_img_cb_status=False):
+    def advance_frame(self, new_frm_number: int, keep_prior_img_cb_status=False):
         self.check_integrity_of_multiple_classifiers()
         if new_frm_number > self.max_frm_no:
             print("FRAME {} CANNOT BE SHOWN - YOU ARE VIEWING THE FINAL FRAME OF THE VIDEO (FRAME NUMBER {})".format(str(new_frm_number), str(self.max_frm_no)))
             self.current_frm_n = IntVar(value=self.max_frm_no)
             self.change_frm_box.delete(0, END)
             self.change_frm_box.insert(0, self.current_frm_n.get())
         elif new_frm_number < 0:
@@ -286,29 +288,29 @@
                 elif new_frame_annotation == 1:
                     self.check_present_vars[target].set(value=1)
                     self.check_absent_vars[target].set(value=0)
                 else:
                     self.check_present_vars[target].set(value=0)
                     self.check_absent_vars[target].set(value=0)
             self.change_frm_box.delete(0, END)
-            self.change_frm_box.insert(0, self.current_frm_n.get())
-            self.read_frm(frm_number=int(self.current_frm_n.get()))
+            self.change_frm_box.insert(0, new_frm_number)
+            self.read_frm(frm_number=int(new_frm_number))
         elif (new_frm_number != self.current_frm_n.get()) and (keep_prior_img_cb_status):
             self.create_print_statements()
             self.save_behavior_in_frm()
             self.current_frm_n = IntVar(value=new_frm_number)
             for target in self.target_lst:
                 new_frame_annotation = self.data_df_targets[target].loc[int(self.current_frm_n.get() -1)]
                 if new_frame_annotation == 0:
                     self.check_absent_vars[target].set(value=1)
                 elif new_frame_annotation == 1:
                     self.check_present_vars[target].set(value=1)
             self.change_frm_box.delete(0, END)
-            self.change_frm_box.insert(0, self.current_frm_n.get())
-            self.read_frm(frm_number=int(self.current_frm_n.get()))
+            self.change_frm_box.insert(0, new_frm_number)
+            self.read_frm(frm_number=int(new_frm_number))
 
     def save_behavior_in_frm(self, selection: str=None):
         for target in self.target_lst:
             target_absent_choice, target_present_choice = self.check_absent_vars[target].get(), self.check_present_vars[target].get()
             if (target_present_choice == 1) & (selection=='present'):
                 self.data_df_targets[target].loc[int(self.current_frm_n.get())] = 1
                 self.check_absent_vars[target].set(value=0)
@@ -321,14 +323,15 @@
                 self.data_df_targets[target].loc[int(self.current_frm_n.get())] = 1
             elif (target_absent_choice == 1):
                 self.data_df_targets[target].loc[int(self.current_frm_n.get())] = 0
 
     def save_behavior_in_range(self):
         self.check_integrity_of_multiple_classifiers()
         start_frm, end_frm = int(self.first_frame.get()), int(self.last_frame.get())
+        print(start_frm, end_frm)
         check_int('START FRAME', int(start_frm), max_value=self.max_frm_no, min_value=0)
         check_int('END FRAME', int(end_frm), max_value=self.max_frm_no, min_value=0)
         if not self.range_on.get():
             raise FrameRangeError(msg='TO SAVE RANGE OF FRAMES, TICK THE `Frame range` checkbox before clicking `Save Range`')
         elif start_frm < 0:
             raise FrameRangeError(msg="FRAME RANGE ERROR: START FRAME {} IS LESS THAN ZERO AND CANNOT BE SHOWN".format(str(start_frm)))
         elif end_frm > self.max_frm_no:
@@ -353,15 +356,18 @@
             self.create_print_statements(frame_range=True, start_frame=start_frm, end_frame=end_frm)
 
     def save_results(self):
         self.save_df = read_df(self.features_extracted_file_path, self.file_type)
         self.save_df = pd.concat([self.save_df, self.data_df_targets], axis=1)
         self.save_df = self.save_df.dropna(subset=self.target_lst)
         try:
-            write_df(self.save_df, self.file_type, self.targets_inserted_file_path)
+            if self.file_type == Formats.CSV.value:
+                self.save_df.to_csv(self.targets_inserted_file_path)
+            if self.file_type == Formats.PARQUET.value:
+                self.save_df.to_parquet(self.targets_inserted_file_path)
         except Exception as e:
             print(e, 'SIMBA ERROR: File for video {} could not be saved.')
             raise FileExistsError
         stdout_success(msg=f'SAVED: Annotation file for video {self.video_name} saved within the project_folder/csv/targets_inserted directory.')
         if not self.config.has_section('Last annotated frames'):
             self.config.add_section('Last annotated frames')
         self.config.set('Last annotated frames', str(self.video_name), str(self.current_frm_n.get()))
```

### Comparing `Simba-UW-tf-dev-1.60.7/simba/labelling/play_annotation_video.py` & `Simba-UW-tf-dev-1.60.9/simba/labelling/play_annotation_video.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.60.7/simba/unsupervised/dbcv_calculator.py` & `Simba-UW-tf-dev-1.60.9/simba/unsupervised/dbcv_calculator.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.60.7/simba/unsupervised/enums.py` & `Simba-UW-tf-dev-1.60.9/simba/unsupervised/enums.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.60.7/simba/unsupervised/.DS_Store` & `Simba-UW-tf-dev-1.60.9/simba/unsupervised/.DS_Store`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.60.7/simba/unsupervised/dataset_creator.py` & `Simba-UW-tf-dev-1.60.9/simba/unsupervised/dataset_creator.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.60.7/simba/unsupervised/grid_search_visualizers.py` & `Simba-UW-tf-dev-1.60.9/simba/unsupervised/grid_search_visualizers.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.60.7/simba/unsupervised/data_extractor.py` & `Simba-UW-tf-dev-1.60.9/simba/unsupervised/data_extractor.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.60.7/simba/unsupervised/ui.py` & `Simba-UW-tf-dev-1.60.9/simba/unsupervised/ui.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.60.7/simba/unsupervised/umap_embedder.py` & `Simba-UW-tf-dev-1.60.9/simba/unsupervised/umap_embedder.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.60.7/simba/unsupervised/pop_up_classes.py` & `Simba-UW-tf-dev-1.60.9/simba/unsupervised/pop_up_classes.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.60.7/simba/unsupervised/bout_aggregator.py` & `Simba-UW-tf-dev-1.60.9/simba/unsupervised/bout_aggregator.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.60.7/simba/unsupervised/cluster_statistics.py` & `Simba-UW-tf-dev-1.60.9/simba/unsupervised/cluster_statistics.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.60.7/simba/unsupervised/data_map.yaml` & `Simba-UW-tf-dev-1.60.9/simba/unsupervised/data_map.yaml`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.60.7/simba/unsupervised/hdbscan_clusterer.py` & `Simba-UW-tf-dev-1.60.9/simba/unsupervised/hdbscan_clusterer.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.60.7/simba/unsupervised/tsne.py` & `Simba-UW-tf-dev-1.60.9/simba/unsupervised/tsne.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.60.7/simba/unsupervised/cluster_visualizer.py` & `Simba-UW-tf-dev-1.60.9/simba/unsupervised/cluster_visualizer.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.60.7/simba/bounding_box_tools/.DS_Store` & `Simba-UW-tf-dev-1.60.9/simba/bounding_box_tools/.DS_Store`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.60.7/simba/bounding_box_tools/agg_boundary_stats.py` & `Simba-UW-tf-dev-1.60.9/simba/bounding_box_tools/agg_boundary_stats.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.60.7/simba/bounding_box_tools/boundary_menus.py` & `Simba-UW-tf-dev-1.60.9/simba/bounding_box_tools/boundary_menus.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.60.7/simba/bounding_box_tools/boundary_statistics.py` & `Simba-UW-tf-dev-1.60.9/simba/bounding_box_tools/boundary_statistics.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.60.7/simba/bounding_box_tools/find_boundaries.py` & `Simba-UW-tf-dev-1.60.9/simba/bounding_box_tools/find_boundaries.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.60.7/simba/bounding_box_tools/visualize_boundaries.py` & `Simba-UW-tf-dev-1.60.9/simba/bounding_box_tools/visualize_boundaries.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.60.7/simba/.DS_Store` & `Simba-UW-tf-dev-1.60.9/simba/.DS_Store`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.60.7/simba/feature_extractors/feature_extractor_14bp.py` & `Simba-UW-tf-dev-1.60.9/simba/feature_extractors/feature_extractor_14bp.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.60.7/simba/feature_extractors/feature_extractor_7bp.py` & `Simba-UW-tf-dev-1.60.9/simba/feature_extractors/feature_extractor_7bp.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.60.7/simba/feature_extractors/misc/doctests.py` & `Simba-UW-tf-dev-1.60.9/simba/feature_extractors/misc/doctests.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.60.7/simba/feature_extractors/misc/fish_feature_extractor_2023_version_3.py` & `Simba-UW-tf-dev-1.60.9/simba/feature_extractors/misc/fish_feature_extractor_2023_version_3.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.60.7/simba/feature_extractors/misc/read_in_mp.py` & `Simba-UW-tf-dev-1.60.9/simba/feature_extractors/misc/read_in_mp.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.60.7/simba/feature_extractors/misc/peaks.py` & `Simba-UW-tf-dev-1.60.9/simba/feature_extractors/misc/peaks.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.60.7/simba/feature_extractors/misc/fish_feature_extractor_2022.py` & `Simba-UW-tf-dev-1.60.9/simba/feature_extractors/misc/fish_feature_extractor_2022.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.60.7/simba/feature_extractors/misc/convex_hull_3_scratch_3.py` & `Simba-UW-tf-dev-1.60.9/simba/feature_extractors/misc/convex_hull_3_scratch_3.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.60.7/simba/feature_extractors/misc/convex_hull_scratch_1.py` & `Simba-UW-tf-dev-1.60.9/simba/feature_extractors/misc/convex_hull_scratch_1.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.60.7/simba/feature_extractors/misc/.DS_Store` & `Simba-UW-tf-dev-1.60.9/simba/feature_extractors/misc/.DS_Store`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.60.7/simba/feature_extractors/misc/fish_feature_extractor_2023_version_2.py` & `Simba-UW-tf-dev-1.60.9/simba/feature_extractors/misc/fish_feature_extractor_2023_version_2.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.60.7/simba/feature_extractors/misc/egocentrical_aligner.py` & `Simba-UW-tf-dev-1.60.9/simba/feature_extractors/misc/egocentrical_aligner.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.60.7/simba/feature_extractors/misc/count_values_in_range.py` & `Simba-UW-tf-dev-1.60.9/simba/feature_extractors/misc/count_values_in_range.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.60.7/simba/feature_extractors/misc/graph_creator.py` & `Simba-UW-tf-dev-1.60.9/simba/feature_extractors/misc/graph_creator.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.60.7/simba/feature_extractors/misc/termite_rois.csv` & `Simba-UW-tf-dev-1.60.9/simba/feature_extractors/misc/termite_rois.csv`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.60.7/simba/feature_extractors/misc/mutual_exclusive.py` & `Simba-UW-tf-dev-1.60.9/simba/feature_extractors/misc/mutual_exclusive.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.60.7/simba/feature_extractors/misc/video_color.py` & `Simba-UW-tf-dev-1.60.9/simba/feature_extractors/misc/video_color.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.60.7/simba/feature_extractors/misc/graph_3d_plotter.py` & `Simba-UW-tf-dev-1.60.9/simba/feature_extractors/misc/graph_3d_plotter.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.60.7/simba/feature_extractors/misc/video_rotator.py` & `Simba-UW-tf-dev-1.60.9/simba/feature_extractors/misc/video_rotator.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.60.7/simba/feature_extractors/misc/add_probability_cnt_features.py` & `Simba-UW-tf-dev-1.60.9/simba/feature_extractors/misc/add_probability_cnt_features.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.60.7/simba/feature_extractors/misc/make_splash.py` & `Simba-UW-tf-dev-1.60.9/simba/feature_extractors/misc/make_splash.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.60.7/simba/feature_extractors/misc/fish_feature_extractor_2023_version_5.py` & `Simba-UW-tf-dev-1.60.9/simba/feature_extractors/misc/fish_feature_extractor_2023_version_5.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.60.7/simba/feature_extractors/misc/time_stamp_calculator.py` & `Simba-UW-tf-dev-1.60.9/simba/feature_extractors/misc/time_stamp_calculator.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.60.7/simba/feature_extractors/misc/video_rotator_mp.py` & `Simba-UW-tf-dev-1.60.9/simba/feature_extractors/misc/video_rotator_mp.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.60.7/simba/feature_extractors/misc/fish_feature_extractor_2023_version_4.py` & `Simba-UW-tf-dev-1.60.9/simba/feature_extractors/misc/fish_feature_extractor_2023_version_4.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.60.7/simba/feature_extractors/misc/convex_hull_scratch_2.py` & `Simba-UW-tf-dev-1.60.9/simba/feature_extractors/misc/convex_hull_scratch_2.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.60.7/simba/feature_extractors/feature_extractor_8bps_2_animals.py` & `Simba-UW-tf-dev-1.60.9/simba/feature_extractors/feature_extractor_8bps_2_animals.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.60.7/simba/feature_extractors/.DS_Store` & `Simba-UW-tf-dev-1.60.9/simba/feature_extractors/.DS_Store`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.60.7/simba/feature_extractors/perimeter_jit.py` & `Simba-UW-tf-dev-1.60.9/simba/feature_extractors/perimeter_jit.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.60.7/simba/feature_extractors/feature_subsets.py` & `Simba-UW-tf-dev-1.60.9/simba/feature_extractors/feature_subsets.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.60.7/simba/feature_extractors/feature_extractor_user_defined.py` & `Simba-UW-tf-dev-1.60.9/simba/feature_extractors/feature_extractor_user_defined.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.60.7/simba/feature_extractors/feature_extractor_16bp.py` & `Simba-UW-tf-dev-1.60.9/simba/feature_extractors/feature_extractor_16bp.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.60.7/simba/feature_extractors/feature_extractor_9bp.py` & `Simba-UW-tf-dev-1.60.9/simba/feature_extractors/feature_extractor_9bp.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.60.7/simba/feature_extractors/feature_extractor_8bp.py` & `Simba-UW-tf-dev-1.60.9/simba/feature_extractors/feature_extractor_8bp.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.60.7/simba/feature_extractors/feature_extractor_4bp.py` & `Simba-UW-tf-dev-1.60.9/simba/feature_extractors/feature_extractor_4bp.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.60.7/simba/feature_extractors/.idea/features_scripts.iml` & `Simba-UW-tf-dev-1.60.9/simba/feature_extractors/.idea/features_scripts.iml`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.60.7/simba/feature_extractors/.idea/inspectionProfiles/Project_Default.xml` & `Simba-UW-tf-dev-1.60.9/simba/feature_extractors/.idea/inspectionProfiles/Project_Default.xml`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.60.7/simba/feature_extractors/.idea/workspace.xml` & `Simba-UW-tf-dev-1.60.9/simba/feature_extractors/.idea/workspace.xml`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.60.7/simba/requirements.txt` & `Simba-UW-tf-dev-1.60.9/simba/requirements.txt`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.60.7/simba/mixins/.DS_Store` & `Simba-UW-tf-dev-1.60.9/simba/mixins/.DS_Store`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.60.7/simba/mixins/pop_up_mixin.py` & `Simba-UW-tf-dev-1.60.9/simba/mixins/pop_up_mixin.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.60.7/simba/mixins/config_reader.py` & `Simba-UW-tf-dev-1.60.9/simba/mixins/config_reader.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.60.7/simba/mixins/pose_importer_mixin.py` & `Simba-UW-tf-dev-1.60.9/simba/mixins/pose_importer_mixin.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.60.7/simba/mixins/__pycache__/feature_extraction_mixin.FeatureExtractionMixin.cdist-333.py36m.nbi` & `Simba-UW-tf-dev-1.60.9/simba/mixins/__pycache__/feature_extraction_mixin.FeatureExtractionMixin.cdist-333.py36m.nbi`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.60.7/simba/mixins/__pycache__/feature_extraction_mixin.FeatureExtractionMixin.angle3pt-84.py36m.nbi` & `Simba-UW-tf-dev-1.60.9/simba/mixins/__pycache__/feature_extraction_mixin.FeatureExtractionMixin.angle3pt-84.py36m.nbi`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.60.7/simba/mixins/__pycache__/feature_extraction_mixin.FeatureExtractionMixin.cdist-333.py36m.1.nbc` & `Simba-UW-tf-dev-1.60.9/simba/mixins/__pycache__/feature_extraction_mixin.FeatureExtractionMixin.cdist-333.py36m.1.nbc`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.60.7/simba/mixins/__pycache__/feature_extraction_mixin.FeatureExtractionMixin.angle3pt-84.py36m.1.nbc` & `Simba-UW-tf-dev-1.60.9/simba/mixins/__pycache__/feature_extraction_mixin.FeatureExtractionMixin.angle3pt-84.py36m.1.nbc`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.60.7/simba/mixins/feature_extraction_mixin.py` & `Simba-UW-tf-dev-1.60.9/simba/mixins/feature_extraction_mixin.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.60.7/simba/mixins/plotting_mixin.py` & `Simba-UW-tf-dev-1.60.9/simba/mixins/plotting_mixin.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.60.7/simba/mixins/unsupervised_mixin.py` & `Simba-UW-tf-dev-1.60.9/simba/mixins/unsupervised_mixin.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.60.7/simba/mixins/train_model_mixin.py` & `Simba-UW-tf-dev-1.60.9/simba/mixins/train_model_mixin.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.60.7/simba/third_party_label_appenders/deepethogram_importer.py` & `Simba-UW-tf-dev-1.60.9/simba/third_party_label_appenders/deepethogram_importer.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.60.7/simba/third_party_label_appenders/BORIS_appender.py` & `Simba-UW-tf-dev-1.60.9/simba/third_party_label_appenders/BORIS_appender.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.60.7/simba/third_party_label_appenders/observer_importer.py` & `Simba-UW-tf-dev-1.60.9/simba/third_party_label_appenders/observer_importer.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.60.7/simba/third_party_label_appenders/tools.py` & `Simba-UW-tf-dev-1.60.9/simba/third_party_label_appenders/tools.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.60.7/simba/third_party_label_appenders/third_party_appender.py` & `Simba-UW-tf-dev-1.60.9/simba/third_party_label_appenders/third_party_appender.py`

 * *Files 1% similar despite different names*

```diff
@@ -224,23 +224,23 @@
                 out_df.loc[annot_idx, clf] = 1
             save_path = os.path.join(self.targets_folder, self.video_name + '.' + self.file_type)
             write_df(out_df, self.file_type, save_path)
             print(f'Saved {self.app} annotations for video {self.video_name}...')
         self.timer.stop_timer()
         stdout_success(msg=f'{self.app} annotations appended to dataset and saved in project_folder/csv/targets_inserted directory', elapsed_time=self.timer.elapsed_time_str)
 
-# settings = {'log': True,  'file_format': 'xlsx', 'errors': {'INVALID annotations file data format': 'WARNING',
-#                                                            'ADDITIONAL third-party behavior detected': 'NONE',
-#                                                            'Annotations EVENT COUNT conflict': 'WARNING',
-#                                                            'Annotations OVERLAP inaccuracy': 'WARNING',
-#                                                            'ZERO third-party video behavior annotations found': 'WARNING',
-#                                                            'Annotations and pose FRAME COUNT conflict': 'WARNING',
-#                                                            'Annotations data file NOT FOUND': 'WARNING'}}
-# #
-#
+settings = {'log': True,  'file_format': 'csv', 'errors': {'INVALID annotations file data format': 'WARNING',
+                                                           'ADDITIONAL third-party behavior detected': 'NONE',
+                                                           'Annotations EVENT COUNT conflict': 'WARNING',
+                                                           'Annotations OVERLAP inaccuracy': 'WARNING',
+                                                           'ZERO third-party video behavior annotations found': 'WARNING',
+                                                           'Annotations and pose FRAME COUNT conflict': 'WARNING',
+                                                           'Annotations data file NOT FOUND': 'WARNING'}}
+
+
 #
 # test = ThirdPartyLabelAppender(config_path='/Users/simon/Desktop/envs/troubleshooting/two_black_animals_14bp/project_folder/project_config.ini',
 #                                data_dir='/Users/simon/Downloads/FIXED',
 #                                settings=settings,
 #                                app='BORIS')
 # test.run()
 
@@ -253,20 +253,20 @@
 
 
 # test = ThirdPartyLabelAppender(config_path='/Users/simon/Desktop/envs/troubleshooting/two_black_animals_14bp/project_folder/project_config.ini',
 #                                data_dir=r'/Users/simon/Desktop/envs/simba_dev/tests/test_data/import_tests/ethovision_data',
 #                                settings=settings,
 #                                app='ETHOVISION')
 # test.run()
-
+#
 # test = ThirdPartyLabelAppender(config_path='/Users/simon/Desktop/envs/troubleshooting/two_black_animals_14bp/project_folder/project_config.ini',
-#                                data_dir=r'/Users/simon/Desktop/envs/simba_dev/tests/test_data/solomon_import/solomon_import',
+#                                data_dir=r'/Users/simon/Desktop/envs/simba_dev/old_tests/test_data/solomon_import/solomon_import',
 #                                settings=settings,
 #                                app='SOLOMON')
 # test.run()
 
 
 # test = ThirdPartyLabelAppender(config_path='/Users/simon/Desktop/envs/troubleshooting/two_black_animals_14bp/project_folder/project_config.ini',
-#                                data_dir=r'/Users/simon/Desktop/envs/simba_dev/tests/test_data/bento_example',
+#                                data_dir=r'/Users/simon/Desktop/envs/simba_dev/old_tests/test_data/bento_example',
 #                                settings=settings,
 #                                app='BENTO')
 # test.run()
```

### Comparing `Simba-UW-tf-dev-1.60.7/simba/third_party_label_appenders/ethovision_import.py` & `Simba-UW-tf-dev-1.60.9/simba/third_party_label_appenders/ethovision_import.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.60.7/simba/third_party_label_appenders/BENTO_appender.py` & `Simba-UW-tf-dev-1.60.9/simba/third_party_label_appenders/BENTO_appender.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.60.7/simba/third_party_label_appenders/solomon_importer.py` & `Simba-UW-tf-dev-1.60.9/simba/third_party_label_appenders/solomon_importer.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.60.7/simba/cue_light_tools/.DS_Store` & `Simba-UW-tf-dev-1.60.9/simba/cue_light_tools/.DS_Store`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.60.7/simba/cue_light_tools/cue_light_clf_statistics.py` & `Simba-UW-tf-dev-1.60.9/simba/cue_light_tools/cue_light_clf_statistics.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.60.7/simba/cue_light_tools/cue_light_analyzer.py` & `Simba-UW-tf-dev-1.60.9/simba/cue_light_tools/cue_light_analyzer.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.60.7/simba/cue_light_tools/cue_light_menues.py` & `Simba-UW-tf-dev-1.60.9/simba/cue_light_tools/cue_light_menues.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.60.7/simba/cue_light_tools/cue_light_tools.py` & `Simba-UW-tf-dev-1.60.9/simba/cue_light_tools/cue_light_tools.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.60.7/simba/cue_light_tools/cue_light_visualizer.py` & `Simba-UW-tf-dev-1.60.9/simba/cue_light_tools/cue_light_visualizer.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.60.7/simba/cue_light_tools/cue_light_movement_statistics.py` & `Simba-UW-tf-dev-1.60.9/simba/cue_light_tools/cue_light_movement_statistics.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.60.7/simba/utils/config_creator.py` & `Simba-UW-tf-dev-1.60.9/simba/utils/config_creator.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.60.7/simba/utils/enums.py` & `Simba-UW-tf-dev-1.60.9/simba/utils/enums.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.60.7/simba/utils/.DS_Store` & `Simba-UW-tf-dev-1.60.9/simba/utils/.DS_Store`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.60.7/simba/utils/warnings.py` & `Simba-UW-tf-dev-1.60.9/simba/utils/warnings.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.60.7/simba/utils/checks.py` & `Simba-UW-tf-dev-1.60.9/simba/utils/checks.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.60.7/simba/utils/read_write.py` & `Simba-UW-tf-dev-1.60.9/simba/utils/read_write.py`

 * *Files 0% similar despite different names*

```diff
@@ -239,15 +239,15 @@
                                      data_type=ConfigKey.FOLDER_PATH.value)
     file_type = read_config_entry(config=config,
                                   section=ConfigKey.GENERAL_SETTINGS.value,
                                   option=ConfigKey.FILE_TYPE.value,
                                   data_type=Dtypes.STR.value,
                                   default_value=Formats.CSV.value)
 
-    return project_path, file_type
+    return project_path.strip(), file_type.strip()
 
 
 def read_video_info_csv(file_path: Union[str, os.PathLike]) -> pd.DataFrame:
 
     """
     Read the project_folder/logs/video_info.csv of the SimBA project as a pd.DataFrame
```

### Comparing `Simba-UW-tf-dev-1.60.7/simba/utils/lookups.py` & `Simba-UW-tf-dev-1.60.9/simba/utils/lookups.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.60.7/simba/utils/cli/cli_tools.py` & `Simba-UW-tf-dev-1.60.9/simba/utils/cli/cli_tools.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.60.7/simba/utils/errors.py` & `Simba-UW-tf-dev-1.60.9/simba/utils/errors.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.60.7/simba/utils/data.py` & `Simba-UW-tf-dev-1.60.9/simba/utils/data.py`

 * *Files 15% similar despite different names*

```diff
@@ -5,15 +5,19 @@
 import pandas as pd
 from copy import deepcopy
 import configparser
 from pathlib import Path
 import ast
 from scipy.signal import savgol_filter
 from pylab import *
-from typing import List, Optional, Union
+from typing import List, Optional, Union, Dict
+try:
+    from typing import Literal
+except:
+    from typing_extensions import Literal
 
 from simba.utils.read_write import (get_fn_ext,
                                     read_project_path_and_file_type,
                                     find_video_of_file,
                                     read_df,
                                     write_df,
                                     read_config_file,
@@ -51,17 +55,17 @@
         v = (data_df[target_name] != data_df[target_name].shift()).cumsum()
         u = data_df.groupby(v)[target_name].agg(['all', 'count'])
         m = u['all'] & u['count'].ge(1)
         groupDf['groups'] = data_df.groupby(v).apply(lambda x: (x.index[0], x.index[-1]))[m]
         for _, row in groupDf.iterrows():
             bout = list(row['groups'])
             bout_time = ((bout[-1] - bout[0]) + 1) / fps
-            bout_start = (bout[0] + 1) / fps
-            bout_end = (bout[1]) / fps
-            bout_start_frm = bout[0] + 1
+            bout_start = (bout[0]) / fps
+            bout_end = (bout[1] + 1) / fps
+            bout_start_frm = bout[0]
             endFrame = (bout[1])
             endTimeList.append(bout_end)
             startTimeList.append(bout_start)
             boutsList.append(bout_time)
             nameList.append(target_name)
             endFrameList.append(endFrame)
             startFrameLst.append(bout_start_frm)
@@ -312,14 +316,63 @@
     if not 'Thickness' in shape_df.columns:
         shape_df['Thickness'] = [5] * len(shape_df)
     if not 'Color name' in shape_df.columns:
         shape_df['Color name'] = 'White'
 
     return shape_df
 
+def find_bins(data: Dict[str, List[int]],
+              bracket_type: Literal['QUANTILE', 'QUANTIZE'],
+              bracket_cnt: int,
+              normalization_method: Literal['ALL VIDEOS', 'BY VIDEO']) -> Dict[str, np.ndarray]:
+
+    """
+    Helper to find bin cut-off points.
+
+    :param dict data: Dictionary with video names as keys and list of values of size len(frames).
+    :param Literal[str] bracket_type: 'QUANTILE' or 'QUANTIZE'
+    :param str bracket_cnt: Number of bins.
+    :param str normalization_method: Create bins based on data in all videos ("ALL VIDEOS") or create different bins per video ('BY VIDEO')
+    :returns dict: The videos as keys and bin cut off points as array of size len(bracket_cnt) x 2.
+    """
+
+    print('Finding bracket cut off points...')
+    video_bins_info = {}
+    if normalization_method == 'ALL VIDEOS':
+        m = []
+        [m.extend((d.tolist())) for d in data.values()]
+        if bracket_type == 'QUANTILE':
+            _, bins = pd.qcut(x=m, q=bracket_cnt, labels=list(range(1, bracket_cnt + 1)), retbins=True)
+        else:
+            _, bins = pd.cut(x=m, bins=bracket_cnt, labels=list(range(1, bracket_cnt + 1)), retbins=True)
+        bins = bins.clip(min=0)
+        for video_name, video_movements in data.items():
+            bin_array = np.full((len(bins) - 1, 2), np.nan)
+            for i in range(len(bins) - 1):
+                bin_array[i] = [bins[i].astype(int), bins[i + 1].astype(int)]
+            video_bins_info[video_name] = bin_array
+    else:
+        for video_name, video_movements in data.items():
+            if bracket_type == 'QUANTILE':
+                _, bins = pd.qcut(x=video_movements, q=bracket_cnt, labels=list(range(1, bracket_cnt + 1)),
+                                  retbins=True)
+            else:
+                _, bins = pd.cut(x=video_movements, bins=bracket_cnt, labels=list(range(1, bracket_cnt + 1)),
+                                 retbins=True)
+            bins = bins.clip(min=0)
+            bin_array = np.full((len(bins) - 1, 2), np.nan)
+            for i in range(len(bins) - 1):
+                bin_array[i] = [bins[i].astype(int), bins[i + 1].astype(int)]
+            video_bins_info[video_name] = bin_array
+
+    return video_bins_info
+
+
+
+
 def run_user_defined_feature_extraction_class(file_path: Union[str, os.PathLike],
                                               config_path: Union[str, os.PathLike]) -> None:
     """
     Loads and executes user-defined feature extraction class.
 
     :param file_path: Path to .py file holding user-defined feature extraction class
     :param str config_path: Path to SimBA project config file.
```

### Comparing `Simba-UW-tf-dev-1.60.7/simba/utils/printing.py` & `Simba-UW-tf-dev-1.60.9/simba/utils/printing.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.60.7/simba/pose_processors/reorganize_keypoint.py` & `Simba-UW-tf-dev-1.60.9/simba/pose_processors/reorganize_keypoint.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.60.7/simba/pose_processors/remove_keypoints.py` & `Simba-UW-tf-dev-1.60.9/simba/pose_processors/remove_keypoints.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.60.7/simba/pose_processors/pose_reset.py` & `Simba-UW-tf-dev-1.60.9/simba/pose_processors/pose_reset.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.60.7/simba/pose_processors/reverse_pose.py` & `Simba-UW-tf-dev-1.60.9/simba/pose_processors/reverse_pose.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.60.7/simba/plotting/gantt_creator.py` & `Simba-UW-tf-dev-1.60.9/simba/plotting/gantt_creator.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.60.7/simba/plotting/tools/tkinter_tools.py` & `Simba-UW-tf-dev-1.60.9/simba/plotting/tools/tkinter_tools.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.60.7/simba/plotting/ROI_plotter_mp.py` & `Simba-UW-tf-dev-1.60.9/simba/plotting/ROI_plotter_mp.py`

 * *Files 2% similar despite different names*

```diff
@@ -33,15 +33,14 @@
 
     .. notes::
        `ROI tutorials <https://github.com/sgoldenlab/simba/blob/master/docs/ROI_tutorial_new.md>`__.
 
     Examples
     ----------
     >>> roi_visualizer = ROIPlotMultiprocess(ini_path=r'MyProjectConfig', video_path="MyVideo.mp4")
-    >>> roi_visualizer.insert_data()
     >>> roi_visualizer.run()
     """
 
     def __init__(
             self,
             ini_path: str,
             video_path: str,
@@ -111,16 +110,14 @@
                 self.loc_dict[animal_name][shape]['timer_text_loc'] = ((self.video_meta_data['width'] + 5), (self.video_meta_data['height'] - (self.video_meta_data['height'] + 10) + self.scalers['space_size'] * add_spacer))
                 self.loc_dict[animal_name][shape]['timer_data_loc'] = (int(self.border_img_w-(self.border_img_w/8)), (self.video_meta_data['height'] - (self.video_meta_data['height'] + 10) + self.scalers['space_size']*add_spacer))
                 add_spacer += 1
                 self.loc_dict[animal_name][shape]['entries_text_loc'] = ((self.video_meta_data['width'] + 5), (self.video_meta_data['height'] - (self.video_meta_data['height'] + 10) + self.scalers['space_size'] * add_spacer))
                 self.loc_dict[animal_name][shape]['entries_data_loc'] = (int(self.border_img_w - (self.border_img_w / 8)), (self.video_meta_data['height'] - (self.video_meta_data['height'] + 10) + self.scalers['space_size'] * add_spacer))
                 add_spacer += 1
 
-
-
     def __create_counters(self):
         self.cnt_dict = {}
         for animal_cnt, animal_name in enumerate(self.roi_analyzer.multi_animal_id_list):
             self.cnt_dict[animal_name] = {}
             for shape in self.video_shapes:
                 self.cnt_dict[animal_name][shape] = {}
                 self.cnt_dict[animal_name][shape]['timer'] = 0
@@ -152,16 +149,15 @@
         directory of the SimBA project.
 
         Returns
         -------
         None
         """
 
-        video_timer = SimbaTimer()
-        video_timer.start_timer()
+        video_timer = SimbaTimer(start=True)
         self.cap = cv2.VideoCapture(self.video_path)
         self.video_meta_data = get_video_meta_data(self.video_path)
         video_settings, pix_per_mm, self.fps = self.read_video_info(video_name=self.video_name)
         self.space_scale, radius_scale, res_scale, font_scale = 25, 10, 1500, 0.8
         max_dim = max(self.video_meta_data['width'], self.video_meta_data['height'])
         self.scalers = {}
         self.scalers['circle_size'], self.scalers['font_size'] = int(radius_scale / (res_scale / max_dim)), float(font_scale / (res_scale / max_dim))
@@ -197,31 +193,28 @@
                 print('Image {}/{}, Video {}...'.format(str(int(frm_per_core * (result + 1))), str(len(self.data_df)), self.video_name))
             print('Joining {} multi-processed video...'.format(self.video_name))
             concatenate_videos_in_folder(in_folder=self.temp_folder, save_path=self.video_save_path, video_format='mp4')
 
             video_timer.stop_timer()
             pool.terminate()
             pool.join()
-
             stdout_success(msg=f'Video {self.video_name} created. Video saved in project_folder/frames/output/ROI_analysis', elapsed_time=video_timer.elapsed_time_str)
 
 # test = ROIPlotMultiprocess(ini_path=r'/Users/simon/Desktop/envs/troubleshooting/Termites_5/project_folder/project_config.ini',
 #                video_path="termite_test.mp4",
 #                core_cnt=5,
 #                style_attr={'Show_body_part': True, 'Show_animal_name': True})
-# test.insert_data()
-# test.visualize_ROI_data()
+# test.run()
 
 # test = ROIPlot(ini_path=r'/Users/simon/Desktop/troubleshooting/train_model_project/project_folder/project_config.ini', video_path=r"Together_1.avi")
 # test.insert_data()
 # test.visualize_ROI_data()
 
 # test = ROIPlot(ini_path=r"Z:\DeepLabCut\DLC_extract\Troubleshooting\ROI_2_animals\project_folder\project_config.ini", video_path=r"Z:\DeepLabCut\DLC_extract\Troubleshooting\ROI_2_animals\project_folder\videos\Video7.mp4")
 # test.insert_data()
 # test.visualize_ROI_data()
 
 # test = ROIPlotMultiprocess(ini_path=r'/Users/simon/Desktop/envs/troubleshooting/two_black_animals_14bp/project_folder/project_config.ini',
 #                video_path="Together_2.avi",
 #                style_attr={'Show_body_part': True, 'Show_animal_name': False},
 #                            core_cnt=5)
-# test.insert_data()
-# test.visualize_ROI_data()
+# test.run()
```

### Comparing `Simba-UW-tf-dev-1.60.7/simba/plotting/.DS_Store` & `Simba-UW-tf-dev-1.60.9/simba/plotting/.DS_Store`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.60.7/simba/plotting/shap_agg_stats_visualizer.py` & `Simba-UW-tf-dev-1.60.9/simba/plotting/shap_agg_stats_visualizer.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.60.7/simba/plotting/gantt_creator_mp.py` & `Simba-UW-tf-dev-1.60.9/simba/plotting/gantt_creator_mp.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.60.7/simba/plotting/heat_mapper_clf_mp.py` & `Simba-UW-tf-dev-1.60.9/simba/plotting/heat_mapper_clf_mp.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.60.7/simba/plotting/probability_plot_creator.py` & `Simba-UW-tf-dev-1.60.9/simba/plotting/probability_plot_creator.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.60.7/simba/plotting/plot_clf_results.py` & `Simba-UW-tf-dev-1.60.9/simba/plotting/plot_clf_results.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.60.7/simba/plotting/plot_clf_results_mp.py` & `Simba-UW-tf-dev-1.60.9/simba/plotting/plot_clf_results_mp.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.60.7/simba/plotting/ROI_feature_visualizer.py` & `Simba-UW-tf-dev-1.60.9/simba/plotting/ROI_feature_visualizer.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.60.7/simba/plotting/heat_mapper_location.py` & `Simba-UW-tf-dev-1.60.9/simba/plotting/heat_mapper_location.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.60.7/simba/plotting/probability_plot_creator_mp.py` & `Simba-UW-tf-dev-1.60.9/simba/plotting/probability_plot_creator_mp.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.60.7/simba/plotting/interactive_probability_grapher.py` & `Simba-UW-tf-dev-1.60.9/simba/plotting/interactive_probability_grapher.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.60.7/simba/plotting/plot_pose_in_dir.py` & `Simba-UW-tf-dev-1.60.9/simba/plotting/plot_pose_in_dir.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.60.7/simba/plotting/single_run_model_validation_video.py` & `Simba-UW-tf-dev-1.60.9/simba/plotting/single_run_model_validation_video.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.60.7/simba/plotting/frame_mergerer_ffmpeg.py` & `Simba-UW-tf-dev-1.60.9/simba/plotting/frame_mergerer_ffmpeg.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.60.7/simba/plotting/Directing_animals_visualizer_mp.py` & `Simba-UW-tf-dev-1.60.9/simba/plotting/Directing_animals_visualizer_mp.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.60.7/simba/plotting/clf_validator.py` & `Simba-UW-tf-dev-1.60.9/simba/plotting/clf_validator.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.60.7/simba/plotting/path_plotter_mp.py` & `Simba-UW-tf-dev-1.60.9/simba/plotting/path_plotter_mp.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.60.7/simba/plotting/ROI_feature_visualizer_mp.py` & `Simba-UW-tf-dev-1.60.9/simba/plotting/ROI_feature_visualizer_mp.py`

 * *Files 0% similar despite different names*

```diff
@@ -143,15 +143,14 @@
                                           tracked_bps=self.bp_names,
                                           animal_bps=self.animal_bp_dict)
             for cnt, result in enumerate(pool.imap(constants, data_arr, chunksize=self.multiprocess_chunksize)):
                 print('Image {}/{}, Video {}...'.format(str(int(frm_per_core * (result + 1))), str(len(self.data_df)), self.video_name))
 
             print('Joining {} multiprocessed video...'.format(self.video_name))
             concatenate_videos_in_folder(in_folder=self.save_temp_dir, save_path=self.save_path, video_format='mp4')
-
             self.timer.stop_timer()
             pool.terminate()
             pool.join()
             stdout_success(msg=f'Video {self.video_name} complete. Video saved in project_folder/frames/output/ROI_features.', elapsed_time=self.timer.elapsed_time_str)
 
 # style_attr = {'ROI_centers': True,
 #               'ROI_ear_tags': True,
```

### Comparing `Simba-UW-tf-dev-1.60.7/simba/plotting/data_plotter.py` & `Simba-UW-tf-dev-1.60.9/simba/plotting/data_plotter.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.60.7/simba/plotting/path_plotter.py` & `Simba-UW-tf-dev-1.60.9/simba/plotting/path_plotter.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.60.7/simba/plotting/ez_lineplot.py` & `Simba-UW-tf-dev-1.60.9/simba/plotting/ez_lineplot.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.60.7/simba/plotting/distance_plotter_mp.py` & `Simba-UW-tf-dev-1.60.9/simba/plotting/distance_plotter_mp.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.60.7/simba/plotting/ROI_plotter.py` & `Simba-UW-tf-dev-1.60.9/simba/plotting/ROI_plotter.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.60.7/simba/plotting/heat_mapper_clf.py` & `Simba-UW-tf-dev-1.60.9/simba/plotting/heat_mapper_clf.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.60.7/simba/plotting/distance_plotter.py` & `Simba-UW-tf-dev-1.60.9/simba/plotting/distance_plotter.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.60.7/simba/plotting/single_run_model_validation_video_mp.py` & `Simba-UW-tf-dev-1.60.9/simba/plotting/single_run_model_validation_video_mp.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.60.7/simba/plotting/Directing_animals_visualizer.py` & `Simba-UW-tf-dev-1.60.9/simba/plotting/Directing_animals_visualizer.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.60.7/simba/plotting/heat_mapper_location_mp.py` & `Simba-UW-tf-dev-1.60.9/simba/plotting/heat_mapper_location_mp.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.60.7/simba/dash_app/SimBA_dash_app.py` & `Simba-UW-tf-dev-1.60.9/simba/dash_app/SimBA_dash_app.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.60.7/simba/dash_app/run_dash_tkinter.py` & `Simba-UW-tf-dev-1.60.9/simba/dash_app/run_dash_tkinter.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.60.7/simba/dash_app/dash_app.py` & `Simba-UW-tf-dev-1.60.9/simba/dash_app/dash_app.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.60.7/simba/data_processors/agg_clf_calculator.py` & `Simba-UW-tf-dev-1.60.9/simba/data_processors/agg_clf_calculator.py`

 * *Files 1% similar despite different names*

```diff
@@ -25,15 +25,15 @@
     :parameter List[str] classifiers: Classifiers to calculate aggregate statistics for. E.g.,: ['Attack', 'Sniffing']
 
     .. note::
        `GitHub tutorial <https://github.com/sgoldenlab/simba/blob/master/docs/Scenario2.md#part-4--analyze-machine-results>`__.
 
     Examples
     -----
-    >>> clf_log_creator = AggregateClfCalculator(config_path="MyConfigPath", data_measures=['Bout count', 'Total event duration'], classifiers=['Attack', 'Sniffing'])
+    >>> clf_log_creator = AggregateClfCalculator(config_path="MyConfigPath", data_measures=['Bout count', 'Total event duration (s)'], classifiers=['Attack', 'Sniffing'])
     >>> clf_log_creator.run()
     >>> clf_log_creator.save()
     """
 
     def __init__(self,
                  config_path: Union[str, os.PathLike],
                  data_measures: List[Literal['Bout count', 'Total event duration (s)', 'Mean event bout duration (s)', 'Median event bout duration (s)', 'First event occurrence (s)', 'Mean event bout interval duration (s)', 'Median event bout interval duration (s)']],
@@ -60,14 +60,15 @@
             for clf in self.clf_names:
                 clf_results_dict = {}
                 clf_data = bouts_df.loc[bouts_df['Event'] == clf]
                 if len(clf_data) > 0:
                     clf_results_dict['First event occurrence (s)'] = round(clf_data['Start_time'].min(), 3)
                     clf_results_dict['Bout count'] = len(clf_data)
                     clf_results_dict['Total event duration (s)'] = round(clf_data['Bout_time'].sum(), 3)
+
                     clf_results_dict['Mean event bout duration (s)'] = round(clf_data['Bout_time'].mean(), 3)
                     clf_results_dict['Median event bout duration (s)'] = round(clf_data['Bout_time'].median(), 3)
                 else:
                     clf_results_dict['First event occurrence (s)'] = None
                     clf_results_dict['Bout count'] = None
                     clf_results_dict['Total event duration (s)'] = None
                     clf_results_dict['Mean event bout duration (s)'] = None
@@ -94,18 +95,17 @@
         None
         """
 
         self.results_df = self.results_df[self.results_df['Measure'].isin(self.chosen_measures)].sort_values(by=['Video', 'Classifier', 'Measure']).reset_index(drop=True)
         self.results_df = self.results_df[self.results_df['Classifier'].isin(self.classifiers)].set_index('Video')
         self.results_df.to_csv(self.file_save_name)
         self.timer.stop_timer()
-
         stdout_success(msg=f'Data log saved at {self.file_save_name}', elapsed_time=self.timer.elapsed_time_str)
 
-# test = ClfLogCreator(config_path=r"/Users/simon/Desktop/envs/troubleshooting/two_black_animals_14bp/project_folder/project_config.ini",
+# test = AggregateClfCalculator(config_path=r"/Users/simon/Desktop/envs/troubleshooting/two_black_animals_14bp/project_folder/project_config.ini",
 #                      data_measures=['Bout count',
 #                                     'Total event duration (s)'],
 #                      classifiers=['Attack', 'Sniffing'])
 # test.run()
 # test.save()
```

### Comparing `Simba-UW-tf-dev-1.60.7/simba/data_processors/severity_bout_based_calculator.py` & `Simba-UW-tf-dev-1.60.9/simba/data_processors/severity_frame_based_calculator.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,205 +1,184 @@
 __author__ = "Simon Nilsson"
 
 import numpy as np
 import os
 import pandas as pd
 from datetime import datetime
-from numba import jit
-from typing import Dict, Union, List
 import cv2
+from typing import Dict, Union
 
-from simba.utils.read_write import get_fn_ext, read_df, get_video_meta_data
-from simba.utils.data import detect_bouts, create_color_palettes
+from simba.utils.read_write import get_fn_ext, read_df
 from simba.utils.checks import check_if_filepath_list_is_empty
+from simba.utils.data import find_bins, detect_bouts, get_video_meta_data, create_color_palettes
 from simba.utils.printing import stdout_success, SimbaTimer
 from simba.utils.warnings import NoDataFoundWarning
 from simba.mixins.config_reader import ConfigReader
 from simba.mixins.feature_extraction_mixin import FeatureExtractionMixin
-from simba.utils.errors import InvalidVideoFileError
+from simba.utils.errors import NoDataError, InvalidVideoFileError
 
-class SeverityBoutCalculator(ConfigReader, FeatureExtractionMixin):
+class SeverityFrameCalculator(ConfigReader, FeatureExtractionMixin):
     """
-    Computes the "severity" of classification bout events based on how much
-    the animals are moving within the bout. Bouts are scored as less or more severe at lower and higher movements, respectively.
+    Computes the "severity" of classification frame events based on how much
+    the animals are moving. Frames are scored as less or more severe at lower and higher movements, respectively.
 
     :parameter str config_path: path to SimBA project config file in Configparser format.
-    :parameter dict settings: how to calculate the severity. E.g., {'brackets': 10, 'clf': 'Attack', 'animals': ['Simon', 'JJ'], 'normalization': 'ALL VIDEOS', 'save_bin_definitions': True, 'visualize': True, 'visualize_event_cnt': 'ALL', 'video_speed': 1.0, 'show_pose': True}
+    :parameter dict settings: how to calculate the severity. E.g., {'brackets': 10, 'clf': 'Attack', 'animals': ['Simon', 'JJ'], 'time': True, 'frames': False}.
 
     .. note::
        `Tutorial <https://github.com/sgoldenlab/simba/blob/master/docs/Scenario2.md>`__.
 
     Examples
     ----------
-    >>> settings = {'brackets': 10, 'clf': 'Attack', 'animals': ['Simon', 'JJ'], 'normalization': 'ALL VIDEOS', 'save_bin_definitions': True, 'visualize': True, 'visualize_event_cnt': 'ALL', 'video_speed': 1.0, 'show_pose': True}
-    >>> processor = SeverityBoutCalculator(config_path='project_folder/project_config.ini', settings=settings)
+    >>> settings = {'brackets': 10, 'clf': 'Attack', 'animals': ['Simon', 'JJ'], 'time': True, 'frames': False, 'normalization': 'ALL VIDEOS', 'save_bin_definitions': True}
+    >>> processor = SeverityFrameCalculator(config_path='project_folder/project_config.ini', settings=settings)
     >>> processor.run()
     >>> processor.save()
     """
 
     def __init__(self,
                  config_path: Union[str, os.PathLike],
                  settings: Dict):
 
         ConfigReader.__init__(self, config_path=config_path)
         self.settings = settings
-        self.movement_animal_bp_dict = {k: self.animal_bp_dict[k] for k in self.settings['animals']}
-        self.color_lst_lst = create_color_palettes(no_animals=len(list(self.animal_bp_dict.keys())), map_size=len(self.bp_headers))
         check_if_filepath_list_is_empty(filepaths=self.machine_results_paths,
                                         error_msg=f'SIMBA ERROR: Cannot process severity. {self.machine_results_dir} directory is empty')
         save_name = os.path.join(f'severity_{datetime.now().strftime("%Y%m%d%H%M%S")}.csv')
+        self.movement_animal_bp_dict = {k: self.animal_bp_dict[k] for k in self.settings['animals']}
+        self.color_lst_lst = create_color_palettes(no_animals=len(list(self.animal_bp_dict.keys())), map_size=len(self.bp_headers))
         definitions_save_name = os.path.join(f'severity_bin_definitions_{datetime.now().strftime("%Y%m%d%H%M%S")}.csv')
         self.save_path = os.path.join(self.logs_path, save_name)
-        self.definitions_path, self.fourcc = os.path.join(self.logs_path, definitions_save_name), cv2.VideoWriter_fourcc(*'mp4v')
+        self.definitions_path = os.path.join(self.logs_path, definitions_save_name)
+        self.results = {}
 
-    @staticmethod
-    @jit(nopython=True)
-    def __movement_rolling_windows_agg(data: np.ndarray, fps: int):
-        results = np.full((40), np.nan)
-        for window_size_s in range(1, 41):
-            window_width = int(fps * window_size_s)
-            window_movement = np.full((data.shape[0]), np.nan)
-            for i in range(window_width, data.shape[0]):
-                window_movement[i] = np.sum(data[i-window_width:i])
-            results[window_size_s-1] = np.nanmean(window_movement)
-        return results
-
-    def __calculate_movements(self, data_paths: List[str]):
-        movements = {}
-        for file_cnt, file_path in enumerate(data_paths):
+    def __calculate_movements(self):
+        self.movements = {}
+        for file_cnt, file_path in enumerate(self.machine_results_paths):
             _, video_name, _ = get_fn_ext(file_path)
-            print(f'Analyzing movements in {video_name} ({file_cnt+1}/{len(data_paths)})...')
+            print(f'Analyzing movements in {video_name} ({file_cnt+1}/{len(self.machine_results_paths)})...')
             _, px_per_mm, fps = self.read_video_info(video_name=video_name)
             df = read_df(file_path=file_path, file_type=self.file_type)
             if self.settings['clf'] not in df.columns:
                 NoDataFoundWarning(msg=f'Skipping file {video_name} - {self.settings["clf"]} data not present in file')
                 continue
             video_movement = np.full((len(df)), 0)
             for animal_name, animal_bodyparts in self.movement_animal_bp_dict.items():
                 animal_df = df[animal_bodyparts['X_bps'] + animal_bodyparts['Y_bps']]
                 animal_df = self.create_shifted_df(df=animal_df)
                 for (bp_x, bp_y) in zip(animal_bodyparts['X_bps'], animal_bodyparts['Y_bps']):
                     video_movement = np.add(video_movement, self.euclidean_distance(animal_df[bp_x].values, animal_df[f'{bp_x}_shifted'].values, animal_df[bp_y].values, animal_df[f'{bp_y}_shifted'].values, px_per_mm))
-            movements[video_name] = video_movement
-        return movements
-
-    def __find_brackets(self, movements: dict):
-        print('Finding bracket cut off points...')
-        video_bins_info = {}
-        if self.settings['normalization'] == 'ALL VIDEOS':
-            m = []
-            [m.extend((d.tolist())) for d in movements.values()]
-            _, bins = pd.qcut(x=m, q=self.settings['brackets'], labels=list(range(1, self.settings['brackets'] + 1)), retbins=True)
-            for video_name, video_movements in movements.items():
-                bin_array = np.full((len(bins) - 1, 2), np.nan)
-                for i in range(len(bins) - 1):
-                    bin_array[i] = [bins[i].astype(int), bins[i+1].astype(int)]
-                video_bins_info[video_name] = bin_array
-        else:
-            for video_name, video_movements in movements.items():
-                _, bins = pd.qcut(x=video_movements, q=self.settings['brackets'], labels=list(range(1, self.settings['brackets'] + 1)), retbins=True)
-                bin_array = np.full((len(bins) - 1, 2), np.nan)
-                for i in range(len(bins) - 1):
-                    bin_array[i] = [bins[i].astype(int), bins[i + 1].astype(int)]
-                video_bins_info[video_name] = bin_array
-        return video_bins_info
+            self.movements[video_name] = video_movement.astype(np.int)
 
     def run(self):
-        movements = self.__calculate_movements(data_paths=self.machine_results_paths)
-        video_bins_info = self.__find_brackets(movements=movements)
-        self.results = pd.DataFrame(columns=['VIDEO', 'EVENT', 'START TIME', 'END TIME', 'START FRAME', 'END FRAME', 'BOUT TIME', 'MOVEMENT', 'SEVERITY'])
+        self.__calculate_movements()
+        self.visualization_data = {}
+        self.video_bins_info = find_bins(data=self.movements, bracket_type=self.settings['bracket_type'], bracket_cnt=self.settings['brackets'], normalization_method=self.settings['normalization'])
         for file_cnt, file_path in enumerate(self.machine_results_paths):
             _, video_name, _ = get_fn_ext(file_path)
+            print(f'Matching brackets to movements in video {video_name} ({file_cnt+1}/{len(self.machine_results_paths)})...')
+            self.results[video_name] = {}
             _, px_per_mm, fps = self.read_video_info(video_name=video_name)
-            df = read_df(file_path=file_path, file_type=self.file_type)
-            bout_df = detect_bouts(data_df=df, target_lst=[self.settings['clf']], fps=fps)
-            bout_df.columns = ['EVENT', 'START TIME', 'END TIME', 'START FRAME', 'END FRAME', 'BOUT TIME']
-            severity_lst, movement_lst = [], []
-            for i in bout_df[['START FRAME', 'END FRAME']].values:
-                bout_move_val = np.mean(movements[video_name][i[0]:i[1]])
-                for j_cnt, j in enumerate(video_bins_info[video_name]):
-                    if j[0] <= bout_move_val <= j[1]:
-                        severity_lst.append(j_cnt+1)
-                        movement_lst.append(round(bout_move_val, 4))
-                        break
-            bout_df['MOVEMENT'] = movement_lst
-            bout_df['SEVERITY'] = severity_lst
-            bout_df.insert(0, 'VIDEO', video_name)
-            self.results = pd.concat([self.results, bout_df], axis=0).reset_index(drop=True)
-        self.save()
-        if self.settings['save_bin_definitions']:
-            self.save_bin_definitions(data=video_bins_info)
+            df = read_df(file_path=file_path, file_type=self.file_type).astype(int)
+            move_df = pd.DataFrame(self.movements[video_name], columns=['MOVEMENT'])
+            video_bins = np.array((0))
+            video_bins = np.hstack((video_bins, self.video_bins_info[video_name][: , -1]))
+            hist = np.histogram([self.movements[video_name]], bins=video_bins)
+            move_df['BIN'] = np.fmin(np.digitize(self.movements[video_name], hist[1]), self.settings['brackets'])
+            df = pd.concat([df, move_df], axis=1)
+            if self.settings['visualize']: self.visualization_data[video_name] = df
+            clf_df = df['BIN'][df[self.settings['clf']] == 1].astype(int).reset_index(drop=True)
+            for i in range(0, self.settings['brackets']):
+                if self.settings['frames']:
+                    self.results[video_name][f'Grade {str(i + 1)} (frames)'] = len(clf_df[clf_df == i])
+                if self.settings['time']:
+                    self.results[video_name][f'Grade {str(i + 1)} (s)'] = round((len(clf_df[clf_df == i])/ fps), 4)
+        self.__save()
         if self.settings['visualize']:
-            self.visualize()
+            self.__visualize()
 
-    def save(self):
-        self.results.to_csv(self.save_path)
+    def __save(self):
+        print('Saving data..')
+        out_df = pd.DataFrame(columns=['VIDEO', 'MEASUREMENT', 'VALUE'])
+        for video_name, video_data in self.results.items():
+            for grade, grade_data in video_data.items():
+                out_df.loc[len(out_df)] = [video_name, grade, grade_data]
+        out_df.to_csv(self.save_path)
         self.timer.stop_timer()
-        stdout_success(msg=f'Bout severity data saved at {self.save_path}', elapsed_time=self.timer.elapsed_time_str)
-
-    def save_bin_definitions(self, data=dict):
-        results = pd.DataFrame(columns=['VIDEO', 'SEVERITY_BIN', '>=', '<'])
-        for video_name, video_bins in data.items():
-            for bin_cnt, video_bin in enumerate(video_bins):
-                results.loc[len(results)] = [video_name, bin_cnt+1, video_bin[0], video_bin[1]]
-        save_path = os.path.join(self.logs_path, f'severity_bin_definitions_{self.datetime}.csv')
-        results.to_csv(save_path)
-        stdout_success(msg=f'Severity bracket definitions saved at {save_path}')
+        stdout_success(msg=f'Severity data saved at {self.save_path}', elapsed_time=self.timer.elapsed_time_str)
 
+        if self.settings['save_bin_definitions']:
+            results = pd.DataFrame(columns=['VIDEO', 'SEVERITY_BIN', '>=', '<'])
+            for video_name, video_bins in self.video_bins_info.items():
+                for bin_cnt, video_bin in enumerate(video_bins):
+                    results.loc[len(results)] = [video_name, bin_cnt + 1, video_bin[0], video_bin[1]]
+            save_path = os.path.join(self.logs_path, f'severity_bin_definitions_{self.datetime}.csv')
+            results.to_csv(save_path)
+            stdout_success(msg=f'Severity bracket definitions saved at {save_path}')
 
-    def visualize(self):
-        if self.settings['visualize_event_cnt'] == 'ALL CLIPS':
-            self.settings['visualize_event_cnt'] = len(self.results)
-        elif self.settings['visualize_event_cnt'] > len(self.results):
-            self.settings['visualize_event_cnt'] = len(self.results)
-            print(f'User specified {self.settings["visualize_event_cnt"]} visualization but only {len(self.results)} bouts where found. Creating {len(self.results)} videos...')
+    def __visualize(self):
+        bouts_df_lst = []
         video_timer, save_dir = SimbaTimer(start=True), os.path.join(self.project_path, 'frames', 'output', 'severity_bouts')
         if not os.path.exists(save_dir): os.makedirs(save_dir)
-        viz_df = self.results.sample(n=self.settings['visualize_event_cnt']).reset_index(drop=True)
-        for idx, r in viz_df.iterrows():
-            video_name, start_frm, end_frame, severity = r['VIDEO'], r['START FRAME'], r['END FRAME'], r['SEVERITY']
-            pose_df = None
-            if self.settings['show_pose']:
-                pose_df = read_df(os.path.join(self.machine_results_dir, video_name + '.' + self.file_type), self.file_type, usecols=self.bp_headers).astype(int)
-            clip_path = os.path.join(save_dir, f'{video_name}_{self.settings["clf"]}_{start_frm}_{end_frame}_{severity}.mp4')
+        for video_name, video_data in self.visualization_data.items():
+            bouts_df = detect_bouts(data_df=video_data, target_lst=[self.settings['clf']], fps=-1)
+            bouts_df.insert(0, 'VIDEO', video_name)
+            bouts_df_lst.append(bouts_df)
+        bouts_df = pd.concat(bouts_df_lst, axis=0)
+        if self.settings['visualize_event_cnt'] == 'ALL CLIPS':
+            self.settings['visualize_event_cnt'] = len(bouts_df)
+        elif self.settings['visualize_event_cnt'] > len(bouts_df):
+            self.settings['visualize_event_cnt'] = len(bouts_df)
+            print(f'User specified {self.settings["visualize_event_cnt"]} visualization but only {len(self.results)} bouts where found. Creating {len(self.results)} videos...')
+        bouts_df = bouts_df.sample(n=self.settings['visualize_event_cnt']).reset_index(drop=True)
+        for idx, r in bouts_df.iterrows():
+            video_name, start_frm, end_frame = r['VIDEO'], r['Start_frame'], r['End_frame']
+            print(start_frm)
+            bout_df = self.visualization_data[video_name].iloc[start_frm:end_frame]
+            clip_path = os.path.join(save_dir, f'{video_name}_{self.settings["clf"]}_{start_frm}_{end_frame}.mp4')
             video_path = self.find_video_of_file(video_dir=self.video_dir, filename=video_name)
             video_meta_data = get_video_meta_data(video_path)
             self.space_scale, self.radius_scale, self.res_scale, self.font_scale = 60, 12, 1500, 1.1
             self.max_dim = max(video_meta_data['width'], video_meta_data['height'])
             self.circle_scale = int(self.radius_scale / (self.res_scale / self.max_dim))
+            self.font_size = float(self.font_scale / (self.res_scale / self.max_dim))
             video_fps = int(video_meta_data['fps'] * self.settings['video_speed'])
             if video_fps < 1: video_fps = 1
             cap = cv2.VideoCapture(video_path)
             writer = cv2.VideoWriter(clip_path, cv2.VideoWriter_fourcc(*'mp4v'), video_fps, (int(video_meta_data['width']), int(video_meta_data['height'])))
-            event_frm_count, frm_cnt, current_frm = end_frame - start_frm, 0, start_frm
+            event_frm_count, frm_cnt, current_frm = (end_frame - start_frm), 0, start_frm
             cap.set(1, current_frm)
+
             while current_frm < end_frame:
                 ret, img = cap.read()
                 if self.settings['show_pose']:
-                    frm_pose = pose_df.iloc[current_frm]
+                    frm_pose = bout_df.loc[current_frm]
+                    cv2.putText(img, f'Severity bin: {frm_pose["BIN"]}', (10, 50), cv2.FONT_HERSHEY_COMPLEX, self.font_size, (255, 0, 0), 2)
                     for animal_cnt, (animal_name, animal_body_parts) in enumerate(self.animal_bp_dict.items()):
                         for bp_cnt, (x_name, y_name) in enumerate(zip(animal_body_parts['X_bps'], animal_body_parts['Y_bps'])):
                             x = frm_pose[[x_name, y_name]].values
                             cv2.circle(img, (x[0], x[1]), 0, self.color_lst_lst[animal_cnt][bp_cnt], self.circle_scale)
 
                 if not ret:
                     raise InvalidVideoFileError(msg=f'Could not find frame {current_frm} in video {video_path}. Video {video_path} contains {video_meta_data["frame_count"]} frames.')
                 writer.write(img)
                 frm_cnt += 1
-                print(f'Frame {str(frm_cnt)} / {str(event_frm_count)}, Event {idx + 1}/{str(len(viz_df))}, Video {video_name}')
+                print(f'Frame {str(frm_cnt)} / {str(event_frm_count)}, Event {idx + 1}/{str(len(bouts_df))}, Video {video_name}')
                 current_frm += 1
             writer.release()
         video_timer.stop_timer()
         stdout_success(msg=f'Videos complete: saved in {save_dir}', elapsed_time=video_timer.elapsed_time_str)
 
 # settings = {'brackets': 10,
 #             'clf': 'Attack',
 #             'animals': ['Simon', 'JJ'],
 #             'normalization': 'ALL VIDEOS', #BY VIDEO
+#             'bracket_type': "QUANTILE",
+#             'time': True,
+#             'frames': True,
 #             'save_bin_definitions': True,
 #             'visualize': True,
 #             'visualize_event_cnt': 'ALL CLIPS',
 #             'video_speed': 0.1,
 #             'show_pose': True}
-# processor = SeverityBoutCalculator(config_path='/Users/simon/Desktop/envs/troubleshooting/two_black_animals_14bp/project_folder/project_config.ini', settings=settings)
-# processor.run()
-# processor.save()
+# processor = SeverityFrameCalculator(config_path='/Users/simon/Desktop/envs/troubleshooting/two_black_animals_14bp/project_folder/project_config.ini', settings=settings)
+# processor.run()
```

### Comparing `Simba-UW-tf-dev-1.60.7/simba/data_processors/interpolation_smoothing.py` & `Simba-UW-tf-dev-1.60.9/simba/data_processors/interpolation_smoothing.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.60.7/simba/data_processors/timebins_clf_calculator.py` & `Simba-UW-tf-dev-1.60.9/simba/data_processors/timebins_clf_calculator.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.60.7/simba/data_processors/fsttc_calculator.py` & `Simba-UW-tf-dev-1.60.9/simba/data_processors/fsttc_calculator.py`

 * *Files 1% similar despite different names*

```diff
@@ -184,17 +184,17 @@
 
         self.out_df['BEHAVIOR COMBINATION'] = self.out_df['FIRST BEHAVIOR'].str.cat(self.out_df['SECOND BEHAVIOR'], sep='-')
         data_df = self.out_df[self.out_df['FSTTC'] != 'No events'].reset_index(drop=True)
         data_df['FSTTC'] = pd.to_numeric(data_df['FSTTC'], errors='coerce')
         figure_FSCTT = sns.violinplot(x='BEHAVIOR COMBINATION', y="FSTTC", data=data_df, cut=0)
         figure_FSCTT.set_xticklabels(figure_FSCTT.get_xticklabels(), rotation=45, size=7)
         figure_FSCTT.figure.set_size_inches(13.7, 8.27)
-        save_plot_path = os.path.join(self.logs_path, f'FSTTC_{self.datetime}.png')
-        figure_FSCTT.figure.savefig(save_plot_path, bbox_inches="tight")
-        stdout_success(msg=f'FSTTC figure saved at {save_plot_path}')
+        self.save_plot_path = os.path.join(self.logs_path, f'FSTTC_{self.datetime}.png')
+        figure_FSCTT.figure.savefig(self.save_plot_path, bbox_inches="tight")
+        stdout_success(msg=f'FSTTC figure saved at {self.save_plot_path}')
 
 
     def save(self):
         """
         Method to save forward spike-time tiling coefficients (FSTTC) to disk within the `project_folder/logs` directory.
 
         Returns
@@ -202,18 +202,18 @@
         None
         """
         self.out_df = pd.DataFrame(columns=['VIDEO', 'FIRST BEHAVIOR', 'SECOND BEHAVIOR', 'FSTTC'])
         for video_name, video_data in self.results_dict.items():
             for first_behavior, first_behavior_data in video_data.items():
                 for second_behavior, fsttc in first_behavior_data.items():
                     self.out_df.loc[len(self.out_df)] = [video_name, first_behavior, second_behavior, fsttc]
-        file_save_path = os.path.join(self.logs_path, 'FSTTC_{}.csv'.format(str(self.datetime)))
-        self.out_df.to_csv(file_save_path)
+        self.file_save_path = os.path.join(self.logs_path, 'FSTTC_{}.csv'.format(str(self.datetime)))
+        self.out_df.to_csv(self.file_save_path)
         self.timer.stop_timer()
-        stdout_success(msg=f'FSTTC data saved at {file_save_path}', elapsed_time=self.timer.elapsed_time_str)
+        stdout_success(msg=f'FSTTC data saved at {self.file_save_path}', elapsed_time=self.timer.elapsed_time_str)
 
 # test = FSTTCCalculator(config_path='/Users/simon/Desktop/envs/troubleshooting/two_black_animals_14bp/project_folder/project_config.ini',
 #                      time_window=2000,
 #                      behavior_lst=['Attack', 'Sniffing'],
 #                     create_graphs=False)
 # test.run()
```

### Comparing `Simba-UW-tf-dev-1.60.7/simba/data_processors/interpolate_pose.py` & `Simba-UW-tf-dev-1.60.9/simba/data_processors/interpolate_pose.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.60.7/simba/data_processors/directing_other_animals_calculator.py` & `Simba-UW-tf-dev-1.60.9/simba/data_processors/directing_other_animals_calculator.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.60.7/simba/data_processors/timebins_movement_calculator.py` & `Simba-UW-tf-dev-1.60.9/simba/data_processors/timebins_movement_calculator.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.60.7/simba/data_processors/severity_calculator.py` & `Simba-UW-tf-dev-1.60.9/simba/data_processors/severity_calculator.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.60.7/simba/data_processors/pup_retrieval_calculator.py` & `Simba-UW-tf-dev-1.60.9/simba/data_processors/pup_retrieval_calculator.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.60.7/simba/data_processors/pybursts_calculator.py` & `Simba-UW-tf-dev-1.60.9/simba/data_processors/pybursts_calculator.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.60.7/simba/data_processors/severity_frame_based_calculator.py` & `Simba-UW-tf-dev-1.60.9/simba/pose_importers/sleap_csv_importer.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,135 +1,132 @@
 __author__ = "Simon Nilsson"
 
-import numpy as np
-import os
 import pandas as pd
-from datetime import datetime
-from numba import jit
-from typing import Dict, Optional, Union
-
-from simba.utils.read_write import get_fn_ext, read_df
-from simba.utils.checks import check_if_filepath_list_is_empty
-from simba.utils.printing import stdout_success
-from simba.utils.warnings import NoDataFoundWarning
+import os
+import numpy as np
+from copy import deepcopy
+
+from simba.data_processors.interpolation_smoothing import Interpolate, Smooth
+from simba.utils.read_write import find_all_videos_in_project
 from simba.mixins.config_reader import ConfigReader
-from simba.mixins.feature_extraction_mixin import FeatureExtractionMixin
+from simba.mixins.pose_importer_mixin import PoseImporterMixin
+from simba.utils.read_write import write_df, find_video_of_file, get_video_meta_data, get_fn_ext
+from simba.utils.printing import stdout_success, SimbaTimer
+from simba.utils.enums import Methods
 
-class SeverityFrameCalculator(ConfigReader, FeatureExtractionMixin):
-    """
-    Computes the "severity" of classification frame events based on how much
-    the animals are moving. Frames are scored as less or more severe at lower and higher movements, respectively.
+class SLEAPImporterCSV(ConfigReader, PoseImporterMixin):
 
-    :parameter str config_path: path to SimBA project config file in Configparser format.
-    :parameter dict settings: how to calculate the severity. E.g., {'brackets': 10, 'clf': 'Attack', 'animals': ['Simon', 'JJ'], 'time': True, 'frames': False}.
+    """
+    Importing SLEAP pose-estimation data into SimBA project in ``CSV`` format.
 
     .. note::
-       `Tutorial <https://github.com/sgoldenlab/simba/blob/master/docs/Scenario2.md>`__.
+      `Google Colab notebook for converting SLEAP .slp to CSV written by @Toshea111  <https://colab.research.google.com/drive/1EpyTKFHVMCqcb9Lj9vjMrriyaG9SvrPO?usp=sharing>`__.
+      `Example expected SLEAP csv data file for 5 animals / 4 pose-estimated body-parts  <https://github.com/sgoldenlab/simba/blob/master/misc/sleap_csv_example.csv>`__.
+
+    :parameter str config_path: path to SimBA project config file in Configparser format
+    :parameter str data_folder: Path to folder containing SLEAP data in `csv` format.
+    :parameter List[str] id_lst: Animal names. This will be ignored in one animal projects and default to ``Animal_1``.
+    :parameter str interpolation_settings: String defining the pose-estimation interpolation method. OPTIONS: 'None', 'Animal(s): Nearest',
+        'Animal(s): Linear', 'Animal(s): Quadratic','Body-parts: Nearest', 'Body-parts: Linear',
+        'Body-parts: Quadratic'.
+    :parameter str smoothing_settings: Dictionary defining the pose estimation smoothing method. EXAMPLE: {'Method': 'Savitzky Golay',
+        'Parameters': {'Time_window': '200'}})
 
-    Examples
+    References
     ----------
-    >>> settings = {'brackets': 10, 'clf': 'Attack', 'animals': ['Simon', 'JJ'], 'time': True, 'frames': False, 'normalization': 'ALL VIDEOS', 'save_bin_definitions': True}
-    >>> processor = SeverityFrameCalculator(config_path='project_folder/project_config.ini', settings=settings)
-    >>> processor.run()
-    >>> processor.save()
+    .. [1] Pereira et al., SLEAP: A deep learning system for multi-animal pose tracking, `Nature Methods`,
+           2022.
+
+    >>> sleap_csv_importer = SLEAPImporterCSV(config_path=r'project_folder/project_config.ini', data_folder=r'data_folder', actor_IDs=['Termite_1', 'Termite_2', 'Termite_3', 'Termite_4', 'Termite_5'], interpolation_settings="Body-parts: Nearest", smoothing_settings = {'Method': 'Savitzky Golay', 'Parameters': {'Time_window': '200'}})
+    >>> sleap_csv_importer.run()
     """
 
     def __init__(self,
-                 config_path: Union[str, os.PathLike],
-                 settings: Dict):
-
-        ConfigReader.__init__(self, config_path=config_path)
-        self.settings = settings
-        check_if_filepath_list_is_empty(filepaths=self.machine_results_paths,
-                                        error_msg=f'SIMBA ERROR: Cannot process severity. {self.machine_results_dir} directory is empty')
-        save_name = os.path.join(f'severity_{datetime.now().strftime("%Y%m%d%H%M%S")}.csv')
-        definitions_save_name = os.path.join(f'severity_bin_definitions_{datetime.now().strftime("%Y%m%d%H%M%S")}.csv')
-        self.save_path = os.path.join(self.logs_path, save_name)
-        self.definitions_path = os.path.join(self.logs_path, definitions_save_name)
-        self.results = {}
-
-    def __calculate_movements(self):
-        self.movements = {}
-        for file_cnt, file_path in enumerate(self.machine_results_paths):
-            _, video_name, _ = get_fn_ext(file_path)
-            print(f'Analyzing movements in {video_name} ({file_cnt+1}/{len(self.machine_results_paths)})...')
-            _, px_per_mm, fps = self.read_video_info(video_name=video_name)
-            df = read_df(file_path=file_path, file_type=self.file_type)
-            if self.settings['clf'] not in df.columns:
-                NoDataFoundWarning(msg=f'Skipping file {video_name} - {self.settings["clf"]} data not present in file')
-                continue
-            video_movement = np.full((len(df)), 0)
-            for animal_name, animal_bodyparts in self.animal_bp_dict.items():
-                animal_df = df[animal_bodyparts['X_bps'] + animal_bodyparts['Y_bps']]
-                animal_df = self.create_shifted_df(df=animal_df)
-                for (bp_x, bp_y) in zip(animal_bodyparts['X_bps'], animal_bodyparts['Y_bps']):
-                    video_movement = np.add(video_movement, self.euclidean_distance(animal_df[bp_x].values, animal_df[f'{bp_x}_shifted'].values, animal_df[bp_y].values, animal_df[f'{bp_y}_shifted'].values, px_per_mm))
-            self.movements[video_name] = video_movement.astype(np.int)
-
+                 config_path: str,
+                 data_folder: str,
+                 id_lst: list,
+                 interpolation_settings: str,
+                 smoothing_settings: dict):
+
+        ConfigReader.__init__(self, config_path=config_path, read_video_info=False)
+        PoseImporterMixin.__init__(self)
+        self.interpolation_settings, self.smoothing_settings = interpolation_settings, smoothing_settings
+        self.data_folder, self.id_lst = data_folder, id_lst
+        self.import_log_path = os.path.join(self.logs_path, f'data_import_log_{self.datetime}.csv')
+        self.video_paths = find_all_videos_in_project(videos_dir=self.video_dir)
+        self.input_data_paths = self.find_data_files(dir=self.data_folder, extensions=['.csv'])
+        self.data_and_videos_lk = self.link_video_paths_to_data_paths(data_paths=self.input_data_paths, video_paths=self.video_paths)
+        if (self.pose_setting is Methods.USER_DEFINED.value):
+            self.__update_config_animal_cnt()
+        if self.animal_cnt > 1:
+            self.check_multi_animal_status()
+            self.animal_bp_dict = self.create_body_part_dictionary(self.multi_animal_status, self.id_lst, self.animal_cnt, self.x_cols, self.y_cols, self.p_cols, self.clr_lst)
+            self.update_bp_headers_file()
+        print(f'Importing {len(list(self.data_and_videos_lk.keys()))} file(s)...')
 
     def run(self):
-        self.__calculate_movements()
-        self.video_bins_info = {}
-        movements_cuts = {}
-        print('Finding bracket cut off points...')
-        if self.settings['normalization'] == 'ALL VIDEOS':
-            m = []
-            [m.extend((d.tolist())) for d in self.movements.values()]
-            _, bins = pd.qcut(x=m, q=self.settings['brackets'], labels=list(range(1, self.settings['brackets'] + 1)), retbins=True)
-            for video_name, video_movements in self.movements.items():
-                self.video_bins_info[video_name] = bins.astype(int)
-                data, _ = pd.cut(x=video_movements, bins=bins, labels=list(range(1, self.settings['brackets'] + 1)), retbins=True)
-                movements_cuts[video_name] = np.hstack((video_movements.reshape(-1, 1), data.astype(np.int8).reshape(-1, 1)))
-        else:
-            for video_name, video_movements in self.movements.items():
-                data, bins = pd.qcut(x=video_movements, q=self.settings['brackets'], labels=list(range(1, self.settings['brackets'] + 1)), retbins=True)
-                movements_cuts[video_name] = np.hstack((video_movements.reshape(-1, 1), data.astype(np.int8).reshape(-1, 1)))
-                self.video_bins_info[video_name] = bins.astype(int)
-
-        for file_cnt, file_path in enumerate(self.machine_results_paths):
-            _, video_name, _ = get_fn_ext(file_path)
-            print(f'Matching brackets to movements in video {video_name} ({file_cnt+1}/{len(self.machine_results_paths)})...')
-            self.results[video_name] = {}
-            _, px_per_mm, fps = self.read_video_info(video_name=video_name)
-            df = read_df(file_path=file_path, file_type=self.file_type)
-            df = pd.concat([df, pd.DataFrame(movements_cuts[video_name], columns=['MOVEMENT', 'BIN'])], axis=1)
-            clf_df = df['BIN'][df[self.settings['clf']] == 1].astype(int).reset_index(drop=True)
-            for i in range(0, self.settings['brackets']):
-                if self.settings['frames']:
-                    self.results[video_name][f'Grade {str(i + 1)} (frames)'] = len(clf_df[clf_df == i])
-                if self.settings['time']:
-                    self.results[video_name][f'Grade {str(i + 1)} (s)'] = round((len(clf_df[clf_df == i])/ fps), 4)
-
-    def save(self):
-        print('Saving data..')
-        out_df = pd.DataFrame(columns=['VIDEO', 'MEASUREMENT', 'VALUE'])
-        for video_name, video_data in self.results.items():
-            for grade, grade_data in video_data.items():
-                out_df.loc[len(out_df)] = [video_name, grade, grade_data]
-        out_df.to_csv(self.save_path)
+        for file_cnt, (video_name, video_data) in enumerate(self.data_and_videos_lk.items()):
+            print(f'Analysing {video_name}...')
+            video_timer = SimbaTimer(start=True)
+            self.video_name = video_name
+            self.save_path = os.path.join(os.path.join(self.input_csv_dir, f'{self.video_name}.{self.file_type}'))
+            data_df = pd.read_csv(video_data['DATA'])
+            idx = data_df.iloc[:, :2]
+            idx['track'] = idx['track'].str.replace(r'[^\d.]+', '').astype(int)
+            data_df = data_df.iloc[:, 2:]
+            if self.animal_cnt > 1:
+                self.data_df = pd.DataFrame(self.transpose_multi_animal_table(data=data_df.values, idx=idx.values, animal_cnt=self.animal_cnt))
+                p_df = pd.DataFrame(1.0, index=self.data_df.index, columns=self.data_df.columns[1::2] + .5)
+                self.data_df = pd.concat([self.data_df, p_df], axis=1).sort_index(axis=1)
+                self.data_df.columns = self.bp_headers
+            else:
+                idx = list(idx.drop('track', axis=1)['frame_idx'])
+                self.data_df = data_df.set_index([idx]).sort_index()
+                self.data_df.columns = np.arange(len(self.data_df.columns))
+                self.data_df = self.data_df.reindex(range(self.data_df.index[0], self.data_df.index[-1] + 1), fill_value=0)
+                p_df = pd.DataFrame(1.0, index=self.data_df.index, columns=self.data_df.columns[1::2] + .5)
+                self.data_df = pd.concat([self.data_df, p_df], axis=1).sort_index(axis=1)
+                self.data_df.columns = self.bp_headers
+
+            self.out_df = deepcopy(self.data_df)
+            if self.animal_cnt > 1:
+                self.initialize_multi_animal_ui(animal_bp_dict=self.animal_bp_dict,
+                                                video_info=get_video_meta_data(video_data['VIDEO']),
+                                                data_df=self.data_df,
+                                                video_path=video_data['VIDEO'])
+                self.multianimal_identification()
+            write_df(df=self.out_df, file_type=self.file_type, save_path=self.save_path, multi_idx_header=True)
+            if self.interpolation_settings != 'None':
+                self.__run_interpolation()
+            if self.smoothing_settings['Method'] != 'None':
+                self.__run_smoothing()
+            video_timer.stop_timer()
+            stdout_success(msg=f'Video {video_name} data imported...', elapsed_time=video_timer.elapsed_time_str)
         self.timer.stop_timer()
-        stdout_success(msg=f'Severity data saved at {self.save_path}', elapsed_time=self.timer.elapsed_time_str)
-
+        stdout_success(msg=f'{len(list(self.data_and_videos_lk.keys()))} file(s) imported to the SimBA project (project_folder/csv/input_csv directory)')
 
-        if self.settings['save_bin_definitions']:
-            brackets_data_cols = ['VIDEO']
-            for i in range(0, self.settings['brackets']):
-                brackets_data_cols.append(f'GRADE {i+1} START'); brackets_data_cols.append(f'GRADE {i + 1} STOP')
-            brackets_df = pd.DataFrame(columns=brackets_data_cols)
-            for video_name, video_bins in self.video_bins_info.items():
-                video_info = [video_name]
-                for i in range(len(video_bins)-1):
-                    video_info.extend((video_bins[i], video_bins[i+1]))
-                brackets_df.loc[len(brackets_df)] = video_info
-            brackets_df.to_csv(self.definitions_path)
-            stdout_success(msg=f'Severity brackets definitions saved at {self.definitions_path}', elapsed_time=self.timer.elapsed_time_str)
-
-# settings = {'brackets': 10,
-#             'clf': 'Attack',
-#             'animals': ['Simon', 'JJ'],
-#             'normalization': 'ALL VIDEOS', #BY VIDEO
-#             'time': True,
-#             'frames': True,
-#             'save_bin_definitions': True}
-# processor = SeverityCalculator(config_path='/Users/simon/Desktop/envs/troubleshooting/two_black_animals_14bp/project_folder/project_config.ini', settings=settings)
-# processor.run()
-# processor.save()
+    def __run_interpolation(self):
+        print(f'Interpolating missing values in video {self.video_name} (Method: {self.interpolation_settings})...')
+        _ = Interpolate(input_path=self.save_path, config_path=self.config_path, method=self.interpolation_settings, initial_import_multi_index=True)
+
+    def __run_smoothing(self):
+        print(f'Performing {self.smoothing_settings["Method"]} smoothing on video {self.video_name}...')
+        Smooth(config_path=self.config_path,
+               input_path=self.save_path,
+               time_window=int(self.smoothing_settings['Parameters']['Time_window']),
+               smoothing_method=self.smoothing_settings['Method'],
+               initial_import_multi_index=True)
+
+# test = SLEAPImporterCSV(config_path=r'/Users/simon/Desktop/envs/troubleshooting/Hornet/project_folder/project_config.ini',
+#                  data_folder=r'/Users/simon/Desktop/envs/troubleshooting/Hornet_single_slp/import',
+#                  id_lst=['Hornet'],
+#                  interpolation_settings="Body-parts: Nearest",
+#                  smoothing_settings = {'Method': 'Savitzky Golay', 'Parameters': {'Time_window': '200'}})
+# test.run()
+
+
+# test = SLEAPImporterCSV(config_path=r'/Users/simon/Desktop/envs/troubleshooting/slp_1_animal_1_bp/project_folder',
+#                  data_folder='/Users/simon/Desktop/envs/troubleshooting/slp_1_animal_1_bp/import',
+#                  actor_IDs=['Termite_1'],
+#                  interpolation_settings="Body-parts: Nearest",
+#                  smoothing_settings = {'Method': 'Savitzky Golay', 'Parameters': {'Time_window': '200'}})
+# test.run()
```

### Comparing `Simba-UW-tf-dev-1.60.7/simba/data_processors/kleinberg_calculator.py` & `Simba-UW-tf-dev-1.60.9/simba/data_processors/kleinberg_calculator.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.60.7/simba/data_processors/movement_calculator.py` & `Simba-UW-tf-dev-1.60.9/simba/data_processors/movement_calculator.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.60.7/simba/pose_configurations_archive/pose_configurations_archive_1/.DS_Store` & `Simba-UW-tf-dev-1.60.9/simba/pose_configurations_archive/pose_configurations_archive_1/.DS_Store`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.60.7/simba/pose_configurations_archive/pose_configurations_archive_1/bp_names/.DS_Store` & `Simba-UW-tf-dev-1.60.9/simba/pose_configurations_archive/pose_configurations_archive_1/bp_names/.DS_Store`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.60.7/simba/pose_configurations_archive/pose_configurations_archive_1/bp_names/bp_names.csv` & `Simba-UW-tf-dev-1.60.9/simba/pose_configurations_archive/pose_configurations_archive_1/bp_names/bp_names.csv`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.60.7/simba/pose_configurations_archive/pose_configurations_archive_1/no_animals/.DS_Store` & `Simba-UW-tf-dev-1.60.9/simba/pose_configurations_archive/pose_configurations_archive_1/no_animals/.DS_Store`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.60.7/simba/pose_configurations_archive/pose_configurations_archive_1/configuration_names/.DS_Store` & `Simba-UW-tf-dev-1.60.9/simba/pose_configurations_archive/pose_configurations_archive_1/configuration_names/.DS_Store`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.60.7/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/.DS_Store` & `Simba-UW-tf-dev-1.60.9/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/.DS_Store`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.60.7/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/8.png` & `Simba-UW-tf-dev-1.60.9/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/8.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.60.7/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/9.png` & `Simba-UW-tf-dev-1.60.9/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/9.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.60.7/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/12.png` & `Simba-UW-tf-dev-1.60.9/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/12.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.60.7/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/13.png` & `Simba-UW-tf-dev-1.60.9/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/13.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.60.7/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/11.png` & `Simba-UW-tf-dev-1.60.9/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/11.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.60.7/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/10.png` & `Simba-UW-tf-dev-1.60.9/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/10.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.60.7/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/4.png` & `Simba-UW-tf-dev-1.60.9/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/4.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.60.7/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/5.png` & `Simba-UW-tf-dev-1.60.9/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/5.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.60.7/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/7.png` & `Simba-UW-tf-dev-1.60.9/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/7.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.60.7/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/6.png` & `Simba-UW-tf-dev-1.60.9/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/6.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.60.7/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/2.png` & `Simba-UW-tf-dev-1.60.9/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/2.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.60.7/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/3.png` & `Simba-UW-tf-dev-1.60.9/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/3.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.60.7/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/1.png` & `Simba-UW-tf-dev-1.60.9/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/1.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.60.7/simba/model/train_rf.py` & `Simba-UW-tf-dev-1.60.9/simba/model/train_rf.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.60.7/simba/model/.DS_Store` & `Simba-UW-tf-dev-1.60.9/simba/model/.DS_Store`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.60.7/simba/model/inference_batch.py` & `Simba-UW-tf-dev-1.60.9/simba/model/inference_batch.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.60.7/simba/model/grid_search_rf.py` & `Simba-UW-tf-dev-1.60.9/simba/model/grid_search_rf.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.60.7/simba/model/inference_validation.py` & `Simba-UW-tf-dev-1.60.9/simba/model/inference_validation.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.60.7/simba/roi_tools/ROI_time_bin_calculator.py` & `Simba-UW-tf-dev-1.60.9/simba/roi_tools/ROI_time_bin_calculator.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.60.7/simba/roi_tools/ROI_movement_analyzer.py` & `Simba-UW-tf-dev-1.60.9/simba/roi_tools/ROI_movement_analyzer.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.60.7/simba/roi_tools/.DS_Store` & `Simba-UW-tf-dev-1.60.9/simba/roi_tools/.DS_Store`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.60.7/simba/roi_tools/ROI_define.py` & `Simba-UW-tf-dev-1.60.9/simba/roi_tools/ROI_define.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.60.7/simba/roi_tools/ROI_reset.py` & `Simba-UW-tf-dev-1.60.9/simba/roi_tools/ROI_reset.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.60.7/simba/roi_tools/ROI_analyzer.py` & `Simba-UW-tf-dev-1.60.9/simba/roi_tools/ROI_analyzer.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.60.7/simba/roi_tools/ROI_feature_analyzer.py` & `Simba-UW-tf-dev-1.60.9/simba/roi_tools/ROI_feature_analyzer.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.60.7/simba/roi_tools/ROI_multiply.py` & `Simba-UW-tf-dev-1.60.9/simba/roi_tools/ROI_multiply.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.60.7/simba/roi_tools/ROI_size_calculations.py` & `Simba-UW-tf-dev-1.60.9/simba/roi_tools/ROI_size_calculations.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.60.7/simba/roi_tools/ROI_zoom.py` & `Simba-UW-tf-dev-1.60.9/simba/roi_tools/ROI_zoom.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.60.7/simba/roi_tools/ROI_directing_analyzer.py` & `Simba-UW-tf-dev-1.60.9/simba/roi_tools/ROI_directing_analyzer.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.60.7/simba/roi_tools/ROI_move_shape.py` & `Simba-UW-tf-dev-1.60.9/simba/roi_tools/ROI_move_shape.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.60.7/simba/roi_tools/ROI_menus.py` & `Simba-UW-tf-dev-1.60.9/simba/roi_tools/ROI_menus.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.60.7/simba/roi_tools/ROI_clf_calculator.py` & `Simba-UW-tf-dev-1.60.9/simba/roi_tools/ROI_clf_calculator.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.60.7/simba/roi_tools/ROI_image.py` & `Simba-UW-tf-dev-1.60.9/simba/roi_tools/ROI_image.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.60.7/simba/pose_importers/sleap_csv_importer.py` & `Simba-UW-tf-dev-1.60.9/simba/pose_importers/madlc_importer.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,132 +1,120 @@
 __author__ = "Simon Nilsson"
 
-import pandas as pd
 import os
+import pandas as pd
 import numpy as np
 from copy import deepcopy
 
-from simba.data_processors.interpolation_smoothing import Interpolate, Smooth
-from simba.utils.read_write import find_all_videos_in_project
+from simba.data_processors.interpolation_smoothing import Smooth, Interpolate
+from simba.utils.errors import BodypartColumnNotFoundError
 from simba.mixins.config_reader import ConfigReader
+from simba.utils.read_write import write_df, get_video_meta_data, find_all_videos_in_project
+from simba.utils.enums import Formats, Methods
 from simba.mixins.pose_importer_mixin import PoseImporterMixin
-from simba.utils.read_write import write_df, find_video_of_file, get_video_meta_data, get_fn_ext
 from simba.utils.printing import stdout_success, SimbaTimer
-from simba.utils.enums import Methods
 
-class SLEAPImporterCSV(ConfigReader, PoseImporterMixin):
+class MADLCImporterH5(ConfigReader, PoseImporterMixin):
 
     """
-    Importing SLEAP pose-estimation data into SimBA project in ``CSV`` format.
-
-    .. note::
-      `Google Colab notebook for converting SLEAP .slp to CSV written by @Toshea111  <https://colab.research.google.com/drive/1EpyTKFHVMCqcb9Lj9vjMrriyaG9SvrPO?usp=sharing>`__.
-      `Example expected SLEAP csv data file for 5 animals / 4 pose-estimated body-parts  <https://github.com/sgoldenlab/simba/blob/master/misc/sleap_csv_example.csv>`__.
+    Importing multi-animal deeplabcut (maDLC) pose-estimation data (in H5 format)
+    into a SimBA project in parquet or CSV format.
 
     :parameter str config_path: path to SimBA project config file in Configparser format
-    :parameter str data_folder: Path to folder containing SLEAP data in `csv` format.
-    :parameter List[str] id_lst: Animal names. This will be ignored in one animal projects and default to ``Animal_1``.
-    :parameter str interpolation_settings: String defining the pose-estimation interpolation method. OPTIONS: 'None', 'Animal(s): Nearest',
+    :parameter str data_folder: Path to folder containing maDLC data in ``.h5`` format.
+    :parameter str file_type: Method used to perform pose-estimation in maDLC. OPTIONS: `skeleton`, `box`, `ellipse`.
+    :param List[str] id_lst: Names of animals.
+    :parameter str interpolation_setting: String defining the pose-estimation interpolation method. OPTIONS: 'None', 'Animal(s): Nearest',
         'Animal(s): Linear', 'Animal(s): Quadratic','Body-parts: Nearest', 'Body-parts: Linear',
         'Body-parts: Quadratic'.
-    :parameter str smoothing_settings: Dictionary defining the pose estimation smoothing method. EXAMPLE: {'Method': 'Savitzky Golay',
+    :parameter dict smoothing_settings: Dictionary defining the pose estimation smoothing method. EXAMPLE: {'Method': 'Savitzky Golay',
         'Parameters': {'Time_window': '200'}})
 
+    .. note::
+       `Multi-animal import tutorial <https://github.com/sgoldenlab/simba/blob/master/docs/Multi_animal_pose.md>`__.
+
+    Examples
+    -----
+    >>> _ = MADLCImporterH5(config_path=r'MyConfigPath', data_folder=r'maDLCDataFolder', file_type='ellipse', id_lst=['Animal_1', 'Animal_2'], interpolation_settings='None', smoothing_settings={'Method': 'None', 'Parameters': {'Time_window': '200'}}).run()
+
     References
     ----------
-    .. [1] Pereira et al., SLEAP: A deep learning system for multi-animal pose tracking, `Nature Methods`,
+    .. [1] Lauer et al., Multi-animal pose estimation, identification and tracking with DeepLabCut, `Nature Methods`,
            2022.
-
-    >>> sleap_csv_importer = SLEAPImporterCSV(config_path=r'project_folder/project_config.ini', data_folder=r'data_folder', actor_IDs=['Termite_1', 'Termite_2', 'Termite_3', 'Termite_4', 'Termite_5'], interpolation_settings="Body-parts: Nearest", smoothing_settings = {'Method': 'Savitzky Golay', 'Parameters': {'Time_window': '200'}})
-    >>> sleap_csv_importer.run()
     """
 
+
     def __init__(self,
                  config_path: str,
                  data_folder: str,
+                 file_type: str,
                  id_lst: list,
                  interpolation_settings: str,
                  smoothing_settings: dict):
 
         ConfigReader.__init__(self, config_path=config_path, read_video_info=False)
         PoseImporterMixin.__init__(self)
+
         self.interpolation_settings, self.smoothing_settings = interpolation_settings, smoothing_settings
         self.data_folder, self.id_lst = data_folder, id_lst
         self.import_log_path = os.path.join(self.logs_path, f'data_import_log_{self.datetime}.csv')
         self.video_paths = find_all_videos_in_project(videos_dir=self.video_dir)
-        self.input_data_paths = self.find_data_files(dir=self.data_folder, extensions=['.csv'])
-        self.data_and_videos_lk = self.link_video_paths_to_data_paths(data_paths=self.input_data_paths, video_paths=self.video_paths)
+        self.input_data_paths = self.find_data_files(dir=self.data_folder, extensions=Formats.DLC_FILETYPES.value[file_type])
+        self.data_and_videos_lk = self.link_video_paths_to_data_paths(data_paths=self.input_data_paths, video_paths=self.video_paths, str_splits=Formats.DLC_NETWORK_FILE_NAMES.value)
         if (self.pose_setting is Methods.USER_DEFINED.value):
             self.__update_config_animal_cnt()
         if self.animal_cnt > 1:
             self.check_multi_animal_status()
             self.animal_bp_dict = self.create_body_part_dictionary(self.multi_animal_status, self.id_lst, self.animal_cnt, self.x_cols, self.y_cols, self.p_cols, self.clr_lst)
             self.update_bp_headers_file()
         print(f'Importing {len(list(self.data_and_videos_lk.keys()))} file(s)...')
 
     def run(self):
-        for file_cnt, (video_name, video_data) in enumerate(self.data_and_videos_lk.items()):
-            print(f'Analysing {video_name}...')
+        import_log = pd.DataFrame(columns=['VIDEO', 'IMPORT_TIME', 'IMPORT_SOURCE', 'INTERPOLATION_SETTING', 'SMOOTHING_SETTING'])
+        for cnt, (video_name, video_data) in enumerate(self.data_and_videos_lk.items()):
             video_timer = SimbaTimer(start=True)
-            self.video_name = video_name
-            self.save_path = os.path.join(os.path.join(self.input_csv_dir, f'{self.video_name}.{self.file_type}'))
-            data_df = pd.read_csv(video_data['DATA'])
-            idx = data_df.iloc[:, :2]
-            idx['track'] = idx['track'].str.replace(r'[^\d.]+', '').astype(int)
-            data_df = data_df.iloc[:, 2:]
-            if self.animal_cnt > 1:
-                self.data_df = pd.DataFrame(self.transpose_multi_animal_table(data=data_df.values, idx=idx.values, animal_cnt=self.animal_cnt))
-                p_df = pd.DataFrame(1.0, index=self.data_df.index, columns=self.data_df.columns[1::2] + .5)
-                self.data_df = pd.concat([self.data_df, p_df], axis=1).sort_index(axis=1)
-                self.data_df.columns = self.bp_headers
-            else:
-                idx = list(idx.drop('track', axis=1)['frame_idx'])
-                self.data_df = data_df.set_index([idx]).sort_index()
-                self.data_df.columns = np.arange(len(self.data_df.columns))
-                self.data_df = self.data_df.reindex(range(self.data_df.index[0], self.data_df.index[-1] + 1), fill_value=0)
-                p_df = pd.DataFrame(1.0, index=self.data_df.index, columns=self.data_df.columns[1::2] + .5)
-                self.data_df = pd.concat([self.data_df, p_df], axis=1).sort_index(axis=1)
-                self.data_df.columns = self.bp_headers
-
+            self.add_spacer, self.frame_no, self.video_data, self.video_name = 2, 1, video_data, video_name
+            print(f'Processing {video_name} ...')
+            self.data_df = pd.read_hdf(video_data['DATA']).replace([np.inf, -np.inf], np.nan).fillna(0)
+            if len(self.data_df.columns) != len(self.bp_headers):
+                raise BodypartColumnNotFoundError(msg=f'The number of body-parts in data file {video_data["DATA"]} do not match the number of body-parts in your SimBA project. '
+                      f'The number of of body-parts expected by your SimBA project is {int(len(self.bp_headers) / 3)}. '
+                      f'The number of of body-parts contained in data file {video_data["DATA"]} is {int(len(self.data_df.columns) / 3)}. '
+                      f'Make sure you have specified the correct number of animals and body-parts in your project.')
+            self.data_df.columns = self.bp_headers
             self.out_df = deepcopy(self.data_df)
             if self.animal_cnt > 1:
                 self.initialize_multi_animal_ui(animal_bp_dict=self.animal_bp_dict,
                                                 video_info=get_video_meta_data(video_data['VIDEO']),
                                                 data_df=self.data_df,
                                                 video_path=video_data['VIDEO'])
                 self.multianimal_identification()
+            self.save_path = os.path.join(os.path.join(self.input_csv_dir, f'{self.video_name}.{self.file_type}'))
             write_df(df=self.out_df, file_type=self.file_type, save_path=self.save_path, multi_idx_header=True)
             if self.interpolation_settings != 'None':
                 self.__run_interpolation()
             if self.smoothing_settings['Method'] != 'None':
                 self.__run_smoothing()
             video_timer.stop_timer()
             stdout_success(msg=f'Video {video_name} data imported...', elapsed_time=video_timer.elapsed_time_str)
         self.timer.stop_timer()
-        stdout_success(msg=f'{len(list(self.data_and_videos_lk.keys()))} file(s) imported to the SimBA project (project_folder/csv/input_csv directory)')
+        stdout_success(msg='All maDLC H5 data files imported', elapsed_time=self.timer.elapsed_time_str)
 
     def __run_interpolation(self):
-        print(f'Interpolating missing values in video {self.video_name} (Method: {self.interpolation_settings})...')
-        _ = Interpolate(input_path=self.save_path, config_path=self.config_path, method=self.interpolation_settings, initial_import_multi_index=True)
+        print('Interpolating missing values in video {} (Method: {}) ...'.format(self.video_name, self.interpolation_settings))
+        _ = Interpolate(input_path=self.save_path,config_path=self.config_path, method=self.interpolation_settings, initial_import_multi_index=True)
 
     def __run_smoothing(self):
         print(f'Performing {self.smoothing_settings["Method"]} smoothing on video {self.video_name}...')
         Smooth(config_path=self.config_path,
                input_path=self.save_path,
                time_window=int(self.smoothing_settings['Parameters']['Time_window']),
                smoothing_method=self.smoothing_settings['Method'],
                initial_import_multi_index=True)
 
-# test = SLEAPImporterCSV(config_path=r'/Users/simon/Desktop/envs/troubleshooting/Hornet/project_folder/project_config.ini',
-#                  data_folder=r'/Users/simon/Desktop/envs/troubleshooting/Hornet_single_slp/import',
-#                  id_lst=['Hornet'],
-#                  interpolation_settings="Body-parts: Nearest",
-#                  smoothing_settings = {'Method': 'Savitzky Golay', 'Parameters': {'Time_window': '200'}})
+# test = MADLCImporterH5(config_path=r'/Users/simon/Desktop/envs/troubleshooting/two_black_animals_14bp/project_folder/project_config.ini',
+#                    data_folder=r'/Users/simon/Desktop/envs/troubleshooting/two_black_animals_14bp/h5',
+#                    file_type='ellipse',
+#                    id_lst=['Simon', 'JJ'],
+#                    interpolation_settings='Body-parts: Nearest',
+#                    smoothing_settings = {'Method': 'Savitzky Golay', 'Parameters': {'Time_window': '200'}})
 # test.run()
-
-
-# test = SLEAPImporterCSV(config_path=r'/Users/simon/Desktop/envs/troubleshooting/slp_1_animal_1_bp/project_folder',
-#                  data_folder='/Users/simon/Desktop/envs/troubleshooting/slp_1_animal_1_bp/import',
-#                  actor_IDs=['Termite_1'],
-#                  interpolation_settings="Body-parts: Nearest",
-#                  smoothing_settings = {'Method': 'Savitzky Golay', 'Parameters': {'Time_window': '200'}})
-# test.run()
```

### Comparing `Simba-UW-tf-dev-1.60.7/simba/pose_importers/misc/.DS_Store` & `Simba-UW-tf-dev-1.60.9/simba/pose_importers/misc/.DS_Store`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.60.7/simba/pose_importers/misc/apt_trk_importer.py` & `Simba-UW-tf-dev-1.60.9/simba/pose_importers/misc/apt_trk_importer.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.60.7/simba/pose_importers/read_DANNCE_mat.py` & `Simba-UW-tf-dev-1.60.9/simba/pose_importers/read_DANNCE_mat.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.60.7/simba/pose_importers/.DS_Store` & `Simba-UW-tf-dev-1.60.9/simba/pose_importers/.DS_Store`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.60.7/simba/pose_importers/sleap_h5_importer.py` & `Simba-UW-tf-dev-1.60.9/simba/pose_importers/sleap_h5_importer.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.60.7/simba/pose_importers/sleap_slp_importer.py` & `Simba-UW-tf-dev-1.60.9/simba/pose_importers/sleap_slp_importer.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.60.7/simba/pose_importers/import_mars.py` & `Simba-UW-tf-dev-1.60.9/simba/pose_importers/import_mars.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.60.7/simba/pose_importers/dlc_importer_csv.py` & `Simba-UW-tf-dev-1.60.9/simba/pose_importers/dlc_importer_csv.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.60.7/simba/pose_importers/trk_importer.py` & `Simba-UW-tf-dev-1.60.9/simba/pose_importers/trk_importer.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.60.7/simba/pose_configurations/.DS_Store` & `Simba-UW-tf-dev-1.60.9/simba/pose_configurations/.DS_Store`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.60.7/simba/pose_configurations/bp_names/.DS_Store` & `Simba-UW-tf-dev-1.60.9/simba/pose_configurations/bp_names/.DS_Store`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.60.7/simba/pose_configurations/bp_names/bp_names.csv` & `Simba-UW-tf-dev-1.60.9/simba/pose_configurations/bp_names/bp_names.csv`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.60.7/simba/pose_configurations/no_animals/.DS_Store` & `Simba-UW-tf-dev-1.60.9/simba/pose_configurations/no_animals/.DS_Store`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.60.7/simba/pose_configurations/configuration_names/.DS_Store` & `Simba-UW-tf-dev-1.60.9/simba/pose_configurations/configuration_names/.DS_Store`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.60.7/simba/pose_configurations/schematics/8.png` & `Simba-UW-tf-dev-1.60.9/simba/pose_configurations/schematics/8.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.60.7/simba/pose_configurations/schematics/9.png` & `Simba-UW-tf-dev-1.60.9/simba/pose_configurations/schematics/9.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.60.7/simba/pose_configurations/schematics/12.png` & `Simba-UW-tf-dev-1.60.9/simba/pose_configurations/schematics/12.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.60.7/simba/pose_configurations/schematics/11.png` & `Simba-UW-tf-dev-1.60.9/simba/pose_configurations/schematics/11.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.60.7/simba/pose_configurations/schematics/10.png` & `Simba-UW-tf-dev-1.60.9/simba/pose_configurations/schematics/10.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.60.7/simba/pose_configurations/schematics/4.png` & `Simba-UW-tf-dev-1.60.9/simba/pose_configurations/schematics/4.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.60.7/simba/pose_configurations/schematics/5.png` & `Simba-UW-tf-dev-1.60.9/simba/pose_configurations/schematics/5.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.60.7/simba/pose_configurations/schematics/7.png` & `Simba-UW-tf-dev-1.60.9/simba/pose_configurations/schematics/7.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.60.7/simba/pose_configurations/schematics/6.png` & `Simba-UW-tf-dev-1.60.9/simba/pose_configurations/schematics/6.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.60.7/simba/pose_configurations/schematics/2.png` & `Simba-UW-tf-dev-1.60.9/simba/pose_configurations/schematics/2.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.60.7/simba/pose_configurations/schematics/3.png` & `Simba-UW-tf-dev-1.60.9/simba/pose_configurations/schematics/3.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.60.7/simba/pose_configurations/schematics/1.png` & `Simba-UW-tf-dev-1.60.9/simba/pose_configurations/schematics/1.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.60.7/simba/video_processors/video_processing.py` & `Simba-UW-tf-dev-1.60.9/simba/video_processors/video_processing.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.60.7/simba/video_processors/.DS_Store` & `Simba-UW-tf-dev-1.60.9/simba/video_processors/.DS_Store`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.60.7/simba/video_processors/px_to_mm.py` & `Simba-UW-tf-dev-1.60.9/simba/video_processors/px_to_mm.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.60.7/simba/video_processors/batch_process_menus.py` & `Simba-UW-tf-dev-1.60.9/simba/video_processors/batch_process_menus.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.60.7/simba/video_processors/multi_cropper.py` & `Simba-UW-tf-dev-1.60.9/simba/video_processors/multi_cropper.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.60.7/simba/video_processors/extract_frames.py` & `Simba-UW-tf-dev-1.60.9/simba/video_processors/extract_frames.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.60.7/simba/video_processors/calculate_px_dist.py` & `Simba-UW-tf-dev-1.60.9/simba/video_processors/calculate_px_dist.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.60.7/simba/video_processors/extract_seqframes.py` & `Simba-UW-tf-dev-1.60.9/simba/video_processors/extract_seqframes.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.60.7/simba/video_processors/batch_process_create_ffmpeg_commands.py` & `Simba-UW-tf-dev-1.60.9/simba/video_processors/batch_process_create_ffmpeg_commands.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.60.7/simba/outlier_tools/outlier_corrector_movement.py` & `Simba-UW-tf-dev-1.60.9/simba/outlier_tools/outlier_corrector_movement.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.60.7/simba/outlier_tools/.DS_Store` & `Simba-UW-tf-dev-1.60.9/simba/outlier_tools/.DS_Store`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.60.7/simba/outlier_tools/outlier_corrector_location.py` & `Simba-UW-tf-dev-1.60.9/simba/outlier_tools/outlier_corrector_location.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.60.7/simba/outlier_tools/skip_outlier_correction.py` & `Simba-UW-tf-dev-1.60.9/simba/outlier_tools/skip_outlier_correction.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.60.7/simba/outlier_tools/.idea/outlier_scripts.iml` & `Simba-UW-tf-dev-1.60.9/simba/outlier_tools/.idea/outlier_scripts.iml`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.60.7/simba/outlier_tools/.idea/inspectionProfiles/Project_Default.xml` & `Simba-UW-tf-dev-1.60.9/simba/outlier_tools/.idea/inspectionProfiles/Project_Default.xml`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.60.7/simba/outlier_tools/.idea/workspace.xml` & `Simba-UW-tf-dev-1.60.9/simba/outlier_tools/.idea/workspace.xml`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.60.7/simba/SimBA.py` & `Simba-UW-tf-dev-1.60.9/simba/SimBA.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.60.7/simba/assets/unsupervised/.DS_Store` & `Simba-UW-tf-dev-1.60.9/simba/assets/unsupervised/.DS_Store`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.60.7/simba/assets/unsupervised/model_names.parquet` & `Simba-UW-tf-dev-1.60.9/simba/assets/unsupervised/model_names.parquet`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.60.7/simba/assets/unsupervised/features.csv` & `Simba-UW-tf-dev-1.60.9/simba/assets/unsupervised/features.csv`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.60.7/simba/assets/shap/down_arrow.jpg` & `Simba-UW-tf-dev-1.60.9/simba/assets/shap/down_arrow.jpg`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.60.7/simba/assets/shap/intruder_shape.jpg` & `Simba-UW-tf-dev-1.60.9/simba/assets/shap/intruder_shape.jpg`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.60.7/simba/assets/shap/feature_categories/shap_feature_categories.csv` & `Simba-UW-tf-dev-1.60.9/simba/assets/shap/feature_categories/shap_feature_categories.csv`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.60.7/simba/assets/shap/.DS_Store` & `Simba-UW-tf-dev-1.60.9/simba/assets/shap/.DS_Store`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.60.7/simba/assets/shap/resident_shape.jpg` & `Simba-UW-tf-dev-1.60.9/simba/assets/shap/resident_shape.jpg`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.60.7/simba/assets/shap/resident_intruder_shape.jpg` & `Simba-UW-tf-dev-1.60.9/simba/assets/shap/resident_intruder_shape.jpg`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.60.7/simba/assets/shap/animal_distances.jpg` & `Simba-UW-tf-dev-1.60.9/simba/assets/shap/animal_distances.jpg`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.60.7/simba/assets/shap/baseline_scale.jpg` & `Simba-UW-tf-dev-1.60.9/simba/assets/shap/baseline_scale.jpg`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.60.7/simba/assets/shap/ubuntu.regular.ttf` & `Simba-UW-tf-dev-1.60.9/simba/assets/shap/ubuntu.regular.ttf`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.60.7/simba/assets/shap/side_scale.jpg` & `Simba-UW-tf-dev-1.60.9/simba/assets/shap/side_scale.jpg`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.60.7/simba/assets/shap/UbuntuMono-Regular.ttf` & `Simba-UW-tf-dev-1.60.9/simba/assets/shap/UbuntuMono-Regular.ttf`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.60.7/simba/assets/shap/side_scale_5.jpg` & `Simba-UW-tf-dev-1.60.9/simba/assets/shap/side_scale_5.jpg`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.60.7/simba/assets/shap/intruder_movement.jpg` & `Simba-UW-tf-dev-1.60.9/simba/assets/shap/intruder_movement.jpg`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.60.7/simba/assets/shap/resident_movement.jpg` & `Simba-UW-tf-dev-1.60.9/simba/assets/shap/resident_movement.jpg`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.60.7/simba/assets/shap/color_bar.jpg` & `Simba-UW-tf-dev-1.60.9/simba/assets/shap/color_bar.jpg`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.60.7/simba/assets/shap/resident_intruder_movement.jpg` & `Simba-UW-tf-dev-1.60.9/simba/assets/shap/resident_intruder_movement.jpg`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.60.7/simba/assets/.DS_Store` & `Simba-UW-tf-dev-1.60.9/simba/assets/.DS_Store`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.60.7/simba/assets/lookups/.DS_Store` & `Simba-UW-tf-dev-1.60.9/simba/assets/lookups/.DS_Store`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.60.7/simba/assets/lookups/model_names.parquet` & `Simba-UW-tf-dev-1.60.9/simba/assets/lookups/model_names.parquet`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.60.7/simba/assets/lookups/feature_extraction_headers.csv` & `Simba-UW-tf-dev-1.60.9/simba/assets/lookups/feature_extraction_headers.csv`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.60.7/simba/assets/lookups/features.csv` & `Simba-UW-tf-dev-1.60.9/simba/assets/lookups/features.csv`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.60.7/simba/assets/lookups/unsupervised_example_x.csv` & `Simba-UW-tf-dev-1.60.9/simba/assets/lookups/unsupervised_example_x.csv`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.60.7/simba/assets/stl/operant_tray.stl` & `Simba-UW-tf-dev-1.60.9/simba/assets/stl/operant_tray.stl`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.60.7/simba/assets/stl/operant_lever.stl` & `Simba-UW-tf-dev-1.60.9/simba/assets/stl/operant_lever.stl`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.60.7/simba/assets/stl/operant_walls.stl` & `Simba-UW-tf-dev-1.60.9/simba/assets/stl/operant_walls.stl`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.60.7/simba/assets/stl/grid_floor.stl` & `Simba-UW-tf-dev-1.60.9/simba/assets/stl/grid_floor.stl`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.60.7/simba/assets/img/.DS_Store` & `Simba-UW-tf-dev-1.60.9/simba/assets/img/.DS_Store`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.60.7/simba/assets/img/about_me.png` & `Simba-UW-tf-dev-1.60.9/simba/assets/img/about_me.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.60.7/simba/assets/img/splash.mp4` & `Simba-UW-tf-dev-1.60.9/simba/assets/img/splash.mp4`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.60.7/simba/assets/img/bg_2.png` & `Simba-UW-tf-dev-1.60.9/simba/assets/img/bg_2.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.60.7/simba/assets/img/splash.pptx` & `Simba-UW-tf-dev-1.60.9/simba/assets/img/splash.pptx`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.60.7/simba/assets/img/bg.png` & `Simba-UW-tf-dev-1.60.9/simba/assets/img/bg.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.60.7/simba/assets/UbuntuMono-Regular.ttf` & `Simba-UW-tf-dev-1.60.9/simba/assets/UbuntuMono-Regular.ttf`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.60.7/simba/assets/icons/factory.png` & `Simba-UW-tf-dev-1.60.9/simba/assets/icons/factory.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.60.7/simba/assets/icons/cluster.png` & `Simba-UW-tf-dev-1.60.9/simba/assets/icons/cluster.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.60.7/simba/assets/icons/load.png` & `Simba-UW-tf-dev-1.60.9/simba/assets/icons/load.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.60.7/simba/assets/icons/gif.png` & `Simba-UW-tf-dev-1.60.9/simba/assets/icons/gif.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.60.7/simba/assets/icons/pose.png` & `Simba-UW-tf-dev-1.60.9/simba/assets/icons/pose.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.60.7/simba/assets/icons/features.png` & `Simba-UW-tf-dev-1.60.9/simba/assets/icons/features.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.60.7/simba/assets/icons/.DS_Store` & `Simba-UW-tf-dev-1.60.9/simba/assets/icons/.DS_Store`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.60.7/simba/assets/icons/settings.png` & `Simba-UW-tf-dev-1.60.9/simba/assets/icons/settings.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.60.7/simba/assets/icons/stopwatch.png` & `Simba-UW-tf-dev-1.60.9/simba/assets/icons/stopwatch.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.60.7/simba/assets/icons/link.png` & `Simba-UW-tf-dev-1.60.9/simba/assets/icons/link.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.60.7/simba/assets/icons/dash_simba.css` & `Simba-UW-tf-dev-1.60.9/simba/assets/icons/dash_simba.css`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.60.7/simba/assets/icons/documentation.png` & `Simba-UW-tf-dev-1.60.9/simba/assets/icons/documentation.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.60.7/simba/assets/icons/fps.png` & `Simba-UW-tf-dev-1.60.9/simba/assets/icons/fps.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.60.7/simba/assets/icons/dimensionality_reduction.png` & `Simba-UW-tf-dev-1.60.9/simba/assets/icons/dimensionality_reduction.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.60.7/simba/assets/icons/roi.png` & `Simba-UW-tf-dev-1.60.9/simba/assets/icons/roi.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.60.7/simba/assets/icons/superimpose.png` & `Simba-UW-tf-dev-1.60.9/simba/assets/icons/superimpose.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.60.7/simba/assets/icons/label.png` & `Simba-UW-tf-dev-1.60.9/simba/assets/icons/label.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.60.7/simba/assets/icons/change.png` & `Simba-UW-tf-dev-1.60.9/simba/assets/icons/change.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.60.7/simba/assets/icons/crop.png` & `Simba-UW-tf-dev-1.60.9/simba/assets/icons/crop.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.60.7/simba/assets/icons/rotate.png` & `Simba-UW-tf-dev-1.60.9/simba/assets/icons/rotate.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.60.7/simba/assets/icons/path.png` & `Simba-UW-tf-dev-1.60.9/simba/assets/icons/path.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.60.7/simba/assets/icons/clip.png` & `Simba-UW-tf-dev-1.60.9/simba/assets/icons/clip.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.60.7/simba/assets/icons/restart.png` & `Simba-UW-tf-dev-1.60.9/simba/assets/icons/restart.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.60.7/simba/assets/icons/calipher.png` & `Simba-UW-tf-dev-1.60.9/simba/assets/icons/calipher.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.60.7/simba/assets/icons/add_on.png` & `Simba-UW-tf-dev-1.60.9/simba/assets/icons/add_on.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.60.7/simba/assets/icons/create.png` & `Simba-UW-tf-dev-1.60.9/simba/assets/icons/create.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.60.7/simba/assets/icons/SimBA_logo.ico` & `Simba-UW-tf-dev-1.60.9/simba/assets/icons/SimBA_logo.ico`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.60.7/simba/assets/icons/print.png` & `Simba-UW-tf-dev-1.60.9/simba/assets/icons/print.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.60.7/simba/assets/icons/clf.png` & `Simba-UW-tf-dev-1.60.9/simba/assets/icons/clf.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.60.7/simba/assets/icons/concat_icons/mosaic.png` & `Simba-UW-tf-dev-1.60.9/simba/assets/icons/concat_icons/mosaic.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.60.7/simba/assets/icons/concat_icons/vertical.png` & `Simba-UW-tf-dev-1.60.9/simba/assets/icons/concat_icons/vertical.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.60.7/simba/assets/icons/concat_icons/horizontal.png` & `Simba-UW-tf-dev-1.60.9/simba/assets/icons/concat_icons/horizontal.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.60.7/simba/assets/icons/concat_icons/mixed_mosaic.png` & `Simba-UW-tf-dev-1.60.9/simba/assets/icons/concat_icons/mixed_mosaic.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.60.7/simba/assets/icons/merge.png` & `Simba-UW-tf-dev-1.60.9/simba/assets/icons/merge.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.60.7/simba/assets/icons/clean.png` & `Simba-UW-tf-dev-1.60.9/simba/assets/icons/clean.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.60.7/simba/assets/icons/clf_2.png` & `Simba-UW-tf-dev-1.60.9/simba/assets/icons/clf_2.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.60.7/simba/assets/icons/visualize.png` & `Simba-UW-tf-dev-1.60.9/simba/assets/icons/visualize.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.60.7/simba/assets/icons/concat.png` & `Simba-UW-tf-dev-1.60.9/simba/assets/icons/concat.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.60.7/simba/assets/icons/boris.png` & `Simba-UW-tf-dev-1.60.9/simba/assets/icons/boris.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.60.7/simba/assets/icons/frames.png` & `Simba-UW-tf-dev-1.60.9/simba/assets/icons/frames.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.60.7/simba/assets/icons/video.png` & `Simba-UW-tf-dev-1.60.9/simba/assets/icons/video.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.60.7/simba/assets/icons/sample.png` & `Simba-UW-tf-dev-1.60.9/simba/assets/icons/sample.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.60.7/simba/assets/icons/metrics.png` & `Simba-UW-tf-dev-1.60.9/simba/assets/icons/metrics.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.60.7/simba/assets/icons/grey.png` & `Simba-UW-tf-dev-1.60.9/simba/assets/icons/grey.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.60.7/simba/assets/icons/exit.png` & `Simba-UW-tf-dev-1.60.9/simba/assets/icons/exit.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.60.7/simba/assets/icons/outlier.png` & `Simba-UW-tf-dev-1.60.9/simba/assets/icons/outlier.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.60.7/simba/assets/icons/clahe.png` & `Simba-UW-tf-dev-1.60.9/simba/assets/icons/clahe.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.60.7/simba/assets/icons/trash.png` & `Simba-UW-tf-dev-1.60.9/simba/assets/icons/trash.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.60.7/simba/assets/icons/about.png` & `Simba-UW-tf-dev-1.60.9/simba/assets/icons/about.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.60.7/simba/assets/icons/convert.png` & `Simba-UW-tf-dev-1.60.9/simba/assets/icons/convert.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.60.7/simba/assets/icons/SimBA_logo.icns` & `Simba-UW-tf-dev-1.60.9/simba/assets/icons/SimBA_logo.icns`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.60.7/simba/assets/icons/reorganize.png` & `Simba-UW-tf-dev-1.60.9/simba/assets/icons/reorganize.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.60.7/simba/assets/icons/browse.png` & `Simba-UW-tf-dev-1.60.9/simba/assets/icons/browse.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.60.7/simba/assets/icons/SimBA_logo.png` & `Simba-UW-tf-dev-1.60.9/simba/assets/icons/SimBA_logo.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.60.7/simba/assets/icons/ethovision.png` & `Simba-UW-tf-dev-1.60.9/simba/assets/icons/ethovision.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.60.7/simba/assets/icons/close.png` & `Simba-UW-tf-dev-1.60.9/simba/assets/icons/close.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.60.7/simba/assets/dash_simba_base.css` & `Simba-UW-tf-dev-1.60.9/simba/assets/dash_simba_base.css`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.60.7/simba/assets/TheGoldenLab.PNG` & `Simba-UW-tf-dev-1.60.9/simba/assets/TheGoldenLab.PNG`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.60.7/Simba_UW_tf_dev.egg-info/PKG-INFO` & `Simba-UW-tf-dev-1.60.9/Simba_UW_tf_dev.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Simba-UW-tf-dev
-Version: 1.60.7
+Version: 1.60.9
 Summary: Toolkit for computer classification of complex social behaviors in experimental animals
 Home-page: https://github.com/sgoldenlab/simba
 Author: Simon Nilsson, Jia Jie Choong, Sophia Hwang
 Author-email: sronilsson@gmail.com
 License: GNU Lesser General Public License v3 (LGPLv3)
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

### Comparing `Simba-UW-tf-dev-1.60.7/Simba_UW_tf_dev.egg-info/SOURCES.txt` & `Simba-UW-tf-dev-1.60.9/Simba_UW_tf_dev.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -425,14 +425,15 @@
 simba/video_processors/calculate_px_dist.py
 simba/video_processors/extract_frames.py
 simba/video_processors/extract_seqframes.py
 simba/video_processors/multi_cropper.py
 simba/video_processors/px_to_mm.py
 simba/video_processors/video_processing.py
 tests/__init__.py
+tests/test_data_processors.py
 tests/test_featurizers.py
 tests/test_thirdparty_appenders.py
 tests/data/__init__.py
 tests/data/test_projects/__init__.py
 tests/data/test_projects/mouse_open_field/__init__.py
 tests/data/test_projects/two_c57/__init__.py
 tests/data/test_projects/zebrafish/__init__.py
```

### Comparing `Simba-UW-tf-dev-1.60.7/Simba_UW_tf_dev.egg-info/requires.txt` & `Simba-UW-tf-dev-1.60.9/Simba_UW_tf_dev.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.60.7/LICENSE.md` & `Simba-UW-tf-dev-1.60.9/LICENSE.md`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.60.7/tests/test_featurizers.py` & `Simba-UW-tf-dev-1.60.9/tests/test_featurizers.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.60.7/tests/data/test_projects/zebrafish/feature_file/fish_feature_extraction_092221.py` & `Simba-UW-tf-dev-1.60.9/tests/data/test_projects/zebrafish/feature_file/fish_feature_extraction_092221.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.60.7/tests/test_thirdparty_appenders.py` & `Simba-UW-tf-dev-1.60.9/tests/test_thirdparty_appenders.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.60.7/README.md` & `Simba-UW-tf-dev-1.60.9/README.md`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.60.7/setup.py` & `Simba-UW-tf-dev-1.60.9/setup.py`

 * *Files 7% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 Licensed under GNU Lesser General Public License v3.0
 """
 
 import setuptools
 
 setuptools.setup(
     name="Simba-UW-tf-dev",
-    version="1.60.7",
+    version="1.60.9",
     author="Simon Nilsson, Jia Jie Choong, Sophia Hwang",
     author_email="sronilsson@gmail.com",
     description="Toolkit for computer classification of complex social behaviors in experimental animals",
     url="https://github.com/sgoldenlab/simba",
     install_requires=['Pillow == 5.4.1', 'pyyaml == 5.3.1','shapely == 1.7','wxpython == 4.0.4',
               'dtreeviz == 0.8.1','eli5 == 0.10.1','graphviz == 0.11',
               'imblearn == 0.0','imgaug == 0.4.0','imutils == 0.5.2','matplotlib == 3.0.3', 'numpy == 1.18.1',
```

