# Comparing `tmp/hexabyte-0.6.0rc0.tar.gz` & `tmp/hexabyte-0.7.0rc0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hexabyte-0.6.0rc0.tar", max compression
+gzip compressed data, was "hexabyte-0.7.0rc0.tar", max compression
```

## Comparing `hexabyte-0.6.0rc0.tar` & `hexabyte-0.7.0rc0.tar`

### file list

```diff
@@ -1,75 +1,66 @@
--rw-r--r--   0        0        0    35149 2023-05-14 03:28:29.577420 hexabyte-0.6.0rc0/LICENSE
--rw-r--r--   0        0        0      784 2023-05-14 03:28:29.577420 hexabyte-0.6.0rc0/docs/README.md
--rw-r--r--   0        0        0       93 2023-05-14 03:28:29.577420 hexabyte-0.6.0rc0/hexabyte/__init__.py
--rw-r--r--   0        0        0     2318 2023-05-14 03:28:29.577420 hexabyte-0.6.0rc0/hexabyte/__main__.py
--rw-r--r--   0        0        0      246 2023-05-14 03:28:29.577420 hexabyte-0.6.0rc0/hexabyte/actions/__init__.py
--rw-r--r--   0        0        0     2027 2023-05-14 03:28:29.577420 hexabyte-0.6.0rc0/hexabyte/actions/_action.py
--rw-r--r--   0        0        0     1516 2023-05-14 03:28:29.577420 hexabyte-0.6.0rc0/hexabyte/actions/action_handler.py
--rw-r--r--   0        0        0      970 2023-05-14 03:28:29.577420 hexabyte-0.6.0rc0/hexabyte/actions/api/__init__.py
--rw-r--r--   0        0        0      550 2023-05-14 03:28:29.577420 hexabyte-0.6.0rc0/hexabyte/actions/api/_api_action.py
--rw-r--r--   0        0        0     1857 2023-05-14 03:28:29.577420 hexabyte-0.6.0rc0/hexabyte/actions/api/clear.py
--rw-r--r--   0        0        0     2441 2023-05-14 03:28:29.577420 hexabyte-0.6.0rc0/hexabyte/actions/api/delete.py
--rw-r--r--   0        0        0     4084 2023-05-14 03:28:29.577420 hexabyte-0.6.0rc0/hexabyte/actions/api/find.py
--rw-r--r--   0        0        0     2125 2023-05-14 03:28:29.577420 hexabyte-0.6.0rc0/hexabyte/actions/api/goto.py
--rw-r--r--   0        0        0     1473 2023-05-14 03:28:29.577420 hexabyte-0.6.0rc0/hexabyte/actions/api/highlight.py
--rw-r--r--   0        0        0     1988 2023-05-14 03:28:29.577420 hexabyte-0.6.0rc0/hexabyte/actions/api/insert.py
--rw-r--r--   0        0        0     2619 2023-05-14 03:28:29.577420 hexabyte-0.6.0rc0/hexabyte/actions/api/move.py
--rw-r--r--   0        0        0     1343 2023-05-14 03:28:29.577420 hexabyte-0.6.0rc0/hexabyte/actions/api/open.py
--rw-r--r--   0        0        0     1306 2023-05-14 03:28:29.577420 hexabyte-0.6.0rc0/hexabyte/actions/api/redo.py
--rw-r--r--   0        0        0     5288 2023-05-14 03:28:29.577420 hexabyte-0.6.0rc0/hexabyte/actions/api/replace.py
--rw-r--r--   0        0        0      851 2023-05-14 03:28:29.577420 hexabyte-0.6.0rc0/hexabyte/actions/api/revert.py
--rw-r--r--   0        0        0      782 2023-05-14 03:28:29.577420 hexabyte-0.6.0rc0/hexabyte/actions/api/save.py
--rw-r--r--   0        0        0      992 2023-05-14 03:28:29.577420 hexabyte-0.6.0rc0/hexabyte/actions/api/save_as.py
--rw-r--r--   0        0        0     1449 2023-05-14 03:28:29.577420 hexabyte-0.6.0rc0/hexabyte/actions/api/select.py
--rw-r--r--   0        0        0     5363 2023-05-14 03:28:29.577420 hexabyte-0.6.0rc0/hexabyte/actions/api/set.py
--rw-r--r--   0        0        0     1307 2023-05-14 03:28:29.577420 hexabyte-0.6.0rc0/hexabyte/actions/api/undo.py
--rw-r--r--   0        0        0     1465 2023-05-14 03:28:29.577420 hexabyte-0.6.0rc0/hexabyte/actions/api/unhighlight.py
--rw-r--r--   0        0        0       69 2023-05-14 03:28:29.577420 hexabyte-0.6.0rc0/hexabyte/actions/app/__init__.py
--rw-r--r--   0        0        0      544 2023-05-14 03:28:29.577420 hexabyte-0.6.0rc0/hexabyte/actions/app/_app_action.py
--rw-r--r--   0        0        0     1161 2023-05-14 03:28:29.577420 hexabyte-0.6.0rc0/hexabyte/actions/app/exit.py
--rw-r--r--   0        0        0       30 2023-05-14 03:28:29.577420 hexabyte-0.6.0rc0/hexabyte/actions/command_prompt/__init__.py
--rw-r--r--   0        0        0     5954 2023-05-14 03:28:29.577420 hexabyte-0.6.0rc0/hexabyte/api.py
--rw-r--r--   0        0        0       28 2023-05-14 03:28:29.577420 hexabyte-0.6.0rc0/hexabyte/assets/__init__.py
--rw-r--r--   0        0        0     1004 2023-05-14 03:28:29.577420 hexabyte-0.6.0rc0/hexabyte/assets/config.toml
--rw-r--r--   0        0        0      306 2023-05-14 03:28:29.577420 hexabyte-0.6.0rc0/hexabyte/commands/__init__.py
--rw-r--r--   0        0        0      445 2023-05-14 03:28:29.577420 hexabyte-0.6.0rc0/hexabyte/commands/command.py
--rw-r--r--   0        0        0     3371 2023-05-14 03:28:29.577420 hexabyte-0.6.0rc0/hexabyte/commands/command_parser.py
--rw-r--r--   0        0        0      883 2023-05-14 03:28:29.581420 hexabyte-0.6.0rc0/hexabyte/commands/decorators.py
--rw-r--r--   0        0        0      106 2023-05-14 03:28:29.581420 hexabyte-0.6.0rc0/hexabyte/constants/__init__.py
--rw-r--r--   0        0        0      379 2023-05-14 03:28:29.581420 hexabyte-0.6.0rc0/hexabyte/constants/enums.py
--rw-r--r--   0        0        0      247 2023-05-14 03:28:29.581420 hexabyte-0.6.0rc0/hexabyte/constants/generic.py
--rw-r--r--   0        0        0     1298 2023-05-14 03:28:29.581420 hexabyte-0.6.0rc0/hexabyte/constants/sizes.py
--rw-r--r--   0        0        0      176 2023-05-14 03:28:29.581420 hexabyte-0.6.0rc0/hexabyte/data_sources/__init__.py
--rw-r--r--   0        0        0     2217 2023-05-14 03:28:29.581420 hexabyte-0.6.0rc0/hexabyte/data_sources/_data_source.py
--rw-r--r--   0        0        0      477 2023-05-14 03:28:29.581420 hexabyte-0.6.0rc0/hexabyte/data_sources/data_block.py
--rw-r--r--   0        0        0     5075 2023-05-14 03:28:29.581420 hexabyte-0.6.0rc0/hexabyte/data_sources/paged_data_source.py
--rw-r--r--   0        0        0     2442 2023-05-14 03:28:29.581420 hexabyte-0.6.0rc0/hexabyte/data_sources/simple_data_source.py
--rw-r--r--   0        0        0      282 2023-05-14 03:28:29.581420 hexabyte-0.6.0rc0/hexabyte/hexabyte_app.css
--rw-r--r--   0        0        0     5012 2023-05-14 03:28:29.581420 hexabyte-0.6.0rc0/hexabyte/hexabyte_app.py
--rw-r--r--   0        0        0      424 2023-05-14 03:28:29.581420 hexabyte-0.6.0rc0/hexabyte/plugins/__init__.py
--rw-r--r--   0        0        0     1203 2023-05-14 03:28:29.581420 hexabyte-0.6.0rc0/hexabyte/plugins/_loader.py
--rw-r--r--   0        0        0      166 2023-05-14 03:28:29.581420 hexabyte-0.6.0rc0/hexabyte/plugins/entropy/__init__.py
--rw-r--r--   0        0        0     3001 2023-05-14 03:28:29.581420 hexabyte-0.6.0rc0/hexabyte/plugins/entropy/entropy.py
--rw-r--r--   0        0        0       38 2023-05-14 03:28:29.581420 hexabyte-0.6.0rc0/hexabyte/plugins/entropy/widgets/__init__.py
--rw-r--r--   0        0        0     3289 2023-05-14 03:28:29.581420 hexabyte-0.6.0rc0/hexabyte/plugins/entropy/widgets/entropy_panel.py
--rw-r--r--   0        0        0      147 2023-05-14 03:28:29.581420 hexabyte-0.6.0rc0/hexabyte/plugins/info/__init__.py
--rw-r--r--   0        0        0       40 2023-05-14 03:28:29.581420 hexabyte-0.6.0rc0/hexabyte/plugins/info/widgets/__init__.py
--rw-r--r--   0        0        0     3894 2023-05-14 03:28:29.581420 hexabyte-0.6.0rc0/hexabyte/plugins/info/widgets/info_panel.py
--rw-r--r--   0        0        0      143 2023-05-14 03:28:29.581420 hexabyte-0.6.0rc0/hexabyte/utils/__init__.py
--rw-r--r--   0        0        0     3174 2023-05-14 03:28:29.581420 hexabyte-0.6.0rc0/hexabyte/utils/config.py
--rw-r--r--   0        0        0      558 2023-05-14 03:28:29.581420 hexabyte-0.6.0rc0/hexabyte/utils/context.py
--rw-r--r--   0        0        0     4611 2023-05-14 03:28:29.581420 hexabyte-0.6.0rc0/hexabyte/utils/cursor.py
--rw-r--r--   0        0        0     3404 2023-05-14 03:28:29.581420 hexabyte-0.6.0rc0/hexabyte/utils/data_types.py
--rw-r--r--   0        0        0     2034 2023-05-14 03:28:29.581420 hexabyte-0.6.0rc0/hexabyte/utils/misc.py
--rw-r--r--   0        0        0      137 2023-05-14 03:28:29.581420 hexabyte-0.6.0rc0/hexabyte/view_components/__init__.py
--rw-r--r--   0        0        0    14267 2023-05-14 03:28:29.581420 hexabyte-0.6.0rc0/hexabyte/view_components/byte_view.py
--rw-r--r--   0        0        0     5885 2023-05-14 03:28:29.581420 hexabyte-0.6.0rc0/hexabyte/view_components/hc_view.py
--rw-r--r--   0        0        0      288 2023-05-14 03:28:29.581420 hexabyte-0.6.0rc0/hexabyte/widgets/__init__.py
--rw-r--r--   0        0        0     4328 2023-05-14 03:28:29.581420 hexabyte-0.6.0rc0/hexabyte/widgets/command_prompt.py
--rw-r--r--   0        0        0    16210 2023-05-14 03:28:29.581420 hexabyte-0.6.0rc0/hexabyte/widgets/editor.py
--rw-r--r--   0        0        0     5965 2023-05-14 03:28:29.581420 hexabyte-0.6.0rc0/hexabyte/widgets/help_screen.py
--rw-r--r--   0        0        0     1588 2023-05-14 03:28:29.581420 hexabyte-0.6.0rc0/hexabyte/widgets/sidebar.py
--rw-r--r--   0        0        0     1043 2023-05-14 03:28:29.581420 hexabyte-0.6.0rc0/hexabyte/widgets/sidebar_panel.py
--rw-r--r--   0        0        0     4088 2023-05-14 03:28:29.581420 hexabyte-0.6.0rc0/hexabyte/widgets/workbench.py
--rw-r--r--   0        0        0     8358 2023-05-14 03:28:29.637421 hexabyte-0.6.0rc0/pyproject.toml
--rw-r--r--   0        0        0     2391 1970-01-01 00:00:00.000000 hexabyte-0.6.0rc0/PKG-INFO
+-rw-r--r--   0        0        0    35149 2023-05-24 02:10:08.294147 hexabyte-0.7.0rc0/LICENSE
+-rw-r--r--   0        0        0      784 2023-05-24 02:10:08.294147 hexabyte-0.7.0rc0/docs/README.md
+-rw-r--r--   0        0        0       93 2023-05-24 02:10:08.294147 hexabyte-0.7.0rc0/hexabyte/__init__.py
+-rw-r--r--   0        0        0     2339 2023-05-24 02:10:08.294147 hexabyte-0.7.0rc0/hexabyte/__main__.py
+-rw-r--r--   0        0        0      246 2023-05-24 02:10:08.294147 hexabyte-0.7.0rc0/hexabyte/actions/__init__.py
+-rw-r--r--   0        0        0     2027 2023-05-24 02:10:08.294147 hexabyte-0.7.0rc0/hexabyte/actions/_action.py
+-rw-r--r--   0        0        0     1510 2023-05-24 02:10:08.294147 hexabyte-0.7.0rc0/hexabyte/actions/action_handler.py
+-rw-r--r--   0        0        0      970 2023-05-24 02:10:08.294147 hexabyte-0.7.0rc0/hexabyte/actions/api/__init__.py
+-rw-r--r--   0        0        0      550 2023-05-24 02:10:08.294147 hexabyte-0.7.0rc0/hexabyte/actions/api/_api_action.py
+-rw-r--r--   0        0        0     1835 2023-05-24 02:10:08.294147 hexabyte-0.7.0rc0/hexabyte/actions/api/clear.py
+-rw-r--r--   0        0        0     2370 2023-05-24 02:10:08.294147 hexabyte-0.7.0rc0/hexabyte/actions/api/delete.py
+-rw-r--r--   0        0        0     4019 2023-05-24 02:10:08.294147 hexabyte-0.7.0rc0/hexabyte/actions/api/find.py
+-rw-r--r--   0        0        0     2060 2023-05-24 02:10:08.294147 hexabyte-0.7.0rc0/hexabyte/actions/api/goto.py
+-rw-r--r--   0        0        0     1420 2023-05-24 02:10:08.294147 hexabyte-0.7.0rc0/hexabyte/actions/api/highlight.py
+-rw-r--r--   0        0        0     1917 2023-05-24 02:10:08.294147 hexabyte-0.7.0rc0/hexabyte/actions/api/insert.py
+-rw-r--r--   0        0        0     2548 2023-05-24 02:10:08.294147 hexabyte-0.7.0rc0/hexabyte/actions/api/move.py
+-rw-r--r--   0        0        0     1336 2023-05-24 02:10:08.294147 hexabyte-0.7.0rc0/hexabyte/actions/api/open.py
+-rw-r--r--   0        0        0     1268 2023-05-24 02:10:08.294147 hexabyte-0.7.0rc0/hexabyte/actions/api/redo.py
+-rw-r--r--   0        0        0     5217 2023-05-24 02:10:08.294147 hexabyte-0.7.0rc0/hexabyte/actions/api/replace.py
+-rw-r--r--   0        0        0      851 2023-05-24 02:10:08.294147 hexabyte-0.7.0rc0/hexabyte/actions/api/revert.py
+-rw-r--r--   0        0        0      782 2023-05-24 02:10:08.294147 hexabyte-0.7.0rc0/hexabyte/actions/api/save.py
+-rw-r--r--   0        0        0      992 2023-05-24 02:10:08.294147 hexabyte-0.7.0rc0/hexabyte/actions/api/save_as.py
+-rw-r--r--   0        0        0     1396 2023-05-24 02:10:08.294147 hexabyte-0.7.0rc0/hexabyte/actions/api/select.py
+-rw-r--r--   0        0        0     5324 2023-05-24 02:10:08.294147 hexabyte-0.7.0rc0/hexabyte/actions/api/set.py
+-rw-r--r--   0        0        0     1269 2023-05-24 02:10:08.294147 hexabyte-0.7.0rc0/hexabyte/actions/api/undo.py
+-rw-r--r--   0        0        0     1412 2023-05-24 02:10:08.294147 hexabyte-0.7.0rc0/hexabyte/actions/api/unhighlight.py
+-rw-r--r--   0        0        0       69 2023-05-24 02:10:08.298147 hexabyte-0.7.0rc0/hexabyte/actions/app/__init__.py
+-rw-r--r--   0        0        0      544 2023-05-24 02:10:08.298147 hexabyte-0.7.0rc0/hexabyte/actions/app/_app_action.py
+-rw-r--r--   0        0        0     1102 2023-05-24 02:10:08.298147 hexabyte-0.7.0rc0/hexabyte/actions/app/exit.py
+-rw-r--r--   0        0        0       30 2023-05-24 02:10:08.298147 hexabyte-0.7.0rc0/hexabyte/actions/command_prompt/__init__.py
+-rw-r--r--   0        0        0     5808 2023-05-24 02:10:08.298147 hexabyte-0.7.0rc0/hexabyte/api.py
+-rw-r--r--   0        0        0     1368 2023-05-24 02:10:08.298147 hexabyte-0.7.0rc0/hexabyte/commands/__init__.py
+-rw-r--r--   0        0        0      445 2023-05-24 02:10:08.298147 hexabyte-0.7.0rc0/hexabyte/commands/command.py
+-rw-r--r--   0        0        0     3325 2023-05-24 02:10:08.298147 hexabyte-0.7.0rc0/hexabyte/commands/command_parser.py
+-rw-r--r--   0        0        0      875 2023-05-24 02:10:08.298147 hexabyte-0.7.0rc0/hexabyte/commands/decorators.py
+-rw-r--r--   0        0        0     2770 2023-05-24 02:10:08.298147 hexabyte-0.7.0rc0/hexabyte/config.py
+-rw-r--r--   0        0        0      106 2023-05-24 02:10:08.298147 hexabyte-0.7.0rc0/hexabyte/constants/__init__.py
+-rw-r--r--   0        0        0      379 2023-05-24 02:10:08.298147 hexabyte-0.7.0rc0/hexabyte/constants/enums.py
+-rw-r--r--   0        0        0      260 2023-05-24 02:10:08.298147 hexabyte-0.7.0rc0/hexabyte/constants/generic.py
+-rw-r--r--   0        0        0     1298 2023-05-24 02:10:08.298147 hexabyte-0.7.0rc0/hexabyte/constants/sizes.py
+-rw-r--r--   0        0        0      558 2023-05-24 02:10:08.298147 hexabyte-0.7.0rc0/hexabyte/context.py
+-rw-r--r--   0        0        0     4613 2023-05-24 02:10:08.298147 hexabyte-0.7.0rc0/hexabyte/cursor.py
+-rw-r--r--   0        0        0      176 2023-05-24 02:10:08.298147 hexabyte-0.7.0rc0/hexabyte/data_sources/__init__.py
+-rw-r--r--   0        0        0     2217 2023-05-24 02:10:08.298147 hexabyte-0.7.0rc0/hexabyte/data_sources/_data_source.py
+-rw-r--r--   0        0        0      477 2023-05-24 02:10:08.298147 hexabyte-0.7.0rc0/hexabyte/data_sources/data_block.py
+-rw-r--r--   0        0        0     5047 2023-05-24 02:10:08.298147 hexabyte-0.7.0rc0/hexabyte/data_sources/paged_data_source.py
+-rw-r--r--   0        0        0     2422 2023-05-24 02:10:08.298147 hexabyte-0.7.0rc0/hexabyte/data_sources/simple_data_source.py
+-rw-r--r--   0        0        0     3404 2023-05-24 02:10:08.298147 hexabyte-0.7.0rc0/hexabyte/data_types.py
+-rw-r--r--   0        0        0      282 2023-05-24 02:10:08.298147 hexabyte-0.7.0rc0/hexabyte/hexabyte_app.css
+-rw-r--r--   0        0        0     4958 2023-05-24 02:10:08.298147 hexabyte-0.7.0rc0/hexabyte/hexabyte_app.py
+-rw-r--r--   0        0        0     1448 2023-05-24 02:10:08.298147 hexabyte-0.7.0rc0/hexabyte/plugins.py
+-rw-r--r--   0        0        0      251 2023-05-24 02:10:08.298147 hexabyte-0.7.0rc0/hexabyte/utils/__init__.py
+-rw-r--r--   0        0        0      807 2023-05-24 02:10:08.298147 hexabyte-0.7.0rc0/hexabyte/utils/data_manipulation.py
+-rw-r--r--   0        0        0      136 2023-05-24 02:10:08.298147 hexabyte-0.7.0rc0/hexabyte/view_components/__init__.py
+-rw-r--r--   0        0        0    14227 2023-05-24 02:10:08.298147 hexabyte-0.7.0rc0/hexabyte/view_components/byte_view.py
+-rw-r--r--   0        0        0     5860 2023-05-24 02:10:08.298147 hexabyte-0.7.0rc0/hexabyte/view_components/hc_view.py
+-rw-r--r--   0        0        0      288 2023-05-24 02:10:08.298147 hexabyte-0.7.0rc0/hexabyte/widgets/__init__.py
+-rw-r--r--   0        0        0     3359 2023-05-24 02:10:08.298147 hexabyte-0.7.0rc0/hexabyte/widgets/command_prompt.py
+-rw-r--r--   0        0        0    16170 2023-05-24 02:10:08.298147 hexabyte-0.7.0rc0/hexabyte/widgets/editor.py
+-rw-r--r--   0        0        0     4915 2023-05-24 02:10:08.298147 hexabyte-0.7.0rc0/hexabyte/widgets/help_screen.py
+-rw-r--r--   0        0        0     3482 2023-05-24 02:10:08.298147 hexabyte-0.7.0rc0/hexabyte/widgets/info_panel.py
+-rw-r--r--   0        0        0     1640 2023-05-24 02:10:08.298147 hexabyte-0.7.0rc0/hexabyte/widgets/sidebar.py
+-rw-r--r--   0        0        0     1043 2023-05-24 02:10:08.298147 hexabyte-0.7.0rc0/hexabyte/widgets/sidebar_panel.py
+-rw-r--r--   0        0        0     4061 2023-05-24 02:10:08.298147 hexabyte-0.7.0rc0/hexabyte/widgets/workbench.py
+-rw-r--r--   0        0        0     8183 2023-05-24 02:10:08.334147 hexabyte-0.7.0rc0/pyproject.toml
+-rw-r--r--   0        0        0     2207 1970-01-01 00:00:00.000000 hexabyte-0.7.0rc0/PKG-INFO
```

### Comparing `hexabyte-0.6.0rc0/LICENSE` & `hexabyte-0.7.0rc0/LICENSE`

 * *Files identical despite different names*

### Comparing `hexabyte-0.6.0rc0/docs/README.md` & `hexabyte-0.7.0rc0/docs/README.md`

 * *Files identical despite different names*

### Comparing `hexabyte-0.6.0rc0/hexabyte/__main__.py` & `hexabyte-0.7.0rc0/hexabyte/__main__.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,17 +1,18 @@
 """Haxabyte Package Main."""
 import argparse
 from importlib.metadata import version
 from pathlib import Path
 
