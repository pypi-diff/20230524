# Comparing `tmp/atomlite-1.1.2.tar.gz` & `tmp/atomlite-1.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "atomlite-1.1.2.tar", last modified: Sun May 21 13:59:11 2023, max compression
+gzip compressed data, was "atomlite-1.2.0.tar", last modified: Wed May 24 15:24:01 2023, max compression
```

## Comparing `atomlite-1.1.2.tar` & `atomlite-1.2.0.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-21 13:59:11.251789 atomlite-1.1.2/
--rw-r--r--   0 root         (0) root         (0)     1545 2023-05-21 13:59:11.251789 atomlite-1.1.2/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1230 2023-05-21 13:59:00.000000 atomlite-1.1.2/README.rst
--rw-r--r--   0 root         (0) root         (0)     1156 2023-05-21 13:59:00.000000 atomlite-1.1.2/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)       38 2023-05-21 13:59:11.251789 atomlite-1.1.2/setup.cfg
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-21 13:59:11.251789 atomlite-1.1.2/src/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-21 13:59:11.251789 atomlite-1.1.2/src/atomlite/
--rw-r--r--   0 root         (0) root         (0)      410 2023-05-21 13:59:00.000000 atomlite-1.1.2/src/atomlite/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-21 13:59:11.251789 atomlite-1.1.2/src/atomlite/_internal/
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-21 13:59:00.000000 atomlite-1.1.2/src/atomlite/_internal/__init__.py
--rw-r--r--   0 root         (0) root         (0)     8351 2023-05-21 13:59:00.000000 atomlite-1.1.2/src/atomlite/_internal/database.py
--rw-r--r--   0 root         (0) root         (0)     5618 2023-05-21 13:59:00.000000 atomlite-1.1.2/src/atomlite/_internal/json.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-21 13:59:00.000000 atomlite-1.1.2/src/atomlite/py.typed
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-21 13:59:11.251789 atomlite-1.1.2/src/atomlite.egg-info/
--rw-r--r--   0 root         (0) root         (0)     1545 2023-05-21 13:59:11.000000 atomlite-1.1.2/src/atomlite.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      375 2023-05-21 13:59:11.000000 atomlite-1.1.2/src/atomlite.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-05-21 13:59:11.000000 atomlite-1.1.2/src/atomlite.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      105 2023-05-21 13:59:11.000000 atomlite-1.1.2/src/atomlite.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        9 2023-05-21 13:59:11.000000 atomlite-1.1.2/src/atomlite.egg-info/top_level.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-21 13:59:11.251789 atomlite-1.1.2/tests/
--rw-r--r--   0 root         (0) root         (0)     8089 2023-05-21 13:59:00.000000 atomlite-1.1.2/tests/test_database.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-24 15:24:01.492031 atomlite-1.2.0/
+-rw-r--r--   0 root         (0) root         (0)     1545 2023-05-24 15:24:01.492031 atomlite-1.2.0/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1230 2023-05-24 15:23:47.000000 atomlite-1.2.0/README.rst
+-rw-r--r--   0 root         (0) root         (0)     1156 2023-05-24 15:23:47.000000 atomlite-1.2.0/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)       38 2023-05-24 15:24:01.492031 atomlite-1.2.0/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-24 15:24:01.488031 atomlite-1.2.0/src/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-24 15:24:01.488031 atomlite-1.2.0/src/atomlite/
+-rw-r--r--   0 root         (0) root         (0)      473 2023-05-24 15:23:47.000000 atomlite-1.2.0/src/atomlite/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-24 15:24:01.492031 atomlite-1.2.0/src/atomlite/_internal/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-24 15:23:47.000000 atomlite-1.2.0/src/atomlite/_internal/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    11418 2023-05-24 15:23:47.000000 atomlite-1.2.0/src/atomlite/_internal/database.py
+-rw-r--r--   0 root         (0) root         (0)     5633 2023-05-24 15:23:47.000000 atomlite-1.2.0/src/atomlite/_internal/json.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-24 15:23:47.000000 atomlite-1.2.0/src/atomlite/py.typed
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-24 15:24:01.492031 atomlite-1.2.0/src/atomlite.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     1545 2023-05-24 15:24:01.000000 atomlite-1.2.0/src/atomlite.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      375 2023-05-24 15:24:01.000000 atomlite-1.2.0/src/atomlite.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-05-24 15:24:01.000000 atomlite-1.2.0/src/atomlite.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      105 2023-05-24 15:24:01.000000 atomlite-1.2.0/src/atomlite.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        9 2023-05-24 15:24:01.000000 atomlite-1.2.0/src/atomlite.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-24 15:24:01.492031 atomlite-1.2.0/tests/
+-rw-r--r--   0 root         (0) root         (0)    10139 2023-05-24 15:23:47.000000 atomlite-1.2.0/tests/test_database.py
```

### Comparing `atomlite-1.1.2/PKG-INFO` & `atomlite-1.2.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: atomlite
-Version: 1.1.2
+Version: 1.2.0
 Maintainer-email: Lukas Turcani <lukasturcani93@gmail.com>
 Project-URL: github, https://github.com/lukasturcani/atomlite
 Project-URL: documentation, https://atomlite.readthedocs.io
 Requires-Python: >=3.11
 Description-Content-Type: text/x-rst
 Provides-Extra: dev
