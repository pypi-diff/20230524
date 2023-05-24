# Comparing `tmp/skelly_synchronize-2023.5.1016.tar.gz` & `tmp/skelly_synchronize-2023.5.1017.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "skelly_synchronize-2023.5.1016.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "skelly_synchronize-2023.5.1017.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `skelly_synchronize-2023.5.1016.tar` & `skelly_synchronize-2023.5.1017.tar`

### file list

```diff
@@ -1,36 +1,37 @@
--rw-r--r--   0        0        0       65 2023-05-22 19:18:07.980949 skelly_synchronize-2023.5.1016/.gitattributes
--rw-r--r--   0        0        0      146 2023-05-22 19:18:07.980949 skelly_synchronize-2023.5.1016/.github/workflows/lint-with-black.yml
--rw-r--r--   0        0        0     1087 2023-05-22 19:18:07.980949 skelly_synchronize-2023.5.1016/.github/workflows/publish_to_pypi_when_new_tag_is_pushed_to_main.yml
--rw-r--r--   0        0        0     1025 2023-05-22 19:18:07.980949 skelly_synchronize-2023.5.1016/.github/workflows/python-testing.yml
--rw-r--r--   0        0        0     2783 2023-05-22 19:18:07.980949 skelly_synchronize-2023.5.1016/.gitignore
--rw-r--r--   0        0        0    34523 2023-05-22 19:18:07.980949 skelly_synchronize-2023.5.1016/LICENSE
--rw-r--r--   0        0        0     3030 2023-05-22 19:18:07.980949 skelly_synchronize-2023.5.1016/README.md
--rw-r--r--   0        0        0     1626 2023-05-22 19:18:07.980949 skelly_synchronize-2023.5.1016/pyproject.toml
--rw-r--r--   0        0        0      132 2023-05-22 19:18:07.980949 skelly_synchronize-2023.5.1016/requirements.txt
--rw-r--r--   0        0        0       50 2023-05-22 19:18:07.980949 skelly_synchronize-2023.5.1016/setup.py
--rw-r--r--   0        0        0     1056 2023-05-22 19:18:07.980949 skelly_synchronize-2023.5.1016/skelly_synchronize/__init__.py
--rw-r--r--   0        0        0      333 2023-05-22 19:18:07.980949 skelly_synchronize-2023.5.1016/skelly_synchronize/__main__.py
--rw-r--r--   0        0        0     2192 2023-05-22 19:18:07.980949 skelly_synchronize-2023.5.1016/skelly_synchronize/core_processes/audio_utilities.py
--rw-r--r--   0        0        0     2758 2023-05-22 19:18:07.980949 skelly_synchronize-2023.5.1016/skelly_synchronize/core_processes/correlation_functions.py
--rw-r--r--   0        0        0      821 2023-05-22 19:18:07.980949 skelly_synchronize-2023.5.1016/skelly_synchronize/core_processes/debug_output.py
--rw-r--r--   0        0        0     1557 2023-05-22 19:18:07.980949 skelly_synchronize-2023.5.1016/skelly_synchronize/core_processes/video_functions/deffcode_functions.py
--rw-r--r--   0        0        0     2699 2023-05-22 19:18:07.980949 skelly_synchronize-2023.5.1016/skelly_synchronize/core_processes/video_functions/ffmpeg_functions.py
--rw-r--r--   0        0        0     4510 2023-05-22 19:18:07.980949 skelly_synchronize-2023.5.1016/skelly_synchronize/core_processes/video_functions/video_utilities.py
--rw-r--r--   0        0        0     1873 2023-05-22 19:18:07.980949 skelly_synchronize-2023.5.1016/skelly_synchronize/gui/skelly_synchronize_gui.py
--rw-r--r--   0        0        0      420 2023-05-22 19:18:07.980949 skelly_synchronize-2023.5.1016/skelly_synchronize/gui/widgets/run_button_widget.py
--rw-r--r--   0        0        0     4740 2023-05-22 19:18:07.980949 skelly_synchronize-2023.5.1016/skelly_synchronize/skelly_synchronize.py
--rw-r--r--   0        0        0        0 2023-05-22 19:18:07.980949 skelly_synchronize-2023.5.1016/skelly_synchronize/system/__init__.py
--rw-r--r--   0        0        0     1479 2023-05-22 19:18:07.980949 skelly_synchronize-2023.5.1016/skelly_synchronize/system/default_paths.py
--rw-r--r--   0        0        0     1402 2023-05-22 19:18:07.980949 skelly_synchronize-2023.5.1016/skelly_synchronize/system/logging_configuration.py
--rw-r--r--   0        0        0      323 2023-05-22 19:18:07.980949 skelly_synchronize-2023.5.1016/skelly_synchronize/system/paths_and_file_names.py
--rw-r--r--   0        0        0     1085 2023-05-22 19:18:07.980949 skelly_synchronize-2023.5.1016/skelly_synchronize/tests/conftest.py
--rw-r--r--   0        0        0      656 2023-05-22 19:18:07.984949 skelly_synchronize-2023.5.1016/skelly_synchronize/tests/test_normalize_lag_dict.py
--rw-r--r--   0        0        0      847 2023-05-22 19:18:07.984949 skelly_synchronize-2023.5.1016/skelly_synchronize/tests/test_trim_single_video_deffcode.py
--rw-r--r--   0        0        0      577 2023-05-22 19:18:07.984949 skelly_synchronize-2023.5.1016/skelly_synchronize/tests/utilities/check_list_values_are_equal.py
--rw-r--r--   0        0        0      262 2023-05-22 19:18:07.984949 skelly_synchronize-2023.5.1016/skelly_synchronize/tests/utilities/find_frame_count_of_video.py
--rw-r--r--   0        0        0     1263 2023-05-22 19:18:07.984949 skelly_synchronize-2023.5.1016/skelly_synchronize/tests/utilities/get_number_of_frames_of_videos_in_a_folder.py
--rw-r--r--   0        0        0     1061 2023-05-22 19:18:07.984949 skelly_synchronize-2023.5.1016/skelly_synchronize/tests/utilities/load_sample_data.py
--rw-r--r--   0        0        0     2048 2023-05-22 19:18:07.984949 skelly_synchronize-2023.5.1016/skelly_synchronize/utils/check_if_video_has_reversed_metadata.py
--rw-r--r--   0        0        0     1340 2023-05-22 19:18:07.984949 skelly_synchronize-2023.5.1016/skelly_synchronize/utils/get_video_files.py
--rw-r--r--   0        0        0     1103 2023-05-22 19:18:07.984949 skelly_synchronize-2023.5.1016/skelly_synchronize/utils/path_handling_utilities.py
--rw-r--r--   0        0        0     3935 1970-01-01 00:00:00.000000 skelly_synchronize-2023.5.1016/PKG-INFO
+-rw-r--r--   0        0        0       65 2023-05-24 17:56:05.918732 skelly_synchronize-2023.5.1017/.gitattributes
+-rw-r--r--   0        0        0      146 2023-05-24 17:56:05.918732 skelly_synchronize-2023.5.1017/.github/workflows/lint-with-black.yml
+-rw-r--r--   0        0        0     1087 2023-05-24 17:56:05.918732 skelly_synchronize-2023.5.1017/.github/workflows/publish_to_pypi_when_new_tag_is_pushed_to_main.yml
+-rw-r--r--   0        0        0     1025 2023-05-24 17:56:05.918732 skelly_synchronize-2023.5.1017/.github/workflows/python-testing.yml
+-rw-r--r--   0        0        0     2783 2023-05-24 17:56:05.918732 skelly_synchronize-2023.5.1017/.gitignore
+-rw-r--r--   0        0        0    34523 2023-05-24 17:56:05.918732 skelly_synchronize-2023.5.1017/LICENSE
+-rw-r--r--   0        0        0     3030 2023-05-24 17:56:05.918732 skelly_synchronize-2023.5.1017/README.md
+-rw-r--r--   0        0        0     1639 2023-05-24 17:56:05.918732 skelly_synchronize-2023.5.1017/pyproject.toml
+-rw-r--r--   0        0        0      150 2023-05-24 17:56:05.918732 skelly_synchronize-2023.5.1017/requirements.txt
+-rw-r--r--   0        0        0       50 2023-05-24 17:56:05.918732 skelly_synchronize-2023.5.1017/setup.py
+-rw-r--r--   0        0        0     1056 2023-05-24 17:56:05.918732 skelly_synchronize-2023.5.1017/skelly_synchronize/__init__.py
+-rw-r--r--   0        0        0      333 2023-05-24 17:56:05.918732 skelly_synchronize-2023.5.1017/skelly_synchronize/__main__.py
+-rw-r--r--   0        0        0     2192 2023-05-24 17:56:05.918732 skelly_synchronize-2023.5.1017/skelly_synchronize/core_processes/audio_utilities.py
+-rw-r--r--   0        0        0     2758 2023-05-24 17:56:05.918732 skelly_synchronize-2023.5.1017/skelly_synchronize/core_processes/correlation_functions.py
+-rw-r--r--   0        0        0      616 2023-05-24 17:56:05.922732 skelly_synchronize-2023.5.1017/skelly_synchronize/core_processes/debugging/debug_output.py
+-rw-r--r--   0        0        0     2697 2023-05-24 17:56:05.922732 skelly_synchronize-2023.5.1017/skelly_synchronize/core_processes/debugging/debug_plots.py
+-rw-r--r--   0        0        0     1557 2023-05-24 17:56:05.922732 skelly_synchronize-2023.5.1017/skelly_synchronize/core_processes/video_functions/deffcode_functions.py
+-rw-r--r--   0        0        0     2699 2023-05-24 17:56:05.922732 skelly_synchronize-2023.5.1017/skelly_synchronize/core_processes/video_functions/ffmpeg_functions.py
+-rw-r--r--   0        0        0     4510 2023-05-24 17:56:05.922732 skelly_synchronize-2023.5.1017/skelly_synchronize/core_processes/video_functions/video_utilities.py
+-rw-r--r--   0        0        0     1873 2023-05-24 17:56:05.922732 skelly_synchronize-2023.5.1017/skelly_synchronize/gui/skelly_synchronize_gui.py
+-rw-r--r--   0        0        0      420 2023-05-24 17:56:05.922732 skelly_synchronize-2023.5.1017/skelly_synchronize/gui/widgets/run_button_widget.py
+-rw-r--r--   0        0        0     4989 2023-05-24 17:56:05.922732 skelly_synchronize-2023.5.1017/skelly_synchronize/skelly_synchronize.py
+-rw-r--r--   0        0        0        0 2023-05-24 17:56:05.922732 skelly_synchronize-2023.5.1017/skelly_synchronize/system/__init__.py
+-rw-r--r--   0        0        0     1479 2023-05-24 17:56:05.922732 skelly_synchronize-2023.5.1017/skelly_synchronize/system/default_paths.py
+-rw-r--r--   0        0        0     1402 2023-05-24 17:56:05.922732 skelly_synchronize-2023.5.1017/skelly_synchronize/system/logging_configuration.py
+-rw-r--r--   0        0        0      555 2023-05-24 17:56:05.922732 skelly_synchronize-2023.5.1017/skelly_synchronize/system/paths_and_file_names.py
+-rw-r--r--   0        0        0     1085 2023-05-24 17:56:05.922732 skelly_synchronize-2023.5.1017/skelly_synchronize/tests/conftest.py
+-rw-r--r--   0        0        0      656 2023-05-24 17:56:05.922732 skelly_synchronize-2023.5.1017/skelly_synchronize/tests/test_normalize_lag_dict.py
+-rw-r--r--   0        0        0      847 2023-05-24 17:56:05.922732 skelly_synchronize-2023.5.1017/skelly_synchronize/tests/test_trim_single_video_deffcode.py
+-rw-r--r--   0        0        0      577 2023-05-24 17:56:05.922732 skelly_synchronize-2023.5.1017/skelly_synchronize/tests/utilities/check_list_values_are_equal.py
+-rw-r--r--   0        0        0      262 2023-05-24 17:56:05.922732 skelly_synchronize-2023.5.1017/skelly_synchronize/tests/utilities/find_frame_count_of_video.py
+-rw-r--r--   0        0        0     1263 2023-05-24 17:56:05.922732 skelly_synchronize-2023.5.1017/skelly_synchronize/tests/utilities/get_number_of_frames_of_videos_in_a_folder.py
+-rw-r--r--   0        0        0     1061 2023-05-24 17:56:05.922732 skelly_synchronize-2023.5.1017/skelly_synchronize/tests/utilities/load_sample_data.py
+-rw-r--r--   0        0        0     2048 2023-05-24 17:56:05.922732 skelly_synchronize-2023.5.1017/skelly_synchronize/utils/check_if_video_has_reversed_metadata.py
+-rw-r--r--   0        0        0     1340 2023-05-24 17:56:05.922732 skelly_synchronize-2023.5.1017/skelly_synchronize/utils/get_video_files.py
+-rw-r--r--   0        0        0     1103 2023-05-24 17:56:05.922732 skelly_synchronize-2023.5.1017/skelly_synchronize/utils/path_handling_utilities.py
+-rw-r--r--   0        0        0     3961 1970-01-01 00:00:00.000000 skelly_synchronize-2023.5.1017/PKG-INFO
```

