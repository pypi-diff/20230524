# Comparing `tmp/robotcode_language_server-0.40.0.tar.gz` & `tmp/robotcode_language_server-0.41.0.tar.gz`

## Comparing `robotcode_language_server-0.40.0.tar` & `robotcode_language_server-0.41.0.tar`

### file list

```diff
@@ -1,87 +1,87 @@
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 robotcode_language_server-0.40.0/src/robotcode/language_server/__init__.py
--rw-r--r--   0        0        0       23 2020-02-02 00:00:00.000000 robotcode_language_server-0.40.0/src/robotcode/language_server/__version__.py
--rw-r--r--   0        0        0     3139 2020-02-02 00:00:00.000000 robotcode_language_server-0.40.0/src/robotcode/language_server/cli.py
--rw-r--r--   0        0        0      209 2020-02-02 00:00:00.000000 robotcode_language_server-0.40.0/src/robotcode/language_server/hooks.py
--rw-r--r--   0        0        0       27 2020-02-02 00:00:00.000000 robotcode_language_server-0.40.0/src/robotcode/language_server/py.typed
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 robotcode_language_server-0.40.0/src/robotcode/language_server/common/__init__.py
--rw-r--r--   0        0        0     2563 2020-02-02 00:00:00.000000 robotcode_language_server-0.40.0/src/robotcode/language_server/common/decorators.py
--rw-r--r--   0        0        0      290 2020-02-02 00:00:00.000000 robotcode_language_server-0.40.0/src/robotcode/language_server/common/has_extend_capabilities.py
--rw-r--r--   0        0        0    11515 2020-02-02 00:00:00.000000 robotcode_language_server-0.40.0/src/robotcode/language_server/common/protocol.py
--rw-r--r--   0        0        0      781 2020-02-02 00:00:00.000000 robotcode_language_server-0.40.0/src/robotcode/language_server/common/server.py
--rw-r--r--   0        0        0     9485 2020-02-02 00:00:00.000000 robotcode_language_server-0.40.0/src/robotcode/language_server/common/text_document.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 robotcode_language_server-0.40.0/src/robotcode/language_server/common/parts/__init__.py
--rw-r--r--   0        0        0     4411 2020-02-02 00:00:00.000000 robotcode_language_server-0.40.0/src/robotcode/language_server/common/parts/code_action.py
--rw-r--r--   0        0        0     4239 2020-02-02 00:00:00.000000 robotcode_language_server-0.40.0/src/robotcode/language_server/common/parts/code_lens.py
--rw-r--r--   0        0        0     3438 2020-02-02 00:00:00.000000 robotcode_language_server-0.40.0/src/robotcode/language_server/common/parts/commands.py
--rw-r--r--   0        0        0     6206 2020-02-02 00:00:00.000000 robotcode_language_server-0.40.0/src/robotcode/language_server/common/parts/completion.py
--rw-r--r--   0        0        0     4648 2020-02-02 00:00:00.000000 robotcode_language_server-0.40.0/src/robotcode/language_server/common/parts/declaration.py
--rw-r--r--   0        0        0     4650 2020-02-02 00:00:00.000000 robotcode_language_server-0.40.0/src/robotcode/language_server/common/parts/definition.py
--rw-r--r--   0        0        0    21107 2020-02-02 00:00:00.000000 robotcode_language_server-0.40.0/src/robotcode/language_server/common/parts/diagnostics.py
--rw-r--r--   0        0        0     2689 2020-02-02 00:00:00.000000 robotcode_language_server-0.40.0/src/robotcode/language_server/common/parts/document_highlight.py
--rw-r--r--   0        0        0     5937 2020-02-02 00:00:00.000000 robotcode_language_server-0.40.0/src/robotcode/language_server/common/parts/document_symbols.py
--rw-r--r--   0        0        0    14870 2020-02-02 00:00:00.000000 robotcode_language_server-0.40.0/src/robotcode/language_server/common/parts/documents.py
--rw-r--r--   0        0        0     2784 2020-02-02 00:00:00.000000 robotcode_language_server-0.40.0/src/robotcode/language_server/common/parts/folding_range.py
--rw-r--r--   0        0        0     4399 2020-02-02 00:00:00.000000 robotcode_language_server-0.40.0/src/robotcode/language_server/common/parts/formatting.py
--rw-r--r--   0        0        0     2676 2020-02-02 00:00:00.000000 robotcode_language_server-0.40.0/src/robotcode/language_server/common/parts/hover.py
--rw-r--r--   0        0        0     4651 2020-02-02 00:00:00.000000 robotcode_language_server-0.40.0/src/robotcode/language_server/common/parts/implementation.py
--rw-r--r--   0        0        0     3858 2020-02-02 00:00:00.000000 robotcode_language_server-0.40.0/src/robotcode/language_server/common/parts/inlay_hint.py
--rw-r--r--   0        0        0     3657 2020-02-02 00:00:00.000000 robotcode_language_server-0.40.0/src/robotcode/language_server/common/parts/inline_value.py
--rw-r--r--   0        0        0     2730 2020-02-02 00:00:00.000000 robotcode_language_server-0.40.0/src/robotcode/language_server/common/parts/linked_editing_ranges.py
--rw-r--r--   0        0        0      424 2020-02-02 00:00:00.000000 robotcode_language_server-0.40.0/src/robotcode/language_server/common/parts/protocol_part.py
--rw-r--r--   0        0        0     2842 2020-02-02 00:00:00.000000 robotcode_language_server-0.40.0/src/robotcode/language_server/common/parts/references.py
--rw-r--r--   0        0        0     5780 2020-02-02 00:00:00.000000 robotcode_language_server-0.40.0/src/robotcode/language_server/common/parts/rename.py
--rw-r--r--   0        0        0     2891 2020-02-02 00:00:00.000000 robotcode_language_server-0.40.0/src/robotcode/language_server/common/parts/selection_range.py
--rw-r--r--   0        0        0     6963 2020-02-02 00:00:00.000000 robotcode_language_server-0.40.0/src/robotcode/language_server/common/parts/semantic_tokens.py
--rw-r--r--   0        0        0     3629 2020-02-02 00:00:00.000000 robotcode_language_server-0.40.0/src/robotcode/language_server/common/parts/signature_help.py
--rw-r--r--   0        0        0     9340 2020-02-02 00:00:00.000000 robotcode_language_server-0.40.0/src/robotcode/language_server/common/parts/window.py
--rw-r--r--   0        0        0    18981 2020-02-02 00:00:00.000000 robotcode_language_server-0.40.0/src/robotcode/language_server/common/parts/workspace.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 robotcode_language_server-0.40.0/src/robotcode/language_server/robotframework/__init__.py
--rw-r--r--   0        0        0     3907 2020-02-02 00:00:00.000000 robotcode_language_server-0.40.0/src/robotcode/language_server/robotframework/configuration.py
--rw-r--r--   0        0        0      350 2020-02-02 00:00:00.000000 robotcode_language_server-0.40.0/src/robotcode/language_server/robotframework/languages.py
--rw-r--r--   0        0        0     8569 2020-02-02 00:00:00.000000 robotcode_language_server-0.40.0/src/robotcode/language_server/robotframework/protocol.py
--rw-r--r--   0        0        0      815 2020-02-02 00:00:00.000000 robotcode_language_server-0.40.0/src/robotcode/language_server/robotframework/server.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 robotcode_language_server-0.40.0/src/robotcode/language_server/robotframework/diagnostics/__init__.py
--rw-r--r--   0        0        0    38199 2020-02-02 00:00:00.000000 robotcode_language_server-0.40.0/src/robotcode/language_server/robotframework/diagnostics/analyzer.py
--rw-r--r--   0        0        0     7935 2020-02-02 00:00:00.000000 robotcode_language_server-0.40.0/src/robotcode/language_server/robotframework/diagnostics/entities.py
--rw-r--r--   0        0        0    56373 2020-02-02 00:00:00.000000 robotcode_language_server-0.40.0/src/robotcode/language_server/robotframework/diagnostics/imports_manager.py
--rw-r--r--   0        0        0    66000 2020-02-02 00:00:00.000000 robotcode_language_server-0.40.0/src/robotcode/language_server/robotframework/diagnostics/library_doc.py
--rw-r--r--   0        0        0    83635 2020-02-02 00:00:00.000000 robotcode_language_server-0.40.0/src/robotcode/language_server/robotframework/diagnostics/namespace.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 robotcode_language_server-0.40.0/src/robotcode/language_server/robotframework/parts/__init__.py
--rw-r--r--   0        0        0    15318 2020-02-02 00:00:00.000000 robotcode_language_server-0.40.0/src/robotcode/language_server/robotframework/parts/code_action_documentation.py
--rw-r--r--   0        0        0     7151 2020-02-02 00:00:00.000000 robotcode_language_server-0.40.0/src/robotcode/language_server/robotframework/parts/code_action_fixes.py
--rw-r--r--   0        0        0     6670 2020-02-02 00:00:00.000000 robotcode_language_server-0.40.0/src/robotcode/language_server/robotframework/parts/codelens.py
--rw-r--r--   0        0        0    85398 2020-02-02 00:00:00.000000 robotcode_language_server-0.40.0/src/robotcode/language_server/robotframework/parts/completion.py
--rw-r--r--   0        0        0     3701 2020-02-02 00:00:00.000000 robotcode_language_server-0.40.0/src/robotcode/language_server/robotframework/parts/debugging_utils.py
--rw-r--r--   0        0        0    16867 2020-02-02 00:00:00.000000 robotcode_language_server-0.40.0/src/robotcode/language_server/robotframework/parts/diagnostics.py
--rw-r--r--   0        0        0     2629 2020-02-02 00:00:00.000000 robotcode_language_server-0.40.0/src/robotcode/language_server/robotframework/parts/document_highlight.py
--rw-r--r--   0        0        0     9872 2020-02-02 00:00:00.000000 robotcode_language_server-0.40.0/src/robotcode/language_server/robotframework/parts/document_symbols.py
--rw-r--r--   0        0        0    19441 2020-02-02 00:00:00.000000 robotcode_language_server-0.40.0/src/robotcode/language_server/robotframework/parts/documents_cache.py
--rw-r--r--   0        0        0     4384 2020-02-02 00:00:00.000000 robotcode_language_server-0.40.0/src/robotcode/language_server/robotframework/parts/folding_range.py
--rw-r--r--   0        0        0     7661 2020-02-02 00:00:00.000000 robotcode_language_server-0.40.0/src/robotcode/language_server/robotframework/parts/formatting.py
--rw-r--r--   0        0        0    26508 2020-02-02 00:00:00.000000 robotcode_language_server-0.40.0/src/robotcode/language_server/robotframework/parts/goto.py
--rw-r--r--   0        0        0    23534 2020-02-02 00:00:00.000000 robotcode_language_server-0.40.0/src/robotcode/language_server/robotframework/parts/hover.py
--rw-r--r--   0        0        0     8872 2020-02-02 00:00:00.000000 robotcode_language_server-0.40.0/src/robotcode/language_server/robotframework/parts/inlay_hint.py
--rw-r--r--   0        0        0     3420 2020-02-02 00:00:00.000000 robotcode_language_server-0.40.0/src/robotcode/language_server/robotframework/parts/inline_value.py
--rw-r--r--   0        0        0    24255 2020-02-02 00:00:00.000000 robotcode_language_server-0.40.0/src/robotcode/language_server/robotframework/parts/model_helper.py
--rw-r--r--   0        0        0      469 2020-02-02 00:00:00.000000 robotcode_language_server-0.40.0/src/robotcode/language_server/robotframework/parts/protocol_part.py
--rw-r--r--   0        0        0    19638 2020-02-02 00:00:00.000000 robotcode_language_server-0.40.0/src/robotcode/language_server/robotframework/parts/references.py
--rw-r--r--   0        0        0    24952 2020-02-02 00:00:00.000000 robotcode_language_server-0.40.0/src/robotcode/language_server/robotframework/parts/rename.py
--rw-r--r--   0        0        0     6299 2020-02-02 00:00:00.000000 robotcode_language_server-0.40.0/src/robotcode/language_server/robotframework/parts/robocop_diagnostics.py
--rw-r--r--   0        0        0     8493 2020-02-02 00:00:00.000000 robotcode_language_server-0.40.0/src/robotcode/language_server/robotframework/parts/robot_workspace.py
--rw-r--r--   0        0        0     2724 2020-02-02 00:00:00.000000 robotcode_language_server-0.40.0/src/robotcode/language_server/robotframework/parts/selection_range.py
--rw-r--r--   0        0        0    42551 2020-02-02 00:00:00.000000 robotcode_language_server-0.40.0/src/robotcode/language_server/robotframework/parts/semantic_tokens.py
--rw-r--r--   0        0        0    15709 2020-02-02 00:00:00.000000 robotcode_language_server-0.40.0/src/robotcode/language_server/robotframework/parts/signature_help.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 robotcode_language_server-0.40.0/src/robotcode/language_server/robotframework/utils/__init__.py
--rw-r--r--   0        0        0     1722 2020-02-02 00:00:00.000000 robotcode_language_server-0.40.0/src/robotcode/language_server/robotframework/utils/_variables.py
--rw-r--r--   0        0        0     7957 2020-02-02 00:00:00.000000 robotcode_language_server-0.40.0/src/robotcode/language_server/robotframework/utils/ast_utils.py
--rw-r--r--   0        0        0     3163 2020-02-02 00:00:00.000000 robotcode_language_server-0.40.0/src/robotcode/language_server/robotframework/utils/async_ast.py
--rw-r--r--   0        0        0    11653 2020-02-02 00:00:00.000000 robotcode_language_server-0.40.0/src/robotcode/language_server/robotframework/utils/markdownformatter.py
--rw-r--r--   0        0        0      268 2020-02-02 00:00:00.000000 robotcode_language_server-0.40.0/src/robotcode/language_server/robotframework/utils/match.py
--rw-r--r--   0        0        0     1739 2020-02-02 00:00:00.000000 robotcode_language_server-0.40.0/src/robotcode/language_server/robotframework/utils/robot_path.py
--rw-r--r--   0        0        0     1357 2020-02-02 00:00:00.000000 robotcode_language_server-0.40.0/src/robotcode/language_server/robotframework/utils/variables.py
--rw-r--r--   0        0        0      482 2020-02-02 00:00:00.000000 robotcode_language_server-0.40.0/src/robotcode/language_server/robotframework/utils/version.py
--rw-r--r--   0        0        0     4277 2020-02-02 00:00:00.000000 robotcode_language_server-0.40.0/.gitignore
--rw-r--r--   0        0        0    10280 2020-02-02 00:00:00.000000 robotcode_language_server-0.40.0/LICENSE.txt
--rw-r--r--   0        0        0      765 2020-02-02 00:00:00.000000 robotcode_language_server-0.40.0/README.md
--rw-r--r--   0        0        0     1799 2020-02-02 00:00:00.000000 robotcode_language_server-0.40.0/pyproject.toml
--rw-r--r--   0        0        0     2185 2020-02-02 00:00:00.000000 robotcode_language_server-0.40.0/PKG-INFO
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 robotcode_language_server-0.41.0/src/robotcode/language_server/__init__.py
+-rw-r--r--   0        0        0       23 2020-02-02 00:00:00.000000 robotcode_language_server-0.41.0/src/robotcode/language_server/__version__.py
+-rw-r--r--   0        0        0     3139 2020-02-02 00:00:00.000000 robotcode_language_server-0.41.0/src/robotcode/language_server/cli.py
+-rw-r--r--   0        0        0      209 2020-02-02 00:00:00.000000 robotcode_language_server-0.41.0/src/robotcode/language_server/hooks.py
+-rw-r--r--   0        0        0       27 2020-02-02 00:00:00.000000 robotcode_language_server-0.41.0/src/robotcode/language_server/py.typed
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 robotcode_language_server-0.41.0/src/robotcode/language_server/common/__init__.py
+-rw-r--r--   0        0        0     2563 2020-02-02 00:00:00.000000 robotcode_language_server-0.41.0/src/robotcode/language_server/common/decorators.py
+-rw-r--r--   0        0        0      290 2020-02-02 00:00:00.000000 robotcode_language_server-0.41.0/src/robotcode/language_server/common/has_extend_capabilities.py
+-rw-r--r--   0        0        0    11515 2020-02-02 00:00:00.000000 robotcode_language_server-0.41.0/src/robotcode/language_server/common/protocol.py
+-rw-r--r--   0        0        0      781 2020-02-02 00:00:00.000000 robotcode_language_server-0.41.0/src/robotcode/language_server/common/server.py
+-rw-r--r--   0        0        0     9485 2020-02-02 00:00:00.000000 robotcode_language_server-0.41.0/src/robotcode/language_server/common/text_document.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 robotcode_language_server-0.41.0/src/robotcode/language_server/common/parts/__init__.py
+-rw-r--r--   0        0        0     4411 2020-02-02 00:00:00.000000 robotcode_language_server-0.41.0/src/robotcode/language_server/common/parts/code_action.py
+-rw-r--r--   0        0        0     4239 2020-02-02 00:00:00.000000 robotcode_language_server-0.41.0/src/robotcode/language_server/common/parts/code_lens.py
+-rw-r--r--   0        0        0     3438 2020-02-02 00:00:00.000000 robotcode_language_server-0.41.0/src/robotcode/language_server/common/parts/commands.py
+-rw-r--r--   0        0        0     6206 2020-02-02 00:00:00.000000 robotcode_language_server-0.41.0/src/robotcode/language_server/common/parts/completion.py
+-rw-r--r--   0        0        0     4648 2020-02-02 00:00:00.000000 robotcode_language_server-0.41.0/src/robotcode/language_server/common/parts/declaration.py
+-rw-r--r--   0        0        0     4650 2020-02-02 00:00:00.000000 robotcode_language_server-0.41.0/src/robotcode/language_server/common/parts/definition.py
+-rw-r--r--   0        0        0    21107 2020-02-02 00:00:00.000000 robotcode_language_server-0.41.0/src/robotcode/language_server/common/parts/diagnostics.py
+-rw-r--r--   0        0        0     2689 2020-02-02 00:00:00.000000 robotcode_language_server-0.41.0/src/robotcode/language_server/common/parts/document_highlight.py
+-rw-r--r--   0        0        0     5937 2020-02-02 00:00:00.000000 robotcode_language_server-0.41.0/src/robotcode/language_server/common/parts/document_symbols.py
+-rw-r--r--   0        0        0    14870 2020-02-02 00:00:00.000000 robotcode_language_server-0.41.0/src/robotcode/language_server/common/parts/documents.py
+-rw-r--r--   0        0        0     2784 2020-02-02 00:00:00.000000 robotcode_language_server-0.41.0/src/robotcode/language_server/common/parts/folding_range.py
+-rw-r--r--   0        0        0     4399 2020-02-02 00:00:00.000000 robotcode_language_server-0.41.0/src/robotcode/language_server/common/parts/formatting.py
+-rw-r--r--   0        0        0     2676 2020-02-02 00:00:00.000000 robotcode_language_server-0.41.0/src/robotcode/language_server/common/parts/hover.py
+-rw-r--r--   0        0        0     4651 2020-02-02 00:00:00.000000 robotcode_language_server-0.41.0/src/robotcode/language_server/common/parts/implementation.py
+-rw-r--r--   0        0        0     3858 2020-02-02 00:00:00.000000 robotcode_language_server-0.41.0/src/robotcode/language_server/common/parts/inlay_hint.py
+-rw-r--r--   0        0        0     3657 2020-02-02 00:00:00.000000 robotcode_language_server-0.41.0/src/robotcode/language_server/common/parts/inline_value.py
+-rw-r--r--   0        0        0     2730 2020-02-02 00:00:00.000000 robotcode_language_server-0.41.0/src/robotcode/language_server/common/parts/linked_editing_ranges.py
+-rw-r--r--   0        0        0      424 2020-02-02 00:00:00.000000 robotcode_language_server-0.41.0/src/robotcode/language_server/common/parts/protocol_part.py
+-rw-r--r--   0        0        0     2842 2020-02-02 00:00:00.000000 robotcode_language_server-0.41.0/src/robotcode/language_server/common/parts/references.py
+-rw-r--r--   0        0        0     5780 2020-02-02 00:00:00.000000 robotcode_language_server-0.41.0/src/robotcode/language_server/common/parts/rename.py
+-rw-r--r--   0        0        0     2891 2020-02-02 00:00:00.000000 robotcode_language_server-0.41.0/src/robotcode/language_server/common/parts/selection_range.py
+-rw-r--r--   0        0        0     6963 2020-02-02 00:00:00.000000 robotcode_language_server-0.41.0/src/robotcode/language_server/common/parts/semantic_tokens.py
+-rw-r--r--   0        0        0     3629 2020-02-02 00:00:00.000000 robotcode_language_server-0.41.0/src/robotcode/language_server/common/parts/signature_help.py
+-rw-r--r--   0        0        0     9340 2020-02-02 00:00:00.000000 robotcode_language_server-0.41.0/src/robotcode/language_server/common/parts/window.py
+-rw-r--r--   0        0        0    18981 2020-02-02 00:00:00.000000 robotcode_language_server-0.41.0/src/robotcode/language_server/common/parts/workspace.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 robotcode_language_server-0.41.0/src/robotcode/language_server/robotframework/__init__.py
+-rw-r--r--   0        0        0     3973 2020-02-02 00:00:00.000000 robotcode_language_server-0.41.0/src/robotcode/language_server/robotframework/configuration.py
+-rw-r--r--   0        0        0      350 2020-02-02 00:00:00.000000 robotcode_language_server-0.41.0/src/robotcode/language_server/robotframework/languages.py
+-rw-r--r--   0        0        0     8569 2020-02-02 00:00:00.000000 robotcode_language_server-0.41.0/src/robotcode/language_server/robotframework/protocol.py
+-rw-r--r--   0        0        0      815 2020-02-02 00:00:00.000000 robotcode_language_server-0.41.0/src/robotcode/language_server/robotframework/server.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 robotcode_language_server-0.41.0/src/robotcode/language_server/robotframework/diagnostics/__init__.py
+-rw-r--r--   0        0        0    38199 2020-02-02 00:00:00.000000 robotcode_language_server-0.41.0/src/robotcode/language_server/robotframework/diagnostics/analyzer.py
+-rw-r--r--   0        0        0     7935 2020-02-02 00:00:00.000000 robotcode_language_server-0.41.0/src/robotcode/language_server/robotframework/diagnostics/entities.py
+-rw-r--r--   0        0        0    56373 2020-02-02 00:00:00.000000 robotcode_language_server-0.41.0/src/robotcode/language_server/robotframework/diagnostics/imports_manager.py
+-rw-r--r--   0        0        0    66000 2020-02-02 00:00:00.000000 robotcode_language_server-0.41.0/src/robotcode/language_server/robotframework/diagnostics/library_doc.py
+-rw-r--r--   0        0        0    83635 2020-02-02 00:00:00.000000 robotcode_language_server-0.41.0/src/robotcode/language_server/robotframework/diagnostics/namespace.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 robotcode_language_server-0.41.0/src/robotcode/language_server/robotframework/parts/__init__.py
+-rw-r--r--   0        0        0    15318 2020-02-02 00:00:00.000000 robotcode_language_server-0.41.0/src/robotcode/language_server/robotframework/parts/code_action_documentation.py
+-rw-r--r--   0        0        0     7151 2020-02-02 00:00:00.000000 robotcode_language_server-0.41.0/src/robotcode/language_server/robotframework/parts/code_action_fixes.py
+-rw-r--r--   0        0        0     6670 2020-02-02 00:00:00.000000 robotcode_language_server-0.41.0/src/robotcode/language_server/robotframework/parts/codelens.py
+-rw-r--r--   0        0        0    85398 2020-02-02 00:00:00.000000 robotcode_language_server-0.41.0/src/robotcode/language_server/robotframework/parts/completion.py
+-rw-r--r--   0        0        0     3701 2020-02-02 00:00:00.000000 robotcode_language_server-0.41.0/src/robotcode/language_server/robotframework/parts/debugging_utils.py
+-rw-r--r--   0        0        0    16867 2020-02-02 00:00:00.000000 robotcode_language_server-0.41.0/src/robotcode/language_server/robotframework/parts/diagnostics.py
+-rw-r--r--   0        0        0     2629 2020-02-02 00:00:00.000000 robotcode_language_server-0.41.0/src/robotcode/language_server/robotframework/parts/document_highlight.py
+-rw-r--r--   0        0        0     9872 2020-02-02 00:00:00.000000 robotcode_language_server-0.41.0/src/robotcode/language_server/robotframework/parts/document_symbols.py
+-rw-r--r--   0        0        0    19441 2020-02-02 00:00:00.000000 robotcode_language_server-0.41.0/src/robotcode/language_server/robotframework/parts/documents_cache.py
+-rw-r--r--   0        0        0     4384 2020-02-02 00:00:00.000000 robotcode_language_server-0.41.0/src/robotcode/language_server/robotframework/parts/folding_range.py
+-rw-r--r--   0        0        0     8495 2020-02-02 00:00:00.000000 robotcode_language_server-0.41.0/src/robotcode/language_server/robotframework/parts/formatting.py
+-rw-r--r--   0        0        0    26508 2020-02-02 00:00:00.000000 robotcode_language_server-0.41.0/src/robotcode/language_server/robotframework/parts/goto.py
+-rw-r--r--   0        0        0    23534 2020-02-02 00:00:00.000000 robotcode_language_server-0.41.0/src/robotcode/language_server/robotframework/parts/hover.py
+-rw-r--r--   0        0        0     8872 2020-02-02 00:00:00.000000 robotcode_language_server-0.41.0/src/robotcode/language_server/robotframework/parts/inlay_hint.py
+-rw-r--r--   0        0        0     3420 2020-02-02 00:00:00.000000 robotcode_language_server-0.41.0/src/robotcode/language_server/robotframework/parts/inline_value.py
+-rw-r--r--   0        0        0    24255 2020-02-02 00:00:00.000000 robotcode_language_server-0.41.0/src/robotcode/language_server/robotframework/parts/model_helper.py
+-rw-r--r--   0        0        0      469 2020-02-02 00:00:00.000000 robotcode_language_server-0.41.0/src/robotcode/language_server/robotframework/parts/protocol_part.py
+-rw-r--r--   0        0        0    19638 2020-02-02 00:00:00.000000 robotcode_language_server-0.41.0/src/robotcode/language_server/robotframework/parts/references.py
+-rw-r--r--   0        0        0    24952 2020-02-02 00:00:00.000000 robotcode_language_server-0.41.0/src/robotcode/language_server/robotframework/parts/rename.py
+-rw-r--r--   0        0        0     6299 2020-02-02 00:00:00.000000 robotcode_language_server-0.41.0/src/robotcode/language_server/robotframework/parts/robocop_diagnostics.py
+-rw-r--r--   0        0        0     8493 2020-02-02 00:00:00.000000 robotcode_language_server-0.41.0/src/robotcode/language_server/robotframework/parts/robot_workspace.py
+-rw-r--r--   0        0        0     2724 2020-02-02 00:00:00.000000 robotcode_language_server-0.41.0/src/robotcode/language_server/robotframework/parts/selection_range.py
+-rw-r--r--   0        0        0    42551 2020-02-02 00:00:00.000000 robotcode_language_server-0.41.0/src/robotcode/language_server/robotframework/parts/semantic_tokens.py
+-rw-r--r--   0        0        0    15709 2020-02-02 00:00:00.000000 robotcode_language_server-0.41.0/src/robotcode/language_server/robotframework/parts/signature_help.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 robotcode_language_server-0.41.0/src/robotcode/language_server/robotframework/utils/__init__.py
+-rw-r--r--   0        0        0     1722 2020-02-02 00:00:00.000000 robotcode_language_server-0.41.0/src/robotcode/language_server/robotframework/utils/_variables.py
+-rw-r--r--   0        0        0     7957 2020-02-02 00:00:00.000000 robotcode_language_server-0.41.0/src/robotcode/language_server/robotframework/utils/ast_utils.py
+-rw-r--r--   0        0        0     3163 2020-02-02 00:00:00.000000 robotcode_language_server-0.41.0/src/robotcode/language_server/robotframework/utils/async_ast.py
+-rw-r--r--   0        0        0    11653 2020-02-02 00:00:00.000000 robotcode_language_server-0.41.0/src/robotcode/language_server/robotframework/utils/markdownformatter.py
+-rw-r--r--   0        0        0      268 2020-02-02 00:00:00.000000 robotcode_language_server-0.41.0/src/robotcode/language_server/robotframework/utils/match.py
+-rw-r--r--   0        0        0     1739 2020-02-02 00:00:00.000000 robotcode_language_server-0.41.0/src/robotcode/language_server/robotframework/utils/robot_path.py
+-rw-r--r--   0        0        0     1357 2020-02-02 00:00:00.000000 robotcode_language_server-0.41.0/src/robotcode/language_server/robotframework/utils/variables.py
+-rw-r--r--   0        0        0      482 2020-02-02 00:00:00.000000 robotcode_language_server-0.41.0/src/robotcode/language_server/robotframework/utils/version.py
+-rw-r--r--   0        0        0     4277 2020-02-02 00:00:00.000000 robotcode_language_server-0.41.0/.gitignore
+-rw-r--r--   0        0        0    10280 2020-02-02 00:00:00.000000 robotcode_language_server-0.41.0/LICENSE.txt
+-rw-r--r--   0        0        0      765 2020-02-02 00:00:00.000000 robotcode_language_server-0.41.0/README.md
+-rw-r--r--   0        0        0     1799 2020-02-02 00:00:00.000000 robotcode_language_server-0.41.0/pyproject.toml
+-rw-r--r--   0        0        0     2185 2020-02-02 00:00:00.000000 robotcode_language_server-0.41.0/PKG-INFO
```

