# Comparing `tmp/pypgstac-0.7.6.tar.gz` & `tmp/pypgstac-0.7.7.tar.gz`

## Comparing `pypgstac-0.7.6.tar` & `pypgstac-0.7.7.tar`

### file list

```diff
@@ -1,100 +1,102 @@
--rw-r--r--   0        0        0      868 2020-02-02 00:00:00.000000 pypgstac-0.7.6/setup.py
--rw-r--r--   0        0        0       92 2020-02-02 00:00:00.000000 pypgstac-0.7.6/pypgstac/__init__.py
--rw-r--r--   0        0        0     8950 2020-02-02 00:00:00.000000 pypgstac-0.7.6/pypgstac/db.py
--rw-r--r--   0        0        0     5520 2020-02-02 00:00:00.000000 pypgstac-0.7.6/pypgstac/hydration.py
--rw-r--r--   0        0        0    25760 2020-02-02 00:00:00.000000 pypgstac-0.7.6/pypgstac/load.py
--rw-r--r--   0        0        0     5244 2020-02-02 00:00:00.000000 pypgstac-0.7.6/pypgstac/migrate.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pypgstac-0.7.6/pypgstac/py.typed
--rwxr-xr-x   0        0        0     3443 2020-02-02 00:00:00.000000 pypgstac-0.7.6/pypgstac/pypgstac.py
--rw-r--r--   0        0        0       37 2020-02-02 00:00:00.000000 pypgstac-0.7.6/pypgstac/version.py
--rw-r--r--   0        0        0       86 2020-02-02 00:00:00.000000 pypgstac-0.7.6/pypgstac/migrations/pgstac.0.1.9-0.2.3.sql
--rw-r--r--   0        0        0    35445 2020-02-02 00:00:00.000000 pypgstac-0.7.6/pypgstac/migrations/pgstac.0.1.9.sql
--rw-r--r--   0        0        0       86 2020-02-02 00:00:00.000000 pypgstac-0.7.6/pypgstac/migrations/pgstac.0.2.3-0.2.4.sql
--rw-r--r--   0        0        0    35445 2020-02-02 00:00:00.000000 pypgstac-0.7.6/pypgstac/migrations/pgstac.0.2.3.sql
--rw-r--r--   0        0        0     7132 2020-02-02 00:00:00.000000 pypgstac-0.7.6/pypgstac/migrations/pgstac.0.2.4-0.2.5.sql
--rw-r--r--   0        0        0     8816 2020-02-02 00:00:00.000000 pypgstac-0.7.6/pypgstac/migrations/pgstac.0.2.4-0.2.7.sql
--rw-r--r--   0        0        0    35445 2020-02-02 00:00:00.000000 pypgstac-0.7.6/pypgstac/migrations/pgstac.0.2.4.sql
--rw-r--r--   0        0        0     1783 2020-02-02 00:00:00.000000 pypgstac-0.7.6/pypgstac/migrations/pgstac.0.2.5-0.2.7.sql
--rw-r--r--   0        0        0    35570 2020-02-02 00:00:00.000000 pypgstac-0.7.6/pypgstac/migrations/pgstac.0.2.5.sql
--rw-r--r--   0        0        0      103 2020-02-02 00:00:00.000000 pypgstac-0.7.6/pypgstac/migrations/pgstac.0.2.7-0.2.8.sql
--rw-r--r--   0        0        0    35570 2020-02-02 00:00:00.000000 pypgstac-0.7.6/pypgstac/migrations/pgstac.0.2.7.sql
--rw-r--r--   0        0        0       86 2020-02-02 00:00:00.000000 pypgstac-0.7.6/pypgstac/migrations/pgstac.0.2.8-0.2.9.sql
--rw-r--r--   0        0        0    30676 2020-02-02 00:00:00.000000 pypgstac-0.7.6/pypgstac/migrations/pgstac.0.2.8.sql
--rw-r--r--   0        0        0    48852 2020-02-02 00:00:00.000000 pypgstac-0.7.6/pypgstac/migrations/pgstac.0.2.9-0.3.0.sql
--rw-r--r--   0        0        0    30676 2020-02-02 00:00:00.000000 pypgstac-0.7.6/pypgstac/migrations/pgstac.0.2.9.sql
--rw-r--r--   0        0        0      732 2020-02-02 00:00:00.000000 pypgstac-0.7.6/pypgstac/migrations/pgstac.0.3.0-0.3.1.sql
--rw-r--r--   0        0        0    48316 2020-02-02 00:00:00.000000 pypgstac-0.7.6/pypgstac/migrations/pgstac.0.3.0.sql
--rw-r--r--   0        0        0     1692 2020-02-02 00:00:00.000000 pypgstac-0.7.6/pypgstac/migrations/pgstac.0.3.1-0.3.2.sql
--rw-r--r--   0        0        0    48318 2020-02-02 00:00:00.000000 pypgstac-0.7.6/pypgstac/migrations/pgstac.0.3.1.sql
--rw-r--r--   0        0        0    10974 2020-02-02 00:00:00.000000 pypgstac-0.7.6/pypgstac/migrations/pgstac.0.3.2-0.3.3.sql
--rw-r--r--   0        0        0    48321 2020-02-02 00:00:00.000000 pypgstac-0.7.6/pypgstac/migrations/pgstac.0.3.2.sql
--rw-r--r--   0        0        0     6266 2020-02-02 00:00:00.000000 pypgstac-0.7.6/pypgstac/migrations/pgstac.0.3.3-0.3.4.sql
--rw-r--r--   0        0        0    49082 2020-02-02 00:00:00.000000 pypgstac-0.7.6/pypgstac/migrations/pgstac.0.3.3.sql
--rw-r--r--   0        0        0    28806 2020-02-02 00:00:00.000000 pypgstac-0.7.6/pypgstac/migrations/pgstac.0.3.4-0.3.5.sql
--rw-r--r--   0        0        0    55504 2020-02-02 00:00:00.000000 pypgstac-0.7.6/pypgstac/migrations/pgstac.0.3.4.sql
--rw-r--r--   0        0        0    14273 2020-02-02 00:00:00.000000 pypgstac-0.7.6/pypgstac/migrations/pgstac.0.3.5-0.3.6.sql
--rw-r--r--   0        0        0    66800 2020-02-02 00:00:00.000000 pypgstac-0.7.6/pypgstac/migrations/pgstac.0.3.5.sql
--rw-r--r--   0        0        0    28561 2020-02-02 00:00:00.000000 pypgstac-0.7.6/pypgstac/migrations/pgstac.0.3.6-0.4.0.sql
--rw-r--r--   0        0        0    68520 2020-02-02 00:00:00.000000 pypgstac-0.7.6/pypgstac/migrations/pgstac.0.3.6.sql
--rw-r--r--   0        0        0     5517 2020-02-02 00:00:00.000000 pypgstac-0.7.6/pypgstac/migrations/pgstac.0.4.0-0.4.1.sql
--rw-r--r--   0        0        0    75093 2020-02-02 00:00:00.000000 pypgstac-0.7.6/pypgstac/migrations/pgstac.0.4.0.sql
--rw-r--r--   0        0        0     5773 2020-02-02 00:00:00.000000 pypgstac-0.7.6/pypgstac/migrations/pgstac.0.4.1-0.4.2.sql
--rw-r--r--   0        0        0    75572 2020-02-02 00:00:00.000000 pypgstac-0.7.6/pypgstac/migrations/pgstac.0.4.1.sql
--rw-r--r--   0        0        0     4725 2020-02-02 00:00:00.000000 pypgstac-0.7.6/pypgstac/migrations/pgstac.0.4.2-0.4.3.sql
--rw-r--r--   0        0        0    75821 2020-02-02 00:00:00.000000 pypgstac-0.7.6/pypgstac/migrations/pgstac.0.4.2.sql
--rw-r--r--   0        0        0    16274 2020-02-02 00:00:00.000000 pypgstac-0.7.6/pypgstac/migrations/pgstac.0.4.3-0.4.4.sql
--rw-r--r--   0        0        0    75829 2020-02-02 00:00:00.000000 pypgstac-0.7.6/pypgstac/migrations/pgstac.0.4.3.sql
--rw-r--r--   0        0        0     8986 2020-02-02 00:00:00.000000 pypgstac-0.7.6/pypgstac/migrations/pgstac.0.4.4-0.4.5.sql
--rw-r--r--   0        0        0    77866 2020-02-02 00:00:00.000000 pypgstac-0.7.6/pypgstac/migrations/pgstac.0.4.4.sql
--rw-r--r--   0        0        0    87157 2020-02-02 00:00:00.000000 pypgstac-0.7.6/pypgstac/migrations/pgstac.0.4.5-0.5.0.sql
--rw-r--r--   0        0        0    77907 2020-02-02 00:00:00.000000 pypgstac-0.7.6/pypgstac/migrations/pgstac.0.4.5.sql
--rw-r--r--   0        0        0     6474 2020-02-02 00:00:00.000000 pypgstac-0.7.6/pypgstac/migrations/pgstac.0.5.0-0.5.1.sql
--rw-r--r--   0        0        0    86941 2020-02-02 00:00:00.000000 pypgstac-0.7.6/pypgstac/migrations/pgstac.0.5.0.sql
--rw-r--r--   0        0        0    23595 2020-02-02 00:00:00.000000 pypgstac-0.7.6/pypgstac/migrations/pgstac.0.5.1-0.6.0.sql
--rw-r--r--   0        0        0    88071 2020-02-02 00:00:00.000000 pypgstac-0.7.6/pypgstac/migrations/pgstac.0.5.1.sql
--rw-r--r--   0        0        0      314 2020-02-02 00:00:00.000000 pypgstac-0.7.6/pypgstac/migrations/pgstac.0.6.0-0.6.1.sql
--rw-r--r--   0        0        0    91221 2020-02-02 00:00:00.000000 pypgstac-0.7.6/pypgstac/migrations/pgstac.0.6.0.sql
--rw-r--r--   0        0        0       64 2020-02-02 00:00:00.000000 pypgstac-0.7.6/pypgstac/migrations/pgstac.0.6.1-0.6.2.sql
--rw-r--r--   0        0        0    91293 2020-02-02 00:00:00.000000 pypgstac-0.7.6/pypgstac/migrations/pgstac.0.6.1.sql
--rw-r--r--   0        0        0     2395 2020-02-02 00:00:00.000000 pypgstac-0.7.6/pypgstac/migrations/pgstac.0.6.10-0.6.11.sql
--rw-r--r--   0        0        0    97746 2020-02-02 00:00:00.000000 pypgstac-0.7.6/pypgstac/migrations/pgstac.0.6.10.sql
--rw-r--r--   0        0        0    23983 2020-02-02 00:00:00.000000 pypgstac-0.7.6/pypgstac/migrations/pgstac.0.6.11-0.6.12.sql
--rw-r--r--   0        0        0    97746 2020-02-02 00:00:00.000000 pypgstac-0.7.6/pypgstac/migrations/pgstac.0.6.11.sql
--rw-r--r--   0        0        0     6177 2020-02-02 00:00:00.000000 pypgstac-0.7.6/pypgstac/migrations/pgstac.0.6.12-0.6.13.sql
--rw-r--r--   0        0        0   109293 2020-02-02 00:00:00.000000 pypgstac-0.7.6/pypgstac/migrations/pgstac.0.6.12.sql
--rw-r--r--   0        0        0    62266 2020-02-02 00:00:00.000000 pypgstac-0.7.6/pypgstac/migrations/pgstac.0.6.13-0.7.0.sql
--rw-r--r--   0        0        0    71093 2020-02-02 00:00:00.000000 pypgstac-0.7.6/pypgstac/migrations/pgstac.0.6.13-0.7.3.sql
--rw-r--r--   0        0        0   109390 2020-02-02 00:00:00.000000 pypgstac-0.7.6/pypgstac/migrations/pgstac.0.6.13.sql
--rw-r--r--   0        0        0      512 2020-02-02 00:00:00.000000 pypgstac-0.7.6/pypgstac/migrations/pgstac.0.6.2-0.6.3.sql
--rw-r--r--   0        0        0    91293 2020-02-02 00:00:00.000000 pypgstac-0.7.6/pypgstac/migrations/pgstac.0.6.2.sql
--rw-r--r--   0        0        0     5310 2020-02-02 00:00:00.000000 pypgstac-0.7.6/pypgstac/migrations/pgstac.0.6.3-0.6.4.sql
--rw-r--r--   0        0        0    91293 2020-02-02 00:00:00.000000 pypgstac-0.7.6/pypgstac/migrations/pgstac.0.6.3.sql
--rw-r--r--   0        0        0     4869 2020-02-02 00:00:00.000000 pypgstac-0.7.6/pypgstac/migrations/pgstac.0.6.4-0.6.5.sql
--rw-r--r--   0        0        0    92207 2020-02-02 00:00:00.000000 pypgstac-0.7.6/pypgstac/migrations/pgstac.0.6.4.sql
--rw-r--r--   0        0        0     6513 2020-02-02 00:00:00.000000 pypgstac-0.7.6/pypgstac/migrations/pgstac.0.6.5-0.6.6.sql
--rw-r--r--   0        0        0    92729 2020-02-02 00:00:00.000000 pypgstac-0.7.6/pypgstac/migrations/pgstac.0.6.5.sql
--rw-r--r--   0        0        0     5879 2020-02-02 00:00:00.000000 pypgstac-0.7.6/pypgstac/migrations/pgstac.0.6.6-0.6.7.sql
--rw-r--r--   0        0        0    93392 2020-02-02 00:00:00.000000 pypgstac-0.7.6/pypgstac/migrations/pgstac.0.6.6.sql
--rw-r--r--   0        0        0    10806 2020-02-02 00:00:00.000000 pypgstac-0.7.6/pypgstac/migrations/pgstac.0.6.7-0.6.8.sql
--rw-r--r--   0        0        0    93421 2020-02-02 00:00:00.000000 pypgstac-0.7.6/pypgstac/migrations/pgstac.0.6.7.sql
--rw-r--r--   0        0        0     6043 2020-02-02 00:00:00.000000 pypgstac-0.7.6/pypgstac/migrations/pgstac.0.6.8-0.6.9.sql
--rw-r--r--   0        0        0    97125 2020-02-02 00:00:00.000000 pypgstac-0.7.6/pypgstac/migrations/pgstac.0.6.8.sql
--rw-r--r--   0        0        0     1323 2020-02-02 00:00:00.000000 pypgstac-0.7.6/pypgstac/migrations/pgstac.0.6.9-0.6.10.sql
--rw-r--r--   0        0        0    97247 2020-02-02 00:00:00.000000 pypgstac-0.7.6/pypgstac/migrations/pgstac.0.6.9.sql
--rw-r--r--   0        0        0    25596 2020-02-02 00:00:00.000000 pypgstac-0.7.6/pypgstac/migrations/pgstac.0.7.0-0.7.1.sql
--rw-r--r--   0        0        0   124336 2020-02-02 00:00:00.000000 pypgstac-0.7.6/pypgstac/migrations/pgstac.0.7.0.sql
--rw-r--r--   0        0        0    12904 2020-02-02 00:00:00.000000 pypgstac-0.7.6/pypgstac/migrations/pgstac.0.7.1-0.7.2.sql
--rw-r--r--   0        0        0   128215 2020-02-02 00:00:00.000000 pypgstac-0.7.6/pypgstac/migrations/pgstac.0.7.1.sql
--rw-r--r--   0        0        0    14951 2020-02-02 00:00:00.000000 pypgstac-0.7.6/pypgstac/migrations/pgstac.0.7.2-0.7.3.sql
--rw-r--r--   0        0        0   129127 2020-02-02 00:00:00.000000 pypgstac-0.7.6/pypgstac/migrations/pgstac.0.7.2.sql
--rw-r--r--   0        0        0    25457 2020-02-02 00:00:00.000000 pypgstac-0.7.6/pypgstac/migrations/pgstac.0.7.3-0.7.4.sql
--rw-r--r--   0        0        0   128574 2020-02-02 00:00:00.000000 pypgstac-0.7.6/pypgstac/migrations/pgstac.0.7.3.sql
--rw-r--r--   0        0        0    35121 2020-02-02 00:00:00.000000 pypgstac-0.7.6/pypgstac/migrations/pgstac.0.7.4-0.7.5.sql
--rw-r--r--   0        0        0   132836 2020-02-02 00:00:00.000000 pypgstac-0.7.6/pypgstac/migrations/pgstac.0.7.4.sql
--rw-r--r--   0        0        0     9372 2020-02-02 00:00:00.000000 pypgstac-0.7.6/pypgstac/migrations/pgstac.0.7.5-0.7.6.sql
--rw-r--r--   0        0        0   135008 2020-02-02 00:00:00.000000 pypgstac-0.7.6/pypgstac/migrations/pgstac.0.7.5.sql
--rw-r--r--   0        0        0   135021 2020-02-02 00:00:00.000000 pypgstac-0.7.6/pypgstac/migrations/pgstac.0.7.6.sql
--rw-r--r--   0        0        0       58 2020-02-02 00:00:00.000000 pypgstac-0.7.6/.gitignore
--rw-r--r--   0        0        0       49 2020-02-02 00:00:00.000000 pypgstac-0.7.6/README.md
--rw-r--r--   0        0        0     3024 2020-02-02 00:00:00.000000 pypgstac-0.7.6/pyproject.toml
--rw-r--r--   0        0        0     2185 2020-02-02 00:00:00.000000 pypgstac-0.7.6/PKG-INFO
+-rw-r--r--   0        0        0      868 2020-02-02 00:00:00.000000 pypgstac-0.7.7/setup.py
+-rw-r--r--   0        0        0       92 2020-02-02 00:00:00.000000 pypgstac-0.7.7/pypgstac/__init__.py
+-rw-r--r--   0        0        0     8950 2020-02-02 00:00:00.000000 pypgstac-0.7.7/pypgstac/db.py
+-rw-r--r--   0        0        0     5520 2020-02-02 00:00:00.000000 pypgstac-0.7.7/pypgstac/hydration.py
+-rw-r--r--   0        0        0    25760 2020-02-02 00:00:00.000000 pypgstac-0.7.7/pypgstac/load.py
+-rw-r--r--   0        0        0     5244 2020-02-02 00:00:00.000000 pypgstac-0.7.7/pypgstac/migrate.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pypgstac-0.7.7/pypgstac/py.typed
+-rwxr-xr-x   0        0        0     3443 2020-02-02 00:00:00.000000 pypgstac-0.7.7/pypgstac/pypgstac.py
+-rw-r--r--   0        0        0       37 2020-02-02 00:00:00.000000 pypgstac-0.7.7/pypgstac/version.py
+-rw-r--r--   0        0        0       86 2020-02-02 00:00:00.000000 pypgstac-0.7.7/pypgstac/migrations/pgstac.0.1.9-0.2.3.sql
+-rw-r--r--   0        0        0    35445 2020-02-02 00:00:00.000000 pypgstac-0.7.7/pypgstac/migrations/pgstac.0.1.9.sql
+-rw-r--r--   0        0        0       86 2020-02-02 00:00:00.000000 pypgstac-0.7.7/pypgstac/migrations/pgstac.0.2.3-0.2.4.sql
+-rw-r--r--   0        0        0    35445 2020-02-02 00:00:00.000000 pypgstac-0.7.7/pypgstac/migrations/pgstac.0.2.3.sql
+-rw-r--r--   0        0        0     7132 2020-02-02 00:00:00.000000 pypgstac-0.7.7/pypgstac/migrations/pgstac.0.2.4-0.2.5.sql
+-rw-r--r--   0        0        0     8816 2020-02-02 00:00:00.000000 pypgstac-0.7.7/pypgstac/migrations/pgstac.0.2.4-0.2.7.sql
+-rw-r--r--   0        0        0    35445 2020-02-02 00:00:00.000000 pypgstac-0.7.7/pypgstac/migrations/pgstac.0.2.4.sql
+-rw-r--r--   0        0        0     1783 2020-02-02 00:00:00.000000 pypgstac-0.7.7/pypgstac/migrations/pgstac.0.2.5-0.2.7.sql
+-rw-r--r--   0        0        0    35570 2020-02-02 00:00:00.000000 pypgstac-0.7.7/pypgstac/migrations/pgstac.0.2.5.sql
+-rw-r--r--   0        0        0      103 2020-02-02 00:00:00.000000 pypgstac-0.7.7/pypgstac/migrations/pgstac.0.2.7-0.2.8.sql
+-rw-r--r--   0        0        0    35570 2020-02-02 00:00:00.000000 pypgstac-0.7.7/pypgstac/migrations/pgstac.0.2.7.sql
+-rw-r--r--   0        0        0       86 2020-02-02 00:00:00.000000 pypgstac-0.7.7/pypgstac/migrations/pgstac.0.2.8-0.2.9.sql
+-rw-r--r--   0        0        0    30676 2020-02-02 00:00:00.000000 pypgstac-0.7.7/pypgstac/migrations/pgstac.0.2.8.sql
+-rw-r--r--   0        0        0    48852 2020-02-02 00:00:00.000000 pypgstac-0.7.7/pypgstac/migrations/pgstac.0.2.9-0.3.0.sql
+-rw-r--r--   0        0        0    30676 2020-02-02 00:00:00.000000 pypgstac-0.7.7/pypgstac/migrations/pgstac.0.2.9.sql
+-rw-r--r--   0        0        0      732 2020-02-02 00:00:00.000000 pypgstac-0.7.7/pypgstac/migrations/pgstac.0.3.0-0.3.1.sql
+-rw-r--r--   0        0        0    48316 2020-02-02 00:00:00.000000 pypgstac-0.7.7/pypgstac/migrations/pgstac.0.3.0.sql
+-rw-r--r--   0        0        0     1692 2020-02-02 00:00:00.000000 pypgstac-0.7.7/pypgstac/migrations/pgstac.0.3.1-0.3.2.sql
+-rw-r--r--   0        0        0    48318 2020-02-02 00:00:00.000000 pypgstac-0.7.7/pypgstac/migrations/pgstac.0.3.1.sql
+-rw-r--r--   0        0        0    10974 2020-02-02 00:00:00.000000 pypgstac-0.7.7/pypgstac/migrations/pgstac.0.3.2-0.3.3.sql
+-rw-r--r--   0        0        0    48321 2020-02-02 00:00:00.000000 pypgstac-0.7.7/pypgstac/migrations/pgstac.0.3.2.sql
+-rw-r--r--   0        0        0     6266 2020-02-02 00:00:00.000000 pypgstac-0.7.7/pypgstac/migrations/pgstac.0.3.3-0.3.4.sql
+-rw-r--r--   0        0        0    49082 2020-02-02 00:00:00.000000 pypgstac-0.7.7/pypgstac/migrations/pgstac.0.3.3.sql
+-rw-r--r--   0        0        0    28806 2020-02-02 00:00:00.000000 pypgstac-0.7.7/pypgstac/migrations/pgstac.0.3.4-0.3.5.sql
+-rw-r--r--   0        0        0    55504 2020-02-02 00:00:00.000000 pypgstac-0.7.7/pypgstac/migrations/pgstac.0.3.4.sql
+-rw-r--r--   0        0        0    14273 2020-02-02 00:00:00.000000 pypgstac-0.7.7/pypgstac/migrations/pgstac.0.3.5-0.3.6.sql
+-rw-r--r--   0        0        0    66800 2020-02-02 00:00:00.000000 pypgstac-0.7.7/pypgstac/migrations/pgstac.0.3.5.sql
+-rw-r--r--   0        0        0    28561 2020-02-02 00:00:00.000000 pypgstac-0.7.7/pypgstac/migrations/pgstac.0.3.6-0.4.0.sql
+-rw-r--r--   0        0        0    68520 2020-02-02 00:00:00.000000 pypgstac-0.7.7/pypgstac/migrations/pgstac.0.3.6.sql
+-rw-r--r--   0        0        0     5517 2020-02-02 00:00:00.000000 pypgstac-0.7.7/pypgstac/migrations/pgstac.0.4.0-0.4.1.sql
+-rw-r--r--   0        0        0    75093 2020-02-02 00:00:00.000000 pypgstac-0.7.7/pypgstac/migrations/pgstac.0.4.0.sql
+-rw-r--r--   0        0        0     5773 2020-02-02 00:00:00.000000 pypgstac-0.7.7/pypgstac/migrations/pgstac.0.4.1-0.4.2.sql
+-rw-r--r--   0        0        0    75572 2020-02-02 00:00:00.000000 pypgstac-0.7.7/pypgstac/migrations/pgstac.0.4.1.sql
+-rw-r--r--   0        0        0     4725 2020-02-02 00:00:00.000000 pypgstac-0.7.7/pypgstac/migrations/pgstac.0.4.2-0.4.3.sql
+-rw-r--r--   0        0        0    75821 2020-02-02 00:00:00.000000 pypgstac-0.7.7/pypgstac/migrations/pgstac.0.4.2.sql
+-rw-r--r--   0        0        0    16274 2020-02-02 00:00:00.000000 pypgstac-0.7.7/pypgstac/migrations/pgstac.0.4.3-0.4.4.sql
+-rw-r--r--   0        0        0    75829 2020-02-02 00:00:00.000000 pypgstac-0.7.7/pypgstac/migrations/pgstac.0.4.3.sql
+-rw-r--r--   0        0        0     8986 2020-02-02 00:00:00.000000 pypgstac-0.7.7/pypgstac/migrations/pgstac.0.4.4-0.4.5.sql
+-rw-r--r--   0        0        0    77866 2020-02-02 00:00:00.000000 pypgstac-0.7.7/pypgstac/migrations/pgstac.0.4.4.sql
+-rw-r--r--   0        0        0    87157 2020-02-02 00:00:00.000000 pypgstac-0.7.7/pypgstac/migrations/pgstac.0.4.5-0.5.0.sql
+-rw-r--r--   0        0        0    77907 2020-02-02 00:00:00.000000 pypgstac-0.7.7/pypgstac/migrations/pgstac.0.4.5.sql
+-rw-r--r--   0        0        0     6474 2020-02-02 00:00:00.000000 pypgstac-0.7.7/pypgstac/migrations/pgstac.0.5.0-0.5.1.sql
+-rw-r--r--   0        0        0    86941 2020-02-02 00:00:00.000000 pypgstac-0.7.7/pypgstac/migrations/pgstac.0.5.0.sql
+-rw-r--r--   0        0        0    23595 2020-02-02 00:00:00.000000 pypgstac-0.7.7/pypgstac/migrations/pgstac.0.5.1-0.6.0.sql
+-rw-r--r--   0        0        0    88071 2020-02-02 00:00:00.000000 pypgstac-0.7.7/pypgstac/migrations/pgstac.0.5.1.sql
+-rw-r--r--   0        0        0      314 2020-02-02 00:00:00.000000 pypgstac-0.7.7/pypgstac/migrations/pgstac.0.6.0-0.6.1.sql
+-rw-r--r--   0        0        0    91221 2020-02-02 00:00:00.000000 pypgstac-0.7.7/pypgstac/migrations/pgstac.0.6.0.sql
+-rw-r--r--   0        0        0       64 2020-02-02 00:00:00.000000 pypgstac-0.7.7/pypgstac/migrations/pgstac.0.6.1-0.6.2.sql
+-rw-r--r--   0        0        0    91293 2020-02-02 00:00:00.000000 pypgstac-0.7.7/pypgstac/migrations/pgstac.0.6.1.sql
+-rw-r--r--   0        0        0     2395 2020-02-02 00:00:00.000000 pypgstac-0.7.7/pypgstac/migrations/pgstac.0.6.10-0.6.11.sql
+-rw-r--r--   0        0        0    97746 2020-02-02 00:00:00.000000 pypgstac-0.7.7/pypgstac/migrations/pgstac.0.6.10.sql
+-rw-r--r--   0        0        0    23983 2020-02-02 00:00:00.000000 pypgstac-0.7.7/pypgstac/migrations/pgstac.0.6.11-0.6.12.sql
+-rw-r--r--   0        0        0    97746 2020-02-02 00:00:00.000000 pypgstac-0.7.7/pypgstac/migrations/pgstac.0.6.11.sql
+-rw-r--r--   0        0        0     6177 2020-02-02 00:00:00.000000 pypgstac-0.7.7/pypgstac/migrations/pgstac.0.6.12-0.6.13.sql
+-rw-r--r--   0        0        0   109293 2020-02-02 00:00:00.000000 pypgstac-0.7.7/pypgstac/migrations/pgstac.0.6.12.sql
+-rw-r--r--   0        0        0    62266 2020-02-02 00:00:00.000000 pypgstac-0.7.7/pypgstac/migrations/pgstac.0.6.13-0.7.0.sql
+-rw-r--r--   0        0        0    71093 2020-02-02 00:00:00.000000 pypgstac-0.7.7/pypgstac/migrations/pgstac.0.6.13-0.7.3.sql
+-rw-r--r--   0        0        0   109390 2020-02-02 00:00:00.000000 pypgstac-0.7.7/pypgstac/migrations/pgstac.0.6.13.sql
+-rw-r--r--   0        0        0      512 2020-02-02 00:00:00.000000 pypgstac-0.7.7/pypgstac/migrations/pgstac.0.6.2-0.6.3.sql
+-rw-r--r--   0        0        0    91293 2020-02-02 00:00:00.000000 pypgstac-0.7.7/pypgstac/migrations/pgstac.0.6.2.sql
+-rw-r--r--   0        0        0     5310 2020-02-02 00:00:00.000000 pypgstac-0.7.7/pypgstac/migrations/pgstac.0.6.3-0.6.4.sql
+-rw-r--r--   0        0        0    91293 2020-02-02 00:00:00.000000 pypgstac-0.7.7/pypgstac/migrations/pgstac.0.6.3.sql
+-rw-r--r--   0        0        0     4869 2020-02-02 00:00:00.000000 pypgstac-0.7.7/pypgstac/migrations/pgstac.0.6.4-0.6.5.sql
+-rw-r--r--   0        0        0    92207 2020-02-02 00:00:00.000000 pypgstac-0.7.7/pypgstac/migrations/pgstac.0.6.4.sql
+-rw-r--r--   0        0        0     6513 2020-02-02 00:00:00.000000 pypgstac-0.7.7/pypgstac/migrations/pgstac.0.6.5-0.6.6.sql
+-rw-r--r--   0        0        0    92729 2020-02-02 00:00:00.000000 pypgstac-0.7.7/pypgstac/migrations/pgstac.0.6.5.sql
+-rw-r--r--   0        0        0     5879 2020-02-02 00:00:00.000000 pypgstac-0.7.7/pypgstac/migrations/pgstac.0.6.6-0.6.7.sql
+-rw-r--r--   0        0        0    93392 2020-02-02 00:00:00.000000 pypgstac-0.7.7/pypgstac/migrations/pgstac.0.6.6.sql
+-rw-r--r--   0        0        0    10806 2020-02-02 00:00:00.000000 pypgstac-0.7.7/pypgstac/migrations/pgstac.0.6.7-0.6.8.sql
+-rw-r--r--   0        0        0    93421 2020-02-02 00:00:00.000000 pypgstac-0.7.7/pypgstac/migrations/pgstac.0.6.7.sql
+-rw-r--r--   0        0        0     6043 2020-02-02 00:00:00.000000 pypgstac-0.7.7/pypgstac/migrations/pgstac.0.6.8-0.6.9.sql
+-rw-r--r--   0        0        0    97125 2020-02-02 00:00:00.000000 pypgstac-0.7.7/pypgstac/migrations/pgstac.0.6.8.sql
+-rw-r--r--   0        0        0     1323 2020-02-02 00:00:00.000000 pypgstac-0.7.7/pypgstac/migrations/pgstac.0.6.9-0.6.10.sql
+-rw-r--r--   0        0        0    97247 2020-02-02 00:00:00.000000 pypgstac-0.7.7/pypgstac/migrations/pgstac.0.6.9.sql
+-rw-r--r--   0        0        0    25596 2020-02-02 00:00:00.000000 pypgstac-0.7.7/pypgstac/migrations/pgstac.0.7.0-0.7.1.sql
+-rw-r--r--   0        0        0   124336 2020-02-02 00:00:00.000000 pypgstac-0.7.7/pypgstac/migrations/pgstac.0.7.0.sql
+-rw-r--r--   0        0        0    12904 2020-02-02 00:00:00.000000 pypgstac-0.7.7/pypgstac/migrations/pgstac.0.7.1-0.7.2.sql
+-rw-r--r--   0        0        0   128215 2020-02-02 00:00:00.000000 pypgstac-0.7.7/pypgstac/migrations/pgstac.0.7.1.sql
+-rw-r--r--   0        0        0    14951 2020-02-02 00:00:00.000000 pypgstac-0.7.7/pypgstac/migrations/pgstac.0.7.2-0.7.3.sql
+-rw-r--r--   0        0        0   129127 2020-02-02 00:00:00.000000 pypgstac-0.7.7/pypgstac/migrations/pgstac.0.7.2.sql
+-rw-r--r--   0        0        0    25457 2020-02-02 00:00:00.000000 pypgstac-0.7.7/pypgstac/migrations/pgstac.0.7.3-0.7.4.sql
+-rw-r--r--   0        0        0   128574 2020-02-02 00:00:00.000000 pypgstac-0.7.7/pypgstac/migrations/pgstac.0.7.3.sql
+-rw-r--r--   0        0        0    35126 2020-02-02 00:00:00.000000 pypgstac-0.7.7/pypgstac/migrations/pgstac.0.7.4-0.7.5.sql
+-rw-r--r--   0        0        0   132836 2020-02-02 00:00:00.000000 pypgstac-0.7.7/pypgstac/migrations/pgstac.0.7.4.sql
+-rw-r--r--   0        0        0     9377 2020-02-02 00:00:00.000000 pypgstac-0.7.7/pypgstac/migrations/pgstac.0.7.5-0.7.6.sql
+-rw-r--r--   0        0        0   135013 2020-02-02 00:00:00.000000 pypgstac-0.7.7/pypgstac/migrations/pgstac.0.7.5.sql
+-rw-r--r--   0        0        0    14610 2020-02-02 00:00:00.000000 pypgstac-0.7.7/pypgstac/migrations/pgstac.0.7.6-0.7.7.sql
+-rw-r--r--   0        0        0   135026 2020-02-02 00:00:00.000000 pypgstac-0.7.7/pypgstac/migrations/pgstac.0.7.6.sql
+-rw-r--r--   0        0        0   136049 2020-02-02 00:00:00.000000 pypgstac-0.7.7/pypgstac/migrations/pgstac.0.7.7.sql
+-rw-r--r--   0        0        0       58 2020-02-02 00:00:00.000000 pypgstac-0.7.7/.gitignore
+-rw-r--r--   0        0        0       49 2020-02-02 00:00:00.000000 pypgstac-0.7.7/README.md
+-rw-r--r--   0        0        0     3024 2020-02-02 00:00:00.000000 pypgstac-0.7.7/pyproject.toml
+-rw-r--r--   0        0        0     2185 2020-02-02 00:00:00.000000 pypgstac-0.7.7/PKG-INFO
```