### Comparing `skelly_synchronize-2023.5.1016/.github/workflows/publish_to_pypi_when_new_tag_is_pushed_to_main.yml` & `skelly_synchronize-2023.5.1017/.github/workflows/publish_to_pypi_when_new_tag_is_pushed_to_main.yml`

 * *Files identical despite different names*

### Comparing `skelly_synchronize-2023.5.1016/.github/workflows/python-testing.yml` & `skelly_synchronize-2023.5.1017/.github/workflows/python-testing.yml`

 * *Files identical despite different names*

### Comparing `skelly_synchronize-2023.5.1016/.gitignore` & `skelly_synchronize-2023.5.1017/.gitignore`

 * *Files identical despite different names*

### Comparing `skelly_synchronize-2023.5.1016/LICENSE` & `skelly_synchronize-2023.5.1017/LICENSE`

 * *Files identical despite different names*

### Comparing `skelly_synchronize-2023.5.1016/README.md` & `skelly_synchronize-2023.5.1017/README.md`

 * *Files identical despite different names*

### Comparing `skelly_synchronize-2023.5.1016/pyproject.toml` & `skelly_synchronize-2023.5.1017/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -31,25 +31,26 @@
 "PyQt6",
 "numpy",
 "scipy",
 "setuptools",
 "opencv-contrib-python==4.6.0.66",
 "deffcode",
 "toml",
