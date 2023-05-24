# Comparing `tmp/microdata_validator-7.3.3.tar.gz` & `tmp/microdata_validator-7.3.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "microdata_validator-7.3.3.tar", max compression
+gzip compressed data, was "microdata_validator-7.3.4.tar", max compression
```

## Comparing `microdata_validator-7.3.3.tar` & `microdata_validator-7.3.4.tar`

### file list

```diff
@@ -1,26 +1,26 @@
--rw-r--r--   0        0        0     1102 2023-05-08 12:02:34.301743 microdata_validator-7.3.3/LICENSE
--rw-r--r--   0        0        0     1707 2023-05-08 12:02:34.301743 microdata_validator-7.3.3/README.md
--rw-r--r--   0        0        0     6877 2023-05-08 12:02:34.305743 microdata_validator-7.3.3/microdata_validator/__init__.py
--rw-r--r--   0        0        0     4424 2023-05-08 12:02:34.305743 microdata_validator-7.3.3/microdata_validator/adapter/local_storage.py
--rw-r--r--   0        0        0     5603 2023-05-08 12:02:34.305743 microdata_validator-7.3.3/microdata_validator/components/temporal_attributes.py
--rw-r--r--   0        0        0      776 2023-05-08 12:02:34.305743 microdata_validator-7.3.3/microdata_validator/components/unit_id_types.py
--rw-r--r--   0        0        0     1581 2023-05-08 12:02:34.305743 microdata_validator-7.3.3/microdata_validator/components/unit_type_variables/BK_HELSESTASJONSKONSULTASJON.json
--rw-r--r--   0        0        0     2091 2023-05-08 12:02:34.305743 microdata_validator-7.3.3/microdata_validator/components/unit_type_variables/FAMILIE.json
--rw-r--r--   0        0        0     1525 2023-05-08 12:02:34.305743 microdata_validator-7.3.3/microdata_validator/components/unit_type_variables/FORETAK.json
--rw-r--r--   0        0        0     2124 2023-05-08 12:02:34.305743 microdata_validator-7.3.3/microdata_validator/components/unit_type_variables/HUSHOLDNING.json
--rw-r--r--   0        0        0     1429 2023-05-08 12:02:34.305743 microdata_validator-7.3.3/microdata_validator/components/unit_type_variables/JOBB.json
--rw-r--r--   0        0        0     1378 2023-05-08 12:02:34.305743 microdata_validator-7.3.3/microdata_validator/components/unit_type_variables/KJORETOY.json
--rw-r--r--   0        0        0   232471 2023-05-08 12:02:34.305743 microdata_validator-7.3.3/microdata_validator/components/unit_type_variables/KOMMUNE.json
--rw-r--r--   0        0        0     1242 2023-05-08 12:02:34.305743 microdata_validator-7.3.3/microdata_validator/components/unit_type_variables/KURS.json
--rw-r--r--   0        0        0     1202 2023-05-08 12:02:34.305743 microdata_validator-7.3.3/microdata_validator/components/unit_type_variables/PERSON.json
--rw-r--r--   0        0        0     1535 2023-05-08 12:02:34.305743 microdata_validator-7.3.3/microdata_validator/components/unit_type_variables/VIRKSOMHET.json
--rw-r--r--   0        0        0     1166 2023-05-08 12:02:34.305743 microdata_validator-7.3.3/microdata_validator/components/unit_type_variables/__init__.py
--rw-r--r--   0        0        0      414 2023-05-08 12:02:34.305743 microdata_validator-7.3.3/microdata_validator/exceptions/__init__.py
--rw-r--r--   0        0        0      872 2023-05-08 12:02:34.305743 microdata_validator-7.3.3/microdata_validator/model/__init__.py
--rw-r--r--   0        0        0     5781 2023-05-08 12:02:34.305743 microdata_validator-7.3.3/microdata_validator/model/metadata.py
--rw-r--r--   0        0        0     7854 2023-05-08 12:02:34.305743 microdata_validator-7.3.3/microdata_validator/steps/dataset_reader.py
--rw-r--r--   0        0        0     7837 2023-05-08 12:02:34.305743 microdata_validator-7.3.3/microdata_validator/steps/dataset_validator.py
--rw-r--r--   0        0        0     1663 2023-05-08 12:02:34.305743 microdata_validator-7.3.3/microdata_validator/steps/metadata_inliner.py
--rw-r--r--   0        0        0     1682 2023-05-08 12:02:34.305743 microdata_validator-7.3.3/microdata_validator/steps/metadata_reader.py
--rw-r--r--   0        0        0      682 2023-05-08 12:02:34.305743 microdata_validator-7.3.3/pyproject.toml
--rw-r--r--   0        0        0     2468 1970-01-01 00:00:00.000000 microdata_validator-7.3.3/PKG-INFO
+-rw-r--r--   0        0        0     1102 2023-05-24 12:57:45.520918 microdata_validator-7.3.4/LICENSE
+-rw-r--r--   0        0        0     1707 2023-05-24 12:57:45.520918 microdata_validator-7.3.4/README.md
+-rw-r--r--   0        0        0     6801 2023-05-24 12:57:45.520918 microdata_validator-7.3.4/microdata_validator/__init__.py
+-rw-r--r--   0        0        0     4392 2023-05-24 12:57:45.520918 microdata_validator-7.3.4/microdata_validator/adapter/local_storage.py
+-rw-r--r--   0        0        0     5605 2023-05-24 12:57:45.524918 microdata_validator-7.3.4/microdata_validator/components/temporal_attributes.py
+-rw-r--r--   0        0        0      777 2023-05-24 12:57:45.524918 microdata_validator-7.3.4/microdata_validator/components/unit_id_types.py
+-rw-r--r--   0        0        0     1581 2023-05-24 12:57:45.524918 microdata_validator-7.3.4/microdata_validator/components/unit_type_variables/BK_HELSESTASJONSKONSULTASJON.json
+-rw-r--r--   0        0        0     2091 2023-05-24 12:57:45.524918 microdata_validator-7.3.4/microdata_validator/components/unit_type_variables/FAMILIE.json
+-rw-r--r--   0        0        0     1525 2023-05-24 12:57:45.524918 microdata_validator-7.3.4/microdata_validator/components/unit_type_variables/FORETAK.json
+-rw-r--r--   0        0        0     2124 2023-05-24 12:57:45.524918 microdata_validator-7.3.4/microdata_validator/components/unit_type_variables/HUSHOLDNING.json
+-rw-r--r--   0        0        0     1429 2023-05-24 12:57:45.524918 microdata_validator-7.3.4/microdata_validator/components/unit_type_variables/JOBB.json
+-rw-r--r--   0        0        0     1378 2023-05-24 12:57:45.524918 microdata_validator-7.3.4/microdata_validator/components/unit_type_variables/KJORETOY.json
+-rw-r--r--   0        0        0   232471 2023-05-24 12:57:45.524918 microdata_validator-7.3.4/microdata_validator/components/unit_type_variables/KOMMUNE.json
+-rw-r--r--   0        0        0     1242 2023-05-24 12:57:45.524918 microdata_validator-7.3.4/microdata_validator/components/unit_type_variables/KURS.json
+-rw-r--r--   0        0        0     1202 2023-05-24 12:57:45.524918 microdata_validator-7.3.4/microdata_validator/components/unit_type_variables/PERSON.json
+-rw-r--r--   0        0        0     1535 2023-05-24 12:57:45.524918 microdata_validator-7.3.4/microdata_validator/components/unit_type_variables/VIRKSOMHET.json
+-rw-r--r--   0        0        0     1167 2023-05-24 12:57:45.524918 microdata_validator-7.3.4/microdata_validator/components/unit_type_variables/__init__.py
+-rw-r--r--   0        0        0      414 2023-05-24 12:57:45.524918 microdata_validator-7.3.4/microdata_validator/exceptions/__init__.py
+-rw-r--r--   0        0        0      888 2023-05-24 12:57:45.524918 microdata_validator-7.3.4/microdata_validator/model/__init__.py
+-rw-r--r--   0        0        0     5781 2023-05-24 12:57:45.524918 microdata_validator-7.3.4/microdata_validator/model/metadata.py
+-rw-r--r--   0        0        0     8062 2023-05-24 12:57:45.524918 microdata_validator-7.3.4/microdata_validator/steps/dataset_reader.py
+-rw-r--r--   0        0        0     7701 2023-05-24 12:57:45.524918 microdata_validator-7.3.4/microdata_validator/steps/dataset_validator.py
+-rw-r--r--   0        0        0     1659 2023-05-24 12:57:45.524918 microdata_validator-7.3.4/microdata_validator/steps/metadata_inliner.py
+-rw-r--r--   0        0        0     1680 2023-05-24 12:57:45.524918 microdata_validator-7.3.4/microdata_validator/steps/metadata_reader.py
+-rw-r--r--   0        0        0      651 2023-05-24 12:57:45.524918 microdata_validator-7.3.4/pyproject.toml
+-rw-r--r--   0        0        0     2468 1970-01-01 00:00:00.000000 microdata_validator-7.3.4/PKG-INFO
```

### Comparing `microdata_validator-7.3.3/LICENSE` & `microdata_validator-7.3.4/LICENSE`

 * *Files identical despite different names*

### Comparing `microdata_validator-7.3.3/README.md` & `microdata_validator-7.3.4/README.md`

 * *Files identical despite different names*

### Comparing `microdata_validator-7.3.3/microdata_validator/__init__.py` & `microdata_validator-7.3.4/microdata_validator/__init__.py`

 * *Files 3% similar despite different names*

```diff
@@ -4,70 +4,69 @@
 from typing import List, Union
 from pathlib import Path
 
 from microdata_validator.model import validate_metadata_model
 from microdata_validator.adapter import local_storage
 from microdata_validator.components import unit_id_types
 from microdata_validator.steps import (
-    dataset_reader, dataset_validator, metadata_reader, metadata_inliner
+    dataset_reader,
+    dataset_validator,
+    metadata_reader,
+    metadata_inliner,
 )
 from microdata_validator.exceptions import (
     InvalidDatasetException,
-    InvalidDatasetName
+    InvalidDatasetName,
 )
 
 logger = logging.getLogger()
 
 
 def validate(
     dataset_name: str,
-    working_directory: str = '',
-    input_directory: str = '',
+    working_directory: str = "",
+    input_directory: str = "",
     keep_temporary_files: bool = False,
-    metadata_ref_directory: str = None
+    metadata_ref_directory: str = None,
 ) -> List[str]:
     """
     Validate a dataset and return a list of errors.
     If the dataset is valid, the list will be empty.
     """
     # validate dataset name
     try:
         validate_dataset_name(dataset_name)
     except InvalidDatasetName as e:
         return [str(e)]
 
     # Generate working directory if not supplied
