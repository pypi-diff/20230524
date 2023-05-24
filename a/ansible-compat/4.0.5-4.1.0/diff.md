# Comparing `tmp/ansible-compat-4.0.5.tar.gz` & `tmp/ansible-compat-4.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ansible-compat-4.0.5.tar", last modified: Sun May 21 12:32:44 2023, max compression
+gzip compressed data, was "ansible-compat-4.1.0.tar", last modified: Wed May 24 13:41:15 2023, max compression
```

## Comparing `ansible-compat-4.0.5.tar` & `ansible-compat-4.1.0.tar`

### file list

```diff
@@ -1,117 +1,118 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 12:32:44.496278 ansible-compat-4.0.5/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 12:32:44.488278 ansible-compat-4.0.5/.github/
--rw-r--r--   0 runner    (1001) docker     (123)       26 2023-05-21 12:32:28.000000 ansible-compat-4.0.5/.github/CODEOWNERS
--rw-r--r--   0 runner    (1001) docker     (123)      162 2023-05-21 12:32:28.000000 ansible-compat-4.0.5/.github/CODE_OF_CONDUCT.md
--rw-r--r--   0 runner    (1001) docker     (123)      593 2023-05-21 12:32:28.000000 ansible-compat-4.0.5/.github/dependabot.yml
--rw-r--r--   0 runner    (1001) docker     (123)       69 2023-05-21 12:32:28.000000 ansible-compat-4.0.5/.github/release-drafter.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 12:32:44.488278 ansible-compat-4.0.5/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)      240 2023-05-21 12:32:28.000000 ansible-compat-4.0.5/.github/workflows/ack.yml
--rw-r--r--   0 runner    (1001) docker     (123)      244 2023-05-21 12:32:28.000000 ansible-compat-4.0.5/.github/workflows/push.yml
--rw-r--r--   0 runner    (1001) docker     (123)      997 2023-05-21 12:32:28.000000 ansible-compat-4.0.5/.github/workflows/release.yml
--rw-r--r--   0 runner    (1001) docker     (123)     3085 2023-05-21 12:32:28.000000 ansible-compat-4.0.5/.github/workflows/tox.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1808 2023-05-21 12:32:28.000000 ansible-compat-4.0.5/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)     3807 2023-05-21 12:32:28.000000 ansible-compat-4.0.5/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)       13 2023-05-21 12:32:28.000000 ansible-compat-4.0.5/.prettierignore
--rw-r--r--   0 runner    (1001) docker     (123)      355 2023-05-21 12:32:28.000000 ansible-compat-4.0.5/.prettierrc.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1041 2023-05-21 12:32:28.000000 ansible-compat-4.0.5/.readthedocs.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 12:32:44.488278 ansible-compat-4.0.5/.vscode/
--rw-r--r--   0 runner    (1001) docker     (123)      458 2023-05-21 12:32:28.000000 ansible-compat-4.0.5/.vscode/extensions.json
--rw-r--r--   0 runner    (1001) docker     (123)     1401 2023-05-21 12:32:28.000000 ansible-compat-4.0.5/.vscode/settings.json
--rw-r--r--   0 runner    (1001) docker     (123)      175 2023-05-21 12:32:28.000000 ansible-compat-4.0.5/.yamllint
--rw-r--r--   0 runner    (1001) docker     (123)     1095 2023-05-21 12:32:28.000000 ansible-compat-4.0.5/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     2244 2023-05-21 12:32:44.496278 ansible-compat-4.0.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      764 2023-05-21 12:32:28.000000 ansible-compat-4.0.5/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      123 2023-05-21 12:32:28.000000 ansible-compat-4.0.5/codecov.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 12:32:44.488278 ansible-compat-4.0.5/docs/
--rw-r--r--   0 runner    (1001) docker     (123)      170 2023-05-21 12:32:28.000000 ansible-compat-4.0.5/docs/api.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 12:32:44.492278 ansible-compat-4.0.5/docs/images/
--rw-r--r--   0 runner    (1001) docker     (123)    15406 2023-05-21 12:32:28.000000 ansible-compat-4.0.5/docs/images/favicon.ico
--rw-r--r--   0 runner    (1001) docker     (123)    10993 2023-05-21 12:32:28.000000 ansible-compat-4.0.5/docs/images/logo.png
--rw-r--r--   0 runner    (1001) docker     (123)     1047 2023-05-21 12:32:28.000000 ansible-compat-4.0.5/docs/images/logo.svg
--rw-r--r--   0 runner    (1001) docker     (123)      360 2023-05-21 12:32:28.000000 ansible-compat-4.0.5/docs/index.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 12:32:44.484278 ansible-compat-4.0.5/examples/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 12:32:44.492278 ansible-compat-4.0.5/examples/reqs_broken/
--rw-r--r--   0 runner    (1001) docker     (123)      125 2023-05-21 12:32:28.000000 ansible-compat-4.0.5/examples/reqs_broken/requirements.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 12:32:44.492278 ansible-compat-4.0.5/examples/reqs_v1/
--rw-r--r--   0 runner    (1001) docker     (123)      179 2023-05-21 12:32:28.000000 ansible-compat-4.0.5/examples/reqs_v1/requirements.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 12:32:44.492278 ansible-compat-4.0.5/examples/reqs_v2/
--rw-r--r--   0 runner    (1001) docker     (123)     7615 2023-05-21 12:32:28.000000 ansible-compat-4.0.5/examples/reqs_v2/community-molecule-0.1.0.tar.gz
--rw-r--r--   0 runner    (1001) docker     (123)      393 2023-05-21 12:32:28.000000 ansible-compat-4.0.5/examples/reqs_v2/requirements.yml
--rw-r--r--   0 runner    (1001) docker     (123)     2265 2023-05-21 12:32:28.000000 ansible-compat-4.0.5/mkdocs.yml
--rw-r--r--   0 runner    (1001) docker     (123)     4274 2023-05-21 12:32:28.000000 ansible-compat-4.0.5/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      263 2023-05-21 12:32:28.000000 ansible-compat-4.0.5/readthedocs.yml
--rw-r--r--   0 runner    (1001) docker     (123)     6305 2023-05-21 12:32:28.000000 ansible-compat-4.0.5/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-21 12:32:44.496278 ansible-compat-4.0.5/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 12:32:44.484278 ansible-compat-4.0.5/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 12:32:44.492278 ansible-compat-4.0.5/src/ansible_compat/
--rw-r--r--   0 runner    (1001) docker     (123)      246 2023-05-21 12:32:28.000000 ansible-compat-4.0.5/src/ansible_compat/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    16108 2023-05-21 12:32:28.000000 ansible-compat-4.0.5/src/ansible_compat/config.py
--rw-r--r--   0 runner    (1001) docker     (123)     1469 2023-05-21 12:32:28.000000 ansible-compat-4.0.5/src/ansible_compat/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)     1511 2023-05-21 12:32:28.000000 ansible-compat-4.0.5/src/ansible_compat/errors.py
--rw-r--r--   0 runner    (1001) docker     (123)      920 2023-05-21 12:32:28.000000 ansible-compat-4.0.5/src/ansible_compat/loaders.py
--rw-r--r--   0 runner    (1001) docker     (123)      112 2023-05-21 12:32:28.000000 ansible-compat-4.0.5/src/ansible_compat/ports.py
--rw-r--r--   0 runner    (1001) docker     (123)      807 2023-05-21 12:32:28.000000 ansible-compat-4.0.5/src/ansible_compat/prerun.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-21 12:32:28.000000 ansible-compat-4.0.5/src/ansible_compat/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    31920 2023-05-21 12:32:28.000000 ansible-compat-4.0.5/src/ansible_compat/runtime.py
--rw-r--r--   0 runner    (1001) docker     (123)     3216 2023-05-21 12:32:28.000000 ansible-compat-4.0.5/src/ansible_compat/schema.py
--rw-r--r--   0 runner    (1001) docker     (123)      552 2023-05-21 12:32:28.000000 ansible-compat-4.0.5/src/ansible_compat/types.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 12:32:44.492278 ansible-compat-4.0.5/src/ansible_compat.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2244 2023-05-21 12:32:44.000000 ansible-compat-4.0.5/src/ansible_compat.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2330 2023-05-21 12:32:44.000000 ansible-compat-4.0.5/src/ansible_compat.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-21 12:32:44.000000 ansible-compat-4.0.5/src/ansible_compat.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      253 2023-05-21 12:32:44.000000 ansible-compat-4.0.5/src/ansible_compat.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       15 2023-05-21 12:32:44.000000 ansible-compat-4.0.5/src/ansible_compat.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 12:32:44.492278 ansible-compat-4.0.5/test/
--rw-r--r--   0 runner    (1001) docker     (123)       40 2023-05-21 12:32:28.000000 ansible-compat-4.0.5/test/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 12:32:44.496278 ansible-compat-4.0.5/test/assets/
--rw-r--r--   0 runner    (1001) docker     (123)      102 2023-05-21 12:32:28.000000 ansible-compat-4.0.5/test/assets/requirements-invalid-collection.yml
--rw-r--r--   0 runner    (1001) docker     (123)       98 2023-05-21 12:32:28.000000 ansible-compat-4.0.5/test/assets/requirements-invalid-role.yml
--rw-r--r--   0 runner    (1001) docker     (123)       57 2023-05-21 12:32:28.000000 ansible-compat-4.0.5/test/assets/validate0_data.json
--rw-r--r--   0 runner    (1001) docker     (123)      631 2023-05-21 12:32:28.000000 ansible-compat-4.0.5/test/assets/validate0_expected.json
--rw-r--r--   0 runner    (1001) docker     (123)      184 2023-05-21 12:32:28.000000 ansible-compat-4.0.5/test/assets/validate0_schema.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 12:32:44.484278 ansible-compat-4.0.5/test/collections/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 12:32:44.496278 ansible-compat-4.0.5/test/collections/acme.broken/
--rw-r--r--   0 runner    (1001) docker     (123)       37 2023-05-21 12:32:28.000000 ansible-compat-4.0.5/test/collections/acme.broken/galaxy.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 12:32:44.496278 ansible-compat-4.0.5/test/collections/acme.goodies/
--rw-r--r--   0 runner    (1001) docker     (123)      573 2023-05-21 12:32:28.000000 ansible-compat-4.0.5/test/collections/acme.goodies/galaxy.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 12:32:44.484278 ansible-compat-4.0.5/test/collections/acme.goodies/molecule/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 12:32:44.496278 ansible-compat-4.0.5/test/collections/acme.goodies/molecule/default/
--rw-r--r--   0 runner    (1001) docker     (123)      158 2023-05-21 12:32:28.000000 ansible-compat-4.0.5/test/collections/acme.goodies/molecule/default/converge.yml
--rw-r--r--   0 runner    (1001) docker     (123)      142 2023-05-21 12:32:28.000000 ansible-compat-4.0.5/test/collections/acme.goodies/molecule/default/molecule.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 12:32:44.484278 ansible-compat-4.0.5/test/collections/acme.goodies/roles/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 12:32:44.484278 ansible-compat-4.0.5/test/collections/acme.goodies/roles/baz/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 12:32:44.484278 ansible-compat-4.0.5/test/collections/acme.goodies/roles/baz/molecule/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 12:32:44.496278 ansible-compat-4.0.5/test/collections/acme.goodies/roles/baz/molecule/deep_scenario/
--rw-r--r--   0 runner    (1001) docker     (123)      156 2023-05-21 12:32:28.000000 ansible-compat-4.0.5/test/collections/acme.goodies/roles/baz/molecule/deep_scenario/converge.yml
--rw-r--r--   0 runner    (1001) docker     (123)      142 2023-05-21 12:32:28.000000 ansible-compat-4.0.5/test/collections/acme.goodies/roles/baz/molecule/deep_scenario/molecule.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 12:32:44.496278 ansible-compat-4.0.5/test/collections/acme.goodies/roles/baz/tasks/
--rw-r--r--   0 runner    (1001) docker     (123)       79 2023-05-21 12:32:28.000000 ansible-compat-4.0.5/test/collections/acme.goodies/roles/baz/tasks/main.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 12:32:44.496278 ansible-compat-4.0.5/test/collections/acme.goodies/tests/
--rw-r--r--   0 runner    (1001) docker     (123)       58 2023-05-21 12:32:28.000000 ansible-compat-4.0.5/test/collections/acme.goodies/tests/requirements.yml
--rw-r--r--   0 runner    (1001) docker     (123)      729 2023-05-21 12:32:28.000000 ansible-compat-4.0.5/test/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 12:32:44.488278 ansible-compat-4.0.5/test/roles/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 12:32:44.496278 ansible-compat-4.0.5/test/roles/acme.missing_deps/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 12:32:44.496278 ansible-compat-4.0.5/test/roles/acme.missing_deps/meta/
--rw-r--r--   0 runner    (1001) docker     (123)      136 2023-05-21 12:32:28.000000 ansible-compat-4.0.5/test/roles/acme.missing_deps/meta/main.yml
--rw-r--r--   0 runner    (1001) docker     (123)       87 2023-05-21 12:32:28.000000 ansible-compat-4.0.5/test/roles/acme.missing_deps/requirements.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 12:32:44.488278 ansible-compat-4.0.5/test/roles/acme.sample2/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 12:32:44.496278 ansible-compat-4.0.5/test/roles/acme.sample2/meta/
--rw-r--r--   0 runner    (1001) docker     (123)      308 2023-05-21 12:32:28.000000 ansible-compat-4.0.5/test/roles/acme.sample2/meta/main.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 12:32:44.488278 ansible-compat-4.0.5/test/roles/ansible-role-sample/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 12:32:44.496278 ansible-compat-4.0.5/test/roles/ansible-role-sample/meta/
--rw-r--r--   0 runner    (1001) docker     (123)      259 2023-05-21 12:32:28.000000 ansible-compat-4.0.5/test/roles/ansible-role-sample/meta/main.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 12:32:44.488278 ansible-compat-4.0.5/test/roles/sample3/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 12:32:44.496278 ansible-compat-4.0.5/test/roles/sample3/meta/
--rw-r--r--   0 runner    (1001) docker     (123)      308 2023-05-21 12:32:28.000000 ansible-compat-4.0.5/test/roles/sample3/meta/main.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 12:32:44.488278 ansible-compat-4.0.5/test/roles/sample4/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 12:32:44.496278 ansible-compat-4.0.5/test/roles/sample4/meta/
--rw-r--r--   0 runner    (1001) docker     (123)      308 2023-05-21 12:32:28.000000 ansible-compat-4.0.5/test/roles/sample4/meta/main.yml
--rw-r--r--   0 runner    (1001) docker     (123)      102 2023-05-21 12:32:28.000000 ansible-compat-4.0.5/test/test_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     2897 2023-05-21 12:32:28.000000 ansible-compat-4.0.5/test/test_config.py
--rw-r--r--   0 runner    (1001) docker     (123)      430 2023-05-21 12:32:28.000000 ansible-compat-4.0.5/test/test_configuration_example.py
--rw-r--r--   0 runner    (1001) docker     (123)      273 2023-05-21 12:32:28.000000 ansible-compat-4.0.5/test/test_loaders.py
--rw-r--r--   0 runner    (1001) docker     (123)      344 2023-05-21 12:32:28.000000 ansible-compat-4.0.5/test/test_prerun.py
--rw-r--r--   0 runner    (1001) docker     (123)    25494 2023-05-21 12:32:28.000000 ansible-compat-4.0.5/test/test_runtime.py
--rw-r--r--   0 runner    (1001) docker     (123)      934 2023-05-21 12:32:28.000000 ansible-compat-4.0.5/test/test_runtime_example.py
--rw-r--r--   0 runner    (1001) docker     (123)     2377 2023-05-21 12:32:28.000000 ansible-compat-4.0.5/test/test_schema.py
--rw-r--r--   0 runner    (1001) docker     (123)     4251 2023-05-21 12:32:28.000000 ansible-compat-4.0.5/tox.ini
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 13:41:15.346953 ansible-compat-4.1.0/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 13:41:15.322954 ansible-compat-4.1.0/.github/
+-rw-r--r--   0 runner    (1001) docker     (123)       26 2023-05-24 13:40:59.000000 ansible-compat-4.1.0/.github/CODEOWNERS
+-rw-r--r--   0 runner    (1001) docker     (123)      162 2023-05-24 13:40:59.000000 ansible-compat-4.1.0/.github/CODE_OF_CONDUCT.md
+-rw-r--r--   0 runner    (1001) docker     (123)      593 2023-05-24 13:40:59.000000 ansible-compat-4.1.0/.github/dependabot.yml
+-rw-r--r--   0 runner    (1001) docker     (123)       69 2023-05-24 13:40:59.000000 ansible-compat-4.1.0/.github/release-drafter.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 13:41:15.322954 ansible-compat-4.1.0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      240 2023-05-24 13:40:59.000000 ansible-compat-4.1.0/.github/workflows/ack.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      244 2023-05-24 13:40:59.000000 ansible-compat-4.1.0/.github/workflows/push.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      997 2023-05-24 13:40:59.000000 ansible-compat-4.1.0/.github/workflows/release.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     3085 2023-05-24 13:40:59.000000 ansible-compat-4.1.0/.github/workflows/tox.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1828 2023-05-24 13:40:59.000000 ansible-compat-4.1.0/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)     3807 2023-05-24 13:40:59.000000 ansible-compat-4.1.0/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-05-24 13:40:59.000000 ansible-compat-4.1.0/.prettierignore
+-rw-r--r--   0 runner    (1001) docker     (123)      355 2023-05-24 13:40:59.000000 ansible-compat-4.1.0/.prettierrc.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1041 2023-05-24 13:40:59.000000 ansible-compat-4.1.0/.readthedocs.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 13:41:15.322954 ansible-compat-4.1.0/.vscode/
+-rw-r--r--   0 runner    (1001) docker     (123)      458 2023-05-24 13:40:59.000000 ansible-compat-4.1.0/.vscode/extensions.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1324 2023-05-24 13:40:59.000000 ansible-compat-4.1.0/.vscode/settings.json
+-rw-r--r--   0 runner    (1001) docker     (123)      175 2023-05-24 13:40:59.000000 ansible-compat-4.1.0/.yamllint
+-rw-r--r--   0 runner    (1001) docker     (123)     1095 2023-05-24 13:40:59.000000 ansible-compat-4.1.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     2244 2023-05-24 13:41:15.346953 ansible-compat-4.1.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      764 2023-05-24 13:40:59.000000 ansible-compat-4.1.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       90 2023-05-24 13:40:59.000000 ansible-compat-4.1.0/ansible.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      123 2023-05-24 13:40:59.000000 ansible-compat-4.1.0/codecov.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 13:41:15.322954 ansible-compat-4.1.0/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)      170 2023-05-24 13:40:59.000000 ansible-compat-4.1.0/docs/api.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 13:41:15.326954 ansible-compat-4.1.0/docs/images/
+-rw-r--r--   0 runner    (1001) docker     (123)    15406 2023-05-24 13:40:59.000000 ansible-compat-4.1.0/docs/images/favicon.ico
+-rw-r--r--   0 runner    (1001) docker     (123)    10993 2023-05-24 13:40:59.000000 ansible-compat-4.1.0/docs/images/logo.png
+-rw-r--r--   0 runner    (1001) docker     (123)     1047 2023-05-24 13:40:59.000000 ansible-compat-4.1.0/docs/images/logo.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      360 2023-05-24 13:40:59.000000 ansible-compat-4.1.0/docs/index.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 13:41:15.302954 ansible-compat-4.1.0/examples/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 13:41:15.326954 ansible-compat-4.1.0/examples/reqs_broken/
+-rw-r--r--   0 runner    (1001) docker     (123)      125 2023-05-24 13:40:59.000000 ansible-compat-4.1.0/examples/reqs_broken/requirements.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 13:41:15.326954 ansible-compat-4.1.0/examples/reqs_v1/
+-rw-r--r--   0 runner    (1001) docker     (123)      179 2023-05-24 13:40:59.000000 ansible-compat-4.1.0/examples/reqs_v1/requirements.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 13:41:15.326954 ansible-compat-4.1.0/examples/reqs_v2/
+-rw-r--r--   0 runner    (1001) docker     (123)     7615 2023-05-24 13:40:59.000000 ansible-compat-4.1.0/examples/reqs_v2/community-molecule-0.1.0.tar.gz
+-rw-r--r--   0 runner    (1001) docker     (123)      393 2023-05-24 13:40:59.000000 ansible-compat-4.1.0/examples/reqs_v2/requirements.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     2265 2023-05-24 13:40:59.000000 ansible-compat-4.1.0/mkdocs.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     4298 2023-05-24 13:40:59.000000 ansible-compat-4.1.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      263 2023-05-24 13:40:59.000000 ansible-compat-4.1.0/readthedocs.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     6305 2023-05-24 13:40:59.000000 ansible-compat-4.1.0/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-24 13:41:15.346953 ansible-compat-4.1.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 13:41:15.302954 ansible-compat-4.1.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 13:41:15.330954 ansible-compat-4.1.0/src/ansible_compat/
+-rw-r--r--   0 runner    (1001) docker     (123)      246 2023-05-24 13:40:59.000000 ansible-compat-4.1.0/src/ansible_compat/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16108 2023-05-24 13:40:59.000000 ansible-compat-4.1.0/src/ansible_compat/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1469 2023-05-24 13:40:59.000000 ansible-compat-4.1.0/src/ansible_compat/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1511 2023-05-24 13:40:59.000000 ansible-compat-4.1.0/src/ansible_compat/errors.py
+-rw-r--r--   0 runner    (1001) docker     (123)      920 2023-05-24 13:40:59.000000 ansible-compat-4.1.0/src/ansible_compat/loaders.py
+-rw-r--r--   0 runner    (1001) docker     (123)      112 2023-05-24 13:40:59.000000 ansible-compat-4.1.0/src/ansible_compat/ports.py
+-rw-r--r--   0 runner    (1001) docker     (123)      807 2023-05-24 13:40:59.000000 ansible-compat-4.1.0/src/ansible_compat/prerun.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 13:40:59.000000 ansible-compat-4.1.0/src/ansible_compat/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    34257 2023-05-24 13:40:59.000000 ansible-compat-4.1.0/src/ansible_compat/runtime.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3216 2023-05-24 13:40:59.000000 ansible-compat-4.1.0/src/ansible_compat/schema.py
+-rw-r--r--   0 runner    (1001) docker     (123)      552 2023-05-24 13:40:59.000000 ansible-compat-4.1.0/src/ansible_compat/types.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 13:41:15.334954 ansible-compat-4.1.0/src/ansible_compat.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2244 2023-05-24 13:41:15.000000 ansible-compat-4.1.0/src/ansible_compat.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2342 2023-05-24 13:41:15.000000 ansible-compat-4.1.0/src/ansible_compat.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-24 13:41:15.000000 ansible-compat-4.1.0/src/ansible_compat.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      253 2023-05-24 13:41:15.000000 ansible-compat-4.1.0/src/ansible_compat.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-05-24 13:41:15.000000 ansible-compat-4.1.0/src/ansible_compat.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 13:41:15.338954 ansible-compat-4.1.0/test/
+-rw-r--r--   0 runner    (1001) docker     (123)       40 2023-05-24 13:40:59.000000 ansible-compat-4.1.0/test/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 13:41:15.342954 ansible-compat-4.1.0/test/assets/
+-rw-r--r--   0 runner    (1001) docker     (123)      102 2023-05-24 13:40:59.000000 ansible-compat-4.1.0/test/assets/requirements-invalid-collection.yml
+-rw-r--r--   0 runner    (1001) docker     (123)       98 2023-05-24 13:40:59.000000 ansible-compat-4.1.0/test/assets/requirements-invalid-role.yml
+-rw-r--r--   0 runner    (1001) docker     (123)       57 2023-05-24 13:40:59.000000 ansible-compat-4.1.0/test/assets/validate0_data.json
+-rw-r--r--   0 runner    (1001) docker     (123)      631 2023-05-24 13:40:59.000000 ansible-compat-4.1.0/test/assets/validate0_expected.json
+-rw-r--r--   0 runner    (1001) docker     (123)      184 2023-05-24 13:40:59.000000 ansible-compat-4.1.0/test/assets/validate0_schema.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 13:41:15.302954 ansible-compat-4.1.0/test/collections/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 13:41:15.342954 ansible-compat-4.1.0/test/collections/acme.broken/
+-rw-r--r--   0 runner    (1001) docker     (123)       37 2023-05-24 13:40:59.000000 ansible-compat-4.1.0/test/collections/acme.broken/galaxy.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 13:41:15.342954 ansible-compat-4.1.0/test/collections/acme.goodies/
+-rw-r--r--   0 runner    (1001) docker     (123)      573 2023-05-24 13:40:59.000000 ansible-compat-4.1.0/test/collections/acme.goodies/galaxy.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 13:41:15.306954 ansible-compat-4.1.0/test/collections/acme.goodies/molecule/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 13:41:15.342954 ansible-compat-4.1.0/test/collections/acme.goodies/molecule/default/
+-rw-r--r--   0 runner    (1001) docker     (123)      158 2023-05-24 13:40:59.000000 ansible-compat-4.1.0/test/collections/acme.goodies/molecule/default/converge.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      142 2023-05-24 13:40:59.000000 ansible-compat-4.1.0/test/collections/acme.goodies/molecule/default/molecule.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 13:41:15.306954 ansible-compat-4.1.0/test/collections/acme.goodies/roles/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 13:41:15.306954 ansible-compat-4.1.0/test/collections/acme.goodies/roles/baz/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 13:41:15.306954 ansible-compat-4.1.0/test/collections/acme.goodies/roles/baz/molecule/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 13:41:15.342954 ansible-compat-4.1.0/test/collections/acme.goodies/roles/baz/molecule/deep_scenario/
+-rw-r--r--   0 runner    (1001) docker     (123)      156 2023-05-24 13:40:59.000000 ansible-compat-4.1.0/test/collections/acme.goodies/roles/baz/molecule/deep_scenario/converge.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      142 2023-05-24 13:40:59.000000 ansible-compat-4.1.0/test/collections/acme.goodies/roles/baz/molecule/deep_scenario/molecule.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 13:41:15.342954 ansible-compat-4.1.0/test/collections/acme.goodies/roles/baz/tasks/
+-rw-r--r--   0 runner    (1001) docker     (123)       79 2023-05-24 13:40:59.000000 ansible-compat-4.1.0/test/collections/acme.goodies/roles/baz/tasks/main.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 13:41:15.342954 ansible-compat-4.1.0/test/collections/acme.goodies/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)       58 2023-05-24 13:40:59.000000 ansible-compat-4.1.0/test/collections/acme.goodies/tests/requirements.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      729 2023-05-24 13:40:59.000000 ansible-compat-4.1.0/test/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 13:41:15.310954 ansible-compat-4.1.0/test/roles/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 13:41:15.346953 ansible-compat-4.1.0/test/roles/acme.missing_deps/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 13:41:15.346953 ansible-compat-4.1.0/test/roles/acme.missing_deps/meta/
+-rw-r--r--   0 runner    (1001) docker     (123)      136 2023-05-24 13:40:59.000000 ansible-compat-4.1.0/test/roles/acme.missing_deps/meta/main.yml
+-rw-r--r--   0 runner    (1001) docker     (123)       87 2023-05-24 13:40:59.000000 ansible-compat-4.1.0/test/roles/acme.missing_deps/requirements.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 13:41:15.310954 ansible-compat-4.1.0/test/roles/acme.sample2/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 13:41:15.346953 ansible-compat-4.1.0/test/roles/acme.sample2/meta/
+-rw-r--r--   0 runner    (1001) docker     (123)      308 2023-05-24 13:40:59.000000 ansible-compat-4.1.0/test/roles/acme.sample2/meta/main.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 13:41:15.310954 ansible-compat-4.1.0/test/roles/ansible-role-sample/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 13:41:15.346953 ansible-compat-4.1.0/test/roles/ansible-role-sample/meta/
+-rw-r--r--   0 runner    (1001) docker     (123)      259 2023-05-24 13:40:59.000000 ansible-compat-4.1.0/test/roles/ansible-role-sample/meta/main.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 13:41:15.310954 ansible-compat-4.1.0/test/roles/sample3/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 13:41:15.346953 ansible-compat-4.1.0/test/roles/sample3/meta/
+-rw-r--r--   0 runner    (1001) docker     (123)      308 2023-05-24 13:40:59.000000 ansible-compat-4.1.0/test/roles/sample3/meta/main.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 13:41:15.310954 ansible-compat-4.1.0/test/roles/sample4/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 13:41:15.346953 ansible-compat-4.1.0/test/roles/sample4/meta/
+-rw-r--r--   0 runner    (1001) docker     (123)      308 2023-05-24 13:40:59.000000 ansible-compat-4.1.0/test/roles/sample4/meta/main.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      102 2023-05-24 13:40:59.000000 ansible-compat-4.1.0/test/test_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2897 2023-05-24 13:40:59.000000 ansible-compat-4.1.0/test/test_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)      430 2023-05-24 13:40:59.000000 ansible-compat-4.1.0/test/test_configuration_example.py
+-rw-r--r--   0 runner    (1001) docker     (123)      273 2023-05-24 13:40:59.000000 ansible-compat-4.1.0/test/test_loaders.py
+-rw-r--r--   0 runner    (1001) docker     (123)      344 2023-05-24 13:40:59.000000 ansible-compat-4.1.0/test/test_prerun.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27639 2023-05-24 13:40:59.000000 ansible-compat-4.1.0/test/test_runtime.py
+-rw-r--r--   0 runner    (1001) docker     (123)      934 2023-05-24 13:40:59.000000 ansible-compat-4.1.0/test/test_runtime_example.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2377 2023-05-24 13:40:59.000000 ansible-compat-4.1.0/test/test_schema.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4292 2023-05-24 13:40:59.000000 ansible-compat-4.1.0/tox.ini
```

### Comparing `ansible-compat-4.0.5/.github/dependabot.yml` & `ansible-compat-4.1.0/.github/dependabot.yml`

 * *Files identical despite different names*

### Comparing `ansible-compat-4.0.5/.github/workflows/release.yml` & `ansible-compat-4.1.0/.github/workflows/release.yml`

 * *Files identical despite different names*

### Comparing `ansible-compat-4.0.5/.github/workflows/tox.yml` & `ansible-compat-4.1.0/.github/workflows/tox.yml`

 * *Files identical despite different names*

### Comparing `ansible-compat-4.0.5/.gitignore` & `ansible-compat-4.1.0/.gitignore`

 * *Files 3% similar despite different names*

```diff
@@ -124,7 +124,8 @@
 .dmypy.json
 dmypy.json
 
 # Pyre type checker
 .pyre/
 .test-results
 *.lcov