### Comparing `robotcode_language_server-0.40.0/src/robotcode/language_server/cli.py` & `robotcode_language_server-0.41.0/src/robotcode/language_server/cli.py`

 * *Files identical despite different names*

### Comparing `robotcode_language_server-0.40.0/src/robotcode/language_server/common/decorators.py` & `robotcode_language_server-0.41.0/src/robotcode/language_server/common/decorators.py`

 * *Files identical despite different names*

### Comparing `robotcode_language_server-0.40.0/src/robotcode/language_server/common/protocol.py` & `robotcode_language_server-0.41.0/src/robotcode/language_server/common/protocol.py`

 * *Files identical despite different names*

### Comparing `robotcode_language_server-0.40.0/src/robotcode/language_server/common/server.py` & `robotcode_language_server-0.41.0/src/robotcode/language_server/common/server.py`

 * *Files identical despite different names*

### Comparing `robotcode_language_server-0.40.0/src/robotcode/language_server/common/text_document.py` & `robotcode_language_server-0.41.0/src/robotcode/language_server/common/text_document.py`

 * *Files identical despite different names*

### Comparing `robotcode_language_server-0.40.0/src/robotcode/language_server/common/parts/code_action.py` & `robotcode_language_server-0.41.0/src/robotcode/language_server/common/parts/code_action.py`

 * *Files identical despite different names*

