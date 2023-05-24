# Comparing `tmp/cercis-0.1.5.tar.gz` & `tmp/cercis-0.1.6.tar.gz`

## Comparing `cercis-0.1.5.tar` & `cercis-0.1.6.tar`

### file list

```diff
@@ -1,362 +1,373 @@
--rw-r--r--   0        0        0      106 2020-02-02 00:00:00.000000 cercis-0.1.5/.coveragerc
--rw-r--r--   0        0        0      360 2020-02-02 00:00:00.000000 cercis-0.1.5/.flake8
--rw-r--r--   0        0        0      125 2020-02-02 00:00:00.000000 cercis-0.1.5/.git_archival.txt
--rw-r--r--   0        0        0       32 2020-02-02 00:00:00.000000 cercis-0.1.5/.gitattributes
--rw-r--r--   0        0        0     1250 2020-02-02 00:00:00.000000 cercis-0.1.5/.pre-commit-config.yaml
--rw-r--r--   0        0        0      533 2020-02-02 00:00:00.000000 cercis-0.1.5/.pre-commit-hooks.yaml
--rw-r--r--   0        0        0       49 2020-02-02 00:00:00.000000 cercis-0.1.5/.prettierrc.yaml
--rw-r--r--   0        0        0      220 2020-02-02 00:00:00.000000 cercis-0.1.5/.readthedocs.yaml
--rw-r--r--   0        0        0     1854 2020-02-02 00:00:00.000000 cercis-0.1.5/CHANGELOG.md
--rw-r--r--   0        0        0      587 2020-02-02 00:00:00.000000 cercis-0.1.5/Dockerfile
--rw-r--r--   0        0        0    21217 2020-02-02 00:00:00.000000 cercis-0.1.5/README.md
--rw-r--r--   0        0        0     1540 2020-02-02 00:00:00.000000 cercis-0.1.5/action.yml
--rw-r--r--   0        0        0      796 2020-02-02 00:00:00.000000 cercis-0.1.5/mypy.ini
--rw-r--r--   0        0        0       99 2020-02-02 00:00:00.000000 cercis-0.1.5/test_requirements.txt
--rw-r--r--   0        0        0     2972 2020-02-02 00:00:00.000000 cercis-0.1.5/tox.ini
--rw-r--r--   0        0        0     1537 2020-02-02 00:00:00.000000 cercis-0.1.5/.github/PULL_REQUEST_TEMPLATE.md
--rw-r--r--   0        0        0      565 2020-02-02 00:00:00.000000 cercis-0.1.5/.github/dependabot.yml
--rw-r--r--   0        0        0     1557 2020-02-02 00:00:00.000000 cercis-0.1.5/.github/ISSUE_TEMPLATE/bug_report.md
--rw-r--r--   0        0        0      545 2020-02-02 00:00:00.000000 cercis-0.1.5/.github/ISSUE_TEMPLATE/config.yml
--rw-r--r--   0        0        0      692 2020-02-02 00:00:00.000000 cercis-0.1.5/.github/ISSUE_TEMPLATE/docs-issue.md
--rw-r--r--   0        0        0      649 2020-02-02 00:00:00.000000 cercis-0.1.5/.github/ISSUE_TEMPLATE/feature_request.md
--rw-r--r--   0        0        0      646 2020-02-02 00:00:00.000000 cercis-0.1.5/.github/ISSUE_TEMPLATE/style_issue.md
--rw-r--r--   0        0        0      795 2020-02-02 00:00:00.000000 cercis-0.1.5/.github/workflows/check-changelog.yml
--rw-r--r--   0        0        0     1894 2020-02-02 00:00:00.000000 cercis-0.1.5/.github/workflows/docker.yml
--rw-r--r--   0        0        0     1127 2020-02-02 00:00:00.000000 cercis-0.1.5/.github/workflows/fuzz.yml
--rw-r--r--   0        0        0     1232 2020-02-02 00:00:00.000000 cercis-0.1.5/.github/workflows/lint.yml
--rw-r--r--   0        0        0      811 2020-02-02 00:00:00.000000 cercis-0.1.5/.github/workflows/python-package.yml
--rw-r--r--   0        0        0     1253 2020-02-02 00:00:00.000000 cercis-0.1.5/.github/workflows/python-publish.yml
--rw-r--r--   0        0        0     2998 2020-02-02 00:00:00.000000 cercis-0.1.5/.github/workflows/test.yml
--rw-r--r--   0        0        0     1910 2020-02-02 00:00:00.000000 cercis-0.1.5/.github/workflows/upload_binary.yml
--rw-r--r--   0        0        0      780 2020-02-02 00:00:00.000000 cercis-0.1.5/.github/workflows/version-check.yml
--rw-r--r--   0        0        0     2245 2020-02-02 00:00:00.000000 cercis-0.1.5/action/main.py
--rw-r--r--   0        0        0     7597 2020-02-02 00:00:00.000000 cercis-0.1.5/autoload/black.vim
--rw-r--r--   0        0        0      342 2020-02-02 00:00:00.000000 cercis-0.1.5/gallery/Dockerfile
--rw-r--r--   0        0        0     1595 2020-02-02 00:00:00.000000 cercis-0.1.5/gallery/README.md
--rwxr-xr-x   0        0        0     9123 2020-02-02 00:00:00.000000 cercis-0.1.5/gallery/gallery.py
--rw-r--r--   0        0        0     2176 2020-02-02 00:00:00.000000 cercis-0.1.5/plugin/black.vim
--rw-r--r--   0        0        0       55 2020-02-02 00:00:00.000000 cercis-0.1.5/scripts/README.md
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 cercis-0.1.5/scripts/__init__.py
--rw-r--r--   0        0        0     2500 2020-02-02 00:00:00.000000 cercis-0.1.5/scripts/check_version_and_changelog.py
--rw-r--r--   0        0        0     8650 2020-02-02 00:00:00.000000 cercis-0.1.5/scripts/diff_shades_gha_helper.py
--rw-r--r--   0        0        0     3527 2020-02-02 00:00:00.000000 cercis-0.1.5/scripts/fuzz.py
--rw-r--r--   0        0        0     2458 2020-02-02 00:00:00.000000 cercis-0.1.5/scripts/make_width_table.py
--rwxr-xr-x   0        0        0     2993 2020-02-02 00:00:00.000000 cercis-0.1.5/scripts/migrate-black.py
--rw-r--r--   0        0        0       18 2020-02-02 00:00:00.000000 cercis-0.1.5/src/_cercis_version.py
--rw-r--r--   0        0        0     8100 2020-02-02 00:00:00.000000 cercis-0.1.5/src/blackd/__init__.py
--rw-r--r--   0        0        0       37 2020-02-02 00:00:00.000000 cercis-0.1.5/src/blackd/__main__.py
--rw-r--r--   0        0        0     1585 2020-02-02 00:00:00.000000 cercis-0.1.5/src/blackd/middlewares.py
--rw-r--r--   0        0        0    11278 2020-02-02 00:00:00.000000 cercis-0.1.5/src/blib2to3/Grammar.txt
--rw-r--r--   0        0        0    12762 2020-02-02 00:00:00.000000 cercis-0.1.5/src/blib2to3/LICENSE
--rw-r--r--   0        0        0      793 2020-02-02 00:00:00.000000 cercis-0.1.5/src/blib2to3/PatternGrammar.txt
--rw-r--r--   0        0        0     1071 2020-02-02 00:00:00.000000 cercis-0.1.5/src/blib2to3/README
--rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 cercis-0.1.5/src/blib2to3/__init__.py
--rw-r--r--   0        0        0     5732 2020-02-02 00:00:00.000000 cercis-0.1.5/src/blib2to3/pygram.py
--rw-r--r--   0        0        0    32612 2020-02-02 00:00:00.000000 cercis-0.1.5/src/blib2to3/pytree.py
--rw-r--r--   0        0        0      143 2020-02-02 00:00:00.000000 cercis-0.1.5/src/blib2to3/pgen2/__init__.py
--rw-r--r--   0        0        0     9607 2020-02-02 00:00:00.000000 cercis-0.1.5/src/blib2to3/pgen2/conv.py
--rw-r--r--   0        0        0    10671 2020-02-02 00:00:00.000000 cercis-0.1.5/src/blib2to3/pgen2/driver.py
--rw-r--r--   0        0        0     6873 2020-02-02 00:00:00.000000 cercis-0.1.5/src/blib2to3/pgen2/grammar.py
--rw-r--r--   0        0        0     1628 2020-02-02 00:00:00.000000 cercis-0.1.5/src/blib2to3/pgen2/literals.py
--rw-r--r--   0        0        0    14859 2020-02-02 00:00:00.000000 cercis-0.1.5/src/blib2to3/pgen2/parse.py
--rw-r--r--   0        0        0    15491 2020-02-02 00:00:00.000000 cercis-0.1.5/src/blib2to3/pgen2/pgen.py
--rw-r--r--   0        0        0     1919 2020-02-02 00:00:00.000000 cercis-0.1.5/src/blib2to3/pgen2/token.py
--rw-r--r--   0        0        0    23120 2020-02-02 00:00:00.000000 cercis-0.1.5/src/blib2to3/pgen2/tokenize.py
--rw-r--r--   0        0        0    51483 2020-02-02 00:00:00.000000 cercis-0.1.5/src/cercis/__init__.py
--rw-r--r--   0        0        0       48 2020-02-02 00:00:00.000000 cercis-0.1.5/src/cercis/__main__.py
--rw-r--r--   0        0        0    10871 2020-02-02 00:00:00.000000 cercis-0.1.5/src/cercis/_width_table.py
--rw-r--r--   0        0        0    12274 2020-02-02 00:00:00.000000 cercis-0.1.5/src/cercis/brackets.py
--rw-r--r--   0        0        0     2952 2020-02-02 00:00:00.000000 cercis-0.1.5/src/cercis/cache.py
--rw-r--r--   0        0        0    12797 2020-02-02 00:00:00.000000 cercis-0.1.5/src/cercis/comments.py
--rw-r--r--   0        0        0     6343 2020-02-02 00:00:00.000000 cercis-0.1.5/src/cercis/concurrency.py
--rw-r--r--   0        0        0      661 2020-02-02 00:00:00.000000 cercis-0.1.5/src/cercis/const.py
--rw-r--r--   0        0        0     1597 2020-02-02 00:00:00.000000 cercis-0.1.5/src/cercis/debug.py
--rw-r--r--   0        0        0    13538 2020-02-02 00:00:00.000000 cercis-0.1.5/src/cercis/files.py
--rw-r--r--   0        0        0    13514 2020-02-02 00:00:00.000000 cercis-0.1.5/src/cercis/handle_ipynb_magics.py
--rw-r--r--   0        0        0     4612 2020-02-02 00:00:00.000000 cercis-0.1.5/src/cercis/indent.py
--rw-r--r--   0        0        0    62861 2020-02-02 00:00:00.000000 cercis-0.1.5/src/cercis/linegen.py
--rw-r--r--   0        0        0    39809 2020-02-02 00:00:00.000000 cercis-0.1.5/src/cercis/lines.py
--rw-r--r--   0        0        0     8223 2020-02-02 00:00:00.000000 cercis-0.1.5/src/cercis/mode.py
--rw-r--r--   0        0        0    25731 2020-02-02 00:00:00.000000 cercis-0.1.5/src/cercis/nodes.py
--rw-r--r--   0        0        0     1653 2020-02-02 00:00:00.000000 cercis-0.1.5/src/cercis/numerics.py
--rw-r--r--   0        0        0     3486 2020-02-02 00:00:00.000000 cercis-0.1.5/src/cercis/output.py
--rw-r--r--   0        0        0    10164 2020-02-02 00:00:00.000000 cercis-0.1.5/src/cercis/parsing.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 cercis-0.1.5/src/cercis/py.typed
--rw-r--r--   0        0        0     3452 2020-02-02 00:00:00.000000 cercis-0.1.5/src/cercis/report.py
--rw-r--r--   0        0        0      556 2020-02-02 00:00:00.000000 cercis-0.1.5/src/cercis/rusty.py
--rw-r--r--   0        0        0    14304 2020-02-02 00:00:00.000000 cercis-0.1.5/src/cercis/strings.py
--rw-r--r--   0        0        0    91890 2020-02-02 00:00:00.000000 cercis-0.1.5/src/cercis/trans.py
--rw-r--r--   0        0        0     2676 2020-02-02 00:00:00.000000 cercis-0.1.5/src/cercis/utils_line_wrapping.py
--rw-r--r--   0        0        0     3267 2020-02-02 00:00:00.000000 cercis-0.1.5/src/cercis/utils_linegen.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 cercis-0.1.5/tests/__init__.py
--rw-r--r--   0        0        0       36 2020-02-02 00:00:00.000000 cercis-0.1.5/tests/conftest.py
--rw-r--r--   0        0        0       89 2020-02-02 00:00:00.000000 cercis-0.1.5/tests/empty.toml
--rw-r--r--   0        0        0     4133 2020-02-02 00:00:00.000000 cercis-0.1.5/tests/optional.py
--rw-r--r--   0        0        0      389 2020-02-02 00:00:00.000000 cercis-0.1.5/tests/test.toml
--rw-r--r--   0        0        0   101263 2020-02-02 00:00:00.000000 cercis-0.1.5/tests/test_black.py
--rw-r--r--   0        0        0     9188 2020-02-02 00:00:00.000000 cercis-0.1.5/tests/test_blackd.py
--rw-r--r--   0        0        0    14908 2020-02-02 00:00:00.000000 cercis-0.1.5/tests/test_format.py
--rw-r--r--   0        0        0    16390 2020-02-02 00:00:00.000000 cercis-0.1.5/tests/test_ipynb.py
--rw-r--r--   0        0        0     1292 2020-02-02 00:00:00.000000 cercis-0.1.5/tests/test_no_ipynb.py
--rw-r--r--   0        0        0     2267 2020-02-02 00:00:00.000000 cercis-0.1.5/tests/test_trans.py
--rw-r--r--   0        0        0     2546 2020-02-02 00:00:00.000000 cercis-0.1.5/tests/test_utils_line_wrapping.py
--rw-r--r--   0        0        0     7023 2020-02-02 00:00:00.000000 cercis-0.1.5/tests/util.py
--rw-r--r--   0        0        0     4160 2020-02-02 00:00:00.000000 cercis-0.1.5/tests/data/conditional_expression.py
--rw-r--r--   0        0        0       99 2020-02-02 00:00:00.000000 cercis-0.1.5/tests/data/empty_pyproject.toml
--rw-r--r--   0        0        0     1611 2020-02-02 00:00:00.000000 cercis-0.1.5/tests/data/configurable_cases/closing_bracket_indent/extra_indent.py
--rw-r--r--   0        0        0     1563 2020-02-02 00:00:00.000000 cercis-0.1.5/tests/data/configurable_cases/closing_bracket_indent/no_extra_indent.py
--rw-r--r--   0        0        0     4438 2020-02-02 00:00:00.000000 cercis-0.1.5/tests/data/configurable_cases/func_def_indent/func_def_extra_indent.py
--rw-r--r--   0        0        0     4262 2020-02-02 00:00:00.000000 cercis-0.1.5/tests/data/configurable_cases/func_def_indent/func_def_no_extra_indent.py
--rw-r--r--   0        0        0     3449 2020-02-02 00:00:00.000000 cercis-0.1.5/tests/data/configurable_cases/indentation/use_spaces/closing_bracket_extra_indent/base_indent_spaces=1/fdei=False_olcei=False.py
--rw-r--r--   0        0        0     3482 2020-02-02 00:00:00.000000 cercis-0.1.5/tests/data/configurable_cases/indentation/use_spaces/closing_bracket_extra_indent/base_indent_spaces=1/fdei=False_olcei=True.py
--rw-r--r--   0        0        0     3502 2020-02-02 00:00:00.000000 cercis-0.1.5/tests/data/configurable_cases/indentation/use_spaces/closing_bracket_extra_indent/base_indent_spaces=1/fdei=True_olcei=False.py
--rw-r--r--   0        0        0     3535 2020-02-02 00:00:00.000000 cercis-0.1.5/tests/data/configurable_cases/indentation/use_spaces/closing_bracket_extra_indent/base_indent_spaces=1/fdei=True_olcei=True.py
--rw-r--r--   0        0        0     3680 2020-02-02 00:00:00.000000 cercis-0.1.5/tests/data/configurable_cases/indentation/use_spaces/closing_bracket_extra_indent/base_indent_spaces=2/fdei=False_olcei=False.py
--rw-r--r--   0        0        0     3747 2020-02-02 00:00:00.000000 cercis-0.1.5/tests/data/configurable_cases/indentation/use_spaces/closing_bracket_extra_indent/base_indent_spaces=2/fdei=False_olcei=True.py
--rw-r--r--   0        0        0     3787 2020-02-02 00:00:00.000000 cercis-0.1.5/tests/data/configurable_cases/indentation/use_spaces/closing_bracket_extra_indent/base_indent_spaces=2/fdei=True_olcei=False.py
--rw-r--r--   0        0        0     3854 2020-02-02 00:00:00.000000 cercis-0.1.5/tests/data/configurable_cases/indentation/use_spaces/closing_bracket_extra_indent/base_indent_spaces=2/fdei=True_olcei=True.py
--rw-r--r--   0        0        0     3911 2020-02-02 00:00:00.000000 cercis-0.1.5/tests/data/configurable_cases/indentation/use_spaces/closing_bracket_extra_indent/base_indent_spaces=3/fdei=False_olcei=False.py
--rw-r--r--   0        0        0     4012 2020-02-02 00:00:00.000000 cercis-0.1.5/tests/data/configurable_cases/indentation/use_spaces/closing_bracket_extra_indent/base_indent_spaces=3/fdei=False_olcei=True.py
--rw-r--r--   0        0        0     4072 2020-02-02 00:00:00.000000 cercis-0.1.5/tests/data/configurable_cases/indentation/use_spaces/closing_bracket_extra_indent/base_indent_spaces=3/fdei=True_olcei=False.py
--rw-r--r--   0        0        0     4173 2020-02-02 00:00:00.000000 cercis-0.1.5/tests/data/configurable_cases/indentation/use_spaces/closing_bracket_extra_indent/base_indent_spaces=3/fdei=True_olcei=True.py
--rw-r--r--   0        0        0     4142 2020-02-02 00:00:00.000000 cercis-0.1.5/tests/data/configurable_cases/indentation/use_spaces/closing_bracket_extra_indent/base_indent_spaces=4/fdei=False_olcei=False.py
--rw-r--r--   0        0        0     4277 2020-02-02 00:00:00.000000 cercis-0.1.5/tests/data/configurable_cases/indentation/use_spaces/closing_bracket_extra_indent/base_indent_spaces=4/fdei=False_olcei=True.py
--rw-r--r--   0        0        0     4357 2020-02-02 00:00:00.000000 cercis-0.1.5/tests/data/configurable_cases/indentation/use_spaces/closing_bracket_extra_indent/base_indent_spaces=4/fdei=True_olcei=False.py
--rw-r--r--   0        0        0     4492 2020-02-02 00:00:00.000000 cercis-0.1.5/tests/data/configurable_cases/indentation/use_spaces/closing_bracket_extra_indent/base_indent_spaces=4/fdei=True_olcei=True.py
--rw-r--r--   0        0        0     5066 2020-02-02 00:00:00.000000 cercis-0.1.5/tests/data/configurable_cases/indentation/use_spaces/closing_bracket_extra_indent/base_indent_spaces=8/fdei=False_olcei=False.py
--rw-r--r--   0        0        0     5337 2020-02-02 00:00:00.000000 cercis-0.1.5/tests/data/configurable_cases/indentation/use_spaces/closing_bracket_extra_indent/base_indent_spaces=8/fdei=False_olcei=True.py
--rw-r--r--   0        0        0     5497 2020-02-02 00:00:00.000000 cercis-0.1.5/tests/data/configurable_cases/indentation/use_spaces/closing_bracket_extra_indent/base_indent_spaces=8/fdei=True_olcei=False.py
--rw-r--r--   0        0        0     5768 2020-02-02 00:00:00.000000 cercis-0.1.5/tests/data/configurable_cases/indentation/use_spaces/closing_bracket_extra_indent/base_indent_spaces=8/fdei=True_olcei=True.py
--rw-r--r--   0        0        0     3434 2020-02-02 00:00:00.000000 cercis-0.1.5/tests/data/configurable_cases/indentation/use_spaces/closing_bracket_no_extra_indent/base_indent_spaces=1/fdei=False_olcei=False.py
--rw-r--r--   0        0        0     3462 2020-02-02 00:00:00.000000 cercis-0.1.5/tests/data/configurable_cases/indentation/use_spaces/closing_bracket_no_extra_indent/base_indent_spaces=1/fdei=False_olcei=True.py
--rw-r--r--   0        0        0     3477 2020-02-02 00:00:00.000000 cercis-0.1.5/tests/data/configurable_cases/indentation/use_spaces/closing_bracket_no_extra_indent/base_indent_spaces=1/fdei=True_olcei=False.py
--rw-r--r--   0        0        0     3505 2020-02-02 00:00:00.000000 cercis-0.1.5/tests/data/configurable_cases/indentation/use_spaces/closing_bracket_no_extra_indent/base_indent_spaces=1/fdei=True_olcei=True.py
--rw-r--r--   0        0        0     3650 2020-02-02 00:00:00.000000 cercis-0.1.5/tests/data/configurable_cases/indentation/use_spaces/closing_bracket_no_extra_indent/base_indent_spaces=2/fdei=False_olcei=False.py
--rw-r--r--   0        0        0     3707 2020-02-02 00:00:00.000000 cercis-0.1.5/tests/data/configurable_cases/indentation/use_spaces/closing_bracket_no_extra_indent/base_indent_spaces=2/fdei=False_olcei=True.py
--rw-r--r--   0        0        0     3737 2020-02-02 00:00:00.000000 cercis-0.1.5/tests/data/configurable_cases/indentation/use_spaces/closing_bracket_no_extra_indent/base_indent_spaces=2/fdei=True_olcei=False.py
--rw-r--r--   0        0        0     3794 2020-02-02 00:00:00.000000 cercis-0.1.5/tests/data/configurable_cases/indentation/use_spaces/closing_bracket_no_extra_indent/base_indent_spaces=2/fdei=True_olcei=True.py
--rw-r--r--   0        0        0     3866 2020-02-02 00:00:00.000000 cercis-0.1.5/tests/data/configurable_cases/indentation/use_spaces/closing_bracket_no_extra_indent/base_indent_spaces=3/fdei=False_olcei=False.py
--rw-r--r--   0        0        0     3952 2020-02-02 00:00:00.000000 cercis-0.1.5/tests/data/configurable_cases/indentation/use_spaces/closing_bracket_no_extra_indent/base_indent_spaces=3/fdei=False_olcei=True.py
--rw-r--r--   0        0        0     3997 2020-02-02 00:00:00.000000 cercis-0.1.5/tests/data/configurable_cases/indentation/use_spaces/closing_bracket_no_extra_indent/base_indent_spaces=3/fdei=True_olcei=False.py
--rw-r--r--   0        0        0     4083 2020-02-02 00:00:00.000000 cercis-0.1.5/tests/data/configurable_cases/indentation/use_spaces/closing_bracket_no_extra_indent/base_indent_spaces=3/fdei=True_olcei=True.py
--rw-r--r--   0        0        0     4082 2020-02-02 00:00:00.000000 cercis-0.1.5/tests/data/configurable_cases/indentation/use_spaces/closing_bracket_no_extra_indent/base_indent_spaces=4/fdei=False_olcei=False.py
--rw-r--r--   0        0        0     4197 2020-02-02 00:00:00.000000 cercis-0.1.5/tests/data/configurable_cases/indentation/use_spaces/closing_bracket_no_extra_indent/base_indent_spaces=4/fdei=False_olcei=True.py
--rw-r--r--   0        0        0     4257 2020-02-02 00:00:00.000000 cercis-0.1.5/tests/data/configurable_cases/indentation/use_spaces/closing_bracket_no_extra_indent/base_indent_spaces=4/fdei=True_olcei=False.py
--rw-r--r--   0        0        0     4372 2020-02-02 00:00:00.000000 cercis-0.1.5/tests/data/configurable_cases/indentation/use_spaces/closing_bracket_no_extra_indent/base_indent_spaces=4/fdei=True_olcei=True.py
--rw-r--r--   0        0        0     4946 2020-02-02 00:00:00.000000 cercis-0.1.5/tests/data/configurable_cases/indentation/use_spaces/closing_bracket_no_extra_indent/base_indent_spaces=8/fdei=False_olcei=False.py
--rw-r--r--   0        0        0     5177 2020-02-02 00:00:00.000000 cercis-0.1.5/tests/data/configurable_cases/indentation/use_spaces/closing_bracket_no_extra_indent/base_indent_spaces=8/fdei=False_olcei=True.py
--rw-r--r--   0        0        0     5297 2020-02-02 00:00:00.000000 cercis-0.1.5/tests/data/configurable_cases/indentation/use_spaces/closing_bracket_no_extra_indent/base_indent_spaces=8/fdei=True_olcei=False.py
--rw-r--r--   0        0        0     5528 2020-02-02 00:00:00.000000 cercis-0.1.5/tests/data/configurable_cases/indentation/use_spaces/closing_bracket_no_extra_indent/base_indent_spaces=8/fdei=True_olcei=True.py
--rw-r--r--   0        0        0     3449 2020-02-02 00:00:00.000000 cercis-0.1.5/tests/data/configurable_cases/indentation/use_tabs/closing_bracket_extra_indent/fdei=False_olcei=False.py
--rw-r--r--   0        0        0     3482 2020-02-02 00:00:00.000000 cercis-0.1.5/tests/data/configurable_cases/indentation/use_tabs/closing_bracket_extra_indent/fdei=False_olcei=True.py
--rw-r--r--   0        0        0     3502 2020-02-02 00:00:00.000000 cercis-0.1.5/tests/data/configurable_cases/indentation/use_tabs/closing_bracket_extra_indent/fdei=True_olcei=False.py
--rw-r--r--   0        0        0     3535 2020-02-02 00:00:00.000000 cercis-0.1.5/tests/data/configurable_cases/indentation/use_tabs/closing_bracket_extra_indent/fdei=True_olcei=True.py
--rw-r--r--   0        0        0     3434 2020-02-02 00:00:00.000000 cercis-0.1.5/tests/data/configurable_cases/indentation/use_tabs/closing_bracket_no_extra_indent/fdei=False_olcei=False.py
--rw-r--r--   0        0        0     3462 2020-02-02 00:00:00.000000 cercis-0.1.5/tests/data/configurable_cases/indentation/use_tabs/closing_bracket_no_extra_indent/fdei=False_olcei=True.py
--rw-r--r--   0        0        0     3477 2020-02-02 00:00:00.000000 cercis-0.1.5/tests/data/configurable_cases/indentation/use_tabs/closing_bracket_no_extra_indent/fdei=True_olcei=False.py
--rw-r--r--   0        0        0     3505 2020-02-02 00:00:00.000000 cercis-0.1.5/tests/data/configurable_cases/indentation/use_tabs/closing_bracket_no_extra_indent/fdei=True_olcei=True.py
--rw-r--r--   0        0        0     1448 2020-02-02 00:00:00.000000 cercis-0.1.5/tests/data/configurable_cases/indentation/use_tabs/line_length_calculation/tab_width_1.py
--rw-r--r--   0        0        0     1453 2020-02-02 00:00:00.000000 cercis-0.1.5/tests/data/configurable_cases/indentation/use_tabs/line_length_calculation/tab_width_2.py
--rw-r--r--   0        0        0     1458 2020-02-02 00:00:00.000000 cercis-0.1.5/tests/data/configurable_cases/indentation/use_tabs/line_length_calculation/tab_width_3.py
--rw-r--r--   0        0        0     1463 2020-02-02 00:00:00.000000 cercis-0.1.5/tests/data/configurable_cases/indentation/use_tabs/line_length_calculation/tab_width_4.py
--rw-r--r--   0        0        0     1468 2020-02-02 00:00:00.000000 cercis-0.1.5/tests/data/configurable_cases/indentation/use_tabs/line_length_calculation/tab_width_5.py
--rw-r--r--   0        0        0     1475 2020-02-02 00:00:00.000000 cercis-0.1.5/tests/data/configurable_cases/indentation/use_tabs/line_length_calculation/tab_width_8.py
--rw-r--r--   0        0        0      863 2020-02-02 00:00:00.000000 cercis-0.1.5/tests/data/configurable_cases/line_with_long_string/edge_cases.py
--rw-r--r--   0        0        0    11060 2020-02-02 00:00:00.000000 cercis-0.1.5/tests/data/configurable_cases/line_with_long_string/long_strings_flag_disabled__Black_default.py
--rw-r--r--   0        0        0    22087 2020-02-02 00:00:00.000000 cercis-0.1.5/tests/data/configurable_cases/line_with_long_string/long_strings_flag_disabled__Cercis_default.py
--rw-r--r--   0        0        0     6138 2020-02-02 00:00:00.000000 cercis-0.1.5/tests/data/configurable_cases/line_with_long_string/test_cases__Black_default.py
--rw-r--r--   0        0        0     6056 2020-02-02 00:00:00.000000 cercis-0.1.5/tests/data/configurable_cases/line_with_long_string/test_cases__Cercis_default.py
--rw-r--r--   0        0        0     6193 2020-02-02 00:00:00.000000 cercis-0.1.5/tests/data/configurable_cases/nested_brackets/nested_brackets__Black_default.py
--rw-r--r--   0        0        0     2832 2020-02-02 00:00:00.000000 cercis-0.1.5/tests/data/configurable_cases/nested_brackets/nested_brackets__Cercis_default.py
--rw-r--r--   0        0        0     2011 2020-02-02 00:00:00.000000 cercis-0.1.5/tests/data/configurable_cases/nested_brackets/nested_brackets_explodes__Black_default.py
--rw-r--r--   0        0        0     2212 2020-02-02 00:00:00.000000 cercis-0.1.5/tests/data/configurable_cases/nested_brackets/nested_brackets_explodes__Cercis_default.py
--rw-r--r--   0        0        0     7699 2020-02-02 00:00:00.000000 cercis-0.1.5/tests/data/configurable_cases/pragma_comments/Black_default.py
--rw-r--r--   0        0        0    10763 2020-02-02 00:00:00.000000 cercis-0.1.5/tests/data/configurable_cases/pragma_comments/Cercis_default.py
--rw-r--r--   0        0        0     7702 2020-02-02 00:00:00.000000 cercis-0.1.5/tests/data/configurable_cases/single_quote/docstring.py
--rw-r--r--   0        0        0      140 2020-02-02 00:00:00.000000 cercis-0.1.5/tests/data/configurable_cases/single_quote/docstring_no_extra_empty_line_before_eof.py
--rw-r--r--   0        0        0     3513 2020-02-02 00:00:00.000000 cercis-0.1.5/tests/data/configurable_cases/single_quote/docstring_preview.py
--rw-r--r--   0        0        0      745 2020-02-02 00:00:00.000000 cercis-0.1.5/tests/data/configurable_cases/single_quote/more_quotes.py
--rw-r--r--   0        0        0      845 2020-02-02 00:00:00.000000 cercis-0.1.5/tests/data/configurable_cases/single_quote/string_prefixes.py
--rw-r--r--   0        0        0     2279 2020-02-02 00:00:00.000000 cercis-0.1.5/tests/data/configurable_cases/single_quote/torture.py
--rw-r--r--   0        0        0      498 2020-02-02 00:00:00.000000 cercis-0.1.5/tests/data/fast/pep_572_do_not_remove_parens.py
--rw-r--r--   0        0        0        5 2020-02-02 00:00:00.000000 cercis-0.1.5/tests/data/gitignore_used_on_multiple_sources/.gitignore
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 cercis-0.1.5/tests/data/gitignore_used_on_multiple_sources/dir1/a.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 cercis-0.1.5/tests/data/gitignore_used_on_multiple_sources/dir1/b.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 cercis-0.1.5/tests/data/gitignore_used_on_multiple_sources/dir2/a.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 cercis-0.1.5/tests/data/gitignore_used_on_multiple_sources/dir2/b.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 cercis-0.1.5/tests/data/ignore_subfolders_gitignore_tests/a.py
--rw-r--r--   0        0        0        4 2020-02-02 00:00:00.000000 cercis-0.1.5/tests/data/ignore_subfolders_gitignore_tests/subdir/.gitignore
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 cercis-0.1.5/tests/data/ignore_subfolders_gitignore_tests/subdir/b.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 cercis-0.1.5/tests/data/ignore_subfolders_gitignore_tests/subdir/subdir/c.py
--rw-r--r--   0        0        0       14 2020-02-02 00:00:00.000000 cercis-0.1.5/tests/data/include_exclude_tests/.gitignore
--rw-r--r--   0        0        0      114 2020-02-02 00:00:00.000000 cercis-0.1.5/tests/data/include_exclude_tests/pyproject.toml
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 cercis-0.1.5/tests/data/include_exclude_tests/b/.definitely_exclude/a.pie
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 cercis-0.1.5/tests/data/include_exclude_tests/b/.definitely_exclude/a.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 cercis-0.1.5/tests/data/include_exclude_tests/b/.definitely_exclude/a.pyi
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 cercis-0.1.5/tests/data/include_exclude_tests/b/dont_exclude/a.pie
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 cercis-0.1.5/tests/data/include_exclude_tests/b/dont_exclude/a.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 cercis-0.1.5/tests/data/include_exclude_tests/b/dont_exclude/a.pyi
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 cercis-0.1.5/tests/data/include_exclude_tests/b/exclude/a.pie
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 cercis-0.1.5/tests/data/include_exclude_tests/b/exclude/a.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 cercis-0.1.5/tests/data/include_exclude_tests/b/exclude/a.pyi
--rw-r--r--   0        0        0        2 2020-02-02 00:00:00.000000 cercis-0.1.5/tests/data/invalid_gitignore_tests/.gitignore
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 cercis-0.1.5/tests/data/invalid_gitignore_tests/a.py
--rw-r--r--   0        0        0       89 2020-02-02 00:00:00.000000 cercis-0.1.5/tests/data/invalid_gitignore_tests/pyproject.toml
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 cercis-0.1.5/tests/data/invalid_nested_gitignore_tests/a.py
--rw-r--r--   0        0        0       89 2020-02-02 00:00:00.000000 cercis-0.1.5/tests/data/invalid_nested_gitignore_tests/pyproject.toml
--rw-r--r--   0        0        0        2 2020-02-02 00:00:00.000000 cercis-0.1.5/tests/data/invalid_nested_gitignore_tests/a/.gitignore
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 cercis-0.1.5/tests/data/invalid_nested_gitignore_tests/a/a.py
--rw-r--r--   0        0        0      436 2020-02-02 00:00:00.000000 cercis-0.1.5/tests/data/jupyter/non_python_notebook.ipynb
--rw-r--r--   0        0        0      371 2020-02-02 00:00:00.000000 cercis-0.1.5/tests/data/jupyter/notebook_empty_metadata.ipynb
--rw-r--r--   0        0        0      641 2020-02-02 00:00:00.000000 cercis-0.1.5/tests/data/jupyter/notebook_no_trailing_newline.ipynb
--rw-r--r--   0        0        0      642 2020-02-02 00:00:00.000000 cercis-0.1.5/tests/data/jupyter/notebook_trailing_newline.ipynb
--rw-r--r--   0        0        0        4 2020-02-02 00:00:00.000000 cercis-0.1.5/tests/data/jupyter/notebook_which_cant_be_parsed.ipynb
--rw-r--r--   0        0        0      761 2020-02-02 00:00:00.000000 cercis-0.1.5/tests/data/jupyter/notebook_without_changes.ipynb
--rw-r--r--   0        0        0      495 2020-02-02 00:00:00.000000 cercis-0.1.5/tests/data/miscellaneous/async_as_identifier.py
--rw-r--r--   0        0        0      255 2020-02-02 00:00:00.000000 cercis-0.1.5/tests/data/miscellaneous/blackd_diff.diff
--rw-r--r--   0        0        0       98 2020-02-02 00:00:00.000000 cercis-0.1.5/tests/data/miscellaneous/blackd_diff.py
--rw-r--r--   0        0        0    15604 2020-02-02 00:00:00.000000 cercis-0.1.5/tests/data/miscellaneous/debug_visitor.out
--rw-r--r--   0        0        0     1193 2020-02-02 00:00:00.000000 cercis-0.1.5/tests/data/miscellaneous/debug_visitor.py
--rw-r--r--   0        0        0     1774 2020-02-02 00:00:00.000000 cercis-0.1.5/tests/data/miscellaneous/decorators.py
--rw-r--r--   0        0        0     3601 2020-02-02 00:00:00.000000 cercis-0.1.5/tests/data/miscellaneous/docstring_no_string_normalization.py
--rw-r--r--   0        0        0      357 2020-02-02 00:00:00.000000 cercis-0.1.5/tests/data/miscellaneous/docstring_preview_no_string_normalization.py
--rw-r--r--   0        0        0    15711 2020-02-02 00:00:00.000000 cercis-0.1.5/tests/data/miscellaneous/expression_skip_magic_trailing_comma.diff
--rw-r--r--   0        0        0      626 2020-02-02 00:00:00.000000 cercis-0.1.5/tests/data/miscellaneous/force_py36.py
--rw-r--r--   0        0        0      793 2020-02-02 00:00:00.000000 cercis-0.1.5/tests/data/miscellaneous/force_pyi.py
--rw-r--r--   0        0        0       59 2020-02-02 00:00:00.000000 cercis-0.1.5/tests/data/miscellaneous/invalid_header.py
--rw-r--r--   0        0        0      101 2020-02-02 00:00:00.000000 cercis-0.1.5/tests/data/miscellaneous/linelength6.py
--rw-r--r--   0        0        0    11583 2020-02-02 00:00:00.000000 cercis-0.1.5/tests/data/miscellaneous/long_strings_flag_disabled.py
--rw-r--r--   0        0        0      293 2020-02-02 00:00:00.000000 cercis-0.1.5/tests/data/miscellaneous/missing_final_newline.diff
--rw-r--r--   0        0        0      145 2020-02-02 00:00:00.000000 cercis-0.1.5/tests/data/miscellaneous/missing_final_newline.py
--rw-r--r--   0        0        0      284 2020-02-02 00:00:00.000000 cercis-0.1.5/tests/data/miscellaneous/nested_class_stub.pyi
--rw-r--r--   0        0        0      279 2020-02-02 00:00:00.000000 cercis-0.1.5/tests/data/miscellaneous/pattern_matching_invalid.py
--rw-r--r--   0        0        0       69 2020-02-02 00:00:00.000000 cercis-0.1.5/tests/data/miscellaneous/power_op_newline.py
--rw-r--r--   0        0        0      758 2020-02-02 00:00:00.000000 cercis-0.1.5/tests/data/miscellaneous/python2_detection.py
--rw-r--r--   0        0        0     2361 2020-02-02 00:00:00.000000 cercis-0.1.5/tests/data/miscellaneous/string_quotes.py
--rw-r--r--   0        0        0     2266 2020-02-02 00:00:00.000000 cercis-0.1.5/tests/data/miscellaneous/stub.pyi
--rw-r--r--   0        0        0      114 2020-02-02 00:00:00.000000 cercis-0.1.5/tests/data/nested_gitignore_tests/pyproject.toml
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 cercis-0.1.5/tests/data/nested_gitignore_tests/x.py
--rw-r--r--   0        0        0        5 2020-02-02 00:00:00.000000 cercis-0.1.5/tests/data/nested_gitignore_tests/root/.gitignore
--rw-r--r--   0        0        0       39 2020-02-02 00:00:00.000000 cercis-0.1.5/tests/data/nested_gitignore_tests/root/a.py
--rw-r--r--   0        0        0       21 2020-02-02 00:00:00.000000 cercis-0.1.5/tests/data/nested_gitignore_tests/root/b.py
--rw-r--r--   0        0        0       21 2020-02-02 00:00:00.000000 cercis-0.1.5/tests/data/nested_gitignore_tests/root/c.py
--rw-r--r--   0        0        0        5 2020-02-02 00:00:00.000000 cercis-0.1.5/tests/data/nested_gitignore_tests/root/child/.gitignore
--rw-r--r--   0        0        0       39 2020-02-02 00:00:00.000000 cercis-0.1.5/tests/data/nested_gitignore_tests/root/child/a.py
--rw-r--r--   0        0        0       40 2020-02-02 00:00:00.000000 cercis-0.1.5/tests/data/nested_gitignore_tests/root/child/b.py
--rw-r--r--   0        0        0       21 2020-02-02 00:00:00.000000 cercis-0.1.5/tests/data/nested_gitignore_tests/root/child/c.py
--rw-r--r--   0        0        0      279 2020-02-02 00:00:00.000000 cercis-0.1.5/tests/data/preview/async_stmts.py
--rw-r--r--   0        0        0     4107 2020-02-02 00:00:00.000000 cercis-0.1.5/tests/data/preview/cantfit.py
--rw-r--r--   0        0        0     8294 2020-02-02 00:00:00.000000 cercis-0.1.5/tests/data/preview/comments7.py
--rw-r--r--   0        0        0      613 2020-02-02 00:00:00.000000 cercis-0.1.5/tests/data/preview/format_unicode_escape_seq.py
--rw-r--r--   0        0        0     2784 2020-02-02 00:00:00.000000 cercis-0.1.5/tests/data/preview/long_dict_values.py
--rw-r--r--   0        0        0    33216 2020-02-02 00:00:00.000000 cercis-0.1.5/tests/data/preview/long_strings.py
--rw-r--r--   0        0        0     1418 2020-02-02 00:00:00.000000 cercis-0.1.5/tests/data/preview/long_strings__east_asian_width.py
--rw-r--r--   0        0        0     6536 2020-02-02 00:00:00.000000 cercis-0.1.5/tests/data/preview/long_strings__edge_case.py
--rw-r--r--   0        0        0    45897 2020-02-02 00:00:00.000000 cercis-0.1.5/tests/data/preview/long_strings__regression.py
--rw-r--r--   0        0        0     1105 2020-02-02 00:00:00.000000 cercis-0.1.5/tests/data/preview/long_strings__type_annotations.py
--rw-r--r--   0        0        0     7207 2020-02-02 00:00:00.000000 cercis-0.1.5/tests/data/preview/multiline_strings.py
--rw-r--r--   0        0        0      481 2020-02-02 00:00:00.000000 cercis-0.1.5/tests/data/preview/percent_precedence.py
--rw-r--r--   0        0        0     2525 2020-02-02 00:00:00.000000 cercis-0.1.5/tests/data/preview/prefer_rhs_split.py
--rw-r--r--   0        0        0      342 2020-02-02 00:00:00.000000 cercis-0.1.5/tests/data/preview/return_annotation_brackets_string.py
--rw-r--r--   0        0        0      655 2020-02-02 00:00:00.000000 cercis-0.1.5/tests/data/preview/trailing_comma.py
--rw-r--r--   0        0        0     1140 2020-02-02 00:00:00.000000 cercis-0.1.5/tests/data/preview_context_managers/targeting_py38.py
--rw-r--r--   0        0        0     3361 2020-02-02 00:00:00.000000 cercis-0.1.5/tests/data/preview_context_managers/targeting_py39.py
--rw-r--r--   0        0        0      595 2020-02-02 00:00:00.000000 cercis-0.1.5/tests/data/preview_context_managers/auto_detect/features_3_10.py
--rw-r--r--   0        0        0      553 2020-02-02 00:00:00.000000 cercis-0.1.5/tests/data/preview_context_managers/auto_detect/features_3_11.py
--rw-r--r--   0        0        0     1058 2020-02-02 00:00:00.000000 cercis-0.1.5/tests/data/preview_context_managers/auto_detect/features_3_8.py
--rw-r--r--   0        0        0      623 2020-02-02 00:00:00.000000 cercis-0.1.5/tests/data/preview_context_managers/auto_detect/features_3_9.py
--rw-r--r--   0        0        0      133 2020-02-02 00:00:00.000000 cercis-0.1.5/tests/data/project_metadata/both_pyproject.toml
--rw-r--r--   0        0        0       74 2020-02-02 00:00:00.000000 cercis-0.1.5/tests/data/project_metadata/neither_pyproject.toml
--rw-r--r--   0        0        0      101 2020-02-02 00:00:00.000000 cercis-0.1.5/tests/data/project_metadata/only_black_pyproject.toml
--rw-r--r--   0        0        0      106 2020-02-02 00:00:00.000000 cercis-0.1.5/tests/data/project_metadata/only_metadata_pyproject.toml
--rw-r--r--   0        0        0      765 2020-02-02 00:00:00.000000 cercis-0.1.5/tests/data/py_310/parenthesized_context_managers.py
--rw-r--r--   0        0        0     2668 2020-02-02 00:00:00.000000 cercis-0.1.5/tests/data/py_310/pattern_matching_complex.py
--rw-r--r--   0        0        0     1965 2020-02-02 00:00:00.000000 cercis-0.1.5/tests/data/py_310/pattern_matching_extras.py
--rw-r--r--   0        0        0     3066 2020-02-02 00:00:00.000000 cercis-0.1.5/tests/data/py_310/pattern_matching_generic.py
--rw-r--r--   0        0        0     2641 2020-02-02 00:00:00.000000 cercis-0.1.5/tests/data/py_310/pattern_matching_simple.py
--rw-r--r--   0        0        0     1061 2020-02-02 00:00:00.000000 cercis-0.1.5/tests/data/py_310/pattern_matching_style.py
--rw-r--r--   0        0        0      491 2020-02-02 00:00:00.000000 cercis-0.1.5/tests/data/py_310/pep_572_py310.py
--rw-r--r--   0        0        0      509 2020-02-02 00:00:00.000000 cercis-0.1.5/tests/data/py_310/remove_newline_after_match.py
--rw-r--r--   0        0        0      380 2020-02-02 00:00:00.000000 cercis-0.1.5/tests/data/py_310/starred_for_target.py
--rw-r--r--   0        0        0     2114 2020-02-02 00:00:00.000000 cercis-0.1.5/tests/data/py_311/pep_646.py
--rw-r--r--   0        0        0      972 2020-02-02 00:00:00.000000 cercis-0.1.5/tests/data/py_311/pep_654.py
--rw-r--r--   0        0        0     2033 2020-02-02 00:00:00.000000 cercis-0.1.5/tests/data/py_311/pep_654_style.py
--rw-r--r--   0        0        0      597 2020-02-02 00:00:00.000000 cercis-0.1.5/tests/data/py_36/numeric_literals.py
--rw-r--r--   0        0        0      267 2020-02-02 00:00:00.000000 cercis-0.1.5/tests/data/py_36/numeric_literals_skip_underscores.py
--rw-r--r--   0        0        0     1199 2020-02-02 00:00:00.000000 cercis-0.1.5/tests/data/py_37/python37.py
--rw-r--r--   0        0        0      740 2020-02-02 00:00:00.000000 cercis-0.1.5/tests/data/py_38/pep_570.py
--rw-r--r--   0        0        0      970 2020-02-02 00:00:00.000000 cercis-0.1.5/tests/data/py_38/pep_572.py
--rw-r--r--   0        0        0     1895 2020-02-02 00:00:00.000000 cercis-0.1.5/tests/data/py_38/pep_572_remove_parens.py
--rw-r--r--   0        0        0      834 2020-02-02 00:00:00.000000 cercis-0.1.5/tests/data/py_38/python38.py
--rw-r--r--   0        0        0      251 2020-02-02 00:00:00.000000 cercis-0.1.5/tests/data/py_39/pep_572_py39.py
--rw-r--r--   0        0        0      696 2020-02-02 00:00:00.000000 cercis-0.1.5/tests/data/py_39/python39.py
--rw-r--r--   0        0        0     2575 2020-02-02 00:00:00.000000 cercis-0.1.5/tests/data/py_39/remove_with_brackets.py
--rw-r--r--   0        0        0      907 2020-02-02 00:00:00.000000 cercis-0.1.5/tests/data/simple_cases/attribute_access_on_number_literals.py
--rw-r--r--   0        0        0       63 2020-02-02 00:00:00.000000 cercis-0.1.5/tests/data/simple_cases/beginning_backslash.py
--rw-r--r--   0        0        0      333 2020-02-02 00:00:00.000000 cercis-0.1.5/tests/data/simple_cases/bracketmatch.py
--rw-r--r--   0        0        0     1091 2020-02-02 00:00:00.000000 cercis-0.1.5/tests/data/simple_cases/class_blank_parentheses.py
--rw-r--r--   0        0        0     4318 2020-02-02 00:00:00.000000 cercis-0.1.5/tests/data/simple_cases/class_methods_new_line.py
--rw-r--r--   0        0        0     3294 2020-02-02 00:00:00.000000 cercis-0.1.5/tests/data/simple_cases/collections.py
--rw-r--r--   0        0        0      212 2020-02-02 00:00:00.000000 cercis-0.1.5/tests/data/simple_cases/comment_after_escaped_newline.py
--rw-r--r--   0        0        0     1909 2020-02-02 00:00:00.000000 cercis-0.1.5/tests/data/simple_cases/comments.py
--rw-r--r--   0        0        0     7639 2020-02-02 00:00:00.000000 cercis-0.1.5/tests/data/simple_cases/comments2.py
--rw-r--r--   0        0        0     1573 2020-02-02 00:00:00.000000 cercis-0.1.5/tests/data/simple_cases/comments3.py
--rw-r--r--   0        0        0     3536 2020-02-02 00:00:00.000000 cercis-0.1.5/tests/data/simple_cases/comments4.py
--rw-r--r--   0        0        0     1196 2020-02-02 00:00:00.000000 cercis-0.1.5/tests/data/simple_cases/comments5.py
--rw-r--r--   0        0        0     2567 2020-02-02 00:00:00.000000 cercis-0.1.5/tests/data/simple_cases/comments6.py
--rw-r--r--   0        0        0      300 2020-02-02 00:00:00.000000 cercis-0.1.5/tests/data/simple_cases/comments8.py
--rw-r--r--   0        0        0     5279 2020-02-02 00:00:00.000000 cercis-0.1.5/tests/data/simple_cases/comments9.py
--rw-r--r--   0        0        0      994 2020-02-02 00:00:00.000000 cercis-0.1.5/tests/data/simple_cases/comments_non_breaking_space.py
--rw-r--r--   0        0        0     5597 2020-02-02 00:00:00.000000 cercis-0.1.5/tests/data/simple_cases/composition.py
--rw-r--r--   0        0        0    11198 2020-02-02 00:00:00.000000 cercis-0.1.5/tests/data/simple_cases/composition_no_trailing_comma.py
--rw-r--r--   0        0        0     7699 2020-02-02 00:00:00.000000 cercis-0.1.5/tests/data/simple_cases/docstring.py
--rw-r--r--   0        0        0      140 2020-02-02 00:00:00.000000 cercis-0.1.5/tests/data/simple_cases/docstring_no_extra_empty_line_before_eof.py
--rw-r--r--   0        0        0     3513 2020-02-02 00:00:00.000000 cercis-0.1.5/tests/data/simple_cases/docstring_preview.py
--rw-r--r--   0        0        0     4596 2020-02-02 00:00:00.000000 cercis-0.1.5/tests/data/simple_cases/empty_lines.py
--rw-r--r--   0        0        0    15801 2020-02-02 00:00:00.000000 cercis-0.1.5/tests/data/simple_cases/expression.diff
--rw-r--r--   0        0        0    18624 2020-02-02 00:00:00.000000 cercis-0.1.5/tests/data/simple_cases/expression.py
--rw-r--r--   0        0        0     9681 2020-02-02 00:00:00.000000 cercis-0.1.5/tests/data/simple_cases/fmtonoff.py
--rw-r--r--   0        0        0      604 2020-02-02 00:00:00.000000 cercis-0.1.5/tests/data/simple_cases/fmtonoff2.py
--rw-r--r--   0        0        0      251 2020-02-02 00:00:00.000000 cercis-0.1.5/tests/data/simple_cases/fmtonoff3.py
--rw-r--r--   0        0        0      278 2020-02-02 00:00:00.000000 cercis-0.1.5/tests/data/simple_cases/fmtonoff4.py
--rw-r--r--   0        0        0     3627 2020-02-02 00:00:00.000000 cercis-0.1.5/tests/data/simple_cases/fmtonoff5.py
--rw-r--r--   0        0        0      277 2020-02-02 00:00:00.000000 cercis-0.1.5/tests/data/simple_cases/fmtpass_imports.py
--rw-r--r--   0        0        0       40 2020-02-02 00:00:00.000000 cercis-0.1.5/tests/data/simple_cases/fmtskip.py
--rw-r--r--   0        0        0      555 2020-02-02 00:00:00.000000 cercis-0.1.5/tests/data/simple_cases/fmtskip2.py
--rw-r--r--   0        0        0      362 2020-02-02 00:00:00.000000 cercis-0.1.5/tests/data/simple_cases/fmtskip3.py
--rw-r--r--   0        0        0       92 2020-02-02 00:00:00.000000 cercis-0.1.5/tests/data/simple_cases/fmtskip4.py
--rw-r--r--   0        0        0      301 2020-02-02 00:00:00.000000 cercis-0.1.5/tests/data/simple_cases/fmtskip5.py
--rw-r--r--   0        0        0      235 2020-02-02 00:00:00.000000 cercis-0.1.5/tests/data/simple_cases/fmtskip6.py
--rw-r--r--   0        0        0      356 2020-02-02 00:00:00.000000 cercis-0.1.5/tests/data/simple_cases/fmtskip7.py
--rw-r--r--   0        0        0     1705 2020-02-02 00:00:00.000000 cercis-0.1.5/tests/data/simple_cases/fmtskip8.py
--rw-r--r--   0        0        0      989 2020-02-02 00:00:00.000000 cercis-0.1.5/tests/data/simple_cases/fstring.py
--rw-r--r--   0        0        0     6482 2020-02-02 00:00:00.000000 cercis-0.1.5/tests/data/simple_cases/function.py
--rw-r--r--   0        0        0     2427 2020-02-02 00:00:00.000000 cercis-0.1.5/tests/data/simple_cases/function2.py
--rw-r--r--   0        0        0     3657 2020-02-02 00:00:00.000000 cercis-0.1.5/tests/data/simple_cases/function_trailing_comma.py
--rw-r--r--   0        0        0     2542 2020-02-02 00:00:00.000000 cercis-0.1.5/tests/data/simple_cases/import_spacing.py
--rw-r--r--   0        0        0      674 2020-02-02 00:00:00.000000 cercis-0.1.5/tests/data/simple_cases/one_element_subscript.py
--rw-r--r--   0        0        0     3359 2020-02-02 00:00:00.000000 cercis-0.1.5/tests/data/simple_cases/power_op_spacing.py
--rw-r--r--   0        0        0     1106 2020-02-02 00:00:00.000000 cercis-0.1.5/tests/data/simple_cases/prefer_rhs_split_reformatted.py
--rw-r--r--   0        0        0     3205 2020-02-02 00:00:00.000000 cercis-0.1.5/tests/data/simple_cases/remove_await_parens.py
--rw-r--r--   0        0        0     2025 2020-02-02 00:00:00.000000 cercis-0.1.5/tests/data/simple_cases/remove_except_parens.py
--rw-r--r--   0        0        0     1460 2020-02-02 00:00:00.000000 cercis-0.1.5/tests/data/simple_cases/remove_for_brackets.py
--rw-r--r--   0        0        0     3351 2020-02-02 00:00:00.000000 cercis-0.1.5/tests/data/simple_cases/remove_newline_after_code_block_open.py
--rw-r--r--   0        0        0     3493 2020-02-02 00:00:00.000000 cercis-0.1.5/tests/data/simple_cases/remove_parens.py
--rw-r--r--   0        0        0     5141 2020-02-02 00:00:00.000000 cercis-0.1.5/tests/data/simple_cases/return_annotation_brackets.py
--rw-r--r--   0        0        0     1398 2020-02-02 00:00:00.000000 cercis-0.1.5/tests/data/simple_cases/skip_magic_trailing_comma.py
--rw-r--r--   0        0        0      787 2020-02-02 00:00:00.000000 cercis-0.1.5/tests/data/simple_cases/slices.py
--rw-r--r--   0        0        0      845 2020-02-02 00:00:00.000000 cercis-0.1.5/tests/data/simple_cases/string_prefixes.py
--rw-r--r--   0        0        0     2279 2020-02-02 00:00:00.000000 cercis-0.1.5/tests/data/simple_cases/torture.py
--rw-r--r--   0        0        0     1615 2020-02-02 00:00:00.000000 cercis-0.1.5/tests/data/simple_cases/trailing_comma_optional_parens1.py
--rw-r--r--   0        0        0      248 2020-02-02 00:00:00.000000 cercis-0.1.5/tests/data/simple_cases/trailing_comma_optional_parens2.py
--rw-r--r--   0        0        0      967 2020-02-02 00:00:00.000000 cercis-0.1.5/tests/data/simple_cases/trailing_comma_optional_parens3.py
--rw-r--r--   0        0        0     2123 2020-02-02 00:00:00.000000 cercis-0.1.5/tests/data/simple_cases/trailing_commas_in_leading_parts.py
--rw-r--r--   0        0        0       80 2020-02-02 00:00:00.000000 cercis-0.1.5/tests/data/simple_cases/tricky_unicode_symbols.py
--rw-r--r--   0        0        0      510 2020-02-02 00:00:00.000000 cercis-0.1.5/tests/data/simple_cases/tupleassign.py
--rw-r--r--   0        0        0       27 2020-02-02 00:00:00.000000 cercis-0.1.5/tests/data/simple_cases/whitespace.py
--rw-r--r--   0        0        0      101 2020-02-02 00:00:00.000000 cercis-0.1.5/tests/data/type_comments/type_comment_syntax_error.py
--rw-r--r--   0        0        0      273 2020-02-02 00:00:00.000000 cercis-0.1.5/.gitignore
--rw-r--r--   0        0        0     1061 2020-02-02 00:00:00.000000 cercis-0.1.5/LICENSE
--rw-r--r--   0        0        0     1080 2020-02-02 00:00:00.000000 cercis-0.1.5/LICENSE_ORIGINAL
--rw-r--r--   0        0        0     7134 2020-02-02 00:00:00.000000 cercis-0.1.5/pyproject.toml
--rw-r--r--   0        0        0    24988 2020-02-02 00:00:00.000000 cercis-0.1.5/PKG-INFO
+-rw-r--r--   0        0        0      106 2020-02-02 00:00:00.000000 cercis-0.1.6/.coveragerc
+-rw-r--r--   0        0        0      360 2020-02-02 00:00:00.000000 cercis-0.1.6/.flake8
+-rw-r--r--   0        0        0      125 2020-02-02 00:00:00.000000 cercis-0.1.6/.git_archival.txt
+-rw-r--r--   0        0        0       32 2020-02-02 00:00:00.000000 cercis-0.1.6/.gitattributes
+-rw-r--r--   0        0        0     1250 2020-02-02 00:00:00.000000 cercis-0.1.6/.pre-commit-config.yaml
+-rw-r--r--   0        0        0      533 2020-02-02 00:00:00.000000 cercis-0.1.6/.pre-commit-hooks.yaml
+-rw-r--r--   0        0        0       49 2020-02-02 00:00:00.000000 cercis-0.1.6/.prettierrc.yaml
+-rw-r--r--   0        0        0      220 2020-02-02 00:00:00.000000 cercis-0.1.6/.readthedocs.yaml
+-rw-r--r--   0        0        0     2133 2020-02-02 00:00:00.000000 cercis-0.1.6/CHANGELOG.md
+-rw-r--r--   0        0        0    49716 2020-02-02 00:00:00.000000 cercis-0.1.6/CHANGES.md
+-rw-r--r--   0        0        0      587 2020-02-02 00:00:00.000000 cercis-0.1.6/Dockerfile
+-rw-r--r--   0        0        0    23227 2020-02-02 00:00:00.000000 cercis-0.1.6/README.md
+-rw-r--r--   0        0        0     1618 2020-02-02 00:00:00.000000 cercis-0.1.6/action.yml
+-rw-r--r--   0        0        0      796 2020-02-02 00:00:00.000000 cercis-0.1.6/mypy.ini
+-rw-r--r--   0        0        0       99 2020-02-02 00:00:00.000000 cercis-0.1.6/test_requirements.txt
+-rw-r--r--   0        0        0     2972 2020-02-02 00:00:00.000000 cercis-0.1.6/tox.ini
+-rw-r--r--   0        0        0     1537 2020-02-02 00:00:00.000000 cercis-0.1.6/.github/PULL_REQUEST_TEMPLATE.md
+-rw-r--r--   0        0        0      565 2020-02-02 00:00:00.000000 cercis-0.1.6/.github/dependabot.yml
+-rw-r--r--   0        0        0     1557 2020-02-02 00:00:00.000000 cercis-0.1.6/.github/ISSUE_TEMPLATE/bug_report.md
+-rw-r--r--   0        0        0      545 2020-02-02 00:00:00.000000 cercis-0.1.6/.github/ISSUE_TEMPLATE/config.yml
+-rw-r--r--   0        0        0      692 2020-02-02 00:00:00.000000 cercis-0.1.6/.github/ISSUE_TEMPLATE/docs-issue.md
+-rw-r--r--   0        0        0      649 2020-02-02 00:00:00.000000 cercis-0.1.6/.github/ISSUE_TEMPLATE/feature_request.md
+-rw-r--r--   0        0        0      646 2020-02-02 00:00:00.000000 cercis-0.1.6/.github/ISSUE_TEMPLATE/style_issue.md
+-rw-r--r--   0        0        0      795 2020-02-02 00:00:00.000000 cercis-0.1.6/.github/workflows/check-changelog.yml
+-rw-r--r--   0        0        0     1534 2020-02-02 00:00:00.000000 cercis-0.1.6/.github/workflows/diff_shades_comment.yml
+-rw-r--r--   0        0        0     1894 2020-02-02 00:00:00.000000 cercis-0.1.6/.github/workflows/docker.yml
+-rw-r--r--   0        0        0     1127 2020-02-02 00:00:00.000000 cercis-0.1.6/.github/workflows/fuzz.yml
+-rw-r--r--   0        0        0     1232 2020-02-02 00:00:00.000000 cercis-0.1.6/.github/workflows/lint.yml
+-rw-r--r--   0        0        0      811 2020-02-02 00:00:00.000000 cercis-0.1.6/.github/workflows/python-package.yml
+-rw-r--r--   0        0        0     1253 2020-02-02 00:00:00.000000 cercis-0.1.6/.github/workflows/python-publish.yml
+-rw-r--r--   0        0        0     2998 2020-02-02 00:00:00.000000 cercis-0.1.6/.github/workflows/test.yml
+-rw-r--r--   0        0        0     1910 2020-02-02 00:00:00.000000 cercis-0.1.6/.github/workflows/upload_binary.yml
+-rw-r--r--   0        0        0      780 2020-02-02 00:00:00.000000 cercis-0.1.6/.github/workflows/version-check.yml
+-rw-r--r--   0        0        0     2467 2020-02-02 00:00:00.000000 cercis-0.1.6/action/main.py
+-rw-r--r--   0        0        0     7597 2020-02-02 00:00:00.000000 cercis-0.1.6/autoload/black.vim
+-rw-r--r--   0        0        0      342 2020-02-02 00:00:00.000000 cercis-0.1.6/gallery/Dockerfile
+-rw-r--r--   0        0        0     1595 2020-02-02 00:00:00.000000 cercis-0.1.6/gallery/README.md
+-rwxr-xr-x   0        0        0     9123 2020-02-02 00:00:00.000000 cercis-0.1.6/gallery/gallery.py
+-rw-r--r--   0        0        0     2176 2020-02-02 00:00:00.000000 cercis-0.1.6/plugin/black.vim
+-rw-r--r--   0        0        0       55 2020-02-02 00:00:00.000000 cercis-0.1.6/scripts/README.md
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 cercis-0.1.6/scripts/__init__.py
+-rw-r--r--   0        0        0     2500 2020-02-02 00:00:00.000000 cercis-0.1.6/scripts/check_version_and_changelog.py
+-rw-r--r--   0        0        0     8650 2020-02-02 00:00:00.000000 cercis-0.1.6/scripts/diff_shades_gha_helper.py
+-rw-r--r--   0        0        0     3527 2020-02-02 00:00:00.000000 cercis-0.1.6/scripts/fuzz.py
+-rw-r--r--   0        0        0     2458 2020-02-02 00:00:00.000000 cercis-0.1.6/scripts/make_width_table.py
+-rwxr-xr-x   0        0        0     2993 2020-02-02 00:00:00.000000 cercis-0.1.6/scripts/migrate-black.py
+-rw-r--r--   0        0        0       18 2020-02-02 00:00:00.000000 cercis-0.1.6/src/_cercis_version.py
+-rw-r--r--   0        0        0     8100 2020-02-02 00:00:00.000000 cercis-0.1.6/src/blackd/__init__.py
+-rw-r--r--   0        0        0       37 2020-02-02 00:00:00.000000 cercis-0.1.6/src/blackd/__main__.py
+-rw-r--r--   0        0        0     1585 2020-02-02 00:00:00.000000 cercis-0.1.6/src/blackd/middlewares.py
+-rw-r--r--   0        0        0    11278 2020-02-02 00:00:00.000000 cercis-0.1.6/src/blib2to3/Grammar.txt
+-rw-r--r--   0        0        0    12762 2020-02-02 00:00:00.000000 cercis-0.1.6/src/blib2to3/LICENSE
+-rw-r--r--   0        0        0      793 2020-02-02 00:00:00.000000 cercis-0.1.6/src/blib2to3/PatternGrammar.txt
+-rw-r--r--   0        0        0     1071 2020-02-02 00:00:00.000000 cercis-0.1.6/src/blib2to3/README
+-rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 cercis-0.1.6/src/blib2to3/__init__.py
+-rw-r--r--   0        0        0     5732 2020-02-02 00:00:00.000000 cercis-0.1.6/src/blib2to3/pygram.py
+-rw-r--r--   0        0        0    32612 2020-02-02 00:00:00.000000 cercis-0.1.6/src/blib2to3/pytree.py
+-rw-r--r--   0        0        0      143 2020-02-02 00:00:00.000000 cercis-0.1.6/src/blib2to3/pgen2/__init__.py
+-rw-r--r--   0        0        0     9607 2020-02-02 00:00:00.000000 cercis-0.1.6/src/blib2to3/pgen2/conv.py
+-rw-r--r--   0        0        0    10671 2020-02-02 00:00:00.000000 cercis-0.1.6/src/blib2to3/pgen2/driver.py
+-rw-r--r--   0        0        0     6873 2020-02-02 00:00:00.000000 cercis-0.1.6/src/blib2to3/pgen2/grammar.py
+-rw-r--r--   0        0        0     1628 2020-02-02 00:00:00.000000 cercis-0.1.6/src/blib2to3/pgen2/literals.py
+-rw-r--r--   0        0        0    14859 2020-02-02 00:00:00.000000 cercis-0.1.6/src/blib2to3/pgen2/parse.py
+-rw-r--r--   0        0        0    15508 2020-02-02 00:00:00.000000 cercis-0.1.6/src/blib2to3/pgen2/pgen.py
+-rw-r--r--   0        0        0     1919 2020-02-02 00:00:00.000000 cercis-0.1.6/src/blib2to3/pgen2/token.py
+-rw-r--r--   0        0        0    23120 2020-02-02 00:00:00.000000 cercis-0.1.6/src/blib2to3/pgen2/tokenize.py
+-rw-r--r--   0        0        0    52483 2020-02-02 00:00:00.000000 cercis-0.1.6/src/cercis/__init__.py
+-rw-r--r--   0        0        0       48 2020-02-02 00:00:00.000000 cercis-0.1.6/src/cercis/__main__.py
+-rw-r--r--   0        0        0    10871 2020-02-02 00:00:00.000000 cercis-0.1.6/src/cercis/_width_table.py
+-rw-r--r--   0        0        0    12274 2020-02-02 00:00:00.000000 cercis-0.1.6/src/cercis/brackets.py
+-rw-r--r--   0        0        0     2952 2020-02-02 00:00:00.000000 cercis-0.1.6/src/cercis/cache.py
+-rw-r--r--   0        0        0    12797 2020-02-02 00:00:00.000000 cercis-0.1.6/src/cercis/comments.py
+-rw-r--r--   0        0        0     6343 2020-02-02 00:00:00.000000 cercis-0.1.6/src/cercis/concurrency.py
+-rw-r--r--   0        0        0      772 2020-02-02 00:00:00.000000 cercis-0.1.6/src/cercis/const.py
+-rw-r--r--   0        0        0     1597 2020-02-02 00:00:00.000000 cercis-0.1.6/src/cercis/debug.py
+-rw-r--r--   0        0        0    13538 2020-02-02 00:00:00.000000 cercis-0.1.6/src/cercis/files.py
+-rw-r--r--   0        0        0    13514 2020-02-02 00:00:00.000000 cercis-0.1.6/src/cercis/handle_ipynb_magics.py
+-rw-r--r--   0        0        0     4612 2020-02-02 00:00:00.000000 cercis-0.1.6/src/cercis/indent.py
+-rw-r--r--   0        0        0    64165 2020-02-02 00:00:00.000000 cercis-0.1.6/src/cercis/linegen.py
+-rw-r--r--   0        0        0    40988 2020-02-02 00:00:00.000000 cercis-0.1.6/src/cercis/lines.py
+-rw-r--r--   0        0        0     8468 2020-02-02 00:00:00.000000 cercis-0.1.6/src/cercis/mode.py
+-rw-r--r--   0        0        0    25731 2020-02-02 00:00:00.000000 cercis-0.1.6/src/cercis/nodes.py
+-rw-r--r--   0        0        0     1653 2020-02-02 00:00:00.000000 cercis-0.1.6/src/cercis/numerics.py
+-rw-r--r--   0        0        0     3487 2020-02-02 00:00:00.000000 cercis-0.1.6/src/cercis/output.py
+-rw-r--r--   0        0        0    10164 2020-02-02 00:00:00.000000 cercis-0.1.6/src/cercis/parsing.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 cercis-0.1.6/src/cercis/py.typed
+-rw-r--r--   0        0        0     3452 2020-02-02 00:00:00.000000 cercis-0.1.6/src/cercis/report.py
+-rw-r--r--   0        0        0      556 2020-02-02 00:00:00.000000 cercis-0.1.6/src/cercis/rusty.py
+-rw-r--r--   0        0        0    14304 2020-02-02 00:00:00.000000 cercis-0.1.6/src/cercis/strings.py
+-rw-r--r--   0        0        0    91890 2020-02-02 00:00:00.000000 cercis-0.1.6/src/cercis/trans.py
+-rw-r--r--   0        0        0     2676 2020-02-02 00:00:00.000000 cercis-0.1.6/src/cercis/utils_line_wrapping.py
+-rw-r--r--   0        0        0     3267 2020-02-02 00:00:00.000000 cercis-0.1.6/src/cercis/utils_linegen.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 cercis-0.1.6/tests/__init__.py
+-rw-r--r--   0        0        0       36 2020-02-02 00:00:00.000000 cercis-0.1.6/tests/conftest.py
+-rw-r--r--   0        0        0       89 2020-02-02 00:00:00.000000 cercis-0.1.6/tests/empty.toml
+-rw-r--r--   0        0        0     4133 2020-02-02 00:00:00.000000 cercis-0.1.6/tests/optional.py
+-rw-r--r--   0        0        0      389 2020-02-02 00:00:00.000000 cercis-0.1.6/tests/test.toml
+-rw-r--r--   0        0        0   101263 2020-02-02 00:00:00.000000 cercis-0.1.6/tests/test_black.py
+-rw-r--r--   0        0        0     9188 2020-02-02 00:00:00.000000 cercis-0.1.6/tests/test_blackd.py
+-rw-r--r--   0        0        0    16234 2020-02-02 00:00:00.000000 cercis-0.1.6/tests/test_format.py
+-rw-r--r--   0        0        0    16390 2020-02-02 00:00:00.000000 cercis-0.1.6/tests/test_ipynb.py
+-rw-r--r--   0        0        0     1292 2020-02-02 00:00:00.000000 cercis-0.1.6/tests/test_no_ipynb.py
+-rw-r--r--   0        0        0     2267 2020-02-02 00:00:00.000000 cercis-0.1.6/tests/test_trans.py
+-rw-r--r--   0        0        0     2546 2020-02-02 00:00:00.000000 cercis-0.1.6/tests/test_utils_line_wrapping.py
+-rw-r--r--   0        0        0     7023 2020-02-02 00:00:00.000000 cercis-0.1.6/tests/util.py
+-rw-r--r--   0        0        0     4160 2020-02-02 00:00:00.000000 cercis-0.1.6/tests/data/conditional_expression.py
+-rw-r--r--   0        0        0       99 2020-02-02 00:00:00.000000 cercis-0.1.6/tests/data/empty_pyproject.toml
+-rw-r--r--   0        0        0     1611 2020-02-02 00:00:00.000000 cercis-0.1.6/tests/data/configurable_cases/closing_bracket_indent/extra_indent.py
+-rw-r--r--   0        0        0     1563 2020-02-02 00:00:00.000000 cercis-0.1.6/tests/data/configurable_cases/closing_bracket_indent/no_extra_indent.py
+-rw-r--r--   0        0        0     4438 2020-02-02 00:00:00.000000 cercis-0.1.6/tests/data/configurable_cases/func_def_indent/func_def_extra_indent.py
+-rw-r--r--   0        0        0     4262 2020-02-02 00:00:00.000000 cercis-0.1.6/tests/data/configurable_cases/func_def_indent/func_def_no_extra_indent.py
+-rw-r--r--   0        0        0     3449 2020-02-02 00:00:00.000000 cercis-0.1.6/tests/data/configurable_cases/indentation/use_spaces/closing_bracket_extra_indent/base_indent_spaces=1/fdei=False_olcei=False.py
+-rw-r--r--   0        0        0     3482 2020-02-02 00:00:00.000000 cercis-0.1.6/tests/data/configurable_cases/indentation/use_spaces/closing_bracket_extra_indent/base_indent_spaces=1/fdei=False_olcei=True.py
+-rw-r--r--   0        0        0     3502 2020-02-02 00:00:00.000000 cercis-0.1.6/tests/data/configurable_cases/indentation/use_spaces/closing_bracket_extra_indent/base_indent_spaces=1/fdei=True_olcei=False.py
+-rw-r--r--   0        0        0     3535 2020-02-02 00:00:00.000000 cercis-0.1.6/tests/data/configurable_cases/indentation/use_spaces/closing_bracket_extra_indent/base_indent_spaces=1/fdei=True_olcei=True.py
+-rw-r--r--   0        0        0     3680 2020-02-02 00:00:00.000000 cercis-0.1.6/tests/data/configurable_cases/indentation/use_spaces/closing_bracket_extra_indent/base_indent_spaces=2/fdei=False_olcei=False.py
+-rw-r--r--   0        0        0     3747 2020-02-02 00:00:00.000000 cercis-0.1.6/tests/data/configurable_cases/indentation/use_spaces/closing_bracket_extra_indent/base_indent_spaces=2/fdei=False_olcei=True.py
+-rw-r--r--   0        0        0     3787 2020-02-02 00:00:00.000000 cercis-0.1.6/tests/data/configurable_cases/indentation/use_spaces/closing_bracket_extra_indent/base_indent_spaces=2/fdei=True_olcei=False.py
+-rw-r--r--   0        0        0     3854 2020-02-02 00:00:00.000000 cercis-0.1.6/tests/data/configurable_cases/indentation/use_spaces/closing_bracket_extra_indent/base_indent_spaces=2/fdei=True_olcei=True.py
+-rw-r--r--   0        0        0     3911 2020-02-02 00:00:00.000000 cercis-0.1.6/tests/data/configurable_cases/indentation/use_spaces/closing_bracket_extra_indent/base_indent_spaces=3/fdei=False_olcei=False.py
+-rw-r--r--   0        0        0     4012 2020-02-02 00:00:00.000000 cercis-0.1.6/tests/data/configurable_cases/indentation/use_spaces/closing_bracket_extra_indent/base_indent_spaces=3/fdei=False_olcei=True.py
+-rw-r--r--   0        0        0     4072 2020-02-02 00:00:00.000000 cercis-0.1.6/tests/data/configurable_cases/indentation/use_spaces/closing_bracket_extra_indent/base_indent_spaces=3/fdei=True_olcei=False.py
+-rw-r--r--   0        0        0     4173 2020-02-02 00:00:00.000000 cercis-0.1.6/tests/data/configurable_cases/indentation/use_spaces/closing_bracket_extra_indent/base_indent_spaces=3/fdei=True_olcei=True.py
+-rw-r--r--   0        0        0     4142 2020-02-02 00:00:00.000000 cercis-0.1.6/tests/data/configurable_cases/indentation/use_spaces/closing_bracket_extra_indent/base_indent_spaces=4/fdei=False_olcei=False.py
+-rw-r--r--   0        0        0     4277 2020-02-02 00:00:00.000000 cercis-0.1.6/tests/data/configurable_cases/indentation/use_spaces/closing_bracket_extra_indent/base_indent_spaces=4/fdei=False_olcei=True.py
+-rw-r--r--   0        0        0     4357 2020-02-02 00:00:00.000000 cercis-0.1.6/tests/data/configurable_cases/indentation/use_spaces/closing_bracket_extra_indent/base_indent_spaces=4/fdei=True_olcei=False.py
+-rw-r--r--   0        0        0     4492 2020-02-02 00:00:00.000000 cercis-0.1.6/tests/data/configurable_cases/indentation/use_spaces/closing_bracket_extra_indent/base_indent_spaces=4/fdei=True_olcei=True.py
+-rw-r--r--   0        0        0     5066 2020-02-02 00:00:00.000000 cercis-0.1.6/tests/data/configurable_cases/indentation/use_spaces/closing_bracket_extra_indent/base_indent_spaces=8/fdei=False_olcei=False.py
+-rw-r--r--   0        0        0     5337 2020-02-02 00:00:00.000000 cercis-0.1.6/tests/data/configurable_cases/indentation/use_spaces/closing_bracket_extra_indent/base_indent_spaces=8/fdei=False_olcei=True.py
+-rw-r--r--   0        0        0     5497 2020-02-02 00:00:00.000000 cercis-0.1.6/tests/data/configurable_cases/indentation/use_spaces/closing_bracket_extra_indent/base_indent_spaces=8/fdei=True_olcei=False.py
+-rw-r--r--   0        0        0     5768 2020-02-02 00:00:00.000000 cercis-0.1.6/tests/data/configurable_cases/indentation/use_spaces/closing_bracket_extra_indent/base_indent_spaces=8/fdei=True_olcei=True.py
+-rw-r--r--   0        0        0     3434 2020-02-02 00:00:00.000000 cercis-0.1.6/tests/data/configurable_cases/indentation/use_spaces/closing_bracket_no_extra_indent/base_indent_spaces=1/fdei=False_olcei=False.py
+-rw-r--r--   0        0        0     3462 2020-02-02 00:00:00.000000 cercis-0.1.6/tests/data/configurable_cases/indentation/use_spaces/closing_bracket_no_extra_indent/base_indent_spaces=1/fdei=False_olcei=True.py
+-rw-r--r--   0        0        0     3477 2020-02-02 00:00:00.000000 cercis-0.1.6/tests/data/configurable_cases/indentation/use_spaces/closing_bracket_no_extra_indent/base_indent_spaces=1/fdei=True_olcei=False.py
+-rw-r--r--   0        0        0     3505 2020-02-02 00:00:00.000000 cercis-0.1.6/tests/data/configurable_cases/indentation/use_spaces/closing_bracket_no_extra_indent/base_indent_spaces=1/fdei=True_olcei=True.py
+-rw-r--r--   0        0        0     3650 2020-02-02 00:00:00.000000 cercis-0.1.6/tests/data/configurable_cases/indentation/use_spaces/closing_bracket_no_extra_indent/base_indent_spaces=2/fdei=False_olcei=False.py
+-rw-r--r--   0        0        0     3707 2020-02-02 00:00:00.000000 cercis-0.1.6/tests/data/configurable_cases/indentation/use_spaces/closing_bracket_no_extra_indent/base_indent_spaces=2/fdei=False_olcei=True.py
+-rw-r--r--   0        0        0     3737 2020-02-02 00:00:00.000000 cercis-0.1.6/tests/data/configurable_cases/indentation/use_spaces/closing_bracket_no_extra_indent/base_indent_spaces=2/fdei=True_olcei=False.py
+-rw-r--r--   0        0        0     3794 2020-02-02 00:00:00.000000 cercis-0.1.6/tests/data/configurable_cases/indentation/use_spaces/closing_bracket_no_extra_indent/base_indent_spaces=2/fdei=True_olcei=True.py
+-rw-r--r--   0        0        0     3866 2020-02-02 00:00:00.000000 cercis-0.1.6/tests/data/configurable_cases/indentation/use_spaces/closing_bracket_no_extra_indent/base_indent_spaces=3/fdei=False_olcei=False.py
+-rw-r--r--   0        0        0     3952 2020-02-02 00:00:00.000000 cercis-0.1.6/tests/data/configurable_cases/indentation/use_spaces/closing_bracket_no_extra_indent/base_indent_spaces=3/fdei=False_olcei=True.py
+-rw-r--r--   0        0        0     3997 2020-02-02 00:00:00.000000 cercis-0.1.6/tests/data/configurable_cases/indentation/use_spaces/closing_bracket_no_extra_indent/base_indent_spaces=3/fdei=True_olcei=False.py
+-rw-r--r--   0        0        0     4083 2020-02-02 00:00:00.000000 cercis-0.1.6/tests/data/configurable_cases/indentation/use_spaces/closing_bracket_no_extra_indent/base_indent_spaces=3/fdei=True_olcei=True.py
+-rw-r--r--   0        0        0     4082 2020-02-02 00:00:00.000000 cercis-0.1.6/tests/data/configurable_cases/indentation/use_spaces/closing_bracket_no_extra_indent/base_indent_spaces=4/fdei=False_olcei=False.py
+-rw-r--r--   0        0        0     4197 2020-02-02 00:00:00.000000 cercis-0.1.6/tests/data/configurable_cases/indentation/use_spaces/closing_bracket_no_extra_indent/base_indent_spaces=4/fdei=False_olcei=True.py
+-rw-r--r--   0        0        0     4257 2020-02-02 00:00:00.000000 cercis-0.1.6/tests/data/configurable_cases/indentation/use_spaces/closing_bracket_no_extra_indent/base_indent_spaces=4/fdei=True_olcei=False.py
+-rw-r--r--   0        0        0     4372 2020-02-02 00:00:00.000000 cercis-0.1.6/tests/data/configurable_cases/indentation/use_spaces/closing_bracket_no_extra_indent/base_indent_spaces=4/fdei=True_olcei=True.py
+-rw-r--r--   0        0        0     4946 2020-02-02 00:00:00.000000 cercis-0.1.6/tests/data/configurable_cases/indentation/use_spaces/closing_bracket_no_extra_indent/base_indent_spaces=8/fdei=False_olcei=False.py
+-rw-r--r--   0        0        0     5177 2020-02-02 00:00:00.000000 cercis-0.1.6/tests/data/configurable_cases/indentation/use_spaces/closing_bracket_no_extra_indent/base_indent_spaces=8/fdei=False_olcei=True.py
+-rw-r--r--   0        0        0     5297 2020-02-02 00:00:00.000000 cercis-0.1.6/tests/data/configurable_cases/indentation/use_spaces/closing_bracket_no_extra_indent/base_indent_spaces=8/fdei=True_olcei=False.py
+-rw-r--r--   0        0        0     5528 2020-02-02 00:00:00.000000 cercis-0.1.6/tests/data/configurable_cases/indentation/use_spaces/closing_bracket_no_extra_indent/base_indent_spaces=8/fdei=True_olcei=True.py
+-rw-r--r--   0        0        0     3449 2020-02-02 00:00:00.000000 cercis-0.1.6/tests/data/configurable_cases/indentation/use_tabs/closing_bracket_extra_indent/fdei=False_olcei=False.py
+-rw-r--r--   0        0        0     3482 2020-02-02 00:00:00.000000 cercis-0.1.6/tests/data/configurable_cases/indentation/use_tabs/closing_bracket_extra_indent/fdei=False_olcei=True.py
+-rw-r--r--   0        0        0     3502 2020-02-02 00:00:00.000000 cercis-0.1.6/tests/data/configurable_cases/indentation/use_tabs/closing_bracket_extra_indent/fdei=True_olcei=False.py
+-rw-r--r--   0        0        0     3535 2020-02-02 00:00:00.000000 cercis-0.1.6/tests/data/configurable_cases/indentation/use_tabs/closing_bracket_extra_indent/fdei=True_olcei=True.py
+-rw-r--r--   0        0        0     3434 2020-02-02 00:00:00.000000 cercis-0.1.6/tests/data/configurable_cases/indentation/use_tabs/closing_bracket_no_extra_indent/fdei=False_olcei=False.py
+-rw-r--r--   0        0        0     3462 2020-02-02 00:00:00.000000 cercis-0.1.6/tests/data/configurable_cases/indentation/use_tabs/closing_bracket_no_extra_indent/fdei=False_olcei=True.py
+-rw-r--r--   0        0        0     3477 2020-02-02 00:00:00.000000 cercis-0.1.6/tests/data/configurable_cases/indentation/use_tabs/closing_bracket_no_extra_indent/fdei=True_olcei=False.py
+-rw-r--r--   0        0        0     3505 2020-02-02 00:00:00.000000 cercis-0.1.6/tests/data/configurable_cases/indentation/use_tabs/closing_bracket_no_extra_indent/fdei=True_olcei=True.py
+-rw-r--r--   0        0        0     1448 2020-02-02 00:00:00.000000 cercis-0.1.6/tests/data/configurable_cases/indentation/use_tabs/line_length_calculation/tab_width_1.py
+-rw-r--r--   0        0        0     1453 2020-02-02 00:00:00.000000 cercis-0.1.6/tests/data/configurable_cases/indentation/use_tabs/line_length_calculation/tab_width_2.py
+-rw-r--r--   0        0        0     1458 2020-02-02 00:00:00.000000 cercis-0.1.6/tests/data/configurable_cases/indentation/use_tabs/line_length_calculation/tab_width_3.py
+-rw-r--r--   0        0        0     1463 2020-02-02 00:00:00.000000 cercis-0.1.6/tests/data/configurable_cases/indentation/use_tabs/line_length_calculation/tab_width_4.py
+-rw-r--r--   0        0        0     1468 2020-02-02 00:00:00.000000 cercis-0.1.6/tests/data/configurable_cases/indentation/use_tabs/line_length_calculation/tab_width_5.py
+-rw-r--r--   0        0        0     1475 2020-02-02 00:00:00.000000 cercis-0.1.6/tests/data/configurable_cases/indentation/use_tabs/line_length_calculation/tab_width_8.py
+-rw-r--r--   0        0        0     1556 2020-02-02 00:00:00.000000 cercis-0.1.6/tests/data/configurable_cases/keep_blank_lines_in_brackets/false.py
+-rw-r--r--   0        0        0     1579 2020-02-02 00:00:00.000000 cercis-0.1.6/tests/data/configurable_cases/keep_blank_lines_in_brackets/true.py
+-rw-r--r--   0        0        0      190 2020-02-02 00:00:00.000000 cercis-0.1.6/tests/data/configurable_cases/line_with_comments/case_False_False.py
+-rw-r--r--   0        0        0      190 2020-02-02 00:00:00.000000 cercis-0.1.6/tests/data/configurable_cases/line_with_comments/case_False_True.py
+-rw-r--r--   0        0        0      397 2020-02-02 00:00:00.000000 cercis-0.1.6/tests/data/configurable_cases/line_with_comments/case_True_False.py
+-rw-r--r--   0        0        0      403 2020-02-02 00:00:00.000000 cercis-0.1.6/tests/data/configurable_cases/line_with_comments/case_True_True.py
+-rw-r--r--   0        0        0      863 2020-02-02 00:00:00.000000 cercis-0.1.6/tests/data/configurable_cases/line_with_long_string/edge_cases.py
+-rw-r--r--   0        0        0    11060 2020-02-02 00:00:00.000000 cercis-0.1.6/tests/data/configurable_cases/line_with_long_string/long_strings_flag_disabled__Black_default.py
+-rw-r--r--   0        0        0    22087 2020-02-02 00:00:00.000000 cercis-0.1.6/tests/data/configurable_cases/line_with_long_string/long_strings_flag_disabled__Cercis_default.py
+-rw-r--r--   0        0        0     6138 2020-02-02 00:00:00.000000 cercis-0.1.6/tests/data/configurable_cases/line_with_long_string/test_cases__Black_default.py
+-rw-r--r--   0        0        0     6056 2020-02-02 00:00:00.000000 cercis-0.1.6/tests/data/configurable_cases/line_with_long_string/test_cases__Cercis_default.py
+-rw-r--r--   0        0        0     6193 2020-02-02 00:00:00.000000 cercis-0.1.6/tests/data/configurable_cases/nested_brackets/nested_brackets__Black_default.py
+-rw-r--r--   0        0        0     2832 2020-02-02 00:00:00.000000 cercis-0.1.6/tests/data/configurable_cases/nested_brackets/nested_brackets__Cercis_default.py
+-rw-r--r--   0        0        0     2011 2020-02-02 00:00:00.000000 cercis-0.1.6/tests/data/configurable_cases/nested_brackets/nested_brackets_explodes__Black_default.py
+-rw-r--r--   0        0        0     2212 2020-02-02 00:00:00.000000 cercis-0.1.6/tests/data/configurable_cases/nested_brackets/nested_brackets_explodes__Cercis_default.py
+-rw-r--r--   0        0        0     7699 2020-02-02 00:00:00.000000 cercis-0.1.6/tests/data/configurable_cases/pragma_comments/Black_default.py
+-rw-r--r--   0        0        0     7703 2020-02-02 00:00:00.000000 cercis-0.1.6/tests/data/configurable_cases/pragma_comments/Black_default_2.py
+-rw-r--r--   0        0        0    10763 2020-02-02 00:00:00.000000 cercis-0.1.6/tests/data/configurable_cases/pragma_comments/Cercis_default.py
+-rw-r--r--   0        0        0    10787 2020-02-02 00:00:00.000000 cercis-0.1.6/tests/data/configurable_cases/pragma_comments/Cercis_default_2.py
+-rw-r--r--   0        0        0     7702 2020-02-02 00:00:00.000000 cercis-0.1.6/tests/data/configurable_cases/single_quote/docstring.py
+-rw-r--r--   0        0        0      140 2020-02-02 00:00:00.000000 cercis-0.1.6/tests/data/configurable_cases/single_quote/docstring_no_extra_empty_line_before_eof.py
+-rw-r--r--   0        0        0     3513 2020-02-02 00:00:00.000000 cercis-0.1.6/tests/data/configurable_cases/single_quote/docstring_preview.py
+-rw-r--r--   0        0        0      745 2020-02-02 00:00:00.000000 cercis-0.1.6/tests/data/configurable_cases/single_quote/more_quotes.py
+-rw-r--r--   0        0        0      845 2020-02-02 00:00:00.000000 cercis-0.1.6/tests/data/configurable_cases/single_quote/string_prefixes.py
+-rw-r--r--   0        0        0     2279 2020-02-02 00:00:00.000000 cercis-0.1.6/tests/data/configurable_cases/single_quote/torture.py
+-rw-r--r--   0        0        0      498 2020-02-02 00:00:00.000000 cercis-0.1.6/tests/data/fast/pep_572_do_not_remove_parens.py
+-rw-r--r--   0        0        0        5 2020-02-02 00:00:00.000000 cercis-0.1.6/tests/data/gitignore_used_on_multiple_sources/.gitignore
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 cercis-0.1.6/tests/data/gitignore_used_on_multiple_sources/dir1/a.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 cercis-0.1.6/tests/data/gitignore_used_on_multiple_sources/dir1/b.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 cercis-0.1.6/tests/data/gitignore_used_on_multiple_sources/dir2/a.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 cercis-0.1.6/tests/data/gitignore_used_on_multiple_sources/dir2/b.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 cercis-0.1.6/tests/data/ignore_subfolders_gitignore_tests/a.py
+-rw-r--r--   0        0        0        4 2020-02-02 00:00:00.000000 cercis-0.1.6/tests/data/ignore_subfolders_gitignore_tests/subdir/.gitignore
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 cercis-0.1.6/tests/data/ignore_subfolders_gitignore_tests/subdir/b.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 cercis-0.1.6/tests/data/ignore_subfolders_gitignore_tests/subdir/subdir/c.py
+-rw-r--r--   0        0        0       14 2020-02-02 00:00:00.000000 cercis-0.1.6/tests/data/include_exclude_tests/.gitignore
+-rw-r--r--   0        0        0      114 2020-02-02 00:00:00.000000 cercis-0.1.6/tests/data/include_exclude_tests/pyproject.toml
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 cercis-0.1.6/tests/data/include_exclude_tests/b/.definitely_exclude/a.pie
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 cercis-0.1.6/tests/data/include_exclude_tests/b/.definitely_exclude/a.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 cercis-0.1.6/tests/data/include_exclude_tests/b/.definitely_exclude/a.pyi
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 cercis-0.1.6/tests/data/include_exclude_tests/b/dont_exclude/a.pie
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 cercis-0.1.6/tests/data/include_exclude_tests/b/dont_exclude/a.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 cercis-0.1.6/tests/data/include_exclude_tests/b/dont_exclude/a.pyi
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 cercis-0.1.6/tests/data/include_exclude_tests/b/exclude/a.pie
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 cercis-0.1.6/tests/data/include_exclude_tests/b/exclude/a.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 cercis-0.1.6/tests/data/include_exclude_tests/b/exclude/a.pyi
+-rw-r--r--   0        0        0        2 2020-02-02 00:00:00.000000 cercis-0.1.6/tests/data/invalid_gitignore_tests/.gitignore
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 cercis-0.1.6/tests/data/invalid_gitignore_tests/a.py
+-rw-r--r--   0        0        0       89 2020-02-02 00:00:00.000000 cercis-0.1.6/tests/data/invalid_gitignore_tests/pyproject.toml
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 cercis-0.1.6/tests/data/invalid_nested_gitignore_tests/a.py
+-rw-r--r--   0        0        0       89 2020-02-02 00:00:00.000000 cercis-0.1.6/tests/data/invalid_nested_gitignore_tests/pyproject.toml
+-rw-r--r--   0        0        0        2 2020-02-02 00:00:00.000000 cercis-0.1.6/tests/data/invalid_nested_gitignore_tests/a/.gitignore
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 cercis-0.1.6/tests/data/invalid_nested_gitignore_tests/a/a.py
+-rw-r--r--   0        0        0      436 2020-02-02 00:00:00.000000 cercis-0.1.6/tests/data/jupyter/non_python_notebook.ipynb
+-rw-r--r--   0        0        0      371 2020-02-02 00:00:00.000000 cercis-0.1.6/tests/data/jupyter/notebook_empty_metadata.ipynb
+-rw-r--r--   0        0        0      641 2020-02-02 00:00:00.000000 cercis-0.1.6/tests/data/jupyter/notebook_no_trailing_newline.ipynb
+-rw-r--r--   0        0        0      642 2020-02-02 00:00:00.000000 cercis-0.1.6/tests/data/jupyter/notebook_trailing_newline.ipynb
+-rw-r--r--   0        0        0        4 2020-02-02 00:00:00.000000 cercis-0.1.6/tests/data/jupyter/notebook_which_cant_be_parsed.ipynb
+-rw-r--r--   0        0        0      761 2020-02-02 00:00:00.000000 cercis-0.1.6/tests/data/jupyter/notebook_without_changes.ipynb
+-rw-r--r--   0        0        0      495 2020-02-02 00:00:00.000000 cercis-0.1.6/tests/data/miscellaneous/async_as_identifier.py
+-rw-r--r--   0        0        0      255 2020-02-02 00:00:00.000000 cercis-0.1.6/tests/data/miscellaneous/blackd_diff.diff
+-rw-r--r--   0        0        0       98 2020-02-02 00:00:00.000000 cercis-0.1.6/tests/data/miscellaneous/blackd_diff.py
+-rw-r--r--   0        0        0    15604 2020-02-02 00:00:00.000000 cercis-0.1.6/tests/data/miscellaneous/debug_visitor.out
+-rw-r--r--   0        0        0     1193 2020-02-02 00:00:00.000000 cercis-0.1.6/tests/data/miscellaneous/debug_visitor.py
+-rw-r--r--   0        0        0     1774 2020-02-02 00:00:00.000000 cercis-0.1.6/tests/data/miscellaneous/decorators.py
+-rw-r--r--   0        0        0     3601 2020-02-02 00:00:00.000000 cercis-0.1.6/tests/data/miscellaneous/docstring_no_string_normalization.py
+-rw-r--r--   0        0        0      357 2020-02-02 00:00:00.000000 cercis-0.1.6/tests/data/miscellaneous/docstring_preview_no_string_normalization.py
+-rw-r--r--   0        0        0    15711 2020-02-02 00:00:00.000000 cercis-0.1.6/tests/data/miscellaneous/expression_skip_magic_trailing_comma.diff
+-rw-r--r--   0        0        0      626 2020-02-02 00:00:00.000000 cercis-0.1.6/tests/data/miscellaneous/force_py36.py
+-rw-r--r--   0        0        0      793 2020-02-02 00:00:00.000000 cercis-0.1.6/tests/data/miscellaneous/force_pyi.py
+-rw-r--r--   0        0        0       59 2020-02-02 00:00:00.000000 cercis-0.1.6/tests/data/miscellaneous/invalid_header.py
+-rw-r--r--   0        0        0      101 2020-02-02 00:00:00.000000 cercis-0.1.6/tests/data/miscellaneous/linelength6.py
+-rw-r--r--   0        0        0    11583 2020-02-02 00:00:00.000000 cercis-0.1.6/tests/data/miscellaneous/long_strings_flag_disabled.py
+-rw-r--r--   0        0        0      293 2020-02-02 00:00:00.000000 cercis-0.1.6/tests/data/miscellaneous/missing_final_newline.diff
+-rw-r--r--   0        0        0      145 2020-02-02 00:00:00.000000 cercis-0.1.6/tests/data/miscellaneous/missing_final_newline.py
+-rw-r--r--   0        0        0      284 2020-02-02 00:00:00.000000 cercis-0.1.6/tests/data/miscellaneous/nested_class_stub.pyi
+-rw-r--r--   0        0        0      279 2020-02-02 00:00:00.000000 cercis-0.1.6/tests/data/miscellaneous/pattern_matching_invalid.py
+-rw-r--r--   0        0        0       69 2020-02-02 00:00:00.000000 cercis-0.1.6/tests/data/miscellaneous/power_op_newline.py
+-rw-r--r--   0        0        0      758 2020-02-02 00:00:00.000000 cercis-0.1.6/tests/data/miscellaneous/python2_detection.py
+-rw-r--r--   0        0        0     2361 2020-02-02 00:00:00.000000 cercis-0.1.6/tests/data/miscellaneous/string_quotes.py
+-rw-r--r--   0        0        0     2266 2020-02-02 00:00:00.000000 cercis-0.1.6/tests/data/miscellaneous/stub.pyi
+-rw-r--r--   0        0        0      114 2020-02-02 00:00:00.000000 cercis-0.1.6/tests/data/nested_gitignore_tests/pyproject.toml
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 cercis-0.1.6/tests/data/nested_gitignore_tests/x.py
+-rw-r--r--   0        0        0        5 2020-02-02 00:00:00.000000 cercis-0.1.6/tests/data/nested_gitignore_tests/root/.gitignore
+-rw-r--r--   0        0        0       39 2020-02-02 00:00:00.000000 cercis-0.1.6/tests/data/nested_gitignore_tests/root/a.py
+-rw-r--r--   0        0        0       21 2020-02-02 00:00:00.000000 cercis-0.1.6/tests/data/nested_gitignore_tests/root/b.py
+-rw-r--r--   0        0        0       21 2020-02-02 00:00:00.000000 cercis-0.1.6/tests/data/nested_gitignore_tests/root/c.py
+-rw-r--r--   0        0        0        5 2020-02-02 00:00:00.000000 cercis-0.1.6/tests/data/nested_gitignore_tests/root/child/.gitignore
+-rw-r--r--   0        0        0       39 2020-02-02 00:00:00.000000 cercis-0.1.6/tests/data/nested_gitignore_tests/root/child/a.py
+-rw-r--r--   0        0        0       40 2020-02-02 00:00:00.000000 cercis-0.1.6/tests/data/nested_gitignore_tests/root/child/b.py
+-rw-r--r--   0        0        0       21 2020-02-02 00:00:00.000000 cercis-0.1.6/tests/data/nested_gitignore_tests/root/child/c.py
+-rw-r--r--   0        0        0      279 2020-02-02 00:00:00.000000 cercis-0.1.6/tests/data/preview/async_stmts.py
+-rw-r--r--   0        0        0     4107 2020-02-02 00:00:00.000000 cercis-0.1.6/tests/data/preview/cantfit.py
+-rw-r--r--   0        0        0     8294 2020-02-02 00:00:00.000000 cercis-0.1.6/tests/data/preview/comments7.py
+-rw-r--r--   0        0        0      613 2020-02-02 00:00:00.000000 cercis-0.1.6/tests/data/preview/format_unicode_escape_seq.py
+-rw-r--r--   0        0        0     2784 2020-02-02 00:00:00.000000 cercis-0.1.6/tests/data/preview/long_dict_values.py
+-rw-r--r--   0        0        0    33216 2020-02-02 00:00:00.000000 cercis-0.1.6/tests/data/preview/long_strings.py
+-rw-r--r--   0        0        0     1418 2020-02-02 00:00:00.000000 cercis-0.1.6/tests/data/preview/long_strings__east_asian_width.py
+-rw-r--r--   0        0        0     6536 2020-02-02 00:00:00.000000 cercis-0.1.6/tests/data/preview/long_strings__edge_case.py
+-rw-r--r--   0        0        0    45897 2020-02-02 00:00:00.000000 cercis-0.1.6/tests/data/preview/long_strings__regression.py
+-rw-r--r--   0        0        0     1105 2020-02-02 00:00:00.000000 cercis-0.1.6/tests/data/preview/long_strings__type_annotations.py
+-rw-r--r--   0        0        0     7207 2020-02-02 00:00:00.000000 cercis-0.1.6/tests/data/preview/multiline_strings.py
+-rw-r--r--   0        0        0      810 2020-02-02 00:00:00.000000 cercis-0.1.6/tests/data/preview/no_blank_line_before_docstring.py
+-rw-r--r--   0        0        0      481 2020-02-02 00:00:00.000000 cercis-0.1.6/tests/data/preview/percent_precedence.py
+-rw-r--r--   0        0        0     2525 2020-02-02 00:00:00.000000 cercis-0.1.6/tests/data/preview/prefer_rhs_split.py
+-rw-r--r--   0        0        0      342 2020-02-02 00:00:00.000000 cercis-0.1.6/tests/data/preview/return_annotation_brackets_string.py
+-rw-r--r--   0        0        0      655 2020-02-02 00:00:00.000000 cercis-0.1.6/tests/data/preview/trailing_comma.py
+-rw-r--r--   0        0        0     1140 2020-02-02 00:00:00.000000 cercis-0.1.6/tests/data/preview_context_managers/targeting_py38.py
+-rw-r--r--   0        0        0     3361 2020-02-02 00:00:00.000000 cercis-0.1.6/tests/data/preview_context_managers/targeting_py39.py
+-rw-r--r--   0        0        0      595 2020-02-02 00:00:00.000000 cercis-0.1.6/tests/data/preview_context_managers/auto_detect/features_3_10.py
+-rw-r--r--   0        0        0      553 2020-02-02 00:00:00.000000 cercis-0.1.6/tests/data/preview_context_managers/auto_detect/features_3_11.py
+-rw-r--r--   0        0        0     1058 2020-02-02 00:00:00.000000 cercis-0.1.6/tests/data/preview_context_managers/auto_detect/features_3_8.py
+-rw-r--r--   0        0        0      623 2020-02-02 00:00:00.000000 cercis-0.1.6/tests/data/preview_context_managers/auto_detect/features_3_9.py
+-rw-r--r--   0        0        0      133 2020-02-02 00:00:00.000000 cercis-0.1.6/tests/data/project_metadata/both_pyproject.toml
+-rw-r--r--   0        0        0       74 2020-02-02 00:00:00.000000 cercis-0.1.6/tests/data/project_metadata/neither_pyproject.toml
+-rw-r--r--   0        0        0      101 2020-02-02 00:00:00.000000 cercis-0.1.6/tests/data/project_metadata/only_black_pyproject.toml
+-rw-r--r--   0        0        0      106 2020-02-02 00:00:00.000000 cercis-0.1.6/tests/data/project_metadata/only_metadata_pyproject.toml
+-rw-r--r--   0        0        0      765 2020-02-02 00:00:00.000000 cercis-0.1.6/tests/data/py_310/parenthesized_context_managers.py
+-rw-r--r--   0        0        0     2668 2020-02-02 00:00:00.000000 cercis-0.1.6/tests/data/py_310/pattern_matching_complex.py
+-rw-r--r--   0        0        0     1965 2020-02-02 00:00:00.000000 cercis-0.1.6/tests/data/py_310/pattern_matching_extras.py
+-rw-r--r--   0        0        0     3066 2020-02-02 00:00:00.000000 cercis-0.1.6/tests/data/py_310/pattern_matching_generic.py
+-rw-r--r--   0        0        0     2641 2020-02-02 00:00:00.000000 cercis-0.1.6/tests/data/py_310/pattern_matching_simple.py
+-rw-r--r--   0        0        0     1061 2020-02-02 00:00:00.000000 cercis-0.1.6/tests/data/py_310/pattern_matching_style.py
+-rw-r--r--   0        0        0      491 2020-02-02 00:00:00.000000 cercis-0.1.6/tests/data/py_310/pep_572_py310.py
+-rw-r--r--   0        0        0      509 2020-02-02 00:00:00.000000 cercis-0.1.6/tests/data/py_310/remove_newline_after_match.py
+-rw-r--r--   0        0        0      380 2020-02-02 00:00:00.000000 cercis-0.1.6/tests/data/py_310/starred_for_target.py
+-rw-r--r--   0        0        0     2114 2020-02-02 00:00:00.000000 cercis-0.1.6/tests/data/py_311/pep_646.py
+-rw-r--r--   0        0        0      972 2020-02-02 00:00:00.000000 cercis-0.1.6/tests/data/py_311/pep_654.py
+-rw-r--r--   0        0        0     2033 2020-02-02 00:00:00.000000 cercis-0.1.6/tests/data/py_311/pep_654_style.py
+-rw-r--r--   0        0        0      597 2020-02-02 00:00:00.000000 cercis-0.1.6/tests/data/py_36/numeric_literals.py
+-rw-r--r--   0        0        0      267 2020-02-02 00:00:00.000000 cercis-0.1.6/tests/data/py_36/numeric_literals_skip_underscores.py
+-rw-r--r--   0        0        0     1199 2020-02-02 00:00:00.000000 cercis-0.1.6/tests/data/py_37/python37.py
+-rw-r--r--   0        0        0      740 2020-02-02 00:00:00.000000 cercis-0.1.6/tests/data/py_38/pep_570.py
+-rw-r--r--   0        0        0      970 2020-02-02 00:00:00.000000 cercis-0.1.6/tests/data/py_38/pep_572.py
+-rw-r--r--   0        0        0     1895 2020-02-02 00:00:00.000000 cercis-0.1.6/tests/data/py_38/pep_572_remove_parens.py
+-rw-r--r--   0        0        0      834 2020-02-02 00:00:00.000000 cercis-0.1.6/tests/data/py_38/python38.py
+-rw-r--r--   0        0        0      251 2020-02-02 00:00:00.000000 cercis-0.1.6/tests/data/py_39/pep_572_py39.py
+-rw-r--r--   0        0        0      696 2020-02-02 00:00:00.000000 cercis-0.1.6/tests/data/py_39/python39.py
+-rw-r--r--   0        0        0     2575 2020-02-02 00:00:00.000000 cercis-0.1.6/tests/data/py_39/remove_with_brackets.py
+-rw-r--r--   0        0        0      907 2020-02-02 00:00:00.000000 cercis-0.1.6/tests/data/simple_cases/attribute_access_on_number_literals.py
+-rw-r--r--   0        0        0       63 2020-02-02 00:00:00.000000 cercis-0.1.6/tests/data/simple_cases/beginning_backslash.py
+-rw-r--r--   0        0        0      333 2020-02-02 00:00:00.000000 cercis-0.1.6/tests/data/simple_cases/bracketmatch.py
+-rw-r--r--   0        0        0     1091 2020-02-02 00:00:00.000000 cercis-0.1.6/tests/data/simple_cases/class_blank_parentheses.py
+-rw-r--r--   0        0        0     4318 2020-02-02 00:00:00.000000 cercis-0.1.6/tests/data/simple_cases/class_methods_new_line.py
+-rw-r--r--   0        0        0     3294 2020-02-02 00:00:00.000000 cercis-0.1.6/tests/data/simple_cases/collections.py
+-rw-r--r--   0        0        0      212 2020-02-02 00:00:00.000000 cercis-0.1.6/tests/data/simple_cases/comment_after_escaped_newline.py
+-rw-r--r--   0        0        0     1909 2020-02-02 00:00:00.000000 cercis-0.1.6/tests/data/simple_cases/comments.py
+-rw-r--r--   0        0        0     7639 2020-02-02 00:00:00.000000 cercis-0.1.6/tests/data/simple_cases/comments2.py
+-rw-r--r--   0        0        0     1573 2020-02-02 00:00:00.000000 cercis-0.1.6/tests/data/simple_cases/comments3.py
+-rw-r--r--   0        0        0     3536 2020-02-02 00:00:00.000000 cercis-0.1.6/tests/data/simple_cases/comments4.py
+-rw-r--r--   0        0        0     1196 2020-02-02 00:00:00.000000 cercis-0.1.6/tests/data/simple_cases/comments5.py
+-rw-r--r--   0        0        0     2567 2020-02-02 00:00:00.000000 cercis-0.1.6/tests/data/simple_cases/comments6.py
+-rw-r--r--   0        0        0      300 2020-02-02 00:00:00.000000 cercis-0.1.6/tests/data/simple_cases/comments8.py
+-rw-r--r--   0        0        0     5279 2020-02-02 00:00:00.000000 cercis-0.1.6/tests/data/simple_cases/comments9.py
+-rw-r--r--   0        0        0      994 2020-02-02 00:00:00.000000 cercis-0.1.6/tests/data/simple_cases/comments_non_breaking_space.py
+-rw-r--r--   0        0        0     5597 2020-02-02 00:00:00.000000 cercis-0.1.6/tests/data/simple_cases/composition.py
+-rw-r--r--   0        0        0    11198 2020-02-02 00:00:00.000000 cercis-0.1.6/tests/data/simple_cases/composition_no_trailing_comma.py
+-rw-r--r--   0        0        0     7699 2020-02-02 00:00:00.000000 cercis-0.1.6/tests/data/simple_cases/docstring.py
+-rw-r--r--   0        0        0      140 2020-02-02 00:00:00.000000 cercis-0.1.6/tests/data/simple_cases/docstring_no_extra_empty_line_before_eof.py
+-rw-r--r--   0        0        0     3513 2020-02-02 00:00:00.000000 cercis-0.1.6/tests/data/simple_cases/docstring_preview.py
+-rw-r--r--   0        0        0     4596 2020-02-02 00:00:00.000000 cercis-0.1.6/tests/data/simple_cases/empty_lines.py
+-rw-r--r--   0        0        0    15801 2020-02-02 00:00:00.000000 cercis-0.1.6/tests/data/simple_cases/expression.diff
+-rw-r--r--   0        0        0    18624 2020-02-02 00:00:00.000000 cercis-0.1.6/tests/data/simple_cases/expression.py
+-rw-r--r--   0        0        0     9681 2020-02-02 00:00:00.000000 cercis-0.1.6/tests/data/simple_cases/fmtonoff.py
+-rw-r--r--   0        0        0      604 2020-02-02 00:00:00.000000 cercis-0.1.6/tests/data/simple_cases/fmtonoff2.py
+-rw-r--r--   0        0        0      251 2020-02-02 00:00:00.000000 cercis-0.1.6/tests/data/simple_cases/fmtonoff3.py
+-rw-r--r--   0        0        0      278 2020-02-02 00:00:00.000000 cercis-0.1.6/tests/data/simple_cases/fmtonoff4.py
+-rw-r--r--   0        0        0     3627 2020-02-02 00:00:00.000000 cercis-0.1.6/tests/data/simple_cases/fmtonoff5.py
+-rw-r--r--   0        0        0      277 2020-02-02 00:00:00.000000 cercis-0.1.6/tests/data/simple_cases/fmtpass_imports.py
+-rw-r--r--   0        0        0       40 2020-02-02 00:00:00.000000 cercis-0.1.6/tests/data/simple_cases/fmtskip.py
+-rw-r--r--   0        0        0      555 2020-02-02 00:00:00.000000 cercis-0.1.6/tests/data/simple_cases/fmtskip2.py
+-rw-r--r--   0        0        0      362 2020-02-02 00:00:00.000000 cercis-0.1.6/tests/data/simple_cases/fmtskip3.py
+-rw-r--r--   0        0        0       92 2020-02-02 00:00:00.000000 cercis-0.1.6/tests/data/simple_cases/fmtskip4.py
+-rw-r--r--   0        0        0      301 2020-02-02 00:00:00.000000 cercis-0.1.6/tests/data/simple_cases/fmtskip5.py
+-rw-r--r--   0        0        0      235 2020-02-02 00:00:00.000000 cercis-0.1.6/tests/data/simple_cases/fmtskip6.py
+-rw-r--r--   0        0        0      356 2020-02-02 00:00:00.000000 cercis-0.1.6/tests/data/simple_cases/fmtskip7.py
+-rw-r--r--   0        0        0     1705 2020-02-02 00:00:00.000000 cercis-0.1.6/tests/data/simple_cases/fmtskip8.py
+-rw-r--r--   0        0        0      989 2020-02-02 00:00:00.000000 cercis-0.1.6/tests/data/simple_cases/fstring.py
+-rw-r--r--   0        0        0     6482 2020-02-02 00:00:00.000000 cercis-0.1.6/tests/data/simple_cases/function.py
+-rw-r--r--   0        0        0     2427 2020-02-02 00:00:00.000000 cercis-0.1.6/tests/data/simple_cases/function2.py
+-rw-r--r--   0        0        0     3657 2020-02-02 00:00:00.000000 cercis-0.1.6/tests/data/simple_cases/function_trailing_comma.py
+-rw-r--r--   0        0        0     2542 2020-02-02 00:00:00.000000 cercis-0.1.6/tests/data/simple_cases/import_spacing.py
+-rw-r--r--   0        0        0      674 2020-02-02 00:00:00.000000 cercis-0.1.6/tests/data/simple_cases/one_element_subscript.py
+-rw-r--r--   0        0        0     3359 2020-02-02 00:00:00.000000 cercis-0.1.6/tests/data/simple_cases/power_op_spacing.py
+-rw-r--r--   0        0        0     1106 2020-02-02 00:00:00.000000 cercis-0.1.6/tests/data/simple_cases/prefer_rhs_split_reformatted.py
+-rw-r--r--   0        0        0     3205 2020-02-02 00:00:00.000000 cercis-0.1.6/tests/data/simple_cases/remove_await_parens.py
+-rw-r--r--   0        0        0     2025 2020-02-02 00:00:00.000000 cercis-0.1.6/tests/data/simple_cases/remove_except_parens.py
+-rw-r--r--   0        0        0     1460 2020-02-02 00:00:00.000000 cercis-0.1.6/tests/data/simple_cases/remove_for_brackets.py
+-rw-r--r--   0        0        0     3351 2020-02-02 00:00:00.000000 cercis-0.1.6/tests/data/simple_cases/remove_newline_after_code_block_open.py
+-rw-r--r--   0        0        0     3493 2020-02-02 00:00:00.000000 cercis-0.1.6/tests/data/simple_cases/remove_parens.py
+-rw-r--r--   0        0        0     5141 2020-02-02 00:00:00.000000 cercis-0.1.6/tests/data/simple_cases/return_annotation_brackets.py
+-rw-r--r--   0        0        0     1398 2020-02-02 00:00:00.000000 cercis-0.1.6/tests/data/simple_cases/skip_magic_trailing_comma.py
+-rw-r--r--   0        0        0      787 2020-02-02 00:00:00.000000 cercis-0.1.6/tests/data/simple_cases/slices.py
+-rw-r--r--   0        0        0      845 2020-02-02 00:00:00.000000 cercis-0.1.6/tests/data/simple_cases/string_prefixes.py
+-rw-r--r--   0        0        0     2279 2020-02-02 00:00:00.000000 cercis-0.1.6/tests/data/simple_cases/torture.py
+-rw-r--r--   0        0        0     1615 2020-02-02 00:00:00.000000 cercis-0.1.6/tests/data/simple_cases/trailing_comma_optional_parens1.py
+-rw-r--r--   0        0        0      248 2020-02-02 00:00:00.000000 cercis-0.1.6/tests/data/simple_cases/trailing_comma_optional_parens2.py
+-rw-r--r--   0        0        0      967 2020-02-02 00:00:00.000000 cercis-0.1.6/tests/data/simple_cases/trailing_comma_optional_parens3.py
+-rw-r--r--   0        0        0     2123 2020-02-02 00:00:00.000000 cercis-0.1.6/tests/data/simple_cases/trailing_commas_in_leading_parts.py
+-rw-r--r--   0        0        0       80 2020-02-02 00:00:00.000000 cercis-0.1.6/tests/data/simple_cases/tricky_unicode_symbols.py
+-rw-r--r--   0        0        0      510 2020-02-02 00:00:00.000000 cercis-0.1.6/tests/data/simple_cases/tupleassign.py
+-rw-r--r--   0        0        0       27 2020-02-02 00:00:00.000000 cercis-0.1.6/tests/data/simple_cases/whitespace.py
+-rw-r--r--   0        0        0      101 2020-02-02 00:00:00.000000 cercis-0.1.6/tests/data/type_comments/type_comment_syntax_error.py
+-rw-r--r--   0        0        0      273 2020-02-02 00:00:00.000000 cercis-0.1.6/.gitignore
+-rw-r--r--   0        0        0     1061 2020-02-02 00:00:00.000000 cercis-0.1.6/LICENSE
+-rw-r--r--   0        0        0     1080 2020-02-02 00:00:00.000000 cercis-0.1.6/LICENSE_ORIGINAL
+-rw-r--r--   0        0        0     7134 2020-02-02 00:00:00.000000 cercis-0.1.6/pyproject.toml
+-rw-r--r--   0        0        0    27277 2020-02-02 00:00:00.000000 cercis-0.1.6/PKG-INFO
```