+ansible_collections
```

### Comparing `ansible-compat-4.0.5/.pre-commit-config.yaml` & `ansible-compat-4.1.0/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `ansible-compat-4.0.5/.readthedocs.yml` & `ansible-compat-4.1.0/.readthedocs.yml`

 * *Files identical despite different names*

### Comparing `ansible-compat-4.0.5/.vscode/settings.json` & `ansible-compat-4.1.0/.vscode/settings.json`

 * *Files 12% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9951923076923077%*

 * *Differences: {"'[python]'": "{'editor.codeActionsOnSave': {delete: ['source.fixAll.ruff', "*

 * *               "'source.organizeImports.ruff']}}"}*

```diff
@@ -1,17 +1,15 @@
 {
     "[markdown]": {
         "editor.defaultFormatter": "esbenp.prettier-vscode"
     },
     "[python]": {
         "editor.codeActionsOnSave": {
             "source.fixAll": true,
-            "source.fixAll.ruff": true,
-            "source.organizeImports": false,
-            "source.organizeImports.ruff": true
+            "source.organizeImports": false
         }
     },
     "editor.formatOnSave": true,
     "evenBetterToml.formatter.alignComments": false,
     "evenBetterToml.formatter.allowedBlankLines": 2,
     "files.exclude": {
         "*.egg-info": true,
```