### Comparing `pypgstac-0.7.6/setup.py` & `pypgstac-0.7.7/setup.py`

 * *Files identical despite different names*

### Comparing `pypgstac-0.7.6/pypgstac/db.py` & `pypgstac-0.7.7/pypgstac/db.py`

 * *Files identical despite different names*

### Comparing `pypgstac-0.7.6/pypgstac/hydration.py` & `pypgstac-0.7.7/pypgstac/hydration.py`

 * *Files identical despite different names*

### Comparing `pypgstac-0.7.6/pypgstac/load.py` & `pypgstac-0.7.7/pypgstac/load.py`

 * *Files identical despite different names*

### Comparing `pypgstac-0.7.6/pypgstac/migrate.py` & `pypgstac-0.7.7/pypgstac/migrate.py`

 * *Files identical despite different names*

### Comparing `pypgstac-0.7.6/pypgstac/pypgstac.py` & `pypgstac-0.7.7/pypgstac/pypgstac.py`

 * *Files identical despite different names*

### Comparing `pypgstac-0.7.6/pypgstac/migrations/pgstac.0.1.9.sql` & `pypgstac-0.7.7/pypgstac/migrations/pgstac.0.1.9.sql`

 * *Files identical despite different names*

### Comparing `pypgstac-0.7.6/pypgstac/migrations/pgstac.0.2.3.sql` & `pypgstac-0.7.7/pypgstac/migrations/pgstac.0.2.3.sql`

 * *Files identical despite different names*