### Comparing `robotcode_language_server-0.40.0/src/robotcode/language_server/common/parts/code_lens.py` & `robotcode_language_server-0.41.0/src/robotcode/language_server/common/parts/code_lens.py`

 * *Files identical despite different names*

### Comparing `robotcode_language_server-0.40.0/src/robotcode/language_server/common/parts/commands.py` & `robotcode_language_server-0.41.0/src/robotcode/language_server/common/parts/commands.py`

 * *Files identical despite different names*

### Comparing `robotcode_language_server-0.40.0/src/robotcode/language_server/common/parts/completion.py` & `robotcode_language_server-0.41.0/src/robotcode/language_server/common/parts/completion.py`

 * *Files identical despite different names*

### Comparing `robotcode_language_server-0.40.0/src/robotcode/language_server/common/parts/declaration.py` & `robotcode_language_server-0.41.0/src/robotcode/language_server/common/parts/declaration.py`

 * *Files identical despite different names*

### Comparing `robotcode_language_server-0.40.0/src/robotcode/language_server/common/parts/definition.py` & `robotcode_language_server-0.41.0/src/robotcode/language_server/common/parts/definition.py`

 * *Files identical despite different names*

### Comparing `robotcode_language_server-0.40.0/src/robotcode/language_server/common/parts/diagnostics.py` & `robotcode_language_server-0.41.0/src/robotcode/language_server/common/parts/diagnostics.py`

 * *Files identical despite different names*