-    working_directory_path, working_directory_was_generated = (
-         local_storage.resolve_working_directory(working_directory)
-    )
+    (
+        working_directory_path,
+        working_directory_was_generated,
+    ) = local_storage.resolve_working_directory(working_directory)
     # Make paths for input and ref directory
     input_directory_path = Path(input_directory)
     if metadata_ref_directory is not None:
         metadata_ref_directory = Path(metadata_ref_directory)
 
     # Run readers and validator
     data_errors = []
     unexpected_exception_occured = False
     try:
         metadata_file_path = (
-            input_directory_path / dataset_name / f'{dataset_name}.json'
+            input_directory_path / dataset_name / f"{dataset_name}.json"
         )
         metadata_dict = metadata_inliner.run_inliner(
-            metadata_file_path,
-            metadata_ref_directory
+            metadata_file_path, metadata_ref_directory
         )
         metadata_reader.run_reader(
-            dataset_name,
-            working_directory_path,
-            metadata_dict
+            dataset_name, working_directory_path, metadata_dict
         )
         dataset_reader.run_reader(
-            dataset_name,
-            working_directory_path,
-            input_directory_path
+            dataset_name, working_directory_path, input_directory_path
         )
         data_errors = dataset_validator.run_validator(
             working_directory_path, dataset_name
         )
     except InvalidDatasetException as e:
         data_errors = e.errors
     except Exception as e:
@@ -76,91 +75,89 @@
         raise e
     finally:
         # Delete temporary files
         if not keep_temporary_files or unexpected_exception_occured:
             local_storage.clean_up_temporary_files(
                 dataset_name,
                 working_directory_path,
-                delete_working_directory=working_directory_was_generated
+                delete_working_directory=working_directory_was_generated,
             )
     return data_errors
 
 
 def validate_metadata(
     dataset_name: str,
-    input_directory: str = '',
+    input_directory: str = "",
     metadata_ref_directory: str = None,
-    working_directory: str = '',
-    keep_temporary_files: bool = False
+    working_directory: str = "",
+    keep_temporary_files: bool = False,
 ) -> List[dict]:
     """
     Validate metadata and return a list of errors.
     If the metadata is valid, the list will be empty.
     """
     data_errors = []
 
     # validate dataset name
     try:
         validate_dataset_name(dataset_name)
     except InvalidDatasetName as e:
         return [str(e)]
 
     # Generate working directory if not supplied