### Comparing `ansible-compat-4.0.5/LICENSE` & `ansible-compat-4.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `ansible-compat-4.0.5/PKG-INFO` & `ansible-compat-4.1.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ansible-compat
-Version: 4.0.5
+Version: 4.1.0
 Summary: Ansible compatibility goodies
 Author-email: Sorin Sbarnea <ssbarnea@redhat.com>
 Maintainer-email: Sorin Sbarnea <ssbarnea@redhat.com>
 License: MIT
 Project-URL: homepage, https://github.com/ansible/ansible-compat
 Project-URL: documentation, https://ansible-compat.readthedocs.io/
 Project-URL: repository, https://github.com/ansible/ansible-compat
```

### Comparing `ansible-compat-4.0.5/README.md` & `ansible-compat-4.1.0/README.md`

 * *Files identical despite different names*

### Comparing `ansible-compat-4.0.5/docs/images/favicon.ico` & `ansible-compat-4.1.0/docs/images/favicon.ico`

 * *Files identical despite different names*

### Comparing `ansible-compat-4.0.5/docs/images/logo.png` & `ansible-compat-4.1.0/docs/images/logo.png`

 * *Files identical despite different names*

### Comparing `ansible-compat-4.0.5/docs/images/logo.svg` & `ansible-compat-4.1.0/docs/images/logo.svg`

 * *Files identical despite different names*

### Comparing `ansible-compat-4.0.5/examples/reqs_v2/community-molecule-0.1.0.tar.gz` & `ansible-compat-4.1.0/examples/reqs_v2/community-molecule-0.1.0.tar.gz`

 * *Files identical despite different names*

### Comparing `ansible-compat-4.0.5/mkdocs.yml` & `ansible-compat-4.1.0/mkdocs.yml`

 * *Files identical despite different names*

### Comparing `ansible-compat-4.0.5/pyproject.toml` & `ansible-compat-4.1.0/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -108,14 +108,15 @@
 disable = [
   # On purpose disabled as we rely on black
   "line-too-long",
   # local imports do not work well with pre-commit hook
   "import-error",
   # already covered by ruff which is faster
   "too-many-arguments", # PLR0913
+  "raise-missing-from",
   # Temporary disable duplicate detection we remove old code from prerun
   "duplicate-code",
 ]
 
 [tool.pytest.ini_options]
 # ensure we treat warnings as error
 filterwarnings = ["error"]