+from hexabyte.config import Config
 from hexabyte.constants import FileMode
 from hexabyte.constants.generic import MAX_FILE_COUNT, MIN_FILE_COUNT
+from hexabyte.context import context
 from hexabyte.hexabyte_app import HexabyteApp
-from hexabyte.plugins._loader import load_plugins
-from hexabyte.utils import Config, context
+from hexabyte.plugins import load_plugins
 
 
 def main():
     """Start the hexabyte application."""
     parser = argparse.ArgumentParser(prog="hexabyte")
     parser.description = (
         "Hexabyte can operate in three distinct modes. "
```

### Comparing `hexabyte-0.6.0rc0/hexabyte/actions/_action.py` & `hexabyte-0.7.0rc0/hexabyte/actions/_action.py`

 * *Files identical despite different names*

### Comparing `hexabyte-0.6.0rc0/hexabyte/actions/action_handler.py` & `hexabyte-0.7.0rc0/hexabyte/actions/action_handler.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,12 +1,11 @@
 """Action Handler Module."""
 from collections import deque
 
-from hexabyte.utils import context
-
+from ..context import context
 from ._action import Action, HandlerAction, ReversibleAction
 
 
 class ActionHandler:
     """Action Handler Class.
 
     Implements action execution and Undo/Redo functionality.
```

### Comparing `hexabyte-0.6.0rc0/hexabyte/actions/api/__init__.py` & `hexabyte-0.7.0rc0/hexabyte/actions/api/__init__.py`

 * *Files identical despite different names*

### Comparing `hexabyte-0.6.0rc0/hexabyte/actions/api/_api_action.py` & `hexabyte-0.7.0rc0/hexabyte/actions/api/_api_action.py`

 * *Files identical despite different names*

### Comparing `hexabyte-0.6.0rc0/hexabyte/actions/api/clear.py` & `hexabyte-0.7.0rc0/hexabyte/actions/api/clear.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,14 +1,13 @@
 """Clear Action."""
 from __future__ import annotations
 
 from typing import TYPE_CHECKING
 
-from hexabyte.commands.command_parser import InvalidCommandError
-
+from ...commands import InvalidCommandError
 from .._action import ActionError
 from ._api_action import ApiAction
 
 if TYPE_CHECKING:
     from hexabyte.api import DataAPI
```

### Comparing `hexabyte-0.6.0rc0/hexabyte/actions/api/delete.py` & `hexabyte-0.7.0rc0/hexabyte/actions/api/delete.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,17 +1,15 @@
 """Delete Action."""
 from __future__ import annotations
 
 from typing import TYPE_CHECKING
 
-from hexabyte.commands.command_parser import InvalidCommandError
-from hexabyte.constants.sizes import BYTE_BITS
-from hexabyte.utils.cursor import Cursor
-from hexabyte.utils.misc import str_to_int
-
+from ...commands import InvalidCommandError, str_to_int
+from ...constants.sizes import BYTE_BITS
+from ...cursor import Cursor
 from .._action import ActionError, UndoError
 from ._api_action import ReversibleApiAction
 
 if TYPE_CHECKING:
     from hexabyte.api import DataAPI
```

### Comparing `hexabyte-0.6.0rc0/hexabyte/actions/api/find.py` & `hexabyte-0.7.0rc0/hexabyte/actions/api/find.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,18 +1,16 @@
 """Find Action."""
 from __future__ import annotations
 
 import struct
 from ast import literal_eval
 from typing import TYPE_CHECKING
 
-from hexabyte.commands.command_parser import InvalidCommandError
-from hexabyte.utils.context import context
-from hexabyte.utils.misc import int_fmt_str
-
+from ...commands import InvalidCommandError, int_fmt_str
+from ...context import context
 from .._action import ActionError
 from ._api_action import ApiAction
 
 if TYPE_CHECKING:
     from hexabyte.api import DataAPI
```

### Comparing `hexabyte-0.6.0rc0/hexabyte/actions/api/goto.py` & `hexabyte-0.7.0rc0/hexabyte/actions/api/goto.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,17 +1,15 @@
 """Goto Action."""
 from __future__ import annotations
 
 from typing import TYPE_CHECKING
 
-from hexabyte.commands.command_parser import InvalidCommandError
-from hexabyte.constants.enums import OffsetType
-from hexabyte.constants.sizes import BYTE_BITS
-from hexabyte.utils.misc import str_to_int
-
+from ...commands import InvalidCommandError, str_to_int
+from ...constants.enums import OffsetType
+from ...constants.sizes import BYTE_BITS
 from .._action import ActionError, UndoError
 from ._api_action import ReversibleApiAction
 
 if TYPE_CHECKING:
     from hexabyte.api import DataAPI
```

### Comparing `hexabyte-0.6.0rc0/hexabyte/actions/api/highlight.py` & `hexabyte-0.7.0rc0/hexabyte/actions/api/highlight.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,15 +1,13 @@
 """Highlight Action."""
 from __future__ import annotations
 
 from typing import TYPE_CHECKING
 
-from hexabyte.commands.command_parser import InvalidCommandError
-from hexabyte.utils.misc import str_to_int
-
+from ...commands import InvalidCommandError, str_to_int
 from .._action import ActionError
 from ._api_action import ApiAction
 
 if TYPE_CHECKING:
     from hexabyte.api import DataAPI
```

### Comparing `hexabyte-0.6.0rc0/hexabyte/actions/api/insert.py` & `hexabyte-0.7.0rc0/hexabyte/actions/api/insert.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,18 +1,16 @@
 """Insert Action."""
 from __future__ import annotations
 
 from struct import pack
 from typing import TYPE_CHECKING
 
-from hexabyte.commands.command_parser import InvalidCommandError
-from hexabyte.constants.sizes import BYTE_BITS, BYTE_MAX
-from hexabyte.utils.cursor import Cursor
-from hexabyte.utils.misc import str_to_int
-
+from ...commands import InvalidCommandError, str_to_int
+from ...constants.sizes import BYTE_BITS, BYTE_MAX
+from ...cursor import Cursor
 from .._action import ActionError, UndoError
 from ._api_action import ReversibleApiAction
 
 if TYPE_CHECKING:
     from hexabyte.api import DataAPI
```

### Comparing `hexabyte-0.6.0rc0/hexabyte/actions/api/move.py` & `hexabyte-0.7.0rc0/hexabyte/actions/api/move.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,17 +1,15 @@
 """Move Action."""
 from __future__ import annotations
 
 from typing import TYPE_CHECKING
 
-from hexabyte.commands.command_parser import InvalidCommandError
-from hexabyte.constants.sizes import BYTE_BITS
-from hexabyte.utils.cursor import Cursor
-from hexabyte.utils.misc import str_to_int
-
+from ...commands import InvalidCommandError, str_to_int
+from ...constants.sizes import BYTE_BITS
+from ...cursor import Cursor
 from .._action import ActionError, UndoError
 from ._api_action import ReversibleApiAction
 
 if TYPE_CHECKING:
     from hexabyte.api import DataAPI
```

### Comparing `hexabyte-0.6.0rc0/hexabyte/actions/api/open.py` & `hexabyte-0.7.0rc0/hexabyte/actions/app/exit.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,55 +1,45 @@
-"""Open Action."""
+"""Exit Action."""
 from __future__ import annotations
 
-from pathlib import Path
+import sys
 from typing import TYPE_CHECKING
 
-from hexabyte.commands.command_parser import InvalidCommandError
-
-from .._action import ActionError
-from ._api_action import ApiAction
+from ...commands import InvalidCommandError, str_to_int
+from ._app_action import AppAction
 
 if TYPE_CHECKING:
-    from hexabyte.api import DataAPI
-
-
-class Open(ApiAction):
-    """Open Action.
-
-    Open a new file in editor:
+    from ...hexabyte_app import HexabyteApp
 
-    open FILENAME
 
-    open new_file.txt
-    """
+class Exit(AppAction):
+    """Exit Action."""
 
-    CMD = "open"
-    MIN_ARGS = 1
+    CMD = "exit"
+    MIN_ARGS = 0
     MAX_ARGS = 1
+    status: int = 0
 
     def __init__(self, argv: tuple[str, ...]) -> None:
         """Initialize action."""
+        super().__init__(argv)
         try:
-            super().__init__(argv)
-            self.new_filepath = Path(argv[0])
-            if not self.new_filepath.exists():
-                raise FileNotFoundError()
-        except FileNotFoundError as err:
+            if self.argc == 1:
+                self.status = str_to_int(argv[0])
+        except ValueError as err:
             raise InvalidCommandError(" ".join([self.CMD, *argv])) from err
 
     @property
-    def target(self) -> DataAPI | None:
+    def target(self) -> HexabyteApp | None:
         """Get action target."""
         return self._target
 
     @target.setter
-    def target(self, target: DataAPI | None) -> None:
+    def target(self, target: HexabyteApp) -> None:
         """Set action target."""
         self._target = target
 
     def do(self) -> None:
         """Perform action."""
         if self.target is None:
-            raise ActionError("Action target not set.")
-        self.target.open(self.new_filepath)
-        self.applied = True
+            sys.exit(self.status)
+        self.target.exit()
```

### Comparing `hexabyte-0.6.0rc0/hexabyte/actions/api/redo.py` & `hexabyte-0.7.0rc0/hexabyte/actions/api/open.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,38 +1,43 @@
-"""Redo Action."""
+"""Open Action."""
 from __future__ import annotations
 
+from pathlib import Path
 from typing import TYPE_CHECKING
 
-from hexabyte.commands import InvalidCommandError
-from hexabyte.utils.misc import str_to_int
-
+from ...commands.command_parser import InvalidCommandError
 from .._action import ActionError
-from ._api_action import ApiHandlerAction
+from ._api_action import ApiAction
 
 if TYPE_CHECKING:
     from hexabyte.api import DataAPI
 
 
-class Redo(ApiHandlerAction):
-    """Redo Action."""
+class Open(ApiAction):
+    """Open Action.
+
+    Open a new file in editor:
+
+    open FILENAME
+
+    open new_file.txt
+    """
 
-    CMD = "redo"
-    MIN_ARGS = 0
+    CMD = "open"
+    MIN_ARGS = 1
     MAX_ARGS = 1
 
     def __init__(self, argv: tuple[str, ...]) -> None:
         """Initialize action."""
         try:
             super().__init__(argv)
-            if self.argc == 0:
-                self.count = 1
-            else:
-                self.count = str_to_int(argv[0])
-        except ValueError as err:
+            self.new_filepath = Path(argv[0])
+            if not self.new_filepath.exists():
+                raise FileNotFoundError()
+        except FileNotFoundError as err:
             raise InvalidCommandError(" ".join([self.CMD, *argv])) from err
 
     @property
     def target(self) -> DataAPI | None:
         """Get action target."""
         return self._target
 
@@ -41,10 +46,9 @@
         """Set action target."""
         self._target = target
 
     def do(self) -> None:
         """Perform action."""
         if self.target is None:
             raise ActionError("Action target not set.")
-        for _ in range(self.count):
-            self.target.action_handler.redo()
+        self.target.open(self.new_filepath)
         self.applied = True
```

### Comparing `hexabyte-0.6.0rc0/hexabyte/actions/api/replace.py` & `hexabyte-0.7.0rc0/hexabyte/actions/api/replace.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,19 +1,17 @@
 """Replace Action."""
 from __future__ import annotations
 
 import struct
 from ast import literal_eval
 from typing import TYPE_CHECKING
 
-from hexabyte.commands.command_parser import InvalidCommandError
-from hexabyte.constants.sizes import BYTE_BITS
-from hexabyte.utils.context import context
-from hexabyte.utils.misc import int_fmt_str
-
+from ...commands import InvalidCommandError, int_fmt_str
+from ...constants.sizes import BYTE_BITS
+from ...context import context
 from .._action import ActionError, UndoError
 from ._api_action import ReversibleApiAction
 
 if TYPE_CHECKING:
     from hexabyte.api import DataAPI
```

### Comparing `hexabyte-0.6.0rc0/hexabyte/actions/api/revert.py` & `hexabyte-0.7.0rc0/hexabyte/actions/api/revert.py`

 * *Files identical despite different names*

### Comparing `hexabyte-0.6.0rc0/hexabyte/actions/api/save.py` & `hexabyte-0.7.0rc0/hexabyte/actions/api/save.py`

 * *Files identical despite different names*

### Comparing `hexabyte-0.6.0rc0/hexabyte/actions/api/save_as.py` & `hexabyte-0.7.0rc0/hexabyte/actions/api/save_as.py`

 * *Files identical despite different names*

### Comparing `hexabyte-0.6.0rc0/hexabyte/actions/api/select.py` & `hexabyte-0.7.0rc0/hexabyte/actions/api/unhighlight.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,33 +1,30 @@
-"""Select Action."""
+"""Unhighlight Action."""
 from __future__ import annotations
 
 from typing import TYPE_CHECKING
 
-from hexabyte.commands.command_parser import InvalidCommandError
-from hexabyte.utils.misc import str_to_int
-
+from ...commands import InvalidCommandError, str_to_int
 from .._action import ActionError
 from ._api_action import ApiAction
 
 if TYPE_CHECKING:
     from hexabyte.api import DataAPI
 
 
-class Select(ApiAction):
-    """Select Action.
+class Unhighlight(ApiAction):
+    """Unhighlight Action.
 
     Supports a one arg and two arg form:
 
-    select BYTE_OFFSET [BYTE_LENGTH]
-    > select 0x100
-    > select 0x100 0x10
+    unhighlight BYTE_OFFSET [BYTE_LENGTH]
+    > unhighlight 0x100 0x10
     """
 
-    CMD = "select"
+    CMD = "unhighlight"
     MIN_ARGS = 1
     MAX_ARGS = 2
 
     def __init__(self, argv: tuple[str, ...]) -> None:
         """Initialize action."""
         try:
             super().__init__(argv)
@@ -48,9 +45,9 @@
 
     def do(self) -> None:
         """Perform action."""
         if self.target is None:
             raise ActionError("Action target not set.")
         api = self.target
         api.seek(self.offset)
-        api.select(self.length)
+        api.unhighlight(self.length)
         self.applied = True
```

### Comparing `hexabyte-0.6.0rc0/hexabyte/actions/api/set.py` & `hexabyte-0.7.0rc0/hexabyte/actions/api/set.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,19 +1,18 @@
 """Set Action."""
 from __future__ import annotations
 
 from struct import pack, unpack
 from typing import TYPE_CHECKING
 
-from hexabyte.commands.command_parser import InvalidCommandError
-from hexabyte.constants.enums import OffsetType
-from hexabyte.constants.sizes import BIT, BYTE_BITS, BYTE_MAX, NIBBLE_BITS
-from hexabyte.utils.cursor import Cursor
-from hexabyte.utils.misc import clear_bit, set_bit, set_nibble, str_to_int
-
+from ...commands import InvalidCommandError, str_to_int
+from ...constants.enums import OffsetType
+from ...constants.sizes import BIT, BYTE_BITS, BYTE_MAX, NIBBLE_BITS
+from ...cursor import Cursor
+from ...utils.data_manipulation import clear_bit, set_bit, set_nibble
 from .._action import ActionError, UndoError
 from ._api_action import ReversibleApiAction
 
 if TYPE_CHECKING:
     from hexabyte.api import DataAPI
```

### Comparing `hexabyte-0.6.0rc0/hexabyte/actions/api/undo.py` & `hexabyte-0.7.0rc0/hexabyte/actions/api/undo.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,15 +1,13 @@
 """Undo Action."""
 from __future__ import annotations
 
 from typing import TYPE_CHECKING
 
-from hexabyte.commands import InvalidCommandError
-from hexabyte.utils.misc import str_to_int
-
+from ...commands import InvalidCommandError, str_to_int
 from .._action import ActionError
 from ._api_action import ApiHandlerAction
 
 if TYPE_CHECKING:
     from hexabyte.api import DataAPI
```

### Comparing `hexabyte-0.6.0rc0/hexabyte/actions/api/unhighlight.py` & `hexabyte-0.7.0rc0/hexabyte/actions/api/select.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,32 +1,31 @@
-"""Unhighlight Action."""
+"""Select Action."""
 from __future__ import annotations
 
 from typing import TYPE_CHECKING
 
-from hexabyte.commands.command_parser import InvalidCommandError
-from hexabyte.utils.misc import str_to_int
-
+from ...commands import InvalidCommandError, str_to_int
 from .._action import ActionError
 from ._api_action import ApiAction
 
 if TYPE_CHECKING:
     from hexabyte.api import DataAPI
 
 
-class Unhighlight(ApiAction):
-    """Unhighlight Action.
+class Select(ApiAction):
+    """Select Action.
 
     Supports a one arg and two arg form:
 
-    unhighlight BYTE_OFFSET [BYTE_LENGTH]
-    > unhighlight 0x100 0x10
+    select BYTE_OFFSET [BYTE_LENGTH]
+    > select 0x100
+    > select 0x100 0x10
     """
 
-    CMD = "unhighlight"
+    CMD = "select"
     MIN_ARGS = 1
     MAX_ARGS = 2
 
     def __init__(self, argv: tuple[str, ...]) -> None:
         """Initialize action."""
         try:
             super().__init__(argv)
@@ -47,9 +46,9 @@
 
     def do(self) -> None:
         """Perform action."""
         if self.target is None:
             raise ActionError("Action target not set.")
         api = self.target
         api.seek(self.offset)
-        api.unhighlight(self.length)
+        api.select(self.length)
         self.applied = True
```

### Comparing `hexabyte-0.6.0rc0/hexabyte/actions/app/_app_action.py` & `hexabyte-0.7.0rc0/hexabyte/actions/app/_app_action.py`

 * *Files identical despite different names*

### Comparing `hexabyte-0.6.0rc0/hexabyte/api.py` & `hexabyte-0.7.0rc0/hexabyte/api.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,34 +1,32 @@
 """Hexabyte Data Api Package."""
 from pathlib import Path
 
 from rich.style import Style
 
-from hexabyte.actions import Action
-from hexabyte.actions.action_handler import ActionHandler
-from hexabyte.actions.api import API_ACTIONS
-from hexabyte.commands import register
-from hexabyte.constants.sizes import KB, MB
-from hexabyte.data_sources import SimpleDataSource
-from hexabyte.utils import context
-from hexabyte.utils.data_types import DataSegment
-
-from .utils.cursor import Cursor
+from .actions import Action
+from .actions.action_handler import ActionHandler
+from .actions.api import API_ACTIONS
+from .commands import register
+from .constants.sizes import KB, MB
+from .context import context
+from .cursor import Cursor
+from .data_sources import SimpleDataSource
+from .data_types import DataSegment
 
 
 @register(API_ACTIONS)
 class DataAPI:
     """Data Api Class.
 
     Provides a translation layer for interacting with data.
 
     Params
     ------
     filename - The filename of the file that will back the data api.
-    block_size - Specified the block size to slice original file data.
     """
 
     SOURCE_THRESHHOLD = 4 * MB  # 4MB
     BLOCK_SIZE = 4 * KB  # 4KB
 
     def __init__(
         self,
```

### Comparing `hexabyte-0.6.0rc0/hexabyte/commands/command_parser.py` & `hexabyte-0.7.0rc0/hexabyte/commands/command_parser.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,33 +1,31 @@
 """Command Parser Module."""
 from __future__ import annotations
 
 from collections.abc import Iterable
 from typing import TYPE_CHECKING, Any
 
-from hexabyte.actions import Action
+from ..actions import Action
 
 if TYPE_CHECKING:
-    from hexabyte.hexabyte_app import HexabyteApp
+    from ..hexabyte_app import HexabyteApp
 
 
 class InvalidCommandError(Exception):
     """Error generated from invalid command strings."""
 
     def __init__(self, cmd: str, msg: str | None = None) -> None:
         """Initialize error."""
         self.cmd = cmd
         self.msg = msg
         super().__init__()
 
     def __str__(self) -> str:
         """Return string representation of error."""
-        if self.msg:
-            return f"{self.msg} - {self.cmd}"
-        return self.cmd
+        return self.msg if self.msg else "Invalid Command"
 
 
 class CommandParser:  # pylint: disable=too-few-public-methods
     """Command Parser Class.
 
     Parses a command string and generates one or more commands.
     """
```

### Comparing `hexabyte-0.6.0rc0/hexabyte/commands/decorators.py` & `hexabyte-0.7.0rc0/hexabyte/commands/decorators.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,12 @@
 """Register actions and associated commands."""
 from collections.abc import Callable, Iterable
 from typing import Any
 
-from hexabyte.actions import Action
-
+from ..actions import Action
 from .command_parser import CommandParser
 
 parser = CommandParser()
 
 
 def register_actions(actions: Iterable[type[Action]]) -> Callable[..., Any]:
     """Class decorator to register new actions."""
```

### Comparing `hexabyte-0.6.0rc0/hexabyte/constants/sizes.py` & `hexabyte-0.7.0rc0/hexabyte/constants/sizes.py`

 * *Files identical despite different names*

### Comparing `hexabyte-0.6.0rc0/hexabyte/data_sources/_data_source.py` & `hexabyte-0.7.0rc0/hexabyte/data_sources/_data_source.py`

 * *Files identical despite different names*

### Comparing `hexabyte-0.6.0rc0/hexabyte/data_sources/paged_data_source.py` & `hexabyte-0.7.0rc0/hexabyte/data_sources/paged_data_source.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,13 @@
 """Paged Data Source Class.
 
 Provides the interface for interacting with raw file data.
 """
-from pathlib import Path
-
-from hexabyte.constants.sizes import DEFAULT_BLOCK_SIZE
-
-from ._data_source import DataSource
+from ..constants.sizes import DEFAULT_BLOCK_SIZE
+from ._data_source import DataSource, Path
 from .data_block import DataBlock
 
 MIN_AUTO_REDUCE_THRESHHOLD = 128
 
 
 class PagedDataSource(DataSource):
     """Data Source Class.
```

### Comparing `hexabyte-0.6.0rc0/hexabyte/data_sources/simple_data_source.py` & `hexabyte-0.7.0rc0/hexabyte/data_sources/simple_data_source.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,12 +1,10 @@
 """Simple Data Source Module."""
 
-from pathlib import Path
-
-from ._data_source import DataSource
+from ._data_source import DataSource, Path
 
 
 class SimpleDataSource(DataSource):
     """A simple no-frills data source for loading files."""
 
     def __len__(self) -> int:
         """Return total data size."""
```

### Comparing `hexabyte-0.6.0rc0/hexabyte/hexabyte_app.py` & `hexabyte-0.7.0rc0/hexabyte/hexabyte_app.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 from textual.widgets import Input
 
 from .actions import Action, ActionError
 from .actions.action_handler import ActionHandler
 from .actions.app import Exit
 from .commands import Command, CommandParser, InvalidCommandError, register_actions
 from .constants.generic import APP_NAME
-from .utils import context
+from .context import context
 from .widgets.command_prompt import CommandPrompt
 from .widgets.help_screen import HelpScreen, HelpWindow
 from .widgets.workbench import Workbench
 
 ACTIONS = [Exit]
 
 
@@ -108,19 +108,17 @@
                     if workbench.active_editor is None:
                         raise ValueError("No active editor")
                     workbench.active_editor.api.do(action)
                     workbench.active_editor.cursor = workbench.active_editor.api.cursor.bit
                     workbench.active_editor.refresh()
                 else:
                     raise InvalidCommandError(event.cmd, f"Unsupported target - {action.TARGET}")
-            prompt.command_success()
-        except InvalidCommandError as err:
-            prompt.command_warn(str(err))
-        except ActionError as err:
-            prompt.command_error(str(err))
+            prompt.set_status("", clear=True)
+        except (ActionError, InvalidCommandError) as err:
+            prompt.set_status(str(err))
 
     def watch_show_help(self, visibility: bool) -> None:
         """Toggle help screen visibility if show_help flag changes."""
         help_screen = self.query_one("#help", HelpScreen)
         help_screen.display = visibility
         window = help_screen.query_one("HelpWindow", HelpWindow)
         window.focus()
```

### Comparing `hexabyte-0.6.0rc0/hexabyte/plugins/info/widgets/info_panel.py` & `hexabyte-0.7.0rc0/hexabyte/widgets/info_panel.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,20 +1,19 @@
 """Sidebar Info Panel."""
 import grp
 import pwd
 import stat
 from hashlib import md5, sha1
 
-import magic
 from textual.app import ComposeResult
 from textual.containers import Horizontal
 from textual.widgets import Label, Static
 
-from hexabyte.constants.sizes import KB, MB
-from hexabyte.widgets.sidebar_panel import SidebarVerticalPanel
+from ..constants.sizes import KB, MB
+from ..widgets.sidebar_panel import SidebarVerticalPanel
 
 
 class InfoItem(Horizontal):  # pylint: disable=too-few-public-methods
     """A row of info."""
 
     DEFAULT_CSS = """
     InfoItem {
@@ -55,15 +54,14 @@
         """Compose child widgets."""
         yield InfoItem(name="filename")
         yield InfoItem(name="path")
         yield InfoItem(name="size")
         yield InfoItem(name="owner")
         yield InfoItem(name="group")
         yield InfoItem(name="permissions")
-        yield InfoItem(name="type")
         yield InfoItem(name="md5")
         yield InfoItem(name="sha1")
 
     def update_hashes(self) -> None:
         """Update file hashes."""
         if self.editor is None:
             return
@@ -94,29 +92,19 @@
 
         group_value = self.query_one("#group-value", Static)
         group_value.update(grp.getgrgid(stats.st_gid).gr_name)
 
         perm_value = self.query_one("#permissions-value", Static)
         perm_value.update(stat.filemode(stats.st_mode))
 
-    def update_type(self) -> None:
-        """Update file type."""
-        if self.editor is None:
-            return
-        filepath = self.editor.api.filepath
-        type_value = self.query_one("#type-value", Static)
-        result = magic.from_file(filepath).replace(", ", "\n - ")
-        type_value.update(result)
-
     def watch_editor(self) -> None:
         """React to changed editor."""
         filename = self.query_one("#filename-value", Static)
         if self.editor is None:
             filename.update("No editor selected")
         else:
             filepath = self.editor.api.filepath
             filename.update(filepath.name)
             path = self.query_one("#path-value", Static)
             path.update(f"{filepath.parent}")
         self.update_stats()
-        self.update_type()
         self.update_hashes()
```

### Comparing `hexabyte-0.6.0rc0/hexabyte/utils/config.py` & `hexabyte-0.7.0rc0/hexabyte/config.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,83 +1,78 @@
 """The hexabyte config module."""
-from importlib.resources import files
+from copy import deepcopy
 from pathlib import Path
-from shutil import copy
 
 import toml
 from munch import Munch
 
-from ..constants.generic import CONFIG_FILENAME, DEFAULT_CONFIG_PATH
+from .constants.generic import CONFIG_FILENAME, DEFAULT_CONFIG_PATH
+
+DEFAULT_SETTINGS: Munch = Munch.fromDict(
+    {
+        "general": {"max-cmd-history": 100, "max-undo": 100, "plugins": []},
+        "normal": {
+            "primary": "hex",
+            "offset-style": "hex",
+            "bin": {"column-count": 8, "column-size": 1},
+            "hex": {"column-count": 32, "column-size": 1},
+            "utf8": {"column-count": 1, "column-size": 64},
+        },
+        "split": {
+            "primary": "hex",
+            "secondary": "utf8",
+            "offset-style": "hex",
+            "bin": {"column-count": 4, "column-size": 1},
+            "hex": {"column-count": 4, "column-size": 4},
+            "utf8": {"column-count": 8, "column-size": 4},
+        },
+        "diff": {
+            "primary": "hex",
+            "secondary": "hex",
+            "offset-style": "hex",
+            "bin": {"column-count": 4, "column-size": 1},
+            "hex": {"column-count": 4, "column-size": 4},
+            "utf8": {"column-count": 8, "column-size": 4},
+        },
+    }
+)
 
 
 class Config:
     """The HexaByte Config Class.
 
-    Responsible for loading, tracking and saving application-wide configurations.
+    Responsible for loading, tracking and saving application-wide configuration settings.
     """
 
     DEFAULT_FILEPATH = DEFAULT_CONFIG_PATH / CONFIG_FILENAME
 
-    # def __new__(cls):
-    #     if not hasattr(cls, 'instance'):
-    #     cls.instance = super(SingletonClass, cls).__new__(cls)
-    #     return cls.instance
-
     def __init__(self) -> None:
         """Initialize the application config."""
         self.filepath: Path | None = None
-        self.settings: Munch = Munch.fromDict(
-            {
-                "general": {"max-cmd-history": 100, "max-undo": 100, "plugins": ["info", "entropy"]},
-                "normal": {
-                    "primary": "hex",
-                    "offset-style": "hex",
-                    "bin": {"column-count": 8, "column-size": 1},
-                    "hex": {"column-count": 32, "column-size": 1},
-                    "utf8": {"column-count": 1, "column-size": 64},
-                },
-                "split": {
-                    "primary": "hex",
-                    "secondary": "utf8",
-                    "offset-style": "hex",
-                    "bin": {"column-count": 4, "column-size": 1},
-                    "hex": {"column-count": 4, "column-size": 4},
-                    "utf8": {"column-count": 8, "column-size": 4},
-                },
-                "diff": {
-                    "primary": "hex",
-                    "secondary": "hex",
-                    "offset-style": "hex",
-                    "bin": {"column-count": 4, "column-size": 1},
-                    "hex": {"column-count": 4, "column-size": 4},
-                    "utf8": {"column-count": 8, "column-size": 4},
-                },
-            }
-        )
+        self.settings: Munch = deepcopy(DEFAULT_SETTINGS)
 
     def save(self) -> None:
         """Save the active configurations to the config file."""
         if self.filepath is None:
             raise ValueError("Config filepath not set.")
         with self.filepath.open("w", encoding="utf8") as config_file:
             toml.dump(self.settings, config_file)
 
     @classmethod
     def from_file(cls, config_filepath: Path = DEFAULT_CONFIG_PATH / CONFIG_FILENAME) -> "Config":
         """Create a config from a config file."""
         config = Config()
-        config_filepath = config_filepath.expanduser()
         config.filepath = config_filepath
         if not config.filepath.exists():
             cls.setup(config.filepath.parent)
         config.settings.update(toml.load(config.filepath))
         return config
 
     @classmethod
     def setup(cls, config_path: Path = DEFAULT_CONFIG_PATH) -> None:
         """Initialize new config for a user."""
         if not config_path.exists():
             config_path.mkdir(parents=True, exist_ok=True)
             plugin_path = config_path / "plugins"
             plugin_path.mkdir(exist_ok=True)
-        src = str(files("hexabyte.assets").joinpath(CONFIG_FILENAME))
-        copy(src, config_path / CONFIG_FILENAME)
+        with (config_path / CONFIG_FILENAME).open("w", encoding="utf8") as config_file:
+            toml.dump(DEFAULT_SETTINGS, config_file)
```

### Comparing `hexabyte-0.6.0rc0/hexabyte/utils/context.py` & `hexabyte-0.7.0rc0/hexabyte/context.py`

 * *Files identical despite different names*

### Comparing `hexabyte-0.6.0rc0/hexabyte/utils/cursor.py` & `hexabyte-0.7.0rc0/hexabyte/cursor.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,23 +1,24 @@
-"""Data Api Cursor Module."""
+"""Data Cursor Module."""
+
 from hexabyte.constants.sizes import (
     BYTE_ALIGN_BITS,
     BYTE_BITS,
     DWORD64_ALIGN_BITS,
     DWORD_ALIGN_BITS,
     NIBBLE_ALIGN_BITS,
     QWORD64_ALIGN_BITS,
     QWORD_ALIGN_BITS,
     WORD64_ALIGN_BITS,
     WORD_ALIGN_BITS,
 )
 
 
 class Cursor:
-    """The Cursor Class.
+    """The Data Cursor Class.
 
     Tracks a cursor position and dynamically converts between different alignments and resolutions.
     Supports bit, nibble, byte, word, word64, and qword64 resolutions.
     """
 
     def __init__(self, val: int = 0, max_bytes: int = 0) -> None:
         """Initialize Cursor."""
```

### Comparing `hexabyte-0.6.0rc0/hexabyte/utils/data_types.py` & `hexabyte-0.7.0rc0/hexabyte/data_types.py`

 * *Files identical despite different names*

### Comparing `hexabyte-0.6.0rc0/hexabyte/view_components/byte_view.py` & `hexabyte-0.7.0rc0/hexabyte/view_components/byte_view.py`

 * *Files 0% similar despite different names*

```diff
@@ -9,18 +9,18 @@
 from rich.measure import Measurement
 from rich.padding import Padding, PaddingDimensions
 from rich.segment import Segment, Segments
 from rich.style import Style
 from rich.text import Text
 from textual.geometry import Size
 
-from hexabyte.constants import DisplayMode
-from hexabyte.constants.sizes import BYTE_BITS, NIBBLE_BITS
-from hexabyte.utils.cursor import Cursor
-from hexabyte.utils.data_types import DataSegment
+from ..constants import DisplayMode
+from ..constants.sizes import BYTE_BITS, NIBBLE_BITS
+from ..cursor import Cursor
+from ..data_types import DataSegment
 
 NUMBERS_COLUMN_DEFAULT_PADDING = 3
 
 
 class ByteView(JupyterMixin):  # pylint: disable=too-many-instance-attributes
     """Construct a ByteView object to render byte data in various formats.
```

### Comparing `hexabyte-0.6.0rc0/hexabyte/view_components/hc_view.py` & `hexabyte-0.7.0rc0/hexabyte/view_components/hc_view.py`

 * *Files 2% similar despite different names*

```diff
@@ -13,16 +13,16 @@
 from rich.padding import Padding, PaddingDimensions
 from rich.segment import Segment, Segments
 from rich.style import Style
 from rich.text import Text
 from textual.color import Color
 from textual.geometry import Size
 
-from hexabyte.utils.cursor import Cursor
-from hexabyte.utils.misc import map_range
+from ..cursor import Cursor
+from ..utils import map_range
 
 HC_DIMENSIONS = 2
 HC_ITERATIONS = 5
 
 
 class HCView(JupyterMixin):
     """Construct a HilbertCurve component.
```

### Comparing `hexabyte-0.6.0rc0/hexabyte/widgets/command_prompt.py` & `hexabyte-0.7.0rc0/hexabyte/widgets/command_prompt.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,19 +1,18 @@
 """Command Prompt Widget."""
 from collections import deque
 from typing import ClassVar
 
 from textual.app import ComposeResult
 from textual.binding import Binding, BindingType
-from textual.color import Color
 from textual.containers import Horizontal
 from textual.reactive import reactive
 from textual.widgets import Input, Label
 
-from hexabyte.commands import Command
+from ..commands import Command
 
 
 class CommandInput(Input):  # pylint: disable=too-few-public-methods
     """Input box for commands."""
 
     BINDINGS: ClassVar[list[BindingType]] = [
         Binding("up", "history_up", "History Previous", show=False),
@@ -54,74 +53,57 @@
         height: 5;
         padding: 0 1;
     }
     CommandPrompt Label {
         dock: left;
         padding: 1;
     }
+    CommandPrompt Label#status {
+        dock: right;
+        padding: 1;
+    }
     CommandPrompt CommandInput {
         margin: 0;
     }
     CommandPrompt CommandInput:focus {
         border: tall $secondary;
     }
     """
 
     def __init__(self, *args, max_cmd_history: int, **kwargs) -> None:
         """Initialize CommandPrompt."""
         super().__init__(*args, **kwargs)
         self.max_cmd_history = max_cmd_history
 
-    def command_success(self, clear: bool = True) -> None:
-        """Flash to signify command success."""
-        box = self.query_one("CommandInput", CommandInput)
-        start_color = box.styles.background
-        box.styles.animate("background", Color(0, 192, 0), final_value=start_color, duration=0.25)  # type: ignore
-        if clear:
-            box.value = ""
+    def set_status(self, msg: str | None = None, clear: bool = False) -> None:
+        """Set the command prompt status message.
 
