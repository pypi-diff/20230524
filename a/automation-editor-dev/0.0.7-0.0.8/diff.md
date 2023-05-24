# Comparing `tmp/automation_editor_dev-0.0.7.tar.gz` & `tmp/automation_editor_dev-0.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "automation_editor_dev-0.0.7.tar", last modified: Thu May 18 02:12:23 2023, max compression
+gzip compressed data, was "automation_editor_dev-0.0.8.tar", last modified: Mon May 22 09:27:44 2023, max compression
```

## Comparing `automation_editor_dev-0.0.7.tar` & `automation_editor_dev-0.0.8.tar`

### file list

```diff
@@ -1,82 +1,82 @@
-drwxrwxrwx   0        0        0        0 2023-05-18 02:12:23.501745 automation_editor_dev-0.0.7/
--rw-rw-rw-   0        0        0     1085 2023-04-19 01:59:04.000000 automation_editor_dev-0.0.7/LICENSE
--rw-rw-rw-   0        0        0     5889 2023-05-18 02:12:23.500838 automation_editor_dev-0.0.7/PKG-INFO
--rw-rw-rw-   0        0        0     5065 2023-05-02 01:28:19.000000 automation_editor_dev-0.0.7/README.md
-drwxrwxrwx   0        0        0        0 2023-05-18 02:12:23.285205 automation_editor_dev-0.0.7/automation_editor/
--rw-rw-rw-   0        0        0      130 2023-05-02 01:28:19.000000 automation_editor_dev-0.0.7/automation_editor/__init__.py
--rw-rw-rw-   0        0        0        0 2023-05-02 01:28:19.000000 automation_editor_dev-0.0.7/automation_editor/__main__.py
-drwxrwxrwx   0        0        0        0 2023-05-18 02:12:23.291950 automation_editor_dev-0.0.7/automation_editor/automation_editor_ui/
--rw-rw-rw-   0        0        0        0 2023-05-02 01:28:19.000000 automation_editor_dev-0.0.7/automation_editor/automation_editor_ui/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-18 02:12:23.298204 automation_editor_dev-0.0.7/automation_editor/automation_editor_ui/editor_main/
--rw-rw-rw-   0        0        0        0 2023-05-02 01:28:19.000000 automation_editor_dev-0.0.7/automation_editor/automation_editor_ui/editor_main/__init__.py
--rw-rw-rw-   0        0        0     1622 2023-05-18 02:09:55.000000 automation_editor_dev-0.0.7/automation_editor/automation_editor_ui/editor_main/main_ui.py
-drwxrwxrwx   0        0        0        0 2023-05-18 02:12:23.305247 automation_editor_dev-0.0.7/automation_editor/automation_editor_ui/menu/
--rw-rw-rw-   0        0        0        0 2023-05-02 01:28:19.000000 automation_editor_dev-0.0.7/automation_editor/automation_editor_ui/menu/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-18 02:12:23.311255 automation_editor_dev-0.0.7/automation_editor/automation_editor_ui/menu/api_testka_menu/
--rw-rw-rw-   0        0        0        0 2023-05-02 01:28:19.000000 automation_editor_dev-0.0.7/automation_editor/automation_editor_ui/menu/api_testka_menu/__init__.py
--rw-rw-rw-   0        0        0     4000 2023-05-03 02:40:57.000000 automation_editor_dev-0.0.7/automation_editor/automation_editor_ui/menu/api_testka_menu/build_api_testka_menu.py
-drwxrwxrwx   0        0        0        0 2023-05-18 02:12:23.321504 automation_editor_dev-0.0.7/automation_editor/automation_editor_ui/menu/auto_control_menu/
--rw-rw-rw-   0        0        0        0 2023-05-02 01:28:19.000000 automation_editor_dev-0.0.7/automation_editor/automation_editor_ui/menu/auto_control_menu/__init__.py
--rw-rw-rw-   0        0        0     4129 2023-05-03 02:33:10.000000 automation_editor_dev-0.0.7/automation_editor/automation_editor_ui/menu/auto_control_menu/build_autocontrol_menu.py
-drwxrwxrwx   0        0        0        0 2023-05-18 02:12:23.328110 automation_editor_dev-0.0.7/automation_editor/automation_editor_ui/menu/install_menu/
--rw-rw-rw-   0        0        0        0 2023-05-03 02:30:10.000000 automation_editor_dev-0.0.7/automation_editor/automation_editor_ui/menu/install_menu/__init__.py
--rw-rw-rw-   0        0        0     3556 2023-05-18 02:09:55.000000 automation_editor_dev-0.0.7/automation_editor/automation_editor_ui/menu/install_menu/build_install_menu.py
-drwxrwxrwx   0        0        0        0 2023-05-18 02:12:23.335167 automation_editor_dev-0.0.7/automation_editor/automation_editor_ui/menu/load_density_menu/
--rw-rw-rw-   0        0        0        0 2023-05-02 01:28:19.000000 automation_editor_dev-0.0.7/automation_editor/automation_editor_ui/menu/load_density_menu/__init__.py
--rw-rw-rw-   0        0        0     4163 2023-05-03 02:40:57.000000 automation_editor_dev-0.0.7/automation_editor/automation_editor_ui/menu/load_density_menu/build_load_density_menu.py
-drwxrwxrwx   0        0        0        0 2023-05-18 02:12:23.342077 automation_editor_dev-0.0.7/automation_editor/automation_editor_ui/menu/web_runner_menu/
--rw-rw-rw-   0        0        0        0 2023-05-02 01:28:19.000000 automation_editor_dev-0.0.7/automation_editor/automation_editor_ui/menu/web_runner_menu/__init__.py
--rw-rw-rw-   0        0        0     4040 2023-05-03 02:39:24.000000 automation_editor_dev-0.0.7/automation_editor/automation_editor_ui/menu/web_runner_menu/build_webrunner_menu.py
-drwxrwxrwx   0        0        0        0 2023-05-18 02:12:23.348957 automation_editor_dev-0.0.7/automation_editor/automation_editor_ui/show_code_window/
--rw-rw-rw-   0        0        0        0 2023-05-02 01:28:19.000000 automation_editor_dev-0.0.7/automation_editor/automation_editor_ui/show_code_window/__init__.py
--rw-rw-rw-   0        0        0      791 2023-05-02 01:28:19.000000 automation_editor_dev-0.0.7/automation_editor/automation_editor_ui/show_code_window/code_window.py
-drwxrwxrwx   0        0        0        0 2023-05-18 02:12:23.361456 automation_editor_dev-0.0.7/automation_editor/automation_editor_ui/syntax/
--rw-rw-rw-   0        0        0        0 2023-05-02 01:28:19.000000 automation_editor_dev-0.0.7/automation_editor/automation_editor_ui/syntax/__init__.py
--rw-rw-rw-   0        0        0      777 2023-05-02 01:28:19.000000 automation_editor_dev-0.0.7/automation_editor/automation_editor_ui/syntax/syntax_extend.py
--rw-rw-rw-   0        0        0     3257 2023-05-02 01:28:19.000000 automation_editor_dev-0.0.7/automation_editor/automation_editor_ui/syntax/syntax_keyword.py
-drwxrwxrwx   0        0        0        0 2023-05-18 02:12:23.365958 automation_editor_dev-0.0.7/automation_editor/extend/
--rw-rw-rw-   0        0        0        0 2023-05-02 01:28:19.000000 automation_editor_dev-0.0.7/automation_editor/extend/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-18 02:12:23.369985 automation_editor_dev-0.0.7/automation_editor/extend/mail_thunder_extend/
--rw-rw-rw-   0        0        0        0 2023-05-02 01:28:19.000000 automation_editor_dev-0.0.7/automation_editor/extend/mail_thunder_extend/__init__.py
--rw-rw-rw-   0        0        0     1696 2023-05-02 01:28:19.000000 automation_editor_dev-0.0.7/automation_editor/extend/mail_thunder_extend/mail_thunder_setting.py
-drwxrwxrwx   0        0        0        0 2023-05-18 02:12:23.372958 automation_editor_dev-0.0.7/automation_editor/utils/
--rw-rw-rw-   0        0        0        0 2023-05-02 01:28:19.000000 automation_editor_dev-0.0.7/automation_editor/utils/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-18 02:12:23.382007 automation_editor_dev-0.0.7/automation_editor/utils/exception/
--rw-rw-rw-   0        0        0        0 2023-05-02 01:28:19.000000 automation_editor_dev-0.0.7/automation_editor/utils/exception/__init__.py
--rw-rw-rw-   0        0        0     1513 2023-05-03 08:50:31.000000 automation_editor_dev-0.0.7/automation_editor/utils/exception/exception_tags.py
--rw-rw-rw-   0        0        0      608 2023-05-02 01:28:19.000000 automation_editor_dev-0.0.7/automation_editor/utils/exception/exceptions.py
-drwxrwxrwx   0        0        0        0 2023-05-18 02:12:23.391647 automation_editor_dev-0.0.7/automation_editor/utils/file_process/
--rw-rw-rw-   0        0        0        0 2023-05-02 01:28:19.000000 automation_editor_dev-0.0.7/automation_editor/utils/file_process/__init__.py
--rw-rw-rw-   0        0        0     1171 2023-05-02 09:53:50.000000 automation_editor_dev-0.0.7/automation_editor/utils/file_process/get_dir_file_list.py
-drwxrwxrwx   0        0        0        0 2023-05-18 02:12:23.403435 automation_editor_dev-0.0.7/automation_editor/utils/json_format/
--rw-rw-rw-   0        0        0        2 2023-05-02 01:28:19.000000 automation_editor_dev-0.0.7/automation_editor/utils/json_format/__init__.py
--rw-rw-rw-   0        0        0      991 2023-05-02 01:28:19.000000 automation_editor_dev-0.0.7/automation_editor/utils/json_format/json_process.py
-drwxrwxrwx   0        0        0        0 2023-05-18 02:12:23.405971 automation_editor_dev-0.0.7/automation_editor/utils/manager/
--rw-rw-rw-   0        0        0        0 2023-05-02 01:28:19.000000 automation_editor_dev-0.0.7/automation_editor/utils/manager/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-18 02:12:23.413421 automation_editor_dev-0.0.7/automation_editor/utils/manager/package_manager/
--rw-rw-rw-   0        0        0        0 2023-05-02 01:28:19.000000 automation_editor_dev-0.0.7/automation_editor/utils/manager/package_manager/__init__.py
--rw-rw-rw-   0        0        0      558 2023-05-03 02:11:15.000000 automation_editor_dev-0.0.7/automation_editor/utils/manager/package_manager/package_manager_class.py
-drwxrwxrwx   0        0        0        0 2023-05-18 02:12:23.429007 automation_editor_dev-0.0.7/automation_editor/utils/test_executor/
--rw-rw-rw-   0        0        0        0 2023-05-02 01:28:19.000000 automation_editor_dev-0.0.7/automation_editor/utils/test_executor/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-18 02:12:23.438143 automation_editor_dev-0.0.7/automation_editor/utils/test_executor/api_testka/
--rw-rw-rw-   0        0        0        0 2023-05-02 01:28:19.000000 automation_editor_dev-0.0.7/automation_editor/utils/test_executor/api_testka/__init__.py
--rw-rw-rw-   0        0        0     3935 2023-05-02 01:28:19.000000 automation_editor_dev-0.0.7/automation_editor/utils/test_executor/api_testka/api_testka_process.py
-drwxrwxrwx   0        0        0        0 2023-05-18 02:12:23.446281 automation_editor_dev-0.0.7/automation_editor/utils/test_executor/auto_control/
--rw-rw-rw-   0        0        0        0 2023-05-02 01:28:19.000000 automation_editor_dev-0.0.7/automation_editor/utils/test_executor/auto_control/__init__.py
--rw-rw-rw-   0        0        0     3939 2023-05-02 01:28:19.000000 automation_editor_dev-0.0.7/automation_editor/utils/test_executor/auto_control/auto_control_process.py
--rw-rw-rw-   0        0        0      498 2023-05-02 01:28:19.000000 automation_editor_dev-0.0.7/automation_editor/utils/test_executor/check_mail_thunder.py
-drwxrwxrwx   0        0        0        0 2023-05-18 02:12:23.452278 automation_editor_dev-0.0.7/automation_editor/utils/test_executor/load_density/
--rw-rw-rw-   0        0        0        0 2023-05-02 01:28:19.000000 automation_editor_dev-0.0.7/automation_editor/utils/test_executor/load_density/__init__.py
--rw-rw-rw-   0        0        0     3949 2023-05-02 01:28:19.000000 automation_editor_dev-0.0.7/automation_editor/utils/test_executor/load_density/load_density_process.py
--rw-rw-rw-   0        0        0     7109 2023-05-03 08:50:31.000000 automation_editor_dev-0.0.7/automation_editor/utils/test_executor/task_process_manager.py
-drwxrwxrwx   0        0        0        0 2023-05-18 02:12:23.459291 automation_editor_dev-0.0.7/automation_editor/utils/test_executor/web_runner/
--rw-rw-rw-   0        0        0        0 2023-05-02 01:28:19.000000 automation_editor_dev-0.0.7/automation_editor/utils/test_executor/web_runner/__init__.py
--rw-rw-rw-   0        0        0     3897 2023-05-02 01:28:19.000000 automation_editor_dev-0.0.7/automation_editor/utils/test_executor/web_runner/web_runner_process.py
-drwxrwxrwx   0        0        0        0 2023-05-18 02:12:23.497846 automation_editor_dev-0.0.7/automation_editor_dev.egg-info/
--rw-rw-rw-   0        0        0     5889 2023-05-18 02:12:23.000000 automation_editor_dev-0.0.7/automation_editor_dev.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     3099 2023-05-18 02:12:23.000000 automation_editor_dev-0.0.7/automation_editor_dev.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-18 02:12:23.000000 automation_editor_dev-0.0.7/automation_editor_dev.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      104 2023-05-18 02:12:23.000000 automation_editor_dev-0.0.7/automation_editor_dev.egg-info/requires.txt
--rw-rw-rw-   0        0        0       18 2023-05-18 02:12:23.000000 automation_editor_dev-0.0.7/automation_editor_dev.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     1272 2023-05-18 02:12:07.000000 automation_editor_dev-0.0.7/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-05-18 02:12:23.503459 automation_editor_dev-0.0.7/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-05-22 09:27:44.075374 automation_editor_dev-0.0.8/
+-rw-rw-rw-   0        0        0     1085 2023-04-19 01:59:04.000000 automation_editor_dev-0.0.8/LICENSE
+-rw-rw-rw-   0        0        0     5889 2023-05-22 09:27:44.073867 automation_editor_dev-0.0.8/PKG-INFO
+-rw-rw-rw-   0        0        0     5065 2023-05-02 01:28:19.000000 automation_editor_dev-0.0.8/README.md
+drwxrwxrwx   0        0        0        0 2023-05-22 09:27:43.878141 automation_editor_dev-0.0.8/automation_editor/
+-rw-rw-rw-   0        0        0      130 2023-05-02 01:28:19.000000 automation_editor_dev-0.0.8/automation_editor/__init__.py
+-rw-rw-rw-   0        0        0        0 2023-05-02 01:28:19.000000 automation_editor_dev-0.0.8/automation_editor/__main__.py
+drwxrwxrwx   0        0        0        0 2023-05-22 09:27:43.881272 automation_editor_dev-0.0.8/automation_editor/automation_editor_ui/
+-rw-rw-rw-   0        0        0        0 2023-05-02 01:28:19.000000 automation_editor_dev-0.0.8/automation_editor/automation_editor_ui/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-22 09:27:43.888288 automation_editor_dev-0.0.8/automation_editor/automation_editor_ui/editor_main/
+-rw-rw-rw-   0        0        0        0 2023-05-02 01:28:19.000000 automation_editor_dev-0.0.8/automation_editor/automation_editor_ui/editor_main/__init__.py
+-rw-rw-rw-   0        0        0     2087 2023-05-22 09:17:26.000000 automation_editor_dev-0.0.8/automation_editor/automation_editor_ui/editor_main/main_ui.py
+drwxrwxrwx   0        0        0        0 2023-05-22 09:27:43.890286 automation_editor_dev-0.0.8/automation_editor/automation_editor_ui/menu/
+-rw-rw-rw-   0        0        0        0 2023-05-02 01:28:19.000000 automation_editor_dev-0.0.8/automation_editor/automation_editor_ui/menu/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-22 09:27:43.896297 automation_editor_dev-0.0.8/automation_editor/automation_editor_ui/menu/api_testka_menu/
+-rw-rw-rw-   0        0        0        0 2023-05-02 01:28:19.000000 automation_editor_dev-0.0.8/automation_editor/automation_editor_ui/menu/api_testka_menu/__init__.py
+-rw-rw-rw-   0        0        0     4016 2023-05-22 01:10:45.000000 automation_editor_dev-0.0.8/automation_editor/automation_editor_ui/menu/api_testka_menu/build_api_testka_menu.py
+drwxrwxrwx   0        0        0        0 2023-05-22 09:27:43.902770 automation_editor_dev-0.0.8/automation_editor/automation_editor_ui/menu/auto_control_menu/
+-rw-rw-rw-   0        0        0        0 2023-05-02 01:28:19.000000 automation_editor_dev-0.0.8/automation_editor/automation_editor_ui/menu/auto_control_menu/__init__.py
+-rw-rw-rw-   0        0        0     4145 2023-05-22 01:10:45.000000 automation_editor_dev-0.0.8/automation_editor/automation_editor_ui/menu/auto_control_menu/build_autocontrol_menu.py
+drwxrwxrwx   0        0        0        0 2023-05-22 09:27:43.908825 automation_editor_dev-0.0.8/automation_editor/automation_editor_ui/menu/install_menu/
+-rw-rw-rw-   0        0        0        0 2023-05-03 02:30:10.000000 automation_editor_dev-0.0.8/automation_editor/automation_editor_ui/menu/install_menu/__init__.py
+-rw-rw-rw-   0        0        0     3604 2023-05-22 01:10:45.000000 automation_editor_dev-0.0.8/automation_editor/automation_editor_ui/menu/install_menu/build_install_menu.py
+drwxrwxrwx   0        0        0        0 2023-05-22 09:27:43.915331 automation_editor_dev-0.0.8/automation_editor/automation_editor_ui/menu/load_density_menu/
+-rw-rw-rw-   0        0        0        0 2023-05-02 01:28:19.000000 automation_editor_dev-0.0.8/automation_editor/automation_editor_ui/menu/load_density_menu/__init__.py
+-rw-rw-rw-   0        0        0     4179 2023-05-22 01:10:45.000000 automation_editor_dev-0.0.8/automation_editor/automation_editor_ui/menu/load_density_menu/build_load_density_menu.py
+drwxrwxrwx   0        0        0        0 2023-05-22 09:27:43.923862 automation_editor_dev-0.0.8/automation_editor/automation_editor_ui/menu/web_runner_menu/
+-rw-rw-rw-   0        0        0        0 2023-05-02 01:28:19.000000 automation_editor_dev-0.0.8/automation_editor/automation_editor_ui/menu/web_runner_menu/__init__.py
+-rw-rw-rw-   0        0        0     4056 2023-05-22 01:10:45.000000 automation_editor_dev-0.0.8/automation_editor/automation_editor_ui/menu/web_runner_menu/build_webrunner_menu.py
+drwxrwxrwx   0        0        0        0 2023-05-22 09:27:43.931263 automation_editor_dev-0.0.8/automation_editor/automation_editor_ui/show_code_window/
+-rw-rw-rw-   0        0        0        0 2023-05-02 01:28:19.000000 automation_editor_dev-0.0.8/automation_editor/automation_editor_ui/show_code_window/__init__.py
+-rw-rw-rw-   0        0        0      791 2023-05-02 01:28:19.000000 automation_editor_dev-0.0.8/automation_editor/automation_editor_ui/show_code_window/code_window.py
+drwxrwxrwx   0        0        0        0 2023-05-22 09:27:43.942280 automation_editor_dev-0.0.8/automation_editor/automation_editor_ui/syntax/
+-rw-rw-rw-   0        0        0        0 2023-05-02 01:28:19.000000 automation_editor_dev-0.0.8/automation_editor/automation_editor_ui/syntax/__init__.py
+-rw-rw-rw-   0        0        0      785 2023-05-22 01:10:45.000000 automation_editor_dev-0.0.8/automation_editor/automation_editor_ui/syntax/syntax_extend.py
+-rw-rw-rw-   0        0        0     3257 2023-05-19 03:00:53.000000 automation_editor_dev-0.0.8/automation_editor/automation_editor_ui/syntax/syntax_keyword.py
+drwxrwxrwx   0        0        0        0 2023-05-22 09:27:43.946289 automation_editor_dev-0.0.8/automation_editor/extend/
+-rw-rw-rw-   0        0        0        0 2023-05-02 01:28:19.000000 automation_editor_dev-0.0.8/automation_editor/extend/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-22 09:27:43.952828 automation_editor_dev-0.0.8/automation_editor/extend/mail_thunder_extend/
+-rw-rw-rw-   0        0        0        0 2023-05-02 01:28:19.000000 automation_editor_dev-0.0.8/automation_editor/extend/mail_thunder_extend/__init__.py
+-rw-rw-rw-   0        0        0     1704 2023-05-22 01:10:45.000000 automation_editor_dev-0.0.8/automation_editor/extend/mail_thunder_extend/mail_thunder_setting.py
+drwxrwxrwx   0        0        0        0 2023-05-22 09:27:43.956022 automation_editor_dev-0.0.8/automation_editor/utils/
+-rw-rw-rw-   0        0        0        0 2023-05-02 01:28:19.000000 automation_editor_dev-0.0.8/automation_editor/utils/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-22 09:27:43.968093 automation_editor_dev-0.0.8/automation_editor/utils/exception/
+-rw-rw-rw-   0        0        0        0 2023-05-02 01:28:19.000000 automation_editor_dev-0.0.8/automation_editor/utils/exception/__init__.py
+-rw-rw-rw-   0        0        0     1513 2023-05-19 03:12:11.000000 automation_editor_dev-0.0.8/automation_editor/utils/exception/exception_tags.py
+-rw-rw-rw-   0        0        0      608 2023-05-02 01:28:19.000000 automation_editor_dev-0.0.8/automation_editor/utils/exception/exceptions.py
+drwxrwxrwx   0        0        0        0 2023-05-22 09:27:43.974096 automation_editor_dev-0.0.8/automation_editor/utils/file_process/
+-rw-rw-rw-   0        0        0        0 2023-05-02 01:28:19.000000 automation_editor_dev-0.0.8/automation_editor/utils/file_process/__init__.py
+-rw-rw-rw-   0        0        0     1171 2023-05-02 09:53:50.000000 automation_editor_dev-0.0.8/automation_editor/utils/file_process/get_dir_file_list.py
+drwxrwxrwx   0        0        0        0 2023-05-22 09:27:43.983027 automation_editor_dev-0.0.8/automation_editor/utils/json_format/
+-rw-rw-rw-   0        0        0        2 2023-05-02 01:28:19.000000 automation_editor_dev-0.0.8/automation_editor/utils/json_format/__init__.py
+-rw-rw-rw-   0        0        0     1005 2023-05-22 01:10:45.000000 automation_editor_dev-0.0.8/automation_editor/utils/json_format/json_process.py
+drwxrwxrwx   0        0        0        0 2023-05-22 09:27:43.986052 automation_editor_dev-0.0.8/automation_editor/utils/manager/
+-rw-rw-rw-   0        0        0        0 2023-05-02 01:28:19.000000 automation_editor_dev-0.0.8/automation_editor/utils/manager/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-22 09:27:43.992581 automation_editor_dev-0.0.8/automation_editor/utils/manager/package_manager/
+-rw-rw-rw-   0        0        0        0 2023-05-02 01:28:19.000000 automation_editor_dev-0.0.8/automation_editor/utils/manager/package_manager/__init__.py
+-rw-rw-rw-   0        0        0      558 2023-05-03 02:11:15.000000 automation_editor_dev-0.0.8/automation_editor/utils/manager/package_manager/package_manager_class.py
+drwxrwxrwx   0        0        0        0 2023-05-22 09:27:44.003096 automation_editor_dev-0.0.8/automation_editor/utils/test_executor/
+-rw-rw-rw-   0        0        0        0 2023-05-02 01:28:19.000000 automation_editor_dev-0.0.8/automation_editor/utils/test_executor/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-22 09:27:44.010002 automation_editor_dev-0.0.8/automation_editor/utils/test_executor/api_testka/
+-rw-rw-rw-   0        0        0        0 2023-05-02 01:28:19.000000 automation_editor_dev-0.0.8/automation_editor/utils/test_executor/api_testka/__init__.py
+-rw-rw-rw-   0        0        0     3935 2023-05-02 01:28:19.000000 automation_editor_dev-0.0.8/automation_editor/utils/test_executor/api_testka/api_testka_process.py
+drwxrwxrwx   0        0        0        0 2023-05-22 09:27:44.017038 automation_editor_dev-0.0.8/automation_editor/utils/test_executor/auto_control/
+-rw-rw-rw-   0        0        0        0 2023-05-02 01:28:19.000000 automation_editor_dev-0.0.8/automation_editor/utils/test_executor/auto_control/__init__.py
+-rw-rw-rw-   0        0        0     3939 2023-05-02 01:28:19.000000 automation_editor_dev-0.0.8/automation_editor/utils/test_executor/auto_control/auto_control_process.py
+-rw-rw-rw-   0        0        0      498 2023-05-02 01:28:19.000000 automation_editor_dev-0.0.8/automation_editor/utils/test_executor/check_mail_thunder.py
+drwxrwxrwx   0        0        0        0 2023-05-22 09:27:44.025216 automation_editor_dev-0.0.8/automation_editor/utils/test_executor/load_density/
+-rw-rw-rw-   0        0        0        0 2023-05-02 01:28:19.000000 automation_editor_dev-0.0.8/automation_editor/utils/test_executor/load_density/__init__.py
+-rw-rw-rw-   0        0        0     3949 2023-05-02 01:28:19.000000 automation_editor_dev-0.0.8/automation_editor/utils/test_executor/load_density/load_density_process.py
+-rw-rw-rw-   0        0        0     7109 2023-05-03 08:50:31.000000 automation_editor_dev-0.0.8/automation_editor/utils/test_executor/task_process_manager.py
+drwxrwxrwx   0        0        0        0 2023-05-22 09:27:44.033421 automation_editor_dev-0.0.8/automation_editor/utils/test_executor/web_runner/
+-rw-rw-rw-   0        0        0        0 2023-05-02 01:28:19.000000 automation_editor_dev-0.0.8/automation_editor/utils/test_executor/web_runner/__init__.py
+-rw-rw-rw-   0        0        0     3897 2023-05-02 01:28:19.000000 automation_editor_dev-0.0.8/automation_editor/utils/test_executor/web_runner/web_runner_process.py
+drwxrwxrwx   0        0        0        0 2023-05-22 09:27:44.070373 automation_editor_dev-0.0.8/automation_editor_dev.egg-info/
+-rw-rw-rw-   0        0        0     5889 2023-05-22 09:27:43.000000 automation_editor_dev-0.0.8/automation_editor_dev.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     3099 2023-05-22 09:27:43.000000 automation_editor_dev-0.0.8/automation_editor_dev.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-22 09:27:43.000000 automation_editor_dev-0.0.8/automation_editor_dev.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      104 2023-05-22 09:27:43.000000 automation_editor_dev-0.0.8/automation_editor_dev.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       18 2023-05-22 09:27:43.000000 automation_editor_dev-0.0.8/automation_editor_dev.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     1272 2023-05-22 09:27:28.000000 automation_editor_dev-0.0.8/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-05-22 09:27:44.075374 automation_editor_dev-0.0.8/setup.cfg
```

### Comparing `automation_editor_dev-0.0.7/LICENSE` & `automation_editor_dev-0.0.8/LICENSE`

 * *Files identical despite different names*

### Comparing `automation_editor_dev-0.0.7/PKG-INFO` & `automation_editor_dev-0.0.8/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: automation_editor_dev
-Version: 0.0.7
+Version: 0.0.8
 Summary: Automation Editor for GUI, WEB, API, Load Automation
 Author-email: JE-Chen <jechenmailman@gmail.com>
 License: MIT
 Project-URL: Homepage, https://github.com/Intergration-Automation-Testing/AutomationEditor
 Project-URL: Code, https://github.com/Intergration-Automation-Testing/AutomationEditor
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Development Status :: 2 - Pre-Alpha
```

### Comparing `automation_editor_dev-0.0.7/README.md` & `automation_editor_dev-0.0.8/README.md`

 * *Files identical despite different names*

### Comparing `automation_editor_dev-0.0.7/automation_editor/automation_editor_ui/menu/api_testka_menu/build_api_testka_menu.py` & `automation_editor_dev-0.0.8/automation_editor/automation_editor_ui/menu/api_testka_menu/build_api_testka_menu.py`

 * *Files 0% similar despite different names*

```diff
@@ -79,16 +79,16 @@
         create_project
     )
     ui_we_want_to_set.apitestka_project_menu.addAction(
         ui_we_want_to_set.create_apitestka_project_action
     )
 
 