```

### Comparing `ansible-compat-4.0.5/requirements.txt` & `ansible-compat-4.1.0/requirements.txt`

 * *Files identical despite different names*

### Comparing `ansible-compat-4.0.5/src/ansible_compat/config.py` & `ansible-compat-4.1.0/src/ansible_compat/config.py`

 * *Files identical despite different names*

### Comparing `ansible-compat-4.0.5/src/ansible_compat/constants.py` & `ansible-compat-4.1.0/src/ansible_compat/constants.py`

 * *Files identical despite different names*

### Comparing `ansible-compat-4.0.5/src/ansible_compat/errors.py` & `ansible-compat-4.1.0/src/ansible_compat/errors.py`

 * *Files identical despite different names*

### Comparing `ansible-compat-4.0.5/src/ansible_compat/loaders.py` & `ansible-compat-4.1.0/src/ansible_compat/loaders.py`

 * *Files identical despite different names*

### Comparing `ansible-compat-4.0.5/src/ansible_compat/prerun.py` & `ansible-compat-4.1.0/src/ansible_compat/prerun.py`

 * *Files identical despite different names*

### Comparing `ansible-compat-4.0.5/src/ansible_compat/runtime.py` & `ansible-compat-4.1.0/src/ansible_compat/runtime.py`

 * *Files 4% similar despite different names*

```diff
@@ -6,24 +6,25 @@
 import os
 import re
 import shutil
 import subprocess
 import tempfile
 import warnings
 from collections import OrderedDict