-    def command_error(self, msg: str | None = None, clear: bool = False) -> None:
-        """Flash to signify command error."""
-        box = self.query_one("CommandInput", CommandInput)
-        start_color = box.styles.background
-        box.styles.animate("background", Color(192, 0, 0), final_value=start_color, duration=0.25)  # type: ignore
+        clear - Clears the command prompt contents
+        """
+        status_msg = self.query_one("#status", Label)
         if msg:
-            box.value = msg
-        elif clear:
-            box.value = ""
-
-    def command_warn(self, msg: str | None = None, clear: bool = False) -> None:
-        """Flash to signify warning for command."""
-        box = self.query_one("CommandInput", CommandInput)
-        start_color = box.styles.background
-        box.styles.animate("background", Color(255, 165, 0), final_value=start_color, duration=0.25)  # type: ignore
-        if msg:
-            box.value = msg
-        elif clear:
+            status_msg.update(msg)
+        else:
+            status_msg.update("")
+        if clear:
+            box = self.query_one("CommandInput", CommandInput)
             box.value = ""
 
     def _update_history(self) -> None:
         """Add current command to input history."""
         box = self.query_one("CommandInput", CommandInput)
         box.history.append(box.value)
         box.history_idx = -1
 
     def compose(self) -> ComposeResult:
         """Compose Command Prompt widgets."""
         yield Label("Command:")
         yield CommandInput(max_cmd_history=self.max_cmd_history)
+        yield Label("", id="status", shrink=True)
 
     def on_input_submitted(self, event: Input.Submitted) -> None:
         """Handle input submitted event."""
         cmd = event.value
         if self.parent is None:
-            self.command_error()
             return
-        if cmd == "test success":
-            self.command_success()
-        elif cmd == "test fail":
-            self.command_error(clear=True)
-        elif cmd == "test warn":
-            self.command_warn()
-        else:
-            self.post_message(Command(cmd))
+        self.post_message(Command(cmd))
         self._update_history()
```

### Comparing `hexabyte-0.6.0rc0/hexabyte/widgets/editor.py` & `hexabyte-0.7.0rc0/hexabyte/widgets/editor.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,20 +6,20 @@
 from textual.binding import Binding, BindingType
 from textual.events import Click, Key, Paste
 from textual.message import Message
 from textual.reactive import reactive
 from textual.scroll_view import ScrollView
 from textual.strip import Strip
 
-from hexabyte.api import DataAPI
-from hexabyte.commands import Command
-from hexabyte.constants import DisplayMode
-from hexabyte.constants.sizes import BIT, BYTE_BITS, NIBBLE_BITS
-from hexabyte.utils import context
-from hexabyte.view_components import ByteView
+from ..api import DataAPI
+from ..commands import Command
+from ..constants import DisplayMode
+from ..constants.sizes import BIT, BYTE_BITS, NIBBLE_BITS
+from ..context import context
+from ..view_components import ByteView
 
 CURSOR_INCREMENTS = {
     DisplayMode.HEX: NIBBLE_BITS,
     DisplayMode.BIN: BIT,
     DisplayMode.UTF8: BYTE_BITS,
 }
```

### Comparing `hexabyte-0.6.0rc0/hexabyte/widgets/help_screen.py` & `hexabyte-0.7.0rc0/hexabyte/widgets/help_screen.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 """Help Screen Widget."""
-
+import toml
 from textual.app import ComposeResult
 from textual.containers import Center, VerticalScroll
 from textual.widgets import Markdown
 
-from hexabyte.constants.generic import APP_NAME
+from ..config import CONFIG_FILENAME, DEFAULT_CONFIG_PATH, DEFAULT_SETTINGS
+from ..constants.generic import APP_NAME
 
 
 class HelpWindow(VerticalScroll):  # pylint: disable=too-few-public-methods
     """Help Screen Content Window Widget."""
 
     can_focus = True
 
@@ -25,15 +26,15 @@
     """Hexabyte Help Screen Widget."""
 
     can_focus_children = True
 
     HELP_TEXT = f"""
 # {APP_NAME} Help
 