### Comparing `robotcode_language_server-0.40.0/src/robotcode/language_server/common/parts/document_highlight.py` & `robotcode_language_server-0.41.0/src/robotcode/language_server/common/parts/document_highlight.py`

 * *Files identical despite different names*

### Comparing `robotcode_language_server-0.40.0/src/robotcode/language_server/common/parts/document_symbols.py` & `robotcode_language_server-0.41.0/src/robotcode/language_server/common/parts/document_symbols.py`

 * *Files identical despite different names*

### Comparing `robotcode_language_server-0.40.0/src/robotcode/language_server/common/parts/documents.py` & `robotcode_language_server-0.41.0/src/robotcode/language_server/common/parts/documents.py`

 * *Files identical despite different names*

### Comparing `robotcode_language_server-0.40.0/src/robotcode/language_server/common/parts/folding_range.py` & `robotcode_language_server-0.41.0/src/robotcode/language_server/common/parts/folding_range.py`

 * *Files identical despite different names*

### Comparing `robotcode_language_server-0.40.0/src/robotcode/language_server/common/parts/formatting.py` & `robotcode_language_server-0.41.0/src/robotcode/language_server/common/parts/formatting.py`

 * *Files identical despite different names*

### Comparing `robotcode_language_server-0.40.0/src/robotcode/language_server/common/parts/hover.py` & `robotcode_language_server-0.41.0/src/robotcode/language_server/common/parts/hover.py`

 * *Files identical despite different names*