+"matplotlib"
 ] #add additional dependencies here - try to pin versions as minimally as possible
 
 requires-python = ">=3.8"
 
 dynamic = ["version"]
 
 [project.optional-dependencies]
 dev = ["black", "bumpver", "isort", "pip-tools", "pytest"]
 
 [tool.bumpver] #bump the version by entering `bumpver update` in the terminal
-current_version = "v2023.05.1016"
+current_version = "v2023.05.1017"
 version_pattern = "vYYYY.0M.BUILD[-TAG]"
 commit_message  = "Bump version {old_version} -> {new_version}"
 commit          = true
 tag             = true
 push            = true
 
 [tool.bumpver.file_patterns]
```

### Comparing `skelly_synchronize-2023.5.1016/skelly_synchronize/__init__.py` & `skelly_synchronize-2023.5.1017/skelly_synchronize/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 """Top-level package for basic_template_repo."""
 
 __package_name__ = "skelly_synchronize"
-__version__ = "v2023.05.1016"
+__version__ = "v2023.05.1017"
 
 __author__ = """Philip Queen"""
 __email__ = "info@freemocap.org"
 __repo_owner_github_user_name__ = "freemocap"
 __repo_url__ = (
     f"https://github.com/{__repo_owner_github_user_name__}/{__package_name__}/"
 )
