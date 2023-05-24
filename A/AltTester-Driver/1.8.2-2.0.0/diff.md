# Comparing `tmp/AltTester-Driver-1.8.2.tar.gz` & `tmp/AltTester-Driver-2.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "AltTester-Driver-1.8.2.tar", last modified: Wed Feb  1 16:02:53 2023, max compression
+gzip compressed data, was "AltTester-Driver-2.0.0.tar", last modified: Wed May 24 14:53:54 2023, max compression
```

## Comparing `AltTester-Driver-1.8.2.tar` & `AltTester-Driver-2.0.0.tar`

### file list

```diff
@@ -1,119 +1,120 @@
-drwxr-xr-x   0 gitlabrunner   (501) staff       (20)        0 2023-02-01 16:02:53.278366 AltTester-Driver-1.8.2/
-drwxr-xr-x   0 gitlabrunner   (501) staff       (20)        0 2023-02-01 16:02:53.200484 AltTester-Driver-1.8.2/AltTester_Driver.egg-info/
--rw-r--r--   0 gitlabrunner   (501) staff       (20)     3410 2023-02-01 16:02:53.000000 AltTester-Driver-1.8.2/AltTester_Driver.egg-info/PKG-INFO
--rw-r--r--   0 gitlabrunner   (501) staff       (20)     4426 2023-02-01 16:02:53.000000 AltTester-Driver-1.8.2/AltTester_Driver.egg-info/SOURCES.txt
--rw-r--r--   0 gitlabrunner   (501) staff       (20)        1 2023-02-01 16:02:53.000000 AltTester-Driver-1.8.2/AltTester_Driver.egg-info/dependency_links.txt
--rw-r--r--   0 gitlabrunner   (501) staff       (20)        1 2023-02-01 16:02:52.000000 AltTester-Driver-1.8.2/AltTester_Driver.egg-info/not-zip-safe
--rw-r--r--   0 gitlabrunner   (501) staff       (20)       51 2023-02-01 16:02:53.000000 AltTester-Driver-1.8.2/AltTester_Driver.egg-info/requires.txt
--rw-r--r--   0 gitlabrunner   (501) staff       (20)       16 2023-02-01 16:02:53.000000 AltTester-Driver-1.8.2/AltTester_Driver.egg-info/top_level.txt
--rw-r--r--   0 gitlabrunner   (501) staff       (20)       56 2022-12-08 10:54:36.000000 AltTester-Driver-1.8.2/MANIFEST.in
--rw-r--r--   0 gitlabrunner   (501) staff       (20)     3410 2023-02-01 16:02:53.277792 AltTester-Driver-1.8.2/PKG-INFO
--rw-r--r--   0 gitlabrunner   (501) staff       (20)     1564 2023-01-18 15:38:48.000000 AltTester-Driver-1.8.2/README.md
-drwxr-xr-x   0 gitlabrunner   (501) staff       (20)        0 2023-02-01 16:02:53.210116 AltTester-Driver-1.8.2/alttester/
--rw-r--r--   0 gitlabrunner   (501) staff       (20)      347 2023-01-31 05:41:51.000000 AltTester-Driver-1.8.2/alttester/__init__.py
--rw-r--r--   0 gitlabrunner   (501) staff       (20)       18 2023-02-01 14:08:08.000000 AltTester-Driver-1.8.2/alttester/__version__.py
--rw-r--r--   0 gitlabrunner   (501) staff       (20)     9379 2023-01-31 05:41:51.000000 AltTester-Driver-1.8.2/alttester/_websocket.py
--rw-r--r--   0 gitlabrunner   (501) staff       (20)    35659 2023-01-31 05:41:51.000000 AltTester-Driver-1.8.2/alttester/altdriver.py
--rw-r--r--   0 gitlabrunner   (501) staff       (20)     9901 2023-01-18 15:38:48.000000 AltTester-Driver-1.8.2/alttester/altobject.py
--rw-r--r--   0 gitlabrunner   (501) staff       (20)      277 2023-02-01 12:34:37.000000 AltTester-Driver-1.8.2/alttester/by.py
-drwxr-xr-x   0 gitlabrunner   (501) staff       (20)        0 2023-02-01 16:02:53.215309 AltTester-Driver-1.8.2/alttester/commands/
-drwxr-xr-x   0 gitlabrunner   (501) staff       (20)        0 2023-02-01 16:02:53.219968 AltTester-Driver-1.8.2/alttester/commands/AltTesterCommands/
--rw-r--r--   0 gitlabrunner   (501) staff       (20)      290 2023-01-18 15:38:48.000000 AltTester-Driver-1.8.2/alttester/commands/AltTesterCommands/__init__.py
--rw-r--r--   0 gitlabrunner   (501) staff       (20)     1770 2023-01-18 15:38:48.000000 AltTester-Driver-1.8.2/alttester/commands/AltTesterCommands/add_notification_listener.py
--rw-r--r--   0 gitlabrunner   (501) staff       (20)     1102 2023-01-18 15:38:48.000000 AltTester-Driver-1.8.2/alttester/commands/AltTesterCommands/remove_notification_listener.py
--rw-r--r--   0 gitlabrunner   (501) staff       (20)      408 2023-01-31 05:41:51.000000 AltTester-Driver-1.8.2/alttester/commands/AltTesterCommands/reset_input.py
--rw-r--r--   0 gitlabrunner   (501) staff       (20)     1208 2023-01-18 15:38:48.000000 AltTester-Driver-1.8.2/alttester/commands/AltTesterCommands/set_server_logging.py
-drwxr-xr-x   0 gitlabrunner   (501) staff       (20)        0 2023-02-01 16:02:53.227083 AltTester-Driver-1.8.2/alttester/commands/FindObjects/
--rw-r--r--   0 gitlabrunner   (501) staff       (20)      548 2023-01-18 15:38:48.000000 AltTester-Driver-1.8.2/alttester/commands/FindObjects/__init__.py
--rw-r--r--   0 gitlabrunner   (501) staff       (20)     1342 2023-01-18 15:38:48.000000 AltTester-Driver-1.8.2/alttester/commands/FindObjects/find_object.py
--rw-r--r--   0 gitlabrunner   (501) staff       (20)      547 2023-01-18 15:38:48.000000 AltTester-Driver-1.8.2/alttester/commands/FindObjects/find_object_at_coordinates.py
--rw-r--r--   0 gitlabrunner   (501) staff       (20)     1363 2023-01-18 15:38:48.000000 AltTester-Driver-1.8.2/alttester/commands/FindObjects/find_object_which_contains.py
--rw-r--r--   0 gitlabrunner   (501) staff       (20)     1343 2023-01-18 15:38:48.000000 AltTester-Driver-1.8.2/alttester/commands/FindObjects/find_objects.py
--rw-r--r--   0 gitlabrunner   (501) staff       (20)     1364 2023-01-18 15:38:48.000000 AltTester-Driver-1.8.2/alttester/commands/FindObjects/find_objects_which_contains.py
--rw-r--r--   0 gitlabrunner   (501) staff       (20)     1796 2023-01-18 15:38:48.000000 AltTester-Driver-1.8.2/alttester/commands/FindObjects/wait_for_object.py
--rw-r--r--   0 gitlabrunner   (501) staff       (20)     1898 2023-01-18 15:38:48.000000 AltTester-Driver-1.8.2/alttester/commands/FindObjects/wait_for_object_to_not_be_present.py
--rw-r--r--   0 gitlabrunner   (501) staff       (20)     1954 2023-01-18 15:38:48.000000 AltTester-Driver-1.8.2/alttester/commands/FindObjects/wait_for_object_which_contains.py
-drwxr-xr-x   0 gitlabrunner   (501) staff       (20)        0 2023-02-01 16:02:53.238954 AltTester-Driver-1.8.2/alttester/commands/InputActions/
--rw-r--r--   0 gitlabrunner   (501) staff       (20)      747 2023-01-18 15:38:48.000000 AltTester-Driver-1.8.2/alttester/commands/InputActions/__init__.py
--rw-r--r--   0 gitlabrunner   (501) staff       (20)      525 2023-01-18 15:38:48.000000 AltTester-Driver-1.8.2/alttester/commands/InputActions/begin_touch.py
--rw-r--r--   0 gitlabrunner   (501) staff       (20)      914 2023-01-18 15:38:48.000000 AltTester-Driver-1.8.2/alttester/commands/InputActions/click_coordinates.py
--rw-r--r--   0 gitlabrunner   (501) staff       (20)      519 2023-01-18 15:38:48.000000 AltTester-Driver-1.8.2/alttester/commands/InputActions/end_touch.py
--rw-r--r--   0 gitlabrunner   (501) staff       (20)     1251 2023-01-18 15:38:48.000000 AltTester-Driver-1.8.2/alttester/commands/InputActions/keys_down.py
--rw-r--r--   0 gitlabrunner   (501) staff       (20)     1182 2023-01-18 15:38:48.000000 AltTester-Driver-1.8.2/alttester/commands/InputActions/keys_up.py
--rw-r--r--   0 gitlabrunner   (501) staff       (20)      834 2023-01-18 15:38:48.000000 AltTester-Driver-1.8.2/alttester/commands/InputActions/move_mouse.py
--rw-r--r--   0 gitlabrunner   (501) staff       (20)      647 2023-01-18 15:38:48.000000 AltTester-Driver-1.8.2/alttester/commands/InputActions/move_touch.py
--rw-r--r--   0 gitlabrunner   (501) staff       (20)      815 2023-01-18 15:38:48.000000 AltTester-Driver-1.8.2/alttester/commands/InputActions/multi_point_swipe.py
--rw-r--r--   0 gitlabrunner   (501) staff       (20)     1539 2023-01-18 15:38:48.000000 AltTester-Driver-1.8.2/alttester/commands/InputActions/press_keys.py
--rw-r--r--   0 gitlabrunner   (501) staff       (20)      923 2023-01-18 15:38:48.000000 AltTester-Driver-1.8.2/alttester/commands/InputActions/scroll_mouse.py
--rw-r--r--   0 gitlabrunner   (501) staff       (20)      874 2023-01-18 15:38:48.000000 AltTester-Driver-1.8.2/alttester/commands/InputActions/swipe.py
--rw-r--r--   0 gitlabrunner   (501) staff       (20)      910 2023-01-18 15:38:48.000000 AltTester-Driver-1.8.2/alttester/commands/InputActions/tap_coordinates.py
--rw-r--r--   0 gitlabrunner   (501) staff       (20)      832 2023-01-18 15:38:48.000000 AltTester-Driver-1.8.2/alttester/commands/InputActions/tilt.py
-drwxr-xr-x   0 gitlabrunner   (501) staff       (20)        0 2023-02-01 16:02:53.243571 AltTester-Driver-1.8.2/alttester/commands/Notifications/
--rw-r--r--   0 gitlabrunner   (501) staff       (20)      449 2023-01-18 15:38:48.000000 AltTester-Driver-1.8.2/alttester/commands/Notifications/__init__.py
--rw-r--r--   0 gitlabrunner   (501) staff       (20)      879 2023-01-18 15:38:48.000000 AltTester-Driver-1.8.2/alttester/commands/Notifications/base_notification_callbacks.py
--rw-r--r--   0 gitlabrunner   (501) staff       (20)      194 2023-01-18 15:38:48.000000 AltTester-Driver-1.8.2/alttester/commands/Notifications/load_scene_mode.py
--rw-r--r--   0 gitlabrunner   (501) staff       (20)      168 2023-01-18 15:38:48.000000 AltTester-Driver-1.8.2/alttester/commands/Notifications/load_scene_notification_result.py
--rw-r--r--   0 gitlabrunner   (501) staff       (20)      178 2023-01-18 15:38:48.000000 AltTester-Driver-1.8.2/alttester/commands/Notifications/log_notification_result.py
--rw-r--r--   0 gitlabrunner   (501) staff       (20)      138 2023-01-18 15:38:48.000000 AltTester-Driver-1.8.2/alttester/commands/Notifications/notification_type.py
-drwxr-xr-x   0 gitlabrunner   (501) staff       (20)        0 2023-02-01 16:02:53.253539 AltTester-Driver-1.8.2/alttester/commands/ObjectCommands/
--rw-r--r--   0 gitlabrunner   (501) staff       (20)      748 2023-01-18 15:38:48.000000 AltTester-Driver-1.8.2/alttester/commands/ObjectCommands/__init__.py
--rw-r--r--   0 gitlabrunner   (501) staff       (20)     1887 2023-01-18 15:38:48.000000 AltTester-Driver-1.8.2/alttester/commands/ObjectCommands/call_method.py
--rw-r--r--   0 gitlabrunner   (501) staff       (20)      799 2023-01-18 15:38:48.000000 AltTester-Driver-1.8.2/alttester/commands/ObjectCommands/click_element.py
--rw-r--r--   0 gitlabrunner   (501) staff       (20)      509 2023-01-18 15:38:48.000000 AltTester-Driver-1.8.2/alttester/commands/ObjectCommands/get_all_components.py
--rw-r--r--   0 gitlabrunner   (501) staff       (20)      905 2023-01-18 15:38:48.000000 AltTester-Driver-1.8.2/alttester/commands/ObjectCommands/get_component_property.py
--rw-r--r--   0 gitlabrunner   (501) staff       (20)      475 2023-01-18 15:38:48.000000 AltTester-Driver-1.8.2/alttester/commands/ObjectCommands/get_text.py
--rw-r--r--   0 gitlabrunner   (501) staff       (20)      509 2023-01-18 15:38:48.000000 AltTester-Driver-1.8.2/alttester/commands/ObjectCommands/pointer_down.py
--rw-r--r--   0 gitlabrunner   (501) staff       (20)      509 2023-01-18 15:38:48.000000 AltTester-Driver-1.8.2/alttester/commands/ObjectCommands/pointer_enter.py
--rw-r--r--   0 gitlabrunner   (501) staff       (20)      489 2023-01-18 15:38:48.000000 AltTester-Driver-1.8.2/alttester/commands/ObjectCommands/pointer_exit.py
--rw-r--r--   0 gitlabrunner   (501) staff       (20)      489 2023-01-18 15:38:48.000000 AltTester-Driver-1.8.2/alttester/commands/ObjectCommands/pointer_up.py
--rw-r--r--   0 gitlabrunner   (501) staff       (20)      910 2023-01-18 15:38:48.000000 AltTester-Driver-1.8.2/alttester/commands/ObjectCommands/set_component_property.py
--rw-r--r--   0 gitlabrunner   (501) staff       (20)      621 2023-01-18 15:38:48.000000 AltTester-Driver-1.8.2/alttester/commands/ObjectCommands/set_text.py
--rw-r--r--   0 gitlabrunner   (501) staff       (20)      795 2023-01-18 15:38:48.000000 AltTester-Driver-1.8.2/alttester/commands/ObjectCommands/tap_element.py
-drwxr-xr-x   0 gitlabrunner   (501) staff       (20)        0 2023-02-01 16:02:53.263403 AltTester-Driver-1.8.2/alttester/commands/UnityCommands/
--rw-r--r--   0 gitlabrunner   (501) staff       (20)      878 2023-01-18 15:38:48.000000 AltTester-Driver-1.8.2/alttester/commands/UnityCommands/__init__.py
--rw-r--r--   0 gitlabrunner   (501) staff       (20)      240 2023-01-18 15:38:48.000000 AltTester-Driver-1.8.2/alttester/commands/UnityCommands/delete_player_pref.py
--rw-r--r--   0 gitlabrunner   (501) staff       (20)      479 2023-01-18 15:38:48.000000 AltTester-Driver-1.8.2/alttester/commands/UnityCommands/delete_player_pref_key.py
--rw-r--r--   0 gitlabrunner   (501) staff       (20)      244 2023-01-18 15:38:48.000000 AltTester-Driver-1.8.2/alttester/commands/UnityCommands/get_all_loaded_scenes.py
--rw-r--r--   0 gitlabrunner   (501) staff       (20)      274 2023-01-18 15:38:48.000000 AltTester-Driver-1.8.2/alttester/commands/UnityCommands/get_current_scene.py
--rw-r--r--   0 gitlabrunner   (501) staff       (20)      968 2023-01-18 15:38:48.000000 AltTester-Driver-1.8.2/alttester/commands/UnityCommands/get_player_pref_key.py
--rw-r--r--   0 gitlabrunner   (501) staff       (20)      375 2023-01-18 15:38:48.000000 AltTester-Driver-1.8.2/alttester/commands/UnityCommands/get_time_scale.py
--rw-r--r--   0 gitlabrunner   (501) staff       (20)      709 2023-01-18 15:38:48.000000 AltTester-Driver-1.8.2/alttester/commands/UnityCommands/load_scene.py
--rw-r--r--   0 gitlabrunner   (501) staff       (20)     1337 2023-01-18 15:38:48.000000 AltTester-Driver-1.8.2/alttester/commands/UnityCommands/set_player_pref_key.py
--rw-r--r--   0 gitlabrunner   (501) staff       (20)      710 2023-01-18 15:38:48.000000 AltTester-Driver-1.8.2/alttester/commands/UnityCommands/set_time_scale.py
--rw-r--r--   0 gitlabrunner   (501) staff       (20)      637 2023-01-18 15:38:48.000000 AltTester-Driver-1.8.2/alttester/commands/UnityCommands/unload_scene.py
--rw-r--r--   0 gitlabrunner   (501) staff       (20)     1010 2023-01-18 15:38:48.000000 AltTester-Driver-1.8.2/alttester/commands/UnityCommands/wait_for_current_scene_to_be.py
--rw-r--r--   0 gitlabrunner   (501) staff       (20)      556 2023-01-18 15:38:48.000000 AltTester-Driver-1.8.2/alttester/commands/__init__.py
--rw-r--r--   0 gitlabrunner   (501) staff       (20)     7279 2023-01-18 15:38:48.000000 AltTester-Driver-1.8.2/alttester/commands/base_command.py
--rw-r--r--   0 gitlabrunner   (501) staff       (20)      487 2023-01-18 15:38:48.000000 AltTester-Driver-1.8.2/alttester/commands/get_png_screenshot.py
--rw-r--r--   0 gitlabrunner   (501) staff       (20)      240 2023-01-18 15:38:48.000000 AltTester-Driver-1.8.2/alttester/commands/get_server_version.py
--rw-r--r--   0 gitlabrunner   (501) staff       (20)      874 2023-01-18 15:38:48.000000 AltTester-Driver-1.8.2/alttester/commands/get_static_property.py
--rw-r--r--   0 gitlabrunner   (501) staff       (20)      854 2023-01-18 15:38:48.000000 AltTester-Driver-1.8.2/alttester/commands/set_static_property.py
--rw-r--r--   0 gitlabrunner   (501) staff       (20)     3442 2023-01-18 15:38:48.000000 AltTester-Driver-1.8.2/alttester/exceptions.py
--rw-r--r--   0 gitlabrunner   (501) staff       (20)     7502 2023-01-18 15:38:48.000000 AltTester-Driver-1.8.2/alttester/keycode.py
--rw-r--r--   0 gitlabrunner   (501) staff       (20)      333 2023-01-18 15:38:48.000000 AltTester-Driver-1.8.2/alttester/logging.py
--rw-r--r--   0 gitlabrunner   (501) staff       (20)      260 2023-01-18 15:38:48.000000 AltTester-Driver-1.8.2/alttester/playerpref.py
--rw-r--r--   0 gitlabrunner   (501) staff       (20)     1830 2023-01-31 05:41:51.000000 AltTester-Driver-1.8.2/alttester/portforwarding.py
--rw-r--r--   0 gitlabrunner   (501) staff       (20)      135 2023-01-31 05:41:51.000000 AltTester-Driver-1.8.2/requirements-dev.txt
--rw-r--r--   0 gitlabrunner   (501) staff       (20)       51 2023-01-31 05:41:51.000000 AltTester-Driver-1.8.2/requirements.txt
--rw-r--r--   0 gitlabrunner   (501) staff       (20)       38 2023-02-01 16:02:53.278562 AltTester-Driver-1.8.2/setup.cfg
--rw-r--r--   0 gitlabrunner   (501) staff       (20)     2569 2023-01-18 15:38:48.000000 AltTester-Driver-1.8.2/setup.py
-drwxr-xr-x   0 gitlabrunner   (501) staff       (20)        0 2023-02-01 16:02:53.194512 AltTester-Driver-1.8.2/tests/
-drwxr-xr-x   0 gitlabrunner   (501) staff       (20)        0 2023-02-01 16:02:53.273408 AltTester-Driver-1.8.2/tests/integration/
--rw-r--r--   0 gitlabrunner   (501) staff       (20)        0 2022-12-08 10:54:36.000000 AltTester-Driver-1.8.2/tests/integration/__init__.py
--rw-r--r--   0 gitlabrunner   (501) staff       (20)      572 2023-01-31 05:41:51.000000 AltTester-Driver-1.8.2/tests/integration/conftest.py
--rw-r--r--   0 gitlabrunner   (501) staff       (20)     4350 2023-01-31 05:41:51.000000 AltTester-Driver-1.8.2/tests/integration/test_driver.py
--rw-r--r--   0 gitlabrunner   (501) staff       (20)     3601 2023-01-31 05:41:51.000000 AltTester-Driver-1.8.2/tests/integration/test_notifications.py
--rw-r--r--   0 gitlabrunner   (501) staff       (20)    34670 2023-02-01 14:08:08.000000 AltTester-Driver-1.8.2/tests/integration/test_scene01.py
--rw-r--r--   0 gitlabrunner   (501) staff       (20)     4542 2023-01-18 15:38:48.000000 AltTester-Driver-1.8.2/tests/integration/test_scene02.py
--rw-r--r--   0 gitlabrunner   (501) staff       (20)     5694 2023-01-18 15:38:48.000000 AltTester-Driver-1.8.2/tests/integration/test_scene03.py
--rw-r--r--   0 gitlabrunner   (501) staff       (20)     4537 2023-01-18 15:38:48.000000 AltTester-Driver-1.8.2/tests/integration/test_scene05.py
--rw-r--r--   0 gitlabrunner   (501) staff       (20)     3824 2023-01-31 05:41:51.000000 AltTester-Driver-1.8.2/tests/integration/test_scene07.py
--rw-r--r--   0 gitlabrunner   (501) staff       (20)     1652 2023-01-18 15:38:48.000000 AltTester-Driver-1.8.2/tests/integration/test_scene09.py
--rw-r--r--   0 gitlabrunner   (501) staff       (20)     3605 2023-01-18 15:38:48.000000 AltTester-Driver-1.8.2/tests/integration/test_scene10.py
--rw-r--r--   0 gitlabrunner   (501) staff       (20)      414 2023-01-18 15:38:48.000000 AltTester-Driver-1.8.2/tests/integration/utils.py
-drwxr-xr-x   0 gitlabrunner   (501) staff       (20)        0 2023-02-01 16:02:53.276786 AltTester-Driver-1.8.2/tests/unit/
--rw-r--r--   0 gitlabrunner   (501) staff       (20)        0 2022-12-08 10:54:36.000000 AltTester-Driver-1.8.2/tests/unit/__init__.py
--rw-r--r--   0 gitlabrunner   (501) staff       (20)     1668 2023-01-18 15:38:48.000000 AltTester-Driver-1.8.2/tests/unit/test_altobject.py
--rw-r--r--   0 gitlabrunner   (501) staff       (20)     1529 2023-01-18 15:38:48.000000 AltTester-Driver-1.8.2/tests/unit/test_commands.py
--rw-r--r--   0 gitlabrunner   (501) staff       (20)      267 2023-01-31 05:41:51.000000 AltTester-Driver-1.8.2/tests/unit/test_portforwarding.py
--rw-r--r--   0 gitlabrunner   (501) staff       (20)     5264 2023-01-18 15:38:48.000000 AltTester-Driver-1.8.2/tests/unit/test_websocket.py
+drwxr-xr-x   0 gitlabrunner   (501) staff       (20)        0 2023-05-24 14:53:54.403305 AltTester-Driver-2.0.0/
+drwxr-xr-x   0 gitlabrunner   (501) staff       (20)        0 2023-05-24 14:53:54.328344 AltTester-Driver-2.0.0/AltTester_Driver.egg-info/
+-rw-r--r--   0 gitlabrunner   (501) staff       (20)     3406 2023-05-24 14:53:54.000000 AltTester-Driver-2.0.0/AltTester_Driver.egg-info/PKG-INFO
+-rw-r--r--   0 gitlabrunner   (501) staff       (20)     4513 2023-05-24 14:53:54.000000 AltTester-Driver-2.0.0/AltTester_Driver.egg-info/SOURCES.txt
+-rw-r--r--   0 gitlabrunner   (501) staff       (20)        1 2023-05-24 14:53:54.000000 AltTester-Driver-2.0.0/AltTester_Driver.egg-info/dependency_links.txt
+-rw-r--r--   0 gitlabrunner   (501) staff       (20)        1 2023-05-24 14:53:54.000000 AltTester-Driver-2.0.0/AltTester_Driver.egg-info/not-zip-safe
+-rw-r--r--   0 gitlabrunner   (501) staff       (20)       51 2023-05-24 14:53:54.000000 AltTester-Driver-2.0.0/AltTester_Driver.egg-info/requires.txt
+-rw-r--r--   0 gitlabrunner   (501) staff       (20)       16 2023-05-24 14:53:54.000000 AltTester-Driver-2.0.0/AltTester_Driver.egg-info/top_level.txt
+-rw-r--r--   0 gitlabrunner   (501) staff       (20)       56 2022-12-08 10:54:36.000000 AltTester-Driver-2.0.0/MANIFEST.in
+-rw-r--r--   0 gitlabrunner   (501) staff       (20)     3406 2023-05-24 14:53:54.402649 AltTester-Driver-2.0.0/PKG-INFO
+-rw-r--r--   0 gitlabrunner   (501) staff       (20)     1569 2023-05-24 13:53:56.000000 AltTester-Driver-2.0.0/README.md
+drwxr-xr-x   0 gitlabrunner   (501) staff       (20)        0 2023-05-24 14:53:54.337319 AltTester-Driver-2.0.0/alttester/
+-rw-r--r--   0 gitlabrunner   (501) staff       (20)      340 2023-05-09 08:10:34.000000 AltTester-Driver-2.0.0/alttester/__init__.py
+-rw-r--r--   0 gitlabrunner   (501) staff       (20)       18 2023-05-23 06:26:45.000000 AltTester-Driver-2.0.0/alttester/__version__.py
+-rw-r--r--   0 gitlabrunner   (501) staff       (20)    10367 2023-05-23 11:50:16.000000 AltTester-Driver-2.0.0/alttester/_websocket.py
+-rw-r--r--   0 gitlabrunner   (501) staff       (20)    36372 2023-05-05 10:42:15.000000 AltTester-Driver-2.0.0/alttester/altdriver.py
+-rw-r--r--   0 gitlabrunner   (501) staff       (20)    11419 2023-05-05 10:42:15.000000 AltTester-Driver-2.0.0/alttester/altobject.py
+-rw-r--r--   0 gitlabrunner   (501) staff       (20)      277 2023-02-01 12:34:37.000000 AltTester-Driver-2.0.0/alttester/by.py
+drwxr-xr-x   0 gitlabrunner   (501) staff       (20)        0 2023-05-24 14:53:54.341904 AltTester-Driver-2.0.0/alttester/commands/
+drwxr-xr-x   0 gitlabrunner   (501) staff       (20)        0 2023-05-24 14:53:54.345639 AltTester-Driver-2.0.0/alttester/commands/AltTesterCommands/
+-rw-r--r--   0 gitlabrunner   (501) staff       (20)      290 2023-03-08 09:20:39.000000 AltTester-Driver-2.0.0/alttester/commands/AltTesterCommands/__init__.py
+-rw-r--r--   0 gitlabrunner   (501) staff       (20)     1838 2023-05-05 10:42:15.000000 AltTester-Driver-2.0.0/alttester/commands/AltTesterCommands/add_notification_listener.py
+-rw-r--r--   0 gitlabrunner   (501) staff       (20)     1124 2023-05-05 10:42:15.000000 AltTester-Driver-2.0.0/alttester/commands/AltTesterCommands/remove_notification_listener.py
+-rw-r--r--   0 gitlabrunner   (501) staff       (20)      292 2023-05-05 10:42:15.000000 AltTester-Driver-2.0.0/alttester/commands/AltTesterCommands/reset_input.py
+-rw-r--r--   0 gitlabrunner   (501) staff       (20)     1208 2023-01-18 15:38:48.000000 AltTester-Driver-2.0.0/alttester/commands/AltTesterCommands/set_server_logging.py
+drwxr-xr-x   0 gitlabrunner   (501) staff       (20)        0 2023-05-24 14:53:54.354214 AltTester-Driver-2.0.0/alttester/commands/FindObjects/
+-rw-r--r--   0 gitlabrunner   (501) staff       (20)      621 2023-05-05 10:42:15.000000 AltTester-Driver-2.0.0/alttester/commands/FindObjects/__init__.py
+-rw-r--r--   0 gitlabrunner   (501) staff       (20)     1342 2023-01-18 15:38:48.000000 AltTester-Driver-2.0.0/alttester/commands/FindObjects/find_object.py
+-rw-r--r--   0 gitlabrunner   (501) staff       (20)      547 2023-01-18 15:38:48.000000 AltTester-Driver-2.0.0/alttester/commands/FindObjects/find_object_at_coordinates.py
+-rw-r--r--   0 gitlabrunner   (501) staff       (20)     1363 2023-01-18 15:38:48.000000 AltTester-Driver-2.0.0/alttester/commands/FindObjects/find_object_which_contains.py
+-rw-r--r--   0 gitlabrunner   (501) staff       (20)     1343 2023-01-18 15:38:48.000000 AltTester-Driver-2.0.0/alttester/commands/FindObjects/find_objects.py
+-rw-r--r--   0 gitlabrunner   (501) staff       (20)     1364 2023-01-18 15:38:48.000000 AltTester-Driver-2.0.0/alttester/commands/FindObjects/find_objects_which_contains.py
+-rw-r--r--   0 gitlabrunner   (501) staff       (20)     1392 2023-05-05 10:42:15.000000 AltTester-Driver-2.0.0/alttester/commands/FindObjects/wait_for_component_property.py
+-rw-r--r--   0 gitlabrunner   (501) staff       (20)     1796 2023-01-18 15:38:48.000000 AltTester-Driver-2.0.0/alttester/commands/FindObjects/wait_for_object.py
+-rw-r--r--   0 gitlabrunner   (501) staff       (20)     1898 2023-01-18 15:38:48.000000 AltTester-Driver-2.0.0/alttester/commands/FindObjects/wait_for_object_to_not_be_present.py
+-rw-r--r--   0 gitlabrunner   (501) staff       (20)     1954 2023-01-18 15:38:48.000000 AltTester-Driver-2.0.0/alttester/commands/FindObjects/wait_for_object_which_contains.py
+drwxr-xr-x   0 gitlabrunner   (501) staff       (20)        0 2023-05-24 14:53:54.365358 AltTester-Driver-2.0.0/alttester/commands/InputActions/
+-rw-r--r--   0 gitlabrunner   (501) staff       (20)      747 2023-01-18 15:38:48.000000 AltTester-Driver-2.0.0/alttester/commands/InputActions/__init__.py
+-rw-r--r--   0 gitlabrunner   (501) staff       (20)      525 2023-01-18 15:38:48.000000 AltTester-Driver-2.0.0/alttester/commands/InputActions/begin_touch.py
+-rw-r--r--   0 gitlabrunner   (501) staff       (20)      914 2023-01-18 15:38:48.000000 AltTester-Driver-2.0.0/alttester/commands/InputActions/click_coordinates.py
+-rw-r--r--   0 gitlabrunner   (501) staff       (20)      519 2023-01-18 15:38:48.000000 AltTester-Driver-2.0.0/alttester/commands/InputActions/end_touch.py
+-rw-r--r--   0 gitlabrunner   (501) staff       (20)     1251 2023-01-18 15:38:48.000000 AltTester-Driver-2.0.0/alttester/commands/InputActions/keys_down.py
+-rw-r--r--   0 gitlabrunner   (501) staff       (20)     1182 2023-01-18 15:38:48.000000 AltTester-Driver-2.0.0/alttester/commands/InputActions/keys_up.py
+-rw-r--r--   0 gitlabrunner   (501) staff       (20)      834 2023-01-18 15:38:48.000000 AltTester-Driver-2.0.0/alttester/commands/InputActions/move_mouse.py
+-rw-r--r--   0 gitlabrunner   (501) staff       (20)      647 2023-01-18 15:38:48.000000 AltTester-Driver-2.0.0/alttester/commands/InputActions/move_touch.py
+-rw-r--r--   0 gitlabrunner   (501) staff       (20)      815 2023-01-18 15:38:48.000000 AltTester-Driver-2.0.0/alttester/commands/InputActions/multi_point_swipe.py
+-rw-r--r--   0 gitlabrunner   (501) staff       (20)     1539 2023-01-18 15:38:48.000000 AltTester-Driver-2.0.0/alttester/commands/InputActions/press_keys.py
+-rw-r--r--   0 gitlabrunner   (501) staff       (20)      923 2023-01-18 15:38:48.000000 AltTester-Driver-2.0.0/alttester/commands/InputActions/scroll_mouse.py
+-rw-r--r--   0 gitlabrunner   (501) staff       (20)      874 2023-01-18 15:38:48.000000 AltTester-Driver-2.0.0/alttester/commands/InputActions/swipe.py
+-rw-r--r--   0 gitlabrunner   (501) staff       (20)      910 2023-01-18 15:38:48.000000 AltTester-Driver-2.0.0/alttester/commands/InputActions/tap_coordinates.py
+-rw-r--r--   0 gitlabrunner   (501) staff       (20)      832 2023-01-18 15:38:48.000000 AltTester-Driver-2.0.0/alttester/commands/InputActions/tilt.py
+drwxr-xr-x   0 gitlabrunner   (501) staff       (20)        0 2023-05-24 14:53:54.369977 AltTester-Driver-2.0.0/alttester/commands/Notifications/
+-rw-r--r--   0 gitlabrunner   (501) staff       (20)      449 2023-01-18 15:38:48.000000 AltTester-Driver-2.0.0/alttester/commands/Notifications/__init__.py
+-rw-r--r--   0 gitlabrunner   (501) staff       (20)      879 2023-01-18 15:38:48.000000 AltTester-Driver-2.0.0/alttester/commands/Notifications/base_notification_callbacks.py
+-rw-r--r--   0 gitlabrunner   (501) staff       (20)      194 2023-01-18 15:38:48.000000 AltTester-Driver-2.0.0/alttester/commands/Notifications/load_scene_mode.py
+-rw-r--r--   0 gitlabrunner   (501) staff       (20)      168 2023-01-18 15:38:48.000000 AltTester-Driver-2.0.0/alttester/commands/Notifications/load_scene_notification_result.py
+-rw-r--r--   0 gitlabrunner   (501) staff       (20)      178 2023-01-18 15:38:48.000000 AltTester-Driver-2.0.0/alttester/commands/Notifications/log_notification_result.py
+-rw-r--r--   0 gitlabrunner   (501) staff       (20)      138 2023-01-18 15:38:48.000000 AltTester-Driver-2.0.0/alttester/commands/Notifications/notification_type.py
+drwxr-xr-x   0 gitlabrunner   (501) staff       (20)        0 2023-05-24 14:53:54.379863 AltTester-Driver-2.0.0/alttester/commands/ObjectCommands/
+-rw-r--r--   0 gitlabrunner   (501) staff       (20)      748 2023-01-18 15:38:48.000000 AltTester-Driver-2.0.0/alttester/commands/ObjectCommands/__init__.py
+-rw-r--r--   0 gitlabrunner   (501) staff       (20)     1887 2023-01-18 15:38:48.000000 AltTester-Driver-2.0.0/alttester/commands/ObjectCommands/call_method.py
+-rw-r--r--   0 gitlabrunner   (501) staff       (20)      799 2023-01-18 15:38:48.000000 AltTester-Driver-2.0.0/alttester/commands/ObjectCommands/click_element.py
+-rw-r--r--   0 gitlabrunner   (501) staff       (20)      509 2023-01-18 15:38:48.000000 AltTester-Driver-2.0.0/alttester/commands/ObjectCommands/get_all_components.py
+-rw-r--r--   0 gitlabrunner   (501) staff       (20)      905 2023-01-18 15:38:48.000000 AltTester-Driver-2.0.0/alttester/commands/ObjectCommands/get_component_property.py
+-rw-r--r--   0 gitlabrunner   (501) staff       (20)      475 2023-01-18 15:38:48.000000 AltTester-Driver-2.0.0/alttester/commands/ObjectCommands/get_text.py
+-rw-r--r--   0 gitlabrunner   (501) staff       (20)      509 2023-05-04 14:17:26.000000 AltTester-Driver-2.0.0/alttester/commands/ObjectCommands/pointer_down.py
+-rw-r--r--   0 gitlabrunner   (501) staff       (20)      509 2023-05-04 14:17:26.000000 AltTester-Driver-2.0.0/alttester/commands/ObjectCommands/pointer_enter.py
+-rw-r--r--   0 gitlabrunner   (501) staff       (20)      489 2023-05-04 14:17:26.000000 AltTester-Driver-2.0.0/alttester/commands/ObjectCommands/pointer_exit.py
+-rw-r--r--   0 gitlabrunner   (501) staff       (20)      489 2023-05-04 14:17:26.000000 AltTester-Driver-2.0.0/alttester/commands/ObjectCommands/pointer_up.py
+-rw-r--r--   0 gitlabrunner   (501) staff       (20)      910 2023-01-18 15:38:48.000000 AltTester-Driver-2.0.0/alttester/commands/ObjectCommands/set_component_property.py
+-rw-r--r--   0 gitlabrunner   (501) staff       (20)      621 2023-01-18 15:38:48.000000 AltTester-Driver-2.0.0/alttester/commands/ObjectCommands/set_text.py
+-rw-r--r--   0 gitlabrunner   (501) staff       (20)      795 2023-01-18 15:38:48.000000 AltTester-Driver-2.0.0/alttester/commands/ObjectCommands/tap_element.py
+drwxr-xr-x   0 gitlabrunner   (501) staff       (20)        0 2023-05-24 14:53:54.389230 AltTester-Driver-2.0.0/alttester/commands/UnityCommands/
+-rw-r--r--   0 gitlabrunner   (501) staff       (20)      878 2023-01-18 15:38:48.000000 AltTester-Driver-2.0.0/alttester/commands/UnityCommands/__init__.py
+-rw-r--r--   0 gitlabrunner   (501) staff       (20)      240 2023-01-18 15:38:48.000000 AltTester-Driver-2.0.0/alttester/commands/UnityCommands/delete_player_pref.py
+-rw-r--r--   0 gitlabrunner   (501) staff       (20)      479 2023-01-18 15:38:48.000000 AltTester-Driver-2.0.0/alttester/commands/UnityCommands/delete_player_pref_key.py
+-rw-r--r--   0 gitlabrunner   (501) staff       (20)      244 2023-01-18 15:38:48.000000 AltTester-Driver-2.0.0/alttester/commands/UnityCommands/get_all_loaded_scenes.py
+-rw-r--r--   0 gitlabrunner   (501) staff       (20)      274 2023-01-18 15:38:48.000000 AltTester-Driver-2.0.0/alttester/commands/UnityCommands/get_current_scene.py
+-rw-r--r--   0 gitlabrunner   (501) staff       (20)      968 2023-01-18 15:38:48.000000 AltTester-Driver-2.0.0/alttester/commands/UnityCommands/get_player_pref_key.py
+-rw-r--r--   0 gitlabrunner   (501) staff       (20)      375 2023-01-18 15:38:48.000000 AltTester-Driver-2.0.0/alttester/commands/UnityCommands/get_time_scale.py
+-rw-r--r--   0 gitlabrunner   (501) staff       (20)      709 2023-01-18 15:38:48.000000 AltTester-Driver-2.0.0/alttester/commands/UnityCommands/load_scene.py
+-rw-r--r--   0 gitlabrunner   (501) staff       (20)     1337 2023-01-18 15:38:48.000000 AltTester-Driver-2.0.0/alttester/commands/UnityCommands/set_player_pref_key.py
+-rw-r--r--   0 gitlabrunner   (501) staff       (20)      710 2023-01-18 15:38:48.000000 AltTester-Driver-2.0.0/alttester/commands/UnityCommands/set_time_scale.py
+-rw-r--r--   0 gitlabrunner   (501) staff       (20)      637 2023-01-18 15:38:48.000000 AltTester-Driver-2.0.0/alttester/commands/UnityCommands/unload_scene.py
+-rw-r--r--   0 gitlabrunner   (501) staff       (20)     1010 2023-01-18 15:38:48.000000 AltTester-Driver-2.0.0/alttester/commands/UnityCommands/wait_for_current_scene_to_be.py
+-rw-r--r--   0 gitlabrunner   (501) staff       (20)      556 2023-03-08 09:20:39.000000 AltTester-Driver-2.0.0/alttester/commands/__init__.py
+-rw-r--r--   0 gitlabrunner   (501) staff       (20)     7280 2023-05-05 10:42:15.000000 AltTester-Driver-2.0.0/alttester/commands/base_command.py
+-rw-r--r--   0 gitlabrunner   (501) staff       (20)      487 2023-01-18 15:38:48.000000 AltTester-Driver-2.0.0/alttester/commands/get_png_screenshot.py
+-rw-r--r--   0 gitlabrunner   (501) staff       (20)      240 2023-01-18 15:38:48.000000 AltTester-Driver-2.0.0/alttester/commands/get_server_version.py
+-rw-r--r--   0 gitlabrunner   (501) staff       (20)      874 2023-01-18 15:38:48.000000 AltTester-Driver-2.0.0/alttester/commands/get_static_property.py
+-rw-r--r--   0 gitlabrunner   (501) staff       (20)      854 2023-03-08 09:20:39.000000 AltTester-Driver-2.0.0/alttester/commands/set_static_property.py
+-rw-r--r--   0 gitlabrunner   (501) staff       (20)     3741 2023-05-05 10:42:15.000000 AltTester-Driver-2.0.0/alttester/exceptions.py
+-rw-r--r--   0 gitlabrunner   (501) staff       (20)     7502 2023-01-18 15:38:48.000000 AltTester-Driver-2.0.0/alttester/keycode.py
+-rw-r--r--   0 gitlabrunner   (501) staff       (20)      333 2023-01-18 15:38:48.000000 AltTester-Driver-2.0.0/alttester/logging.py
+-rw-r--r--   0 gitlabrunner   (501) staff       (20)      260 2023-01-18 15:38:48.000000 AltTester-Driver-2.0.0/alttester/playerpref.py
+-rw-r--r--   0 gitlabrunner   (501) staff       (20)      980 2023-05-09 08:10:34.000000 AltTester-Driver-2.0.0/alttester/reverse_port_forwarding.py
+-rw-r--r--   0 gitlabrunner   (501) staff       (20)      112 2023-05-05 10:42:15.000000 AltTester-Driver-2.0.0/requirements-dev.txt
+-rw-r--r--   0 gitlabrunner   (501) staff       (20)       50 2023-05-09 08:10:34.000000 AltTester-Driver-2.0.0/requirements.txt
+-rw-r--r--   0 gitlabrunner   (501) staff       (20)       38 2023-05-24 14:53:54.403512 AltTester-Driver-2.0.0/setup.cfg
+-rw-r--r--   0 gitlabrunner   (501) staff       (20)     2560 2023-05-12 12:36:10.000000 AltTester-Driver-2.0.0/setup.py
+drwxr-xr-x   0 gitlabrunner   (501) staff       (20)        0 2023-05-24 14:53:54.321061 AltTester-Driver-2.0.0/tests/
+drwxr-xr-x   0 gitlabrunner   (501) staff       (20)        0 2023-05-24 14:53:54.399345 AltTester-Driver-2.0.0/tests/integration/
+-rw-r--r--   0 gitlabrunner   (501) staff       (20)        0 2022-12-08 10:54:36.000000 AltTester-Driver-2.0.0/tests/integration/__init__.py
+-rw-r--r--   0 gitlabrunner   (501) staff       (20)      622 2023-05-12 12:36:10.000000 AltTester-Driver-2.0.0/tests/integration/conftest.py
+-rw-r--r--   0 gitlabrunner   (501) staff       (20)     4408 2023-05-05 10:42:15.000000 AltTester-Driver-2.0.0/tests/integration/test_driver.py
+-rw-r--r--   0 gitlabrunner   (501) staff       (20)     3625 2023-05-05 10:42:15.000000 AltTester-Driver-2.0.0/tests/integration/test_notifications.py
+-rw-r--r--   0 gitlabrunner   (501) staff       (20)      812 2023-05-09 08:10:34.000000 AltTester-Driver-2.0.0/tests/integration/test_reverse_port_forwarding.py
+-rw-r--r--   0 gitlabrunner   (501) staff       (20)    34917 2023-05-05 10:42:15.000000 AltTester-Driver-2.0.0/tests/integration/test_scene01.py
+-rw-r--r--   0 gitlabrunner   (501) staff       (20)     4542 2023-03-08 09:20:39.000000 AltTester-Driver-2.0.0/tests/integration/test_scene02.py
+-rw-r--r--   0 gitlabrunner   (501) staff       (20)     5694 2023-03-08 09:20:39.000000 AltTester-Driver-2.0.0/tests/integration/test_scene03.py
+-rw-r--r--   0 gitlabrunner   (501) staff       (20)     4537 2023-03-08 09:20:39.000000 AltTester-Driver-2.0.0/tests/integration/test_scene05.py
+-rw-r--r--   0 gitlabrunner   (501) staff       (20)     3824 2023-05-05 10:42:15.000000 AltTester-Driver-2.0.0/tests/integration/test_scene07.py
+-rw-r--r--   0 gitlabrunner   (501) staff       (20)     1652 2023-03-08 09:20:39.000000 AltTester-Driver-2.0.0/tests/integration/test_scene09.py
+-rw-r--r--   0 gitlabrunner   (501) staff       (20)     3605 2023-03-08 09:20:39.000000 AltTester-Driver-2.0.0/tests/integration/test_scene10.py
+-rw-r--r--   0 gitlabrunner   (501) staff       (20)      414 2023-01-18 15:38:48.000000 AltTester-Driver-2.0.0/tests/integration/utils.py
+drwxr-xr-x   0 gitlabrunner   (501) staff       (20)        0 2023-05-24 14:53:54.401815 AltTester-Driver-2.0.0/tests/unit/
+-rw-r--r--   0 gitlabrunner   (501) staff       (20)        0 2022-12-08 10:54:36.000000 AltTester-Driver-2.0.0/tests/unit/__init__.py
+-rw-r--r--   0 gitlabrunner   (501) staff       (20)     1668 2023-01-18 15:38:48.000000 AltTester-Driver-2.0.0/tests/unit/test_altobject.py
+-rw-r--r--   0 gitlabrunner   (501) staff       (20)     1529 2023-01-18 15:38:48.000000 AltTester-Driver-2.0.0/tests/unit/test_commands.py
+-rw-r--r--   0 gitlabrunner   (501) staff       (20)     5403 2023-05-05 10:42:15.000000 AltTester-Driver-2.0.0/tests/unit/test_websocket.py
```

### Comparing `AltTester-Driver-1.8.2/AltTester_Driver.egg-info/PKG-INFO` & `AltTester-Driver-2.0.0/AltTester_Driver.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 Metadata-Version: 2.1
 Name: AltTester-Driver