### Comparing `cercis-0.1.5/.pre-commit-config.yaml` & `cercis-0.1.6/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `cercis-0.1.5/.pre-commit-hooks.yaml` & `cercis-0.1.6/.pre-commit-hooks.yaml`

 * *Files identical despite different names*

### Comparing `cercis-0.1.5/CHANGELOG.md` & `cercis-0.1.6/CHANGELOG.md`

 * *Files 24% similar despite different names*

```diff
@@ -1,16 +1,25 @@
 # Change Log
 
+## [0.1.6] - 2023-05-23
+
+- Added
+  - A new option `--wrap-comments` to not wrap any comments (not just pragma comments)
+  - A new option `--keep-blank-lines-in-brackets`
+- Changed
+  - Improved the CLI output text colors because the current colors are confusing or not
+    quite legible
+
 ## [0.1.5] - 2023-05-09
 
 - Added
-  - Configurability to use tabs instead of spaces (two new options:
-    `--use-tabs` and `--tab-width`)
-  - Configurability on base indentation spaces and extra indentation at
-    different line continuation situations
+  - Configurability to use tabs instead of spaces (two new options: `--use-tabs` and
+    `--tab-width`)
+  - Configurability on base indentation spaces and extra indentation at different line
+    continuation situations
 
 ## [0.1.4] - 2023-05-07
 
 - Added
   - A new configurable option: `--closing-bracket-extra-indent`
 
 ## [0.1.3] - 2023-05-07
@@ -28,34 +37,32 @@
 
 - Removed
   - Some unrelated documentation and config files
 
 ## [0.1.2] - 2023-05-04
 
 - Added
-  - Merged 2 changes from psf/black:main
-    ([#5](https://github.com/jsh9/cercis/pull/5))
+  - Merged 2 changes from psf/black:main ([#5](https://github.com/jsh9/cercis/pull/5))
   - Added option to not wrap "simple" lines with long strings
     ([#6](https://github.com/jsh9/cercis/pull/6))
 - Full changelog
   - https://github.com/jsh9/cercis/compare/0.1.1...0.1.2
 
 ## [0.1.1] - 2023-05-03
 
 - Added
-  - A configurable option: `single-quote`, for formatting code into single
-    quotes
+  - A configurable option: `single-quote`, for formatting code into single quotes
 - Full changelog
   - https://github.com/jsh9/cercis/compare/0.1.0...0.1.1
 
 ## [0.1.0] - 2023-04-30
 
 - This is the initial version that branches away from Black (commit:
   [e712e4](https://github.com/psf/black/commit/e712e48e06420d9240ce95c81acfcf6f11d14c83))
 - Changed
-  - The default indentation within a function definition (when line wrap
-    happens) is now 8 spaces. (Black's default is 4, which is
+  - The default indentation within a function definition (when line wrap happens) is now
+    8 spaces. (Black's default is 4, which is
     [not PEP8-compatible](https://github.com/psf/black/issues/1127))
   - Updated README, because `cercis` now branches away from Black
 - Added
-  - A configurable option (`function-definition-extra-indent`) is added instead
-    of enforcing 8 spaces for everyone
+  - A configurable option (`function-definition-extra-indent`) is added instead of
+    enforcing 8 spaces for everyone
```