```

### Comparing `skelly_synchronize-2023.5.1016/skelly_synchronize/core_processes/audio_utilities.py` & `skelly_synchronize-2023.5.1017/skelly_synchronize/core_processes/audio_utilities.py`

 * *Files identical despite different names*

### Comparing `skelly_synchronize-2023.5.1016/skelly_synchronize/core_processes/correlation_functions.py` & `skelly_synchronize-2023.5.1017/skelly_synchronize/core_processes/correlation_functions.py`

 * *Files identical despite different names*

### Comparing `skelly_synchronize-2023.5.1016/skelly_synchronize/core_processes/debug_output.py` & `skelly_synchronize-2023.5.1017/skelly_synchronize/core_processes/debugging/debug_output.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,19 +1,15 @@
 import toml
 from pathlib import Path
 
 
 def save_dictionaries_to_toml(input_dictionaries: dict, output_file_path: Path):
     """Saves informative dictionaries to a TOML file for debugging"""
     with open(output_file_path, "w") as toml_file:
-        for idx, (name, dictionary) in enumerate(input_dictionaries.items()):
-            toml_file.write(f"[{name}]\n")
-            toml_file.write(toml.dumps(dictionary))
-            if idx < len(input_dictionaries) - 1:
-                toml_file.write("\n")
+        toml_file.write(toml.dumps(input_dictionaries))
 
 
 def remove_audio_files_from_audio_signal_dict(audio_signal_dictionary: dict) -> dict:
     """Remove audio files from audio signal dict to reduce unnessary storage"""
     for audio_info_dictionary in audio_signal_dictionary.values():
         audio_info_dictionary.pop("audio file")