-def open_web_browser(url: str):
+def open_web_browser(url: str) -> None:
     webbrowser.open(url=url)
 
 
-def create_project():
+def create_project() -> None:
     package = package_manager.installed_package_dict.get("je_api_testka", None)
     if package is not None:
         package.create_project_dir()
```

### Comparing `automation_editor_dev-0.0.7/automation_editor/automation_editor_ui/menu/auto_control_menu/build_autocontrol_menu.py` & `automation_editor_dev-0.0.8/automation_editor/automation_editor_ui/menu/auto_control_menu/build_autocontrol_menu.py`

 * *Files 1% similar despite different names*

```diff
@@ -80,16 +80,16 @@
         create_project
     )
     ui_we_want_to_set.autocontrol_project_menu.addAction(
         ui_we_want_to_set.create_autocontrol_project_action
     )
 
 
-def open_web_browser(url: str):
+def open_web_browser(url: str) -> None:
     webbrowser.open(url=url)
 
 
-def create_project():
+def create_project() -> None:
     package = package_manager.installed_package_dict.get("je_auto_control", None)
     if package is not None:
         package.create_project_dir()
```

### Comparing `automation_editor_dev-0.0.7/automation_editor/automation_editor_ui/menu/install_menu/build_install_menu.py` & `automation_editor_dev-0.0.8/automation_editor/automation_editor_ui/menu/install_menu/build_install_menu.py`

 * *Files 12% similar despite different names*

```diff
@@ -37,15 +37,15 @@
     ui_we_want_to_set.install_web_runner_action = QAction("Install WebRunner")
     ui_we_want_to_set.install_web_runner_action.triggered.connect(
         lambda: install_web_runner(ui_we_want_to_set)
     )
     ui_we_want_to_set.install_menu.addAction(ui_we_want_to_set.install_web_runner_action)
 
 