-from dataclasses import dataclass
+from dataclasses import dataclass, field
 from pathlib import Path
-from typing import TYPE_CHECKING, Any, Callable, Optional, Union
+from typing import TYPE_CHECKING, Any, Callable, Optional, Union, no_type_check
 
 import subprocess_tee
 from packaging.version import Version
 
 from ansible_compat.config import (
     AnsibleConfig,
     ansible_collections_path,
+    ansible_version,
     parse_ansible_version,
 )
 from ansible_compat.constants import (
     MSG_INVALID_FQRL,
     RC_ANSIBLE_OPTIONS_ERROR,
     REQUIREMENT_LOCATIONS,
 )
@@ -69,24 +70,90 @@
         # As packaging Version class does not support wildcard, we convert it
         # to "0", as this being the smallest version possible.
         if version == "*":
             version = "0"
         super().__init__(version)
 
 
+@dataclass
+class Plugins:  # pylint: disable=too-many-instance-attributes
+    """Dataclass to access installed Ansible plugins, uses ansible-doc to retrieve them."""
+
+    runtime: "Runtime"
+    become: dict[str, str] = field(init=False)
+    cache: dict[str, str] = field(init=False)
+    callback: dict[str, str] = field(init=False)
+    cliconf: dict[str, str] = field(init=False)
+    connection: dict[str, str] = field(init=False)
+    httpapi: dict[str, str] = field(init=False)
+    inventory: dict[str, str] = field(init=False)
+    lookup: dict[str, str] = field(init=False)
+    netconf: dict[str, str] = field(init=False)
+    shell: dict[str, str] = field(init=False)
+    vars: dict[str, str] = field(init=False)  # noqa: A003
+    module: dict[str, str] = field(init=False)
+    strategy: dict[str, str] = field(init=False)
+    test: dict[str, str] = field(init=False)
+    filter: dict[str, str] = field(init=False)  # noqa: A003
+    role: dict[str, str] = field(init=False)
+    keyword: dict[str, str] = field(init=False)
+
+    @no_type_check
+    def __getattribute__(self, attr: str):  # noqa: ANN204
+        """Get attribute."""
+        if attr in {
+            "become",
+            "cache",
+            "callback",
+            "cliconf",
+            "connection",
+            "httpapi",
+            "inventory",
+            "lookup",
+            "netconf",
+            "shell",
+            "vars",
+            "module",
+            "strategy",
+            "test",
+            "filter",
+            "role",
+            "keyword",
+        }:
+            try:
+                result = super().__getattribute__(attr)
+            except AttributeError as exc:
+                if ansible_version() < Version("2.14") and attr in {"filter", "test"}:
+                    msg = "Ansible version below 2.14 does not support retrieving filter and test plugins."
+                    raise RuntimeError(msg) from exc
+                proc = self.runtime.run(
+                    ["ansible-doc", "--json", "-l", "-t", attr],
+                )
+                data = json.loads(proc.stdout)
+                if not isinstance(data, dict):  # pragma: no cover
+                    msg = "Unexpected output from ansible-doc"
+                    raise AnsibleCompatError(msg) from exc
+                result = data
+        else:
+            result = super().__getattribute__(attr)
+
+        return result
+
+
 # pylint: disable=too-many-instance-attributes
 class Runtime:
     """Ansible Runtime manager."""
 
     _version: Optional[Version] = None
     collections: OrderedDict[str, Collection] = OrderedDict()
     cache_dir: Optional[Path] = None
     # Used to track if we have already initialized the Ansible runtime as attempts
     # to do it multiple tilmes will cause runtime warnings from within ansible-core
     initialized: bool = False