```

### Comparing `atomlite-1.1.2/README.rst` & `atomlite-1.2.0/README.rst`

 * *Files identical despite different names*

### Comparing `atomlite-1.1.2/pyproject.toml` & `atomlite-1.2.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `atomlite-1.1.2/src/atomlite/_internal/database.py` & `atomlite-1.2.0/src/atomlite/_internal/database.py`

 * *Files 22% similar despite different names*

```diff
@@ -6,15 +6,14 @@
 from dataclasses import asdict, dataclass, field
 
 import rdkit.Chem as rdkit
 
 from atomlite._internal.json import Json, Molecule, json_from_rdkit
 
 Properties: typing.TypeAlias = dict[str, Json] | None
-DatabaseGetMolecules: typing.TypeAlias = collections.abc.Iterator["Entry"]
 
 
 @dataclass(frozen=True, slots=True)
 class Entry:
     """
     A database entry.
 
@@ -82,14 +81,22 @@
 
 def _property_entry_to_sqlite(entry: PropertyEntry) -> dict:
     d = asdict(entry)
     d["properties"] = json.dumps(d["properties"])
     return d
 
 
+class MoleculeNotFound(Exception):
+    """
+    Raised when a molecule is not found in the database.
+    """
+
+    pass
+
+
 class Database:
     """
     A molecular SQLite database.
     """
 
     connection: sqlite3.Connection
     """
@@ -186,15 +193,15 @@
             )
         if commit:
             self.connection.commit()
 
     def get_entries(
         self,
         keys: str | collections.abc.Iterable[str] | None = None,
-    ) -> "DatabaseGetMolecules":
+    ) -> collections.abc.Iterator[Entry]:
         """
         Get molecular entries from the database.
 
         .. tip::
 
             The molecules returned from the database are in JSON
             format, you may need to convert them to something more
@@ -204,15 +211,14 @@
         Parameters:
             keys (str | list[str] | None):
                 The keys of the molecules to retrieve from the
                 database. If ``None``, all entries will be returned.
         Yields:
             A molecular entry matching `keys`.
         """
-
         if keys is None:
             for key, molecule, properties in self.connection.execute(
                 f"SELECT * FROM {self._molecule_table}",
             ):
                 yield Entry(
                     key=key,
                     molecule=json.loads(molecule),
@@ -231,25 +237,116 @@
         ):
             yield Entry(
                 key=key,
                 molecule=json.loads(molecule),
                 properties=json.loads(properties),
             )
 
+    def get_property(
+        self,
+        key: str,
+        path: str,
+    ) -> "Json":
+        """
+        Get the property of a molecule.
+
+        .. note::
+
+            If `path` does not lead to a property which exists,
+            ``None`` will be returned. This means that the same
+            value is returned for a missing value as well as an
+            exisiting value set to ``None``. If you need to
+            distinguish between missing and ``None`` values you
+            can use a different value to represent missing data,
+            for example the string ``"MISSING"``.
+
+        Parameters:
+            key: The key of the molecule.
+            path:
+                A path to the property of the molecule. Valid
+                paths are described here_. You can also view various
+                code :ref:`examples<examples-valid-property-paths>`
+                in our docs.
+        Returns:
+            The property.
+        Raises:
+            MoleculeNotFound:
+                If the molecule is not found in the database.
+
+        .. _here: https://www.sqlite.org/json1.html#path_arguments
+        """
+        result = self.connection.execute(
+            "SELECT json_extract(properties,?), "
+            "json_type(properties,?) "
+            f"FROM {self._molecule_table} "
+            "WHERE key=?",
+            (path, path, key),
+        ).fetchone()
+        if result is None:
+            raise MoleculeNotFound(
+                "Can't get property of a molecule not in the database."
+            )
+        property, property_type = result
+        if property_type == "object" or property_type == "array":
+            return json.loads(property)
+        elif property_type == "true" or property_type == "false":
+            return bool(property)
+        else:
+            return property
+
+    def set_property(
+        self,
+        key: str,
+        path: str,
+        property: float | str | bool | None,
+        commit: bool = True,
+    ) -> None:
+        """
+        Set the property of molecule.
+
+        .. note::
+
+            If `key` does not exist in the database, this function
+            will finish successfully but it will not change the database.
+
+        Parameters:
+            key:
+                The key of the molecule.
+            path:
+                A path to the property of the molecule. Valid
+                paths are described here_. You can also view various
+                code :ref:`examples<examples-valid-property-paths>`
+                in our docs.
+            property:
+                The desired value of the property.
+            commit:
+                If ``True`` changes will be automatically
+                commited to the database file.
+        """
+        self.connection.execute(
+            f"UPDATE {self._molecule_table} "
+            "SET properties=json_set(properties,?,?) "
+            "WHERE key=?",
+            (path, property, key),
+        )
+
+        if commit:
+            self.connection.commit()
+
     def update_properties(
         self,
         entries: PropertyEntry | collections.abc.Iterable[PropertyEntry],
         merge_properties: bool = True,
         commit: bool = True,
     ) -> None:
         """
         Update molecular properties.
 
         Parameters:
-            entries (Entry | list[Entry]):
+            entries (PropertyEntry | list[PropertyEntry]):
                 The entries to update in the database.
             merge_properties:
                 If ``True``, the molecular properties will be
                 merged rather than replaced. Properties present
                 in both the update and the database will be
                 overwritten.
             commit:
```