-def install_package(package_text: str, ui_we_want_to_set: QMainWindow):
+def install_package(package_text: str, ui_we_want_to_set: QMainWindow) -> None:
     if sys.platform in ["win32", "cygwin", "msys"]:
         venv_path = Path(os.getcwd() + "/venv/Scripts")
     else:
         venv_path = Path(os.getcwd() + "/venv/bin")
     if venv_path.is_dir() and venv_path.exists():
         compiler_path = shutil.which(
             cmd="python3",
@@ -62,27 +62,27 @@
         compiler_path = shutil.which(cmd="python")
     shell_manager = ShellManager()
     shell_manager.main_window = ui_we_want_to_set
     shell_manager.later_init()
     shell_manager.exec_shell([f"{compiler_path}", "-m", "pip", "install", f"{package_text}"])
 
 
-def install_build_tools(ui_we_want_to_set: QMainWindow):
+def install_build_tools(ui_we_want_to_set: QMainWindow) -> None:
     install_package("setuptools", ui_we_want_to_set)
     install_package("build", ui_we_want_to_set)
     install_package("wheel", ui_we_want_to_set)
 
 
-def install_autocontrol(ui_we_want_to_set: QMainWindow):
+def install_autocontrol(ui_we_want_to_set: QMainWindow) -> None:
     install_package("je_auto_control", ui_we_want_to_set)
 
 
-def install_api_testka(ui_we_want_to_set: QMainWindow):
+def install_api_testka(ui_we_want_to_set: QMainWindow) -> None:
     install_package("je_api_testka", ui_we_want_to_set)
 
 
-def install_load_density(ui_we_want_to_set: QMainWindow):
+def install_load_density(ui_we_want_to_set: QMainWindow) -> None:
     install_package("je_load_density", ui_we_want_to_set)
 
 
-def install_web_runner(ui_we_want_to_set: QMainWindow):
+def install_web_runner(ui_we_want_to_set: QMainWindow) -> None:
     install_package("je_web_runner", ui_we_want_to_set)
```

### Comparing `automation_editor_dev-0.0.7/automation_editor/automation_editor_ui/menu/load_density_menu/build_load_density_menu.py` & `automation_editor_dev-0.0.8/automation_editor/automation_editor_ui/menu/load_density_menu/build_load_density_menu.py`

 * *Files 4% similar despite different names*

```diff
@@ -80,15 +80,15 @@
         create_project
     )
     ui_we_want_to_set.load_density_project_menu.addAction(
         ui_we_want_to_set.create_load_density_project_action
     )
 
 