-    working_directory_path, working_directory_was_generated = (
-         local_storage.resolve_working_directory(working_directory)
-    )
+    (
+        working_directory_path,
+        working_directory_was_generated,
+    ) = local_storage.resolve_working_directory(working_directory)
 
     # Make paths for input and ref directory
     input_directory_path = Path(input_directory)
     if metadata_ref_directory is not None:
         metadata_ref_directory = Path(metadata_ref_directory)
 
     try:
         metadata_file_path = (
-            input_directory_path / dataset_name / f'{dataset_name}.json'
+            input_directory_path / dataset_name / f"{dataset_name}.json"
         )
         metadata_dict = metadata_inliner.run_inliner(
-            metadata_file_path,
-            metadata_ref_directory
+            metadata_file_path, metadata_ref_directory
         )
         metadata_reader.run_reader(
-            dataset_name,
-            working_directory_path,
-            metadata_dict
+            dataset_name, working_directory_path, metadata_dict
         )
     except InvalidDatasetException as e:
         data_errors = e.errors
     except InvalidDatasetName as e:
         data_errors = [str(e)]
     except Exception as e:
         # Raise unexpected exceptions to user
         raise e
     finally:
         # Delete temporary files
         if not keep_temporary_files:
             local_storage.clean_up_temporary_files(
                 dataset_name,
                 working_directory_path,
-                delete_working_directory=working_directory_was_generated
+                delete_working_directory=working_directory_was_generated,
             )
     return data_errors
 
 
 def inline_metadata(
     metadata_file_path: str,
     metadata_ref_directory: str,
-    output_file_path: str = None
+    output_file_path: str = None,
 ) -> Path:
     """
     Generate a metadata file with inlined references from a supplied
     metadata file and a reference directory.
     Returns the path to the generated file.
     Throws an error if the metadata is invalid.
     """
-    dataset_name = metadata_file_path.split('/')[-1][:-5]
+    dataset_name = metadata_file_path.split("/")[-1][:-5]
     validate_dataset_name(dataset_name)
     if output_file_path is None:
         output_file_path = Path(
             f"{metadata_file_path.strip('.json')}_INLINED.json"
         )
     else:
         output_file_path = Path(output_file_path)
@@ -191,29 +188,27 @@
 
 
 def validate_dataset_name(dataset_name: str) -> None:
     """
     Validates that the name of the dataset only contains valid
     characters (uppercase A-Z, numbers 0-9 and _)
     """
-    valid_characters = (
-        string.ascii_uppercase + string.digits + '_'
-    )
+    valid_characters = string.ascii_uppercase + string.digits + "_"
     if not all([character in valid_characters for character in dataset_name]):
         raise InvalidDatasetName(
             f'"{dataset_name}" contains invalid characters. '
             'Please use only uppercase A-Z, numbers 0-9 or "_"'
         )
-    if dataset_name[0] in string.digits + '_':
+    if dataset_name[0] in string.digits + "_":
         raise InvalidDatasetName(
             f'"{dataset_name}" has a leading number or _.'
-            'Please start dataset names with an upper case character A-Z'
+            "Please start dataset names with an upper case character A-Z"
         )
 
 
 __all__ = [
     "validate",
     "validate_metadata",
     "validate_dataset_name",
     "inline_metadata",
-    "get_unit_id_type_for_unit_type"
+    "get_unit_id_type_for_unit_type",
 ]
```

### Comparing `microdata_validator-7.3.3/microdata_validator/adapter/local_storage.py` & `microdata_validator-7.3.4/microdata_validator/adapter/local_storage.py`

 * *Files 8% similar despite different names*

```diff
@@ -10,26 +10,24 @@
 
 
 logger = logging.getLogger()
 
 
 def load_json(filepath: Path) -> dict:
     try:
-        with open(filepath, 'r', encoding='utf-8') as f:
+        with open(filepath, "r", encoding="utf-8") as f:
             return json.load(f)
     except Exception as e:
         logging.error(f"Failed to open file at {str(Path)}")
         raise e
 
 
 def write_json(filepath: Path, content: dict) -> None:
-    with open(filepath, 'w', encoding='utf-8') as json_file:
-        json.dump(
-            content, json_file, indent=4, ensure_ascii=False
-        )
+    with open(filepath, "w", encoding="utf-8") as json_file:
+        json.dump(content, json_file, indent=4, ensure_ascii=False)
 
 
 def resolve_working_directory(
     working_directory: Union[str, None]
 ) -> Tuple[Path, bool]:
     """
     Generates a working directory if a working directory is not supplied.
@@ -44,99 +42,97 @@
         os.mkdir(generated_working_directory)
         return generated_working_directory, True
 
 
 def clean_up_temporary_files(
     dataset_name: str,
     working_directory: Path,
-    delete_working_directory: Path = False
+    delete_working_directory: Path = False,
 ):
     generated_files = [
-        f'{dataset_name}.csv',
-        f'{dataset_name}.json',
-        f'{dataset_name}.db',
+        f"{dataset_name}.csv",
+        f"{dataset_name}.json",
+        f"{dataset_name}.db",
     ]
     if delete_working_directory:
         temporary_files = os.listdir(working_directory)
         unknown_files = [
             file for file in temporary_files if file not in generated_files
         ]
         if not unknown_files:
             try:
                 shutil.rmtree(working_directory)
             except Exception as e:
                 logger.error(
-                    'An exception occured while attempting to delete'
-                    f'temporary files: {e}'
+                    "An exception occured while attempting to delete"
+                    f"temporary files: {e}"
                 )
         else:
             for file in generated_files:
                 try:
                     os.remove(working_directory / file)
                 except FileNotFoundError:
                     logger.error(
-                        f'Could not find file {file} in working directory '
-                        'when attempting to delete temporary files.'
+                        f"Could not find file {file} in working directory "
+                        "when attempting to delete temporary files."
                     )
     else:
         for file in generated_files:
             try:
                 os.remove(working_directory / file)
             except FileNotFoundError:
                 logger.error(
-                    f'Could not find file {file} in working directory '
-                    'when attempting to delete temporary files.'
+                    f"Could not find file {file} in working directory "
+                    "when attempting to delete temporary files."
                 )
 
 
 def _create_temp_sqlite_db_file(
-    db_file: Path
+    db_file: Path,
 ) -> Tuple[db.Connection, db.Cursor]:
     sql_create_table = """
         CREATE TABLE temp_dataset (
             row_number INT NOT NULL,
             unit_id TEXT NOT NULL,
             value TEXT NOT NULL,
             start TEXT,
             stop TEXT,
             attributes TEXT) """
 
     db_conn = db.connect(db_file)
     cursor = db_conn.cursor()
     cursor.execute(sql_create_table)
     # Set Sqlite-params to speed up performance
-    cursor.execute('PRAGMA synchronous = OFF')
-    cursor.execute('BEGIN TRANSACTION')
+    cursor.execute("PRAGMA synchronous = OFF")
+    cursor.execute("BEGIN TRANSACTION")
     return (db_conn, cursor)
 
 
 def insert_data_csv_into_sqlite(
     sqlite_file_path, dataset_data_file, field_separator=";"
 ) -> None:
-    db_conn, cursor = _create_temp_sqlite_db_file(
-        sqlite_file_path
-    )
-    with open(file=dataset_data_file, newline='', encoding='utf-8') as f:
+    db_conn, cursor = _create_temp_sqlite_db_file(sqlite_file_path)
+    with open(file=dataset_data_file, newline="", encoding="utf-8") as f:
         reader = csv.reader(f, delimiter=field_separator)
         cursor.executemany(
-            'INSERT INTO temp_dataset '
-            '(row_number, unit_id, value, start, stop, attributes) '
-            'VALUES (?, ?, ?, ?, ?, ?)',
-            reader
+            "INSERT INTO temp_dataset "
+            "(row_number, unit_id, value, start, stop, attributes) "
+            "VALUES (?, ?, ?, ?, ?, ?)",
+            reader,
         )
     db_conn.commit()
     db_conn.close()
     logger.debug(
         f'Done reading datafile "{dataset_data_file}" '
-        'into temp Sqlite database table.'
+        "into temp Sqlite database table."
     )
 
 
 def read_temp_sqlite_db_data_sorted(
-    db_file: Path
+    db_file: Path,
 ) -> Tuple[db.Connection, db.Cursor]:
     sql_select_sorted = """
         SELECT row_number, unit_id, value, start, stop, attributes
         FROM temp_dataset
         ORDER BY unit_id, start, stop
     """
```

### Comparing `microdata_validator-7.3.3/microdata_validator/components/temporal_attributes.py` & `microdata_validator-7.3.4/microdata_validator/components/temporal_attributes.py`

 * *Files 1% similar despite different names*

```diff
@@ -146,28 +146,28 @@
     "variableRole": "Start",
     "shortName": "START",
     "dataType": "DATE",
     "valueDomain": {
         "description": [
             {
                 "languageCode": "no",
-                "value": "Dato oppgitt i dager siden 1970-01-01"
+                "value": "Dato oppgitt i dager siden 1970-01-01",
             }
         ]
     },
 }
 STOP_VARIABLE_DEFINITION = {
     "variableRole": "Stop",
     "shortName": "STOP",
     "dataType": "DATE",
     "valueDomain": {
         "description": [
             {
                 "languageCode": "no",
-                "value": "Dato oppgitt i dager siden 1970-01-01"
+                "value": "Dato oppgitt i dager siden 1970-01-01",
             }
         ]
     },
 }
 
 
 def generate_start_time_attribute(temporality_type: str):
```

### Comparing `microdata_validator-7.3.3/microdata_validator/components/unit_id_types.py` & `microdata_validator-7.3.4/microdata_validator/components/unit_id_types.py`

 * *Files 16% similar despite different names*

```diff
@@ -2,25 +2,25 @@
 
 from microdata_validator.exceptions import UnregisteredUnitTypeError
 
 # When updating this dictionary remember to also
 # update the Metadata model with the
 # same key value in the enum for unitType
 UNIT_ID_TYPE_FOR_UNIT_TYPE = {
-    'JOBB': 'JOBBID_1',
-    'KJORETOY': 'KJORETOY_ID',
-    'FAMILIE': 'FNR',
-    'FORETAK': 'ORGNR',
-    'HUSHOLDNING': 'FNR',
-    'KOMMUNE': None,
-    'KURS': 'KURSID',
-    'PERSON': 'FNR',
-    'VIRKSOMHET': 'ORGNR',
-    'BK_HELSESTASJONSKONSULTASJON': 'BK_STASJONS_BESOKS_ID'
+    "JOBB": "JOBBID_1",
+    "KJORETOY": "KJORETOY_ID",
+    "FAMILIE": "FNR",
+    "FORETAK": "ORGNR",
+    "HUSHOLDNING": "FNR",
+    "KOMMUNE": None,
+    "KURS": "KURSID",
+    "PERSON": "FNR",
+    "VIRKSOMHET": "ORGNR",
+    "BK_HELSESTASJONSKONSULTASJON": "BK_STASJONS_BESOKS_ID",
 }
 
 
 def get_unit_id_type_for_unit_type(unit_type: str) -> Union[str, None]:
     try:
         return UNIT_ID_TYPE_FOR_UNIT_TYPE[unit_type]
     except KeyError as e:
-        raise UnregisteredUnitTypeError(f'No such unit type: {str(e)}') from e
+        raise UnregisteredUnitTypeError(f"No such unit type: {str(e)}") from e
```

### Comparing `microdata_validator-7.3.3/microdata_validator/components/unit_type_variables/BK_HELSESTASJONSKONSULTASJON.json` & `microdata_validator-7.3.4/microdata_validator/components/unit_type_variables/BK_HELSESTASJONSKONSULTASJON.json`

 * *Files identical despite different names*

### Comparing `microdata_validator-7.3.3/microdata_validator/components/unit_type_variables/FAMILIE.json` & `microdata_validator-7.3.4/microdata_validator/components/unit_type_variables/FAMILIE.json`

 * *Files identical despite different names*

### Comparing `microdata_validator-7.3.3/microdata_validator/components/unit_type_variables/FORETAK.json` & `microdata_validator-7.3.4/microdata_validator/components/unit_type_variables/FORETAK.json`

 * *Files identical despite different names*

### Comparing `microdata_validator-7.3.3/microdata_validator/components/unit_type_variables/HUSHOLDNING.json` & `microdata_validator-7.3.4/microdata_validator/components/unit_type_variables/HUSHOLDNING.json`

 * *Files identical despite different names*

### Comparing `microdata_validator-7.3.3/microdata_validator/components/unit_type_variables/JOBB.json` & `microdata_validator-7.3.4/microdata_validator/components/unit_type_variables/JOBB.json`

 * *Files identical despite different names*

### Comparing `microdata_validator-7.3.3/microdata_validator/components/unit_type_variables/KJORETOY.json` & `microdata_validator-7.3.4/microdata_validator/components/unit_type_variables/KJORETOY.json`

 * *Files identical despite different names*

### Comparing `microdata_validator-7.3.3/microdata_validator/components/unit_type_variables/KOMMUNE.json` & `microdata_validator-7.3.4/microdata_validator/components/unit_type_variables/KOMMUNE.json`

 * *Files identical despite different names*

### Comparing `microdata_validator-7.3.3/microdata_validator/components/unit_type_variables/KURS.json` & `microdata_validator-7.3.4/microdata_validator/components/unit_type_variables/KURS.json`

 * *Files identical despite different names*

### Comparing `microdata_validator-7.3.3/microdata_validator/components/unit_type_variables/PERSON.json` & `microdata_validator-7.3.4/microdata_validator/components/unit_type_variables/PERSON.json`

 * *Files identical despite different names*

### Comparing `microdata_validator-7.3.3/microdata_validator/components/unit_type_variables/VIRKSOMHET.json` & `microdata_validator-7.3.4/microdata_validator/components/unit_type_variables/VIRKSOMHET.json`

 * *Files identical despite different names*

### Comparing `microdata_validator-7.3.3/microdata_validator/model/__init__.py` & `microdata_validator-7.3.4/microdata_validator/model/__init__.py`

 * *Files 18% similar despite different names*

```diff
@@ -13,18 +13,19 @@
 def validate_metadata_model(metadata_json: dict) -> None:
     try:
         Metadata(**metadata_json)
     except ValidationError as e:
         logger.exception(e)
         error_messages = []
         for error in e.errors():
-            location = '->'.join(
-                loc for loc in error['loc']
-                if loc != '__root__' and not isinstance(loc, int)
+            location = "->".join(
+                loc
+                for loc in error["loc"]
+                if loc != "__root__" and not isinstance(loc, int)
             )
             error_messages.append(f'{location}: {error["msg"]}')
         raise InvalidDatasetException(
-            'Invalid metadata file', errors=error_messages
+            "Invalid metadata file", errors=error_messages
         )
     except Exception as e:
         logger.exception(e)
         raise e
```

### Comparing `microdata_validator-7.3.3/microdata_validator/model/metadata.py` & `microdata_validator-7.3.4/microdata_validator/model/metadata.py`

 * *Files 13% similar despite different names*

```diff
@@ -70,24 +70,25 @@
     @classmethod
     def validate_code_list_item(cls, values):
         def validate_date_string(field_name: str, date_string: str):
             try:
                 datetime.datetime(
                     int(date_string[:4]),
                     int(date_string[5:7]),
-                    int(date_string[8:10])
+                    int(date_string[8:10]),
                 )
             except ValueError as e:
                 raise ValueError(
                     f'Invalid {field_name} date for {values["code"]}. '
-                    'Date format: YYYY-MM-DD'
+                    "Date format: YYYY-MM-DD"
                 ) from e
-        validate_date_string('validFrom', values['validFrom'])
-        if values.get('validUntil' is not None):
-            validate_date_string('validUntil', values['validUntil'])
+
+        validate_date_string("validFrom", values["validFrom"])
+        if values.get("validUntil" != None):
+            validate_date_string("validUntil", values["validUntil"])
         return values
 
 
 class SentinelItem(BaseModel, extra=Extra.forbid):
     code: str
     categoryTitle: conlist(MultiLingualString, min_items=1)
 
@@ -103,33 +104,34 @@
     sentinelAndMissingValues: Optional[List[SentinelItem]]
 
     @root_validator(skip_on_failure=True)
     @classmethod
     def validate_value_domain(cls, values: dict):
         def raise_invalid_with_code_list(field_name: str):
             raise ValueError(
-                f'Can not add a {field_name} in a valuedomain with a codeList'
+                f"Can not add a {field_name} in a valuedomain with a codeList"
             )
-        if values.get('codeList', None) is not None:
-            if values.get('description', None) is not None:
-                raise_invalid_with_code_list('description')
-            if values.get('measurementType', None) is not None:
-                raise_invalid_with_code_list('measurementType')
-            if values.get('measurementUnitDescription', None) is not None:
-                raise_invalid_with_code_list('measurementUnitDescription')
-        elif values.get('description', None) is not None:
-            if values.get('sentinelAndMissingValues', None) is not None:
+
+        if values.get("codeList", None) is not None:
+            if values.get("description", None) is not None:
+                raise_invalid_with_code_list("description")
+            if values.get("measurementType", None) is not None:
+                raise_invalid_with_code_list("measurementType")
+            if values.get("measurementUnitDescription", None) is not None:
+                raise_invalid_with_code_list("measurementUnitDescription")
+        elif values.get("description", None) is not None:
+            if values.get("sentinelAndMissingValues", None) is not None:
                 raise ValueError(
-                    'Can not add sentinelAndMissingValues '
-                    'in valuedomain with a description'
+                    "Can not add sentinelAndMissingValues "
+                    "in valuedomain with a description"
                 )
         else:
             raise ValueError(
-                'A valueDomain must contain either a codeList '
-                'or a description'
+                "A valueDomain must contain either a codeList "
+                "or a description"
             )
         return values
 
 
 class MeasureVariable(BaseModel):
     unitType: Optional[UnitType]
     name: conlist(MultiLingualString, min_items=1)
@@ -140,27 +142,28 @@
     valueDomain: Optional[ValueDomain]
 
     @root_validator(skip_on_failure=True)
     @classmethod
     def validate_measure(cls, values: dict):
         def raise_invalid_with_unit_type(field_name: str):
             raise ValueError(
-                f'Can not set a {field_name} in a measure variable '
-                'together with a unitType'
+                f"Can not set a {field_name} in a measure variable "
+                "together with a unitType"
             )
-        if values.get('unitType', None) is not None:
-            if values.get('dataType', None) is not None:
-                raise_invalid_with_unit_type('dataType')
-            if values.get('valueDomain', None) is not None:
-                raise_invalid_with_unit_type('valueDomain')
+
+        if values.get("unitType", None) is not None:
+            if values.get("dataType", None) is not None:
+                raise_invalid_with_unit_type("dataType")
+            if values.get("valueDomain", None) is not None:
+                raise_invalid_with_unit_type("valueDomain")
         else:
-            if values.get('dataType', None) is None:
-                raise ValueError('Missing dataType in measure variable')
-            if values.get('valueDomain', None) is None:
-                raise ValueError('Missing valueDomain in measure variable')
+            if values.get("dataType", None) is None:
+                raise ValueError("Missing dataType in measure variable")
+            if values.get("valueDomain", None) is None:
+                raise ValueError("Missing valueDomain in measure variable")
         return values
 
 
 class Metadata(BaseModel):
     temporalityType: TemporalityType
     sensitivityLevel: SensitivityLevel
     populationDescription: conlist(MultiLingualString, min_items=1)
```

### Comparing `microdata_validator-7.3.3/microdata_validator/steps/dataset_reader.py` & `microdata_validator-7.3.4/microdata_validator/steps/dataset_reader.py`

 * *Files 8% similar despite different names*

```diff
@@ -10,53 +10,61 @@
 logger = logging.getLogger()
 
 
 def _read_and_process_data(
     data_file_path: Path,
     enriched_data_file_path: Path,
     field_separator: str = ";",
-    data_error_limit: int = 50
+    data_error_limit: int = 50,
 ) -> dict:
     data_errors = []
     start_dates = set()
     stop_dates = set()
     rows_validated = 0
 
     logger.debug(f'Validate datafile "{data_file_path}"')
     data_file_with_row_numbers = open(
-        enriched_data_file_path, 'w', encoding='utf-8'
+        enriched_data_file_path, "w", encoding="utf-8"
     )
     with open(
-        file=data_file_path, newline='', encoding='utf-8', errors="strict"
+        file=data_file_path, newline="", encoding="utf-8", errors="strict"
     ) as f:
         csv_sniffer = csv.Sniffer()
-        csv_file_separator = csv_sniffer.sniff(f.read(5000)).delimiter
+        try:
+            csv_file_separator = csv_sniffer.sniff(f.read(5000)).delimiter
+        except csv.Error as e:
+            error_message = (
+                "Can not read separator from dataset. The .csv file might be empty.",
+            )
+            raise InvalidDatasetException(
+                error_message, [error_message]
+            ) from e
         if csv_file_separator != field_separator:
             error_message = (
                 f'Invalid field separator "{csv_file_separator}". Use ";".'
             )
             raise InvalidDatasetException(error_message, [error_message])
 
     with open(
-        file=data_file_path, newline='', encoding='utf-8', errors="strict"
+        file=data_file_path, newline="", encoding="utf-8", errors="strict"
     ) as f:
         reader = csv.reader(f, delimiter=field_separator)
         try:
             for data_row in reader:
                 if reader.line_num % 1_000_000 == 0:
                     logger.debug(f".. now reading row: {reader.line_num}")
                 rows_validated += 1
                 if len(data_errors) >= data_error_limit:
                     logger.debug(
                         f"Validation stopped - error limit reached, "
                         f"{str(rows_validated)} rows validated"
                     )
                     raise InvalidDatasetException(
-                        'Invalid data found while reading data file',
-                        data_errors
+                        "Invalid data found while reading data file",
+                        data_errors,
                     )
 
                 if not data_row:
                     data_errors.append(
                         f"row {reader.line_num}: "
                         "Empty data row. Expected row with fields "
                         "UNIT_ID, VALUE, (START), (STOP), (ATTRIBUTES))"
@@ -69,129 +77,124 @@
                     )
                 else:
                     unit_id = data_row[0].strip('"').strip()
                     value = data_row[1].strip('"').strip()
                     start = data_row[2].strip('"').strip()
                     stop = data_row[3].strip('"').strip()
                     data_file_with_row_numbers.write(
-                        f'{reader.line_num};{unit_id};{value};'
-                        f'{start};{stop};\n'
+                        f"{reader.line_num};{unit_id};{value};"
+                        f"{start};{stop};\n"
                     )
                     if unit_id is None or str(unit_id).strip(" ") == "":
                         data_errors.append(
-                            f'row {reader.line_num}: '
+                            f"row {reader.line_num}: "
                             f'identifier missing or null - "{unit_id}"'
                         )
                     if value is None or str(value).strip(" ") == "":
                         data_errors.append(
-                            f'row {reader.line_num}: '
+                            f"row {reader.line_num}: "
                             f'measure missing or null - "{value}"'
                         )
                     if start not in (None, ""):
                         try:
                             datetime.datetime(
                                 int(start[:4]),
                                 int(start[5:7]),
-                                int(start[8:10])
+                                int(start[8:10]),
                             )
                         except Exception:
                             data_errors.append(
-                                f'row {reader.line_num}: '
+                                f"row {reader.line_num}: "
                                 f'START date not valid - "{start}"'
                             )
                     if stop not in (None, ""):
                         try:
                             datetime.datetime(
                                 int(stop[:4]), int(stop[5:7]), int(stop[8:10])
                             )
                         except Exception:
                             data_errors.append(
-                                f'row {reader.line_num}: '
+                                f"row {reader.line_num}: "
                                 f'STOP date not valid - "{stop}"'
                             )
                     # find temporalCoverage from datafile
                     start_dates.add(str(start).strip('"'))
                     stop_dates.add(str(stop).strip('"'))
             data_file_with_row_numbers.close()
         except UnicodeDecodeError as e:
             error_message = (
-                f'ERROR (csv.reader error). Data file not UTF-8 encoded. '
-                f'File {data_file_path}, near row {reader.line_num}: {e}'
+                f"ERROR (csv.reader error). Data file not UTF-8 encoded. "
+                f"File {data_file_path}, near row {reader.line_num}: {e}"
             )
             logger.error(error_message)
             raise InvalidDatasetException(
-                error_message, ['UTF-8 encoding error']
+                error_message, ["UTF-8 encoding error"]
             ) from e
         except csv.Error as e:
             error_message = (
-                f'ERROR (csv.reader error) in file {data_file_path}, '
-                f'near row {reader.line_num}: {e}'
+                f"ERROR (csv.reader error) in file {data_file_path}, "
+                f"near row {reader.line_num}: {e}"
             )
             logger.error(error_message)
             raise InvalidDatasetException(
-                error_message, ['CSV reader error']
+                error_message, ["CSV reader error"]
             ) from e
 
     if data_errors:
-        logger.debug(f'ERROR in file - {data_file_path}')
-        logger.debug(f'{str(rows_validated)} rows validated')
+        logger.debug(f"ERROR in file - {data_file_path}")
+        logger.debug(f"{str(rows_validated)} rows validated")
         raise InvalidDatasetException(
-            'Invalid data found while reading data file', data_errors
+            "Invalid data found while reading data file", data_errors
         )
     else:
-        logger.debug(f'{str(rows_validated)} rows validated')
+        logger.debug(f"{str(rows_validated)} rows validated")
         return {
-            'start': min(start_dates),
-            'latest': max(start_dates.union(stop_dates)),
-            'status_list': list(start_dates.union(stop_dates))
+            "start": min(start_dates),
+            "latest": max(start_dates.union(stop_dates)),
+            "status_list": list(start_dates.union(stop_dates)),
         }
 
 
-def _metadata_update_temporal_coverage(metadata: dict,
-                                       temporal_data: dict) -> None:
+def _metadata_update_temporal_coverage(
+    metadata: dict, temporal_data: dict
+) -> None:
     logger.debug(
-        'Append temporal coverage (start, stop, status dates) to metadata'
-    )
-    metadata['dataRevision']['temporalCoverageStart'] = (
-        temporal_data["start"]
-    )
-    metadata['dataRevision']['temporalCoverageLatest'] = (
-        temporal_data['latest']
+        "Append temporal coverage (start, stop, status dates) to metadata"
     )
-    if metadata['temporalityType'] == 'FIXED':
-        metadata['dataRevision']['temporalCoverageStart'] = (
-            '1900-01-01'
-        )
-    if metadata['temporalityType'] == 'STATUS':
-        temporal_status_dates_list = temporal_data['status_list']
+    metadata["dataRevision"]["temporalCoverageStart"] = temporal_data["start"]
+    metadata["dataRevision"]["temporalCoverageLatest"] = temporal_data[
+        "latest"
+    ]
+    if metadata["temporalityType"] == "FIXED":
+        metadata["dataRevision"]["temporalCoverageStart"] = "1900-01-01"
+    if metadata["temporalityType"] == "STATUS":
+        temporal_status_dates_list = temporal_data["status_list"]
         temporal_status_dates_list.sort()
-        metadata['dataRevision']['temporalStatusDates'] = (
-            temporal_status_dates_list
-        )
+        metadata["dataRevision"][
+            "temporalStatusDates"
+        ] = temporal_status_dates_list
 
 
 def run_reader(
-    dataset_name: str,
-    working_directory: Path,
-    input_directory: Path
+    dataset_name: str, working_directory: Path, input_directory: Path
 ) -> None:
     input_dataset_dir = input_directory / dataset_name
-    input_data_path = input_dataset_dir / f'{dataset_name}.csv'
-    metadata_path = working_directory / f'{dataset_name}.json'
+    input_data_path = input_dataset_dir / f"{dataset_name}.csv"
+    metadata_path = working_directory / f"{dataset_name}.json"
 
     logger.debug(f'Start reading dataset "{dataset_name}"')
-    processed_data_path = working_directory / f'{dataset_name}.csv'
+    processed_data_path = working_directory / f"{dataset_name}.csv"
     temporal_data = _read_and_process_data(
         input_data_path, processed_data_path
     )
-    logger.debug('Enriching metadata with temporal coverage')
+    logger.debug("Enriching metadata with temporal coverage")
     metadata_dict = local_storage.load_json(metadata_path)
     _metadata_update_temporal_coverage(metadata_dict, temporal_data)
 
-    logger.debug('Writing updated metadata JSON file to working directory')
+    logger.debug("Writing updated metadata JSON file to working directory")
     local_storage.write_json(metadata_path, metadata_dict)
 
-    sqlite_file_path = working_directory.joinpath(f'{dataset_name}.db')
+    sqlite_file_path = working_directory.joinpath(f"{dataset_name}.db")
     local_storage.insert_data_csv_into_sqlite(
         sqlite_file_path, processed_data_path
     )
     logger.debug(f'OK - reading dataset "{dataset_name}"')
```

### Comparing `microdata_validator-7.3.3/microdata_validator/steps/dataset_validator.py` & `microdata_validator-7.3.4/microdata_validator/steps/dataset_validator.py`

 * *Files 4% similar despite different names*

```diff
@@ -11,37 +11,37 @@
 
 def _get_data_type(metadata: dict) -> str:
     return metadata["measureVariables"][0]["dataType"]
 
 
 def _get_valid_code_set(metadata: dict) -> Set[str]:
     """get codeList if exists in enumerated-valueDomain"""
-    value_domain = metadata['measureVariables'][0]['valueDomain']
+    value_domain = metadata["measureVariables"][0]["valueDomain"]
     code_list_codes = (
-        [] if 'codeList' not in value_domain
-        else [
-            item["code"] for item in value_domain["codeList"]
-        ]
+        []
+        if "codeList" not in value_domain
+        else [item["code"] for item in value_domain["codeList"]]
     )
     sentinel_codes = (
-        [] if 'sentinelAndMissingValues' not in value_domain
+        []
+        if "sentinelAndMissingValues" not in value_domain
         else [
-            missing_item["code"] for missing_item
-            in value_domain["sentinelAndMissingValues"]
+            missing_item["code"]
+            for missing_item in value_domain["sentinelAndMissingValues"]
         ]
     )
     return set(code_list_codes + sentinel_codes)
 
 
 def _validate_data(
     sqlite_db_file_path: str, metadata: dict, error_limit: int = 50
 ) -> int:
     """