### Comparing `pypgstac-0.7.6/pypgstac/migrations/pgstac.0.2.4-0.2.5.sql` & `pypgstac-0.7.7/pypgstac/migrations/pgstac.0.2.4-0.2.5.sql`

 * *Files identical despite different names*

### Comparing `pypgstac-0.7.6/pypgstac/migrations/pgstac.0.2.4-0.2.7.sql` & `pypgstac-0.7.7/pypgstac/migrations/pgstac.0.2.4-0.2.7.sql`

 * *Files identical despite different names*

### Comparing `pypgstac-0.7.6/pypgstac/migrations/pgstac.0.2.4.sql` & `pypgstac-0.7.7/pypgstac/migrations/pgstac.0.2.4.sql`

 * *Files identical despite different names*

### Comparing `pypgstac-0.7.6/pypgstac/migrations/pgstac.0.2.5-0.2.7.sql` & `pypgstac-0.7.7/pypgstac/migrations/pgstac.0.2.5-0.2.7.sql`

 * *Files identical despite different names*

### Comparing `pypgstac-0.7.6/pypgstac/migrations/pgstac.0.2.5.sql` & `pypgstac-0.7.7/pypgstac/migrations/pgstac.0.2.5.sql`

 * *Files identical despite different names*

### Comparing `pypgstac-0.7.6/pypgstac/migrations/pgstac.0.2.7.sql` & `pypgstac-0.7.7/pypgstac/migrations/pgstac.0.2.7.sql`

 * *Files identical despite different names*