-Version: 1.8.2
+Version: 2.0.0
 Summary: Python bindings for the AltTester framework. AltTester is an open-source UI driven test automation tool that helps you find objects in your game and interacts with them.
-Home-page: https://altom.com/alttester/docs/sdk
+Home-page: https://alttester.com/docs/pro/sdk
 Author: Altom Consulting
-Author-email: suport.alttester@altom.com
+Author-email: contact@alttester.com
 License: GNU GPLv3
 Project-URL: Bug Tracker, https://github.com/alttester/AltTester-Unity-SDK/issues
-Project-URL: Documentation, https://altom.com/alttester/docs/sdk
+Project-URL: Documentation, https://alttester.com/docs/pro/sdk
 Project-URL: Source, https://github.com/alttester/AltTester-Unity-SDK
 Keywords: unity testing tests
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Other Audience
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Programming Language :: C#
@@ -35,28 +35,28 @@
 Requires-Python: >=3.4.0
 Description-Content-Type: text/markdown
 
 # AltTester Python Bindings
 
 This package contains an library for adding Python language binding to the AltTester framework.
 
-AltTester Unity SDK is an open-source UI driven test automation tool that helps you find objects in your game and interacts with them using tests written in C#, Python or Java.
+AltTester Unity SDK is an open-source UI driven test automation tool that helps you find objects in your application and interacts with them using tests written in C#, Python or Java.
 
 You can run your tests on real devices (mobile, PCs, etc.) or inside the Unity Editor.
 