### Comparing `cercis-0.1.5/Dockerfile` & `cercis-0.1.6/Dockerfile`

 * *Files identical despite different names*

### Comparing `cercis-0.1.5/README.md` & `cercis-0.1.6/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -1,44 +1,40 @@
 # _Cercis_
 
 [![](https://upload.wikimedia.org/wikipedia/commons/thumb/4/4c/Red_bud_2009.jpg/320px-Red_bud_2009.jpg)](https://en.wikipedia.org/wiki/Cercis)
 
-_**Cercis**_ /ˈsɜːrsɪs/ is a Python code formatter that is more configurable
-than [Black](https://github.com/psf/black) (a popular Python code formatter).
+_**Cercis**_ /ˈsɜːrsɪs/ is a Python code formatter that is more configurable than
+[Black](https://github.com/psf/black) (a popular Python code formatter).
 
-[_Cercis_](https://en.wikipedia.org/wiki/Cercis) is also the name of a
-deciduous tree that boasts vibrant pink to purple-hued flowers, which bloom in
-early spring.
+[_Cercis_](https://en.wikipedia.org/wiki/Cercis) is also the name of a deciduous tree
+that boasts vibrant pink to purple-hued flowers, which bloom in early spring.
 
 This code repository is forked from and directly inspired by
-[Black](https://github.com/psf/black). The original license of Black is
-included in this repository (see [LICENSE_ORIGINAL](./LICENSE_ORIGINAL)).
+[Black](https://github.com/psf/black). The original license of Black is included in this
+repository (see [LICENSE_ORIGINAL](./LICENSE_ORIGINAL)).
 
-_Cercis_ inherited Black's very comprehensive test cases, which means we are
-confident that our configurability addition does not introduce any undesirable
-side effects. We also thoroughly tested every configurable options that we
-added.
-
-In particular, via its configurable options, _Cercis_ can completely fall back
-to Black. See [Section 4.5](#45-how-to-fall-back-to-blacks-behavior) below for
-more details.
+_Cercis_ inherited Black's very comprehensive test cases, which means we are confident
+that our configurability addition does not introduce any undesirable side effects. We
+also thoroughly tested every configurable options that we added.
+
+In particular, via its configurable options, _Cercis_ can completely fall back to Black.
+See [Section 4.5](#45-how-to-fall-back-to-blacks-behavior) below for more details.
 
 ## 1. Motivations
 
-While we like the idea of auto-formatting and code readability, we take issue
-with some style choices and the lack of configurability of the Black formatter.
-Therefore, _Cercis_ aims at providing some configurability beyond Black's
-limited offering.
+While we like the idea of auto-formatting and code readability, we take issue with some
+style choices and the lack of configurability of the Black formatter. Therefore,
+_Cercis_ aims at providing some configurability beyond Black's limited offering.
 
 ## 2. Installation and usage
 
 ### 2.1. Installation
 
-_Cercis_ can be installed by running `pip install cercis`. It requires Python
-3.7+ to run. If you want to format Jupyter Notebooks, install with
+_Cercis_ can be installed by running `pip install cercis`. It requires Python 3.7+ to
+run. If you want to format Jupyter Notebooks, install with
 `pip install "cercis[jupyter]"`.
 
 ### 2.2. Usage
 
 #### 2.2.1. Command line usage
 
 To get started right away with sensible defaults:
@@ -53,17 +49,16 @@
 python -m cercis {source_file_or_directory}
 ```
 
 The commands above reformat entire file(s) in place.
 
 #### 2.2.2. As pre-commit hook
 
-To format Python files (.py), put the following into your
-`.pre-commit-config.yaml` file. Remember to replace `<VERSION>` with your
-version of this tool (such as `v0.1.0`):
+To format Python files (.py), put the following into your `.pre-commit-config.yaml`
+file. Remember to replace `<VERSION>` with your version of this tool (such as `v0.1.0`):
 
 ```yaml
 - repo: https://github.com/jsh9/cercis
   rev: <VERSION>
   hooks:
     - id: cercis
       args: [--line-length=88]
@@ -76,48 +71,47 @@
 - repo: https://github.com/jsh9/cercis
   rev: <VERSION>
   hooks:
     - id: cercis-jupyter
       args: [--line-length=88]
 ```
 
-See [pre-commit](https://github.com/pre-commit/pre-commit) for more
-instructions. In particular,
-[here](https://pre-commit.com/#passing-arguments-to-hooks) is how to specify
+See [pre-commit](https://github.com/pre-commit/pre-commit) for more instructions. In
+particular, [here](https://pre-commit.com/#passing-arguments-to-hooks) is how to specify
 arguments in pre-commit config.
 
 ## 3. _Cercis_'s code style
 
 _Cercis_'s code style is largely consistent with the
 [style of of Black](https://black.readthedocs.io/en/stable/the_black_code_style/current_style.html).
 
-The main difference is that _Cercis_ provides several configurable options that
-Black doesn't. Configurability is our main motivation behind creating _Cercis_.
+The main difference is that _Cercis_ provides several configurable options that Black
+doesn't. Configurability is our main motivation behind creating _Cercis_.
 
 _Cercis_ offers the following configurable options:
 
 1. [Line length](#31-line-length)
 2. [Single quote vs double quote](#32-single-quote-vs-double-quote)
 3. [Tabs vs spaces](#33-tabs-vs-spaces)
 4. [Base indentation spaces](#34-base-indentation-spaces)
 5. [Extra indentation at line continuation](#35-extra-indentation-at-line-continuation)
    1. [At function definition](#351-at-function-definition---function-definition-extra-indent)
    2. [In other line continuations](#352-in-other-line-continuations---other-line-continuation-extra-indent)
    3. [At closing brackets](#353-at-closing-brackets---closing-bracket-extra-indent)
 6. ["Simple" lines with long strings](#36-simple-lines-with-long-strings)
 7. [Collapse nested brackets](#37-collapse-nested-brackets)
-8. [Wrap pragma comments](#38-wrapping-long-lines-ending-with-pragma-comments)
+8. [Wrap lines ending with comments](#38-wrapping-long-lines-ending-with-comments)
+9. [Keep blank lines in brackets](#39-keep-blank-lines-in-brackets)
 
-The next section ([How to configure _Cercis_](#4-how-to-configure-cercis))
-contains detailed instructions of how to configure these options.
+The next section ([How to configure _Cercis_](#4-how-to-configure-cercis)) contains
+detailed instructions of how to configure these options.
 
 ### 3.1. Line length
 
-_Cercis_ uses 79 characters as the line length limit, instead of 88 (Black's
-default).
+_Cercis_ uses 79 characters as the line length limit, instead of 88 (Black's default).
 
 You can override this default if necessary.
 
 | Option                 |                                           |
 | ---------------------- | ----------------------------------------- |
 | Name                   | `--line-length`                           |
 | Abbreviation           | `-l`                                      |
@@ -125,16 +119,16 @@
 | Black's default        | 88                                        |
 | Command line usage     | `cercis -l=120 myScript.py`               |
 | `pyproject.toml` usage | `line-length = 120` under `[tool.cercis]` |
 | `pre-commit` usage     | `args: [--line-length=120]`               |
 
 ### 3.2. Single quote vs double quote
 
-_Cercis_ uses single quotes (`'`) as the default for strings, instead of double
-quotes (`"`) which is Black's default.
+_Cercis_ uses single quotes (`'`) as the default for strings, instead of double quotes
+(`"`) which is Black's default.
 
 You can override this default if necessary.
 
 | Option                 |                                              |
 | ---------------------- | -------------------------------------------- |
 | Name                   | `--single-quote`                             |
 | Abbreviation           | `-sq`                                        |
@@ -158,35 +152,34 @@
 | Abbreviation           | `-tab`                                   |
 | Default                | `False`                                  |
 | Black's default        | `False`                                  |
 | Command line usage     | `cercis -tab=True myScript.py`           |
 | `pyproject.toml` usage | `use-tabs = false` under `[tool.cercis]` |
 | `pre-commit` usage     | `args: [--use-tabs=False]`               |
 
-- `--tab-width` (int): when calculating line length (to determine whether to
-  wrap lines), how wide shall _Cercis_ treat each tab. Only effective when
-  `--use-tabs` is set to `True`.
+- `--tab-width` (int): when calculating line length (to determine whether to wrap
+  lines), how wide shall _Cercis_ treat each tab. Only effective when `--use-tabs` is
+  set to `True`.
 
 | Option                 |                                       |
 | ---------------------- | ------------------------------------- |
 | Name                   | `--tab-width`                         |
 | Abbreviation           | `-tw`                                 |
 | Default                | 4                                     |
 | Black's default        | N/A                                   |
 | Command line usage     | `cercis -tab=True -tw=2 myScript.py`  |
 | `pyproject.toml` usage | `tab-width = 2` under `[tool.cercis]` |
 | `pre-commit` usage     | `args: [--tab-width=2]`               |
 
 ### 3.4. Base indentation spaces
 
-This option defines the number of spaces that each indentation level adds. This
-option has no effect when `--use-tabs` is set to `True`.
+This option defines the number of spaces that each indentation level adds. This option
+has no effect when `--use-tabs` is set to `True`.
 
-For example, if you set it to 2, contents within a `for` block is indented 2
-spaces:
+For example, if you set it to 2, contents within a `for` block is indented 2 spaces:
 
 ```python
 for i in (1, 2, 3, 4, 5):
   print(i)
 ```
 
 | Option                 |                                                     |
@@ -203,17 +196,16 @@
 
 There are three associated options:
 
 - `--function-definition-extra-indent`
 - `--other-line-continuation-extra-indent`
 - `--closing-bracket-extra-indent`
 
-They control whether we add an **additional** indentation level in some
-situations. Note that these options can work well with tabs
-(`--use-tabs=True`).
+They control whether we add an **additional** indentation level in some situations. Note
+that these options can work well with tabs (`--use-tabs=True`).
 
 #### 3.5.1. At function definition (`--function-definition-extra-indent`)
 
 <table>
   <tr>
     <td>
 
@@ -244,55 +236,53 @@
 ```
 
   </td>
 
   </tr>
 </table>
 
-We choose to add an extra indentation level when wrapping a function signature
-line. This is because `def␣` happens to be 4 characters, so when the base
-indentation is 4 spaces, it can be difficult to visually distinguish the
-function name and the argument list if we don't add an extra indentation.
+We choose to add an extra indentation level when wrapping a function signature line.
+This is because `def␣` happens to be 4 characters, so when the base indentation is 4
+spaces, it can be difficult to visually distinguish the function name and the argument
+list if we don't add an extra indentation.
 
-If you set `--base-indentation-spaces` to other values than 4, this visual
-separation issue will disappear, and you may not need to turn this option on.
+If you set `--base-indentation-spaces` to other values than 4, this visual separation
+issue will disappear, and you may not need to turn this option on.
 
-This style is encouraged
-[in PEP8](https://peps.python.org/pep-0008/#indentation).
+This style is encouraged [in PEP8](https://peps.python.org/pep-0008/#indentation).
 
 | Option                 |                                                                 |
 | ---------------------- | --------------------------------------------------------------- |
 | Name                   | `--function-definition-extra-indent`                            |
 | Abbreviation           | `-fdei`                                                         |
 | Default                | `True`                                                          |
 | Black's default        | `False`                                                         |
 | Command line usage     | `cercis -fdei=False myScript.py`                                |
 | `pyproject.toml` usage | `function-definition-extra-indent = true` under `[tool.cercis]` |
 | `pre-commit` usage     | `args: [--function-definition-extra-indent=False]`              |
 
 #### 3.5.2. In other line continuations (`--other-line-continuation-extra-indent`)
 
-"Other line continuations" are cases other than in function definitions, such
-as:
+"Other line continuations" are cases other than in function definitions, such as:
 
 ```python
 var = some_function(
     arg1_with_long_name,
     arg2_with_longer_name,
 )
 
 var2 = [
     'something',
     'something else',
     'something more',
 ]
 ```
 
-So if you set this option (`--other-line-continuation-extra-indent`) to `True`,
-you can add an extra level of indentation in these cases:
+So if you set this option (`--other-line-continuation-extra-indent`) to `True`, you can
+add an extra level of indentation in these cases:
 
 ```python
 var = some_function(
         arg1_with_long_name,
         arg2_with_longer_name,
 )
 
@@ -311,17 +301,16 @@
 | Black's default        | `False`                                                             |
 | Command line usage     | `cercis -olcei=True myScript.py`                                    |
 | `pyproject.toml` usage | `other-line-continuation-extra-indent = true` under `[tool.cercis]` |
 | `pre-commit` usage     | `args: [----other-line-continuation-extra-indent=False]`            |
 
 #### 3.5.3. At closing brackets (`--closing-bracket-extra-indent`)
 
-This option lets people customize where the closing bracket should be. Note
-that both styles are OK according to
-[PEP8](https://peps.python.org/pep-0008/#indentation).
+This option lets people customize where the closing bracket should be. Note that both
+styles are OK according to [PEP8](https://peps.python.org/pep-0008/#indentation).
 
 <table>
   <tr>
     <td>
 
 ```python
 # --closing-bracket-extra-indent=False
@@ -390,17 +379,16 @@
 | Black's default        | `False`                                                     |
 | Command line usage     | `cercis -cbei=True myScript.py`                             |
 | `pyproject.toml` usage | `closing-bracket-extra-indent = true` under `[tool.cercis]` |
 | `pre-commit` usage     | `args: [--closing-bracket-extra-indent=False]`              |
 
 ### 3.6. "Simple" lines with long strings
 
-By default, Black wraps lines that exceed length limit. But for very simple
-lines (such as assigning a long string to a variable), line wrapping is not
-necessary.
+By default, Black wraps lines that exceed length limit. But for very simple lines (such
+as assigning a long string to a variable), line wrapping is not necessary.
 
 <table>
   <tr>
     <td>
 
 ```python
 # Cercis's default style
@@ -531,155 +519,195 @@
 | Command line usage     | `cercis -cnb=True myScript.py`                          |
 | `pyproject.toml` usage | `collapse-nested-brackets = true` under `[tool.cercis]` |
 | `pre-commit` usage     | `args: [--collapse-nested-brackets=False]`              |
 
 The code implementation of this option comes from
 [Pyink](https://github.com/google/pyink), another forked project from Black.
 
-### 3.8. Wrapping long lines ending with pragma comments
+### 3.8. Wrapping long lines ending with comments
+
+Sometimes we have lines that exceed the length limit only because of the in-line
+comment. If we do not want to wrap those lines, we can use two options provided here:
 
-"Pragma comments", in this context, mean the directives for Python linters
-usually to tell them to ignore certain errors. Pragma comments that _Cercis_
-currently recognizes include:
+- `--wrap-comments`
+- `--wrap-pragma-comments`
+
+"Pragma comments", in this context, mean the directives for Python linters usually to
+tell them to ignore certain errors. Pragma comments that _Cercis_ currently recognizes
+include:
 
 - _noqa_: `# noqa: E501`
 - _type: ignore_: `# type: ignore[no-untyped-def]`
 - _pylint_: `# pylint: disable=protected-access`
 - _pytype_: `# pytype: disable=attribute-error`
 
-<table>
-  <tr>
-    <td>
+| Option                 |                                              |
+| ---------------------- | -------------------------------------------- |
+| Name                   | `--wrap-comments`                            |
+| Abbreviation           | `-wc`                                        |
+| Default                | `False`                                      |
+| Black's style          | `True`                                       |
+| Command line usage     | `cercis -wc=True myScript.py`                |
+| `pyproject.toml` usage | `wrap-comments = true` under `[tool.cercis]` |
+| `pre-commit` usage     | `args: [--wrap-comments=False]`              |
 
-```python
-# Cercis's default style
-# (Suppose line length limit is 30)
+| Option                 |                                                     |
+| ---------------------- | --------------------------------------------------- |
+| Name                   | `--wrap-pragma-comments`                            |
+| Abbreviation           | `-wpc`                                              |
+| Default                | `False`                                             |
+| Black's style          | `True`                                              |
+| Command line usage     | `cercis -wpc=True myScript.py`                      |
+| `pyproject.toml` usage | `wrap-pragma-comments = true` under `[tool.cercis]` |
+| `pre-commit` usage     | `args: [--wrap-pragma-comments=False]`              |
+
+And below is a 2x2 matrix to explain how these two options work together:
+
+|              | `-wc=True`                          | `-wc=False`             |
+| ------------ | ----------------------------------- | ----------------------- |
+| `-wpc=True`  | All comments wrapped w.n.           | No comments are wrapped |
+| `-wpc=False` | p.c. not wrapped; o.c. wrapped w.n. | No comments are wrapped |
 
-# This line has 30 characters
-var = some_func(some_long_arg)  # noqa:F501
+Note:
 
-# This line has 31 characters
-var_ = some_func(
-    some_long_arg
-)  # type: ignore
-
-# Cercis doesn't wraps a line if its main
-# content (without the comment) does not
-# exceed the line length limit.
+- "w.n." means "when necessary"
+- "p.c." means "pragma comments"
+- "o.c." means "other comments"
 
+### 3.9. Keep blank lines in brackets
 
+This option allows us to keep the blank lines that we intentionally add into the
+contents of brackets.
 
+<table>
+  <tr>
+    <td>
+
+Cercis's default style:
 
+```python
+my_list = [
+    # Group 1
+    1,
+    2,
 
+    # Group 2
+    3,
+    4,
+
+    # Group 3
+    5,
+    6,
+]
 ```
 
   </td>
 
   <td>
 
+Black's default style (not configurable):
+
 ```python
-# Black's style (not configurable)
-# (Suppose line length limit is 30)
+my_list = [
+    # Group 1
+    1,
+    2,
+    # Group 2
+    3,
+    4,
+    # Group 3
+    5,
+    6,
+]
+
 
-# Black doesn't wrap lines, no matter
-# how long, if the line has
-# a "# type: ignore..." comment.
-# (This line has 31 characters.)
-var_ = some_func(some_long_arg)  # type: ignore
-
-# Black does not recognize "# type:ignore",
-# even though mypy recognizes it.
-var_ = some_func(
-    some_long_arg
-)  # type:ignore
-
-# Black only recognizes "# type: ignore"
-var_ = some_func(
-    some_long_arg
-)  # noqa:F501
 ```
 
   </td>
 
   </tr>
 </table>
 
-| Option                 |                                                     |
-| ---------------------- | --------------------------------------------------- |
-| Name                   | `--wrap-pragma-comments`                            |
-| Abbreviation           | `-wpc`                                              |
-| Default                | `False`                                             |
-| Black's style          | `True`                                              |
-| Command line usage     | `cercis -wpc=True myScript.py`                      |
-| `pyproject.toml` usage | `wrap-pragma-comments = true` under `[tool.cercis]` |
-| `pre-commit` usage     | `args: [--wrap-pragma-comments=False]`              |
+| Option                 |                                                             |
+| ---------------------- | ----------------------------------------------------------- |
+| Name                   | `--keep-blank-lines-in-brackets`                            |
+| Abbreviation           | `-kblib`                                                    |
+| Default                | `True`                                                      |
+| Black's style          | `False`                                                     |
+| Command line usage     | `cercis -kblib=True myScript.py`                            |
+| `pyproject.toml` usage | `keep-blank-lines-in-brackets = true` under `[tool.cercis]` |
+| `pre-commit` usage     | `args: [--keep-blank-lines-in-bracketss=False]`             |
+
+(Note: if `--keep-blank-lines-in-brackets` is `True`, multiple consecutive blank lines
+are compressed into one blank line after formatting.)
 
 ## 4. How to configure _Cercis_
 
 ### 4.1. Dynamically in the command line
 
 Here are some examples:
 
 - `cercis --single-quote=True myScript.py` to format files to single quotes
-- `cercis --function-definition-extra-indent=False myScript.py` to format files
-  without extra indentation at function definition
-- `cercis --line-length=79 myScript.py` to format files with a line length of
-  79 characters
+- `cercis --function-definition-extra-indent=False myScript.py` to format files without
+  extra indentation at function definition
+- `cercis --line-length=79 myScript.py` to format files with a line length of 79
+  characters
 
 ### 4.2. In your project's `pyproject.toml` file
 
 You can specify the options under the `[tool.cercis]` section of the file:
 
 ```toml
 [tool.cercis]
 line-length = 88
 function-definition-extra-indent = true
 single-quote = false
 ```
 
 ### 4.3. In your project's `.pre-commit-config.yaml` file
 
-You can specify the options under the `args` section of your
-`.pre-commit-config.yaml` file.
+You can specify the options under the `args` section of your `.pre-commit-config.yaml`
+file.
 
 For example:
 
 ```yaml
 repos:
   - repo: https://github.com/jsh9/cercis
     rev: 0.1.0
     hooks:
       - id: cercis
-        args: [--function-definition-extra-indent=False, --ling-length=79]
+        args: [--function-definition-extra-indent=False, --line-length=79]
   - repo: https://github.com/jsh9/cercis
     rev: 0.1.0
     hooks:
       - id: cercis-jupyter
         args: [--function-definition-extra-indent=False, --line-length=79]
 ```
 
-The value in `rev` can be any _Cercis_ release, or it can be `main`, which
-means to always use the latest (including unreleased) _Cercis_ features.
+The value in `rev` can be any _Cercis_ release, or it can be `main`, which means to
+always use the latest (including unreleased) _Cercis_ features.
 
 ### 4.4. Specify options in `tox.ini`
 
-Currently, _Cercis_ does not support a config section in `tox.ini`. Instead,
-you can specify the options in `pyproject.toml`.
+Currently, _Cercis_ does not support a config section in `tox.ini`. Instead, you can
+specify the options in `pyproject.toml`.
 
 ### 4.5. How to fall back to Black's behavior
 
-Here are the configuration options to fall back to Black's behavior. Put them
-in `pyproject.toml`:
+Here are the configuration options to fall back to Black's behavior. Put them in
+`pyproject.toml`:
 
 ```toml
 [tool.cercis]
 line-length = 88
 single-quote = false
 use-tabs = false
 base-indentation-spaces = 4
 function-definition-extra-indent = false
 other-line-continuation-extra-indent = false
 closing-bracket-extra-indent = false
 wrap-line-with-long-string = true
 collapse-nested-brackets = false
+wrap-comments = true
 wrap-pragma-comments = true
 ```
```

### Comparing `cercis-0.1.5/action.yml` & `cercis-0.1.6/action.yml`

 * *Files 14% similar despite different names*

```diff
@@ -29,19 +29,20 @@
     default: ""
 branding:
   color: "cercis"
   icon: "check-circle"
 runs:
   using: composite
   steps:
-    - run: |
+    - name: black
+      run: |
         if [ "$RUNNER_OS" == "Windows" ]; then
-          python $GITHUB_ACTION_PATH/action/main.py
+          python $GITHUB_ACTION_PATH/action/main.py | tee -a $GITHUB_STEP_SUMMARY
         else
-          python3 $GITHUB_ACTION_PATH/action/main.py
+          python3 $GITHUB_ACTION_PATH/action/main.py | tee -a $GITHUB_STEP_SUMMARY
         fi
       env:
         # TODO: Remove once https://github.com/actions/runner/issues/665 is fixed.
         INPUT_OPTIONS: ${{ inputs.options }}
         INPUT_SRC: ${{ inputs.src }}
         INPUT_JUPYTER: ${{ inputs.jupyter }}
         INPUT_BLACK_ARGS: ${{ inputs.black_args }}
```

### Comparing `cercis-0.1.5/mypy.ini` & `cercis-0.1.6/mypy.ini`

 * *Files identical despite different names*

### Comparing `cercis-0.1.5/tox.ini` & `cercis-0.1.6/tox.ini`

 * *Files identical despite different names*

### Comparing `cercis-0.1.5/.github/PULL_REQUEST_TEMPLATE.md` & `cercis-0.1.6/.github/PULL_REQUEST_TEMPLATE.md`

 * *Files identical despite different names*

### Comparing `cercis-0.1.5/.github/dependabot.yml` & `cercis-0.1.6/.github/dependabot.yml`

 * *Files identical despite different names*

### Comparing `cercis-0.1.5/.github/ISSUE_TEMPLATE/bug_report.md` & `cercis-0.1.6/.github/ISSUE_TEMPLATE/bug_report.md`

 * *Files identical despite different names*

### Comparing `cercis-0.1.5/.github/ISSUE_TEMPLATE/config.yml` & `cercis-0.1.6/.github/ISSUE_TEMPLATE/config.yml`

 * *Files identical despite different names*

### Comparing `cercis-0.1.5/.github/ISSUE_TEMPLATE/docs-issue.md` & `cercis-0.1.6/.github/ISSUE_TEMPLATE/docs-issue.md`

 * *Files identical despite different names*

### Comparing `cercis-0.1.5/.github/ISSUE_TEMPLATE/feature_request.md` & `cercis-0.1.6/.github/ISSUE_TEMPLATE/feature_request.md`

 * *Files identical despite different names*

### Comparing `cercis-0.1.5/.github/ISSUE_TEMPLATE/style_issue.md` & `cercis-0.1.6/.github/ISSUE_TEMPLATE/style_issue.md`

 * *Files identical despite different names*

### Comparing `cercis-0.1.5/.github/workflows/check-changelog.yml` & `cercis-0.1.6/.github/workflows/check-changelog.yml`

 * *Files identical despite different names*

### Comparing `cercis-0.1.5/.github/workflows/docker.yml` & `cercis-0.1.6/.github/workflows/docker.yml`

 * *Files identical despite different names*

### Comparing `cercis-0.1.5/.github/workflows/fuzz.yml` & `cercis-0.1.6/.github/workflows/fuzz.yml`

 * *Files identical despite different names*

### Comparing `cercis-0.1.5/.github/workflows/lint.yml` & `cercis-0.1.6/.github/workflows/lint.yml`

 * *Files identical despite different names*

### Comparing `cercis-0.1.5/.github/workflows/python-package.yml` & `cercis-0.1.6/.github/workflows/python-package.yml`

 * *Files identical despite different names*

### Comparing `cercis-0.1.5/.github/workflows/python-publish.yml` & `cercis-0.1.6/.github/workflows/python-publish.yml`

 * *Files identical despite different names*

### Comparing `cercis-0.1.5/.github/workflows/test.yml` & `cercis-0.1.6/.github/workflows/test.yml`

 * *Files identical despite different names*

### Comparing `cercis-0.1.5/.github/workflows/upload_binary.yml` & `cercis-0.1.6/.github/workflows/upload_binary.yml`

 * *Files identical despite different names*

### Comparing `cercis-0.1.5/.github/workflows/version-check.yml` & `cercis-0.1.6/.github/workflows/version-check.yml`

 * *Files identical despite different names*

### Comparing `cercis-0.1.5/action/main.py` & `cercis-0.1.6/action/main.py`

 * *Files 7% similar despite different names*

```diff
@@ -28,15 +28,15 @@
     describe_name = ""
     with open(ACTION_PATH / ".git_archival.txt", encoding="utf-8") as fp:
         for line in fp:
             if line.startswith("describe-name: "):
                 describe_name = line[len("describe-name: ") :].rstrip()
                 break
     if not describe_name:
-        print("::error::Failed to detect action version.", flush=True)
+        print("::error::Failed to detect action version.", file=sys.stderr, flush=True)
         sys.exit(1)
     # expected format is one of:
     # - 23.1.0
     # - 23.1.0-51-g448bba7
     if describe_name.count("-") < 2:
         # the action's commit matches a tag exactly, install exact version from PyPI
         req = f"cercis{extra_deps}=={describe_name}"
@@ -49,19 +49,29 @@
     stdout=PIPE,
     stderr=STDOUT,
     encoding="utf-8",
     cwd=ACTION_PATH,
 )
 if pip_proc.returncode:
     print(pip_proc.stdout)
-    print("::error::Failed to install Black.", flush=True)
+    print("::error::Failed to install Black.", file=sys.stderr, flush=True)
     sys.exit(pip_proc.returncode)
 
 
 base_cmd = [str(ENV_BIN / "cercis")]
 if BLACK_ARGS:
     # TODO: remove after a while since this is deprecated in favour of SRC + OPTIONS.
-    proc = run([*base_cmd, *shlex.split(BLACK_ARGS)])
+    proc = run(
+        [*base_cmd, *shlex.split(BLACK_ARGS)],
+        stdout=PIPE,
+        stderr=STDOUT,
+        encoding="utf-8",
+    )
 else:
-    proc = run([*base_cmd, *shlex.split(OPTIONS), *shlex.split(SRC)])
-
+    proc = run(
+        [*base_cmd, *shlex.split(OPTIONS), *shlex.split(SRC)],
+        stdout=PIPE,
+        stderr=STDOUT,
+        encoding="utf-8",
+    )
+print(proc.stdout)
 sys.exit(proc.returncode)
```

### Comparing `cercis-0.1.5/autoload/black.vim` & `cercis-0.1.6/autoload/black.vim`

 * *Files identical despite different names*

### Comparing `cercis-0.1.5/gallery/README.md` & `cercis-0.1.6/gallery/README.md`

 * *Files 14% similar despite different names*

```diff
@@ -1,12 +1,11 @@
 # Gallery
 
-Gallery is a script that automates the process of applying different _Black_
-versions to a selected PyPI package and seeing the results between _Black_
-versions.
+Gallery is a script that automates the process of applying different _Black_ versions to
+a selected PyPI package and seeing the results between _Black_ versions.
 
 ## Build
 
 ```console
 $ docker build -t black_gallery .
 ```
```

### Comparing `cercis-0.1.5/gallery/gallery.py` & `cercis-0.1.6/gallery/gallery.py`

 * *Files identical despite different names*

### Comparing `cercis-0.1.5/plugin/black.vim` & `cercis-0.1.6/plugin/black.vim`

 * *Files identical despite different names*

### Comparing `cercis-0.1.5/scripts/check_version_and_changelog.py` & `cercis-0.1.6/scripts/check_version_and_changelog.py`

 * *Files identical despite different names*

### Comparing `cercis-0.1.5/scripts/diff_shades_gha_helper.py` & `cercis-0.1.6/scripts/diff_shades_gha_helper.py`

 * *Files identical despite different names*

### Comparing `cercis-0.1.5/scripts/fuzz.py` & `cercis-0.1.6/scripts/fuzz.py`

 * *Files identical despite different names*

### Comparing `cercis-0.1.5/scripts/make_width_table.py` & `cercis-0.1.6/scripts/make_width_table.py`

 * *Files identical despite different names*

### Comparing `cercis-0.1.5/scripts/migrate-black.py` & `cercis-0.1.6/scripts/migrate-black.py`

 * *Files identical despite different names*

### Comparing `cercis-0.1.5/src/blackd/__init__.py` & `cercis-0.1.6/src/blackd/__init__.py`

 * *Files identical despite different names*

### Comparing `cercis-0.1.5/src/blackd/middlewares.py` & `cercis-0.1.6/src/blackd/middlewares.py`

 * *Files identical despite different names*

### Comparing `cercis-0.1.5/src/blib2to3/Grammar.txt` & `cercis-0.1.6/src/blib2to3/Grammar.txt`

 * *Files identical despite different names*

### Comparing `cercis-0.1.5/src/blib2to3/LICENSE` & `cercis-0.1.6/src/blib2to3/LICENSE`

 * *Files identical despite different names*

### Comparing `cercis-0.1.5/src/blib2to3/PatternGrammar.txt` & `cercis-0.1.6/src/blib2to3/PatternGrammar.txt`

 * *Files identical despite different names*

### Comparing `cercis-0.1.5/src/blib2to3/README` & `cercis-0.1.6/src/blib2to3/README`

 * *Files identical despite different names*

### Comparing `cercis-0.1.5/src/blib2to3/pygram.py` & `cercis-0.1.6/src/blib2to3/pygram.py`

 * *Files identical despite different names*

### Comparing `cercis-0.1.5/src/blib2to3/pytree.py` & `cercis-0.1.6/src/blib2to3/pytree.py`

 * *Files identical despite different names*

### Comparing `cercis-0.1.5/src/blib2to3/pgen2/conv.py` & `cercis-0.1.6/src/blib2to3/pgen2/conv.py`

 * *Files identical despite different names*

### Comparing `cercis-0.1.5/src/blib2to3/pgen2/driver.py` & `cercis-0.1.6/src/blib2to3/pgen2/driver.py`

 * *Files identical despite different names*

### Comparing `cercis-0.1.5/src/blib2to3/pgen2/grammar.py` & `cercis-0.1.6/src/blib2to3/pgen2/grammar.py`

 * *Files identical despite different names*

### Comparing `cercis-0.1.5/src/blib2to3/pgen2/literals.py` & `cercis-0.1.6/src/blib2to3/pgen2/literals.py`

 * *Files identical despite different names*

### Comparing `cercis-0.1.5/src/blib2to3/pgen2/parse.py` & `cercis-0.1.6/src/blib2to3/pgen2/parse.py`

 * *Files identical despite different names*

### Comparing `cercis-0.1.5/src/blib2to3/pgen2/pgen.py` & `cercis-0.1.6/src/blib2to3/pgen2/pgen.py`

 * *Files 1% similar despite different names*

```diff
@@ -26,24 +26,23 @@
 
 
 class PgenGrammar(grammar.Grammar):
     pass
 
 
 class ParserGenerator(object):
-
     filename: Path
     stream: IO[Text]
     generator: Iterator[GoodTokenInfo]
     first: Dict[Text, Optional[Dict[Text, int]]]
 
     def __init__(self, filename: Path, stream: Optional[IO[Text]] = None) -> None:
         close_stream = None
         if stream is None:
-            stream = open(filename)
+            stream = open(filename, encoding="utf-8")
             close_stream = stream.close
         self.filename = filename
         self.stream = stream
         self.generator = tokenize.generate_tokens(stream.readline)
         self.gettoken()  # Initialize lookahead
         self.dfas, self.startsymbol = self.parse()
         if close_stream is not None:
```

### Comparing `cercis-0.1.5/src/blib2to3/pgen2/token.py` & `cercis-0.1.6/src/blib2to3/pgen2/token.py`

 * *Files identical despite different names*

### Comparing `cercis-0.1.5/src/blib2to3/pgen2/tokenize.py` & `cercis-0.1.6/src/blib2to3/pgen2/tokenize.py`

 * *Files identical despite different names*

### Comparing `cercis-0.1.5/src/cercis/__init__.py` & `cercis-0.1.6/src/cercis/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -41,19 +41,21 @@
 from cercis.const import (
     DEFAULT_BASE_INDENTATION_SPACES,
     DEFAULT_CLOSING_BRACKET_EXTRA_INDENT,
     DEFAULT_COLLAPSE_NESTED_BRACKETS,
     DEFAULT_EXCLUDES,
     DEFAULT_FUNCTION_DEFINITION_EXTRA_INDENT,
     DEFAULT_INCLUDES,
+    DEFAULT_KEEP_BLANK_LINES_IN_BRACKETS,
     DEFAULT_LINE_LENGTH,
     DEFAULT_OTHER_LINE_CONTINUATION_EXTRA_INDENT,
     DEFAULT_SINGLE_QUOTE,
     DEFAULT_TAB_WIDTH,
     DEFAULT_USE_TABS,
+    DEFAULT_WRAP_COMMENTS,
     DEFAULT_WRAP_LINE_WITH_LONG_STRING,
     DEFAULT_WRAP_PRAGMA_COMMENTS,
     STDIN_PLACEHOLDER,
 )
 from cercis.files import (
     find_project_root,
     find_pyproject_toml,
@@ -218,15 +220,15 @@
     return value
 
 
 @click.command(
     context_settings={"help_option_names": ["-h", "--help"]},
     # While Click does set this field automatically using the docstring, mypyc
     # (annoyingly) strips 'em so we need to set it here too.
-    help="The uncompromising code formatter.",
+    help="Cercis, a more configurable Python code formatter.",
 )
 @click.option("-c", "--code", type=str, help="Format the code passed in as a string.")
 @click.option(
     "-l",
     "--line-length",
     type=int,
     default=DEFAULT_LINE_LENGTH,
@@ -325,26 +327,50 @@
     default=DEFAULT_COLLAPSE_NESTED_BRACKETS,
     help=(
         "If True, collapse nested brackets on one line, instead of exploding"
         " into multiple levels in multiple lines"
     ),
 )
 @click.option(
+    "-wc",
+    "--wrap-comments",
+    type=bool,
+    show_default=True,
+    default=DEFAULT_WRAP_COMMENTS,
+    help=(
+        "If False, do not wrap long lines if the line exceeds length limit"
+        " only because of trailing comments. Black's"
+        " default behavior is 'True'. Note that 'comments' are a superset"
+        " of 'pragma comments', which is controled in --wrap-pragma-comments."
+    ),
+)
+@click.option(
     "-wpc",
     "--wrap-pragma-comments",
     type=bool,
     show_default=True,
     default=DEFAULT_WRAP_PRAGMA_COMMENTS,
     help=(
         "If False, do not wrap long lines if the line exceeds length limit"
         " only because of trailing pragma comments. Black's default behavior"
         " is 'True'."
     ),
 )
 @click.option(
+    "-kblib",
+    "--keep-blank-lines-in-brackets",
+    type=bool,
+    show_default=True,
+    default=DEFAULT_KEEP_BLANK_LINES_IN_BRACKETS,
+    help=(
+        "Preserve single blank lines inside brackets (tuples, lists, "
+        "dictionaries, function arguments, etc.)."
+    ),
+)
+@click.option(
     "-t",
     "--target-version",
     type=click.Choice([v.name.lower() for v in TargetVersion]),
     callback=target_version_option_callback,
     multiple=True,
     help=(
         "Python versions that should be supported by Cercis's output. By default,"
@@ -558,15 +584,17 @@
         code: Optional[str],
         line_length: int,
         function_definition_extra_indent: bool,
         closing_bracket_extra_indent: bool,
         single_quote: bool,
         wrap_line_with_long_string: bool,
         collapse_nested_brackets: bool,
+        wrap_comments: bool,
         wrap_pragma_comments: bool,
+        keep_blank_lines_in_brackets: bool,
         base_indentation_spaces: int,
         other_line_continuation_extra_indent: bool,
         use_tabs: bool,
         tab_width: int,
         target_version: List[TargetVersion],
         check: bool,
         diff: bool,
@@ -588,15 +616,14 @@
         extend_exclude: Optional[Pattern[str]],
         force_exclude: Optional[Pattern[str]],
         stdin_filename: Optional[str],
         workers: Optional[int],
         src: Tuple[str, ...],
         config: Optional[str],
 ) -> None:
-    """The uncompromising code formatter."""
     ctx.ensure_object(dict)
 
     if src and code is not None:
         out(
             main.get_usage(ctx)
             + "\n\n'SRC' and 'code' cannot be passed simultaneously."
         )
@@ -690,15 +717,17 @@
         preview=preview,
         python_cell_magics=set(python_cell_magics),
         function_definition_extra_indent=function_definition_extra_indent,
         closing_bracket_extra_indent=closing_bracket_extra_indent,
         single_quote=single_quote,
         wrap_line_with_long_string=wrap_line_with_long_string,
         collapse_nested_brackets=collapse_nested_brackets,
+        wrap_comments=wrap_comments,
         wrap_pragma_comments=wrap_pragma_comments,
+        keep_blank_lines_in_brackets=keep_blank_lines_in_brackets,
         base_indentation_spaces=base_indentation_spaces,
         other_line_continuation_extra_indent=other_line_continuation_extra_indent,
         use_tabs=use_tabs,
         tab_width=tab_width,
     )
 
     if code is not None:
@@ -756,15 +785,20 @@
                 report=report,
                 workers=workers,
             )
 
     if verbose or not quiet:
         if code is None and (verbose or report.change_count or report.failure_count):
             out()
-        out(error_msg if report.return_code else "All done! ✨ 🍰 ✨")
+
+        if report.return_code:
+            out(error_msg, fg="red")
+        else:
+            out("🎉 All done! 🎉", fg="green")
+
         if code is None:
             click.echo(str(report), err=True)
     ctx.exit(report.return_code)
 
 
 def get_sources(
         *,
```

### Comparing `cercis-0.1.5/src/cercis/_width_table.py` & `cercis-0.1.6/src/cercis/_width_table.py`

 * *Files identical despite different names*

### Comparing `cercis-0.1.5/src/cercis/brackets.py` & `cercis-0.1.6/src/cercis/brackets.py`

 * *Files identical despite different names*

### Comparing `cercis-0.1.5/src/cercis/cache.py` & `cercis-0.1.6/src/cercis/cache.py`

 * *Files identical despite different names*

### Comparing `cercis-0.1.5/src/cercis/comments.py` & `cercis-0.1.6/src/cercis/comments.py`

 * *Files identical despite different names*

### Comparing `cercis-0.1.5/src/cercis/concurrency.py` & `cercis-0.1.6/src/cercis/concurrency.py`

 * *Files identical despite different names*

### Comparing `cercis-0.1.5/src/cercis/const.py` & `cercis-0.1.6/src/cercis/const.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,14 +1,16 @@
 DEFAULT_LINE_LENGTH = 79
-DEFAULT_EXCLUDES = r"/(\.direnv|\.eggs|\.git|\.hg|\.mypy_cache|\.nox|\.tox|\.venv|venv|\.svn|\.ipynb_checkpoints|_build|buck-out|build|dist|__pypackages__)/"  # noqa: B950
+DEFAULT_EXCLUDES = r"/(\.direnv|\.eggs|\.git|\.hg|\.ipynb_checkpoints|\.mypy_cache|\.nox|\.pytest_cache|\.ruff_cache|\.tox|\.svn|\.venv|\.vscode|__pypackages__|_build|buck-out|build|dist|venv)/"  # noqa: B950
 DEFAULT_INCLUDES = r"(\.pyi?|\.ipynb)$"
 STDIN_PLACEHOLDER = "__BLACK_STDIN_FILENAME__"
 DEFAULT_FUNCTION_DEFINITION_EXTRA_INDENT = True
 DEFAULT_CLOSING_BRACKET_EXTRA_INDENT = False
 DEFAULT_SINGLE_QUOTE = True
 DEFAULT_WRAP_LINE_WITH_LONG_STRING = False
 DEFAULT_COLLAPSE_NESTED_BRACKETS = True
+DEFAULT_KEEP_BLANK_LINES_IN_BRACKETS = True
+DEFAULT_WRAP_COMMENTS = False
 DEFAULT_WRAP_PRAGMA_COMMENTS = False
 DEFAULT_BASE_INDENTATION_SPACES = 4
 DEFAULT_OTHER_LINE_CONTINUATION_EXTRA_INDENT = False
 DEFAULT_USE_TABS = False
 DEFAULT_TAB_WIDTH = 4
```

### Comparing `cercis-0.1.5/src/cercis/debug.py` & `cercis-0.1.6/src/cercis/debug.py`

 * *Files identical despite different names*

### Comparing `cercis-0.1.5/src/cercis/files.py` & `cercis-0.1.6/src/cercis/files.py`

 * *Files identical despite different names*

### Comparing `cercis-0.1.5/src/cercis/handle_ipynb_magics.py` & `cercis-0.1.6/src/cercis/handle_ipynb_magics.py`

 * *Files identical despite different names*

### Comparing `cercis-0.1.5/src/cercis/indent.py` & `cercis-0.1.6/src/cercis/indent.py`

 * *Files identical despite different names*

### Comparing `cercis-0.1.5/src/cercis/linegen.py` & `cercis-0.1.6/src/cercis/linegen.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,14 +3,19 @@
 """
 import sys
 from dataclasses import replace
 from enum import Enum, auto
 from functools import partial, wraps
 from typing import Collection, Iterator, List, Optional, Set, Union, cast
 
+if sys.version_info >= (3, 8):
+    from typing import Final
+else:
+    from typing_extensions import Final
+
 from blib2to3.pgen2 import token
 from blib2to3.pytree import Leaf, Node
 from cercis.brackets import (
     COMMA_PRIORITY,
     DOT_PRIORITY,
     get_leaves_inside_matching_brackets,
     max_delimiter_priority_in_atom,
@@ -74,14 +79,16 @@
     StringSplitter,
     Transformer,
     hug_power_op,
 )
 from cercis.utils_line_wrapping import check_eligibility_to_opt_out_of_line_wrapping
 from cercis.utils_linegen import perform_collapse_nested_brackets
 
+COMMENTS: Final = {token.COMMENT, STANDALONE_COMMENT}
+
 # types
 LeafID = int
 LN = Union[Leaf, Node]
 
 
 class CannotSplit(CannotTransform):
     """A readable split that fits the allotted line length is impossible."""
@@ -141,30 +148,61 @@
         self.current_line = Line(mode=self.mode, depth=new_depth)
         yield complete_line
 
     def visit_default(self, node: LN) -> Iterator[Line]:
         """Default `visit_*()` implementation. Recurses to children of `node`."""
         if isinstance(node, Leaf):
             any_open_brackets = self.current_line.bracket_tracker.any_open_brackets()
+
+            append_blank_lines = (
+                any_open_brackets and self.mode.keep_blank_lines_in_brackets
+            )
+
+            if len(self.current_line.leaves) > 0:
+                last_leaf: Optional[Leaf] = self.current_line.leaves[-1]
+            else:
+                last_leaf = None
+
             for comment in generate_comments(node):
+                if (
+                    append_blank_lines
+                    and last_leaf
+                    and last_leaf.type not in OPENING_BRACKETS
+                ):
+                    newlines = comment.prefix.count("\n")
+                    if last_leaf and last_leaf.type in COMMENTS:
+                        newlines += 1
+                    if newlines > 1:
+                        self.current_line.append(Leaf(STANDALONE_COMMENT, ""))
+
                 if any_open_brackets:
                     # any comment within brackets is subject to splitting
                     self.current_line.append(comment)
+                    last_leaf = comment
                 elif comment.type == token.COMMENT:
                     # regular trailing comment
                     self.current_line.append(comment)
                     yield from self.line()
 
                 else:
                     # regular standalone comment
                     yield from self.line()
 
                     self.current_line.append(comment)
                     yield from self.line()
 
+            if (
+                append_blank_lines
+                and last_leaf
+                and last_leaf.type not in OPENING_BRACKETS
+                and node.type not in CLOSING_BRACKETS
+                and node.prefix.split("#")[-1].count("\n") > 1
+            ):
+                self.current_line.append(Leaf(STANDALONE_COMMENT, ""))
+
             normalize_prefix(node, inside_brackets=any_open_brackets)
             if self.mode.string_normalization and node.type == token.STRING:
                 node.value = normalize_string_prefix(node.value)
                 node.value = normalize_string_quotes(
                     node.value,
                     single_quote=self.mode.single_quote,
                 )
```

### Comparing `cercis-0.1.5/src/cercis/lines.py` & `cercis-0.1.6/src/cercis/lines.py`

 * *Files 2% similar despite different names*

```diff
@@ -77,15 +77,19 @@
         Unless `preformatted` is True, the `leaf` will receive a new consistent
         whitespace prefix and metadata applied by :class:`BracketTracker`.
         Trailing commas are maybe removed, unpacked for loop variables are
         demoted from being delimiters.
 
         Inline comments are put aside.
         """
-        has_value = leaf.type in BRACKETS or bool(leaf.value.strip())
+        has_value = (
+            leaf.type in BRACKETS
+            or leaf.type == STANDALONE_COMMENT
+            or bool(leaf.value.strip())
+        )
         if not has_value:
             return
 
         if token.COLON == leaf.type and self.is_class_paren_empty:
             del self.leaves[-2:]
         if self.leaves and not preformatted:
             # Note: at this point leaf.prefix should be empty except for
@@ -325,33 +329,55 @@
             for node in self.leaves[-2:]:
                 for comment in self.comments.get(id(node), []):
                     if is_type_comment(comment, " ignore"):
                         return True
 
         return False
 
-    def trailing_pragma_comment_length(self) -> int:
+    def calc_comment_length(self) -> int:
         """
-        This method comes from the wonderful implementation in Pyink:
+        This method is adapted from the wonderful implementation in Pyink:
         https://github.com/google/pyink/blob/f93771c02e9a26ce9508c59d69c9337c95797eac/src/pyink/lines.py#L316-L328
 
         Pyink is another fork from Black, and inherits Black's MIT license.
         """
         if not self.leaves:
             return 0
 
         last_leaf = self.leaves[-1]
         length = 0
-        for comment in self.comments.get(id(last_leaf), []):
-            # str(comment) contains the whitespace preceding the `#`
-            comment_str = str(comment)
+
+        if id(last_leaf) in self.comments:
+            # In many cases, the ID of the last leaf is the same as one of
+            # the comments.
+            for comment in self.comments.get(id(last_leaf), []):
+                length += self._calc_comment_length_inner(comment)
+        elif len(self.leaves) >= 2 and id(self.leaves[-2]) in self.comments:
+            # In other cases (such as `some_var = some_value  # some comment`),
+            # it's the 2nd to the last leaf that has the same ID as one
+            # of the comments.
+            for comment in self.comments.get(id(self.leaves[-2]), []):
+                length += self._calc_comment_length_inner(comment)
+
+        return length
+
+    def _calc_comment_length_inner(self, comment: Leaf) -> int:
+        comment_str = str(comment)  # contains the whitespace preceding the `#`
+
+        # We need to put this `if` before the other, because `--wrap-comments`
+        # has higher priority than `--wrap-pragma-comments`
+        if not self.mode.wrap_comments:
+            return len(comment_str)
+
+        if not self.mode.wrap_pragma_comments:
             parts = _PRAGMA_REGEX.split(comment_str, maxsplit=1)
             if len(parts) == 3:
-                length += len(parts[1]) + len(parts[2])
-        return length
+                return len(parts[1]) + len(parts[2])
+
+        return 0
 
     def contains_multiline_strings(self) -> bool:
         return any(is_multiline_string(leaf) for leaf in self.leaves)
 
     def has_magic_trailing_comma(
             self, closing: Leaf, ensure_removable: bool = False
     ) -> bool:
@@ -526,14 +552,16 @@
         leaves = iter(self.leaves)
         first = next(leaves)
         res = f"{first.prefix}{indent}{first.value}"
         for leaf in leaves:
             res += str(leaf)
         for comment in itertools.chain.from_iterable(self.comments.values()):
             res += str(comment)
+        if res == indent:
+            res = ""
 
         return res + "\n"
 
     def __bool__(self) -> bool:
         """Return True if the line has leaves or comments."""
         return bool(self.leaves or self.comments)
 
@@ -692,14 +720,16 @@
             return (before or 1), 0
 
         if (
             self.previous_line
             and self.previous_line.is_class
             and current_line.is_triple_quoted_string
         ):
+            if Preview.no_blank_line_before_class_docstring in current_line.mode:
+                return 0, 1
             return before, 1
 
         if self.previous_line and self.previous_line.opens_block:
             return 0, 0
         return before, 0
 
     def _maybe_empty_lines_for_class_or_def(
@@ -824,18 +854,18 @@
 
     if mode.use_tabs:
         # Override previous calculation of `line_str`, because we need
         # to treat the width of '\t' as more than 1 character
         line_str = line.render_as_str_for_width_calculation().strip("\n")
 
     width = str_width if mode.preview else len
-    if mode.wrap_pragma_comments:  # Black's default
+    if mode.wrap_pragma_comments and mode.wrap_comments:  # Black's default
         effective_length = width(line_str)
     else:  # Cercis's default
-        effective_length = width(line_str) - line.trailing_pragma_comment_length()
+        effective_length = width(line_str) - line.calc_comment_length()
 
     if Preview.multiline_string_handling not in mode:
         return (
             effective_length <= mode.line_length
             and "\n" not in line_str  # multiline strings
             and not line.contains_standalone_comments()
         )
```

### Comparing `cercis-0.1.5/src/cercis/mode.py` & `cercis-0.1.6/src/cercis/mode.py`

 * *Files 3% similar despite different names*

```diff
@@ -18,19 +18,21 @@
     from typing import Final
 
 from cercis.const import (
     DEFAULT_BASE_INDENTATION_SPACES,
     DEFAULT_CLOSING_BRACKET_EXTRA_INDENT,
     DEFAULT_COLLAPSE_NESTED_BRACKETS,
     DEFAULT_FUNCTION_DEFINITION_EXTRA_INDENT,
+    DEFAULT_KEEP_BLANK_LINES_IN_BRACKETS,
     DEFAULT_LINE_LENGTH,
     DEFAULT_OTHER_LINE_CONTINUATION_EXTRA_INDENT,
     DEFAULT_SINGLE_QUOTE,
     DEFAULT_TAB_WIDTH,
     DEFAULT_USE_TABS,
+    DEFAULT_WRAP_COMMENTS,
     DEFAULT_WRAP_LINE_WITH_LONG_STRING,
     DEFAULT_WRAP_PRAGMA_COMMENTS,
 )
 
 
 class TargetVersion(Enum):
     PY33 = 3
@@ -166,14 +168,15 @@
     """Individual preview style features."""
 
     add_trailing_comma_consistently = auto()
     blank_line_after_nested_stub_class = auto()
     hex_codes_in_unicode_sequences = auto()
     improved_async_statements_handling = auto()
     multiline_string_handling = auto()
+    no_blank_line_before_class_docstring = auto()
     prefer_splitting_right_hand_side_of_assignments = auto()
     # NOTE: string_processing requires wrap_long_dict_values_in_parens
     # for https://github.com/psf/black/issues/3117 to be fixed.
     string_processing = auto()
     parenthesize_conditional_expressions = auto()
     skip_magic_trailing_comma_in_subscript = auto()
     wrap_long_dict_values_in_parens = auto()
@@ -198,14 +201,16 @@
     preview: bool = False
     function_definition_extra_indent: bool = DEFAULT_FUNCTION_DEFINITION_EXTRA_INDENT
     closing_bracket_extra_indent: bool = DEFAULT_CLOSING_BRACKET_EXTRA_INDENT
     single_quote: bool = DEFAULT_SINGLE_QUOTE
     wrap_line_with_long_string: bool = DEFAULT_WRAP_LINE_WITH_LONG_STRING
     collapse_nested_brackets: bool = DEFAULT_COLLAPSE_NESTED_BRACKETS
     wrap_pragma_comments: bool = DEFAULT_WRAP_PRAGMA_COMMENTS
+    wrap_comments: bool = DEFAULT_WRAP_COMMENTS
+    keep_blank_lines_in_brackets: bool = DEFAULT_KEEP_BLANK_LINES_IN_BRACKETS
     base_indentation_spaces: int = DEFAULT_BASE_INDENTATION_SPACES
     other_line_continuation_extra_indent: bool = (
         DEFAULT_OTHER_LINE_CONTINUATION_EXTRA_INDENT
     )
     use_tabs: bool = DEFAULT_USE_TABS
     tab_width: int = DEFAULT_TAB_WIDTH
```

### Comparing `cercis-0.1.5/src/cercis/nodes.py` & `cercis-0.1.6/src/cercis/nodes.py`

 * *Files identical despite different names*

### Comparing `cercis-0.1.5/src/cercis/numerics.py` & `cercis-0.1.6/src/cercis/numerics.py`

 * *Files identical despite different names*

### Comparing `cercis-0.1.5/src/cercis/output.py` & `cercis-0.1.6/src/cercis/output.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-"""Nice output for Black.
+"""Nice output for Cercis.
 
 The double calls are for patching purposes in tests.
 """
 
 import json
 import tempfile
 from typing import Any, Optional
```

### Comparing `cercis-0.1.5/src/cercis/parsing.py` & `cercis-0.1.6/src/cercis/parsing.py`

 * *Files identical despite different names*

### Comparing `cercis-0.1.5/src/cercis/report.py` & `cercis-0.1.6/src/cercis/report.py`

 * *Files 2% similar despite different names*

```diff
@@ -89,18 +89,18 @@
             reformatted = "reformatted"
             unchanged = "left unchanged"
             failed = "failed to reformat"
         report = []
         if self.change_count:
             s = "s" if self.change_count > 1 else ""
             report.append(
-                style(f"{self.change_count} file{s} ", bold=True, fg="blue")
+                style(f"{self.change_count} file{s} ", bold=True, fg="cyan")
                 + style(f"{reformatted}", bold=True)
             )
 
         if self.same_count:
             s = "s" if self.same_count > 1 else ""
-            report.append(style(f"{self.same_count} file{s} ", fg="blue") + unchanged)
+            report.append(style(f"{self.same_count} file{s} ", fg="cyan") + unchanged)
         if self.failure_count:
             s = "s" if self.failure_count > 1 else ""
             report.append(style(f"{self.failure_count} file{s} {failed}", fg="red"))
         return ", ".join(report) + "."
```

### Comparing `cercis-0.1.5/src/cercis/rusty.py` & `cercis-0.1.6/src/cercis/rusty.py`

 * *Files identical despite different names*

### Comparing `cercis-0.1.5/src/cercis/strings.py` & `cercis-0.1.6/src/cercis/strings.py`

 * *Files identical despite different names*

### Comparing `cercis-0.1.5/src/cercis/trans.py` & `cercis-0.1.6/src/cercis/trans.py`

 * *Files identical despite different names*

### Comparing `cercis-0.1.5/src/cercis/utils_line_wrapping.py` & `cercis-0.1.6/src/cercis/utils_line_wrapping.py`

 * *Files identical despite different names*

### Comparing `cercis-0.1.5/src/cercis/utils_linegen.py` & `cercis-0.1.6/src/cercis/utils_linegen.py`

 * *Files identical despite different names*

### Comparing `cercis-0.1.5/tests/optional.py` & `cercis-0.1.6/tests/optional.py`

 * *Files identical despite different names*

### Comparing `cercis-0.1.5/tests/test_black.py` & `cercis-0.1.6/tests/test_black.py`

 * *Files identical despite different names*

### Comparing `cercis-0.1.5/tests/test_blackd.py` & `cercis-0.1.6/tests/test_blackd.py`

 * *Files identical despite different names*

### Comparing `cercis-0.1.5/tests/test_format.py` & `cercis-0.1.6/tests/test_format.py`

 * *Files 7% similar despite different names*

```diff
@@ -45,26 +45,29 @@
     magic_trailing_comma = filename != "skip_magic_trailing_comma"
     single_quote = filename == "expression"
     mode = cercis.Mode(
         magic_trailing_comma=magic_trailing_comma,
         wrap_line_with_long_string=True,
         collapse_nested_brackets=False,
         single_quote=single_quote,
+        wrap_comments=True,
         wrap_pragma_comments=True,
+        keep_blank_lines_in_brackets=False,
         line_length=88,
     )
     check_file("simple_cases", filename, mode)
 
 
 @pytest.mark.parametrize("filename", all_data_cases("preview"))
 def test_preview_format(filename: str) -> None:
     mode = cercis.Mode(
         preview=True,
         wrap_line_with_long_string=True,
         collapse_nested_brackets=False,
+        wrap_comments=True,
         wrap_pragma_comments=True,
         line_length=88,
     )
     _override_single_quote_for_cleaner_future_rebase(mode)
     check_file("preview", filename, mode)
 
 
@@ -286,14 +289,15 @@
 )
 def test_single_quote(filename: str) -> None:
     mode = replace(
         DEFAULT_MODE,
         single_quote=True,
         wrap_line_with_long_string=True,
         collapse_nested_brackets=False,
+        wrap_comments=True,
         wrap_pragma_comments=True,
         line_length=88,
     )
     check_file("configurable_cases/single_quote", filename, mode)
 
 
 @pytest.mark.parametrize(
@@ -304,15 +308,19 @@
         ("long_strings_flag_disabled__Cercis_default.py", False),
         ("long_strings_flag_disabled__Black_default.py", True),
         ("edge_cases.py", False),
         ("edge_cases.py", True),
     ],
 )
 def test_opt_out_of_wrapping(filename: str, wrap_line: bool) -> None:
-    mode = replace(DEFAULT_MODE, wrap_line_with_long_string=wrap_line)
+    mode = replace(
+        DEFAULT_MODE,
+        wrap_line_with_long_string=wrap_line,
+        wrap_comments=True,
+    )
     _override_single_quote_for_cleaner_future_rebase(mode)
     _use_line_length_of_88_for_cleaner_future_rebase(mode)
     check_file("configurable_cases/line_with_long_string", filename, mode)
 
 
 @pytest.mark.parametrize(
     "filename, collapse_nested_brackets",
@@ -329,23 +337,53 @@
     check_file("configurable_cases/nested_brackets", filename, mode)
 
 
 @pytest.mark.parametrize(
     "filename, wrap",
     [
         ("Cercis_default.py", False),
+        ("Cercis_default_2.py", False),
         ("Black_default.py", True),
+        ("Black_default_2.py", True),
     ],
 )
 def test_wrap_pragma_comments(filename: str, wrap: bool) -> None:
-    mode = replace(DEFAULT_MODE, wrap_pragma_comments=wrap, line_length=80)
+    mode = replace(
+        DEFAULT_MODE,
+        wrap_comments=True,
+        wrap_pragma_comments=wrap,
+        line_length=80,
+    )
     check_file("configurable_cases/pragma_comments", filename, mode)
 
 
 @pytest.mark.parametrize(
+    "filename, wrap_comments, wrap_pragma_comments",
+    [
+        ("case_False_False.py", False, False),
+        ("case_True_False.py", True, False),
+        ("case_True_True.py", True, True),
+        ("case_False_True.py", False, True),
+    ],
+)
+def test_wrap_comments(
+        filename: str,
+        wrap_comments: bool,
+        wrap_pragma_comments: bool,
+) -> None:
+    mode = replace(
+        DEFAULT_MODE,
+        wrap_comments=wrap_comments,
+        wrap_pragma_comments=wrap_pragma_comments,
+        line_length=80,
+    )
+    check_file("configurable_cases/line_with_comments", filename, mode)
+
+
+@pytest.mark.parametrize(
     "closing_bracket_extra_indent, base_indent_spaces, fdei, olcei",
     list(
         itertools.product(  # each list here corresponds to 1 argument above
             [False, True],
             [1, 2, 3, 4, 8],
             [False, True],
             [False, True],
@@ -431,7 +469,23 @@
     )
     filename = f"tab_width_{tab_width}"
     check_file(
         "configurable_cases/indentation/use_tabs/line_length_calculation",
         filename,
         mode,
     )
+
+
+@pytest.mark.parametrize(
+    "filename, kblib",
+    [("true.py", True), ("false.py", False)],
+)
+def test_keep_blank_lines_in_brackets(filename: str, kblib: bool) -> None:
+    mode = replace(
+        DEFAULT_MODE,
+        keep_blank_lines_in_brackets=kblib,
+    )
+    check_file(
+        "configurable_cases/keep_blank_lines_in_brackets",
+        filename,
+        mode,
+    )
```

### Comparing `cercis-0.1.5/tests/test_ipynb.py` & `cercis-0.1.6/tests/test_ipynb.py`

 * *Files identical despite different names*

### Comparing `cercis-0.1.5/tests/test_no_ipynb.py` & `cercis-0.1.6/tests/test_no_ipynb.py`

 * *Files identical despite different names*

### Comparing `cercis-0.1.5/tests/test_trans.py` & `cercis-0.1.6/tests/test_trans.py`

 * *Files identical despite different names*

### Comparing `cercis-0.1.5/tests/test_utils_line_wrapping.py` & `cercis-0.1.6/tests/test_utils_line_wrapping.py`

 * *Files identical despite different names*

### Comparing `cercis-0.1.5/tests/util.py` & `cercis-0.1.6/tests/util.py`

 * *Files identical despite different names*

### Comparing `cercis-0.1.5/tests/data/conditional_expression.py` & `cercis-0.1.6/tests/data/conditional_expression.py`

 * *Files identical despite different names*

### Comparing `cercis-0.1.5/tests/data/configurable_cases/closing_bracket_indent/extra_indent.py` & `cercis-0.1.6/tests/data/configurable_cases/closing_bracket_indent/extra_indent.py`

 * *Files identical despite different names*

### Comparing `cercis-0.1.5/tests/data/configurable_cases/closing_bracket_indent/no_extra_indent.py` & `cercis-0.1.6/tests/data/configurable_cases/closing_bracket_indent/no_extra_indent.py`

 * *Files identical despite different names*

### Comparing `cercis-0.1.5/tests/data/configurable_cases/func_def_indent/func_def_extra_indent.py` & `cercis-0.1.6/tests/data/configurable_cases/func_def_indent/func_def_extra_indent.py`

 * *Files identical despite different names*

### Comparing `cercis-0.1.5/tests/data/configurable_cases/func_def_indent/func_def_no_extra_indent.py` & `cercis-0.1.6/tests/data/configurable_cases/func_def_indent/func_def_no_extra_indent.py`

 * *Files identical despite different names*

### Comparing `cercis-0.1.5/tests/data/configurable_cases/indentation/use_spaces/closing_bracket_extra_indent/base_indent_spaces=1/fdei=False_olcei=False.py` & `cercis-0.1.6/tests/data/configurable_cases/indentation/use_spaces/closing_bracket_extra_indent/base_indent_spaces=1/fdei=False_olcei=False.py`

 * *Files identical despite different names*

### Comparing `cercis-0.1.5/tests/data/configurable_cases/indentation/use_spaces/closing_bracket_extra_indent/base_indent_spaces=1/fdei=False_olcei=True.py` & `cercis-0.1.6/tests/data/configurable_cases/indentation/use_spaces/closing_bracket_extra_indent/base_indent_spaces=1/fdei=False_olcei=True.py`

 * *Files identical despite different names*

### Comparing `cercis-0.1.5/tests/data/configurable_cases/indentation/use_spaces/closing_bracket_extra_indent/base_indent_spaces=1/fdei=True_olcei=False.py` & `cercis-0.1.6/tests/data/configurable_cases/indentation/use_spaces/closing_bracket_extra_indent/base_indent_spaces=1/fdei=True_olcei=False.py`

 * *Files identical despite different names*

### Comparing `cercis-0.1.5/tests/data/configurable_cases/indentation/use_spaces/closing_bracket_extra_indent/base_indent_spaces=1/fdei=True_olcei=True.py` & `cercis-0.1.6/tests/data/configurable_cases/indentation/use_spaces/closing_bracket_extra_indent/base_indent_spaces=1/fdei=True_olcei=True.py`

 * *Files identical despite different names*

### Comparing `cercis-0.1.5/tests/data/configurable_cases/indentation/use_spaces/closing_bracket_extra_indent/base_indent_spaces=2/fdei=False_olcei=False.py` & `cercis-0.1.6/tests/data/configurable_cases/indentation/use_spaces/closing_bracket_extra_indent/base_indent_spaces=2/fdei=False_olcei=False.py`

 * *Files identical despite different names*

### Comparing `cercis-0.1.5/tests/data/configurable_cases/indentation/use_spaces/closing_bracket_extra_indent/base_indent_spaces=2/fdei=False_olcei=True.py` & `cercis-0.1.6/tests/data/configurable_cases/indentation/use_spaces/closing_bracket_extra_indent/base_indent_spaces=2/fdei=False_olcei=True.py`

 * *Files identical despite different names*

### Comparing `cercis-0.1.5/tests/data/configurable_cases/indentation/use_spaces/closing_bracket_extra_indent/base_indent_spaces=2/fdei=True_olcei=False.py` & `cercis-0.1.6/tests/data/configurable_cases/indentation/use_spaces/closing_bracket_extra_indent/base_indent_spaces=2/fdei=True_olcei=False.py`

 * *Files identical despite different names*

### Comparing `cercis-0.1.5/tests/data/configurable_cases/indentation/use_spaces/closing_bracket_extra_indent/base_indent_spaces=2/fdei=True_olcei=True.py` & `cercis-0.1.6/tests/data/configurable_cases/indentation/use_spaces/closing_bracket_extra_indent/base_indent_spaces=2/fdei=True_olcei=True.py`

 * *Files identical despite different names*

### Comparing `cercis-0.1.5/tests/data/configurable_cases/indentation/use_spaces/closing_bracket_extra_indent/base_indent_spaces=3/fdei=False_olcei=False.py` & `cercis-0.1.6/tests/data/configurable_cases/indentation/use_spaces/closing_bracket_extra_indent/base_indent_spaces=3/fdei=False_olcei=False.py`

 * *Files identical despite different names*

### Comparing `cercis-0.1.5/tests/data/configurable_cases/indentation/use_spaces/closing_bracket_extra_indent/base_indent_spaces=3/fdei=False_olcei=True.py` & `cercis-0.1.6/tests/data/configurable_cases/indentation/use_spaces/closing_bracket_extra_indent/base_indent_spaces=3/fdei=False_olcei=True.py`

 * *Files identical despite different names*

### Comparing `cercis-0.1.5/tests/data/configurable_cases/indentation/use_spaces/closing_bracket_extra_indent/base_indent_spaces=3/fdei=True_olcei=False.py` & `cercis-0.1.6/tests/data/configurable_cases/indentation/use_spaces/closing_bracket_extra_indent/base_indent_spaces=3/fdei=True_olcei=False.py`

 * *Files identical despite different names*

### Comparing `cercis-0.1.5/tests/data/configurable_cases/indentation/use_spaces/closing_bracket_extra_indent/base_indent_spaces=3/fdei=True_olcei=True.py` & `cercis-0.1.6/tests/data/configurable_cases/indentation/use_spaces/closing_bracket_extra_indent/base_indent_spaces=3/fdei=True_olcei=True.py`

 * *Files identical despite different names*

### Comparing `cercis-0.1.5/tests/data/configurable_cases/indentation/use_spaces/closing_bracket_extra_indent/base_indent_spaces=4/fdei=False_olcei=False.py` & `cercis-0.1.6/tests/data/configurable_cases/indentation/use_spaces/closing_bracket_extra_indent/base_indent_spaces=4/fdei=False_olcei=False.py`

 * *Files identical despite different names*

### Comparing `cercis-0.1.5/tests/data/configurable_cases/indentation/use_spaces/closing_bracket_extra_indent/base_indent_spaces=4/fdei=False_olcei=True.py` & `cercis-0.1.6/tests/data/configurable_cases/indentation/use_spaces/closing_bracket_extra_indent/base_indent_spaces=4/fdei=False_olcei=True.py`

 * *Files identical despite different names*

### Comparing `cercis-0.1.5/tests/data/configurable_cases/indentation/use_spaces/closing_bracket_extra_indent/base_indent_spaces=4/fdei=True_olcei=False.py` & `cercis-0.1.6/tests/data/configurable_cases/indentation/use_spaces/closing_bracket_extra_indent/base_indent_spaces=4/fdei=True_olcei=False.py`

 * *Files identical despite different names*

### Comparing `cercis-0.1.5/tests/data/configurable_cases/indentation/use_spaces/closing_bracket_extra_indent/base_indent_spaces=4/fdei=True_olcei=True.py` & `cercis-0.1.6/tests/data/configurable_cases/indentation/use_spaces/closing_bracket_extra_indent/base_indent_spaces=4/fdei=True_olcei=True.py`

 * *Files identical despite different names*

### Comparing `cercis-0.1.5/tests/data/configurable_cases/indentation/use_spaces/closing_bracket_extra_indent/base_indent_spaces=8/fdei=False_olcei=False.py` & `cercis-0.1.6/tests/data/configurable_cases/indentation/use_spaces/closing_bracket_extra_indent/base_indent_spaces=8/fdei=False_olcei=False.py`

 * *Files identical despite different names*

### Comparing `cercis-0.1.5/tests/data/configurable_cases/indentation/use_spaces/closing_bracket_extra_indent/base_indent_spaces=8/fdei=False_olcei=True.py` & `cercis-0.1.6/tests/data/configurable_cases/indentation/use_spaces/closing_bracket_extra_indent/base_indent_spaces=8/fdei=False_olcei=True.py`

 * *Files identical despite different names*

### Comparing `cercis-0.1.5/tests/data/configurable_cases/indentation/use_spaces/closing_bracket_extra_indent/base_indent_spaces=8/fdei=True_olcei=False.py` & `cercis-0.1.6/tests/data/configurable_cases/indentation/use_spaces/closing_bracket_extra_indent/base_indent_spaces=8/fdei=True_olcei=False.py`

 * *Files identical despite different names*

### Comparing `cercis-0.1.5/tests/data/configurable_cases/indentation/use_spaces/closing_bracket_extra_indent/base_indent_spaces=8/fdei=True_olcei=True.py` & `cercis-0.1.6/tests/data/configurable_cases/indentation/use_spaces/closing_bracket_extra_indent/base_indent_spaces=8/fdei=True_olcei=True.py`

 * *Files identical despite different names*

### Comparing `cercis-0.1.5/tests/data/configurable_cases/indentation/use_spaces/closing_bracket_no_extra_indent/base_indent_spaces=1/fdei=False_olcei=False.py` & `cercis-0.1.6/tests/data/configurable_cases/indentation/use_spaces/closing_bracket_no_extra_indent/base_indent_spaces=1/fdei=False_olcei=False.py`

 * *Files identical despite different names*

### Comparing `cercis-0.1.5/tests/data/configurable_cases/indentation/use_spaces/closing_bracket_no_extra_indent/base_indent_spaces=1/fdei=False_olcei=True.py` & `cercis-0.1.6/tests/data/configurable_cases/indentation/use_spaces/closing_bracket_no_extra_indent/base_indent_spaces=1/fdei=False_olcei=True.py`

 * *Files identical despite different names*

### Comparing `cercis-0.1.5/tests/data/configurable_cases/indentation/use_spaces/closing_bracket_no_extra_indent/base_indent_spaces=1/fdei=True_olcei=False.py` & `cercis-0.1.6/tests/data/configurable_cases/indentation/use_spaces/closing_bracket_no_extra_indent/base_indent_spaces=1/fdei=True_olcei=False.py`

 * *Files identical despite different names*

### Comparing `cercis-0.1.5/tests/data/configurable_cases/indentation/use_spaces/closing_bracket_no_extra_indent/base_indent_spaces=1/fdei=True_olcei=True.py` & `cercis-0.1.6/tests/data/configurable_cases/indentation/use_spaces/closing_bracket_no_extra_indent/base_indent_spaces=1/fdei=True_olcei=True.py`

 * *Files identical despite different names*

### Comparing `cercis-0.1.5/tests/data/configurable_cases/indentation/use_spaces/closing_bracket_no_extra_indent/base_indent_spaces=2/fdei=False_olcei=False.py` & `cercis-0.1.6/tests/data/configurable_cases/indentation/use_spaces/closing_bracket_no_extra_indent/base_indent_spaces=2/fdei=False_olcei=False.py`

 * *Files identical despite different names*

### Comparing `cercis-0.1.5/tests/data/configurable_cases/indentation/use_spaces/closing_bracket_no_extra_indent/base_indent_spaces=2/fdei=False_olcei=True.py` & `cercis-0.1.6/tests/data/configurable_cases/indentation/use_spaces/closing_bracket_no_extra_indent/base_indent_spaces=2/fdei=False_olcei=True.py`

 * *Files identical despite different names*

### Comparing `cercis-0.1.5/tests/data/configurable_cases/indentation/use_spaces/closing_bracket_no_extra_indent/base_indent_spaces=2/fdei=True_olcei=False.py` & `cercis-0.1.6/tests/data/configurable_cases/indentation/use_spaces/closing_bracket_no_extra_indent/base_indent_spaces=2/fdei=True_olcei=False.py`

 * *Files identical despite different names*

### Comparing `cercis-0.1.5/tests/data/configurable_cases/indentation/use_spaces/closing_bracket_no_extra_indent/base_indent_spaces=2/fdei=True_olcei=True.py` & `cercis-0.1.6/tests/data/configurable_cases/indentation/use_spaces/closing_bracket_no_extra_indent/base_indent_spaces=2/fdei=True_olcei=True.py`

 * *Files identical despite different names*

### Comparing `cercis-0.1.5/tests/data/configurable_cases/indentation/use_spaces/closing_bracket_no_extra_indent/base_indent_spaces=3/fdei=False_olcei=False.py` & `cercis-0.1.6/tests/data/configurable_cases/indentation/use_spaces/closing_bracket_no_extra_indent/base_indent_spaces=3/fdei=False_olcei=False.py`

 * *Files identical despite different names*

### Comparing `cercis-0.1.5/tests/data/configurable_cases/indentation/use_spaces/closing_bracket_no_extra_indent/base_indent_spaces=3/fdei=False_olcei=True.py` & `cercis-0.1.6/tests/data/configurable_cases/indentation/use_spaces/closing_bracket_no_extra_indent/base_indent_spaces=3/fdei=False_olcei=True.py`

 * *Files identical despite different names*

### Comparing `cercis-0.1.5/tests/data/configurable_cases/indentation/use_spaces/closing_bracket_no_extra_indent/base_indent_spaces=3/fdei=True_olcei=False.py` & `cercis-0.1.6/tests/data/configurable_cases/indentation/use_spaces/closing_bracket_no_extra_indent/base_indent_spaces=3/fdei=True_olcei=False.py`

 * *Files identical despite different names*

### Comparing `cercis-0.1.5/tests/data/configurable_cases/indentation/use_spaces/closing_bracket_no_extra_indent/base_indent_spaces=3/fdei=True_olcei=True.py` & `cercis-0.1.6/tests/data/configurable_cases/indentation/use_spaces/closing_bracket_no_extra_indent/base_indent_spaces=3/fdei=True_olcei=True.py`

 * *Files identical despite different names*

### Comparing `cercis-0.1.5/tests/data/configurable_cases/indentation/use_spaces/closing_bracket_no_extra_indent/base_indent_spaces=4/fdei=False_olcei=False.py` & `cercis-0.1.6/tests/data/configurable_cases/indentation/use_spaces/closing_bracket_no_extra_indent/base_indent_spaces=4/fdei=False_olcei=False.py`

 * *Files identical despite different names*

### Comparing `cercis-0.1.5/tests/data/configurable_cases/indentation/use_spaces/closing_bracket_no_extra_indent/base_indent_spaces=4/fdei=False_olcei=True.py` & `cercis-0.1.6/tests/data/configurable_cases/indentation/use_spaces/closing_bracket_no_extra_indent/base_indent_spaces=4/fdei=False_olcei=True.py`

 * *Files identical despite different names*

### Comparing `cercis-0.1.5/tests/data/configurable_cases/indentation/use_spaces/closing_bracket_no_extra_indent/base_indent_spaces=4/fdei=True_olcei=False.py` & `cercis-0.1.6/tests/data/configurable_cases/indentation/use_spaces/closing_bracket_no_extra_indent/base_indent_spaces=4/fdei=True_olcei=False.py`

 * *Files identical despite different names*

### Comparing `cercis-0.1.5/tests/data/configurable_cases/indentation/use_spaces/closing_bracket_no_extra_indent/base_indent_spaces=4/fdei=True_olcei=True.py` & `cercis-0.1.6/tests/data/configurable_cases/indentation/use_spaces/closing_bracket_no_extra_indent/base_indent_spaces=4/fdei=True_olcei=True.py`

 * *Files identical despite different names*

### Comparing `cercis-0.1.5/tests/data/configurable_cases/indentation/use_spaces/closing_bracket_no_extra_indent/base_indent_spaces=8/fdei=False_olcei=False.py` & `cercis-0.1.6/tests/data/configurable_cases/indentation/use_spaces/closing_bracket_no_extra_indent/base_indent_spaces=8/fdei=False_olcei=False.py`

 * *Files identical despite different names*

### Comparing `cercis-0.1.5/tests/data/configurable_cases/indentation/use_spaces/closing_bracket_no_extra_indent/base_indent_spaces=8/fdei=False_olcei=True.py` & `cercis-0.1.6/tests/data/configurable_cases/indentation/use_spaces/closing_bracket_no_extra_indent/base_indent_spaces=8/fdei=False_olcei=True.py`

 * *Files identical despite different names*

### Comparing `cercis-0.1.5/tests/data/configurable_cases/indentation/use_spaces/closing_bracket_no_extra_indent/base_indent_spaces=8/fdei=True_olcei=False.py` & `cercis-0.1.6/tests/data/configurable_cases/indentation/use_spaces/closing_bracket_no_extra_indent/base_indent_spaces=8/fdei=True_olcei=False.py`

 * *Files identical despite different names*

### Comparing `cercis-0.1.5/tests/data/configurable_cases/indentation/use_spaces/closing_bracket_no_extra_indent/base_indent_spaces=8/fdei=True_olcei=True.py` & `cercis-0.1.6/tests/data/configurable_cases/indentation/use_spaces/closing_bracket_no_extra_indent/base_indent_spaces=8/fdei=True_olcei=True.py`

 * *Files identical despite different names*

### Comparing `cercis-0.1.5/tests/data/configurable_cases/indentation/use_tabs/closing_bracket_extra_indent/fdei=False_olcei=False.py` & `cercis-0.1.6/tests/data/configurable_cases/indentation/use_tabs/closing_bracket_extra_indent/fdei=False_olcei=False.py`

 * *Files identical despite different names*

### Comparing `cercis-0.1.5/tests/data/configurable_cases/indentation/use_tabs/closing_bracket_extra_indent/fdei=False_olcei=True.py` & `cercis-0.1.6/tests/data/configurable_cases/indentation/use_tabs/closing_bracket_extra_indent/fdei=False_olcei=True.py`

 * *Files identical despite different names*

### Comparing `cercis-0.1.5/tests/data/configurable_cases/indentation/use_tabs/closing_bracket_extra_indent/fdei=True_olcei=False.py` & `cercis-0.1.6/tests/data/configurable_cases/indentation/use_tabs/closing_bracket_extra_indent/fdei=True_olcei=False.py`

 * *Files identical despite different names*

### Comparing `cercis-0.1.5/tests/data/configurable_cases/indentation/use_tabs/closing_bracket_extra_indent/fdei=True_olcei=True.py` & `cercis-0.1.6/tests/data/configurable_cases/indentation/use_tabs/closing_bracket_extra_indent/fdei=True_olcei=True.py`

 * *Files identical despite different names*

### Comparing `cercis-0.1.5/tests/data/configurable_cases/indentation/use_tabs/closing_bracket_no_extra_indent/fdei=False_olcei=False.py` & `cercis-0.1.6/tests/data/configurable_cases/indentation/use_tabs/closing_bracket_no_extra_indent/fdei=False_olcei=False.py`

 * *Files identical despite different names*

### Comparing `cercis-0.1.5/tests/data/configurable_cases/indentation/use_tabs/closing_bracket_no_extra_indent/fdei=False_olcei=True.py` & `cercis-0.1.6/tests/data/configurable_cases/indentation/use_tabs/closing_bracket_no_extra_indent/fdei=False_olcei=True.py`

 * *Files identical despite different names*

### Comparing `cercis-0.1.5/tests/data/configurable_cases/indentation/use_tabs/closing_bracket_no_extra_indent/fdei=True_olcei=False.py` & `cercis-0.1.6/tests/data/configurable_cases/indentation/use_tabs/closing_bracket_no_extra_indent/fdei=True_olcei=False.py`

 * *Files identical despite different names*

### Comparing `cercis-0.1.5/tests/data/configurable_cases/indentation/use_tabs/closing_bracket_no_extra_indent/fdei=True_olcei=True.py` & `cercis-0.1.6/tests/data/configurable_cases/indentation/use_tabs/closing_bracket_no_extra_indent/fdei=True_olcei=True.py`

 * *Files identical despite different names*

### Comparing `cercis-0.1.5/tests/data/configurable_cases/indentation/use_tabs/line_length_calculation/tab_width_1.py` & `cercis-0.1.6/tests/data/configurable_cases/indentation/use_tabs/line_length_calculation/tab_width_1.py`

 * *Files identical despite different names*

### Comparing `cercis-0.1.5/tests/data/configurable_cases/indentation/use_tabs/line_length_calculation/tab_width_2.py` & `cercis-0.1.6/tests/data/configurable_cases/indentation/use_tabs/line_length_calculation/tab_width_2.py`

 * *Files identical despite different names*

### Comparing `cercis-0.1.5/tests/data/configurable_cases/indentation/use_tabs/line_length_calculation/tab_width_3.py` & `cercis-0.1.6/tests/data/configurable_cases/indentation/use_tabs/line_length_calculation/tab_width_3.py`

 * *Files identical despite different names*

### Comparing `cercis-0.1.5/tests/data/configurable_cases/indentation/use_tabs/line_length_calculation/tab_width_4.py` & `cercis-0.1.6/tests/data/configurable_cases/indentation/use_tabs/line_length_calculation/tab_width_4.py`

 * *Files identical despite different names*

### Comparing `cercis-0.1.5/tests/data/configurable_cases/indentation/use_tabs/line_length_calculation/tab_width_5.py` & `cercis-0.1.6/tests/data/configurable_cases/indentation/use_tabs/line_length_calculation/tab_width_5.py`

 * *Files identical despite different names*

### Comparing `cercis-0.1.5/tests/data/configurable_cases/indentation/use_tabs/line_length_calculation/tab_width_8.py` & `cercis-0.1.6/tests/data/configurable_cases/indentation/use_tabs/line_length_calculation/tab_width_8.py`

 * *Files identical despite different names*

### Comparing `cercis-0.1.5/tests/data/configurable_cases/line_with_long_string/edge_cases.py` & `cercis-0.1.6/tests/data/configurable_cases/line_with_long_string/edge_cases.py`

 * *Files identical despite different names*

### Comparing `cercis-0.1.5/tests/data/configurable_cases/line_with_long_string/long_strings_flag_disabled__Black_default.py` & `cercis-0.1.6/tests/data/configurable_cases/line_with_long_string/long_strings_flag_disabled__Black_default.py`

 * *Files identical despite different names*

### Comparing `cercis-0.1.5/tests/data/configurable_cases/line_with_long_string/long_strings_flag_disabled__Cercis_default.py` & `cercis-0.1.6/tests/data/configurable_cases/line_with_long_string/long_strings_flag_disabled__Cercis_default.py`

 * *Files identical despite different names*

### Comparing `cercis-0.1.5/tests/data/configurable_cases/line_with_long_string/test_cases__Black_default.py` & `cercis-0.1.6/tests/data/configurable_cases/line_with_long_string/test_cases__Black_default.py`

 * *Files identical despite different names*

### Comparing `cercis-0.1.5/tests/data/configurable_cases/line_with_long_string/test_cases__Cercis_default.py` & `cercis-0.1.6/tests/data/configurable_cases/line_with_long_string/test_cases__Cercis_default.py`

 * *Files identical despite different names*

### Comparing `cercis-0.1.5/tests/data/configurable_cases/nested_brackets/nested_brackets__Black_default.py` & `cercis-0.1.6/tests/data/configurable_cases/nested_brackets/nested_brackets__Black_default.py`

 * *Files identical despite different names*

### Comparing `cercis-0.1.5/tests/data/configurable_cases/nested_brackets/nested_brackets__Cercis_default.py` & `cercis-0.1.6/tests/data/configurable_cases/nested_brackets/nested_brackets__Cercis_default.py`

 * *Files identical despite different names*

### Comparing `cercis-0.1.5/tests/data/configurable_cases/nested_brackets/nested_brackets_explodes__Black_default.py` & `cercis-0.1.6/tests/data/configurable_cases/nested_brackets/nested_brackets_explodes__Black_default.py`

 * *Files identical despite different names*

### Comparing `cercis-0.1.5/tests/data/configurable_cases/nested_brackets/nested_brackets_explodes__Cercis_default.py` & `cercis-0.1.6/tests/data/configurable_cases/nested_brackets/nested_brackets_explodes__Cercis_default.py`

 * *Files identical despite different names*

### Comparing `cercis-0.1.5/tests/data/configurable_cases/pragma_comments/Black_default.py` & `cercis-0.1.6/tests/data/configurable_cases/pragma_comments/Black_default.py`

 * *Files identical despite different names*

### Comparing `cercis-0.1.5/tests/data/configurable_cases/pragma_comments/Cercis_default.py` & `cercis-0.1.6/tests/data/configurable_cases/pragma_comments/Cercis_default.py`

 * *Files identical despite different names*

### Comparing `cercis-0.1.5/tests/data/configurable_cases/single_quote/docstring.py` & `cercis-0.1.6/tests/data/configurable_cases/single_quote/docstring.py`

 * *Files identical despite different names*

### Comparing `cercis-0.1.5/tests/data/configurable_cases/single_quote/docstring_preview.py` & `cercis-0.1.6/tests/data/configurable_cases/single_quote/docstring_preview.py`

 * *Files identical despite different names*

### Comparing `cercis-0.1.5/tests/data/configurable_cases/single_quote/more_quotes.py` & `cercis-0.1.6/tests/data/configurable_cases/single_quote/more_quotes.py`

 * *Files identical despite different names*

### Comparing `cercis-0.1.5/tests/data/configurable_cases/single_quote/string_prefixes.py` & `cercis-0.1.6/tests/data/configurable_cases/single_quote/string_prefixes.py`

 * *Files identical despite different names*

### Comparing `cercis-0.1.5/tests/data/configurable_cases/single_quote/torture.py` & `cercis-0.1.6/tests/data/configurable_cases/single_quote/torture.py`

 * *Files identical despite different names*

### Comparing `cercis-0.1.5/tests/data/jupyter/notebook_no_trailing_newline.ipynb` & `cercis-0.1.6/tests/data/jupyter/notebook_no_trailing_newline.ipynb`

 * *Files identical despite different names*

### Comparing `cercis-0.1.5/tests/data/jupyter/notebook_trailing_newline.ipynb` & `cercis-0.1.6/tests/data/jupyter/notebook_trailing_newline.ipynb`

 * *Files identical despite different names*

### Comparing `cercis-0.1.5/tests/data/jupyter/notebook_without_changes.ipynb` & `cercis-0.1.6/tests/data/jupyter/notebook_without_changes.ipynb`

 * *Files identical despite different names*

### Comparing `cercis-0.1.5/tests/data/miscellaneous/debug_visitor.out` & `cercis-0.1.6/tests/data/miscellaneous/debug_visitor.out`

 * *Files identical despite different names*

### Comparing `cercis-0.1.5/tests/data/miscellaneous/debug_visitor.py` & `cercis-0.1.6/tests/data/miscellaneous/debug_visitor.py`

 * *Files identical despite different names*

### Comparing `cercis-0.1.5/tests/data/miscellaneous/decorators.py` & `cercis-0.1.6/tests/data/miscellaneous/decorators.py`

 * *Files identical despite different names*

### Comparing `cercis-0.1.5/tests/data/miscellaneous/docstring_no_string_normalization.py` & `cercis-0.1.6/tests/data/miscellaneous/docstring_no_string_normalization.py`

 * *Files identical despite different names*

### Comparing `cercis-0.1.5/tests/data/miscellaneous/expression_skip_magic_trailing_comma.diff` & `cercis-0.1.6/tests/data/miscellaneous/expression_skip_magic_trailing_comma.diff`

 * *Files identical despite different names*

### Comparing `cercis-0.1.5/tests/data/miscellaneous/force_py36.py` & `cercis-0.1.6/tests/data/miscellaneous/force_py36.py`

 * *Files identical despite different names*

### Comparing `cercis-0.1.5/tests/data/miscellaneous/force_pyi.py` & `cercis-0.1.6/tests/data/miscellaneous/force_pyi.py`

 * *Files identical despite different names*

### Comparing `cercis-0.1.5/tests/data/miscellaneous/long_strings_flag_disabled.py` & `cercis-0.1.6/tests/data/miscellaneous/long_strings_flag_disabled.py`

 * *Files identical despite different names*

### Comparing `cercis-0.1.5/tests/data/miscellaneous/python2_detection.py` & `cercis-0.1.6/tests/data/miscellaneous/python2_detection.py`

 * *Files identical despite different names*

### Comparing `cercis-0.1.5/tests/data/miscellaneous/string_quotes.py` & `cercis-0.1.6/tests/data/miscellaneous/string_quotes.py`

 * *Files identical despite different names*

### Comparing `cercis-0.1.5/tests/data/miscellaneous/stub.pyi` & `cercis-0.1.6/tests/data/miscellaneous/stub.pyi`

 * *Files identical despite different names*

### Comparing `cercis-0.1.5/tests/data/preview/cantfit.py` & `cercis-0.1.6/tests/data/preview/cantfit.py`

 * *Files identical despite different names*

### Comparing `cercis-0.1.5/tests/data/preview/comments7.py` & `cercis-0.1.6/tests/data/preview/comments7.py`

 * *Files identical despite different names*

### Comparing `cercis-0.1.5/tests/data/preview/format_unicode_escape_seq.py` & `cercis-0.1.6/tests/data/preview/format_unicode_escape_seq.py`

 * *Files identical despite different names*

### Comparing `cercis-0.1.5/tests/data/preview/long_dict_values.py` & `cercis-0.1.6/tests/data/preview/long_dict_values.py`

 * *Files identical despite different names*

### Comparing `cercis-0.1.5/tests/data/preview/long_strings.py` & `cercis-0.1.6/tests/data/preview/long_strings.py`

 * *Files identical despite different names*

### Comparing `cercis-0.1.5/tests/data/preview/long_strings__east_asian_width.py` & `cercis-0.1.6/tests/data/preview/long_strings__east_asian_width.py`

 * *Files identical despite different names*

### Comparing `cercis-0.1.5/tests/data/preview/long_strings__edge_case.py` & `cercis-0.1.6/tests/data/preview/long_strings__edge_case.py`

 * *Files identical despite different names*

### Comparing `cercis-0.1.5/tests/data/preview/long_strings__regression.py` & `cercis-0.1.6/tests/data/preview/long_strings__regression.py`

 * *Files identical despite different names*

### Comparing `cercis-0.1.5/tests/data/preview/long_strings__type_annotations.py` & `cercis-0.1.6/tests/data/preview/long_strings__type_annotations.py`

 * *Files identical despite different names*

### Comparing `cercis-0.1.5/tests/data/preview/multiline_strings.py` & `cercis-0.1.6/tests/data/preview/multiline_strings.py`

 * *Files identical despite different names*

### Comparing `cercis-0.1.5/tests/data/preview/prefer_rhs_split.py` & `cercis-0.1.6/tests/data/preview/prefer_rhs_split.py`

 * *Files identical despite different names*

### Comparing `cercis-0.1.5/tests/data/preview/trailing_comma.py` & `cercis-0.1.6/tests/data/preview/trailing_comma.py`

 * *Files identical despite different names*

### Comparing `cercis-0.1.5/tests/data/preview_context_managers/targeting_py38.py` & `cercis-0.1.6/tests/data/preview_context_managers/targeting_py38.py`

 * *Files identical despite different names*

### Comparing `cercis-0.1.5/tests/data/preview_context_managers/targeting_py39.py` & `cercis-0.1.6/tests/data/preview_context_managers/targeting_py39.py`

 * *Files identical despite different names*

### Comparing `cercis-0.1.5/tests/data/preview_context_managers/auto_detect/features_3_10.py` & `cercis-0.1.6/tests/data/preview_context_managers/auto_detect/features_3_10.py`

 * *Files identical despite different names*

### Comparing `cercis-0.1.5/tests/data/preview_context_managers/auto_detect/features_3_11.py` & `cercis-0.1.6/tests/data/preview_context_managers/auto_detect/features_3_11.py`

 * *Files identical despite different names*

### Comparing `cercis-0.1.5/tests/data/preview_context_managers/auto_detect/features_3_8.py` & `cercis-0.1.6/tests/data/preview_context_managers/auto_detect/features_3_8.py`

 * *Files identical despite different names*

### Comparing `cercis-0.1.5/tests/data/preview_context_managers/auto_detect/features_3_9.py` & `cercis-0.1.6/tests/data/preview_context_managers/auto_detect/features_3_9.py`

 * *Files identical despite different names*

### Comparing `cercis-0.1.5/tests/data/py_310/parenthesized_context_managers.py` & `cercis-0.1.6/tests/data/py_310/parenthesized_context_managers.py`

 * *Files identical despite different names*

### Comparing `cercis-0.1.5/tests/data/py_310/pattern_matching_complex.py` & `cercis-0.1.6/tests/data/py_310/pattern_matching_complex.py`

 * *Files identical despite different names*

### Comparing `cercis-0.1.5/tests/data/py_310/pattern_matching_extras.py` & `cercis-0.1.6/tests/data/py_310/pattern_matching_extras.py`

 * *Files identical despite different names*

### Comparing `cercis-0.1.5/tests/data/py_310/pattern_matching_generic.py` & `cercis-0.1.6/tests/data/py_310/pattern_matching_generic.py`

 * *Files identical despite different names*

### Comparing `cercis-0.1.5/tests/data/py_310/pattern_matching_simple.py` & `cercis-0.1.6/tests/data/py_310/pattern_matching_simple.py`

 * *Files identical despite different names*

### Comparing `cercis-0.1.5/tests/data/py_310/pattern_matching_style.py` & `cercis-0.1.6/tests/data/py_310/pattern_matching_style.py`

 * *Files identical despite different names*

### Comparing `cercis-0.1.5/tests/data/py_311/pep_646.py` & `cercis-0.1.6/tests/data/py_311/pep_646.py`

 * *Files identical despite different names*

### Comparing `cercis-0.1.5/tests/data/py_311/pep_654.py` & `cercis-0.1.6/tests/data/py_311/pep_654.py`

 * *Files identical despite different names*

### Comparing `cercis-0.1.5/tests/data/py_311/pep_654_style.py` & `cercis-0.1.6/tests/data/py_311/pep_654_style.py`

 * *Files identical despite different names*

### Comparing `cercis-0.1.5/tests/data/py_36/numeric_literals.py` & `cercis-0.1.6/tests/data/py_36/numeric_literals.py`

 * *Files identical despite different names*

### Comparing `cercis-0.1.5/tests/data/py_37/python37.py` & `cercis-0.1.6/tests/data/py_37/python37.py`

 * *Files identical despite different names*

### Comparing `cercis-0.1.5/tests/data/py_38/pep_570.py` & `cercis-0.1.6/tests/data/py_38/pep_570.py`

 * *Files identical despite different names*

### Comparing `cercis-0.1.5/tests/data/py_38/pep_572.py` & `cercis-0.1.6/tests/data/py_38/pep_572.py`

 * *Files identical despite different names*

### Comparing `cercis-0.1.5/tests/data/py_38/pep_572_remove_parens.py` & `cercis-0.1.6/tests/data/py_38/pep_572_remove_parens.py`

 * *Files identical despite different names*

### Comparing `cercis-0.1.5/tests/data/py_38/python38.py` & `cercis-0.1.6/tests/data/py_38/python38.py`

 * *Files identical despite different names*

### Comparing `cercis-0.1.5/tests/data/py_39/python39.py` & `cercis-0.1.6/tests/data/py_39/python39.py`

 * *Files identical despite different names*

### Comparing `cercis-0.1.5/tests/data/py_39/remove_with_brackets.py` & `cercis-0.1.6/tests/data/py_39/remove_with_brackets.py`

 * *Files identical despite different names*

### Comparing `cercis-0.1.5/tests/data/simple_cases/attribute_access_on_number_literals.py` & `cercis-0.1.6/tests/data/simple_cases/attribute_access_on_number_literals.py`

 * *Files identical despite different names*

### Comparing `cercis-0.1.5/tests/data/simple_cases/class_blank_parentheses.py` & `cercis-0.1.6/tests/data/simple_cases/class_blank_parentheses.py`

 * *Files identical despite different names*

### Comparing `cercis-0.1.5/tests/data/simple_cases/class_methods_new_line.py` & `cercis-0.1.6/tests/data/simple_cases/class_methods_new_line.py`

 * *Files identical despite different names*

### Comparing `cercis-0.1.5/tests/data/simple_cases/collections.py` & `cercis-0.1.6/tests/data/simple_cases/collections.py`

 * *Files identical despite different names*

### Comparing `cercis-0.1.5/tests/data/simple_cases/comments.py` & `cercis-0.1.6/tests/data/simple_cases/comments.py`

 * *Files identical despite different names*

### Comparing `cercis-0.1.5/tests/data/simple_cases/comments2.py` & `cercis-0.1.6/tests/data/simple_cases/comments2.py`

 * *Files identical despite different names*

### Comparing `cercis-0.1.5/tests/data/simple_cases/comments3.py` & `cercis-0.1.6/tests/data/simple_cases/comments3.py`

 * *Files identical despite different names*

### Comparing `cercis-0.1.5/tests/data/simple_cases/comments4.py` & `cercis-0.1.6/tests/data/simple_cases/comments4.py`

 * *Files identical despite different names*

### Comparing `cercis-0.1.5/tests/data/simple_cases/comments5.py` & `cercis-0.1.6/tests/data/simple_cases/comments5.py`

 * *Files identical despite different names*

### Comparing `cercis-0.1.5/tests/data/simple_cases/comments6.py` & `cercis-0.1.6/tests/data/simple_cases/comments6.py`

 * *Files identical despite different names*

### Comparing `cercis-0.1.5/tests/data/simple_cases/comments9.py` & `cercis-0.1.6/tests/data/simple_cases/comments9.py`

 * *Files identical despite different names*

### Comparing `cercis-0.1.5/tests/data/simple_cases/comments_non_breaking_space.py` & `cercis-0.1.6/tests/data/simple_cases/comments_non_breaking_space.py`

 * *Files identical despite different names*

### Comparing `cercis-0.1.5/tests/data/simple_cases/composition.py` & `cercis-0.1.6/tests/data/simple_cases/composition.py`

 * *Files identical despite different names*

### Comparing `cercis-0.1.5/tests/data/simple_cases/composition_no_trailing_comma.py` & `cercis-0.1.6/tests/data/simple_cases/composition_no_trailing_comma.py`

 * *Files identical despite different names*

### Comparing `cercis-0.1.5/tests/data/simple_cases/docstring.py` & `cercis-0.1.6/tests/data/simple_cases/docstring.py`

 * *Files identical despite different names*

### Comparing `cercis-0.1.5/tests/data/simple_cases/docstring_preview.py` & `cercis-0.1.6/tests/data/simple_cases/docstring_preview.py`

 * *Files identical despite different names*

### Comparing `cercis-0.1.5/tests/data/simple_cases/empty_lines.py` & `cercis-0.1.6/tests/data/simple_cases/empty_lines.py`

 * *Files identical despite different names*

### Comparing `cercis-0.1.5/tests/data/simple_cases/expression.diff` & `cercis-0.1.6/tests/data/simple_cases/expression.diff`

 * *Files identical despite different names*

### Comparing `cercis-0.1.5/tests/data/simple_cases/expression.py` & `cercis-0.1.6/tests/data/simple_cases/expression.py`

 * *Files identical despite different names*

### Comparing `cercis-0.1.5/tests/data/simple_cases/fmtonoff.py` & `cercis-0.1.6/tests/data/simple_cases/fmtonoff.py`

 * *Files identical despite different names*

### Comparing `cercis-0.1.5/tests/data/simple_cases/fmtonoff2.py` & `cercis-0.1.6/tests/data/simple_cases/fmtonoff2.py`

 * *Files identical despite different names*

### Comparing `cercis-0.1.5/tests/data/simple_cases/fmtonoff5.py` & `cercis-0.1.6/tests/data/simple_cases/fmtonoff5.py`

 * *Files identical despite different names*

### Comparing `cercis-0.1.5/tests/data/simple_cases/fmtskip2.py` & `cercis-0.1.6/tests/data/simple_cases/fmtskip2.py`

 * *Files identical despite different names*

### Comparing `cercis-0.1.5/tests/data/simple_cases/fmtskip8.py` & `cercis-0.1.6/tests/data/simple_cases/fmtskip8.py`

 * *Files identical despite different names*

### Comparing `cercis-0.1.5/tests/data/simple_cases/fstring.py` & `cercis-0.1.6/tests/data/simple_cases/fstring.py`

 * *Files identical despite different names*

### Comparing `cercis-0.1.5/tests/data/simple_cases/function.py` & `cercis-0.1.6/tests/data/simple_cases/function.py`

 * *Files identical despite different names*

### Comparing `cercis-0.1.5/tests/data/simple_cases/function2.py` & `cercis-0.1.6/tests/data/simple_cases/function2.py`

 * *Files identical despite different names*

### Comparing `cercis-0.1.5/tests/data/simple_cases/function_trailing_comma.py` & `cercis-0.1.6/tests/data/simple_cases/function_trailing_comma.py`

 * *Files identical despite different names*

### Comparing `cercis-0.1.5/tests/data/simple_cases/import_spacing.py` & `cercis-0.1.6/tests/data/simple_cases/import_spacing.py`

 * *Files identical despite different names*

### Comparing `cercis-0.1.5/tests/data/simple_cases/one_element_subscript.py` & `cercis-0.1.6/tests/data/simple_cases/one_element_subscript.py`

 * *Files identical despite different names*

### Comparing `cercis-0.1.5/tests/data/simple_cases/power_op_spacing.py` & `cercis-0.1.6/tests/data/simple_cases/power_op_spacing.py`

 * *Files identical despite different names*

### Comparing `cercis-0.1.5/tests/data/simple_cases/prefer_rhs_split_reformatted.py` & `cercis-0.1.6/tests/data/simple_cases/prefer_rhs_split_reformatted.py`

 * *Files identical despite different names*

### Comparing `cercis-0.1.5/tests/data/simple_cases/remove_await_parens.py` & `cercis-0.1.6/tests/data/simple_cases/remove_await_parens.py`

 * *Files identical despite different names*

### Comparing `cercis-0.1.5/tests/data/simple_cases/remove_except_parens.py` & `cercis-0.1.6/tests/data/simple_cases/remove_except_parens.py`

 * *Files identical despite different names*

### Comparing `cercis-0.1.5/tests/data/simple_cases/remove_for_brackets.py` & `cercis-0.1.6/tests/data/simple_cases/remove_for_brackets.py`

 * *Files identical despite different names*

### Comparing `cercis-0.1.5/tests/data/simple_cases/remove_newline_after_code_block_open.py` & `cercis-0.1.6/tests/data/simple_cases/remove_newline_after_code_block_open.py`

 * *Files identical despite different names*

### Comparing `cercis-0.1.5/tests/data/simple_cases/remove_parens.py` & `cercis-0.1.6/tests/data/simple_cases/remove_parens.py`

 * *Files identical despite different names*

### Comparing `cercis-0.1.5/tests/data/simple_cases/return_annotation_brackets.py` & `cercis-0.1.6/tests/data/simple_cases/return_annotation_brackets.py`

 * *Files identical despite different names*

### Comparing `cercis-0.1.5/tests/data/simple_cases/skip_magic_trailing_comma.py` & `cercis-0.1.6/tests/data/simple_cases/skip_magic_trailing_comma.py`

 * *Files identical despite different names*

### Comparing `cercis-0.1.5/tests/data/simple_cases/slices.py` & `cercis-0.1.6/tests/data/simple_cases/slices.py`

 * *Files identical despite different names*

### Comparing `cercis-0.1.5/tests/data/simple_cases/string_prefixes.py` & `cercis-0.1.6/tests/data/simple_cases/string_prefixes.py`

 * *Files identical despite different names*

### Comparing `cercis-0.1.5/tests/data/simple_cases/torture.py` & `cercis-0.1.6/tests/data/simple_cases/torture.py`

 * *Files identical despite different names*

### Comparing `cercis-0.1.5/tests/data/simple_cases/trailing_comma_optional_parens1.py` & `cercis-0.1.6/tests/data/simple_cases/trailing_comma_optional_parens1.py`

 * *Files identical despite different names*

### Comparing `cercis-0.1.5/tests/data/simple_cases/trailing_comma_optional_parens3.py` & `cercis-0.1.6/tests/data/simple_cases/trailing_comma_optional_parens3.py`

 * *Files identical despite different names*

### Comparing `cercis-0.1.5/tests/data/simple_cases/trailing_commas_in_leading_parts.py` & `cercis-0.1.6/tests/data/simple_cases/trailing_commas_in_leading_parts.py`

 * *Files identical despite different names*

### Comparing `cercis-0.1.5/LICENSE` & `cercis-0.1.6/LICENSE`

 * *Files identical despite different names*

### Comparing `cercis-0.1.5/LICENSE_ORIGINAL` & `cercis-0.1.6/LICENSE_ORIGINAL`

 * *Files identical despite different names*

### Comparing `cercis-0.1.5/pyproject.toml` & `cercis-0.1.6/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -31,15 +31,15 @@
 
 [build-system]
 requires = ["hatchling>=1.8.0", "hatch-vcs", "hatch-fancy-pypi-readme"]
 build-backend = "hatchling.build"
 
 [project]
 name = "cercis"
-version = "0.1.5"
+version = "0.1.6"
 description = "A more configurable Python code formatter"
 license = { text = "MIT" }
 requires-python = ">=3.7"
 authors = [
   { name = "Łukasz Langa", email = "lukasz@langa.pl" },
   { name = "jsh9", email = "" },
 ]
```

### Comparing `cercis-0.1.5/PKG-INFO` & `cercis-0.1.6/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cercis
-Version: 0.1.5
+Version: 0.1.6
 Summary: A more configurable Python code formatter
 Project-URL: Changelog, https://github.com/jsh9/cercis/blob/main/CHANGES.md
 Project-URL: Homepage, https://github.com/jsh9/cercis
 Author: jsh9
 Author-email: Łukasz Langa <lukasz@langa.pl>
 License: MIT
 License-File: LICENSE
@@ -44,47 +44,43 @@
 Requires-Dist: uvloop>=0.15.2; extra == 'uvloop'
 Description-Content-Type: text/markdown
 
 # _Cercis_
 
 [![](https://upload.wikimedia.org/wikipedia/commons/thumb/4/4c/Red_bud_2009.jpg/320px-Red_bud_2009.jpg)](https://en.wikipedia.org/wiki/Cercis)
 
-_**Cercis**_ /ˈsɜːrsɪs/ is a Python code formatter that is more configurable
-than [Black](https://github.com/psf/black) (a popular Python code formatter).
+_**Cercis**_ /ˈsɜːrsɪs/ is a Python code formatter that is more configurable than
+[Black](https://github.com/psf/black) (a popular Python code formatter).
 
-[_Cercis_](https://en.wikipedia.org/wiki/Cercis) is also the name of a
-deciduous tree that boasts vibrant pink to purple-hued flowers, which bloom in
-early spring.
+[_Cercis_](https://en.wikipedia.org/wiki/Cercis) is also the name of a deciduous tree
+that boasts vibrant pink to purple-hued flowers, which bloom in early spring.
 
 This code repository is forked from and directly inspired by
-[Black](https://github.com/psf/black). The original license of Black is
-included in this repository (see [LICENSE_ORIGINAL](./LICENSE_ORIGINAL)).
+[Black](https://github.com/psf/black). The original license of Black is included in this
+repository (see [LICENSE_ORIGINAL](./LICENSE_ORIGINAL)).
 
-_Cercis_ inherited Black's very comprehensive test cases, which means we are
-confident that our configurability addition does not introduce any undesirable
-side effects. We also thoroughly tested every configurable options that we
-added.
-
-In particular, via its configurable options, _Cercis_ can completely fall back
-to Black. See [Section 4.5](#45-how-to-fall-back-to-blacks-behavior) below for
-more details.
+_Cercis_ inherited Black's very comprehensive test cases, which means we are confident
+that our configurability addition does not introduce any undesirable side effects. We
+also thoroughly tested every configurable options that we added.
+
+In particular, via its configurable options, _Cercis_ can completely fall back to Black.
+See [Section 4.5](#45-how-to-fall-back-to-blacks-behavior) below for more details.
 
 ## 1. Motivations
 
-While we like the idea of auto-formatting and code readability, we take issue
-with some style choices and the lack of configurability of the Black formatter.
-Therefore, _Cercis_ aims at providing some configurability beyond Black's
-limited offering.
+While we like the idea of auto-formatting and code readability, we take issue with some
+style choices and the lack of configurability of the Black formatter. Therefore,
+_Cercis_ aims at providing some configurability beyond Black's limited offering.
 
 ## 2. Installation and usage
 
 ### 2.1. Installation
 
-_Cercis_ can be installed by running `pip install cercis`. It requires Python
-3.7+ to run. If you want to format Jupyter Notebooks, install with
+_Cercis_ can be installed by running `pip install cercis`. It requires Python 3.7+ to
+run. If you want to format Jupyter Notebooks, install with
 `pip install "cercis[jupyter]"`.
 
 ### 2.2. Usage
 
 #### 2.2.1. Command line usage
 
 To get started right away with sensible defaults:
@@ -99,17 +95,16 @@
 python -m cercis {source_file_or_directory}
 ```
 
 The commands above reformat entire file(s) in place.
 
 #### 2.2.2. As pre-commit hook
 
-To format Python files (.py), put the following into your
-`.pre-commit-config.yaml` file. Remember to replace `<VERSION>` with your
-version of this tool (such as `v0.1.0`):
+To format Python files (.py), put the following into your `.pre-commit-config.yaml`
+file. Remember to replace `<VERSION>` with your version of this tool (such as `v0.1.0`):
 
 ```yaml
 - repo: https://github.com/jsh9/cercis
   rev: <VERSION>
   hooks:
     - id: cercis
       args: [--line-length=88]
@@ -122,48 +117,47 @@
 - repo: https://github.com/jsh9/cercis
   rev: <VERSION>
   hooks:
     - id: cercis-jupyter
       args: [--line-length=88]
 ```
 
-See [pre-commit](https://github.com/pre-commit/pre-commit) for more
-instructions. In particular,
-[here](https://pre-commit.com/#passing-arguments-to-hooks) is how to specify
+See [pre-commit](https://github.com/pre-commit/pre-commit) for more instructions. In
+particular, [here](https://pre-commit.com/#passing-arguments-to-hooks) is how to specify
 arguments in pre-commit config.
 
 ## 3. _Cercis_'s code style
 
 _Cercis_'s code style is largely consistent with the
 [style of of Black](https://black.readthedocs.io/en/stable/the_black_code_style/current_style.html).
 
-The main difference is that _Cercis_ provides several configurable options that
-Black doesn't. Configurability is our main motivation behind creating _Cercis_.
+The main difference is that _Cercis_ provides several configurable options that Black
+doesn't. Configurability is our main motivation behind creating _Cercis_.
 
 _Cercis_ offers the following configurable options:
 
 1. [Line length](#31-line-length)
 2. [Single quote vs double quote](#32-single-quote-vs-double-quote)
 3. [Tabs vs spaces](#33-tabs-vs-spaces)
 4. [Base indentation spaces](#34-base-indentation-spaces)
 5. [Extra indentation at line continuation](#35-extra-indentation-at-line-continuation)
    1. [At function definition](#351-at-function-definition---function-definition-extra-indent)
    2. [In other line continuations](#352-in-other-line-continuations---other-line-continuation-extra-indent)
    3. [At closing brackets](#353-at-closing-brackets---closing-bracket-extra-indent)
 6. ["Simple" lines with long strings](#36-simple-lines-with-long-strings)
 7. [Collapse nested brackets](#37-collapse-nested-brackets)
-8. [Wrap pragma comments](#38-wrapping-long-lines-ending-with-pragma-comments)
+8. [Wrap lines ending with comments](#38-wrapping-long-lines-ending-with-comments)
+9. [Keep blank lines in brackets](#39-keep-blank-lines-in-brackets)
 
-The next section ([How to configure _Cercis_](#4-how-to-configure-cercis))
-contains detailed instructions of how to configure these options.
+The next section ([How to configure _Cercis_](#4-how-to-configure-cercis)) contains
+detailed instructions of how to configure these options.
 
 ### 3.1. Line length
 
-_Cercis_ uses 79 characters as the line length limit, instead of 88 (Black's
-default).
+_Cercis_ uses 79 characters as the line length limit, instead of 88 (Black's default).
 
 You can override this default if necessary.
 
 | Option                 |                                           |
 | ---------------------- | ----------------------------------------- |
 | Name                   | `--line-length`                           |
 | Abbreviation           | `-l`                                      |
@@ -171,16 +165,16 @@
 | Black's default        | 88                                        |
 | Command line usage     | `cercis -l=120 myScript.py`               |
 | `pyproject.toml` usage | `line-length = 120` under `[tool.cercis]` |
 | `pre-commit` usage     | `args: [--line-length=120]`               |
 
 ### 3.2. Single quote vs double quote
 
-_Cercis_ uses single quotes (`'`) as the default for strings, instead of double
-quotes (`"`) which is Black's default.
+_Cercis_ uses single quotes (`'`) as the default for strings, instead of double quotes
+(`"`) which is Black's default.
 
 You can override this default if necessary.
 
 | Option                 |                                              |
 | ---------------------- | -------------------------------------------- |
 | Name                   | `--single-quote`                             |
 | Abbreviation           | `-sq`                                        |
@@ -204,35 +198,34 @@
 | Abbreviation           | `-tab`                                   |
 | Default                | `False`                                  |
 | Black's default        | `False`                                  |
 | Command line usage     | `cercis -tab=True myScript.py`           |
 | `pyproject.toml` usage | `use-tabs = false` under `[tool.cercis]` |
 | `pre-commit` usage     | `args: [--use-tabs=False]`               |
 
-- `--tab-width` (int): when calculating line length (to determine whether to
-  wrap lines), how wide shall _Cercis_ treat each tab. Only effective when
-  `--use-tabs` is set to `True`.
+- `--tab-width` (int): when calculating line length (to determine whether to wrap
+  lines), how wide shall _Cercis_ treat each tab. Only effective when `--use-tabs` is
+  set to `True`.
 
 | Option                 |                                       |
 | ---------------------- | ------------------------------------- |
 | Name                   | `--tab-width`                         |
 | Abbreviation           | `-tw`                                 |
 | Default                | 4                                     |
 | Black's default        | N/A                                   |
 | Command line usage     | `cercis -tab=True -tw=2 myScript.py`  |
 | `pyproject.toml` usage | `tab-width = 2` under `[tool.cercis]` |
 | `pre-commit` usage     | `args: [--tab-width=2]`               |
 
 ### 3.4. Base indentation spaces
 
-This option defines the number of spaces that each indentation level adds. This
-option has no effect when `--use-tabs` is set to `True`.
+This option defines the number of spaces that each indentation level adds. This option
+has no effect when `--use-tabs` is set to `True`.
 
-For example, if you set it to 2, contents within a `for` block is indented 2
-spaces:
+For example, if you set it to 2, contents within a `for` block is indented 2 spaces:
 
 ```python
 for i in (1, 2, 3, 4, 5):
   print(i)
 ```
 
 | Option                 |                                                     |
@@ -249,17 +242,16 @@
 
 There are three associated options:
 
 - `--function-definition-extra-indent`
 - `--other-line-continuation-extra-indent`
 - `--closing-bracket-extra-indent`
 
-They control whether we add an **additional** indentation level in some
-situations. Note that these options can work well with tabs
-(`--use-tabs=True`).
+They control whether we add an **additional** indentation level in some situations. Note
+that these options can work well with tabs (`--use-tabs=True`).
 
 #### 3.5.1. At function definition (`--function-definition-extra-indent`)
 
 <table>
   <tr>
     <td>
 
@@ -290,55 +282,53 @@
 ```
 
   </td>
 
   </tr>
 </table>
 
-We choose to add an extra indentation level when wrapping a function signature
-line. This is because `def␣` happens to be 4 characters, so when the base
-indentation is 4 spaces, it can be difficult to visually distinguish the
-function name and the argument list if we don't add an extra indentation.
+We choose to add an extra indentation level when wrapping a function signature line.
+This is because `def␣` happens to be 4 characters, so when the base indentation is 4
+spaces, it can be difficult to visually distinguish the function name and the argument
+list if we don't add an extra indentation.
 
-If you set `--base-indentation-spaces` to other values than 4, this visual
-separation issue will disappear, and you may not need to turn this option on.
+If you set `--base-indentation-spaces` to other values than 4, this visual separation
+issue will disappear, and you may not need to turn this option on.
 
-This style is encouraged
-[in PEP8](https://peps.python.org/pep-0008/#indentation).
+This style is encouraged [in PEP8](https://peps.python.org/pep-0008/#indentation).
 
 | Option                 |                                                                 |
 | ---------------------- | --------------------------------------------------------------- |
 | Name                   | `--function-definition-extra-indent`                            |
 | Abbreviation           | `-fdei`                                                         |
 | Default                | `True`                                                          |
 | Black's default        | `False`                                                         |
 | Command line usage     | `cercis -fdei=False myScript.py`                                |
 | `pyproject.toml` usage | `function-definition-extra-indent = true` under `[tool.cercis]` |
 | `pre-commit` usage     | `args: [--function-definition-extra-indent=False]`              |
 
 #### 3.5.2. In other line continuations (`--other-line-continuation-extra-indent`)
 
-"Other line continuations" are cases other than in function definitions, such
-as:
+"Other line continuations" are cases other than in function definitions, such as:
 
 ```python
 var = some_function(
     arg1_with_long_name,
     arg2_with_longer_name,
 )
 
 var2 = [
     'something',
     'something else',
     'something more',
 ]
 ```
 
-So if you set this option (`--other-line-continuation-extra-indent`) to `True`,
-you can add an extra level of indentation in these cases:
+So if you set this option (`--other-line-continuation-extra-indent`) to `True`, you can
+add an extra level of indentation in these cases:
 
 ```python
 var = some_function(
         arg1_with_long_name,
         arg2_with_longer_name,
 )
 
@@ -357,17 +347,16 @@
 | Black's default        | `False`                                                             |
 | Command line usage     | `cercis -olcei=True myScript.py`                                    |
 | `pyproject.toml` usage | `other-line-continuation-extra-indent = true` under `[tool.cercis]` |
 | `pre-commit` usage     | `args: [----other-line-continuation-extra-indent=False]`            |
 
 #### 3.5.3. At closing brackets (`--closing-bracket-extra-indent`)
 
-This option lets people customize where the closing bracket should be. Note
-that both styles are OK according to
-[PEP8](https://peps.python.org/pep-0008/#indentation).
+This option lets people customize where the closing bracket should be. Note that both
+styles are OK according to [PEP8](https://peps.python.org/pep-0008/#indentation).
 
 <table>
   <tr>
     <td>
 
 ```python
 # --closing-bracket-extra-indent=False
@@ -436,17 +425,16 @@
 | Black's default        | `False`                                                     |
 | Command line usage     | `cercis -cbei=True myScript.py`                             |
 | `pyproject.toml` usage | `closing-bracket-extra-indent = true` under `[tool.cercis]` |
 | `pre-commit` usage     | `args: [--closing-bracket-extra-indent=False]`              |
 
 ### 3.6. "Simple" lines with long strings
 
-By default, Black wraps lines that exceed length limit. But for very simple
-lines (such as assigning a long string to a variable), line wrapping is not
-necessary.
+By default, Black wraps lines that exceed length limit. But for very simple lines (such
+as assigning a long string to a variable), line wrapping is not necessary.
 
 <table>
   <tr>
     <td>
 
 ```python
 # Cercis's default style
@@ -577,171 +565,220 @@
 | Command line usage     | `cercis -cnb=True myScript.py`                          |
 | `pyproject.toml` usage | `collapse-nested-brackets = true` under `[tool.cercis]` |
 | `pre-commit` usage     | `args: [--collapse-nested-brackets=False]`              |
 
 The code implementation of this option comes from
 [Pyink](https://github.com/google/pyink), another forked project from Black.
 
-### 3.8. Wrapping long lines ending with pragma comments
+### 3.8. Wrapping long lines ending with comments
+
+Sometimes we have lines that exceed the length limit only because of the in-line
+comment. If we do not want to wrap those lines, we can use two options provided here:
 
-"Pragma comments", in this context, mean the directives for Python linters
-usually to tell them to ignore certain errors. Pragma comments that _Cercis_
-currently recognizes include:
+- `--wrap-comments`
+- `--wrap-pragma-comments`
+
+"Pragma comments", in this context, mean the directives for Python linters usually to
+tell them to ignore certain errors. Pragma comments that _Cercis_ currently recognizes
+include:
 
 - _noqa_: `# noqa: E501`
 - _type: ignore_: `# type: ignore[no-untyped-def]`
 - _pylint_: `# pylint: disable=protected-access`
 - _pytype_: `# pytype: disable=attribute-error`
 
-<table>
-  <tr>
-    <td>
+| Option                 |                                              |
+| ---------------------- | -------------------------------------------- |
+| Name                   | `--wrap-comments`                            |
+| Abbreviation           | `-wc`                                        |
+| Default                | `False`                                      |
+| Black's style          | `True`                                       |
+| Command line usage     | `cercis -wc=True myScript.py`                |
+| `pyproject.toml` usage | `wrap-comments = true` under `[tool.cercis]` |
+| `pre-commit` usage     | `args: [--wrap-comments=False]`              |
 
-```python
-# Cercis's default style
-# (Suppose line length limit is 30)
+| Option                 |                                                     |
+| ---------------------- | --------------------------------------------------- |
+| Name                   | `--wrap-pragma-comments`                            |
+| Abbreviation           | `-wpc`                                              |
+| Default                | `False`                                             |
+| Black's style          | `True`                                              |
+| Command line usage     | `cercis -wpc=True myScript.py`                      |
+| `pyproject.toml` usage | `wrap-pragma-comments = true` under `[tool.cercis]` |
+| `pre-commit` usage     | `args: [--wrap-pragma-comments=False]`              |
 
-# This line has 30 characters
-var = some_func(some_long_arg)  # noqa:F501
+And below is a 2x2 matrix to explain how these two options work together:
 
-# This line has 31 characters
-var_ = some_func(
-    some_long_arg
-)  # type: ignore
-
-# Cercis doesn't wraps a line if its main
-# content (without the comment) does not
-# exceed the line length limit.
+|              | `-wc=True`                          | `-wc=False`             |
+| ------------ | ----------------------------------- | ----------------------- |
+| `-wpc=True`  | All comments wrapped w.n.           | No comments are wrapped |
+| `-wpc=False` | p.c. not wrapped; o.c. wrapped w.n. | No comments are wrapped |
 
+Note:
 
+- "w.n." means "when necessary"
+- "p.c." means "pragma comments"
+- "o.c." means "other comments"
 
+### 3.9. Keep blank lines in brackets
 
+This option allows us to keep the blank lines that we intentionally add into the
+contents of brackets.
+
+<table>
+  <tr>
+    <td>
 
+Cercis's default style:
+
+```python
+my_list = [
+    # Group 1
+    1,
+    2,
+
+    # Group 2
+    3,
+    4,
+
+    # Group 3
+    5,
+    6,
+]
 ```
 
   </td>
 
   <td>
 
+Black's default style (not configurable):
+
 ```python
-# Black's style (not configurable)
-# (Suppose line length limit is 30)
+my_list = [
+    # Group 1
+    1,
+    2,
+    # Group 2
+    3,
+    4,
+    # Group 3
+    5,
+    6,
+]
+
 
-# Black doesn't wrap lines, no matter
-# how long, if the line has
-# a "# type: ignore..." comment.
-# (This line has 31 characters.)
-var_ = some_func(some_long_arg)  # type: ignore
-
-# Black does not recognize "# type:ignore",
-# even though mypy recognizes it.
-var_ = some_func(
-    some_long_arg
-)  # type:ignore
-
-# Black only recognizes "# type: ignore"
-var_ = some_func(
-    some_long_arg
-)  # noqa:F501
 ```
 
   </td>
 
   </tr>
 </table>
 
-| Option                 |                                                     |
-| ---------------------- | --------------------------------------------------- |
-| Name                   | `--wrap-pragma-comments`                            |
-| Abbreviation           | `-wpc`                                              |
-| Default                | `False`                                             |
-| Black's style          | `True`                                              |
-| Command line usage     | `cercis -wpc=True myScript.py`                      |
-| `pyproject.toml` usage | `wrap-pragma-comments = true` under `[tool.cercis]` |
-| `pre-commit` usage     | `args: [--wrap-pragma-comments=False]`              |
+| Option                 |                                                             |
+| ---------------------- | ----------------------------------------------------------- |
+| Name                   | `--keep-blank-lines-in-brackets`                            |
+| Abbreviation           | `-kblib`                                                    |
+| Default                | `True`                                                      |
+| Black's style          | `False`                                                     |
+| Command line usage     | `cercis -kblib=True myScript.py`                            |
+| `pyproject.toml` usage | `keep-blank-lines-in-brackets = true` under `[tool.cercis]` |
+| `pre-commit` usage     | `args: [--keep-blank-lines-in-bracketss=False]`             |
+
+(Note: if `--keep-blank-lines-in-brackets` is `True`, multiple consecutive blank lines
+are compressed into one blank line after formatting.)
 
 ## 4. How to configure _Cercis_
 
 ### 4.1. Dynamically in the command line
 
 Here are some examples:
 
 - `cercis --single-quote=True myScript.py` to format files to single quotes
-- `cercis --function-definition-extra-indent=False myScript.py` to format files
-  without extra indentation at function definition
-- `cercis --line-length=79 myScript.py` to format files with a line length of
-  79 characters
+- `cercis --function-definition-extra-indent=False myScript.py` to format files without
+  extra indentation at function definition
+- `cercis --line-length=79 myScript.py` to format files with a line length of 79
+  characters
 
 ### 4.2. In your project's `pyproject.toml` file
 
 You can specify the options under the `[tool.cercis]` section of the file:
 
 ```toml
 [tool.cercis]
 line-length = 88
 function-definition-extra-indent = true
 single-quote = false
 ```
 
 ### 4.3. In your project's `.pre-commit-config.yaml` file
 
-You can specify the options under the `args` section of your
-`.pre-commit-config.yaml` file.
+You can specify the options under the `args` section of your `.pre-commit-config.yaml`
+file.
 
 For example:
 
 ```yaml
 repos:
   - repo: https://github.com/jsh9/cercis
     rev: 0.1.0
     hooks:
       - id: cercis
-        args: [--function-definition-extra-indent=False, --ling-length=79]
+        args: [--function-definition-extra-indent=False, --line-length=79]
   - repo: https://github.com/jsh9/cercis
     rev: 0.1.0
     hooks:
       - id: cercis-jupyter
         args: [--function-definition-extra-indent=False, --line-length=79]
 ```
 
-The value in `rev` can be any _Cercis_ release, or it can be `main`, which
-means to always use the latest (including unreleased) _Cercis_ features.
+The value in `rev` can be any _Cercis_ release, or it can be `main`, which means to
+always use the latest (including unreleased) _Cercis_ features.
 
 ### 4.4. Specify options in `tox.ini`
 
-Currently, _Cercis_ does not support a config section in `tox.ini`. Instead,
-you can specify the options in `pyproject.toml`.
+Currently, _Cercis_ does not support a config section in `tox.ini`. Instead, you can
+specify the options in `pyproject.toml`.
 
 ### 4.5. How to fall back to Black's behavior
 
-Here are the configuration options to fall back to Black's behavior. Put them
-in `pyproject.toml`:
+Here are the configuration options to fall back to Black's behavior. Put them in
+`pyproject.toml`:
 
 ```toml
 [tool.cercis]
 line-length = 88
 single-quote = false
 use-tabs = false
 base-indentation-spaces = 4
 function-definition-extra-indent = false
 other-line-continuation-extra-indent = false
 closing-bracket-extra-indent = false
 wrap-line-with-long-string = true
 collapse-nested-brackets = false
+wrap-comments = true
 wrap-pragma-comments = true
 ```
 # Change Log
 
+## [0.1.6] - 2023-05-23
+
+- Added
+  - A new option `--wrap-comments` to not wrap any comments (not just pragma comments)
+  - A new option `--keep-blank-lines-in-brackets`
+- Changed
+  - Improved the CLI output text colors because the current colors are confusing or not
+    quite legible
+
 ## [0.1.5] - 2023-05-09
 
 - Added
-  - Configurability to use tabs instead of spaces (two new options:
-    `--use-tabs` and `--tab-width`)
-  - Configurability on base indentation spaces and extra indentation at
-    different line continuation situations
+  - Configurability to use tabs instead of spaces (two new options: `--use-tabs` and
+    `--tab-width`)
+  - Configurability on base indentation spaces and extra indentation at different line
+    continuation situations
 
 ## [0.1.4] - 2023-05-07
 
 - Added
   - A new configurable option: `--closing-bracket-extra-indent`
 
 ## [0.1.3] - 2023-05-07
@@ -759,34 +796,32 @@
 
 - Removed
   - Some unrelated documentation and config files
 
 ## [0.1.2] - 2023-05-04
 
 - Added
-  - Merged 2 changes from psf/black:main
-    ([#5](https://github.com/jsh9/cercis/pull/5))
+  - Merged 2 changes from psf/black:main ([#5](https://github.com/jsh9/cercis/pull/5))
   - Added option to not wrap "simple" lines with long strings
     ([#6](https://github.com/jsh9/cercis/pull/6))
 - Full changelog
   - https://github.com/jsh9/cercis/compare/0.1.1...0.1.2
 
 ## [0.1.1] - 2023-05-03
 
 - Added
-  - A configurable option: `single-quote`, for formatting code into single
-    quotes
+  - A configurable option: `single-quote`, for formatting code into single quotes
 - Full changelog
   - https://github.com/jsh9/cercis/compare/0.1.0...0.1.1
 
 ## [0.1.0] - 2023-04-30
 
 - This is the initial version that branches away from Black (commit:
   [e712e4](https://github.com/psf/black/commit/e712e48e06420d9240ce95c81acfcf6f11d14c83))
 - Changed
-  - The default indentation within a function definition (when line wrap
-    happens) is now 8 spaces. (Black's default is 4, which is
+  - The default indentation within a function definition (when line wrap happens) is now
+    8 spaces. (Black's default is 4, which is
     [not PEP8-compatible](https://github.com/psf/black/issues/1127))
   - Updated README, because `cercis` now branches away from Black
 - Added
-  - A configurable option (`function-definition-extra-indent`) is added instead
-    of enforcing 8 spaces for everyone
+  - A configurable option (`function-definition-extra-indent`) is added instead of
+    enforcing 8 spaces for everyone
```