-def open_web_browser(url: str):
+def open_web_browser(url: str) -> None:
     webbrowser.open(url=url)
 
 
-def create_project():
+def create_project() -> None:
     package = package_manager.installed_package_dict.get("je_load_density", None)
     if package is not None:
         package.create_project_dir()
```

### Comparing `automation_editor_dev-0.0.7/automation_editor/automation_editor_ui/menu/web_runner_menu/build_webrunner_menu.py` & `automation_editor_dev-0.0.8/automation_editor/automation_editor_ui/menu/web_runner_menu/build_webrunner_menu.py`

 * *Files 2% similar despite different names*

```diff
@@ -79,15 +79,15 @@
         create_project
     )
     ui_we_want_to_set.web_runner_project_menu.addAction(
         ui_we_want_to_set.create_web_runner_project_action
     )
 
 
-def open_web_browser(url: str):
+def open_web_browser(url: str) -> None:
     webbrowser.open(url=url)
 
 
-def create_project():
+def create_project() -> None:
     package = package_manager.installed_package_dict.get("je_web_runner", None)
     if package is not None:
         package.create_project_dir()
```

### Comparing `automation_editor_dev-0.0.7/automation_editor/automation_editor_ui/show_code_window/code_window.py` & `automation_editor_dev-0.0.8/automation_editor/automation_editor_ui/show_code_window/code_window.py`

 * *Files identical despite different names*

### Comparing `automation_editor_dev-0.0.7/automation_editor/automation_editor_ui/syntax/syntax_extend.py` & `automation_editor_dev-0.0.8/automation_editor/automation_editor_ui/syntax/syntax_extend.py`

 * *Files 15% similar despite different names*

```diff
@@ -3,14 +3,14 @@
 from PySide6.QtWidgets import QMainWindow
 
 from automation_editor.automation_editor_ui.syntax.syntax_keyword import \
     package_keyword_list
 from automation_editor.utils.manager.package_manager.package_manager_class import package_manager
 
 