-        Read and validate sorted data rows from the temporary Sqlite
-        database file (sorted by unit_id, start, stop)
+    Read and validate sorted data rows from the temporary Sqlite
+    database file (sorted by unit_id, start, stop)
     """
     db_conn, db_cursor = local_storage.read_temp_sqlite_db_data_sorted(
         sqlite_db_file_path
     )
     temporality_type = metadata["temporalityType"]
     data_type = _get_data_type(metadata)
     valid_code_set = _get_valid_code_set(metadata)
@@ -52,34 +52,31 @@
     for data_row in db_cursor:
         row_errors = [
             _is_data_row_consistent(
                 temporality_type, data_row, previous_data_row
             ),
             _is_data_row_consistent_with_metadata(
                 data_type, valid_code_set, data_row
-            )
+            ),
         ]
         data_errors += [error for error in row_errors if error is not None]
         if len(data_errors) >= error_limit:
             raise InvalidDatasetException(
-                'Invalid data found found in data file',
-                data_errors
+                "Invalid data found found in data file", data_errors
             )
         previous_data_row = data_row
     db_conn.close()
     return data_errors
 
 
 def _is_data_row_consistent(
-    temporality_type: str,
-    data_row: tuple,
-    previous_data_row: tuple
+    temporality_type: str, data_row: tuple, previous_data_row: tuple
 ) -> Union[tuple, None]:
     """Validate consistency and event-history (unit_id * start * stop)