+    plugins: Plugins
 
     def __init__(
         self,
         project_dir: Optional[Path] = None,
         *,
         isolated: bool = False,
         min_required_version: Optional[str] = None,
@@ -115,14 +182,15 @@
         :param environ: Environment dictionary to use, if undefined
                         ``os.environ`` will be copied and used.
         """
         self.project_dir = project_dir or Path.cwd()
         self.isolated = isolated
         self.max_retries = max_retries
         self.environ = environ or os.environ.copy()
+        self.plugins = Plugins(runtime=self)
         # Reduce noise from paramiko, unless user already defined PYTHONWARNINGS
         # paramiko/transport.py:236: CryptographyDeprecationWarning: Blowfish has been deprecated
         # https://github.com/paramiko/paramiko/issues/2038
         # As CryptographyDeprecationWarning is not a builtin, we cannot use
         # PYTHONWARNINGS to ignore it using category but we can use message.
         # https://stackoverflow.com/q/68251969/99834
         if "PYTHONWARNINGS" not in self.environ:  # pragma: no cover
@@ -160,17 +228,14 @@
         Display.warning = warning
 
     def load_collections(self) -> None:
         """Load collection data."""
         self.collections = OrderedDict()
         no_collections_msg = "None of the provided paths were usable"
 
-        # Workaround for https://github.com/ansible/ansible/issues/73127
-        Path("~/.ansible/collections").expanduser().mkdir(exist_ok=True, parents=True)
-
         proc = self.run(["ansible-galaxy", "collection", "list", "--format=json"])
         if proc.returncode == RC_ANSIBLE_OPTIONS_ERROR and (
             no_collections_msg in proc.stdout or no_collections_msg in proc.stderr
         ):
             _logger.debug("Ansible reported no installed collections at all.")
             return
         if proc.returncode != 0:
```

### Comparing `ansible-compat-4.0.5/src/ansible_compat/schema.py` & `ansible-compat-4.1.0/src/ansible_compat/schema.py`

 * *Files identical despite different names*

### Comparing `ansible-compat-4.0.5/src/ansible_compat/types.py` & `ansible-compat-4.1.0/src/ansible_compat/types.py`

 * *Files identical despite different names*

### Comparing `ansible-compat-4.0.5/src/ansible_compat.egg-info/PKG-INFO` & `ansible-compat-4.1.0/src/ansible_compat.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ansible-compat
-Version: 4.0.5
+Version: 4.1.0
 Summary: Ansible compatibility goodies
 Author-email: Sorin Sbarnea <ssbarnea@redhat.com>
 Maintainer-email: Sorin Sbarnea <ssbarnea@redhat.com>
 License: MIT
 Project-URL: homepage, https://github.com/ansible/ansible-compat
 Project-URL: documentation, https://ansible-compat.readthedocs.io/
 Project-URL: repository, https://github.com/ansible/ansible-compat
```

### Comparing `ansible-compat-4.0.5/src/ansible_compat.egg-info/SOURCES.txt` & `ansible-compat-4.1.0/src/ansible_compat.egg-info/SOURCES.txt`

 * *Files 0% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 .pre-commit-config.yaml
 .prettierignore
 .prettierrc.yaml
 .readthedocs.yml
 .yamllint
 LICENSE
 README.md
+ansible.cfg
 codecov.yml
 mkdocs.yml
 pyproject.toml
 readthedocs.yml
 requirements.txt
 tox.ini
 .github/CODEOWNERS
```

### Comparing `ansible-compat-4.0.5/test/assets/validate0_expected.json` & `ansible-compat-4.1.0/test/assets/validate0_expected.json`

 * *Files identical despite different names*

### Comparing `ansible-compat-4.0.5/test/collections/acme.goodies/galaxy.yml` & `ansible-compat-4.1.0/test/collections/acme.goodies/galaxy.yml`

 * *Files identical despite different names*

### Comparing `ansible-compat-4.0.5/test/conftest.py` & `ansible-compat-4.1.0/test/conftest.py`

 * *Files identical despite different names*

### Comparing `ansible-compat-4.0.5/test/test_config.py` & `ansible-compat-4.1.0/test/test_config.py`

 * *Files identical despite different names*

### Comparing `ansible-compat-4.0.5/test/test_runtime.py` & `ansible-compat-4.1.0/test/test_runtime.py`

 * *Files 4% similar despite different names*

```diff
@@ -11,14 +11,15 @@
 from typing import Any, Union
 
 import pytest
 from _pytest.monkeypatch import MonkeyPatch
 from packaging.version import Version
 from pytest_mock import MockerFixture
 
+from ansible_compat.config import ansible_version
 from ansible_compat.constants import INVALID_PREREQUISITES_RC
 from ansible_compat.errors import (
     AnsibleCommandError,
     AnsibleCompatError,
     InvalidPrerequisiteError,
 )
 from ansible_compat.runtime import CompletedProcess, Runtime
@@ -743,7 +744,48 @@
 
     result = runtime.run(["printenv", "FOO"], env={"FOO": "bar"})
     assert result.stdout.rstrip() == "bar"
 
     runtime.environ["FOO"] = "bar"
     result = runtime.run(["printenv", "FOO"])
     assert result.stdout.rstrip() == "bar"
+
+
+def test_runtime_plugins(runtime: Runtime) -> None:
+    """Tests ability to access detected plugins."""
+    assert len(runtime.plugins.cliconf) == 0
+    # ansible.netcommon.restconf might be in httpapi
+    assert isinstance(runtime.plugins.httpapi, dict)
+    # "ansible.netcommon.default" might be in runtime.plugins.netconf
+    assert isinstance(runtime.plugins.netconf, dict)
+    assert isinstance(runtime.plugins.role, dict)
+    assert "become" in runtime.plugins.keyword
+
+    if ansible_version() < Version("2.14.0"):
+        assert "sudo" in runtime.plugins.become
+        assert "memory" in runtime.plugins.cache
+        assert "default" in runtime.plugins.callback
+        assert "local" in runtime.plugins.connection
+        assert "ini" in runtime.plugins.inventory
+        assert "env" in runtime.plugins.lookup
+        assert "sh" in runtime.plugins.shell
+        assert "host_group_vars" in runtime.plugins.vars
+        assert "file" in runtime.plugins.module
+        assert "free" in runtime.plugins.strategy
+        # ansible-doc below 2.14 does not support listing 'test' and 'filter' types:
+        with pytest.raises(RuntimeError):
+            assert "is_abs" in runtime.plugins.test
+        with pytest.raises(RuntimeError):
+            assert "bool" in runtime.plugins.filter
+    else:
+        assert "ansible.builtin.sudo" in runtime.plugins.become
+        assert "ansible.builtin.memory" in runtime.plugins.cache
+        assert "ansible.builtin.default" in runtime.plugins.callback
+        assert "ansible.builtin.local" in runtime.plugins.connection
+        assert "ansible.builtin.ini" in runtime.plugins.inventory
+        assert "ansible.builtin.env" in runtime.plugins.lookup
+        assert "ansible.builtin.sh" in runtime.plugins.shell
+        assert "ansible.builtin.host_group_vars" in runtime.plugins.vars
+        assert "ansible.builtin.file" in runtime.plugins.module
+        assert "ansible.builtin.free" in runtime.plugins.strategy
+        assert "ansible.builtin.is_abs" in runtime.plugins.test
+        assert "ansible.builtin.bool" in runtime.plugins.filter
```

### Comparing `ansible-compat-4.0.5/test/test_runtime_example.py` & `ansible-compat-4.1.0/test/test_runtime_example.py`

 * *Files identical despite different names*

### Comparing `ansible-compat-4.0.5/test/test_schema.py` & `ansible-compat-4.1.0/test/test_schema.py`

 * *Files identical despite different names*

### Comparing `ansible-compat-4.0.5/tox.ini` & `ansible-compat-4.1.0/tox.ini`

 * *Files 3% similar despite different names*

```diff
@@ -4,15 +4,14 @@
   lint
   pkg
   docs
   # matrix assumed current (implicit) is 2.13:
   py{39,310,311}{,-devel,-ansible212,-ansible213,-ansible214,-ansible215}
 isolated_build = true
 skip_missing_interpreters = True
-skipsdist = true
 
 [testenv]
 description =
   Run the tests with {basepython}
   devel: ansible devel branch
   ansible212: ansible-core 2.12
   ansible213: ansible-core 2.13
@@ -24,15 +23,16 @@
   ansible213: ansible-core>=2.13,<2.14
   ansible214: ansible-core>=2.14,<2.15
   ansible215: ansible-core>=2.15,<2.16
 
   devel: ansible-core @ git+https://github.com/ansible/ansible.git  # GPLv3+
   # avoid installing ansible-core on -devel envs:
   !devel: ansible-core
-  --editable .[test]
+extras =
+  test
 
 commands =
   sh -c "ansible --version | head -n 1"
   # We add coverage options but not making them mandatory as we do not want to force
   # pytest users to run coverage when they just want to run a single test with `pytest -k test`
   coverage run -m pytest {posargs:}
   sh -c "coverage combine -a -q --data-file=.coverage {toxworkdir}/.coverage.*"
@@ -64,20 +64,22 @@
 setenv =
   ANSIBLE_DEVEL_WARNING='false'
   COVERAGE_FILE = {env:COVERAGE_FILE:{toxworkdir}/.coverage.{envname}}
   COVERAGE_PROCESS_START={toxinidir}/pyproject.toml
   PIP_DISABLE_PIP_VERSION_CHECK = 1
   PIP_CONSTRAINT = {toxinidir}/requirements.txt
   PRE_COMMIT_COLOR = always
-  PYTEST_REQPASS = 81
+  PYTEST_REQPASS = 82
   FORCE_COLOR = 1
 allowlist_externals =
   ansible
   git
   sh
+# https://tox.wiki/en/latest/upgrading.html#editable-mode
+package = editable
 
 [testenv:lint]
 description = Run all linters
 # locked basepython is needed because to keep constrains.txt predictable
 basepython = python3.9
 deps =
   pre-commit>=2.6.0
@@ -136,10 +138,9 @@
   {[testenv]deps}
   ansible-core>=2.12
 
 [testenv:docs]
 description = Build docs
 commands =
   mkdocs {posargs:build} --strict
-deps =
-  --editable .[docs]
+extras = docs
 passenv = *
```

