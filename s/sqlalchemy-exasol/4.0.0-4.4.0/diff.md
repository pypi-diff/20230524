# Comparing `tmp/sqlalchemy_exasol-4.0.0.tar.gz` & `tmp/sqlalchemy_exasol-4.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sqlalchemy_exasol-4.0.0.tar", max compression
+gzip compressed data, was "sqlalchemy_exasol-4.4.0.tar", max compression
```

## Comparing `sqlalchemy_exasol-4.0.0.tar` & `sqlalchemy_exasol-4.4.0.tar`

### file list

```diff
@@ -1,14 +1,14 @@
--rw-r--r--   0        0        0    13009 2022-12-01 10:39:57.772348 sqlalchemy_exasol-4.0.0/CHANGELOG.rst
--rw-r--r--   0        0        0     1395 2022-12-01 10:39:57.772348 sqlalchemy_exasol-4.0.0/LICENSE
--rw-r--r--   0        0        0     4979 2022-12-01 10:39:57.772348 sqlalchemy_exasol-4.0.0/README.rst
--rw-r--r--   0        0        0     3348 2022-12-01 10:39:57.828352 sqlalchemy_exasol-4.0.0/pyproject.toml
--rw-r--r--   0        0        0      413 2022-12-01 10:39:57.828352 sqlalchemy_exasol-4.0.0/sqlalchemy_exasol/__init__.py
--rw-r--r--   0        0        0    35498 2022-12-01 10:39:57.832352 sqlalchemy_exasol-4.0.0/sqlalchemy_exasol/base.py
--rw-r--r--   0        0        0      166 2022-12-01 10:39:57.832352 sqlalchemy_exasol-4.0.0/sqlalchemy_exasol/constraints.py
--rw-r--r--   0        0        0    12880 2022-12-01 10:39:57.832352 sqlalchemy_exasol-4.0.0/sqlalchemy_exasol/pyodbc.py
--rw-r--r--   0        0        0     7522 2022-12-01 10:39:57.832352 sqlalchemy_exasol-4.0.0/sqlalchemy_exasol/requirements.py
--rw-r--r--   0        0        0     5130 2022-12-01 10:39:57.832352 sqlalchemy_exasol-4.0.0/sqlalchemy_exasol/turbodbc.py
--rw-r--r--   0        0        0     1646 2022-12-01 10:39:57.832352 sqlalchemy_exasol-4.0.0/sqlalchemy_exasol/util.py
--rw-r--r--   0        0        0      235 2022-12-01 10:39:57.832352 sqlalchemy_exasol-4.0.0/sqlalchemy_exasol/version.py
--rw-r--r--   0        0        0     6187 1970-01-01 00:00:00.000000 sqlalchemy_exasol-4.0.0/setup.py
--rw-r--r--   0        0        0     6939 1970-01-01 00:00:00.000000 sqlalchemy_exasol-4.0.0/PKG-INFO
+-rw-r--r--   0        0        0    14389 2023-05-16 06:24:15.278817 sqlalchemy_exasol-4.4.0/CHANGELOG.rst
+-rw-r--r--   0        0        0     1395 2023-05-16 06:24:15.278817 sqlalchemy_exasol-4.4.0/LICENSE
+-rw-r--r--   0        0        0     5119 2023-05-16 06:24:15.278817 sqlalchemy_exasol-4.4.0/README.rst
+-rw-r--r--   0        0        0     3341 2023-05-16 06:24:15.334818 sqlalchemy_exasol-4.4.0/pyproject.toml
+-rw-r--r--   0        0        0      413 2023-05-16 06:24:15.334818 sqlalchemy_exasol-4.4.0/sqlalchemy_exasol/__init__.py
+-rw-r--r--   0        0        0    33000 2023-05-16 06:24:15.334818 sqlalchemy_exasol-4.4.0/sqlalchemy_exasol/base.py
+-rw-r--r--   0        0        0      165 2023-05-16 06:24:15.334818 sqlalchemy_exasol-4.4.0/sqlalchemy_exasol/constraints.py
+-rw-r--r--   0        0        0    12880 2023-05-16 06:24:15.334818 sqlalchemy_exasol-4.4.0/sqlalchemy_exasol/pyodbc.py
+-rw-r--r--   0        0        0     7522 2023-05-16 06:24:15.334818 sqlalchemy_exasol-4.4.0/sqlalchemy_exasol/requirements.py
+-rw-r--r--   0        0        0     5130 2023-05-16 06:24:15.334818 sqlalchemy_exasol-4.4.0/sqlalchemy_exasol/turbodbc.py
+-rw-r--r--   0        0        0     1646 2023-05-16 06:24:15.334818 sqlalchemy_exasol-4.4.0/sqlalchemy_exasol/util.py
+-rw-r--r--   0        0        0      235 2023-05-16 06:24:15.334818 sqlalchemy_exasol-4.4.0/sqlalchemy_exasol/version.py
+-rw-r--r--   0        0        0     6371 1970-01-01 00:00:00.000000 sqlalchemy_exasol-4.4.0/setup.py
+-rw-r--r--   0        0        0     7117 1970-01-01 00:00:00.000000 sqlalchemy_exasol-4.4.0/PKG-INFO
```

### Comparing `sqlalchemy_exasol-4.0.0/CHANGELOG.rst` & `sqlalchemy_exasol-4.4.0/CHANGELOG.rst`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,57 @@
+.. _changelog-unreleased:
 
+Unreleased
+==========
+
+.. _changelog-4.4.0:
+
+4.4.0 — 2023-05-16
+==================
+
+ **🚨 Attention:**
+
+    The turbodbc dependency was pinned to *4.5.4* due to issues with newer versions.
+
+    Failing tests in the SQLA compliance test suite, in regard to the turbodbc dialect
+    won't be addressed until explicitly required/requested by users.
+
+    Note: It is also very likely that turbodbc support will be dropped in future versions.
+
+🐞 Fixed
+--------
+
+* Fixed invalid implicit autocommit behaviour, for details see `<Issue-https://github.com/exasol/sqlalchemy-exasol/issues/335>`_
+
+✨ Added
+--------
+
+* Added websocket based dbapi2 compliant database driver
+
+🔧 Changed
+----------
+
+* Updated pytest
+* Updated Dependencies
+* Loosened version constraints on 'packaging' dependency
+* Loosened dev dependency constraints
+
+🧰 Internal
+-----------
+* Changed changelog workflow
+
+    - Removed scriv
+    - Added unreleased section to track unreleased changes
+
+* Simplified workflows by factoring out python & poetry setup into an action
+* Added a internal category to the changelog fragment template
+* Added manual trigger for the gh-pages workflow
+* Removed workaround for outdated DB versions
+  (for further details see https://github.com/exasol/sqlalchemy-exasol/issues/5)
+* Added exasol-integration-test-docker-environment as dev dependency
 
 .. _changelog-4.0.0:
 
 4.0.0 — 2022-12-01
 ==================
 
 ✨ Added
```

### Comparing `sqlalchemy_exasol-4.0.0/LICENSE` & `sqlalchemy_exasol-4.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `sqlalchemy_exasol-4.0.0/README.rst` & `sqlalchemy_exasol-4.4.0/README.rst`

 * *Files 6% similar despite different names*

```diff
@@ -59,14 +59,18 @@
 - The packages unixODBC and unixODBC-dev >= 2.2.14
 - The Exasol `ODBC driver <odbc_driver_>`_
 - The ODBC.ini and ODBCINST.ini configurations files setup
 
 Turbodbc support
 ````````````````
 
+.. warning::
+
+    Maintenance of this feature is on hold. Also it is very likely that turbodbc support will be dropped in future versions.
+
 - You can use Turbodbc with sqlalchemy_exasol if you use a python version >= 3.8.
 - Multi row update is not supported, see
   `test/test_update.py <test/test_update.py>`_ for an example
 
 
 Setup your python project and install sqlalchemy-exasol
 ```````````````````````````````````````````````````````
```

### Comparing `sqlalchemy_exasol-4.0.0/pyproject.toml` & `sqlalchemy_exasol-4.4.0/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 requires = [
     "poetry>=1.0.0",
 ]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
 name = "sqlalchemy_exasol"
-version = "4.0.0"
+version = "4.4.0"
 description = "EXASOL dialect for SQLAlchemy"
 readme = "README.rst"
 authors = [
     "Exasol AG <opensource@exasol.com>",
     "Blue Yonder GmbH",
 ]
 license = "BSD"
@@ -49,52 +49,57 @@
 
 [tool.poetry.urls]
 "Homepage" = "https://www.exasol.com/"
 "Documentation" = "https://exasol.github.io/sqlalchemy-exasol/"
 "Source" = "https://github.com/exasol/sqlalchemy-exasol"
 "Issues" = "https://github.com/exasol/sqlalchemy-exasol/issues"
 "Changelog" = "https://exasol.github.io/sqlalchemy-exasol/changelog.html"
-"Github" = "https://github.com/exasol/sqlalchemy-exasol"
 
 
 [tool.poetry.dependencies]
 python = ">=3.8,<4.0"
-SQLAlchemy = ">=1.4"
-pyodbc = ">=4.0.34"
-packaging = "^21.3"
-turbodbc = { version = ">=4.5.4", optional = true }
+pyodbc = "^4.0.34"
+packaging = ">=21.3"
+pyexasol = "^0.25.1"
+sqlalchemy = ">=1.4,<1.4.45"
+
+[tool.poetry.dependencies.turbodbc]
+version = "==4.5.4"
+optional = true
 
-[tool.poetry.dev-dependencies]
+[tool.poetry.group.dev.dependencies]
 nox = ">=2022.1.7"
 urlscan = ">=0.9.9"
 pytest-json-report = ">=1.5.0"
 # The excluded versions mirror the excluded versions of sqla 1.3.X.
 # The limitation/issue pytest <6 is tracked in https://github.com/exasol/sqlalchemy-exasol/issues/144
-pytest = ">=6,<7"
+pytest = ">=6"
 pytest-cov = ">=2.7.0"
-pre-commit = "^2.19.0"
-black = "^22.6.0"
+pre-commit = ">=2.19.0"
+black = ">=22.6.0"
 isort = "^5.10.1"
 pylint = "^2.14.5"
-scriv = "^0.16.0"
-Sphinx = "^5.1.1"
+Sphinx = ">=6"
 furo = "^2022.6.21"
 sphinx-copybutton = "^0.5.0"
-mypy = "^0.982"
-pyupgrade = "^3.0.0"
+mypy = ">=0.982"
+pyupgrade = ">=3.0.0"
+rich = "^13.3.1"
+exasol-integration-test-docker-environment = "^1.5.0"
 
 [tool.poetry.extras]
 turbodbc = ["turbodbc"]
 
 [tool.poetry.plugins."sqlalchemy.dialects"]
 "exa.pyodbc" = "sqlalchemy_exasol.pyodbc:EXADialect_pyodbc"
 "exa.turbodbc" = "sqlalchemy_exasol.turbodbc:EXADialect_turbodbc"
 
+
 [tool.pytest.ini_options]
-addopts = "--tb native -v -r fxX --log-debug=sqlalchemy.engine --log-debug=sqlalchemy.pool"
+addopts = "--tb native -v -r fxX"
 filterwarnings = [
     "error::DeprecationWarning",
     "ignore::DeprecationWarning:sqlalchemy.testing.plugin.*",
 ]
 
 [tool.black]
 line-length = 88
@@ -102,15 +107,15 @@
 include = "\\.pyi?$"
 
 [tool.isort]
 profile = "black"
 force_grid_wrap = 2
 
 [tool.pylint.master]
-fail-under = 5.6
+fail-under = 5.5
 
 [tool.pylint.format]
 max-line-length = 88
 max-module-lines = 800
 
 [tool.mypy]
 files = [
```

### Comparing `sqlalchemy_exasol-4.0.0/sqlalchemy_exasol/base.py` & `sqlalchemy_exasol-4.4.0/sqlalchemy_exasol/base.py`

 * *Files 4% similar despite different names*

```diff
@@ -43,14 +43,15 @@
 dialect takes care of converting them to the internal case insensitive
 representation (all uppercase).
 
 """
 
 import logging
 import re
+from contextlib import closing
 from datetime import (
     date,
     datetime,
 )
 from decimal import Decimal
 
 import sqlalchemy.exc
@@ -746,73 +747,19 @@
                 "WHERE column_object_type = 'TABLE' and column_table",
                 "= ? AND column_name = ?",
             )
         )
         sql_stmnt += " AND column_schema = ?" if schema else ""
         args = (table, id_col, schema) if schema else (table, id_col)
 
-        with self.create_cursor() as cursor:
+        with closing(self.create_cursor()) as cursor:
             cursor.execute(sql_stmnt, args)
             result = cursor.fetchone()
             return int(result[0]) - 1
 
-    def pre_exec(self):
-        """
-        This routine inserts the parameters into the compiled query prior to executing it.
-        The reason for this workaround is the poor performance for prepared statements.
-        Note: Parameter replacement is done for server versions < 4.1.8 or
-              in case a delete query is executed.
-        """
-        server_version = self.root_connection.dialect.server_version_info
-        # FIXME: drop exasol verison support < 4.1.0
-        # see https://github.com/exasol/sqlalchemy-exasol/pull/191#discussion_r942595818
-        skip_pre_exec = (
-            not self.isdelete and server_version is None or server_version >= (4, 1, 8)
-        )
-        if skip_pre_exec:
-            return
-
-        db_query = self.unicode_statement
-        for i in range(1, len(self.parameters)):
-            db_query += ", (" + ", ".join(["?"] * len(self.parameters[i])) + ")"
-        for db_para in self.parameters:
-            for value in db_para:
-                ident = "?"
-                if value is None:
-                    db_query = db_query.replace(ident, "NULL", 1)
-                elif isinstance(value, int):
-                    db_query = db_query.replace(ident, str(value), 1)
-                elif isinstance(value, (float, Decimal)):
-                    db_query = db_query.replace(ident, str(float(value)), 1)
-                elif isinstance(value, bool):
-                    db_query = db_query.replace(ident, "1" if value else "0", 1)
-                elif isinstance(value, datetime):
-                    db_query = db_query.replace(
-                        ident,
-                        "to_timestamp('%s', 'YYYY-MM-DD HH24:MI:SS.FF6')"
-                        % value.strftime("%Y-%m-%d %H:%M:%S.%f"),
-                        1,
-                    )
-                elif isinstance(value, date):
-                    db_query = db_query.replace(
-                        ident,
-                        "to_date('%s', 'YYYY-MM-DD')" % value.strftime("%Y-%m-%d"),
-                        1,
-                    )
-                elif isinstance(value, bytes):
-                    db_query = db_query.replace(
-                        ident, "'%s'" % value.decode("UTF-8"), 1
-                    )
-                elif isinstance(value, str):
-                    db_query = db_query.replace(ident, "'%s'" % value, 1)
-                else:
-                    raise TypeError("Data type not supported: %s" % type(value))
-        self.statement = db_query
-        self.parameters = [[]]
-
     def should_autocommit_text(self, statement):
         return AUTOCOMMIT_REGEXP.match(statement)
 
 
 class EXADialect(default.DefaultDialect):
     name = "exasol"
     max_identifier_length = 128
```

### Comparing `sqlalchemy_exasol-4.0.0/sqlalchemy_exasol/pyodbc.py` & `sqlalchemy_exasol-4.4.0/sqlalchemy_exasol/pyodbc.py`

 * *Files identical despite different names*

### Comparing `sqlalchemy_exasol-4.0.0/sqlalchemy_exasol/requirements.py` & `sqlalchemy_exasol-4.4.0/sqlalchemy_exasol/requirements.py`

 * *Files identical despite different names*

### Comparing `sqlalchemy_exasol-4.0.0/sqlalchemy_exasol/turbodbc.py` & `sqlalchemy_exasol-4.4.0/sqlalchemy_exasol/turbodbc.py`

 * *Files identical despite different names*

### Comparing `sqlalchemy_exasol-4.0.0/sqlalchemy_exasol/util.py` & `sqlalchemy_exasol-4.4.0/sqlalchemy_exasol/util.py`

 * *Files identical despite different names*

### Comparing `sqlalchemy_exasol-4.0.0/setup.py` & `sqlalchemy_exasol-4.4.0/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -4,30 +4,33 @@
 packages = \
 ['sqlalchemy_exasol']
 
 package_data = \
 {'': ['*']}
 
 install_requires = \
-['SQLAlchemy>=1.4', 'packaging>=21.3,<22.0', 'pyodbc>=4.0.34']
+['packaging>=21.3',
+ 'pyexasol>=0.25.1,<0.26.0',
+ 'pyodbc>=4.0.34,<5.0.0',
+ 'sqlalchemy>=1.4,<1.4.45']
 
 extras_require = \
-{'turbodbc': ['turbodbc>=4.5.4']}
+{'turbodbc': ['turbodbc==4.5.4']}
 
 entry_points = \
 {'sqlalchemy.dialects': ['exa.pyodbc = '
                          'sqlalchemy_exasol.pyodbc:EXADialect_pyodbc',
                          'exa.turbodbc = '
                          'sqlalchemy_exasol.turbodbc:EXADialect_turbodbc']}
 
 setup_kwargs = {
     'name': 'sqlalchemy-exasol',
-    'version': '4.0.0',
+    'version': '4.4.0',
     'description': 'EXASOL dialect for SQLAlchemy',
-    'long_description': 'SQLAlchemy Dialect for EXASOL DB\n================================\n\n\n.. image:: https://github.com/exasol/sqlalchemy_exasol/workflows/CI/badge.svg?branch=master\n    :target: https://github.com/exasol/sqlalchemy_exasol/actions?query=workflow%3ACI\n     :alt: CI Status\n\n.. image:: https://img.shields.io/pypi/v/sqlalchemy_exasol\n     :target: https://pypi.org/project/sqlalchemy-exasol/\n     :alt: PyPI Version\n\n.. image:: https://img.shields.io/pypi/pyversions/sqlalchemy-exasol\n    :target: https://pypi.org/project/sqlalchemy-exasol\n    :alt: PyPI - Python Version\n\n.. image:: https://img.shields.io/badge/exasol-7.1.9%20%7C%207.0.18-green\n    :target: https://www.exasol.com/\n    :alt: Exasol - Supported Version(s)\n\n.. image:: https://img.shields.io/badge/code%20style-black-000000.svg\n    :target: https://github.com/psf/black\n    :alt: Formatter - Black\n\n.. image:: https://img.shields.io/badge/imports-isort-ef8336.svg\n    :target: https://pycqa.github.io/isort/\n    :alt: Formatter - Isort\n\n.. image:: https://img.shields.io/badge/pylint-5.8-yellow\n    :target: https://github.com/PyCQA/pylint\n    :alt: Pylint\n\n.. image:: https://img.shields.io/pypi/l/sqlalchemy-exasol\n     :target: https://opensource.org/licenses/BSD-2-Clause\n     :alt: License\n\n.. image:: https://img.shields.io/github/last-commit/exasol/sqlalchemy-exasol\n     :target: https://pypi.org/project/sqlalchemy-exasol/\n     :alt: Last Commit\n\n.. image:: https://img.shields.io/pypi/dm/sqlalchemy-exasol\n    :target: https://pypi.org/project/sqlalchemy-exasol\n    :alt: PyPI - Downloads\n\n\nHow to get started\n------------------\n\nWe assume you have a good understanding of (unix)ODBC. If not, make sure you\nread their documentation carefully - there are lot\'s of traps \U0001faa4 to step into.\n\nMeet the system requirements\n````````````````````````````\n\nOn Linux/Unix like systems you need:\n\n- Python\n- An Exasol DB (e.g. `docker-db <test_docker_image_>`_ or a `cloud instance <test_drive_>`_)\n- The packages unixODBC and unixODBC-dev >= 2.2.14\n- The Exasol `ODBC driver <odbc_driver_>`_\n- The ODBC.ini and ODBCINST.ini configurations files setup\n\nTurbodbc support\n````````````````\n\n- You can use Turbodbc with sqlalchemy_exasol if you use a python version >= 3.8.\n- Multi row update is not supported, see\n  `test/test_update.py <test/test_update.py>`_ for an example\n\n\nSetup your python project and install sqlalchemy-exasol\n```````````````````````````````````````````````````````\n\n.. code-block:: shell\n\n    $ pip install sqlalchemy-exasol\n\nfor turbodbc support:\n\n.. code-block:: shell\n\n    $ pip install sqlalchemy-exasol[turbodbc]\n\nTalk to the EXASOL DB using SQLAlchemy\n``````````````````````````````````````\n\n.. code-block:: python\n\n\tfrom sqlalchemy import create_engine\n\turl = "exa+pyodbc://A_USER:A_PASSWORD@192.168.1.2..8:1234/my_schema?CONNECTIONLCALL=en_US.UTF-8&driver=EXAODBC"\n\te = create_engine(url)\n\tr = e.execute("select 42 from dual").fetchall()\n\nto use turbodbc as driver:\n\n.. code-block:: python\n\n\tfrom sqlalchemy import create_engine\n\turl = "exa+turbodbc://A_USER:A_PASSWORD@192.168.1.2..8:1234/my_schema?CONNECTIONLCALL=en_US.UTF-8&driver=EXAODBC"\n\te = create_engine(url)\n\tr = e.execute("select 42 from dual").fetchall()\n\n\nThe dialect supports two types of connection urls creating an engine. A DSN (Data Source Name) mode and a host mode:\n\n.. list-table::\n\n   * - Type\n     - Example\n   * - DSN URL\n     - \'exa+pyodbc://USER:PWD@exa_test\'\n   * - HOST URL\n     - \'exa+pyodbc://USER:PWD@192.168.14.227..228:1234/my_schema?parameter\'\n\nFeatures\n++++++++\n\n- SELECT, INSERT, UPDATE, DELETE statements\n- you can even use the MERGE statement (see unit tests for examples)\n\nNotes\n+++++\n\n- Schema name and parameters are optional for the host url\n- At least on Linux/Unix systems it has proven valuable to pass \'CONNECTIONLCALL=en_US.UTF-8\' as a url parameter. This will make sure that the client process (Python) and the EXASOL driver (UTF-8 internal) know how to interpret code pages correctly.\n- Always use all lower-case identifiers for schema, table and column names. SQLAlchemy treats all lower-case identifiers as case-insensitive, the dialect takes care of transforming the identifier into a case-insensitive representation of the specific database (in case of EXASol this is upper-case as for Oracle)\n- As of Exasol client driver version 4.1.2 you can pass the flag \'INTTYPESINRESULTSIFPOSSIBLE=y\' in the connection string (or configure it in your DSN). This will convert DECIMAL data types to Integer-like data types. Creating integers is a factor three faster in Python than creating Decimals.\n\n.. _developer guide: https://github.com/exasol/sqlalchemy-exasol/blob/master/doc/developer_guide/developer_guide.rst\n.. _odbc_driver: https://docs.exasol.com/db/latest/connect_exasol/drivers/odbc/odbc_linux.htm\n.. _test_drive: https://www.exasol.com/test-it-now/cloud/\n.. _test_docker_image: https://github.com/exasol/docker-db\n\nDevelopment & Testing\n`````````````````````\nSee `developer guide`_\n\n',
+    'long_description': 'SQLAlchemy Dialect for EXASOL DB\n================================\n\n\n.. image:: https://github.com/exasol/sqlalchemy_exasol/workflows/CI/badge.svg?branch=master\n    :target: https://github.com/exasol/sqlalchemy_exasol/actions?query=workflow%3ACI\n     :alt: CI Status\n\n.. image:: https://img.shields.io/pypi/v/sqlalchemy_exasol\n     :target: https://pypi.org/project/sqlalchemy-exasol/\n     :alt: PyPI Version\n\n.. image:: https://img.shields.io/pypi/pyversions/sqlalchemy-exasol\n    :target: https://pypi.org/project/sqlalchemy-exasol\n    :alt: PyPI - Python Version\n\n.. image:: https://img.shields.io/badge/exasol-7.1.9%20%7C%207.0.18-green\n    :target: https://www.exasol.com/\n    :alt: Exasol - Supported Version(s)\n\n.. image:: https://img.shields.io/badge/code%20style-black-000000.svg\n    :target: https://github.com/psf/black\n    :alt: Formatter - Black\n\n.. image:: https://img.shields.io/badge/imports-isort-ef8336.svg\n    :target: https://pycqa.github.io/isort/\n    :alt: Formatter - Isort\n\n.. image:: https://img.shields.io/badge/pylint-5.8-yellow\n    :target: https://github.com/PyCQA/pylint\n    :alt: Pylint\n\n.. image:: https://img.shields.io/pypi/l/sqlalchemy-exasol\n     :target: https://opensource.org/licenses/BSD-2-Clause\n     :alt: License\n\n.. image:: https://img.shields.io/github/last-commit/exasol/sqlalchemy-exasol\n     :target: https://pypi.org/project/sqlalchemy-exasol/\n     :alt: Last Commit\n\n.. image:: https://img.shields.io/pypi/dm/sqlalchemy-exasol\n    :target: https://pypi.org/project/sqlalchemy-exasol\n    :alt: PyPI - Downloads\n\n\nHow to get started\n------------------\n\nWe assume you have a good understanding of (unix)ODBC. If not, make sure you\nread their documentation carefully - there are lot\'s of traps \U0001faa4 to step into.\n\nMeet the system requirements\n````````````````````````````\n\nOn Linux/Unix like systems you need:\n\n- Python\n- An Exasol DB (e.g. `docker-db <test_docker_image_>`_ or a `cloud instance <test_drive_>`_)\n- The packages unixODBC and unixODBC-dev >= 2.2.14\n- The Exasol `ODBC driver <odbc_driver_>`_\n- The ODBC.ini and ODBCINST.ini configurations files setup\n\nTurbodbc support\n````````````````\n\n.. warning::\n\n    Maintenance of this feature is on hold. Also it is very likely that turbodbc support will be dropped in future versions.\n\n- You can use Turbodbc with sqlalchemy_exasol if you use a python version >= 3.8.\n- Multi row update is not supported, see\n  `test/test_update.py <test/test_update.py>`_ for an example\n\n\nSetup your python project and install sqlalchemy-exasol\n```````````````````````````````````````````````````````\n\n.. code-block:: shell\n\n    $ pip install sqlalchemy-exasol\n\nfor turbodbc support:\n\n.. code-block:: shell\n\n    $ pip install sqlalchemy-exasol[turbodbc]\n\nTalk to the EXASOL DB using SQLAlchemy\n``````````````````````````````````````\n\n.. code-block:: python\n\n\tfrom sqlalchemy import create_engine\n\turl = "exa+pyodbc://A_USER:A_PASSWORD@192.168.1.2..8:1234/my_schema?CONNECTIONLCALL=en_US.UTF-8&driver=EXAODBC"\n\te = create_engine(url)\n\tr = e.execute("select 42 from dual").fetchall()\n\nto use turbodbc as driver:\n\n.. code-block:: python\n\n\tfrom sqlalchemy import create_engine\n\turl = "exa+turbodbc://A_USER:A_PASSWORD@192.168.1.2..8:1234/my_schema?CONNECTIONLCALL=en_US.UTF-8&driver=EXAODBC"\n\te = create_engine(url)\n\tr = e.execute("select 42 from dual").fetchall()\n\n\nThe dialect supports two types of connection urls creating an engine. A DSN (Data Source Name) mode and a host mode:\n\n.. list-table::\n\n   * - Type\n     - Example\n   * - DSN URL\n     - \'exa+pyodbc://USER:PWD@exa_test\'\n   * - HOST URL\n     - \'exa+pyodbc://USER:PWD@192.168.14.227..228:1234/my_schema?parameter\'\n\nFeatures\n++++++++\n\n- SELECT, INSERT, UPDATE, DELETE statements\n- you can even use the MERGE statement (see unit tests for examples)\n\nNotes\n+++++\n\n- Schema name and parameters are optional for the host url\n- At least on Linux/Unix systems it has proven valuable to pass \'CONNECTIONLCALL=en_US.UTF-8\' as a url parameter. This will make sure that the client process (Python) and the EXASOL driver (UTF-8 internal) know how to interpret code pages correctly.\n- Always use all lower-case identifiers for schema, table and column names. SQLAlchemy treats all lower-case identifiers as case-insensitive, the dialect takes care of transforming the identifier into a case-insensitive representation of the specific database (in case of EXASol this is upper-case as for Oracle)\n- As of Exasol client driver version 4.1.2 you can pass the flag \'INTTYPESINRESULTSIFPOSSIBLE=y\' in the connection string (or configure it in your DSN). This will convert DECIMAL data types to Integer-like data types. Creating integers is a factor three faster in Python than creating Decimals.\n\n.. _developer guide: https://github.com/exasol/sqlalchemy-exasol/blob/master/doc/developer_guide/developer_guide.rst\n.. _odbc_driver: https://docs.exasol.com/db/latest/connect_exasol/drivers/odbc/odbc_linux.htm\n.. _test_drive: https://www.exasol.com/test-it-now/cloud/\n.. _test_docker_image: https://github.com/exasol/docker-db\n\nDevelopment & Testing\n`````````````````````\nSee `developer guide`_\n\n',
     'author': 'Exasol AG',
     'author_email': 'opensource@exasol.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'None',
     'packages': packages,
     'package_data': package_data,
```

### Comparing `sqlalchemy_exasol-4.0.0/PKG-INFO` & `sqlalchemy_exasol-4.4.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sqlalchemy-exasol
-Version: 4.0.0
+Version: 4.4.0
 Summary: EXASOL dialect for SQLAlchemy
 License: BSD
 Keywords: exasol,sql,sqlalchemy,data science,database
 Author: Exasol AG
 Author-email: opensource@exasol.com
 Requires-Python: >=3.8,<4.0
 Classifier: Development Status :: 5 - Production/Stable
@@ -13,33 +13,34 @@
 Classifier: Intended Audience :: Information Technology
 Classifier: License :: Other/Proprietary License
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: SQL
 Classifier: Topic :: Database
 Classifier: Topic :: Scientific/Engineering :: Information Analysis
 Classifier: Topic :: Software Development
 Classifier: Topic :: Software Development :: Libraries
 Classifier: Topic :: Software Development :: Libraries :: Application Frameworks
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Provides-Extra: turbodbc
-Requires-Dist: SQLAlchemy (>=1.4)
-Requires-Dist: packaging (>=21.3,<22.0)
-Requires-Dist: pyodbc (>=4.0.34)
-Requires-Dist: turbodbc (>=4.5.4); extra == "turbodbc"
+Requires-Dist: packaging (>=21.3)
+Requires-Dist: pyexasol (>=0.25.1,<0.26.0)
+Requires-Dist: pyodbc (>=4.0.34,<5.0.0)
+Requires-Dist: sqlalchemy (>=1.4,<1.4.45)
+Requires-Dist: turbodbc (==4.5.4); extra == "turbodbc"
 Project-URL: Changelog, https://exasol.github.io/sqlalchemy-exasol/changelog.html
 Project-URL: Documentation, https://exasol.github.io/sqlalchemy-exasol/
-Project-URL: Github, https://github.com/exasol/sqlalchemy-exasol
 Project-URL: Homepage, https://www.exasol.com/
 Project-URL: Issues, https://github.com/exasol/sqlalchemy-exasol/issues
 Project-URL: Source, https://github.com/exasol/sqlalchemy-exasol
 Description-Content-Type: text/x-rst
 
 SQLAlchemy Dialect for EXASOL DB
 ================================
@@ -102,14 +103,18 @@
 - The packages unixODBC and unixODBC-dev >= 2.2.14
 - The Exasol `ODBC driver <odbc_driver_>`_
 - The ODBC.ini and ODBCINST.ini configurations files setup
 
 Turbodbc support
 ````````````````
 
+.. warning::
+
+    Maintenance of this feature is on hold. Also it is very likely that turbodbc support will be dropped in future versions.
+
 - You can use Turbodbc with sqlalchemy_exasol if you use a python version >= 3.8.
 - Multi row update is not supported, see
   `test/test_update.py <test/test_update.py>`_ for an example
 
 
 Setup your python project and install sqlalchemy-exasol
 ```````````````````````````````````````````````````````
```