```

### Comparing `skelly_synchronize-2023.5.1016/skelly_synchronize/core_processes/video_functions/deffcode_functions.py` & `skelly_synchronize-2023.5.1017/skelly_synchronize/core_processes/video_functions/deffcode_functions.py`

 * *Files identical despite different names*

### Comparing `skelly_synchronize-2023.5.1016/skelly_synchronize/core_processes/video_functions/ffmpeg_functions.py` & `skelly_synchronize-2023.5.1017/skelly_synchronize/core_processes/video_functions/ffmpeg_functions.py`

 * *Files identical despite different names*

### Comparing `skelly_synchronize-2023.5.1016/skelly_synchronize/core_processes/video_functions/video_utilities.py` & `skelly_synchronize-2023.5.1017/skelly_synchronize/core_processes/video_functions/video_utilities.py`

 * *Files identical despite different names*

### Comparing `skelly_synchronize-2023.5.1016/skelly_synchronize/gui/skelly_synchronize_gui.py` & `skelly_synchronize-2023.5.1017/skelly_synchronize/gui/skelly_synchronize_gui.py`

 * *Files identical despite different names*

### Comparing `skelly_synchronize-2023.5.1016/skelly_synchronize/skelly_synchronize.py` & `skelly_synchronize-2023.5.1017/skelly_synchronize/skelly_synchronize.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,40 +1,44 @@
 import time
 import logging
 from pathlib import Path
-from skelly_synchronize.core_processes.debug_output import (
-    remove_audio_files_from_audio_signal_dict,
-    save_dictionaries_to_toml,
-)
-
+from skelly_synchronize.core_processes.debugging.debug_plots import create_debug_plots
 
 logging.basicConfig(level=logging.INFO)
 
 from skelly_synchronize.utils.get_video_files import get_video_file_list
 from skelly_synchronize.core_processes.audio_utilities import (
     extract_audio_files,
     get_audio_sample_rates,
 )
 from skelly_synchronize.core_processes.correlation_functions import find_lags
 from skelly_synchronize.core_processes.video_functions.video_utilities import (
     get_fps_list,
     create_video_info_dict,
     trim_videos,
 )