### Comparing `pypgstac-0.7.6/pypgstac/migrations/pgstac.0.2.8.sql` & `pypgstac-0.7.7/pypgstac/migrations/pgstac.0.2.8.sql`

 * *Files identical despite different names*

### Comparing `pypgstac-0.7.6/pypgstac/migrations/pgstac.0.2.9-0.3.0.sql` & `pypgstac-0.7.7/pypgstac/migrations/pgstac.0.2.9-0.3.0.sql`

 * *Files identical despite different names*

### Comparing `pypgstac-0.7.6/pypgstac/migrations/pgstac.0.2.9.sql` & `pypgstac-0.7.7/pypgstac/migrations/pgstac.0.2.9.sql`

 * *Files identical despite different names*

### Comparing `pypgstac-0.7.6/pypgstac/migrations/pgstac.0.3.0-0.3.1.sql` & `pypgstac-0.7.7/pypgstac/migrations/pgstac.0.3.0-0.3.1.sql`

 * *Files identical despite different names*

### Comparing `pypgstac-0.7.6/pypgstac/migrations/pgstac.0.3.0.sql` & `pypgstac-0.7.7/pypgstac/migrations/pgstac.0.3.0.sql`

 * *Files identical despite different names*

### Comparing `pypgstac-0.7.6/pypgstac/migrations/pgstac.0.3.1-0.3.2.sql` & `pypgstac-0.7.7/pypgstac/migrations/pgstac.0.3.1-0.3.2.sql`

 * *Files identical despite different names*