### Comparing `robotcode_language_server-0.40.0/src/robotcode/language_server/common/parts/implementation.py` & `robotcode_language_server-0.41.0/src/robotcode/language_server/common/parts/implementation.py`

 * *Files identical despite different names*

### Comparing `robotcode_language_server-0.40.0/src/robotcode/language_server/common/parts/inlay_hint.py` & `robotcode_language_server-0.41.0/src/robotcode/language_server/common/parts/inlay_hint.py`

 * *Files identical despite different names*

### Comparing `robotcode_language_server-0.40.0/src/robotcode/language_server/common/parts/inline_value.py` & `robotcode_language_server-0.41.0/src/robotcode/language_server/common/parts/inline_value.py`

 * *Files identical despite different names*

### Comparing `robotcode_language_server-0.40.0/src/robotcode/language_server/common/parts/linked_editing_ranges.py` & `robotcode_language_server-0.41.0/src/robotcode/language_server/common/parts/linked_editing_ranges.py`

 * *Files identical despite different names*

### Comparing `robotcode_language_server-0.40.0/src/robotcode/language_server/common/parts/references.py` & `robotcode_language_server-0.41.0/src/robotcode/language_server/common/parts/references.py`

 * *Files identical despite different names*

### Comparing `robotcode_language_server-0.40.0/src/robotcode/language_server/common/parts/rename.py` & `robotcode_language_server-0.41.0/src/robotcode/language_server/common/parts/rename.py`

 * *Files identical despite different names*