-Hexabyte can operate in three distinct modes:
+{APP_NAME} can operate in three distinct modes:
 - single file mode - Opens a single file with a single editor.
 - split screen mode - Opens a single file with a split screen view.
 - diff mode - Opens two files side by side.
 
 ## Global Shortcuts
 
 - `:` - Open Command Prompt
@@ -92,90 +93,31 @@
 - **open** *( primary | secondary )* *filename* - Open a file into the specified editor.
 - **revert** - Revert all unsaved data modifications.
 - **save** - Save data changes to file.
 - **saveas** *new_filename* - Save data changes to a new file.
 - **select** *BYTE_OFFSET* *[LENGTH]* - Select a segment of data. Only one active selection allowed.
 - **unhighlight** *BYTE_OFFSET* *[LENGTH]* - Remove all highlights within specified range.
 
-## Command Prompt
-- **test** *success* - Flash green
-- **test** *fail* - Flash red
-- **test** *warn* - Flash orange
-
 ## Planned Commands
 
 - **copy** - Copy current selection to clipboard.
 - **cut** - Cut current selection to clipboard.
 - **paste** *[ insert ]* - Paste clipboard contents at current offset. Overwrites by default.
 - **match** *sequence* *[mask]* - Highlight all data segments that match the masked byte sequence.
   - **match** *b'abc'*
   - **match** *b'abc'* *b'\\xff\\xff\\xff'*
   - **match** *b'abc'* *b'\\xf0\\x0f\\xf0'*
 