### Comparing `pypgstac-0.7.6/pypgstac/migrations/pgstac.0.3.1.sql` & `pypgstac-0.7.7/pypgstac/migrations/pgstac.0.3.1.sql`

 * *Files identical despite different names*

### Comparing `pypgstac-0.7.6/pypgstac/migrations/pgstac.0.3.2-0.3.3.sql` & `pypgstac-0.7.7/pypgstac/migrations/pgstac.0.3.2-0.3.3.sql`

 * *Files identical despite different names*

### Comparing `pypgstac-0.7.6/pypgstac/migrations/pgstac.0.3.2.sql` & `pypgstac-0.7.7/pypgstac/migrations/pgstac.0.3.2.sql`

 * *Files identical despite different names*

### Comparing `pypgstac-0.7.6/pypgstac/migrations/pgstac.0.3.3-0.3.4.sql` & `pypgstac-0.7.7/pypgstac/migrations/pgstac.0.3.3-0.3.4.sql`

 * *Files identical despite different names*

### Comparing `pypgstac-0.7.6/pypgstac/migrations/pgstac.0.3.3.sql` & `pypgstac-0.7.7/pypgstac/migrations/pgstac.0.3.3.sql`

 * *Files identical despite different names*

### Comparing `pypgstac-0.7.6/pypgstac/migrations/pgstac.0.3.4-0.3.5.sql` & `pypgstac-0.7.7/pypgstac/migrations/pgstac.0.3.4-0.3.5.sql`

 * *Files identical despite different names*