-       and check for row duplicates.
+    and check for row duplicates.
     """
     row_number = previous_data_row[0]
     unit_id = data_row[1]
     # value = data_row[2]
     start = data_row[3]
     stop = data_row[4]
     # attributes = data_row[5]
@@ -177,49 +174,43 @@
             )
 
     # else: Described value-domain for variable
     if data_type == "LONG":
         try:
             int(str(value).strip('"'))
         except ValueError:
-            return (
-                f"row {row_number}: "
-                f"'{value}' not of type LONG"
-            )
+            return f"row {row_number}: " f"'{value}' not of type LONG"
     elif data_type == "DOUBLE":
         try:
             float(str(value).strip('"'))
         except ValueError:
-            return (
-                f"row {row_number}: "
-                f"'{value}' not of type DOUBLE"
-            )
+            return f"row {row_number}: " f"'{value}' not of type DOUBLE"
     elif data_type == "DATE":
         try:
             datetime.datetime(
                 int(value[:4]), int(value[5:7]), int(value[8:10])
             )
         except ValueError:
             return (
                 f"row {row_number}: "
                 f"'{value}' not of type DATE (YYYY-MM-DD)"
             )
 
 
 def run_validator(working_directory: Path, dataset_name: str) -> list:
-    metadata_path = working_directory / f'{dataset_name}.json'
+    metadata_path = working_directory / f"{dataset_name}.json"
     sqlite_path = working_directory / f"{dataset_name}.db"
     logger.debug(
         f'Dataset "{dataset_name}" - validate consistency between '
-        'data and metadata, event-history (unit_id * start * stop)'
-        'and check for row duplicates'
+        "data and metadata, event-history (unit_id * start * stop)"
+        "and check for row duplicates"
     )
     metadata = local_storage.load_json(metadata_path)
     data_errors = _validate_data(sqlite_path, metadata)
     if len(data_errors) > 0:
-        logger.debug('Found data consistency error(s)')
+        logger.debug("Found data consistency error(s)")
         return data_errors
     else:
         logger.debug(
             f'OK - consistency validation for dataset "{dataset_name}"'
         )
         return []
```

### Comparing `microdata_validator-7.3.3/microdata_validator/steps/metadata_inliner.py` & `microdata_validator-7.3.4/microdata_validator/steps/metadata_inliner.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,16 +7,15 @@
 from microdata_validator.exceptions import ParseMetadataError
 
 
 logger = logging.getLogger()
 
 
 def run_inliner(
-    metadata_file_path: Path,
-    metadata_ref_directory: Union[None, Path]
+    metadata_file_path: Path, metadata_ref_directory: Union[None, Path]
 ) -> dict:
     def recursive_ref_insert(metadata_object: dict):
         for key, value in metadata_object.items():
             if isinstance(value, dict):
                 if "$ref" in value:
                     metadata_object[key] = local_storage.load_json(
                         metadata_ref_directory / Path(value["$ref"])
```

### Comparing `microdata_validator-7.3.3/microdata_validator/steps/metadata_reader.py` & `microdata_validator-7.3.4/microdata_validator/steps/metadata_reader.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,45 +1,44 @@
 import logging
 from pathlib import Path
 
 from microdata_validator.adapter import local_storage
 from microdata_validator.components import (
-    temporal_attributes, unit_type_variables
+    temporal_attributes,
+    unit_type_variables,
 )
 from microdata_validator.model import validate_metadata_model
 
 
 logger = logging.getLogger()
 
 
 def _insert_centralized_variable_definitions(metadata: dict):
-    metadata['identifierVariables'] = [unit_type_variables.get(
-        metadata['identifierVariables'][0]['unitType']
-    )]
-    measure_variable = metadata['measureVariables'][0]
-    if 'unitType' in measure_variable:
-        insert_measure = unit_type_variables.get(measure_variable['unitType'])
-        insert_measure['name'] = measure_variable['name']
-        insert_measure['description'] = measure_variable['description']
-        metadata['measureVariables'] = [insert_measure]
-    temporality_type = metadata['temporalityType']
-    metadata['attributeVariables'] = [
+    metadata["identifierVariables"] = [
+        unit_type_variables.get(metadata["identifierVariables"][0]["unitType"])
+    ]
+    measure_variable = metadata["measureVariables"][0]
+    if "unitType" in measure_variable:
+        insert_measure = unit_type_variables.get(measure_variable["unitType"])
+        insert_measure["name"] = measure_variable["name"]
+        insert_measure["description"] = measure_variable["description"]
+        metadata["measureVariables"] = [insert_measure]
+    temporality_type = metadata["temporalityType"]
+    metadata["attributeVariables"] = [
         temporal_attributes.generate_start_time_attribute(temporality_type),
-        temporal_attributes.generate_stop_time_attribute(temporality_type)
-    ] + metadata.get('attributeVariables', [])
+        temporal_attributes.generate_stop_time_attribute(temporality_type),
+    ] + metadata.get("attributeVariables", [])
 
 
 def run_reader(
-    dataset_name: str,
-    working_directory: Path,
-    metadata_dict: dict
+    dataset_name: str, working_directory: Path, metadata_dict: dict
 ) -> None:
-    logger.debug('Validating metadata JSON with JSON schema')
+    logger.debug("Validating metadata JSON with JSON schema")
     validate_metadata_model(metadata_dict)
     _insert_centralized_variable_definitions(metadata_dict)
-    metadata_dict['shortName'] = dataset_name
-    metadata_dict['measureVariables'][0]['shortName'] = dataset_name
+    metadata_dict["shortName"] = dataset_name
+    metadata_dict["measureVariables"][0]["shortName"] = dataset_name
 
-    logger.debug('Writing inlined metadata JSON file to working directory')
+    logger.debug("Writing inlined metadata JSON file to working directory")
     local_storage.write_json(
-        working_directory / f'{dataset_name}.json', metadata_dict
+        working_directory / f"{dataset_name}.json", metadata_dict
     )
```

### Comparing `microdata_validator-7.3.3/pyproject.toml` & `microdata_validator-7.3.4/pyproject.toml`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "microdata-validator"
-version = "7.3.3"
+version = "7.3.4"
 description = "Python package for validating datasets in the microdata platform"
 authors = ["microdata-developers"]
 license = "Apache-2.0"
 repository = 'https://github.com/statisticsnorway/microdata-validator'
 readme = 'README.md'
 
 [tool.poetry.dependencies]
@@ -12,14 +12,16 @@
 pydantic = "^1.10.4"
 
 [tool.poetry.group.dev.dependencies]
 pytest-mock = "^3.10.0"
 pytest = "^6.2.5"
 pytest-cov = "^3.0.0"
 pytest-dotenv = "^0.5.2"
-black = {version = "^22.3.0", allow-prereleases = true}
-pylint = "^2.15.3"
-pycodestyle = "^2.9.1"
+black = "^23.3.0"
+ruff = "^0.0.269"
 
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
+
+[tool.black]
+line-length = 79
```

### Comparing `microdata_validator-7.3.3/PKG-INFO` & `microdata_validator-7.3.4/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: microdata-validator
-Version: 7.3.3
+Version: 7.3.4
 Summary: Python package for validating datasets in the microdata platform
 Home-page: https://github.com/statisticsnorway/microdata-validator
 License: Apache-2.0
 Author: microdata-developers
 Requires-Python: >=3.7.2,<4.0
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3
```