### Comparing `robotcode_language_server-0.40.0/src/robotcode/language_server/common/parts/selection_range.py` & `robotcode_language_server-0.41.0/src/robotcode/language_server/common/parts/selection_range.py`

 * *Files identical despite different names*

### Comparing `robotcode_language_server-0.40.0/src/robotcode/language_server/common/parts/semantic_tokens.py` & `robotcode_language_server-0.41.0/src/robotcode/language_server/common/parts/semantic_tokens.py`

 * *Files identical despite different names*

### Comparing `robotcode_language_server-0.40.0/src/robotcode/language_server/common/parts/signature_help.py` & `robotcode_language_server-0.41.0/src/robotcode/language_server/common/parts/signature_help.py`

 * *Files identical despite different names*

### Comparing `robotcode_language_server-0.40.0/src/robotcode/language_server/common/parts/window.py` & `robotcode_language_server-0.41.0/src/robotcode/language_server/common/parts/window.py`

 * *Files identical despite different names*

### Comparing `robotcode_language_server-0.40.0/src/robotcode/language_server/common/parts/workspace.py` & `robotcode_language_server-0.41.0/src/robotcode/language_server/common/parts/workspace.py`

 * *Files identical despite different names*

### Comparing `robotcode_language_server-0.40.0/src/robotcode/language_server/robotframework/configuration.py` & `robotcode_language_server-0.41.0/src/robotcode/language_server/robotframework/configuration.py`

 * *Files 1% similar despite different names*

```diff
@@ -67,14 +67,16 @@
     configurations: List[str] = field(default_factory=list)
 
 
 @config_section("robotcode.robotidy")
 @dataclass
 class RoboTidyConfig(ConfigBase):
     enabled: bool = True
+    ignore_git_dir: bool = False
+    config: Optional[str] = None
 
 
 @config_section("robotcode.workspace")
 @dataclass
 class WorkspaceConfig(ConfigBase):
     exclude_patterns: List[str] = field(default_factory=list)
```

### Comparing `robotcode_language_server-0.40.0/src/robotcode/language_server/robotframework/protocol.py` & `robotcode_language_server-0.41.0/src/robotcode/language_server/robotframework/protocol.py`

 * *Files identical despite different names*

### Comparing `robotcode_language_server-0.40.0/src/robotcode/language_server/robotframework/server.py` & `robotcode_language_server-0.41.0/src/robotcode/language_server/robotframework/server.py`

 * *Files identical despite different names*

### Comparing `robotcode_language_server-0.40.0/src/robotcode/language_server/robotframework/diagnostics/analyzer.py` & `robotcode_language_server-0.41.0/src/robotcode/language_server/robotframework/diagnostics/analyzer.py`

 * *Files identical despite different names*

### Comparing `robotcode_language_server-0.40.0/src/robotcode/language_server/robotframework/diagnostics/entities.py` & `robotcode_language_server-0.41.0/src/robotcode/language_server/robotframework/diagnostics/entities.py`

 * *Files identical despite different names*

### Comparing `robotcode_language_server-0.40.0/src/robotcode/language_server/robotframework/diagnostics/imports_manager.py` & `robotcode_language_server-0.41.0/src/robotcode/language_server/robotframework/diagnostics/imports_manager.py`

 * *Files identical despite different names*

### Comparing `robotcode_language_server-0.40.0/src/robotcode/language_server/robotframework/diagnostics/library_doc.py` & `robotcode_language_server-0.41.0/src/robotcode/language_server/robotframework/diagnostics/library_doc.py`

 * *Files identical despite different names*

### Comparing `robotcode_language_server-0.40.0/src/robotcode/language_server/robotframework/diagnostics/namespace.py` & `robotcode_language_server-0.41.0/src/robotcode/language_server/robotframework/diagnostics/namespace.py`

 * *Files identical despite different names*

### Comparing `robotcode_language_server-0.40.0/src/robotcode/language_server/robotframework/parts/code_action_documentation.py` & `robotcode_language_server-0.41.0/src/robotcode/language_server/robotframework/parts/code_action_documentation.py`

 * *Files identical despite different names*

### Comparing `robotcode_language_server-0.40.0/src/robotcode/language_server/robotframework/parts/code_action_fixes.py` & `robotcode_language_server-0.41.0/src/robotcode/language_server/robotframework/parts/code_action_fixes.py`

 * *Files identical despite different names*

### Comparing `robotcode_language_server-0.40.0/src/robotcode/language_server/robotframework/parts/codelens.py` & `robotcode_language_server-0.41.0/src/robotcode/language_server/robotframework/parts/codelens.py`

 * *Files identical despite different names*