### Comparing `pypgstac-0.7.6/pypgstac/migrations/pgstac.0.3.4.sql` & `pypgstac-0.7.7/pypgstac/migrations/pgstac.0.3.4.sql`

 * *Files identical despite different names*

### Comparing `pypgstac-0.7.6/pypgstac/migrations/pgstac.0.3.5-0.3.6.sql` & `pypgstac-0.7.7/pypgstac/migrations/pgstac.0.3.5-0.3.6.sql`

 * *Files identical despite different names*

### Comparing `pypgstac-0.7.6/pypgstac/migrations/pgstac.0.3.5.sql` & `pypgstac-0.7.7/pypgstac/migrations/pgstac.0.3.5.sql`

 * *Files identical despite different names*

### Comparing `pypgstac-0.7.6/pypgstac/migrations/pgstac.0.3.6-0.4.0.sql` & `pypgstac-0.7.7/pypgstac/migrations/pgstac.0.3.6-0.4.0.sql`

 * *Files identical despite different names*

### Comparing `pypgstac-0.7.6/pypgstac/migrations/pgstac.0.3.6.sql` & `pypgstac-0.7.7/pypgstac/migrations/pgstac.0.3.6.sql`

 * *Files identical despite different names*

### Comparing `pypgstac-0.7.6/pypgstac/migrations/pgstac.0.4.0-0.4.1.sql` & `pypgstac-0.7.7/pypgstac/migrations/pgstac.0.4.0-0.4.1.sql`

 * *Files identical despite different names*

### Comparing `pypgstac-0.7.6/pypgstac/migrations/pgstac.0.4.0.sql` & `pypgstac-0.7.7/pypgstac/migrations/pgstac.0.4.0.sql`

 * *Files identical despite different names*

### Comparing `pypgstac-0.7.6/pypgstac/migrations/pgstac.0.4.1-0.4.2.sql` & `pypgstac-0.7.7/pypgstac/migrations/pgstac.0.4.1-0.4.2.sql`

 * *Files identical despite different names*

### Comparing `pypgstac-0.7.6/pypgstac/migrations/pgstac.0.4.1.sql` & `pypgstac-0.7.7/pypgstac/migrations/pgstac.0.4.1.sql`

 * *Files identical despite different names*

### Comparing `pypgstac-0.7.6/pypgstac/migrations/pgstac.0.4.2-0.4.3.sql` & `pypgstac-0.7.7/pypgstac/migrations/pgstac.0.4.2-0.4.3.sql`

 * *Files identical despite different names*

### Comparing `pypgstac-0.7.6/pypgstac/migrations/pgstac.0.4.2.sql` & `pypgstac-0.7.7/pypgstac/migrations/pgstac.0.4.2.sql`

 * *Files identical despite different names*

### Comparing `pypgstac-0.7.6/pypgstac/migrations/pgstac.0.4.3-0.4.4.sql` & `pypgstac-0.7.7/pypgstac/migrations/pgstac.0.4.3-0.4.4.sql`

 * *Files identical despite different names*

### Comparing `pypgstac-0.7.6/pypgstac/migrations/pgstac.0.4.3.sql` & `pypgstac-0.7.7/pypgstac/migrations/pgstac.0.4.3.sql`

 * *Files identical despite different names*

### Comparing `pypgstac-0.7.6/pypgstac/migrations/pgstac.0.4.4-0.4.5.sql` & `pypgstac-0.7.7/pypgstac/migrations/pgstac.0.4.4-0.4.5.sql`

 * *Files identical despite different names*