-def syntax_extend_package(main_window: QMainWindow):
+def syntax_extend_package(main_window: QMainWindow) -> None:
     for package in package_manager.syntax_check_list:
         text_char_format = QTextCharFormat()
         text_char_format.setForeground(QColor(255, 255, 0))
         for word in package_keyword_list.get(package):
             pattern = QRegularExpression(rf"\b{word}\b")
             main_window.code_edit.highlighter.highlight_rules.append((pattern, text_char_format))
```

### Comparing `automation_editor_dev-0.0.7/automation_editor/extend/mail_thunder_extend/mail_thunder_setting.py` & `automation_editor_dev-0.0.8/automation_editor/extend/mail_thunder_extend/mail_thunder_setting.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import sys
 from email.mime.multipart import MIMEMultipart
 
 from automation_editor.utils.exception.exception_tags import send_html_exception_tag
 from automation_editor.utils.exception.exceptions import ITESendHtmlReportException
 
 
-def send_after_test(html_report_path: str = None):
+def send_after_test(html_report_path: str = None) -> None:
     try:
         from je_mail_thunder import SMTPWrapper
         mail_thunder_smtp: SMTPWrapper = SMTPWrapper()
         if html_report_path is None and mail_thunder_smtp.login_state is True:
             user: str = mail_thunder_smtp.user
             with open("default_name.html", "r+") as file:
                 html_string: str = file.read()