-## Example Configuration File
+## Configuration File
 
-Default Location: `~/.config/hexabyte/config.toml`
+Default Location: `{DEFAULT_CONFIG_PATH/CONFIG_FILENAME}`
 
+Default Settings:
 ```toml
-[general]
-max-cmd-history = 100
-max-undo = 100
-
-[normal]
-primary      = 'hex' # 'hex', 'bin', 'utf8'
-offset-style = 'hex' # 'hex', 'dec', 'off'
-
-# Column count is the number of columns per row
-# Column width represents the byte width of each column
-
-[normal.bin]
-column-count = 8
-column-size  = 1
-
-[normal.hex]
-column-count = 32
-column-size  = 1
-
-[normal.utf8]
-column-count = 1
-column-size  = 64
-
-[split]
-primary      = 'hex'  # 'hex', 'bin', 'utf8'
-secondary    = 'utf8' # 'hex', 'bin', 'utf8'
-offset-style = 'hex'  # 'hex', 'dec', 'off'
-
-[split.bin]
-column-count = 4
-column-size  = 1
-
-[split.hex]
-column-count = 4
-column-size  = 4
-
-[split.utf8]
-column-count = 8
-column-size  = 4
-
-[diff]
-primary      = 'hex' # 'hex', 'bin', 'utf8'
-secondary    = 'hex' # 'hex', 'bin', 'utf8'
-offset-style = 'hex' # 'hex', 'dec', 'off'
-
-[diff.bin]
-column-count = 4
-column-size  = 1
-
-[diff.hex]
-column-count = 4
-column-size  = 4
-
-[diff.utf8]
-column-count = 8
-column-size  = 4
+{toml.dumps(DEFAULT_SETTINGS)}
 ```
 """
 
     DEFAULT_CSS = """
     HelpScreen {
         width: 100%;
         height: 100%;
@@ -189,11 +131,7 @@
         padding: 2;
     }
     """
 
     def compose(self) -> ComposeResult:
         """Compose help screen widgets."""
         yield HelpWindow(Markdown(self.HELP_TEXT, id=f"{self.id}-text"), id=f"{self.id}-window")
-
-    # def on_click(self) -> None:
-    #     """React to click event."""
-    #     self.display = False
```

### Comparing `hexabyte-0.6.0rc0/hexabyte/widgets/sidebar.py` & `hexabyte-0.7.0rc0/hexabyte/widgets/sidebar.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 """The Workbench Sidebar Module."""
 
 from textual.app import ComposeResult
 from textual.containers import Vertical
 from textual.reactive import reactive
 from textual.widgets import ContentSwitcher, Tab, Tabs
 
-from hexabyte.widgets.sidebar_panel import SidebarPanel
-
+from ..widgets.info_panel import InfoPanel
+from ..widgets.sidebar_panel import SidebarPanel
 from .editor import Editor
 
-sidebar_panels: dict[str, type[SidebarPanel]] = {}
+sidebar_panels: dict[str, type[SidebarPanel]] = {"info": InfoPanel}
 
 
 class Sidebar(Vertical):
     """The tabbed sidebar container."""
 
     DEFAULT_CSS = """
     Sidebar {
```

### Comparing `hexabyte-0.6.0rc0/hexabyte/widgets/sidebar_panel.py` & `hexabyte-0.7.0rc0/hexabyte/widgets/sidebar_panel.py`

 * *Files identical despite different names*

### Comparing `hexabyte-0.6.0rc0/hexabyte/widgets/workbench.py` & `hexabyte-0.7.0rc0/hexabyte/widgets/workbench.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,18 +1,17 @@
 """Workbench Class Module."""
 from textual.app import ComposeResult
 from textual.containers import Container, Vertical
 from textual.reactive import reactive
 from textual.widgets import Footer, Header
 
-from hexabyte.api import DataAPI
-from hexabyte.constants import FileMode
-from hexabyte.constants.generic import DIFF_FILE_COUNT
-from hexabyte.utils import context
-
+from ..api import DataAPI
+from ..constants import FileMode
+from ..constants.generic import DIFF_FILE_COUNT
+from ..context import context
 from .editor import Editor
 from .sidebar import Sidebar
 
 
 class Body(Container):  # pylint: disable=too-few-public-methods
     """Main container for workspace."""
```

### Comparing `hexabyte-0.6.0rc0/pyproject.toml` & `hexabyte-0.7.0rc0/pyproject.toml`

 * *Files 11% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 [tool.poetry]
 name = "hexabyte"
-version = "0.6.0rc0"
+version = "0.7.0-rc.0"
 description = "A modern, modular, and robust TUI hex editor."
-keywords = ["commandline", "hexeditor", "binary", "hexadecimal", "raw", "byteview"]
+keywords = ["commandline", "hexeditor", "binary", "hexadecimal", "raw", "byteview", "bytes"]
 repository = "https://github.com/thetacom/hexabyte"
 authors = ["Justin C <justin@thetacom.info>"]
 readme = "docs/README.md"
 classifiers = [
     "Development Status :: 3 - Alpha",
     "Environment :: Console",
     "Intended Audience :: Developers",
@@ -25,53 +25,47 @@
     "Topic :: Software Development",
     "Topic :: Utilities",
 ]
 packages = [{ include = 'hexabyte' }]
 
 [tool.poetry.dependencies]
 python       = "^3.10"
-textual      = "^0.24.1"
+textual      = "^0.26.0"
 toml         = "^0.10.2"
-python-magic = "^0.4.27"
-hilbertcurve = "^2.0.5"
 munch        = "^2.5.0"
 
 [tool.poetry.group.dev.dependencies]
 black                  = "^23.3.0"
 bandit                 = "^1.7.5"
 coverage               = "^7.2.3"
 deepdiff               = "^6.3.0"
 ipython                = "^8.13.2"
 isort                  = "^5.12.0"
 httpretty              = "^1.1.4"
-livereload             = "^2.6.3"
 mkdocs                 = "^1.4.2"
 mkdocstrings           = "^0.21.2"
 mkdocs-jupyter         = "^0.24.1"
 mkdocs-material        = "^9.1.8"
 mkdocs-mermaid2-plugin = "^0.6.0"
 mkdocs-minify-plugin   = "^0.6.4"
 mkdocs-redirects       = "^1.2.0"
 matplotlib             = "^3.7.1"
-msgpack                = "^1.0.5"
 mypy                   = "^1.2.0"
 pydocstyle             = "^6.3.0"
 pylint                 = "^2.17.3"
 pytest                 = "^7.3.1"
 pytest-bandit          = "^0.6.1"
 pytest-cov             = "^4.0.0"
 pytest-mock            = "^3.10.0"
 pytest-pydocstyle      = "^2.3.2"
 pytest-sugar           = "^0.9.7"
 pre-commit             = "^3.2.2"
 ruff                   = "^0.0.263"
-tox                    = "^4.5.1"
 types-toml             = "^0.10.8.5"
 typing-extensions      = "^4.5.0"
-zipp                   = "^3.15.0"
 
 [build-system]
 requires      = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry.scripts]
 hexabyte = "hexabyte.__main__:main"
```

### Comparing `hexabyte-0.6.0rc0/PKG-INFO` & `hexabyte-0.7.0rc0/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: hexabyte
-Version: 0.6.0rc0
+Version: 0.7.0rc0
 Summary: A modern, modular, and robust TUI hex editor.
 Home-page: https://github.com/thetacom/hexabyte
-Keywords: commandline,hexeditor,binary,hexadecimal,raw,byteview
+Keywords: commandline,hexeditor,binary,hexadecimal,raw,byteview,bytes
 Author: Justin C
 Author-email: justin@thetacom.info
 Requires-Python: >=3.10,<4.0
 Classifier: Development Status :: 3 - Alpha
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Information Technology
@@ -17,24 +17,20 @@
 Classifier: Natural Language :: English
 Classifier: Operating System :: MacOS :: MacOS X
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3 :: Only
-Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Topic :: Software Development
 Classifier: Topic :: Utilities
-Requires-Dist: hilbertcurve (>=2.0.5,<3.0.0)
 Requires-Dist: munch (>=2.5.0,<3.0.0)
-Requires-Dist: python-magic (>=0.4.27,<0.5.0)
-Requires-Dist: textual (>=0.24.1,<0.25.0)
+Requires-Dist: textual (>=0.26.0,<0.27.0)
 Requires-Dist: toml (>=0.10.2,<0.11.0)
 Project-URL: Repository, https://github.com/thetacom/hexabyte
 Description-Content-Type: text/markdown
 
 # Hexabyte - Commandline Hex Editor
 
 A modern, robust, and extensible commandline hex editor.
```