### Comparing `pypgstac-0.7.6/pypgstac/migrations/pgstac.0.4.4.sql` & `pypgstac-0.7.7/pypgstac/migrations/pgstac.0.4.4.sql`

 * *Files identical despite different names*

### Comparing `pypgstac-0.7.6/pypgstac/migrations/pgstac.0.4.5-0.5.0.sql` & `pypgstac-0.7.7/pypgstac/migrations/pgstac.0.4.5-0.5.0.sql`

 * *Files identical despite different names*

### Comparing `pypgstac-0.7.6/pypgstac/migrations/pgstac.0.4.5.sql` & `pypgstac-0.7.7/pypgstac/migrations/pgstac.0.4.5.sql`

 * *Files identical despite different names*

### Comparing `pypgstac-0.7.6/pypgstac/migrations/pgstac.0.5.0-0.5.1.sql` & `pypgstac-0.7.7/pypgstac/migrations/pgstac.0.5.0-0.5.1.sql`

 * *Files identical despite different names*

### Comparing `pypgstac-0.7.6/pypgstac/migrations/pgstac.0.5.0.sql` & `pypgstac-0.7.7/pypgstac/migrations/pgstac.0.5.0.sql`

 * *Files identical despite different names*

### Comparing `pypgstac-0.7.6/pypgstac/migrations/pgstac.0.5.1-0.6.0.sql` & `pypgstac-0.7.7/pypgstac/migrations/pgstac.0.5.1-0.6.0.sql`

 * *Files identical despite different names*

### Comparing `pypgstac-0.7.6/pypgstac/migrations/pgstac.0.5.1.sql` & `pypgstac-0.7.7/pypgstac/migrations/pgstac.0.5.1.sql`

 * *Files identical despite different names*

### Comparing `pypgstac-0.7.6/pypgstac/migrations/pgstac.0.6.0.sql` & `pypgstac-0.7.7/pypgstac/migrations/pgstac.0.6.0.sql`

 * *Files identical despite different names*

### Comparing `pypgstac-0.7.6/pypgstac/migrations/pgstac.0.6.1.sql` & `pypgstac-0.7.7/pypgstac/migrations/pgstac.0.6.1.sql`

 * *Files identical despite different names*

### Comparing `pypgstac-0.7.6/pypgstac/migrations/pgstac.0.6.10-0.6.11.sql` & `pypgstac-0.7.7/pypgstac/migrations/pgstac.0.6.10-0.6.11.sql`

 * *Files identical despite different names*

### Comparing `pypgstac-0.7.6/pypgstac/migrations/pgstac.0.6.10.sql` & `pypgstac-0.7.7/pypgstac/migrations/pgstac.0.6.10.sql`

 * *Files identical despite different names*

### Comparing `pypgstac-0.7.6/pypgstac/migrations/pgstac.0.6.11-0.6.12.sql` & `pypgstac-0.7.7/pypgstac/migrations/pgstac.0.6.11-0.6.12.sql`

 * *Files identical despite different names*

### Comparing `pypgstac-0.7.6/pypgstac/migrations/pgstac.0.6.11.sql` & `pypgstac-0.7.7/pypgstac/migrations/pgstac.0.6.11.sql`

 * *Files identical despite different names*

### Comparing `pypgstac-0.7.6/pypgstac/migrations/pgstac.0.6.12-0.6.13.sql` & `pypgstac-0.7.7/pypgstac/migrations/pgstac.0.6.12-0.6.13.sql`

 * *Files identical despite different names*

### Comparing `pypgstac-0.7.6/pypgstac/migrations/pgstac.0.6.12.sql` & `pypgstac-0.7.7/pypgstac/migrations/pgstac.0.6.12.sql`

 * *Files identical despite different names*

### Comparing `pypgstac-0.7.6/pypgstac/migrations/pgstac.0.6.13-0.7.0.sql` & `pypgstac-0.7.7/pypgstac/migrations/pgstac.0.6.13-0.7.0.sql`

 * *Files identical despite different names*

### Comparing `pypgstac-0.7.6/pypgstac/migrations/pgstac.0.6.13-0.7.3.sql` & `pypgstac-0.7.7/pypgstac/migrations/pgstac.0.6.13-0.7.3.sql`

 * *Files identical despite different names*

### Comparing `pypgstac-0.7.6/pypgstac/migrations/pgstac.0.6.13.sql` & `pypgstac-0.7.7/pypgstac/migrations/pgstac.0.6.13.sql`

 * *Files identical despite different names*

### Comparing `pypgstac-0.7.6/pypgstac/migrations/pgstac.0.6.2-0.6.3.sql` & `pypgstac-0.7.7/pypgstac/migrations/pgstac.0.6.2-0.6.3.sql`

 * *Files identical despite different names*

### Comparing `pypgstac-0.7.6/pypgstac/migrations/pgstac.0.6.2.sql` & `pypgstac-0.7.7/pypgstac/migrations/pgstac.0.6.2.sql`

 * *Files identical despite different names*

### Comparing `pypgstac-0.7.6/pypgstac/migrations/pgstac.0.6.3-0.6.4.sql` & `pypgstac-0.7.7/pypgstac/migrations/pgstac.0.6.3-0.6.4.sql`

 * *Files identical despite different names*

### Comparing `pypgstac-0.7.6/pypgstac/migrations/pgstac.0.6.3.sql` & `pypgstac-0.7.7/pypgstac/migrations/pgstac.0.6.3.sql`

 * *Files identical despite different names*

### Comparing `pypgstac-0.7.6/pypgstac/migrations/pgstac.0.6.4-0.6.5.sql` & `pypgstac-0.7.7/pypgstac/migrations/pgstac.0.6.4-0.6.5.sql`

 * *Files identical despite different names*

### Comparing `pypgstac-0.7.6/pypgstac/migrations/pgstac.0.6.4.sql` & `pypgstac-0.7.7/pypgstac/migrations/pgstac.0.6.4.sql`

 * *Files identical despite different names*

### Comparing `pypgstac-0.7.6/pypgstac/migrations/pgstac.0.6.5-0.6.6.sql` & `pypgstac-0.7.7/pypgstac/migrations/pgstac.0.6.5-0.6.6.sql`

 * *Files identical despite different names*

### Comparing `pypgstac-0.7.6/pypgstac/migrations/pgstac.0.6.5.sql` & `pypgstac-0.7.7/pypgstac/migrations/pgstac.0.6.5.sql`

 * *Files identical despite different names*

### Comparing `pypgstac-0.7.6/pypgstac/migrations/pgstac.0.6.6-0.6.7.sql` & `pypgstac-0.7.7/pypgstac/migrations/pgstac.0.6.6-0.6.7.sql`

 * *Files identical despite different names*

### Comparing `pypgstac-0.7.6/pypgstac/migrations/pgstac.0.6.6.sql` & `pypgstac-0.7.7/pypgstac/migrations/pgstac.0.6.6.sql`

 * *Files identical despite different names*

### Comparing `pypgstac-0.7.6/pypgstac/migrations/pgstac.0.6.7-0.6.8.sql` & `pypgstac-0.7.7/pypgstac/migrations/pgstac.0.6.7-0.6.8.sql`

 * *Files identical despite different names*

### Comparing `pypgstac-0.7.6/pypgstac/migrations/pgstac.0.6.7.sql` & `pypgstac-0.7.7/pypgstac/migrations/pgstac.0.6.7.sql`

 * *Files identical despite different names*

### Comparing `pypgstac-0.7.6/pypgstac/migrations/pgstac.0.6.8-0.6.9.sql` & `pypgstac-0.7.7/pypgstac/migrations/pgstac.0.6.8-0.6.9.sql`

 * *Files identical despite different names*