+from skelly_synchronize.core_processes.debugging.debug_output import (
+    remove_audio_files_from_audio_signal_dict,
+    save_dictionaries_to_toml,
+)
 from skelly_synchronize.utils.path_handling_utilities import (
     create_directory,
 )
 from skelly_synchronize.tests.utilities.check_list_values_are_equal import (
     check_list_values_are_equal,
 )
 from skelly_synchronize.tests.utilities.get_number_of_frames_of_videos_in_a_folder import (
     get_number_of_frames_of_videos_in_a_folder,
 )
 from skelly_synchronize.system.paths_and_file_names import (
+    AUDIO_NAME,
     DEBUG_TOML_NAME,
+    LAG_DICTIONARY_NAME,
+    RAW_VIDEO_NAME,
+    SYNCHRONIZED_VIDEO_NAME,
     SYNCHRONIZED_VIDEOS_FOLDER_NAME,
     AUDIO_FILES_FOLDER_NAME,
 )
 
 
 def synchronize_videos_from_audio(
     raw_video_folder_path: Path,
@@ -105,24 +109,26 @@
         video_filepath_list=get_video_file_list(
             synchronized_video_folder_path, file_type=file_type
         )
     )
 
     save_dictionaries_to_toml(
         input_dictionaries={
-            "Raw video information": video_info_dict,
-            "Synchronized video information": synchronized_video_info_dict,
-            "Audio information": remove_audio_files_from_audio_signal_dict(
+            RAW_VIDEO_NAME: video_info_dict,
+            SYNCHRONIZED_VIDEO_NAME: synchronized_video_info_dict,
+            AUDIO_NAME: remove_audio_files_from_audio_signal_dict(
                 audio_signal_dictionary=audio_signal_dict
             ),
-            "Lag dictionary": lag_dict,
+            LAG_DICTIONARY_NAME: lag_dict,
         },
         output_file_path=synchronized_video_folder_path / DEBUG_TOML_NAME,
     )
 
+    create_debug_plots(synchronized_video_folder_path=synchronized_video_folder_path)
+
     end_timer = time.time()
 
     logging.info(f"Elapsed processing time in seconds: {end_timer - start_timer}")
 
     return synchronized_video_folder_path
```

### Comparing `skelly_synchronize-2023.5.1016/skelly_synchronize/system/default_paths.py` & `skelly_synchronize-2023.5.1017/skelly_synchronize/system/default_paths.py`

 * *Files identical despite different names*

### Comparing `skelly_synchronize-2023.5.1016/skelly_synchronize/system/logging_configuration.py` & `skelly_synchronize-2023.5.1017/skelly_synchronize/system/logging_configuration.py`

 * *Files identical despite different names*

### Comparing `skelly_synchronize-2023.5.1016/skelly_synchronize/tests/conftest.py` & `skelly_synchronize-2023.5.1017/skelly_synchronize/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `skelly_synchronize-2023.5.1016/skelly_synchronize/tests/test_normalize_lag_dict.py` & `skelly_synchronize-2023.5.1017/skelly_synchronize/tests/test_normalize_lag_dict.py`

 * *Files identical despite different names*

### Comparing `skelly_synchronize-2023.5.1016/skelly_synchronize/tests/test_trim_single_video_deffcode.py` & `skelly_synchronize-2023.5.1017/skelly_synchronize/tests/test_trim_single_video_deffcode.py`

 * *Files identical despite different names*

### Comparing `skelly_synchronize-2023.5.1016/skelly_synchronize/tests/utilities/check_list_values_are_equal.py` & `skelly_synchronize-2023.5.1017/skelly_synchronize/tests/utilities/check_list_values_are_equal.py`

 * *Files identical despite different names*

### Comparing `skelly_synchronize-2023.5.1016/skelly_synchronize/tests/utilities/get_number_of_frames_of_videos_in_a_folder.py` & `skelly_synchronize-2023.5.1017/skelly_synchronize/tests/utilities/get_number_of_frames_of_videos_in_a_folder.py`

 * *Files identical despite different names*

### Comparing `skelly_synchronize-2023.5.1016/skelly_synchronize/tests/utilities/load_sample_data.py` & `skelly_synchronize-2023.5.1017/skelly_synchronize/tests/utilities/load_sample_data.py`

 * *Files identical despite different names*

### Comparing `skelly_synchronize-2023.5.1016/skelly_synchronize/utils/check_if_video_has_reversed_metadata.py` & `skelly_synchronize-2023.5.1017/skelly_synchronize/utils/check_if_video_has_reversed_metadata.py`

 * *Files identical despite different names*

### Comparing `skelly_synchronize-2023.5.1016/skelly_synchronize/utils/get_video_files.py` & `skelly_synchronize-2023.5.1017/skelly_synchronize/utils/get_video_files.py`

 * *Files identical despite different names*

### Comparing `skelly_synchronize-2023.5.1016/skelly_synchronize/utils/path_handling_utilities.py` & `skelly_synchronize-2023.5.1017/skelly_synchronize/utils/path_handling_utilities.py`

 * *Files identical despite different names*

### Comparing `skelly_synchronize-2023.5.1016/PKG-INFO` & `skelly_synchronize-2023.5.1017/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: skelly_synchronize
-Version: 2023.5.1016
+Version: 2023.5.1017
 Summary: Basic template of a python repository
 Keywords: basic,template,python,repository
 Author-email: skelly_synchronize <info@freemocap.org>
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Classifier: License :: OSI Approved :: GNU Affero General Public License v3 or later (AGPLv3+)
 Classifier: Programming Language :: Python
@@ -14,14 +14,15 @@
 Requires-Dist: PyQt6
 Requires-Dist: numpy
 Requires-Dist: scipy
 Requires-Dist: setuptools
 Requires-Dist: opencv-contrib-python==4.6.0.66
 Requires-Dist: deffcode
 Requires-Dist: toml
+Requires-Dist: matplotlib
 Requires-Dist: black ; extra == "dev"
 Requires-Dist: bumpver ; extra == "dev"
 Requires-Dist: isort ; extra == "dev"
 Requires-Dist: pip-tools ; extra == "dev"
 Requires-Dist: pytest ; extra == "dev"
 Provides-Extra: dev
```

