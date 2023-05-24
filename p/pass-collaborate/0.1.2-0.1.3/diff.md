# Comparing `tmp/pass-collaborate-0.1.2.tar.gz` & `tmp/pass-collaborate-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pass-collaborate-0.1.2.tar", last modified: Wed May 24 16:10:35 2023, max compression
+gzip compressed data, was "pass-collaborate-0.1.3.tar", last modified: Wed May 24 16:17:57 2023, max compression
```

## Comparing `pass-collaborate-0.1.2.tar` & `pass-collaborate-0.1.3.tar`

### file list

```diff
@@ -1,67 +1,67 @@
--rw-r--r--   0        0        0    35149 2022-11-28 10:47:21.404003 pass-collaborate-0.1.2/LICENSE
--rw-r--r--   0        0        0     1685 2023-05-24 15:57:02.065536 pass-collaborate-0.1.2/README.md
--rw-r--r--   0        0        0     7260 2023-05-24 16:10:28.369046 pass-collaborate-0.1.2/pyproject.toml
--rw-r--r--   0        0        0       84 2022-11-28 10:47:21.428003 pass-collaborate-0.1.2/src/pass_collaborate/__init__.py
--rw-r--r--   0        0        0     6150 2023-03-15 11:56:14.649915 pass-collaborate-0.1.2/src/pass_collaborate/adapters.py
--rwxr-xr-x   0        0        0       58 2023-03-15 11:56:14.645915 pass-collaborate-0.1.2/src/pass_collaborate/assets/access.bash
--rw-r--r--   0        0        0       25 2023-03-15 11:56:14.645915 pass-collaborate-0.1.2/src/pass_collaborate/assets/auth.yaml
--rwxr-xr-x   0        0        0       58 2023-03-15 11:56:14.645915 pass-collaborate-0.1.2/src/pass_collaborate/assets/group.bash
--rwxr-xr-x   0        0        0       56 2023-03-15 11:56:14.645915 pass-collaborate-0.1.2/src/pass_collaborate/assets/user.bash
--rw-r--r--   0        0        0     1151 2023-05-24 15:54:04.914319 pass-collaborate-0.1.2/src/pass_collaborate/entrypoints/__init__.py
--rw-r--r--   0        0        0     4358 2023-05-24 15:57:02.073536 pass-collaborate-0.1.2/src/pass_collaborate/entrypoints/cli.py
--rw-r--r--   0        0        0     4763 2023-05-24 15:54:04.922319 pass-collaborate-0.1.2/src/pass_collaborate/entrypoints/group.py
--rw-r--r--   0        0        0     1463 2023-05-24 15:54:04.918319 pass-collaborate-0.1.2/src/pass_collaborate/entrypoints/user.py
--rw-r--r--   0        0        0      411 2023-05-24 15:54:06.290344 pass-collaborate-0.1.2/src/pass_collaborate/exceptions.py
--rw-r--r--   0        0        0        0 2023-03-15 11:56:14.649915 pass-collaborate-0.1.2/src/pass_collaborate/model/__init__.py
--rw-r--r--   0        0        0    19782 2023-05-24 15:54:04.942319 pass-collaborate-0.1.2/src/pass_collaborate/model/auth.py
--rw-r--r--   0        0        0      175 2023-05-24 15:54:04.934319 pass-collaborate-0.1.2/src/pass_collaborate/model/key.py
--rw-r--r--   0        0        0    18390 2023-03-15 11:56:14.649915 pass-collaborate-0.1.2/src/pass_collaborate/model/pass_.py
--rw-r--r--   0        0        0        0 2022-11-28 10:47:21.424003 pass-collaborate-0.1.2/src/pass_collaborate/py.typed
--rw-r--r--   0        0        0      219 2023-02-01 16:38:07.222221 pass-collaborate-0.1.2/src/pass_collaborate/services.py
--rw-r--r--   0        0        0      650 2023-05-24 16:10:28.237053 pass-collaborate-0.1.2/src/pass_collaborate/version.py
--rw-r--r--   0        0        0     2511 2023-03-15 11:56:14.649915 pass-collaborate-0.1.2/src/pass_collaborate/views.py
--rw-r--r--   0        0        0        0 2022-11-28 10:47:21.436003 pass-collaborate-0.1.2/tests/__init__.py
--rw-r--r--   0        0        0     1604 2023-03-15 11:56:14.653915 pass-collaborate-0.1.2/tests/assets/gpg/admin/openpgp-revocs.d/5E435D54DDC11A0F303910AEDECE5B3C889F13DE.rev
--rw-r--r--   0        0        0     1426 2023-03-15 11:56:14.653915 pass-collaborate-0.1.2/tests/assets/gpg/admin/private-keys-v1.d/40861802C330F5AF0234DDEC19C25604FCF0F054.key
--rw-r--r--   0        0        0     1425 2023-03-15 11:56:14.653915 pass-collaborate-0.1.2/tests/assets/gpg/admin/private-keys-v1.d/6486C0B48C58C33A94A759D3C71E5BB2A46334BF.key
--rw-r--r--   0        0        0     6715 2023-03-15 11:56:14.653915 pass-collaborate-0.1.2/tests/assets/gpg/admin/pubring.kbx
--rw-r--r--   0        0        0      600 2023-03-15 11:56:14.653915 pass-collaborate-0.1.2/tests/assets/gpg/admin/random_seed
--rw-r--r--   0        0        0    49152 2023-03-15 11:56:14.653915 pass-collaborate-0.1.2/tests/assets/gpg/admin/tofu.db
--rw-r--r--   0        0        0     1400 2023-03-15 11:56:14.653915 pass-collaborate-0.1.2/tests/assets/gpg/admin/trustdb.gpg
--rw-r--r--   0        0        0     2428 2023-03-15 11:56:14.649915 pass-collaborate-0.1.2/tests/assets/gpg/admin.pub
--rw-r--r--   0        0        0     1610 2023-03-15 11:56:14.653915 pass-collaborate-0.1.2/tests/assets/gpg/attacker/openpgp-revocs.d/C810FD864F7BAED8AD1D233C6E3A5366E18CBE77.rev
--rw-r--r--   0        0        0     1425 2023-03-15 11:56:14.653915 pass-collaborate-0.1.2/tests/assets/gpg/attacker/private-keys-v1.d/41083288E21D89088C2D006CEF671B784ECF5138.key
--rw-r--r--   0        0        0     1425 2023-03-15 11:56:14.653915 pass-collaborate-0.1.2/tests/assets/gpg/attacker/private-keys-v1.d/57893AE2099ADF0FFD3DD349236793A55F92B321.key
--rw-r--r--   0        0        0     1961 2023-03-15 11:56:14.653915 pass-collaborate-0.1.2/tests/assets/gpg/attacker/pubring.kbx
--rw-r--r--   0        0        0     1280 2023-03-15 11:56:14.653915 pass-collaborate-0.1.2/tests/assets/gpg/attacker/trustdb.gpg
--rw-r--r--   0        0        0     2436 2023-03-15 11:56:14.653915 pass-collaborate-0.1.2/tests/assets/gpg/attacker.pub
--rw-r--r--   0        0        0     1612 2023-03-15 11:56:14.657915 pass-collaborate-0.1.2/tests/assets/gpg/developer/openpgp-revocs.d/8DFE8782CD025ED6220D305115575911602DDD94.rev
--rw-r--r--   0        0        0     1426 2023-03-15 11:56:14.657915 pass-collaborate-0.1.2/tests/assets/gpg/developer/private-keys-v1.d/E316C952CE5A90CF5CB2AB91B9FE64DCD585F363.key
--rw-r--r--   0        0        0     1425 2023-03-15 11:56:14.657915 pass-collaborate-0.1.2/tests/assets/gpg/developer/private-keys-v1.d/E5E7DB1CAF2638BF2CED3CE2B310551D08DC1CFF.key
--rw-r--r--   0        0        0     1963 2023-03-15 11:56:14.657915 pass-collaborate-0.1.2/tests/assets/gpg/developer/pubring.kbx
--rw-r--r--   0        0        0      600 2023-03-15 11:56:14.657915 pass-collaborate-0.1.2/tests/assets/gpg/developer/random_seed
--rw-r--r--   0        0        0     1280 2023-03-15 11:56:14.657915 pass-collaborate-0.1.2/tests/assets/gpg/developer/trustdb.gpg
--rw-r--r--   0        0        0     2440 2023-03-15 11:56:14.657915 pass-collaborate-0.1.2/tests/assets/gpg/developer.pub
--rw-r--r--   0        0        0       25 2023-03-15 11:56:14.657915 pass-collaborate-0.1.2/tests/assets/pass/.auth.yaml
--rw-r--r--   0        0        0       41 2023-03-15 11:56:14.657915 pass-collaborate-0.1.2/tests/assets/pass/.gpg-id
--rw-r--r--   0        0        0      476 2023-03-15 11:56:14.657915 pass-collaborate-0.1.2/tests/assets/pass/bastion.gpg
--rw-r--r--   0        0        0      476 2023-03-15 11:56:14.657915 pass-collaborate-0.1.2/tests/assets/pass/database/production.gpg
--rw-r--r--   0        0        0      476 2023-03-15 11:56:14.657915 pass-collaborate-0.1.2/tests/assets/pass/database/staging.gpg
--rw-r--r--   0        0        0      476 2023-03-15 11:56:14.657915 pass-collaborate-0.1.2/tests/assets/pass/web/production.gpg
--rw-r--r--   0        0        0      476 2023-03-15 11:56:14.657915 pass-collaborate-0.1.2/tests/assets/pass/web/staging.gpg
--rw-r--r--   0        0        0     2875 2023-05-24 15:57:02.073536 pass-collaborate-0.1.2/tests/conftest.py
--rw-r--r--   0        0        0        0 2022-11-28 10:47:21.440003 pass-collaborate-0.1.2/tests/e2e/__init__.py
--rw-r--r--   0        0        0      429 2023-03-15 11:56:14.657915 pass-collaborate-0.1.2/tests/e2e/conftest.py
--rw-r--r--   0        0        0     3734 2023-03-15 11:56:14.661915 pass-collaborate-0.1.2/tests/e2e/test_access.py
--rw-r--r--   0        0        0     3539 2023-04-04 10:59:40.612231 pass-collaborate-0.1.2/tests/e2e/test_cli.py
--rw-r--r--   0        0        0    15522 2023-03-15 11:56:14.661915 pass-collaborate-0.1.2/tests/e2e/test_group.py
--rw-r--r--   0        0        0     3824 2023-03-15 11:56:14.661915 pass-collaborate-0.1.2/tests/e2e/test_user.py
--rw-r--r--   0        0        0      381 2023-03-15 11:56:14.661915 pass-collaborate-0.1.2/tests/factories.py
--rw-r--r--   0        0        0        0 2022-11-28 10:47:21.444003 pass-collaborate-0.1.2/tests/integration/__init__.py
--rw-r--r--   0        0        0        0 2022-11-28 10:47:21.440003 pass-collaborate-0.1.2/tests/unit/__init__.py
--rw-r--r--   0        0        0        0 2023-03-15 11:56:14.661915 pass-collaborate-0.1.2/tests/unit/adapters/__init__.py
--rw-r--r--   0        0        0     5280 2023-03-15 11:56:14.661915 pass-collaborate-0.1.2/tests/unit/adapters/test_authstore.py
--rw-r--r--   0        0        0     3865 2023-05-24 15:57:02.077536 pass-collaborate-0.1.2/tests/unit/adapters/test_keystore.py
--rw-r--r--   0        0        0     4040 2023-03-15 11:56:14.661915 pass-collaborate-0.1.2/tests/unit/adapters/test_passstore.py
--rw-r--r--   0        0        0      422 2023-02-13 13:00:27.977468 pass-collaborate-0.1.2/tests/unit/test_version.py
--rw-r--r--   0        0        0     2798 1970-01-01 00:00:00.000000 pass-collaborate-0.1.2/PKG-INFO
+-rw-r--r--   0        0        0    35149 2022-11-28 10:47:21.404003 pass-collaborate-0.1.3/LICENSE
+-rw-r--r--   0        0        0     1685 2023-05-24 15:57:02.065536 pass-collaborate-0.1.3/README.md
+-rw-r--r--   0        0        0     7260 2023-05-24 16:17:50.837488 pass-collaborate-0.1.3/pyproject.toml
+-rw-r--r--   0        0        0       84 2022-11-28 10:47:21.428003 pass-collaborate-0.1.3/src/pass_collaborate/__init__.py
+-rw-r--r--   0        0        0     6150 2023-03-15 11:56:14.649915 pass-collaborate-0.1.3/src/pass_collaborate/adapters.py
+-rwxr-xr-x   0        0        0       58 2023-03-15 11:56:14.645915 pass-collaborate-0.1.3/src/pass_collaborate/assets/access.bash
+-rw-r--r--   0        0        0       25 2023-03-15 11:56:14.645915 pass-collaborate-0.1.3/src/pass_collaborate/assets/auth.yaml
+-rwxr-xr-x   0        0        0       58 2023-03-15 11:56:14.645915 pass-collaborate-0.1.3/src/pass_collaborate/assets/group.bash
+-rwxr-xr-x   0        0        0       56 2023-03-15 11:56:14.645915 pass-collaborate-0.1.3/src/pass_collaborate/assets/user.bash
+-rw-r--r--   0        0        0     1151 2023-05-24 15:54:04.914319 pass-collaborate-0.1.3/src/pass_collaborate/entrypoints/__init__.py
+-rw-r--r--   0        0        0     4457 2023-05-24 16:17:21.030141 pass-collaborate-0.1.3/src/pass_collaborate/entrypoints/cli.py
+-rw-r--r--   0        0        0     4763 2023-05-24 15:54:04.922319 pass-collaborate-0.1.3/src/pass_collaborate/entrypoints/group.py
+-rw-r--r--   0        0        0     1463 2023-05-24 15:54:04.918319 pass-collaborate-0.1.3/src/pass_collaborate/entrypoints/user.py
+-rw-r--r--   0        0        0      411 2023-05-24 15:54:06.290344 pass-collaborate-0.1.3/src/pass_collaborate/exceptions.py
+-rw-r--r--   0        0        0        0 2023-03-15 11:56:14.649915 pass-collaborate-0.1.3/src/pass_collaborate/model/__init__.py
+-rw-r--r--   0        0        0    19782 2023-05-24 15:54:04.942319 pass-collaborate-0.1.3/src/pass_collaborate/model/auth.py
+-rw-r--r--   0        0        0      175 2023-05-24 15:54:04.934319 pass-collaborate-0.1.3/src/pass_collaborate/model/key.py
+-rw-r--r--   0        0        0    18390 2023-03-15 11:56:14.649915 pass-collaborate-0.1.3/src/pass_collaborate/model/pass_.py
+-rw-r--r--   0        0        0        0 2022-11-28 10:47:21.424003 pass-collaborate-0.1.3/src/pass_collaborate/py.typed
+-rw-r--r--   0        0        0      219 2023-02-01 16:38:07.222221 pass-collaborate-0.1.3/src/pass_collaborate/services.py
+-rw-r--r--   0        0        0      650 2023-05-24 16:17:50.677491 pass-collaborate-0.1.3/src/pass_collaborate/version.py
+-rw-r--r--   0        0        0     2511 2023-03-15 11:56:14.649915 pass-collaborate-0.1.3/src/pass_collaborate/views.py
+-rw-r--r--   0        0        0        0 2022-11-28 10:47:21.436003 pass-collaborate-0.1.3/tests/__init__.py
+-rw-r--r--   0        0        0     1604 2023-03-15 11:56:14.653915 pass-collaborate-0.1.3/tests/assets/gpg/admin/openpgp-revocs.d/5E435D54DDC11A0F303910AEDECE5B3C889F13DE.rev
+-rw-r--r--   0        0        0     1426 2023-03-15 11:56:14.653915 pass-collaborate-0.1.3/tests/assets/gpg/admin/private-keys-v1.d/40861802C330F5AF0234DDEC19C25604FCF0F054.key
+-rw-r--r--   0        0        0     1425 2023-03-15 11:56:14.653915 pass-collaborate-0.1.3/tests/assets/gpg/admin/private-keys-v1.d/6486C0B48C58C33A94A759D3C71E5BB2A46334BF.key
+-rw-r--r--   0        0        0     6715 2023-03-15 11:56:14.653915 pass-collaborate-0.1.3/tests/assets/gpg/admin/pubring.kbx
+-rw-r--r--   0        0        0      600 2023-03-15 11:56:14.653915 pass-collaborate-0.1.3/tests/assets/gpg/admin/random_seed
+-rw-r--r--   0        0        0    49152 2023-03-15 11:56:14.653915 pass-collaborate-0.1.3/tests/assets/gpg/admin/tofu.db
+-rw-r--r--   0        0        0     1400 2023-03-15 11:56:14.653915 pass-collaborate-0.1.3/tests/assets/gpg/admin/trustdb.gpg
+-rw-r--r--   0        0        0     2428 2023-03-15 11:56:14.649915 pass-collaborate-0.1.3/tests/assets/gpg/admin.pub
+-rw-r--r--   0        0        0     1610 2023-03-15 11:56:14.653915 pass-collaborate-0.1.3/tests/assets/gpg/attacker/openpgp-revocs.d/C810FD864F7BAED8AD1D233C6E3A5366E18CBE77.rev
+-rw-r--r--   0        0        0     1425 2023-03-15 11:56:14.653915 pass-collaborate-0.1.3/tests/assets/gpg/attacker/private-keys-v1.d/41083288E21D89088C2D006CEF671B784ECF5138.key
+-rw-r--r--   0        0        0     1425 2023-03-15 11:56:14.653915 pass-collaborate-0.1.3/tests/assets/gpg/attacker/private-keys-v1.d/57893AE2099ADF0FFD3DD349236793A55F92B321.key
+-rw-r--r--   0        0        0     1961 2023-03-15 11:56:14.653915 pass-collaborate-0.1.3/tests/assets/gpg/attacker/pubring.kbx
+-rw-r--r--   0        0        0     1280 2023-03-15 11:56:14.653915 pass-collaborate-0.1.3/tests/assets/gpg/attacker/trustdb.gpg
+-rw-r--r--   0        0        0     2436 2023-03-15 11:56:14.653915 pass-collaborate-0.1.3/tests/assets/gpg/attacker.pub
+-rw-r--r--   0        0        0     1612 2023-03-15 11:56:14.657915 pass-collaborate-0.1.3/tests/assets/gpg/developer/openpgp-revocs.d/8DFE8782CD025ED6220D305115575911602DDD94.rev
+-rw-r--r--   0        0        0     1426 2023-03-15 11:56:14.657915 pass-collaborate-0.1.3/tests/assets/gpg/developer/private-keys-v1.d/E316C952CE5A90CF5CB2AB91B9FE64DCD585F363.key
+-rw-r--r--   0        0        0     1425 2023-03-15 11:56:14.657915 pass-collaborate-0.1.3/tests/assets/gpg/developer/private-keys-v1.d/E5E7DB1CAF2638BF2CED3CE2B310551D08DC1CFF.key
+-rw-r--r--   0        0        0     1963 2023-03-15 11:56:14.657915 pass-collaborate-0.1.3/tests/assets/gpg/developer/pubring.kbx
+-rw-r--r--   0        0        0      600 2023-03-15 11:56:14.657915 pass-collaborate-0.1.3/tests/assets/gpg/developer/random_seed
+-rw-r--r--   0        0        0     1280 2023-03-15 11:56:14.657915 pass-collaborate-0.1.3/tests/assets/gpg/developer/trustdb.gpg
+-rw-r--r--   0        0        0     2440 2023-03-15 11:56:14.657915 pass-collaborate-0.1.3/tests/assets/gpg/developer.pub
+-rw-r--r--   0        0        0       25 2023-03-15 11:56:14.657915 pass-collaborate-0.1.3/tests/assets/pass/.auth.yaml
+-rw-r--r--   0        0        0       41 2023-03-15 11:56:14.657915 pass-collaborate-0.1.3/tests/assets/pass/.gpg-id
+-rw-r--r--   0        0        0      476 2023-03-15 11:56:14.657915 pass-collaborate-0.1.3/tests/assets/pass/bastion.gpg
+-rw-r--r--   0        0        0      476 2023-03-15 11:56:14.657915 pass-collaborate-0.1.3/tests/assets/pass/database/production.gpg
+-rw-r--r--   0        0        0      476 2023-03-15 11:56:14.657915 pass-collaborate-0.1.3/tests/assets/pass/database/staging.gpg
+-rw-r--r--   0        0        0      476 2023-03-15 11:56:14.657915 pass-collaborate-0.1.3/tests/assets/pass/web/production.gpg
+-rw-r--r--   0        0        0      476 2023-03-15 11:56:14.657915 pass-collaborate-0.1.3/tests/assets/pass/web/staging.gpg
+-rw-r--r--   0        0        0     2875 2023-05-24 15:57:02.073536 pass-collaborate-0.1.3/tests/conftest.py
+-rw-r--r--   0        0        0        0 2022-11-28 10:47:21.440003 pass-collaborate-0.1.3/tests/e2e/__init__.py
+-rw-r--r--   0        0        0      429 2023-03-15 11:56:14.657915 pass-collaborate-0.1.3/tests/e2e/conftest.py
+-rw-r--r--   0        0        0     3734 2023-03-15 11:56:14.661915 pass-collaborate-0.1.3/tests/e2e/test_access.py
+-rw-r--r--   0        0        0     3539 2023-04-04 10:59:40.612231 pass-collaborate-0.1.3/tests/e2e/test_cli.py
+-rw-r--r--   0        0        0    15522 2023-03-15 11:56:14.661915 pass-collaborate-0.1.3/tests/e2e/test_group.py
+-rw-r--r--   0        0        0     3824 2023-03-15 11:56:14.661915 pass-collaborate-0.1.3/tests/e2e/test_user.py
+-rw-r--r--   0        0        0      381 2023-03-15 11:56:14.661915 pass-collaborate-0.1.3/tests/factories.py
+-rw-r--r--   0        0        0        0 2022-11-28 10:47:21.444003 pass-collaborate-0.1.3/tests/integration/__init__.py
+-rw-r--r--   0        0        0        0 2022-11-28 10:47:21.440003 pass-collaborate-0.1.3/tests/unit/__init__.py
+-rw-r--r--   0        0        0        0 2023-03-15 11:56:14.661915 pass-collaborate-0.1.3/tests/unit/adapters/__init__.py
+-rw-r--r--   0        0        0     5280 2023-03-15 11:56:14.661915 pass-collaborate-0.1.3/tests/unit/adapters/test_authstore.py
+-rw-r--r--   0        0        0     3865 2023-05-24 15:57:02.077536 pass-collaborate-0.1.3/tests/unit/adapters/test_keystore.py
+-rw-r--r--   0        0        0     4040 2023-03-15 11:56:14.661915 pass-collaborate-0.1.3/tests/unit/adapters/test_passstore.py
+-rw-r--r--   0        0        0      422 2023-02-13 13:00:27.977468 pass-collaborate-0.1.3/tests/unit/test_version.py
+-rw-r--r--   0        0        0     2798 1970-01-01 00:00:00.000000 pass-collaborate-0.1.3/PKG-INFO
```

### Comparing `pass-collaborate-0.1.2/LICENSE` & `pass-collaborate-0.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `pass-collaborate-0.1.2/README.md` & `pass-collaborate-0.1.3/README.md`

 * *Files identical despite different names*