### Comparing `robotcode_language_server-0.40.0/src/robotcode/language_server/robotframework/parts/completion.py` & `robotcode_language_server-0.41.0/src/robotcode/language_server/robotframework/parts/completion.py`

 * *Files identical despite different names*

### Comparing `robotcode_language_server-0.40.0/src/robotcode/language_server/robotframework/parts/debugging_utils.py` & `robotcode_language_server-0.41.0/src/robotcode/language_server/robotframework/parts/debugging_utils.py`

 * *Files identical despite different names*

### Comparing `robotcode_language_server-0.40.0/src/robotcode/language_server/robotframework/parts/diagnostics.py` & `robotcode_language_server-0.41.0/src/robotcode/language_server/robotframework/parts/diagnostics.py`

 * *Files identical despite different names*

### Comparing `robotcode_language_server-0.40.0/src/robotcode/language_server/robotframework/parts/document_highlight.py` & `robotcode_language_server-0.41.0/src/robotcode/language_server/robotframework/parts/document_highlight.py`

 * *Files identical despite different names*

### Comparing `robotcode_language_server-0.40.0/src/robotcode/language_server/robotframework/parts/document_symbols.py` & `robotcode_language_server-0.41.0/src/robotcode/language_server/robotframework/parts/document_symbols.py`

 * *Files identical despite different names*

### Comparing `robotcode_language_server-0.40.0/src/robotcode/language_server/robotframework/parts/documents_cache.py` & `robotcode_language_server-0.41.0/src/robotcode/language_server/robotframework/parts/documents_cache.py`

 * *Files identical despite different names*

### Comparing `robotcode_language_server-0.40.0/src/robotcode/language_server/robotframework/parts/folding_range.py` & `robotcode_language_server-0.41.0/src/robotcode/language_server/robotframework/parts/folding_range.py`

 * *Files identical despite different names*

### Comparing `robotcode_language_server-0.40.0/src/robotcode/language_server/robotframework/parts/formatting.py` & `robotcode_language_server-0.41.0/src/robotcode/language_server/robotframework/parts/formatting.py`

 * *Files 7% similar despite different names*

```diff
@@ -51,34 +51,34 @@
 
         self.space_count = 4
         self.use_pipes = False
         self.line_separator = os.linesep
         self.short_test_name_length = 18
         self.setting_and_variable_name_length = 14
 
-    async def get_config(self, document: TextDocument) -> Optional[RoboTidyConfig]:
+    async def get_config(self, document: TextDocument) -> RoboTidyConfig:
         folder = self.parent.workspace.get_workspace_folder(document.uri)
         if folder is None:
-            return None
+            return RoboTidyConfig()
 
         return await self.parent.workspace.get_configuration(RoboTidyConfig, folder.uri)
 
     @language_id("robotframework")
     @_logger.call
     async def format(
         self,
         sender: Any,
         document: TextDocument,
         options: FormattingOptions,
         **further_options: Any,
     ) -> Optional[List[TextEdit]]:
         config = await self.get_config(document)
 
-        if config and (config.enabled or get_robot_version() >= (5, 0)) and robotidy_installed():
-            return await self.format_robot_tidy(document, options, **further_options)
+        if (config.enabled or get_robot_version() >= (5, 0)) and robotidy_installed():
+            return await self.format_robot_tidy(document, options, config=config, **further_options)
 
         if get_robot_version() < (5, 0):
             return await self.format_internal(document, options, **further_options)
 
         self.parent.window.show_message(
             "RobotFramework formatter is not available, please install 'robotframework-tidy'.",
             MessageType.ERROR,
@@ -89,28 +89,46 @@
     RE_LINEBREAKS = re.compile(r"\r\n|\r|\n")
 
     async def format_robot_tidy(
         self,
         document: TextDocument,
         options: FormattingOptions,
         range: Optional[Range] = None,
+        config: Optional[RoboTidyConfig] = None,
         **further_options: Any,
     ) -> Optional[List[TextEdit]]:
         from robotidy.version import __version__
 
         try:
+            if config is None:
+                config = await self.get_config(document)
+
             robotidy_version = create_version_from_str(__version__)
 
             model = await self.parent.documents_cache.get_model(document, False)
 
             if robotidy_version >= (3, 0):
                 from robotidy.api import get_robotidy
                 from robotidy.disablers import RegisterDisablers
 
-                robot_tidy = get_robotidy(document.uri.to_path(), None)
+                if robotidy_version >= (4, 2):
+                    robot_tidy = get_robotidy(
+                        document.uri.to_path(),
+                        None,
+                        ignore_git_dir=config.ignore_git_dir,
+                        config=config.config,
+                    )
+                elif robotidy_version >= (4, 1):
+                    robot_tidy = get_robotidy(
+                        document.uri.to_path(),
+                        None,
+                        ignore_git_dir=config.ignore_git_dir,
+                    )
+                else:
+                    robot_tidy = get_robotidy(document.uri.to_path(), None)
 
                 if range is not None:
                     robot_tidy.config.formatting.start_line = range.start.line + 1
                     robot_tidy.config.formatting.end_line = range.end.line + 1
 
                 disabler_finder = RegisterDisablers(
                     robot_tidy.config.formatting.start_line,
@@ -164,14 +182,15 @@
                 )
             ]
 
         except (SystemExit, KeyboardInterrupt, asyncio.CancelledError):
             raise
         except BaseException as e:
             self._logger.exception(e)
+            self.parent.window.show_message(f"Executing `robotidy` failed: {e}", MessageType.ERROR)
         return None
 
     async def format_internal(
         self, document: TextDocument, options: FormattingOptions, **further_options: Any
     ) -> Optional[List[TextEdit]]:
         from robot.parsing.model.blocks import File
         from robot.tidypkg import (  # pyright: ignore [reportMissingImports]
@@ -214,11 +233,11 @@
         sender: Any,
         document: TextDocument,
         range: Range,
         options: FormattingOptions,
         **further_options: Any,
     ) -> Optional[List[TextEdit]]:
         config = await self.get_config(document)
-        if config and config.enabled and robotidy_installed():
-            return await self.format_robot_tidy(document, options, range=range, **further_options)
+        if config.enabled and robotidy_installed():
+            return await self.format_robot_tidy(document, options, range=range, config=config, **further_options)
 
         return None
```

### Comparing `robotcode_language_server-0.40.0/src/robotcode/language_server/robotframework/parts/goto.py` & `robotcode_language_server-0.41.0/src/robotcode/language_server/robotframework/parts/goto.py`

 * *Files identical despite different names*

### Comparing `robotcode_language_server-0.40.0/src/robotcode/language_server/robotframework/parts/hover.py` & `robotcode_language_server-0.41.0/src/robotcode/language_server/robotframework/parts/hover.py`

 * *Files identical despite different names*