```

### Comparing `automation_editor_dev-0.0.7/automation_editor/utils/exception/exception_tags.py` & `automation_editor_dev-0.0.8/automation_editor/utils/exception/exception_tags.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # add command exception
 add_command_type_exception_tag: str = "command execute_return_value type should be as method or function"
 add_command_not_allow_package_exception_tag: str = "choose to add command package not allow"
 # send html report exception
 send_html_exception_tag: str = """
 make sure you have installed je_mail_thunder \n
-can't send html report check login user and password is correct \n
+can"t send html report check login user and password is correct \n
 and current working folder have default_name.html (html report default execute_detail) \n
 or you should get the function file_path to read
 """
 # test executor exception
 auto_control_test_executor_exception_tag: str = "can't run AutoControl"
 api_testka_test_executor_exception_tag: str = "can't run APITestka"
 web_runner_test_executor_exception_tag: str = "can't run WebRunner"
```

### Comparing `automation_editor_dev-0.0.7/automation_editor/utils/exception/exceptions.py` & `automation_editor_dev-0.0.8/automation_editor/utils/exception/exceptions.py`

 * *Files identical despite different names*

### Comparing `automation_editor_dev-0.0.7/automation_editor/utils/file_process/get_dir_file_list.py` & `automation_editor_dev-0.0.8/automation_editor/utils/file_process/get_dir_file_list.py`

 * *Files identical despite different names*

### Comparing `automation_editor_dev-0.0.7/automation_editor/utils/json_format/json_process.py` & `automation_editor_dev-0.0.8/automation_editor/utils/json_format/json_process.py`

 * *Files 3% similar despite different names*

```diff
@@ -4,25 +4,25 @@
 from json import loads
 
 from automation_editor.utils.exception.exception_tags import cant_reformat_json_error
 from automation_editor.utils.exception.exception_tags import wrong_json_data_error
 from automation_editor.utils.exception.exceptions import ITEJsonException
 
 