### Comparing `pass-collaborate-0.1.2/pyproject.toml` & `pass-collaborate-0.1.3/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.commitizen]
 name = "cz_conventional_commits"
-version = "0.1.2"
+version = "0.1.3"
 tag_format = "$version"
 version_files = [
     "pyproject.toml:version",
     "src/pass_collaborate/version.py",
 ]
 
 [tool.autoimport.common_statements]
@@ -346,15 +346,15 @@
     "Programming Language :: Python :: 3.7",
     "Programming Language :: Python :: 3.8",
     "Programming Language :: Python :: 3.9",
     "Programming Language :: Python :: 3.10",
     "Topic :: Utilities",
     "Natural Language :: English",
 ]
-version = "0.1.2"
+version = "0.1.3"
 
 [project.license]
 text = "GPL-3.0-only"
 
 [project.urls]
 Issues = "https://github.com/lyz-code/pass-collaborate/issues"
 homepage = "https://github.com/lyz-code/pass-collaborate"
```

### Comparing `pass-collaborate-0.1.2/src/pass_collaborate/adapters.py` & `pass-collaborate-0.1.3/src/pass_collaborate/adapters.py`

 * *Files identical despite different names*

### Comparing `pass-collaborate-0.1.2/src/pass_collaborate/entrypoints/__init__.py` & `pass-collaborate-0.1.3/src/pass_collaborate/entrypoints/__init__.py`

 * *Files identical despite different names*

### Comparing `pass-collaborate-0.1.2/src/pass_collaborate/entrypoints/cli.py` & `pass-collaborate-0.1.3/src/pass_collaborate/entrypoints/cli.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 """Command line interface definition."""
 
 import logging
 import os