### Comparing `robotcode_language_server-0.40.0/src/robotcode/language_server/robotframework/parts/inlay_hint.py` & `robotcode_language_server-0.41.0/src/robotcode/language_server/robotframework/parts/inlay_hint.py`

 * *Files identical despite different names*

### Comparing `robotcode_language_server-0.40.0/src/robotcode/language_server/robotframework/parts/inline_value.py` & `robotcode_language_server-0.41.0/src/robotcode/language_server/robotframework/parts/inline_value.py`

 * *Files identical despite different names*

### Comparing `robotcode_language_server-0.40.0/src/robotcode/language_server/robotframework/parts/model_helper.py` & `robotcode_language_server-0.41.0/src/robotcode/language_server/robotframework/parts/model_helper.py`

 * *Files identical despite different names*

### Comparing `robotcode_language_server-0.40.0/src/robotcode/language_server/robotframework/parts/references.py` & `robotcode_language_server-0.41.0/src/robotcode/language_server/robotframework/parts/references.py`

 * *Files identical despite different names*

### Comparing `robotcode_language_server-0.40.0/src/robotcode/language_server/robotframework/parts/rename.py` & `robotcode_language_server-0.41.0/src/robotcode/language_server/robotframework/parts/rename.py`

 * *Files identical despite different names*

### Comparing `robotcode_language_server-0.40.0/src/robotcode/language_server/robotframework/parts/robocop_diagnostics.py` & `robotcode_language_server-0.41.0/src/robotcode/language_server/robotframework/parts/robocop_diagnostics.py`

 * *Files identical despite different names*

### Comparing `robotcode_language_server-0.40.0/src/robotcode/language_server/robotframework/parts/robot_workspace.py` & `robotcode_language_server-0.41.0/src/robotcode/language_server/robotframework/parts/robot_workspace.py`

 * *Files identical despite different names*

### Comparing `robotcode_language_server-0.40.0/src/robotcode/language_server/robotframework/parts/selection_range.py` & `robotcode_language_server-0.41.0/src/robotcode/language_server/robotframework/parts/selection_range.py`

 * *Files identical despite different names*

### Comparing `robotcode_language_server-0.40.0/src/robotcode/language_server/robotframework/parts/semantic_tokens.py` & `robotcode_language_server-0.41.0/src/robotcode/language_server/robotframework/parts/semantic_tokens.py`

 * *Files identical despite different names*

### Comparing `robotcode_language_server-0.40.0/src/robotcode/language_server/robotframework/parts/signature_help.py` & `robotcode_language_server-0.41.0/src/robotcode/language_server/robotframework/parts/signature_help.py`

 * *Files identical despite different names*

### Comparing `robotcode_language_server-0.40.0/src/robotcode/language_server/robotframework/utils/_variables.py` & `robotcode_language_server-0.41.0/src/robotcode/language_server/robotframework/utils/_variables.py`

 * *Files identical despite different names*

### Comparing `robotcode_language_server-0.40.0/src/robotcode/language_server/robotframework/utils/ast_utils.py` & `robotcode_language_server-0.41.0/src/robotcode/language_server/robotframework/utils/ast_utils.py`

 * *Files identical despite different names*

### Comparing `robotcode_language_server-0.40.0/src/robotcode/language_server/robotframework/utils/async_ast.py` & `robotcode_language_server-0.41.0/src/robotcode/language_server/robotframework/utils/async_ast.py`

 * *Files identical despite different names*

### Comparing `robotcode_language_server-0.40.0/src/robotcode/language_server/robotframework/utils/markdownformatter.py` & `robotcode_language_server-0.41.0/src/robotcode/language_server/robotframework/utils/markdownformatter.py`

 * *Files identical despite different names*

### Comparing `robotcode_language_server-0.40.0/src/robotcode/language_server/robotframework/utils/robot_path.py` & `robotcode_language_server-0.41.0/src/robotcode/language_server/robotframework/utils/robot_path.py`

 * *Files identical despite different names*

### Comparing `robotcode_language_server-0.40.0/src/robotcode/language_server/robotframework/utils/variables.py` & `robotcode_language_server-0.41.0/src/robotcode/language_server/robotframework/utils/variables.py`

 * *Files identical despite different names*

### Comparing `robotcode_language_server-0.40.0/.gitignore` & `robotcode_language_server-0.41.0/.gitignore`

 * *Files identical despite different names*

### Comparing `robotcode_language_server-0.40.0/LICENSE.txt` & `robotcode_language_server-0.41.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `robotcode_language_server-0.40.0/README.md` & `robotcode_language_server-0.41.0/README.md`

 * *Files identical despite different names*

### Comparing `robotcode_language_server-0.40.0/pyproject.toml` & `robotcode_language_server-0.41.0/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -23,16 +23,16 @@
   "Topic :: Utilities",
   "Typing :: Typed",
   "Framework :: Robot Framework",
   "Framework :: Robot Framework :: Tool",
 ]
 dependencies = [
   "robotframework>=4.1.0",
-  "robotcode-jsonrpc2==0.40.0",
-  "robotcode==0.40.0",
+  "robotcode-jsonrpc2==0.41.0",
+  "robotcode==0.41.0",
 ]
 dynamic = ["version"]
 
 [project.entry-points.robotcode]
 langserver = "robotcode.language_server.hooks"
 
 [project.urls]
```

### Comparing `robotcode_language_server-0.40.0/PKG-INFO` & `robotcode_language_server-0.41.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: robotcode-language-server
-Version: 0.40.0
+Version: 0.41.0
 Summary: RobotCode Language Server for Robot Framework
 Project-URL: Homepage, https://robotcode.io
 Project-URL: Donate, https://github.com/sponsors/d-biehl
 Project-URL: Documentation, https://github.com/d-biehl/robotcode#readme
 Project-URL: Changelog, https://github.com/d-biehl/robotcode/blob/main/CHANGELOG.md
 Project-URL: Issues, https://github.com/d-biehl/robotcode/issues
 Project-URL: Source, https://github.com/d-biehl/robotcode
@@ -21,16 +21,16 @@
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Classifier: Topic :: Utilities
 Classifier: Typing :: Typed
 Requires-Python: >=3.8
-Requires-Dist: robotcode-jsonrpc2==0.40.0
-Requires-Dist: robotcode==0.40.0
+Requires-Dist: robotcode-jsonrpc2==0.41.0
+Requires-Dist: robotcode==0.41.0
 Requires-Dist: robotframework>=4.1.0
 Description-Content-Type: text/markdown
 
 # robotcode-language-server
 
 [![PyPI - Version](https://img.shields.io/pypi/v/robotcode-language-server.svg)](https://pypi.org/project/robotcode-language-server)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/robotcode-language-server.svg)](https://pypi.org/project/robotcode-language-server)
```