-Read the documentation on https://altom.com/alttester/docs/sdk/
+Read the documentation on https://alttester.com/docs/pro/sdk/
 
 ## Get Started
 
-Check out the [Get Started](https://altom.com/alttester/docs/sdk/pages/get-started.html) guide from the documentation.
+Check out the [Get Started](https://alttester.com/docs/pro/sdk/pages/get-started.html) guide from the documentation.
 
 ## Development
 
-* Code Style: [PEP-0008](https://www.python.org/dev/peps/pep-0008/)
-* Docstring style: [Google Style Docstrings](https://sphinxcontrib-napoleon.readthedocs.io/en/latest/example_google.html).
+-   Code Style: [PEP-0008](https://www.python.org/dev/peps/pep-0008/)
+-   Docstring style: [Google Style Docstrings](https://sphinxcontrib-napoleon.readthedocs.io/en/latest/example_google.html).
 
 ### Running Tests
 
 Run the following command to install the dev dependencies:
 
 ```
 $ pip install -r requirements-dev.txt
@@ -72,15 +72,15 @@
 
 ```
 $ pytest tests/integration/
 ```
 
 ## Contributing
 
-Check out the full contributing guide [contributing](https://altom.com/alttester/docs/sdk/pages/contributing.html).
+Check out the full contributing guide [contributing](https://alttester.com/docs/pro/sdk/pages/contributing.html).
 
 ## Support
 
 Join our Google Group for questions and discussions: https://groups.google.com/a/altom.com/g/alttesterforum
 
 Join our Discord Server to chat with other members of the community: https://discord.gg/Ag9RSuS
```

### Comparing `AltTester-Driver-1.8.2/AltTester_Driver.egg-info/SOURCES.txt` & `AltTester-Driver-2.0.0/AltTester_Driver.egg-info/SOURCES.txt`

 * *Files 3% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 alttester/altdriver.py
 alttester/altobject.py
 alttester/by.py
 alttester/exceptions.py
 alttester/keycode.py
 alttester/logging.py
 alttester/playerpref.py
-alttester/portforwarding.py
+alttester/reverse_port_forwarding.py
 alttester/commands/__init__.py
 alttester/commands/base_command.py
 alttester/commands/get_png_screenshot.py
 alttester/commands/get_server_version.py
 alttester/commands/get_static_property.py
 alttester/commands/set_static_property.py
 alttester/commands/AltTesterCommands/__init__.py
@@ -33,14 +33,15 @@
 alttester/commands/AltTesterCommands/set_server_logging.py
 alttester/commands/FindObjects/__init__.py
 alttester/commands/FindObjects/find_object.py
 alttester/commands/FindObjects/find_object_at_coordinates.py
 alttester/commands/FindObjects/find_object_which_contains.py
 alttester/commands/FindObjects/find_objects.py
 alttester/commands/FindObjects/find_objects_which_contains.py
+alttester/commands/FindObjects/wait_for_component_property.py
 alttester/commands/FindObjects/wait_for_object.py
 alttester/commands/FindObjects/wait_for_object_to_not_be_present.py
 alttester/commands/FindObjects/wait_for_object_which_contains.py
 alttester/commands/InputActions/__init__.py
 alttester/commands/InputActions/begin_touch.py
 alttester/commands/InputActions/click_coordinates.py
 alttester/commands/InputActions/end_touch.py
@@ -85,20 +86,20 @@
 alttester/commands/UnityCommands/set_time_scale.py
 alttester/commands/UnityCommands/unload_scene.py
 alttester/commands/UnityCommands/wait_for_current_scene_to_be.py
 tests/integration/__init__.py
 tests/integration/conftest.py
 tests/integration/test_driver.py
 tests/integration/test_notifications.py
+tests/integration/test_reverse_port_forwarding.py
 tests/integration/test_scene01.py
 tests/integration/test_scene02.py
 tests/integration/test_scene03.py
 tests/integration/test_scene05.py
 tests/integration/test_scene07.py
 tests/integration/test_scene09.py
 tests/integration/test_scene10.py
 tests/integration/utils.py
 tests/unit/__init__.py
 tests/unit/test_altobject.py
 tests/unit/test_commands.py
-tests/unit/test_portforwarding.py
 tests/unit/test_websocket.py
```

### Comparing `AltTester-Driver-1.8.2/PKG-INFO` & `AltTester-Driver-2.0.0/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 Metadata-Version: 2.1
 Name: AltTester-Driver
-Version: 1.8.2
+Version: 2.0.0
 Summary: Python bindings for the AltTester framework. AltTester is an open-source UI driven test automation tool that helps you find objects in your game and interacts with them.
-Home-page: https://altom.com/alttester/docs/sdk
+Home-page: https://alttester.com/docs/pro/sdk
 Author: Altom Consulting
-Author-email: suport.alttester@altom.com
+Author-email: contact@alttester.com
 License: GNU GPLv3
 Project-URL: Bug Tracker, https://github.com/alttester/AltTester-Unity-SDK/issues
-Project-URL: Documentation, https://altom.com/alttester/docs/sdk
+Project-URL: Documentation, https://alttester.com/docs/pro/sdk
 Project-URL: Source, https://github.com/alttester/AltTester-Unity-SDK
 Keywords: unity testing tests
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Other Audience
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Programming Language :: C#
@@ -35,28 +35,28 @@
 Requires-Python: >=3.4.0
 Description-Content-Type: text/markdown
 
 # AltTester Python Bindings
 
 This package contains an library for adding Python language binding to the AltTester framework.
 
-AltTester Unity SDK is an open-source UI driven test automation tool that helps you find objects in your game and interacts with them using tests written in C#, Python or Java.
+AltTester Unity SDK is an open-source UI driven test automation tool that helps you find objects in your application and interacts with them using tests written in C#, Python or Java.
 
 You can run your tests on real devices (mobile, PCs, etc.) or inside the Unity Editor.
 
-Read the documentation on https://altom.com/alttester/docs/sdk/
+Read the documentation on https://alttester.com/docs/pro/sdk/
 
 ## Get Started
 
-Check out the [Get Started](https://altom.com/alttester/docs/sdk/pages/get-started.html) guide from the documentation.
+Check out the [Get Started](https://alttester.com/docs/pro/sdk/pages/get-started.html) guide from the documentation.
 
 ## Development
 
-* Code Style: [PEP-0008](https://www.python.org/dev/peps/pep-0008/)
-* Docstring style: [Google Style Docstrings](https://sphinxcontrib-napoleon.readthedocs.io/en/latest/example_google.html).
+-   Code Style: [PEP-0008](https://www.python.org/dev/peps/pep-0008/)
+-   Docstring style: [Google Style Docstrings](https://sphinxcontrib-napoleon.readthedocs.io/en/latest/example_google.html).
 
 ### Running Tests
 
 Run the following command to install the dev dependencies:
 
 ```
 $ pip install -r requirements-dev.txt
@@ -72,15 +72,15 @@
 
 ```
 $ pytest tests/integration/
 ```
 
 ## Contributing
 
-Check out the full contributing guide [contributing](https://altom.com/alttester/docs/sdk/pages/contributing.html).
+Check out the full contributing guide [contributing](https://alttester.com/docs/pro/sdk/pages/contributing.html).
 
 ## Support
 
 Join our Google Group for questions and discussions: https://groups.google.com/a/altom.com/g/alttesterforum
 
 Join our Discord Server to chat with other members of the community: https://discord.gg/Ag9RSuS
```

### Comparing `AltTester-Driver-1.8.2/README.md` & `AltTester-Driver-2.0.0/README.md`

 * *Files 18% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 # AltTester Python Bindings
 
 This package contains an library for adding Python language binding to the AltTester framework.
 
-AltTester Unity SDK is an open-source UI driven test automation tool that helps you find objects in your game and interacts with them using tests written in C#, Python or Java.
+AltTester Unity SDK is an open-source UI driven test automation tool that helps you find objects in your application and interacts with them using tests written in C#, Python or Java.
 
 You can run your tests on real devices (mobile, PCs, etc.) or inside the Unity Editor.
 
-Read the documentation on https://altom.com/alttester/docs/sdk/
+Read the documentation on https://alttester.com/docs/pro/sdk/
 
 ## Get Started
 
-Check out the [Get Started](https://altom.com/alttester/docs/sdk/pages/get-started.html) guide from the documentation.
+Check out the [Get Started](https://alttester.com/docs/pro/sdk/pages/get-started.html) guide from the documentation.
 
 ## Development
 
-* Code Style: [PEP-0008](https://www.python.org/dev/peps/pep-0008/)
-* Docstring style: [Google Style Docstrings](https://sphinxcontrib-napoleon.readthedocs.io/en/latest/example_google.html).
+-   Code Style: [PEP-0008](https://www.python.org/dev/peps/pep-0008/)
+-   Docstring style: [Google Style Docstrings](https://sphinxcontrib-napoleon.readthedocs.io/en/latest/example_google.html).
 
 ### Running Tests
 
 Run the following command to install the dev dependencies:
 
 ```
 $ pip install -r requirements-dev.txt
@@ -35,15 +35,15 @@
 
 ```
 $ pytest tests/integration/
 ```
 
 ## Contributing
 
-Check out the full contributing guide [contributing](https://altom.com/alttester/docs/sdk/pages/contributing.html).
+Check out the full contributing guide [contributing](https://alttester.com/docs/pro/sdk/pages/contributing.html).
 
 ## Support
 
 Join our Google Group for questions and discussions: https://groups.google.com/a/altom.com/g/alttesterforum
 
 Join our Discord Server to chat with other members of the community: https://discord.gg/Ag9RSuS
```

### Comparing `AltTester-Driver-1.8.2/alttester/_websocket.py` & `AltTester-Driver-2.0.0/alttester/_websocket.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,24 +1,25 @@
 import time
 import json
 from collections import defaultdict, deque
+from urllib.parse import urlencode, urlunparse
 from threading import Thread
 
 from loguru import logger
 import websocket
 
+from . import exceptions
 from .commands.Notifications.notification_type import NotificationType
 from .commands.Notifications.load_scene_notification_result import LoadSceneNotificationResult
 from .commands.Notifications.log_notification_result import LogNotificationResult
 from .commands.Notifications.load_scene_mode import LoadSceneMode
-from .exceptions import ConnectionError, ConnectionTimeoutError, CommandResponseTimeoutException
 
 
 class Store:
-    """Stores the responses from AltTester."""
+    """Stores the responses from AltServer."""
 
     def __init__(self, dict=None):
         self._store = dict or defaultdict(deque)
 
     def __repr__(self):
         return "{}({!r})".format(self.__class__.__name__, self._store)
 
@@ -35,15 +36,15 @@
         try:
             return self._store[key].popleft()
         except IndexError:
             return None
 
 
 class NotificationHandler:
-    """Handles the parsing of the notification messages from AltTester."""
+    """Handles the parsing of the notification messages from AltServer."""
 
     def __init__(self):
         self._notification_callbacks = defaultdict(list)
 
     def __repr__(self):
         return "{}()".format(self.__class__.__name__)
 
@@ -82,15 +83,15 @@
         self._notification_callbacks[notification_type].append(callback)
 
     def remove_notification_listener(self, notification_type):
         self._notification_callbacks[notification_type].clear()
 
 
 class CommandHandler:
-    """Handles the parsing of command messages from AltTester."""
+    """Handles the parsing of command messages from AltServer."""
 
     def __init__(self):
         self._store = Store()
 
         self._current_command = None
         self._timeout_commands = []
 
@@ -100,67 +101,76 @@
     def set_current_command(self, message):
         self._current_command = (message.get("messageId"), message.get("commandName"))
 
     def get_current_command(self):
         return self._current_command
 
     def timeout(self):
-        """Mark the current command as timedout."""
+        """Mark the current command as timeout."""
 
         self._timeout_commands.append(self._current_command)
 
     def handle_command(self, message):
         command = (message.get("messageId"), message.get("commandName"))
 
-        # Skip messages for commands that timedout
+        # Skip messages for commands that timeout
         if command in self._timeout_commands:
             return
 
         self._store.push(command, message)
 
     def has_response(self):
         return self._store.has(self._current_command)
 
     def get_response(self):
         return self._store.pop(self._current_command)
 
 
 class WebsocketConnection:
-    """Handles the websocket connection with AltTester.
+    """Handles the websocket connection with AltServer.
 
     Args:
-        host (:obj:`str`): The host to connect to.
-        port (:obj:`int`): The port to connect to.
-        timeout (:obj:`int` or :obj:`float`): The connection timeout time.
+        host (:obj:`str`, optional): The host to connect to. Defaults to ``127.0.0.1``.
+        port (:obj:`int`, optional): The port to connect to. Defaults to ``13000``.
+        path (:obj:`int`, optional): The path section of the url. Defaults to ``/``.
+        params (:obj:`dict`, optional): The params/query component of the url. Default to ``None``.
+        timeout (:obj:`int` or :obj:`float`, optional): The connection timeout time.
 
     """
 
-    def __init__(self, host="127.0.0.1", port=13000, timeout=None):
+    def __init__(self, host="127.0.0.1", port=13000, path="/", params=None, timeout=None, command_handler=None,
+                 notification_handler=None):
         self.host = host
         self.port = port
-        self.url = "ws://{}:{}/altws/".format(host, port)
+        self.path = path
+        self.params = params or {}
+
+        self.url = urlunparse(["ws", "{}:{}".format(self.host, self.port), self.path, "", urlencode(self.params), ""])
 
         self.timeout = timeout
         self.command_timeout = 60
         self.delay = 0.1
 
         self._errors = deque()
+        self._close_message = None
 
         self._thread = None
         self._websocket = None
         self._is_open = False
 
-        self._command_handler = CommandHandler()
-        self._notification_handler = NotificationHandler()
+        self._command_handler = command_handler
+        self._notification_handler = notification_handler
 
     def __repr__(self):
-        return "{}({!r}, {!r}, {!r})".format(
+        return "{}({!r}, {!r}, {!r}, {!r}, {!r})".format(
             self.__class__.__name__,
             self.host,
             self.port,
+            self.path,
+            self.params,
             self.timeout,
         )
 
     def _create_connection(self):
         # TODO: Enable and disable the trace based on an environment variable or config option
         # Uncomment the following line if you are debugging the websocket connection
         # websocket.enableTrace(True)
@@ -169,90 +179,109 @@
             on_open=self._on_open,
             on_message=self._on_message,
             on_error=self._on_error,
             on_close=self._on_close
         )
         self._thread = Thread(target=self._websocket.run_forever, daemon=True).start()
 
-    def _ensure_connection_is_open(self):
+    def _check_close_message(self):
+        if self._close_message:
+            reason = self._close_message[1]
+
+            if self._close_message[0] == 4001:
+                raise exceptions.NoAppConnected(reason)
+            if self._close_message[0] == 4002:
+                raise exceptions.AppDisconnectedError(reason)
+            if self._close_message[0] == 4005:
+                raise exceptions.AppDisconnectedError(reason)
+
+            raise exceptions.ConnectionError("Connection closed by AltServer with reason: {}.".format(reason))
+
+    def _check_errors(self):
         if self._errors:
             error = self._errors.pop()
             self.close()
-            raise ConnectionError(error)
+            raise exceptions.ConnectionError(error)
+
+    def _ensure_connection_is_open(self):
+        self._check_close_message()
+        self._check_errors()
 
         if self._websocket is None or not self._is_open:
             self.close()
-            raise ConnectionError("Connection already closed.")
+            raise exceptions.ConnectionError("Connection closed. An unexpected error ocurred.")
 
     def _on_message(self, ws, message):
-        """A callback which is called when the connection is opened."""
+        """A callback which is called when the connection receives data."""
 
         logger.debug("Received: {}", message)
         response = json.loads(message)
 
         if response.get("isNotification"):
             self._notification_handler.handle_notification(response)
         else:
             self._command_handler.handle_command(response)
 
     def _on_error(self, ws, error):
         """A callback which is called when the connection gets an error."""
 
-        logger.debug("Error: {}", error)
+        logger.error("Error: {}", error)
         self._errors.append(error)
 
     def _on_close(self, ws, close_status_code, close_msg):
         """A callback which is called when the connection is closed."""
 
         logger.debug(
-            "Connection to AltTester closed with status code: {} and message: {}.",
+            "Connection to AltServer closed with status code: {} and message: '{}'.",
             close_status_code,
             close_msg
         )
 
+        self._close_message = (close_status_code, close_msg)
+
         self._is_open = False
         self._websocket = None
 
     def _on_open(self, ws):
-        """A callback which is called when the connection recives data."""
+        """A callback which is called when the connection is opened."""
 
-        logger.debug("Connection oppend successfully.")
+        logger.debug("Connection opened successfully.")
         self._is_open = True
 
     def set_command_timeout(self, timeout):
         self.command_timeout = timeout
 
     def get_command_timeout(self):
         return self.command_timeout
 
     def connect(self):
-        logger.info("Connecting to host: {} port: {}.", self.host, self.port)
+        logger.info("Connecting to URL: '{}'.", self.url)
 
         elapsed_time = 0
         self._create_connection()
 
         while not self._is_open and (self.timeout is None or elapsed_time < self.timeout):
-            time.sleep(self.delay)
-            elapsed_time += self.delay
+            self._close_message = None
+            self._errors = []
 
-            if self._errors:
+            if self._errors or self._close_message:
                 self.close()
                 self._create_connection()
 
-        if self._errors and not self._is_open:
-            error = self._errors.pop()
-            self.close()
+            time.sleep(self.delay)
+            elapsed_time += self.delay
 
-            raise ConnectionError(error)
+        self._check_close_message()
+        self._check_errors()
 
         if not self._is_open:
             self.close()
 
-            raise ConnectionTimeoutError(
-                "Failed to connect to AltTester host: {} port: {}.".format(self.host, self.port)
+            raise exceptions.ConnectionTimeoutError(
+                "Failed to connect to AltServer host: {} port: {}.".format(self.host, self.port)
             )
 
     def send(self, data):
         self._ensure_connection_is_open()
 
         message = json.dumps(data)
         logger.debug("Sent: {}", message)
@@ -270,28 +299,23 @@
                 return self._command_handler.get_response()
 
             elapsed_time += delay
             time.sleep(delay)
 
         if elapsed_time > self.command_timeout:
             self._command_handler.timeout()
-            raise CommandResponseTimeoutException()
+            raise exceptions.CommandResponseTimeoutException()
 
     def close(self):
-        logger.info("Closing connection to AltTester on host: {} port: {}", self.host, self.port)
+        logger.info("Closing connection to AltServer on host: {} port: {}", self.host, self.port)
 
         if self._websocket:
             self._websocket.close()
             self._websocket = None
 
         if self._thread:
             self._thread.join(0)
             self._thread = None
 
         self._errors = []
+        self._close_message = None
         self._is_open = False
-
-    def add_notification_listener(self, notification_type, callback, overwrite=False):
-        self._notification_handler.add_notification_listener(notification_type, callback, overwrite=overwrite)
-
-    def remove_notification_listener(self, notification_type):
-        self._notification_handler.remove_notification_listener(notification_type)
```

### Comparing `AltTester-Driver-1.8.2/alttester/altdriver.py` & `AltTester-Driver-2.0.0/alttester/altdriver.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,46 +2,78 @@
 import sys
 
 from loguru import logger
 
 import alttester.commands as commands
 from alttester.commands.base_command import Command
 from alttester.__version__ import VERSION
-from alttester._websocket import WebsocketConnection
+from alttester._websocket import WebsocketConnection, CommandHandler, NotificationHandler
 from alttester.altobject import AltObject
 from alttester.by import By
 
 
 warnings.filterwarnings("default", category=DeprecationWarning, module=__name__)
 
 
 class AltDriver:
-    """The driver object will help interacting with all the game objects, their properties and methods.
+    """The driver object will help interacting with all the application objects, their properties and methods.
 
-    When you instantiate an ``AltDriver`` object in your tests, you can use it to “drive” your game like one of
-    your users would, by interacting with all the game objects, their properties and methods.  An ``AltDriver``
-    instance will connect to the AltProxy.
+    When you instantiate an ``AltDriver`` object in your tests, you can use it to “drive” your application like one of
+    your users would, by interacting with all the application objects, their properties and methods.  An ``AltDriver``
+    instance will connect to the AltServer.
 
     Args:
-        host (:obj:`str`): The proxy host to connect to.
-        port (:obj:`int`): The proxy port to connect to.
+        host (:obj:`str`, optional): The host to connect to.
+        port (:obj:`int`, optional): The port to connect to.
+        app_name (:obj:`str`, optional): The application name. Defaults to ``__default__``.
         enable_logging (:obj:`bool`, optional): If set to ``True`` will turn on logging, by default logging is disabled.
-        timeout (:obj:`int`, :obj:`float`, optional): The connect timeout time in seconds.
+        timeout (:obj:`int`, :obj:`float`, optional): The timeout duration for establishing a connection, in seconds.
+            If set to ``None``, the connection attempt will wait indefinitely. The default value is ``60`` seconds.
 
     """
 
-    def __init__(self, host="127.0.0.1", port=13000, enable_logging=False, timeout=None):
+    def __init__(self, host="127.0.0.1", port=13000, app_name="__default__", enable_logging=False, timeout=60):
         self.host = host
         self.port = port
+        self.app_name = app_name
         self.enable_logging = enable_logging
+        self.timeout = timeout
 
         self._config_logging(self.enable_logging)
 
-        self._connection = WebsocketConnection(host=host, port=port, timeout=timeout)
+        logger.debug(
+            "Connecting to AltTester on host: '{}', port: '{}' and app name: '{}'.",
+            self.host,
+            self.port,
+            self.app_name
+        )
+
+        self._command_handler = CommandHandler()
+        self._notification_handler = NotificationHandler()
+        self._connection = WebsocketConnection(
+            host=self.host,
+            port=self.port,
+            timeout=self.timeout,
+            path="altws",
+            params={"appName": self.app_name},
+            command_handler=self._command_handler,
+            notification_handler=self._notification_handler
+        )
         self._connection.connect()
+        self._check_server_version()
+
+    def __repr__(self):
+        return "{}({!r}, {!r}, {!r}, {!r}, {!r})".format(
+            self.__class__.__name__,
+            self.host,
+            self.port,
+            self.app_name,
+            self.enable_logging,
+            self.timeout
+        )
 
     @staticmethod
     def _config_logging(enable_logging):
         if enable_logging:
             logger.configure(
                 handlers=[
                     dict(sink=sys.stdout, diagnose=False),
@@ -156,15 +188,15 @@
             log_lever (:obj:`AltLogLevel`): The logging level.
 
         """
 
         commands.SetServerLogging.run(self._connection, logger, log_level)
 
     def call_static_method(self, type_name, method_name, assembly, parameters=None, type_of_parameters=None):
-        """Invoke a static method from your game.
+        """Invoke a static method from your application.
 
         Args:
             type_name (:obj:`str`): The name of the script. If the script has a namespace the format should look like
                 this: ``"namespace.typeName"``.
             method_name (:obj:`str`): The name of the public method that we want to call. If the method is inside a
                 static property/field to be able to call that method, methodName need to be the following format
                 ``"propertyName.MethodName"``.
@@ -524,28 +556,28 @@
             list of AltObjects: The list of objects.
 
         """
 
         return self.find_objects(By.PATH, "//*", camera_by=camera_by, camera_value=camera_value, enabled=enabled)
 
     def move_mouse(self, coordinates, duration=0.1, wait=True):
-        """Simulates mouse movement in your game.
+        """Simulates mouse movement in your application.
 
         Args:
             coordinates (:obj:`dict`): The screen coordinates
             duration (:obj:`int`, optional): The time measured in seconds to move the mouse from current position to
                 the set location. Defaults to ``0.1``
             wait (:obj:`bool`, optional): If set wait for command to finish. Defaults to ``True``.
 
         """
 
         commands.MoveMouse.run(self._connection, coordinates, duration, wait)
 
     def scroll(self, speed_vertical=1, duration=0.1, wait=True, speed_horizontal=1):
-        """Simulate scroll mouse action in your game.
+        """Simulate scroll mouse action in your application.
 
         Args:
             speed_vertical (:obj:`int`, :obj:`float`): Set how fast to scroll. Positive values will scroll up and
                 negative values will scroll down. Defaults to ``1``
             duration (:obj:`int`, :obj:`float`, optional): The duration of the scroll in seconds. Defaults to ``0.1``.
             wait (:obj:`bool`, optional): If set wait for command to finish. Defaults to ``True``.
             speed_horizontal (:obj:`int`, :obj:`float`): Set how fast to scroll right or left. Defaults to ``1``
@@ -612,29 +644,29 @@
             key_codes (:obj:`list` of :obj:`AltKeyCode`): The key codes of the keys simulated to be released.
 
         """
 
         commands.KeysUp.run(self._connection, key_codes)
 
     def press_key(self, key_code, power=1, duration=0.1, wait=True):
-        """Simulates key press action in your game.
+        """Simulates key press action in your application.
 
         Args:
             key_code (:obj:`AltKeyCode`): The key code of the key simulated to be pressed.
             power (:obj:`int`, :obj:`float`, optional): A value between [-1,1] used for joysticks to indicate how hard
                 the button was pressed. Defaults to ``1``.
             duration (:obj:`float`, optional): The time measured in seconds from the key press to the key release.
             wait (:obj:`bool`, optional): If set wait for command to finish. Defaults to ``True``.
 
         """
 
         self.press_keys([key_code], power=power, duration=duration, wait=wait)
 
     def press_keys(self, key_codes, power=1, duration=0.1, wait=True):
-        """Simulates multiple keypress action in your game.
+        """Simulates multiple keypress action in your application.
 
         Args:
             key_codes (:obj:`list` of :obj:`AltKeyCode`): The key codes of the keys simulated to be pressed.
             power (:obj:`float`): A value between [-1,1] used for joysticks to indicate how hard the buttons were
                 pressed. Defaults to ``1``.
             duration (:obj:`float`): The time measured in seconds from the key press to the key release.
             wait (:obj:`bool`): If set wait for command to finish. Defaults to ``True``.
@@ -719,15 +751,15 @@
             wait (:obj:`bool`, optional): If set wait for command to finish. Defaults to ``True``.
 
         """
 
         commands.TapCoordinates.run(self._connection, coordinates, count, interval, wait)
 
     def tilt(self, acceleration, duration=0.1, wait=True):
-        """Simulates device rotation action in your game.
+        """Simulates device rotation action in your application.
 
         Args:
             acceleration (:obj:`dict`): The linear acceleration of a device.
             duration (:obj:`int`, :obj:`float`, optional): How long the rotation will take in seconds.
                 Defaults to ``0.1``.
             wait (:obj:`bool`, optional): If set wait for command to finish. Defaults to ``True``.
 
@@ -740,15 +772,15 @@
             "UnityEngine.Screen", "get_width",
             "UnityEngine.CoreModule"
         )
         screen_height = self.call_static_method(
             "UnityEngine.Screen", "get_height",
             "UnityEngine.CoreModule"
         )
-        return [screen_width, screen_height]
+        return (screen_width, screen_height)
 
     def get_png_screenshot(self, path):
         """Creates a screenshot of the current scene in png format at the given path.
 
         Args:
             path (:obj:`str`): The path where the image will be created.
 
@@ -819,26 +851,14 @@
             AltObject: The UI object hit by event system Raycast, ``None`` otherwise.
 
         """
 
         data = commands.FindObjectAtCoordinates.run(self._connection, coordinates)
         return self._get_alt_object(data)
 
-    def set_notification(self, notification_type, notification_callback=None):
-        """Sets what notifications will the tester send and what to do with those notifications.
-
-        Args:
-            notification_type (:obj:`int`): Flag that sets which notification to be turned on.
-            notification_callback (:obj:`class`): Class which contains callbacks used by notifications.
-
-        """
-
-        self._connection.notification_callbacks = notification_callback
-        commands.SetNotification.run(self._connection, notification_type)
-
     def add_notification_listener(self, notification_type, notification_callback, overwrite=True):
         """Activates a notification that the tester will send.
 
         Args:
             notification_type (:obj:`int`): Flag that indicates which notification to be turned on.
             notification_callback (:obj:`method`): callback used when a notification is received.
             overwrite (:obj:'bool', optional): Flag to set if the new callback will overwrite the other
@@ -855,10 +875,10 @@
             notification_type (:obj:`int`): Flag that indicates which notification to be turned off.
 
         """
 
         commands.RemoveNotificationListener.run(self._connection, notification_type)
 
     def reset_input(self):
-        """Clear all active input actions simulated by AltTester.
-        """
+        """Clear all active input actions simulated by AltTester."""
+
         commands.ResetInput.run(self._connection)
```

### Comparing `AltTester-Driver-1.8.2/alttester/altobject.py` & `AltTester-Driver-2.0.0/alttester/altobject.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import json
 
 import alttester.commands as commands
 from alttester.by import By
 
 
 class AltObject:
-    """The AltObject class represents an object present in the game and it allows you to interact with it.
+    """The AltObject class represents an object present in the application and it allows you to interact with it.
 
     It is the return type of the methods in the “find_*” category from the AltDriver class.
     """
 
     def __init__(self, altdriver, data):
         self._altdriver = altdriver
         self._data = data
@@ -141,14 +141,39 @@
         return AltObject(self._altdriver, data)
 
     def get_all_components(self):
         """Returns all components."""
 
         return commands.GetAllComponents.run(self._connection, self)
 
+    def wait_for_component_property(self, component_name, property_name,
+                                    property_value, assembly,  timeout=20, interval=0.5):
+        """Wait until a property has a specific value and returns the value of the given component property.
+
+        Args:
+            component_name (:obj:`str`): The name of the component. If the component has a namespace the format should
+                look like this: ``"namespace.componentName"``.
+            property_name (:obj:`str`): The name of the property of which value you want. If the property is an array
+                you can specify which element of the array to return by doing ``property[index]``, or if you want a
+                property inside of another property you can get by doing ``property.subProperty``.
+            property_value(:obj:`str`): The value of the component expected
+            assembly (:obj:`str`): The name of the assembly containing the component.
+            timeout (:obj:`int`, optional): The number of seconds that it will wait for property.
+            interval (:obj:`float`, optional): The number of seconds after which it will try to find the object again.
+                The interval should be smaller than timeout.
+
+        Returns:
+            str: The property value is serialized to a JSON string.
+
+        """
+        return commands.WaitForComponentProperty.run(
+            component_name, property_name, property_value,
+            assembly, self, timeout, interval
+        )
+
     def get_component_property(self, component_name, property_name, assembly, max_depth=2):
         """Returns the value of the given component property.
 
         Args:
             component_name (:obj:`str`): The name of the component. If the component has a namespace the format should
                 look like this: ``"namespace.componentName"``.
             property_name (:obj:`str`): The name of the property of which value you want. If the property is an array
```

### Comparing `AltTester-Driver-1.8.2/alttester/commands/AltTesterCommands/add_notification_listener.py` & `AltTester-Driver-2.0.0/alttester/commands/AltTesterCommands/add_notification_listener.py`

 * *Files 2% similar despite different names*

```diff
@@ -38,12 +38,16 @@
         parameters.update(**{
             "notificationType": str(int(self.notification_type)),
         })
 
         return parameters
 
     def execute(self):
-        self.connection.add_notification_listener(self.notification_type, self.notification_callback, self.overwrite)
+        self.connection._notification_handler.add_notification_listener(
+            self.notification_type,
+            self.notification_callback,
+            self.overwrite
+        )
         data = self.send()
         self.validate_response("Ok", data)
 
         return data
```

### Comparing `AltTester-Driver-1.8.2/alttester/commands/AltTesterCommands/remove_notification_listener.py` & `AltTester-Driver-2.0.0/alttester/commands/AltTesterCommands/remove_notification_listener.py`

 * *Files 9% similar despite different names*

```diff
@@ -22,12 +22,12 @@
         parameters.update(**{
             "notificationType": str(int(self.notification_type)),
         })
 
         return parameters
 
     def execute(self):
-        self.connection.remove_notification_listener(self.notification_type)
+        self.connection._notification_handler.remove_notification_listener(self.notification_type)
         data = self.send()
         self.validate_response("Ok", data)
 
         return data
```

### Comparing `AltTester-Driver-1.8.2/alttester/commands/AltTesterCommands/set_server_logging.py` & `AltTester-Driver-2.0.0/alttester/commands/AltTesterCommands/set_server_logging.py`

 * *Files identical despite different names*

### Comparing `AltTester-Driver-1.8.2/alttester/commands/FindObjects/__init__.py` & `AltTester-Driver-2.0.0/alttester/commands/FindObjects/__init__.py`

 * *Files 9% similar despite different names*

```diff
@@ -2,7 +2,8 @@
 from alttester.commands.FindObjects.find_object import *
 from alttester.commands.FindObjects.find_objects import *
 from alttester.commands.FindObjects.find_objects_which_contains import *
 from alttester.commands.FindObjects.wait_for_object import *
 from alttester.commands.FindObjects.wait_for_object_to_not_be_present import *
 from alttester.commands.FindObjects.wait_for_object_which_contains import *
 from alttester.commands.FindObjects.find_object_at_coordinates import *
+from alttester.commands.FindObjects.wait_for_component_property import *
```

### Comparing `AltTester-Driver-1.8.2/alttester/commands/FindObjects/find_object.py` & `AltTester-Driver-2.0.0/alttester/commands/FindObjects/find_object.py`

 * *Files identical despite different names*

### Comparing `AltTester-Driver-1.8.2/alttester/commands/FindObjects/find_object_at_coordinates.py` & `AltTester-Driver-2.0.0/alttester/commands/FindObjects/find_object_at_coordinates.py`

 * *Files identical despite different names*

### Comparing `AltTester-Driver-1.8.2/alttester/commands/FindObjects/find_object_which_contains.py` & `AltTester-Driver-2.0.0/alttester/commands/FindObjects/find_object_which_contains.py`

 * *Files identical despite different names*

### Comparing `AltTester-Driver-1.8.2/alttester/commands/FindObjects/find_objects.py` & `AltTester-Driver-2.0.0/alttester/commands/FindObjects/find_objects.py`

 * *Files identical despite different names*

### Comparing `AltTester-Driver-1.8.2/alttester/commands/FindObjects/find_objects_which_contains.py` & `AltTester-Driver-2.0.0/alttester/commands/FindObjects/find_objects_which_contains.py`

 * *Files identical despite different names*

### Comparing `AltTester-Driver-1.8.2/alttester/commands/FindObjects/wait_for_object.py` & `AltTester-Driver-2.0.0/alttester/commands/FindObjects/wait_for_object.py`

 * *Files identical despite different names*

### Comparing `AltTester-Driver-1.8.2/alttester/commands/FindObjects/wait_for_object_to_not_be_present.py` & `AltTester-Driver-2.0.0/alttester/commands/FindObjects/wait_for_object_to_not_be_present.py`

 * *Files identical despite different names*

### Comparing `AltTester-Driver-1.8.2/alttester/commands/FindObjects/wait_for_object_which_contains.py` & `AltTester-Driver-2.0.0/alttester/commands/FindObjects/wait_for_object_which_contains.py`

 * *Files identical despite different names*

### Comparing `AltTester-Driver-1.8.2/alttester/commands/InputActions/__init__.py` & `AltTester-Driver-2.0.0/alttester/commands/InputActions/__init__.py`

 * *Files identical despite different names*

### Comparing `AltTester-Driver-1.8.2/alttester/commands/InputActions/begin_touch.py` & `AltTester-Driver-2.0.0/alttester/commands/InputActions/begin_touch.py`

 * *Files identical despite different names*

### Comparing `AltTester-Driver-1.8.2/alttester/commands/InputActions/click_coordinates.py` & `AltTester-Driver-2.0.0/alttester/commands/InputActions/click_coordinates.py`

 * *Files identical despite different names*

### Comparing `AltTester-Driver-1.8.2/alttester/commands/InputActions/end_touch.py` & `AltTester-Driver-2.0.0/alttester/commands/InputActions/end_touch.py`

 * *Files identical despite different names*

### Comparing `AltTester-Driver-1.8.2/alttester/commands/InputActions/keys_down.py` & `AltTester-Driver-2.0.0/alttester/commands/InputActions/keys_down.py`

 * *Files identical despite different names*

### Comparing `AltTester-Driver-1.8.2/alttester/commands/InputActions/keys_up.py` & `AltTester-Driver-2.0.0/alttester/commands/InputActions/keys_up.py`

 * *Files identical despite different names*

### Comparing `AltTester-Driver-1.8.2/alttester/commands/InputActions/move_mouse.py` & `AltTester-Driver-2.0.0/alttester/commands/InputActions/move_mouse.py`

 * *Files identical despite different names*

### Comparing `AltTester-Driver-1.8.2/alttester/commands/InputActions/move_touch.py` & `AltTester-Driver-2.0.0/alttester/commands/InputActions/move_touch.py`

 * *Files identical despite different names*

### Comparing `AltTester-Driver-1.8.2/alttester/commands/InputActions/multi_point_swipe.py` & `AltTester-Driver-2.0.0/alttester/commands/InputActions/multi_point_swipe.py`

 * *Files identical despite different names*

### Comparing `AltTester-Driver-1.8.2/alttester/commands/InputActions/press_keys.py` & `AltTester-Driver-2.0.0/alttester/commands/InputActions/press_keys.py`

 * *Files identical despite different names*

### Comparing `AltTester-Driver-1.8.2/alttester/commands/InputActions/scroll_mouse.py` & `AltTester-Driver-2.0.0/alttester/commands/InputActions/scroll_mouse.py`

 * *Files identical despite different names*

### Comparing `AltTester-Driver-1.8.2/alttester/commands/InputActions/swipe.py` & `AltTester-Driver-2.0.0/alttester/commands/InputActions/swipe.py`

 * *Files identical despite different names*

### Comparing `AltTester-Driver-1.8.2/alttester/commands/InputActions/tap_coordinates.py` & `AltTester-Driver-2.0.0/alttester/commands/InputActions/tap_coordinates.py`

 * *Files identical despite different names*

### Comparing `AltTester-Driver-1.8.2/alttester/commands/InputActions/tilt.py` & `AltTester-Driver-2.0.0/alttester/commands/InputActions/tilt.py`

 * *Files identical despite different names*

### Comparing `AltTester-Driver-1.8.2/alttester/commands/Notifications/base_notification_callbacks.py` & `AltTester-Driver-2.0.0/alttester/commands/Notifications/base_notification_callbacks.py`

 * *Files identical despite different names*

### Comparing `AltTester-Driver-1.8.2/alttester/commands/ObjectCommands/__init__.py` & `AltTester-Driver-2.0.0/alttester/commands/ObjectCommands/__init__.py`

 * *Files identical despite different names*

### Comparing `AltTester-Driver-1.8.2/alttester/commands/ObjectCommands/call_method.py` & `AltTester-Driver-2.0.0/alttester/commands/ObjectCommands/call_method.py`

 * *Files identical despite different names*

### Comparing `AltTester-Driver-1.8.2/alttester/commands/ObjectCommands/click_element.py` & `AltTester-Driver-2.0.0/alttester/commands/ObjectCommands/click_element.py`

 * *Files identical despite different names*

### Comparing `AltTester-Driver-1.8.2/alttester/commands/ObjectCommands/get_component_property.py` & `AltTester-Driver-2.0.0/alttester/commands/ObjectCommands/get_component_property.py`

 * *Files identical despite different names*

### Comparing `AltTester-Driver-1.8.2/alttester/commands/ObjectCommands/set_component_property.py` & `AltTester-Driver-2.0.0/alttester/commands/ObjectCommands/set_component_property.py`

 * *Files identical despite different names*

### Comparing `AltTester-Driver-1.8.2/alttester/commands/ObjectCommands/set_text.py` & `AltTester-Driver-2.0.0/alttester/commands/ObjectCommands/set_text.py`

 * *Files identical despite different names*

### Comparing `AltTester-Driver-1.8.2/alttester/commands/ObjectCommands/tap_element.py` & `AltTester-Driver-2.0.0/alttester/commands/ObjectCommands/tap_element.py`

 * *Files identical despite different names*

### Comparing `AltTester-Driver-1.8.2/alttester/commands/UnityCommands/__init__.py` & `AltTester-Driver-2.0.0/alttester/commands/UnityCommands/__init__.py`

 * *Files identical despite different names*

### Comparing `AltTester-Driver-1.8.2/alttester/commands/UnityCommands/get_player_pref_key.py` & `AltTester-Driver-2.0.0/alttester/commands/UnityCommands/get_player_pref_key.py`

 * *Files identical despite different names*

### Comparing `AltTester-Driver-1.8.2/alttester/commands/UnityCommands/load_scene.py` & `AltTester-Driver-2.0.0/alttester/commands/UnityCommands/load_scene.py`

 * *Files identical despite different names*

### Comparing `AltTester-Driver-1.8.2/alttester/commands/UnityCommands/set_player_pref_key.py` & `AltTester-Driver-2.0.0/alttester/commands/UnityCommands/set_player_pref_key.py`

 * *Files identical despite different names*

### Comparing `AltTester-Driver-1.8.2/alttester/commands/UnityCommands/set_time_scale.py` & `AltTester-Driver-2.0.0/alttester/commands/UnityCommands/set_time_scale.py`

 * *Files identical despite different names*

### Comparing `AltTester-Driver-1.8.2/alttester/commands/UnityCommands/unload_scene.py` & `AltTester-Driver-2.0.0/alttester/commands/UnityCommands/unload_scene.py`

 * *Files identical despite different names*

### Comparing `AltTester-Driver-1.8.2/alttester/commands/UnityCommands/wait_for_current_scene_to_be.py` & `AltTester-Driver-2.0.0/alttester/commands/UnityCommands/wait_for_current_scene_to_be.py`

 * *Files identical despite different names*

### Comparing `AltTester-Driver-1.8.2/alttester/commands/__init__.py` & `AltTester-Driver-2.0.0/alttester/commands/__init__.py`

 * *Files identical despite different names*

### Comparing `AltTester-Driver-1.8.2/alttester/commands/base_command.py` & `AltTester-Driver-2.0.0/alttester/commands/base_command.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 import abc
 import json
 import time
 from datetime import datetime
+
 from loguru import logger
 
 import alttester.exceptions as exceptions
 from alttester.by import By
 
 
 EPOCH = datetime.utcfromtimestamp(0)
```

### Comparing `AltTester-Driver-1.8.2/alttester/commands/get_static_property.py` & `AltTester-Driver-2.0.0/alttester/commands/get_static_property.py`

 * *Files identical despite different names*

### Comparing `AltTester-Driver-1.8.2/alttester/commands/set_static_property.py` & `AltTester-Driver-2.0.0/alttester/commands/set_static_property.py`

 * *Files identical despite different names*

### Comparing `AltTester-Driver-1.8.2/alttester/exceptions.py` & `AltTester-Driver-2.0.0/alttester/exceptions.py`

 * *Files 3% similar despite different names*

```diff
@@ -2,23 +2,31 @@
 
 
 class AltException(Exception):
     """Base exception class for AltTester."""
 
 
 class ConnectionError(AltException):
-    """Raised when the client can not connect to the server."""
+    """Raised when the client can not connect to the server. Used as base class for all connection exceptions."""
 
 
 class ConnectionTimeoutError(ConnectionError):
-    """Raised when the client connection timesout."""
+    """Raised when the client connection timeouts."""
+
+
+class NoAppConnected(ConnectionError):
+    """Raised when the client tries to connect to a server without an app."""
+
+
+class AppDisconnectedError(ConnectionError):
+    """Raised when the app closed the connection or unexpectedly disconnected."""
 
 
 class AltTesterInvalidServerResponse(AltException):
-    """Raised when the server responds with an invalid respose."""
+    """Raised when the server responds with an invalid response."""
 
     def __init__(self, expected, received):
         super().__init__("Expected to get response {}; got {}".format(expected, received))
 
 
 class InvalidParameterTypeException(TypeError, AltException):
     """Raised when an function or method receives an parameter that has the inappropriate type."""
@@ -69,15 +77,15 @@
 
 
 class AssemblyNotFoundException(NotFoundException):
     """Raised when an assembly is not found."""
 
 
 class CouldNotPerformOperationException(AltException):
-    """Raised when an opperation could not be performed."""
+    """Raised when an operation could not be performed."""
 
 
 class CouldNotParseJsonStringException(AltException):
     """Raised when AltTester could not parse an JSON command."""
 
 
 class NullReferenceException(AltException):
@@ -101,15 +109,15 @@
 
 
 class FormatException(AltException):
     pass
 
 
 class InvalidPathException(AltException):
-    """Raised when a command recives an invalid path."""
+    """Raised when a command receives an invalid path."""
 
 
 class AltTesterInputModuleException(AltException):
     pass
 
 
 class UnknownErrorException(AltException):
```

### Comparing `AltTester-Driver-1.8.2/alttester/keycode.py` & `AltTester-Driver-2.0.0/alttester/keycode.py`

 * *Files identical despite different names*

### Comparing `AltTester-Driver-1.8.2/setup.py` & `AltTester-Driver-2.0.0/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 
 
 NAME = 'AltTester-Driver'
 DESCRIPTION = "Python bindings for the AltTester framework. AltTester is an open-source UI driven test " \
     "automation tool that helps you find objects in your game and interacts with them."
-URL = 'https://altom.com/alttester/docs/sdk'
-EMAIL = 'suport.alttester@altom.com'
+URL = 'https://alttester.com/docs/pro/sdk'
+EMAIL = 'contact@alttester.com'
 AUTHOR = 'Altom Consulting'
 REQUIRES_PYTHON = '>=3.4.0'
 LICENSE = 'GNU GPLv3'
 
 
 with open("alttester/__version__.py") as f:
     VERSION = f.readline().replace("VERSION = ", "").replace("\"", "").replace("\n", "")
@@ -29,15 +29,15 @@
     description=DESCRIPTION,
     long_description=README,
     long_description_content_type='text/markdown',
     license=LICENSE,
     url=URL,
     project_urls={
         "Bug Tracker": "https://github.com/alttester/AltTester-Unity-SDK/issues",
-        "Documentation": "https://altom.com/alttester/docs/sdk",
+        "Documentation": "https://alttester.com/docs/pro/sdk",
         "Source": "https://github.com/alttester/AltTester-Unity-SDK",
     },
 
     author=AUTHOR,
     author_email=EMAIL,
 
     zip_safe=False,
```

### Comparing `AltTester-Driver-1.8.2/tests/integration/test_driver.py` & `AltTester-Driver-2.0.0/tests/integration/test_driver.py`

 * *Files 2% similar despite different names*

```diff
@@ -84,28 +84,29 @@
 
     def test_unload_only_scene(self):
         self.altdriver.load_scene(Scenes.Scene01, load_single=True)
 
         with pytest.raises(exceptions.CouldNotPerformOperationException):
             self.altdriver.unload_scene(Scenes.Scene01)
 
+    @pytest.mark.WebGLUnsupported
     def test_set_server_logging(self):
         rule = self.altdriver.call_static_method(
-            "Altom.AltTester.Logging.ServerLogManager",
+            "AltTester.AltTesterUnitySDK.Logging.ServerLogManager",
             "Instance.Configuration.FindRuleByName",
             "Assembly-CSharp",
             parameters=["AltServerFileRule"],
         )
 
         # Default logging level in AltTester is Debug level
         assert len(rule["Levels"]) == 5
 
         self.altdriver.set_server_logging(AltLogger.File, AltLogLevel.Off)
         rule = self.altdriver.call_static_method(
-            "Altom.AltTester.Logging.ServerLogManager",
+            "AltTester.AltTesterUnitySDK.Logging.ServerLogManager",
             "Instance.Configuration.FindRuleByName",
             "Assembly-CSharp",
             parameters=["AltServerFileRule"],
         )
 
         assert len(rule["Levels"]) == 0
```

### Comparing `AltTester-Driver-1.8.2/tests/integration/test_notifications.py` & `AltTester-Driver-2.0.0/tests/integration/test_notifications.py`

 * *Files 1% similar despite different names*

```diff
@@ -67,14 +67,14 @@
     def test_application_paused_notification(self):
         test_notification_callbacks = MockNotificationCallbacks()
         self.altdriver.add_notification_listener(
             NotificationType.APPLICATION_PAUSED, test_notification_callbacks.application_paused_callback)
         self.altdriver.load_scene(Scenes.Scene01)
         alt_object = self.altdriver.find_object(By.NAME, "AltTesterPrefab")
         alt_object.call_component_method(
-            "Altom.AltTester.AltRunner", "OnApplicationPause", "Assembly-CSharp",
+            "AltTester.AltTesterUnitySDK.AltRunner", "OnApplicationPause", "AltTester.AltTesterUnitySDK",
             parameters=[True],
             type_of_parameters=["System.Boolean"]
         )
 
         assert test_notification_callbacks.application_paused
         self.altdriver.remove_notification_listener(NotificationType.APPLICATION_PAUSED)
```

### Comparing `AltTester-Driver-1.8.2/tests/integration/test_scene01.py` & `AltTester-Driver-2.0.0/tests/integration/test_scene01.py`

 * *Files 1% similar despite different names*

```diff
@@ -139,14 +139,15 @@
     def test_wait_for_object_by_name(self):
         plane = self.altdriver.wait_for_object(By.NAME, "Plane")
         capsule = self.altdriver.wait_for_object(By.NAME, "Capsule")
 
         assert plane.name == "Plane"
         assert capsule.name == "Capsule"
 
+    @pytest.mark.WebGLUnsupported
     def test_get_application_screen_size(self):
         self.altdriver.call_static_method(
             "UnityEngine.Screen", "SetResolution", "UnityEngine.CoreModule",
             parameters=["1920", "1080", "True"],
             type_of_parameters=["System.Int32", "System.Int32", "System.Boolean"],
         )
         screensize = self.altdriver.get_application_screensize()
@@ -223,14 +224,22 @@
 
         time.sleep(2)
 
         capsule_info = self.altdriver.find_object(By.NAME, "CapsuleInfo")
         text = capsule_info.get_text()
         assert text == "UIButton clicked to jump capsule!"
 
+    def test_wait_for_component_property(self):
+        alt_object = self.altdriver.find_object(By.NAME, "Capsule")
+        result = alt_object.wait_for_component_property(
+            "AltExampleScriptCapsule", "TestBool", True,
+            "Assembly-CSharp")
+
+        assert result is True
+
     def test_get_component_property(self):
         alt_object = self.altdriver.find_object(By.NAME, "Capsule")
         result = alt_object.get_component_property(
             "AltExampleScriptCapsule", "arrayOfInts", "Assembly-CSharp")
 
         assert result == [1, 2, 3]
 
@@ -711,14 +720,15 @@
 
         assert input_field.get_text() == "example"
         assert input_field.get_component_property(
             "AltInputFieldRaisedEvents", "onValueChangedInvoked", "Assembly-CSharp")
         assert input_field.get_component_property(
             "AltInputFieldRaisedEvents", "onSubmitInvoked", "Assembly-CSharp")
 
+    @pytest.mark.WebGLUnsupported
     def test_get_static_property(self):
 
         self.altdriver.call_static_method(
             "UnityEngine.Screen", "SetResolution", "UnityEngine.CoreModule",
             parameters=["1920", "1080", "True"],
             type_of_parameters=["System.Int32", "System.Int32", "System.Boolean"],
         )
@@ -763,24 +773,17 @@
         plane = self.altdriver.find_object(By.NAME, "Plane")
 
         assert type(plane.worldX) == float
         assert type(plane.worldY) == float
         assert type(plane.worldZ) == float
 
     def test_set_command_response_timeout(self):
-        alt_object = self.altdriver.find_object(By.NAME, "Capsule")
         self.altdriver.set_command_response_timeout(1)
-
         with pytest.raises(exceptions.CommandResponseTimeoutException) as execinfo:
-
-            alt_object.call_component_method(
-                "AltExampleScriptCapsule", "JumpWithDelay", "Assembly-CSharp",
-                parameters=[], type_of_parameters=[],
-            )
-
+            self.altdriver.tilt([1, 1, 1], duration=2, wait=True)
         self.altdriver.set_command_response_timeout(60)
         assert str(execinfo.value) == ""
 
     def test_keys_down(self):
         keys = [AltKeyCode.K, AltKeyCode.L]
         self.altdriver.keys_down(keys)
         self.altdriver.keys_up(keys)
@@ -821,15 +824,17 @@
                                               "callJump", "Assembly-CSharp", parameters=[])
         capsule_info = self.altdriver.find_object(By.NAME, "CapsuleInfo")
         assert capsule_info.get_text() == "Capsule jumps!"
 
     def test_reset_input(self):
         self.altdriver.key_down(AltKeyCode.P, 1)
         assert self.altdriver.find_object(By.NAME, "AltTesterPrefab").get_component_property(
-            "Altom.AltTester.NewInputSystem", "Keyboard.pKey.isPressed", "Assembly-CSharp") is True
+            "AltTester.AltTesterUnitySDK.NewInputSystem",
+            "Keyboard.pKey.isPressed", "AltTester.AltTesterUnitySDK") is True
         self.altdriver.reset_input()
         assert self.altdriver.find_object(By.NAME, "AltTesterPrefab").get_component_property(
-            "Altom.AltTester.NewInputSystem", "Keyboard.pKey.isPressed", "Assembly-CSharp") is False
+            "AltTester.AltTesterUnitySDK.NewInputSystem",
+            "Keyboard.pKey.isPressed", "AltTester.AltTesterUnitySDK") is False
 
         countKeyDown = self.altdriver.find_object(By.NAME, "AltTesterPrefab").get_component_property(
-            "Input", "_keyCodesPressed.Count", "Assembly-CSharp")
+            "Input", "_keyCodesPressed.Count", "AltTester.AltTesterUnitySDK")
         assert 0 == countKeyDown
```

### Comparing `AltTester-Driver-1.8.2/tests/integration/test_scene02.py` & `AltTester-Driver-2.0.0/tests/integration/test_scene02.py`

 * *Files identical despite different names*

### Comparing `AltTester-Driver-1.8.2/tests/integration/test_scene03.py` & `AltTester-Driver-2.0.0/tests/integration/test_scene03.py`

 * *Files identical despite different names*

### Comparing `AltTester-Driver-1.8.2/tests/integration/test_scene05.py` & `AltTester-Driver-2.0.0/tests/integration/test_scene05.py`

 * *Files identical despite different names*

### Comparing `AltTester-Driver-1.8.2/tests/integration/test_scene07.py` & `AltTester-Driver-2.0.0/tests/integration/test_scene07.py`

 * *Ordering differences only*

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import pytest
+from alttester import By
 
 from .utils import Scenes
-from alttester import By
 
 
 class TestScene07A:
 
     @pytest.fixture(autouse=True)
     def setup(self, altdriver):
         self.altdriver = altdriver
```

### Comparing `AltTester-Driver-1.8.2/tests/integration/test_scene09.py` & `AltTester-Driver-2.0.0/tests/integration/test_scene09.py`

 * *Files identical despite different names*

### Comparing `AltTester-Driver-1.8.2/tests/integration/test_scene10.py` & `AltTester-Driver-2.0.0/tests/integration/test_scene10.py`

 * *Files identical despite different names*

### Comparing `AltTester-Driver-1.8.2/tests/unit/test_altobject.py` & `AltTester-Driver-2.0.0/tests/unit/test_altobject.py`

 * *Files identical despite different names*

### Comparing `AltTester-Driver-1.8.2/tests/unit/test_commands.py` & `AltTester-Driver-2.0.0/tests/unit/test_commands.py`

 * *Files identical despite different names*

### Comparing `AltTester-Driver-1.8.2/tests/unit/test_websocket.py` & `AltTester-Driver-2.0.0/tests/unit/test_websocket.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import json
 import unittest.mock as mock
 
 import pytest
 
-from alttester._websocket import Store, WebsocketConnection
+from alttester._websocket import Store, WebsocketConnection, CommandHandler, NotificationHandler
 from alttester.exceptions import ConnectionError
 
 
 class TestStore:
 
     @pytest.fixture(autouse=True)
     def setup(self):
@@ -79,15 +79,17 @@
         self.create_connection_mock = mock.Mock(
             return_value=self.websocket_mock
         )
 
         self.connection = WebsocketConnection(
             host=self.host,
             port=self.port,
-            timeout=self.timeout
+            timeout=self.timeout,
+            command_handler=CommandHandler(),
+            notification_handler=NotificationHandler()
         )
         self.connection._create_connection = self.create_connection_mock
         self.connection._is_open = True
 
     def test_connect(self):
         self.connection.connect()
         self.create_connection_mock.assert_called_once()
```