-def __process_json(json_string: str, **kwargs):
+def __process_json(json_string: str, **kwargs) -> str:
     try:
         return dumps(loads(json_string), indent=4, sort_keys=True, **kwargs)
     except json.JSONDecodeError as error:
         print(wrong_json_data_error, file=sys.stderr)
         raise error
     except TypeError:
         try:
             return dumps(json_string, indent=4, sort_keys=True, **kwargs)
         except TypeError:
             raise ITEJsonException(wrong_json_data_error)
 
 
-def reformat_json(json_string: str, **kwargs):
+def reformat_json(json_string: str, **kwargs) -> str:
     try:
         return __process_json(json_string, **kwargs)
     except ITEJsonException:
         raise ITEJsonException(cant_reformat_json_error)
```

### Comparing `automation_editor_dev-0.0.7/automation_editor/utils/manager/package_manager/package_manager_class.py` & `automation_editor_dev-0.0.8/automation_editor/utils/manager/package_manager/package_manager_class.py`

 * *Files identical despite different names*

### Comparing `automation_editor_dev-0.0.7/automation_editor/utils/test_executor/api_testka/api_testka_process.py` & `automation_editor_dev-0.0.8/automation_editor/utils/test_executor/api_testka/api_testka_process.py`

 * *Files identical despite different names*

### Comparing `automation_editor_dev-0.0.7/automation_editor/utils/test_executor/auto_control/auto_control_process.py` & `automation_editor_dev-0.0.8/automation_editor/utils/test_executor/auto_control/auto_control_process.py`

 * *Files identical despite different names*

### Comparing `automation_editor_dev-0.0.7/automation_editor/utils/test_executor/load_density/load_density_process.py` & `automation_editor_dev-0.0.8/automation_editor/utils/test_executor/load_density/load_density_process.py`

 * *Files identical despite different names*

### Comparing `automation_editor_dev-0.0.7/automation_editor/utils/test_executor/task_process_manager.py` & `automation_editor_dev-0.0.8/automation_editor/utils/test_executor/task_process_manager.py`

 * *Files identical despite different names*

### Comparing `automation_editor_dev-0.0.7/automation_editor/utils/test_executor/web_runner/web_runner_process.py` & `automation_editor_dev-0.0.8/automation_editor/utils/test_executor/web_runner/web_runner_process.py`

 * *Files identical despite different names*

### Comparing `automation_editor_dev-0.0.7/automation_editor_dev.egg-info/PKG-INFO` & `automation_editor_dev-0.0.8/automation_editor_dev.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: automation-editor-dev
-Version: 0.0.7
+Version: 0.0.8
 Summary: Automation Editor for GUI, WEB, API, Load Automation
 Author-email: JE-Chen <jechenmailman@gmail.com>
 License: MIT
 Project-URL: Homepage, https://github.com/Intergration-Automation-Testing/AutomationEditor
 Project-URL: Code, https://github.com/Intergration-Automation-Testing/AutomationEditor
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Development Status :: 2 - Pre-Alpha
```

### Comparing `automation_editor_dev-0.0.7/automation_editor_dev.egg-info/SOURCES.txt` & `automation_editor_dev-0.0.8/automation_editor_dev.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `automation_editor_dev-0.0.7/pyproject.toml` & `automation_editor_dev-0.0.8/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 # This is dev version
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "automation_editor_dev"
-version = "0.0.7"
+version = "0.0.8"
 authors = [
     { name = "JE-Chen", email = "jechenmailman@gmail.com" },
 ]
 description = "Automation Editor for GUI, WEB, API, Load Automation"
 requires-python = ">=3.8"
 license = { text = "MIT" }
 dependencies = [
```