### Comparing `pypgstac-0.7.6/pypgstac/migrations/pgstac.0.6.8.sql` & `pypgstac-0.7.7/pypgstac/migrations/pgstac.0.6.8.sql`

 * *Files identical despite different names*

### Comparing `pypgstac-0.7.6/pypgstac/migrations/pgstac.0.6.9-0.6.10.sql` & `pypgstac-0.7.7/pypgstac/migrations/pgstac.0.6.9-0.6.10.sql`

 * *Files identical despite different names*

### Comparing `pypgstac-0.7.6/pypgstac/migrations/pgstac.0.6.9.sql` & `pypgstac-0.7.7/pypgstac/migrations/pgstac.0.6.9.sql`

 * *Files identical despite different names*

### Comparing `pypgstac-0.7.6/pypgstac/migrations/pgstac.0.7.0-0.7.1.sql` & `pypgstac-0.7.7/pypgstac/migrations/pgstac.0.7.0-0.7.1.sql`

 * *Files identical despite different names*

### Comparing `pypgstac-0.7.6/pypgstac/migrations/pgstac.0.7.0.sql` & `pypgstac-0.7.7/pypgstac/migrations/pgstac.0.7.0.sql`

 * *Files identical despite different names*

### Comparing `pypgstac-0.7.6/pypgstac/migrations/pgstac.0.7.1-0.7.2.sql` & `pypgstac-0.7.7/pypgstac/migrations/pgstac.0.7.1-0.7.2.sql`

 * *Files identical despite different names*

### Comparing `pypgstac-0.7.6/pypgstac/migrations/pgstac.0.7.1.sql` & `pypgstac-0.7.7/pypgstac/migrations/pgstac.0.7.1.sql`

 * *Files identical despite different names*

### Comparing `pypgstac-0.7.6/pypgstac/migrations/pgstac.0.7.2-0.7.3.sql` & `pypgstac-0.7.7/pypgstac/migrations/pgstac.0.7.2-0.7.3.sql`

 * *Files identical despite different names*

### Comparing `pypgstac-0.7.6/pypgstac/migrations/pgstac.0.7.2.sql` & `pypgstac-0.7.7/pypgstac/migrations/pgstac.0.7.2.sql`

 * *Files identical despite different names*

### Comparing `pypgstac-0.7.6/pypgstac/migrations/pgstac.0.7.3-0.7.4.sql` & `pypgstac-0.7.7/pypgstac/migrations/pgstac.0.7.3-0.7.4.sql`

 * *Files identical despite different names*

### Comparing `pypgstac-0.7.6/pypgstac/migrations/pgstac.0.7.3.sql` & `pypgstac-0.7.7/pypgstac/migrations/pgstac.0.7.3.sql`

 * *Files identical despite different names*

### Comparing `pypgstac-0.7.6/pypgstac/migrations/pgstac.0.7.4-0.7.5.sql` & `pypgstac-0.7.7/pypgstac/migrations/pgstac.0.7.4-0.7.5.sql`

 * *Files 0% similar despite different names*

```diff
@@ -1029,9 +1029,9 @@
 GRANT SELECT ON ALL TABLES IN SCHEMA pgstac TO pgstac_read;
 
 
 GRANT EXECUTE ON ALL FUNCTIONS IN SCHEMA pgstac to pgstac_ingest;
 GRANT ALL ON ALL TABLES IN SCHEMA pgstac to pgstac_ingest;
 GRANT USAGE ON ALL SEQUENCES IN SCHEMA pgstac to pgstac_ingest;
 
-SELECT update_partition_stats_q(partition) FROM partitions;
+SELECT update_partition_stats_q(partition) FROM partitions_view;
 SELECT set_version('0.7.5');
```

### Comparing `pypgstac-0.7.6/pypgstac/migrations/pgstac.0.7.4.sql` & `pypgstac-0.7.7/pypgstac/migrations/pgstac.0.7.4.sql`

 * *Files identical despite different names*

### Comparing `pypgstac-0.7.6/pypgstac/migrations/pgstac.0.7.5-0.7.6.sql` & `pypgstac-0.7.7/pypgstac/migrations/pgstac.0.7.5-0.7.6.sql`

 * *Files 1% similar despite different names*

```diff
@@ -294,9 +294,9 @@
 GRANT SELECT ON ALL TABLES IN SCHEMA pgstac TO pgstac_read;
 
 
 GRANT EXECUTE ON ALL FUNCTIONS IN SCHEMA pgstac to pgstac_ingest;
 GRANT ALL ON ALL TABLES IN SCHEMA pgstac to pgstac_ingest;
 GRANT USAGE ON ALL SEQUENCES IN SCHEMA pgstac to pgstac_ingest;
 
-SELECT update_partition_stats_q(partition) FROM partitions;
+SELECT update_partition_stats_q(partition) FROM partitions_view;
 SELECT set_version('0.7.6');
```

### Comparing `pypgstac-0.7.6/pypgstac/migrations/pgstac.0.7.5.sql` & `pypgstac-0.7.7/pypgstac/migrations/pgstac.0.7.5.sql`

 * *Files 0% similar despite different names*

```diff
@@ -4010,9 +4010,9 @@
 GRANT SELECT ON ALL TABLES IN SCHEMA pgstac TO pgstac_read;
 
 
 GRANT EXECUTE ON ALL FUNCTIONS IN SCHEMA pgstac to pgstac_ingest;
 GRANT ALL ON ALL TABLES IN SCHEMA pgstac to pgstac_ingest;
 GRANT USAGE ON ALL SEQUENCES IN SCHEMA pgstac to pgstac_ingest;
 
-SELECT update_partition_stats_q(partition) FROM partitions;
+SELECT update_partition_stats_q(partition) FROM partitions_view;
 SELECT set_version('0.7.5');
```

### Comparing `pypgstac-0.7.6/pypgstac/migrations/pgstac.0.7.6.sql` & `pypgstac-0.7.7/pypgstac/migrations/pgstac.0.7.6.sql`

 * *Files 0% similar despite different names*

```diff
@@ -4010,9 +4010,9 @@
 GRANT SELECT ON ALL TABLES IN SCHEMA pgstac TO pgstac_read;
 
 
 GRANT EXECUTE ON ALL FUNCTIONS IN SCHEMA pgstac to pgstac_ingest;
 GRANT ALL ON ALL TABLES IN SCHEMA pgstac to pgstac_ingest;
 GRANT USAGE ON ALL SEQUENCES IN SCHEMA pgstac to pgstac_ingest;
 
-SELECT update_partition_stats_q(partition) FROM partitions;
+SELECT update_partition_stats_q(partition) FROM partitions_view;
 SELECT set_version('0.7.6');
```

### Comparing `pypgstac-0.7.6/pyproject.toml` & `pypgstac-0.7.7/pyproject.toml`

 * *Files identical despite different names*

### Comparing `pypgstac-0.7.6/PKG-INFO` & `pypgstac-0.7.7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pypgstac
-Version: 0.7.6
+Version: 0.7.7
 Summary: Schema, functions and a python library for storing and accessing STAC collections and items in PostgreSQL
 Project-URL: Homepage, https://stac-utils.github.io/pgstac/
 Project-URL: Documentation, https://stac-utils.github.io/pgstac/
 Project-URL: Issues, https://github.com/stac-utils/pgstac/issues
 Project-URL: Source, https://github.com/stac-utils/pgstac
 Project-URL: Changelog, https://stac-utils.github.io/pgstac/release-notes/
 Author-email: David Bitner <bitner@dbspatial.com>
```