+import sys
 import shutil
 from pathlib import Path
 from typing import Optional
 
 import typer
 from pydantic import ValidationError
 from rich.console import Console
@@ -113,16 +114,17 @@
         lib = Path(os.environ["PASSWORD_STORE_EXTENSIONS_DIR"])
     else:
         lib = Path.home() / ".password-store" / ".extensions"
     log.debug(f"Creating the {lib} directory")
     os.makedirs(lib, exist_ok=True)
 
     log.debug("Copying the plugin files")
+    package_directory = sys.modules['pass_collaborate'].__path__[0]
     for filename in ["user.bash", "group.bash", "access.bash"]:
-        shutil.copyfile(f"assets/{filename}", lib / filename)
+        shutil.copyfile(f"{package_directory}/assets/{filename}", lib / filename)
         # nosec: We need the files to be executable
         os.chmod(lib / filename, 0o755)  # nosec
 
     # Enable the extensions
     for filename in [".bashrc", ".zshrc"]:
         config = Path.home() / filename
         if (
```

### Comparing `pass-collaborate-0.1.2/src/pass_collaborate/entrypoints/group.py` & `pass-collaborate-0.1.3/src/pass_collaborate/entrypoints/group.py`

 * *Files identical despite different names*

### Comparing `pass-collaborate-0.1.2/src/pass_collaborate/entrypoints/user.py` & `pass-collaborate-0.1.3/src/pass_collaborate/entrypoints/user.py`

 * *Files identical despite different names*

### Comparing `pass-collaborate-0.1.2/src/pass_collaborate/model/auth.py` & `pass-collaborate-0.1.3/src/pass_collaborate/model/auth.py`

 * *Files identical despite different names*

### Comparing `pass-collaborate-0.1.2/src/pass_collaborate/model/pass_.py` & `pass-collaborate-0.1.3/src/pass_collaborate/model/pass_.py`

 * *Files identical despite different names*

### Comparing `pass-collaborate-0.1.2/src/pass_collaborate/version.py` & `pass-collaborate-0.1.3/src/pass_collaborate/version.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 import platform
 import sys
 from textwrap import dedent
 
 # Do not edit the version manually, let `make bump` do it.
 
-__version__ = "0.1.2"
+__version__ = "0.1.3"
 
 
 def version_info() -> str:
     """Display the version of the program, python and the platform."""
     return dedent(
         f"""\
         ------------------------------------------------------------------
```

### Comparing `pass-collaborate-0.1.2/src/pass_collaborate/views.py` & `pass-collaborate-0.1.3/src/pass_collaborate/views.py`

 * *Files identical despite different names*

### Comparing `pass-collaborate-0.1.2/tests/assets/gpg/admin/openpgp-revocs.d/5E435D54DDC11A0F303910AEDECE5B3C889F13DE.rev` & `pass-collaborate-0.1.3/tests/assets/gpg/admin/openpgp-revocs.d/5E435D54DDC11A0F303910AEDECE5B3C889F13DE.rev`

 * *Files identical despite different names*

### Comparing `pass-collaborate-0.1.2/tests/assets/gpg/admin/private-keys-v1.d/40861802C330F5AF0234DDEC19C25604FCF0F054.key` & `pass-collaborate-0.1.3/tests/assets/gpg/admin/private-keys-v1.d/40861802C330F5AF0234DDEC19C25604FCF0F054.key`

 * *Files identical despite different names*

### Comparing `pass-collaborate-0.1.2/tests/assets/gpg/admin/private-keys-v1.d/6486C0B48C58C33A94A759D3C71E5BB2A46334BF.key` & `pass-collaborate-0.1.3/tests/assets/gpg/admin/private-keys-v1.d/6486C0B48C58C33A94A759D3C71E5BB2A46334BF.key`

 * *Files identical despite different names*

### Comparing `pass-collaborate-0.1.2/tests/assets/gpg/admin/pubring.kbx` & `pass-collaborate-0.1.3/tests/assets/gpg/admin/pubring.kbx`

 * *Files identical despite different names*

### Comparing `pass-collaborate-0.1.2/tests/assets/gpg/admin/random_seed` & `pass-collaborate-0.1.3/tests/assets/gpg/admin/random_seed`

 * *Files identical despite different names*

### Comparing `pass-collaborate-0.1.2/tests/assets/gpg/admin/tofu.db` & `pass-collaborate-0.1.3/tests/assets/gpg/admin/tofu.db`

 * *Files identical despite different names*

### Comparing `pass-collaborate-0.1.2/tests/assets/gpg/admin/trustdb.gpg` & `pass-collaborate-0.1.3/tests/assets/gpg/admin/trustdb.gpg`

 * *Files identical despite different names*

### Comparing `pass-collaborate-0.1.2/tests/assets/gpg/admin.pub` & `pass-collaborate-0.1.3/tests/assets/gpg/admin.pub`

 * *Files identical despite different names*

### Comparing `pass-collaborate-0.1.2/tests/assets/gpg/attacker/openpgp-revocs.d/C810FD864F7BAED8AD1D233C6E3A5366E18CBE77.rev` & `pass-collaborate-0.1.3/tests/assets/gpg/attacker/openpgp-revocs.d/C810FD864F7BAED8AD1D233C6E3A5366E18CBE77.rev`

 * *Files identical despite different names*

### Comparing `pass-collaborate-0.1.2/tests/assets/gpg/attacker/private-keys-v1.d/41083288E21D89088C2D006CEF671B784ECF5138.key` & `pass-collaborate-0.1.3/tests/assets/gpg/attacker/private-keys-v1.d/41083288E21D89088C2D006CEF671B784ECF5138.key`

 * *Files identical despite different names*

### Comparing `pass-collaborate-0.1.2/tests/assets/gpg/attacker/private-keys-v1.d/57893AE2099ADF0FFD3DD349236793A55F92B321.key` & `pass-collaborate-0.1.3/tests/assets/gpg/attacker/private-keys-v1.d/57893AE2099ADF0FFD3DD349236793A55F92B321.key`

 * *Files identical despite different names*

### Comparing `pass-collaborate-0.1.2/tests/assets/gpg/attacker/pubring.kbx` & `pass-collaborate-0.1.3/tests/assets/gpg/attacker/pubring.kbx`

 * *Files identical despite different names*

### Comparing `pass-collaborate-0.1.2/tests/assets/gpg/attacker/trustdb.gpg` & `pass-collaborate-0.1.3/tests/assets/gpg/attacker/trustdb.gpg`

 * *Files identical despite different names*

### Comparing `pass-collaborate-0.1.2/tests/assets/gpg/attacker.pub` & `pass-collaborate-0.1.3/tests/assets/gpg/attacker.pub`

 * *Files identical despite different names*

### Comparing `pass-collaborate-0.1.2/tests/assets/gpg/developer/openpgp-revocs.d/8DFE8782CD025ED6220D305115575911602DDD94.rev` & `pass-collaborate-0.1.3/tests/assets/gpg/developer/openpgp-revocs.d/8DFE8782CD025ED6220D305115575911602DDD94.rev`

 * *Files identical despite different names*

### Comparing `pass-collaborate-0.1.2/tests/assets/gpg/developer/private-keys-v1.d/E316C952CE5A90CF5CB2AB91B9FE64DCD585F363.key` & `pass-collaborate-0.1.3/tests/assets/gpg/developer/private-keys-v1.d/E316C952CE5A90CF5CB2AB91B9FE64DCD585F363.key`

 * *Files identical despite different names*

### Comparing `pass-collaborate-0.1.2/tests/assets/gpg/developer/private-keys-v1.d/E5E7DB1CAF2638BF2CED3CE2B310551D08DC1CFF.key` & `pass-collaborate-0.1.3/tests/assets/gpg/developer/private-keys-v1.d/E5E7DB1CAF2638BF2CED3CE2B310551D08DC1CFF.key`

 * *Files identical despite different names*

### Comparing `pass-collaborate-0.1.2/tests/assets/gpg/developer/pubring.kbx` & `pass-collaborate-0.1.3/tests/assets/gpg/developer/pubring.kbx`

 * *Files identical despite different names*

### Comparing `pass-collaborate-0.1.2/tests/assets/gpg/developer/random_seed` & `pass-collaborate-0.1.3/tests/assets/gpg/developer/random_seed`

 * *Files identical despite different names*

### Comparing `pass-collaborate-0.1.2/tests/assets/gpg/developer/trustdb.gpg` & `pass-collaborate-0.1.3/tests/assets/gpg/developer/trustdb.gpg`

 * *Files identical despite different names*

### Comparing `pass-collaborate-0.1.2/tests/assets/gpg/developer.pub` & `pass-collaborate-0.1.3/tests/assets/gpg/developer.pub`

 * *Files identical despite different names*

### Comparing `pass-collaborate-0.1.2/tests/conftest.py` & `pass-collaborate-0.1.3/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `pass-collaborate-0.1.2/tests/e2e/test_access.py` & `pass-collaborate-0.1.3/tests/e2e/test_access.py`

 * *Files identical despite different names*

### Comparing `pass-collaborate-0.1.2/tests/e2e/test_cli.py` & `pass-collaborate-0.1.3/tests/e2e/test_cli.py`

 * *Files identical despite different names*

### Comparing `pass-collaborate-0.1.2/tests/e2e/test_group.py` & `pass-collaborate-0.1.3/tests/e2e/test_group.py`

 * *Files identical despite different names*

### Comparing `pass-collaborate-0.1.2/tests/e2e/test_user.py` & `pass-collaborate-0.1.3/tests/e2e/test_user.py`

 * *Files identical despite different names*

### Comparing `pass-collaborate-0.1.2/tests/unit/adapters/test_authstore.py` & `pass-collaborate-0.1.3/tests/unit/adapters/test_authstore.py`

 * *Files identical despite different names*

### Comparing `pass-collaborate-0.1.2/tests/unit/adapters/test_keystore.py` & `pass-collaborate-0.1.3/tests/unit/adapters/test_keystore.py`

 * *Files identical despite different names*

### Comparing `pass-collaborate-0.1.2/tests/unit/adapters/test_passstore.py` & `pass-collaborate-0.1.3/tests/unit/adapters/test_passstore.py`

 * *Files identical despite different names*

### Comparing `pass-collaborate-0.1.2/PKG-INFO` & `pass-collaborate-0.1.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pass-collaborate
-Version: 0.1.2
+Version: 0.1.3
 Summary: A pass extension that helps collectives manage the access to their passwords
 License: GPL-3.0-only
 Author-email: Lyz <lyz-code-security-advisories@riseup.net>
 Requires-Python: >=3.9
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: pass-collaborate Version: 0.1.2 Summary: A pass
+Metadata-Version: 2.1 Name: pass-collaborate Version: 0.1.3 Summary: A pass
 extension that helps collectives manage the access to their passwords License:
 GPL-3.0-only Author-email: Lyz
 riseup.net> Requires-Python: >=3.9 Classifier: Development Status :: 2 - Pre-
 Alpha Classifier: Intended Audience :: Developers Classifier: License :: OSI
 Approved :: GNU General Public License v3 (GPLv3) Classifier: Natural Language
 :: English Classifier: Operating System :: POSIX Classifier: Operating System
 :: Unix Classifier: Programming Language :: Python Classifier: Programming
```