### Comparing `atomlite-1.1.2/src/atomlite/_internal/json.py` & `atomlite-1.2.0/src/atomlite/_internal/json.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,14 @@
 import typing
 
 import rdkit.Chem as rdkit
 
-Json: typing.TypeAlias = float | str | None | list["Json"] | dict[str, "Json"]
+Json: typing.TypeAlias = (
+    bool | float | str | None | list["Json"] | dict[str, "Json"]
+)
 Conformer: typing.TypeAlias = list[list[float]]
 
 
 class Bonds(typing.TypedDict):
     """
     JSON representation of bonds.
     """
```

### Comparing `atomlite-1.1.2/src/atomlite.egg-info/PKG-INFO` & `atomlite-1.2.0/src/atomlite.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: atomlite
-Version: 1.1.2
+Version: 1.2.0
 Maintainer-email: Lukas Turcani <lukasturcani93@gmail.com>
 Project-URL: github, https://github.com/lukasturcani/atomlite
 Project-URL: documentation, https://atomlite.readthedocs.io
 Requires-Python: >=3.11
 Description-Content-Type: text/x-rst
 Provides-Extra: dev
```

### Comparing `atomlite-1.1.2/tests/test_database.py` & `atomlite-1.2.0/tests/test_database.py`

 * *Files 15% similar despite different names*

```diff
@@ -15,14 +15,80 @@
 
 @dataclass(frozen=True, slots=True)
 class MultipleEntryCase:
     entries: tuple[atomlite.Entry, ...]
     molecules: tuple[rdkit.Mol, ...]
 
 
+def test_set_property(database: atomlite.Database) -> None:
+    entry = atomlite.Entry.from_rdkit(
+        key="first",
+        molecule=rdkit.MolFromSmiles("C"),
+        properties={
+            "a": {
+                "b": 12,
+            },
+        },
+    )
+    database.add_entries(entry)
+    database.set_property("first", "$.a.c", 12)
+    assert database.get_property("first", "$.a.c") == 12
+
+
+def test_get_missing_property(database: atomlite.Database) -> None:
+    entry = atomlite.Entry.from_rdkit(
+        key="first",
+        molecule=rdkit.MolFromSmiles("C"),
+        properties={
+            "a": {
+                "b": 12,
+            },
+        },
+    )
+    database.add_entries(entry)
+    assert database.get_property("first", "$.a.not_here") is None
+
+
+def test_get_property_from_missing_molecule(
+    database: atomlite.Database,
+) -> None:
+    with pytest.raises(atomlite.MoleculeNotFound):
+        database.get_property("first", "$.a.a")
+
+
+def test_get_property(database: atomlite.Database) -> None:
+    entry = atomlite.Entry.from_rdkit(
+        key="first",
+        molecule=rdkit.MolFromSmiles("C"),
+        properties={
+            "a": {
+                "b": 12,
+                "c": [1, 2, 3],
+                "d": "[4, 5, 6]",
+                "e": "hi",
+                "f": None,
+                "g": {"a": 12, "b": 24},
+                "h": True,
+                "i": False,
+                "j": 12.2,
+            },
+        },
+    )
+    database.add_entries(entry)
+    assert database.get_property("first", "$.a.b") == 12
+    assert database.get_property("first", "$.a.c") == [1, 2, 3]
+    assert database.get_property("first", "$.a.d") == "[4, 5, 6]"
+    assert database.get_property("first", "$.a.e") == "hi"
+    assert database.get_property("first", "$.a.f") is None
+    assert database.get_property("first", "$.a.g") == {"a": 12, "b": 24}
+    assert database.get_property("first", "$.a.h") is True
+    assert database.get_property("first", "$.a.i") is False
+    assert database.get_property("first", "$.a.j") == 12.2
+
+
 def test_entry_is_replaced_on_update(database: atomlite.Database) -> None:
     entry1 = atomlite.Entry.from_rdkit(
         key="first",
         molecule=rdkit.MolFromSmiles("C"),
         properties={"a": 12},
     )
     database.add_entries(entry1)
```

