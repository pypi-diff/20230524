# Comparing `tmp/lib310-0.2.8.tar.gz` & `tmp/lib310-0.2.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lib310-0.2.8.tar", max compression
+gzip compressed data, was "lib310-0.2.9.tar", max compression
```

## Comparing `lib310-0.2.8.tar` & `lib310-0.2.9.tar`

### file list

```diff
@@ -1,51 +1,51 @@
--rw-r--r--   0        0        0     1100 2022-12-07 10:43:24.974734 lib310-0.2.8/lib310/__init__.py
--rw-r--r--   0        0        0     1423 2022-09-28 06:41:20.155194 lib310-0.2.8/lib310/_settings.py
--rw-r--r--   0        0        0      172 2022-11-21 15:26:51.496922 lib310-0.2.8/lib310/data/__init__.py
--rw-r--r--   0        0        0      390 2022-09-29 09:42:49.165629 lib310-0.2.8/lib310/data/__pycache__/__init__.cpython-310.pyc
--rw-r--r--   0        0        0     3436 2022-10-05 15:53:32.813083 lib310-0.2.8/lib310/data/__pycache__/_base.cpython-310.pyc
--rw-r--r--   0        0        0      494 2022-09-28 11:38:07.190169 lib310-0.2.8/lib310/data/__pycache__/_utils.cpython-310.pyc
--rw-r--r--   0        0        0     3095 2022-10-03 09:29:03.092362 lib310-0.2.8/lib310/data/_base.py
--rw-r--r--   0        0        0      242 2022-09-28 06:41:20.155671 lib310-0.2.8/lib310/data/_utils.py
--rw-r--r--   0        0        0     6668 2022-12-09 12:53:46.065778 lib310-0.2.8/lib310/database/__init__.py
--rw-r--r--   0        0        0     5425 2022-12-09 12:53:46.432613 lib310-0.2.8/lib310/database/__pycache__/__init__.cpython-310.pyc
--rw-r--r--   0        0        0     2674 2022-11-23 14:27:42.641550 lib310-0.2.8/lib310/database/__pycache__/_connection.cpython-310.pyc
--rw-r--r--   0        0        0     1355 2022-12-07 10:12:16.242432 lib310-0.2.8/lib310/database/__pycache__/_constants.cpython-310.pyc
--rw-r--r--   0        0        0      925 2022-11-23 14:27:42.940826 lib310-0.2.8/lib310/database/__pycache__/_functions.cpython-310.pyc
--rw-r--r--   0        0        0     3390 2022-10-05 15:58:11.836095 lib310-0.2.8/lib310/database/__pycache__/_visualize.cpython-310.pyc
--rw-r--r--   0        0        0     3791 2022-11-23 15:18:15.481486 lib310-0.2.8/lib310/database/__pycache__/client.cpython-310.pyc
--rw-r--r--   0        0        0      575 2022-09-28 11:38:05.956805 lib310-0.2.8/lib310/database/__pycache__/exceptions.cpython-310.pyc
--rw-r--r--   0        0        0     2109 2022-12-09 13:15:32.908342 lib310-0.2.8/lib310/database/__pycache__/gcs_dataset.cpython-310.pyc
--rw-r--r--   0        0        0     4078 2022-11-22 10:21:17.744323 lib310-0.2.8/lib310/database/_connection.py
--rw-r--r--   0        0        0     1009 2022-12-07 09:47:12.929323 lib310-0.2.8/lib310/database/_constants.py
--rw-r--r--   0        0        0      489 2022-11-22 10:21:17.744577 lib310-0.2.8/lib310/database/_functions.py
--rw-r--r--   0        0        0     2977 2022-10-04 09:22:04.446845 lib310-0.2.8/lib310/database/_visualize.py
--rw-r--r--   0        0        0     4191 2022-09-28 11:38:17.905696 lib310-0.2.8/lib310/database/charts/__pycache__/bubble_chart.cpython-310.pyc
--rw-r--r--   0        0        0     5339 2022-09-28 06:41:20.156786 lib310-0.2.8/lib310/database/charts/bubble_chart.py
--rw-r--r--   0        0        0     3787 2022-11-23 15:18:14.051684 lib310-0.2.8/lib310/database/client.py
--rw-r--r--   0        0        0      150 2022-09-28 06:41:20.157073 lib310-0.2.8/lib310/database/exceptions.py
--rw-r--r--   0        0        0     2123 2022-12-09 13:15:31.895865 lib310-0.2.8/lib310/database/gcs_dataset.py
--rw-r--r--   0        0        0     2146 2022-10-05 15:47:43.205995 lib310-0.2.8/lib310/lazy_loader.py
--rw-r--r--   0        0        0      147 2022-09-28 06:41:20.157266 lib310-0.2.8/lib310/machinelearning/__init__.py
--rw-r--r--   0        0        0      307 2022-09-28 11:38:18.011808 lib310-0.2.8/lib310/machinelearning/__pycache__/__init__.cpython-310.pyc
--rw-r--r--   0        0        0      806 2022-09-28 11:38:21.628658 lib310-0.2.8/lib310/machinelearning/__pycache__/_base.cpython-310.pyc
--rw-r--r--   0        0        0     2975 2022-10-05 15:53:33.009766 lib310-0.2.8/lib310/machinelearning/__pycache__/_goa.cpython-310.pyc
--rw-r--r--   0        0        0     1581 2022-09-28 11:38:21.647306 lib310-0.2.8/lib310/machinelearning/__pycache__/_io.cpython-310.pyc
--rw-r--r--   0        0        0     2207 2022-09-28 11:38:21.648512 lib310-0.2.8/lib310/machinelearning/__pycache__/_lm.cpython-310.pyc
--rw-r--r--   0        0        0      357 2022-09-28 06:41:20.157404 lib310-0.2.8/lib310/machinelearning/_base.py
--rw-r--r--   0        0        0     3023 2022-10-03 09:34:09.018879 lib310-0.2.8/lib310/machinelearning/_goa.py
--rw-r--r--   0        0        0      717 2022-09-28 06:41:20.157729 lib310-0.2.8/lib310/machinelearning/_io.py
--rw-r--r--   0        0        0     1998 2022-09-28 06:41:20.157877 lib310-0.2.8/lib310/machinelearning/_lm.py
--rw-r--r--   0        0        0      173 2022-09-28 06:41:20.158009 lib310-0.2.8/lib310/machinelearning/_mlm.py
--rw-r--r--   0        0        0      195 2022-09-28 06:41:20.158332 lib310-0.2.8/lib310/tools/__init__.py
--rw-r--r--   0        0        0      340 2022-09-28 11:38:21.649036 lib310-0.2.8/lib310/tools/__pycache__/__init__.cpython-310.pyc
--rw-r--r--   0        0        0      597 2022-09-28 11:38:21.649388 lib310-0.2.8/lib310/tools/__pycache__/_clustering.cpython-310.pyc
--rw-r--r--   0        0        0     2410 2022-09-28 11:38:24.034217 lib310-0.2.8/lib310/tools/__pycache__/_pdb.cpython-310.pyc
--rw-r--r--   0        0        0      498 2022-09-28 06:41:20.158451 lib310-0.2.8/lib310/tools/_clustering.py
--rw-r--r--   0        0        0     2309 2022-09-28 06:41:20.158578 lib310-0.2.8/lib310/tools/_pdb.py
--rw-r--r--   0        0        0      170 2022-09-28 06:41:20.158754 lib310-0.2.8/lib310/visualization/__init__.py
--rw-r--r--   0        0        0      315 2022-09-28 11:38:24.034698 lib310-0.2.8/lib310/visualization/__pycache__/__init__.cpython-310.pyc
--rw-r--r--   0        0        0     8196 2022-09-28 11:38:24.037632 lib310-0.2.8/lib310/visualization/__pycache__/_repr.cpython-310.pyc
--rw-r--r--   0        0        0     8823 2022-09-28 06:41:20.158912 lib310-0.2.8/lib310/visualization/_repr.py
--rw-r--r--   0        0        0      705 2022-12-09 13:16:17.350227 lib310-0.2.8/pyproject.toml
--rw-r--r--   0        0        0     1016 1970-01-01 00:00:00.000000 lib310-0.2.8/setup.py
--rw-r--r--   0        0        0      858 1970-01-01 00:00:00.000000 lib310-0.2.8/PKG-INFO
+-rw-r--r--   0        0        0     1100 2022-12-07 10:43:24.974734 lib310-0.2.9/lib310/__init__.py
+-rw-r--r--   0        0        0     1423 2022-09-28 06:41:20.155194 lib310-0.2.9/lib310/_settings.py
+-rw-r--r--   0        0        0      172 2022-11-21 15:26:51.496922 lib310-0.2.9/lib310/data/__init__.py
+-rw-r--r--   0        0        0      390 2022-12-09 15:24:19.612334 lib310-0.2.9/lib310/data/__pycache__/__init__.cpython-310.pyc
+-rw-r--r--   0        0        0     3436 2022-10-05 15:53:32.813083 lib310-0.2.9/lib310/data/__pycache__/_base.cpython-310.pyc
+-rw-r--r--   0        0        0      494 2022-09-28 11:38:07.190169 lib310-0.2.9/lib310/data/__pycache__/_utils.cpython-310.pyc
+-rw-r--r--   0        0        0     3095 2022-10-03 09:29:03.092362 lib310-0.2.9/lib310/data/_base.py
+-rw-r--r--   0        0        0      242 2022-09-28 06:41:20.155671 lib310-0.2.9/lib310/data/_utils.py
+-rw-r--r--   0        0        0     6746 2022-12-09 17:05:53.273516 lib310-0.2.9/lib310/database/__init__.py
+-rw-r--r--   0        0        0     5474 2022-12-09 17:05:53.369079 lib310-0.2.9/lib310/database/__pycache__/__init__.cpython-310.pyc
+-rw-r--r--   0        0        0     2674 2022-11-23 14:27:42.641550 lib310-0.2.9/lib310/database/__pycache__/_connection.cpython-310.pyc
+-rw-r--r--   0        0        0     1355 2022-12-07 10:12:16.242432 lib310-0.2.9/lib310/database/__pycache__/_constants.cpython-310.pyc
+-rw-r--r--   0        0        0      925 2022-11-23 14:27:42.940826 lib310-0.2.9/lib310/database/__pycache__/_functions.cpython-310.pyc
+-rw-r--r--   0        0        0     3390 2022-10-05 15:58:11.836095 lib310-0.2.9/lib310/database/__pycache__/_visualize.cpython-310.pyc
+-rw-r--r--   0        0        0     3791 2022-12-09 15:35:08.976055 lib310-0.2.9/lib310/database/__pycache__/client.cpython-310.pyc
+-rw-r--r--   0        0        0      575 2022-09-28 11:38:05.956805 lib310-0.2.9/lib310/database/__pycache__/exceptions.cpython-310.pyc
+-rw-r--r--   0        0        0     3231 2022-12-09 19:10:28.827544 lib310-0.2.9/lib310/database/__pycache__/gcs_dataset.cpython-310.pyc
+-rw-r--r--   0        0        0     4078 2022-11-22 10:21:17.744323 lib310-0.2.9/lib310/database/_connection.py
+-rw-r--r--   0        0        0     1009 2022-12-07 09:47:12.929323 lib310-0.2.9/lib310/database/_constants.py
+-rw-r--r--   0        0        0      489 2022-11-22 10:21:17.744577 lib310-0.2.9/lib310/database/_functions.py
+-rw-r--r--   0        0        0     2977 2022-10-04 09:22:04.446845 lib310-0.2.9/lib310/database/_visualize.py
+-rw-r--r--   0        0        0     4191 2022-09-28 11:38:17.905696 lib310-0.2.9/lib310/database/charts/__pycache__/bubble_chart.cpython-310.pyc
+-rw-r--r--   0        0        0     5339 2022-09-28 06:41:20.156786 lib310-0.2.9/lib310/database/charts/bubble_chart.py
+-rw-r--r--   0        0        0     3787 2022-12-09 15:29:15.822732 lib310-0.2.9/lib310/database/client.py
+-rw-r--r--   0        0        0      150 2022-09-28 06:41:20.157073 lib310-0.2.9/lib310/database/exceptions.py
+-rw-r--r--   0        0        0     4186 2022-12-09 19:33:58.485699 lib310-0.2.9/lib310/database/gcs_dataset.py
+-rw-r--r--   0        0        0     2146 2022-10-05 15:47:43.205995 lib310-0.2.9/lib310/lazy_loader.py
+-rw-r--r--   0        0        0      147 2022-09-28 06:41:20.157266 lib310-0.2.9/lib310/machinelearning/__init__.py
+-rw-r--r--   0        0        0      307 2022-09-28 11:38:18.011808 lib310-0.2.9/lib310/machinelearning/__pycache__/__init__.cpython-310.pyc
+-rw-r--r--   0        0        0      806 2022-09-28 11:38:21.628658 lib310-0.2.9/lib310/machinelearning/__pycache__/_base.cpython-310.pyc
+-rw-r--r--   0        0        0     2975 2022-10-05 15:53:33.009766 lib310-0.2.9/lib310/machinelearning/__pycache__/_goa.cpython-310.pyc
+-rw-r--r--   0        0        0     1581 2022-09-28 11:38:21.647306 lib310-0.2.9/lib310/machinelearning/__pycache__/_io.cpython-310.pyc
+-rw-r--r--   0        0        0     2207 2022-09-28 11:38:21.648512 lib310-0.2.9/lib310/machinelearning/__pycache__/_lm.cpython-310.pyc
+-rw-r--r--   0        0        0      357 2022-09-28 06:41:20.157404 lib310-0.2.9/lib310/machinelearning/_base.py
+-rw-r--r--   0        0        0     3023 2022-10-03 09:34:09.018879 lib310-0.2.9/lib310/machinelearning/_goa.py
+-rw-r--r--   0        0        0      717 2022-09-28 06:41:20.157729 lib310-0.2.9/lib310/machinelearning/_io.py
+-rw-r--r--   0        0        0     1998 2022-09-28 06:41:20.157877 lib310-0.2.9/lib310/machinelearning/_lm.py
+-rw-r--r--   0        0        0      173 2022-09-28 06:41:20.158009 lib310-0.2.9/lib310/machinelearning/_mlm.py
+-rw-r--r--   0        0        0      195 2022-09-28 06:41:20.158332 lib310-0.2.9/lib310/tools/__init__.py
+-rw-r--r--   0        0        0      340 2022-09-28 11:38:21.649036 lib310-0.2.9/lib310/tools/__pycache__/__init__.cpython-310.pyc
+-rw-r--r--   0        0        0      597 2022-09-28 11:38:21.649388 lib310-0.2.9/lib310/tools/__pycache__/_clustering.cpython-310.pyc
+-rw-r--r--   0        0        0     2410 2022-09-28 11:38:24.034217 lib310-0.2.9/lib310/tools/__pycache__/_pdb.cpython-310.pyc
+-rw-r--r--   0        0        0      498 2022-09-28 06:41:20.158451 lib310-0.2.9/lib310/tools/_clustering.py
+-rw-r--r--   0        0        0     2309 2022-09-28 06:41:20.158578 lib310-0.2.9/lib310/tools/_pdb.py
+-rw-r--r--   0        0        0      170 2022-09-28 06:41:20.158754 lib310-0.2.9/lib310/visualization/__init__.py
+-rw-r--r--   0        0        0      315 2022-09-28 11:38:24.034698 lib310-0.2.9/lib310/visualization/__pycache__/__init__.cpython-310.pyc
+-rw-r--r--   0        0        0     8196 2022-09-28 11:38:24.037632 lib310-0.2.9/lib310/visualization/__pycache__/_repr.cpython-310.pyc
+-rw-r--r--   0        0        0     8823 2022-09-28 06:41:20.158912 lib310-0.2.9/lib310/visualization/_repr.py
+-rw-r--r--   0        0        0      758 2022-12-09 17:05:53.266111 lib310-0.2.9/pyproject.toml
+-rw-r--r--   0        0        0     1067 1970-01-01 00:00:00.000000 lib310-0.2.9/setup.py
+-rw-r--r--   0        0        0      937 1970-01-01 00:00:00.000000 lib310-0.2.9/PKG-INFO
```

### Comparing `lib310-0.2.8/lib310/__init__.py` & `lib310-0.2.9/lib310/__init__.py`

 * *Files identical despite different names*

### Comparing `lib310-0.2.8/lib310/_settings.py` & `lib310-0.2.9/lib310/_settings.py`

 * *Files identical despite different names*

### Comparing `lib310-0.2.8/lib310/data/__pycache__/_base.cpython-310.pyc` & `lib310-0.2.9/lib310/data/__pycache__/_base.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `lib310-0.2.8/lib310/data/_base.py` & `lib310-0.2.9/lib310/data/_base.py`

 * *Files identical despite different names*

### Comparing `lib310-0.2.8/lib310/database/__init__.py` & `lib310-0.2.9/lib310/database/__init__.py`

 * *Files 3% similar despite different names*

```diff
@@ -7,16 +7,15 @@
 import hashlib
 
 
 db_connection: DatabaseConnection = None
 __db_info = 'system.info'
 __db_gcs_cache = 'system.gcs_cache'
 
-__all__ = ['fetch', 'get_table_info', 'list_datasets', 'list_tables', 'summary', 'visualize', 'db_connector',
-           'CacheResponseType']
+__all__ = ['fetch', 'get_table_info', 'list_datasets', 'list_tables', 'summary', 'visualize', 'CacheResponseType']
 def fetch(*args, **kwargs):
     global db_connection
     if db_connection is None:
         db_connection = DatabaseConnection()
 
     query_results = db_connection.query(*args, **kwargs)
     return query_results
@@ -112,14 +111,15 @@
     :param destination_format: format of the file to store in GCS
     :param days: days to keep the file in GCS
     :param ignore_hit: ignore cache hit and run the query again
     :param response_type: return response as cache info or as a dataset
     :param target_column: target column to use for the dataset
     :return: cache info or dataset
     """
+
     if response_type == CacheResponseType.DATASET and FileFormat.to_format(destination_format) == FileFormat.AVRO:
         raise ValueError("Cannot return dataset for AVRO format")
     if str is None:
         name = get_random_string(10)
 
     hashed_query = hashlib.sha1(query.encode('utf-8')).hexdigest()
     if days <= 0:
@@ -137,21 +137,21 @@
                 row = cached.iloc[0].to_dict()
     if row is not None:
         # hit happened
         row['hit'] = True
         if response_type == CacheResponseType.CACHE_INFO:
             return row
         return GCSDataset(row['uri'], target_col_name=target_column,
-                          file_format=FileFormat.to_format(destination_format))
+                          file_format=FileFormat.to_format(destination_format), size=row['total_rows'])
 
 
     table = db.client.build_temp_table()
     log.debug(f'Created table {table.table_id} in {db.client.CACHE_DATASET}')
 
-    db.client.query_to_cached_dataset(query=query, destination=table)
+    qresult = db.client.query_to_cached_dataset(query=query, destination=table)
     log.debug(f'Insert query {query} to {table.table_id}')
 
     destination_format = destination_format.upper()
     try:
         destination_format = FileFormat.to_format(destination_format)
     except KeyError:
         raise TypeError('The destination format is not supported')
@@ -165,14 +165,15 @@
             'folder': table.table_id,
             'uri': res.destination_uris[0],
             'length': res.destination_uri_file_counts[0],
             'created_at': datetime.now().isoformat(),
             'expired_at': (datetime.now() + timedelta(days=days)).isoformat(),
             'query': query,
             'hash': hashed_query,
+            'total_rows': qresult.total_rows,
             'status_code': 1
         }
         info = db.client.insert_rows_json(__db_gcs_cache, [row])
         if len(info) > 0 and len(info[0]['errors']) != 0:
             log.error(info[0]['errors'])
     except Exception as e:
         log.error(e)
@@ -180,9 +181,9 @@
     db.client.delete_table(table)
     log.debug(f'Deleted table {table.table_id} from {db.client.CACHE_DATASET}')
 
     row['hit'] = False
 
     if response_type == CacheResponseType.CACHE_INFO:
         return row
-    return GCSDataset(row['uri'], target_col_name=target_column, file_format=FileFormat.to_format(destination_format))
+    return GCSDataset(row['uri'], target_col_name=target_column, file_format=FileFormat.to_format(destination_format), size=row['total_rows'])
```

### Comparing `lib310-0.2.8/lib310/database/__pycache__/__init__.cpython-310.pyc` & `lib310-0.2.9/lib310/database/__pycache__/__init__.cpython-310.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Fri Dec  9 12:53:46 2022 UTC, .py size: 6668 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 22% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 6f0d 0d0a 0000 0000 da2f 9363 0c1a 0000  o......../.c....
+00000000: 6f0d 0d0a 0000 0000 f16a 9363 5a1a 0000  o........j.cZ...
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 000b 0000 0040 0000 0073 e200 0000 5500  .....@...s....U.
 00000030: 6400 6401 6c00 6d01 5a01 6d02 5a02 0100  d.d.l.m.Z.m.Z...
 00000040: 6400 6402 6c03 5400 6400 6403 6c04 6d05  d.d.l.T.d.d.l.m.
 00000050: 5a05 6d06 5a06 0100 6404 6405 6c07 6d07  Z.m.Z...d.d.l.m.
 00000060: 5a07 6d08 5a08 0100 6400 6406 6c09 6d0a  Z.m.Z...d.d.l.m.
 00000070: 5a0a 0100 6404 6407 6c0b 5a0c 6404 6407  Z...d.d.l.Z.d.d.
@@ -22,319 +22,322 @@
 00000150: 6f72 6d61 74da 1143 6163 6865 5265 7370  ormat..CacheResp
 00000160: 6f6e 7365 5479 7065 e900 0000 0029 02da  onseType.....)..
 00000170: 0864 6174 6574 696d 65da 0974 696d 6564  .datetime..timed
 00000180: 656c 7461 2901 da0a 4743 5344 6174 6173  elta)...GCSDatas
 00000190: 6574 4eda 0d64 625f 636f 6e6e 6563 7469  etN..db_connecti
 000001a0: 6f6e 7a0b 7379 7374 656d 2e69 6e66 6f7a  onz.system.infoz
 000001b0: 1073 7973 7465 6d2e 6763 735f 6361 6368  .system.gcs_cach
-000001c0: 6529 08da 0566 6574 6368 da0e 6765 745f  e)...fetch..get_
+000001c0: 6529 07da 0566 6574 6368 da0e 6765 745f  e)...fetch..get_
 000001d0: 7461 626c 655f 696e 666f da0d 6c69 7374  table_info..list
 000001e0: 5f64 6174 6173 6574 73da 0b6c 6973 745f  _datasets..list_
 000001f0: 7461 626c 6573 da07 7375 6d6d 6172 79da  tables..summary.
-00000200: 0976 6973 7561 6c69 7a65 da0c 6462 5f63  .visualize..db_c
-00000210: 6f6e 6e65 6374 6f72 7206 0000 0063 0000  onnectorr....c..
-00000220: 0000 0000 0000 0000 0000 0300 0000 0400  ................
-00000230: 0000 4f00 0000 7322 0000 0074 0064 0075  ..O...s"...t.d.u
-00000240: 0072 0774 0183 0061 0074 006a 027c 0069  .r.t...a.t.j.|.i
-00000250: 007c 01a4 018e 017d 027c 0253 00a9 014e  .|.....}.|.S...N
-00000260: 2903 720b 0000 0072 0200 0000 da05 7175  ).r....r......qu
-00000270: 6572 7929 03da 0461 7267 73da 066b 7761  ery)...args..kwa
-00000280: 7267 735a 0d71 7565 7279 5f72 6573 756c  rgsZ.query_resul
-00000290: 7473 a900 7217 0000 00fa 3d2f 5573 6572  ts..r.....=/User
-000002a0: 732f 7361 6d61 6e2f 446f 6375 6d65 6e74  s/saman/Document
-000002b0: 732f 3331 302f 6c69 6233 3130 2f6c 6962  s/310/lib310/lib
-000002c0: 3331 302f 6461 7461 6261 7365 2f5f 5f69  310/database/__i
-000002d0: 6e69 745f 5f2e 7079 720c 0000 0010 0000  nit__.pyr.......
-000002e0: 0073 0800 0000 0802 0601 1002 0401 720c  .s............r.
-000002f0: 0000 0063 0000 0000 0000 0000 0000 0000  ...c............
-00000300: 0100 0000 0500 0000 4b00 0000 7338 0000  ........K...s8..
-00000310: 0074 0064 0075 0072 0b74 0183 0061 0074  .t.d.u.r.t...a.t
-00000320: 00a0 04a1 0053 0074 006a 027c 00a0 0364  .....S.t.j.|...d
-00000330: 0174 006a 02a1 026b 0372 1874 0183 0061  .t.j...k.r.t...a
-00000340: 0074 00a0 04a1 0053 0029 024e da0a 7461  .t.....S.).N..ta
-00000350: 626c 655f 6e61 6d65 2905 720b 0000 0072  ble_name).r....r
-00000360: 0200 0000 7219 0000 00da 0367 6574 720d  ....r......getr.
-00000370: 0000 00a9 0172 1600 0000 7217 0000 0072  .....r....r....r
-00000380: 1700 0000 7218 0000 0072 0d00 0000 1900  ....r....r......
-00000390: 0000 730c 0000 0008 0206 0108 0414 fd06  ..s.............
-000003a0: 0108 0272 0d00 0000 6300 0000 0000 0000  ...r....c.......
-000003b0: 0000 0000 0001 0000 0003 0000 004b 0000  .............K..
-000003c0: 0073 1c00 0000 7400 6400 7500 7207 7401  .s....t.d.u.r.t.
-000003d0: 8300 6100 7402 7400 6a03 a004 a100 8301  ..a.t.t.j.......
-000003e0: 5300 7213 0000 0029 0572 0b00 0000 7202  S.r....).r....r.
-000003f0: 0000 00da 046c 6973 74da 0663 6c69 656e  .....list..clien
-00000400: 7472 0e00 0000 721b 0000 0072 1700 0000  tr....r....r....
-00000410: 7217 0000 0072 1800 0000 720e 0000 0023  r....r....r....#
-00000420: 0000 0073 0600 0000 0802 0601 0e01 720e  ...s..........r.
-00000430: 0000 0063 0000 0000 0000 0000 0000 0000  ...c............
-00000440: 0400 0000 0500 0000 4b00 0000 7382 0000  ........K...s...
-00000450: 0074 0064 0075 0072 0774 0183 0061 007c  .t.d.u.r.t...a.|
-00000460: 00a0 0264 01a1 017d 017c 0164 0075 0072  ...d...}.|.d.u.r
-00000470: 1c64 0264 0384 0074 0374 006a 04a0 05a1  .d.d...t.t.j....
-00000480: 0083 0144 0083 017d 0174 067c 0174 0383  ...D...}.t.|.t..
-00000490: 0273 2e7c 0167 017d 0174 0374 006a 04a0  .s.|.g.}.t.t.j..
-000004a0: 077c 0164 0419 00a1 0183 0153 0069 007d  .|.d.......S.i.}
-000004b0: 027c 0144 005d 0c7d 0374 0374 006a 04a0  .|.D.].}.t.t.j..
-000004c0: 077c 03a1 0183 017c 027c 033c 0071 327c  .|.....|.|.<.q2|
-000004d0: 0253 0029 054e da0b 6461 7461 7365 745f  .S.).N..dataset_
-000004e0: 6964 7363 0100 0000 0000 0000 0000 0000  idsc............
-000004f0: 0200 0000 0300 0000 5300 0000 7312 0000  ........S...s...
-00000500: 0067 007c 005d 057d 017c 016a 0091 0271  .g.|.].}.|.j...q
-00000510: 0253 0072 1700 0000 2901 da0a 6461 7461  .S.r....)...data
-00000520: 7365 745f 6964 2902 da02 2e30 da01 6472  set_id)....0..dr
-00000530: 1700 0000 7217 0000 0072 1800 0000 da0a  ....r....r......
-00000540: 3c6c 6973 7463 6f6d 703e 3200 0000 7302  <listcomp>2...s.
-00000550: 0000 0012 007a 1f6c 6973 745f 7461 626c  .....z.list_tabl
-00000560: 6573 2e3c 6c6f 6361 6c73 3e2e 3c6c 6973  es.<locals>.<lis
-00000570: 7463 6f6d 703e 7207 0000 0029 0872 0b00  tcomp>r....).r..
-00000580: 0000 7202 0000 0072 1a00 0000 721c 0000  ..r....r....r...
-00000590: 0072 1d00 0000 720e 0000 00da 0a69 7369  .r....r......isi
-000005a0: 6e73 7461 6e63 6572 0f00 0000 2904 7216  nstancer....).r.
-000005b0: 0000 0072 1e00 0000 da06 7265 7375 6c74  ...r......result
-000005c0: 721f 0000 0072 1700 0000 7217 0000 0072  r....r....r....r
-000005d0: 1800 0000 720f 0000 002a 0000 0073 1800  ....r....*...s..
-000005e0: 0000 0802 0601 0a02 0802 1801 0a02 0601  ................
-000005f0: 1401 0402 0801 1601 0401 720f 0000 0063  ..........r....c
-00000600: 0000 0000 0000 0000 0000 0000 0400 0000  ................
-00000610: 0500 0000 4b00 0000 7362 0000 0074 0083  ....K...sb...t..
-00000620: 0001 0074 016a 027d 017c 01a0 0364 0174  ...t.j.}.|...d.t
-00000630: 049b 0064 029d 03a1 01a0 05a1 007d 027c  ...d.........}.|
-00000640: 00a0 0664 03a1 017d 037c 0364 0075 0073  ...d...}.|.d.u.s
-00000650: 1e7c 0364 0475 0072 2f7c 0264 0519 00a0  .|.d.u.r/|.d....
-00000660: 0774 08a1 017c 0264 053c 0074 097c 026a  .t...|.d.<.t.|.j
-00000670: 0a64 0664 078d 0183 0101 007c 0253 0029  .d.d.......|.S.)
-00000680: 084e fa40 5345 4c45 4354 2064 6174 6173  .N.@SELECT datas
-00000690: 6574 5f6e 616d 652c 2074 6162 6c65 5f6e  et_name, table_n
-000006a0: 616d 652c 206e 756d 5f72 6f77 732c 206e  ame, num_rows, n
-000006b0: 756d 5f63 6f6c 732c 2073 697a 6520 4652  um_cols, size FR
-000006c0: 4f4d 2060 fa01 60da 0570 7269 6e74 54da  OM `..`..printT.
-000006d0: 0473 697a 6546 2901 da05 696e 6465 7829  .sizeF)...index)
-000006e0: 0b72 1200 0000 720b 0000 0072 1d00 0000  .r....r....r....
-000006f0: 7214 0000 00da 095f 5f64 625f 696e 666f  r......__db_info
-00000700: da0c 746f 5f64 6174 6166 7261 6d65 721a  ..to_dataframer.
-00000710: 0000 00da 0561 7070 6c79 5a13 7369 7a65  .....applyZ.size
-00000720: 5f74 6f5f 6162 6272 6576 6174 696f 6e72  _to_abbrevationr
-00000730: 2700 0000 5a09 746f 5f73 7472 696e 6729  '...Z.to_string)
-00000740: 0472 1600 0000 721d 0000 00da 0264 665a  .r....r......dfZ
-00000750: 0870 7269 6e74 5f69 7472 1700 0000 7217  .print_itr....r.
-00000760: 0000 0072 1800 0000 7210 0000 003e 0000  ...r....r....>..
-00000770: 0073 1000 0000 0602 0601 1601 0a02 1001  .s..............
-00000780: 1201 1001 0401 7210 0000 0063 0000 0000  ......r....c....
-00000790: 0000 0000 0000 0000 0500 0000 0500 0000  ................
-000007a0: 4b00 0000 738e 0000 007c 00a0 0064 01a1  K...s....|...d..
-000007b0: 017d 0174 0183 0001 0074 026a 037d 027c  .}.t.....t.j.}.|
-000007c0: 0164 0075 0072 207c 02a0 0464 0274 059b  .d.u.r |...d.t..
-000007d0: 0064 039d 03a1 01a0 06a1 007d 0374 077c  .d.........}.t.|
-000007e0: 0383 0101 0064 0053 007c 02a0 0464 0474  .....d.S.|...d.t
-000007f0: 059b 0064 059d 03a1 01a0 06a1 007d 037c  ...d.........}.|
-00000800: 03a0 087c 0364 0619 007c 01a0 09a1 006b  ...|.d...|.....k
-00000810: 02a1 01a0 0aa1 007d 0474 0b7c 0483 0164  .......}.t.|...d
-00000820: 076b 0172 4064 0053 0074 0c7c 047c 0183  .k.r@d.S.t.|.|..
-00000830: 0201 0064 0053 0029 084e da07 6461 7461  ...d.S.).N..data
-00000840: 7365 747a 7a0a 2020 2020 2020 2020 2020  setzz.          
-00000850: 2020 2020 2020 5345 4c45 4354 2064 6174        SELECT dat
-00000860: 6173 6574 2c20 6461 7461 7365 745f 6e61  aset, dataset_na
-00000870: 6d65 2c20 7461 626c 652c 2074 6162 6c65  me, table, table
-00000880: 5f6e 616d 652c 206e 756d 5f72 6f77 732c  _name, num_rows,
-00000890: 206e 756d 5f63 6f6c 732c 2073 697a 652c   num_cols, size,
-000008a0: 2074 7265 656d 6170 0a20 2020 2020 2020   treemap.       
-000008b0: 2020 2020 2020 2020 2046 524f 4d20 607a           FROM `z
-000008c0: 3c60 0a20 2020 2020 2020 2020 2020 2020  <`.             
-000008d0: 2020 2057 4845 5245 2074 7265 656d 6170     WHERE treemap
-000008e0: 2e73 686f 7720 3d20 7472 7565 2041 4e44  .show = true AND
-000008f0: 206e 756d 5f72 6f77 7320 3e20 3072 2500   num_rows > 0r%.
-00000900: 0000 7226 0000 005a 0c64 6174 6173 6574  ..r&...Z.dataset
-00000910: 5f6e 616d 6572 0700 0000 290d 721a 0000  _namer....).r...
-00000920: 0072 1200 0000 720b 0000 0072 1d00 0000  .r....r....r....
-00000930: 7214 0000 0072 2a00 0000 722b 0000 005a  r....r*...r+...Z
-00000940: 0d76 6973 7561 6c69 7a65 5f61 6c6c da05  .visualize_all..
-00000950: 7768 6572 65da 0575 7070 6572 da06 6472  where..upper..dr
-00000960: 6f70 6e61 da03 6c65 6e5a 1176 6973 7561  opna..lenZ.visua
-00000970: 6c69 7a65 5f64 6174 6173 6574 2905 7216  lize_dataset).r.
-00000980: 0000 00da 046e 616d 6572 1d00 0000 722d  .....namer....r-
-00000990: 0000 005a 0674 6162 6c65 7372 1700 0000  ...Z.tablesr....
-000009a0: 7217 0000 0072 1800 0000 7211 0000 004b  r....r....r....K
-000009b0: 0000 0073 2000 0000 0a01 0602 0601 0801  ...s ...........
-000009c0: 0601 0202 08fe 0403 02fd 0805 0401 1601  ................
-000009d0: 1a01 0c01 0401 0e01 7211 0000 0063 0000  ........r....c..
-000009e0: 0000 0000 0000 0000 0000 0000 0000 0200  ................
-000009f0: 0000 4300 0000 7312 0000 0074 0064 0075  ..C...s....t.d.u
-00000a00: 0072 0774 0183 0061 0074 0053 0072 1300  .r.t...a.t.S.r..
-00000a10: 0000 2902 720b 0000 0072 0200 0000 7217  ..).r....r....r.
-00000a20: 0000 0072 1700 0000 7217 0000 0072 1800  ...r....r....r..
-00000a30: 0000 7212 0000 005f 0000 0073 0600 0000  ..r...._...s....
-00000a40: 0802 0601 0401 7212 0000 00e9 0700 0000  ......r.........
-00000a50: 46da 0072 3300 0000 da12 6465 7374 696e  F..r3.....destin
-00000a60: 6174 696f 6e5f 666f 726d 6174 da04 6461  ation_format..da
-00000a70: 7973 da0a 6967 6e6f 7265 5f68 6974 da0d  ys..ignore_hit..
-00000a80: 7265 7370 6f6e 7365 5f74 7970 6563 0700  response_typec..
-00000a90: 0000 0000 0000 0000 0000 0f00 0000 0b00  ................
-00000aa0: 0000 4300 0000 73b6 0200 007c 0574 006a  ..C...s....|.t.j
-00000ab0: 016b 0272 1174 02a0 037c 02a1 0174 026a  .k.r.t...|...t.j
-00000ac0: 046b 0272 1174 0564 0183 0182 0174 0664  .k.r.t.d.....t.d
-00000ad0: 0275 0072 1974 0764 0383 017d 0174 08a0  .u.r.t.d...}.t..
-00000ae0: 097c 00a0 0a64 04a1 01a1 01a0 0ba1 007d  .|...d.........}
-00000af0: 077c 0364 056b 0172 2964 067d 0374 0c83  .|.d.k.r)d.}.t..
-00000b00: 007d 0864 027d 097c 0473 5c7c 086a 0da0  .}.d.}.|.s\|.j..
-00000b10: 0e64 07a1 01a0 0fa1 007d 0a74 107c 0a83  .d.......}.t.|..
-00000b20: 0164 056b 0472 5c7c 0aa0 117c 0a64 0819  .d.k.r\|...|.d..
-00000b30: 007c 076b 02a1 01a0 12a1 006a 1364 0967  .|.k.......j.d.g
-00000b40: 0164 0a64 0b8d 027d 0a74 107c 0a83 0164  .d.d...}.t.|...d
-00000b50: 056b 0472 5c7c 0a6a 1464 0519 00a0 15a1  .k.r\|.j.d......
-00000b60: 007d 097c 0964 0275 0172 7764 0c7c 0964  .}.|.d.u.rwd.|.d
-00000b70: 0d3c 007c 0574 006a 166b 0272 6b7c 0953  .<.|.t.j.k.rk|.S
-00000b80: 0074 177c 0964 0e19 007c 0674 02a0 037c  .t.|.d...|.t...|
-00000b90: 02a1 0164 0f8d 0353 007c 086a 0da0 18a1  ...d...S.|.j....
-00000ba0: 007d 0b74 19a0 1a64 107c 0b6a 1b9b 0064  .}.t...d.|.j...d
-00000bb0: 117c 086a 0d6a 1c9b 009d 04a1 0101 007c  .|.j.j.........|
-00000bc0: 086a 0d6a 1d7c 007c 0b64 128d 0201 0074  .j.j.|.|.d.....t
-00000bd0: 19a0 1a64 137c 009b 0064 147c 0b6a 1b9b  ...d.|...d.|.j..
-00000be0: 009d 04a1 0101 007c 02a0 1ea1 007d 027a  .......|.....}.z
-00000bf0: 0774 02a0 037c 02a1 017d 0257 006e 0b04  .t...|...}.W.n..
-00000c00: 0074 1f79 b401 0001 0001 0074 2064 1583  .t.y.......t d..
-00000c10: 0182 0177 007c 086a 0da0 217c 0b7c 017c  ...w.|.j..!|.|.|
-00000c20: 02a1 037d 0c74 19a0 1a64 167c 0b6a 1b9b  ...}.t...d.|.j..
-00000c30: 0064 177c 0b6a 1b9b 0064 187c 019b 0064  .d.|.j...d.|...d
-00000c40: 197c 029b 0064 1a9d 09a1 0101 007a 457c  .|...d.......zE|
-00000c50: 017c 0b6a 1b7c 0c6a 2264 0519 007c 0c6a  .|.j.|.j"d...|.j
-00000c60: 2364 0519 0074 24a0 25a1 00a0 26a1 0074  #d...t$.%...&..t
-00000c70: 24a0 25a1 0074 277c 0364 1b8d 0117 00a0  $.%..t'|.d......
-00000c80: 26a1 007c 007c 0764 1c64 1d9c 097d 097c  &..|.|.d.d...}.|
-00000c90: 086a 0da0 2874 297c 0967 01a1 027d 0d74  .j..(t)|.g...}.t
-00000ca0: 107c 0d83 0164 056b 0490 0172 1574 107c  .|...d.k...r.t.|
-00000cb0: 0d64 0519 0064 1e19 0083 0164 056b 0390  .d...d.....d.k..
-00000cc0: 0172 1574 19a0 2a7c 0d64 0519 0064 1e19  .r.t..*|.d...d..
-00000cd0: 00a1 0101 0057 006e 1804 0074 2b90 0179  .....W.n...t+..y
-00000ce0: 2e01 007d 0e01 007a 0b74 19a0 2a7c 0ea1  ...}...z.t..*|..
-00000cf0: 0101 0057 0059 0064 027d 0e7e 0e6e 0564  ...W.Y.d.}.~.n.d
-00000d00: 027d 0e7e 0e77 0177 007c 086a 0da0 2c7c  .}.~.w.w.|.j..,|
-00000d10: 0ba1 0101 0074 19a0 1a64 1f7c 0b6a 1b9b  .....t...d.|.j..
-00000d20: 0064 207c 086a 0d6a 1c9b 009d 04a1 0101  .d |.j.j........
-00000d30: 0064 0a7c 0964 0d3c 007c 0574 006a 166b  .d.|.d.<.|.t.j.k
-00000d40: 0290 0172 4f7c 0953 0074 177c 0964 0e19  ...rO|.S.t.|.d..
-00000d50: 007c 0674 02a0 037c 02a1 0164 0f8d 0353  .|.t...|...d...S
-00000d60: 0029 2161 0402 0000 0a20 2020 2043 6163  .)!a.....    Cac
-00000d70: 6865 2061 2071 7565 7279 2072 6573 756c  he a query resul
-00000d80: 7420 696e 2047 6f6f 676c 6520 436c 6f75  t in Google Clou
-00000d90: 6420 5374 6f72 6167 6520 2847 4353 290a  d Storage (GCS).
-00000da0: 2020 2020 3a70 6172 616d 2071 7565 7279      :param query
-00000db0: 3a20 7175 6572 7920 746f 2072 756e 206f  : query to run o
-00000dc0: 6e20 6269 6771 7565 7279 2061 6e64 2063  n bigquery and c
-00000dd0: 6163 6865 2069 6e20 4743 530a 2020 2020  ache in GCS.    
-00000de0: 3a70 6172 616d 206e 616d 653a 206e 616d  :param name: nam
-00000df0: 6520 6f66 2074 6865 2066 696c 6520 746f  e of the file to
-00000e00: 2073 746f 7265 2069 6e20 4743 530a 2020   store in GCS.  
-00000e10: 2020 3a70 6172 616d 2064 6573 7469 6e61    :param destina
-00000e20: 7469 6f6e 5f66 6f72 6d61 743a 2066 6f72  tion_format: for
-00000e30: 6d61 7420 6f66 2074 6865 2066 696c 6520  mat of the file 
-00000e40: 746f 2073 746f 7265 2069 6e20 4743 530a  to store in GCS.
-00000e50: 2020 2020 3a70 6172 616d 2064 6179 733a      :param days:
-00000e60: 2064 6179 7320 746f 206b 6565 7020 7468   days to keep th
-00000e70: 6520 6669 6c65 2069 6e20 4743 530a 2020  e file in GCS.  
-00000e80: 2020 3a70 6172 616d 2069 676e 6f72 655f    :param ignore_
-00000e90: 6869 743a 2069 676e 6f72 6520 6361 6368  hit: ignore cach
-00000ea0: 6520 6869 7420 616e 6420 7275 6e20 7468  e hit and run th
-00000eb0: 6520 7175 6572 7920 6167 6169 6e0a 2020  e query again.  
-00000ec0: 2020 3a70 6172 616d 2072 6573 706f 6e73    :param respons
-00000ed0: 655f 7479 7065 3a20 7265 7475 726e 2072  e_type: return r
-00000ee0: 6573 706f 6e73 6520 6173 2063 6163 6865  esponse as cache
-00000ef0: 2069 6e66 6f20 6f72 2061 7320 6120 6461   info or as a da
-00000f00: 7461 7365 740a 2020 2020 3a70 6172 616d  taset.    :param
-00000f10: 2074 6172 6765 745f 636f 6c75 6d6e 3a20   target_column: 
-00000f20: 7461 7267 6574 2063 6f6c 756d 6e20 746f  target column to
-00000f30: 2075 7365 2066 6f72 2074 6865 2064 6174   use for the dat
-00000f40: 6173 6574 0a20 2020 203a 7265 7475 726e  aset.    :return
-00000f50: 3a20 6361 6368 6520 696e 666f 206f 7220  : cache info or 
-00000f60: 6461 7461 7365 740a 2020 2020 7a25 4361  dataset.    z%Ca
-00000f70: 6e6e 6f74 2072 6574 7572 6e20 6461 7461  nnot return data
-00000f80: 7365 7420 666f 7220 4156 524f 2066 6f72  set for AVRO for
-00000f90: 6d61 744e e90a 0000 007a 0575 7466 2d38  matN.....z.utf-8
-00000fa0: 7207 0000 0072 3400 0000 7a38 5345 4c45  r....r4...z8SELE
-00000fb0: 4354 202a 2066 726f 6d20 6073 7973 7465  CT * from `syste
-00000fc0: 6d2e 6763 735f 6361 6368 6560 2057 4845  m.gcs_cache` WHE
-00000fd0: 5245 2073 7461 7475 735f 636f 6465 2021  RE status_code !
-00000fe0: 3d20 2d31 da04 6861 7368 da0a 6372 6561  = -1..hash..crea
-00000ff0: 7465 645f 6174 4629 02da 0262 795a 0961  ted_atF)...byZ.a
-00001000: 7363 656e 6469 6e67 54da 0368 6974 da03  scendingT..hit..
-00001010: 7572 6929 025a 0f74 6172 6765 745f 636f  uri).Z.target_co
-00001020: 6c5f 6e61 6d65 5a0b 6669 6c65 5f66 6f72  l_nameZ.file_for
-00001030: 6d61 747a 0e43 7265 6174 6564 2074 6162  matz.Created tab
-00001040: 6c65 207a 0420 696e 2029 0272 1400 0000  le z. in ).r....
-00001050: da0b 6465 7374 696e 6174 696f 6e7a 0d49  ..destinationz.I
-00001060: 6e73 6572 7420 7175 6572 7920 7a04 2074  nsert query z. t
-00001070: 6f20 7a27 5468 6520 6465 7374 696e 6174  o z'The destinat
-00001080: 696f 6e20 666f 726d 6174 2069 7320 6e6f  ion format is no
-00001090: 7420 7375 7070 6f72 7465 647a 0745 7870  t supportedz.Exp
-000010a0: 6f72 7420 7a09 2074 6f20 4743 5328 2ffa  ort z. to GCS(/.
-000010b0: 012f 7a03 5f2a 2efa 0129 2901 7237 0000  ./z._*...)).r7..
-000010c0: 0072 0100 0000 2909 7233 0000 00da 0666  .r....).r3.....f
-000010d0: 6f6c 6465 7272 3f00 0000 da06 6c65 6e67  olderr?.....leng
-000010e0: 7468 723c 0000 005a 0a65 7870 6972 6564  thr<...Z.expired
-000010f0: 5f61 7472 1400 0000 723b 0000 005a 0b73  _atr....r;...Z.s
-00001100: 7461 7475 735f 636f 6465 da06 6572 726f  tatus_code..erro
-00001110: 7273 7a0e 4465 6c65 7465 6420 7461 626c  rsz.Deleted tabl
-00001120: 6520 7a06 2066 726f 6d20 292d 7206 0000  e z. from )-r...
-00001130: 00da 0744 4154 4153 4554 7205 0000 005a  ...DATASETr....Z
-00001140: 0974 6f5f 666f 726d 6174 5a04 4156 524f  .to_formatZ.AVRO
-00001150: da0a 5661 6c75 6545 7272 6f72 da03 7374  ..ValueError..st
-00001160: 725a 1167 6574 5f72 616e 646f 6d5f 7374  rZ.get_random_st
-00001170: 7269 6e67 da07 6861 7368 6c69 62da 0473  ring..hashlib..s
-00001180: 6861 31da 0665 6e63 6f64 65da 0968 6578  ha1..encode..hex
-00001190: 6469 6765 7374 7212 0000 0072 1d00 0000  digestr....r....
-000011a0: 7214 0000 0072 2b00 0000 7232 0000 0072  r....r+...r2...r
-000011b0: 2f00 0000 7231 0000 005a 0b73 6f72 745f  /...r1...Z.sort_
-000011c0: 7661 6c75 6573 da04 696c 6f63 5a07 746f  values..ilocZ.to
-000011d0: 5f64 6963 74da 0a43 4143 4845 5f49 4e46  _dict..CACHE_INF
-000011e0: 4f72 0a00 0000 5a10 6275 696c 645f 7465  Or....Z.build_te
-000011f0: 6d70 5f74 6162 6c65 da03 6c6f 67da 0564  mp_table..log..d
-00001200: 6562 7567 da08 7461 626c 655f 6964 5a0d  ebug..table_idZ.
-00001210: 4341 4348 455f 4441 5441 5345 545a 1771  CACHE_DATASETZ.q
-00001220: 7565 7279 5f74 6f5f 6361 6368 6564 5f64  uery_to_cached_d
-00001230: 6174 6173 6574 7230 0000 00da 084b 6579  atasetr0.....Key
-00001240: 4572 726f 72da 0954 7970 6545 7272 6f72  Error..TypeError
-00001250: 5a0d 6578 706f 7274 5f74 6f5f 6763 735a  Z.export_to_gcsZ
-00001260: 1064 6573 7469 6e61 7469 6f6e 5f75 7269  .destination_uri
-00001270: 735a 1b64 6573 7469 6e61 7469 6f6e 5f75  sZ.destination_u
-00001280: 7269 5f66 696c 655f 636f 756e 7473 7208  ri_file_countsr.
-00001290: 0000 00da 036e 6f77 da09 6973 6f66 6f72  .....now..isofor
-000012a0: 6d61 7472 0900 0000 5a10 696e 7365 7274  matr....Z.insert
-000012b0: 5f72 6f77 735f 6a73 6f6e da0e 5f5f 6462  _rows_json..__db
-000012c0: 5f67 6373 5f63 6163 6865 da05 6572 726f  _gcs_cache..erro
-000012d0: 72da 0945 7863 6570 7469 6f6e 5a0c 6465  r..ExceptionZ.de
-000012e0: 6c65 7465 5f74 6162 6c65 290f 7214 0000  lete_table).r...
-000012f0: 0072 3300 0000 7236 0000 0072 3700 0000  .r3...r6...r7...
-00001300: 7238 0000 0072 3900 0000 5a0d 7461 7267  r8...r9...Z.targ
-00001310: 6574 5f63 6f6c 756d 6e5a 0c68 6173 6865  et_columnZ.hashe
-00001320: 645f 7175 6572 79da 0264 62da 0372 6f77  d_query..db..row
-00001330: da06 6361 6368 6564 da05 7461 626c 65da  ..cached..table.
-00001340: 0372 6573 da04 696e 666f da01 6572 1700  .res..info..er..
-00001350: 0000 7217 0000 0072 1800 0000 da0b 6361  ..r....r......ca
-00001360: 6368 655f 7175 6572 7966 0000 0073 7a00  che_queryf...sz.
-00001370: 0000 1a11 0801 0801 0801 1402 0801 0401  ................
-00001380: 0601 0403 0401 1001 0c01 1a01 0201 06ff  ................
-00001390: 0c02 0e01 0801 0802 0a01 0401 0a01 0801  ................
-000013a0: 06ff 0a04 1c01 1002 1801 0802 0201 0e01  ................
-000013b0: 0c01 0801 02ff 1003 2801 0202 0202 0401  ........(.......
-000013c0: 0801 0801 0a01 1401 0201 0201 0201 06f7  ................
-000013d0: 100b 2401 1201 0480 1001 1601 0880 02ff  ..$.............
-000013e0: 0c03 1c01 0802 0c02 0401 1801 7260 0000  ............r`..
-000013f0: 0029 205a 0b5f 636f 6e6e 6563 7469 6f6e  .) Z._connection
-00001400: 7202 0000 0072 0300 0000 5a0a 5f76 6973  r....r....Z._vis
-00001410: 7561 6c69 7a65 5a0a 5f63 6f6e 7374 616e  ualizeZ._constan
-00001420: 7473 7205 0000 0072 0600 0000 7208 0000  tsr....r....r...
-00001430: 0072 0900 0000 5a0b 6763 735f 6461 7461  .r....Z.gcs_data
-00001440: 7365 7472 0a00 0000 da07 6c6f 6767 696e  setr......loggin
-00001450: 6772 4f00 0000 7249 0000 0072 0b00 0000  grO...rI...r....
-00001460: da0f 5f5f 616e 6e6f 7461 7469 6f6e 735f  ..__annotations_
-00001470: 5f72 2a00 0000 7256 0000 00da 075f 5f61  _r*...rV.....__a
-00001480: 6c6c 5f5f 720c 0000 0072 0d00 0000 720e  ll__r....r....r.
-00001490: 0000 0072 0f00 0000 7210 0000 0072 1100  ...r....r....r..
-000014a0: 0000 7212 0000 00da 0343 5356 724e 0000  ..r......CSVrN..
-000014b0: 0072 4800 0000 da03 696e 74da 0462 6f6f  .rH.....int..boo
-000014c0: 6c72 6000 0000 7217 0000 0072 1700 0000  lr`...r....r....
-000014d0: 7217 0000 0072 1800 0000 da08 3c6d 6f64  r....r......<mod
-000014e0: 756c 653e 0100 0000 7344 0000 0012 0008  ule>....sD......
-000014f0: 0110 0110 010c 0108 0108 010c 0304 0104  ................
-00001500: 0108 0208 0208 0908 0a08 0708 1408 0d08  ................
-00001510: 1402 0804 0102 0102 0106 0104 fb02 0102  ................
-00001520: ff06 0202 fe02 0302 fd02 0402 fc02 050e  ................
-00001530: fb                                       .
+00000200: 0976 6973 7561 6c69 7a65 7206 0000 0063  .visualizer....c
+00000210: 0000 0000 0000 0000 0000 0000 0300 0000  ................
+00000220: 0400 0000 4f00 0000 7322 0000 0074 0064  ....O...s"...t.d
+00000230: 0075 0072 0774 0183 0061 0074 006a 027c  .u.r.t...a.t.j.|
+00000240: 0069 007c 01a4 018e 017d 027c 0253 00a9  .i.|.....}.|.S..
+00000250: 014e 2903 720b 0000 0072 0200 0000 da05  .N).r....r......
+00000260: 7175 6572 7929 03da 0461 7267 73da 066b  query)...args..k
+00000270: 7761 7267 735a 0d71 7565 7279 5f72 6573  wargsZ.query_res
+00000280: 756c 7473 a900 7216 0000 00fa 3d2f 5573  ults..r.....=/Us
+00000290: 6572 732f 7361 6d61 6e2f 446f 6375 6d65  ers/saman/Docume
+000002a0: 6e74 732f 3331 302f 6c69 6233 3130 2f6c  nts/310/lib310/l
+000002b0: 6962 3331 302f 6461 7461 6261 7365 2f5f  ib310/database/_
+000002c0: 5f69 6e69 745f 5f2e 7079 720c 0000 000f  _init__.pyr.....
+000002d0: 0000 0073 0800 0000 0802 0601 1002 0401  ...s............
+000002e0: 720c 0000 0063 0000 0000 0000 0000 0000  r....c..........
+000002f0: 0000 0100 0000 0500 0000 4b00 0000 7338  ..........K...s8
+00000300: 0000 0074 0064 0075 0072 0b74 0183 0061  ...t.d.u.r.t...a
+00000310: 0074 00a0 04a1 0053 0074 006a 027c 00a0  .t.....S.t.j.|..
+00000320: 0364 0174 006a 02a1 026b 0372 1874 0183  .d.t.j...k.r.t..
+00000330: 0061 0074 00a0 04a1 0053 0029 024e da0a  .a.t.....S.).N..
+00000340: 7461 626c 655f 6e61 6d65 2905 720b 0000  table_name).r...
+00000350: 0072 0200 0000 7218 0000 00da 0367 6574  .r....r......get
+00000360: 720d 0000 00a9 0172 1500 0000 7216 0000  r......r....r...
+00000370: 0072 1600 0000 7217 0000 0072 0d00 0000  .r....r....r....
+00000380: 1800 0000 730c 0000 0008 0206 0108 0414  ....s...........
+00000390: fd06 0108 0272 0d00 0000 6300 0000 0000  .....r....c.....
+000003a0: 0000 0000 0000 0001 0000 0003 0000 004b  ...............K
+000003b0: 0000 0073 1c00 0000 7400 6400 7500 7207  ...s....t.d.u.r.
+000003c0: 7401 8300 6100 7402 7400 6a03 a004 a100  t...a.t.t.j.....
+000003d0: 8301 5300 7212 0000 0029 0572 0b00 0000  ..S.r....).r....
+000003e0: 7202 0000 00da 046c 6973 74da 0663 6c69  r......list..cli
+000003f0: 656e 7472 0e00 0000 721a 0000 0072 1600  entr....r....r..
+00000400: 0000 7216 0000 0072 1700 0000 720e 0000  ..r....r....r...
+00000410: 0022 0000 0073 0600 0000 0802 0601 0e01  ."...s..........
+00000420: 720e 0000 0063 0000 0000 0000 0000 0000  r....c..........
+00000430: 0000 0400 0000 0500 0000 4b00 0000 7382  ..........K...s.
+00000440: 0000 0074 0064 0075 0072 0774 0183 0061  ...t.d.u.r.t...a
+00000450: 007c 00a0 0264 01a1 017d 017c 0164 0075  .|...d...}.|.d.u
+00000460: 0072 1c64 0264 0384 0074 0374 006a 04a0  .r.d.d...t.t.j..
+00000470: 05a1 0083 0144 0083 017d 0174 067c 0174  .....D...}.t.|.t
+00000480: 0383 0273 2e7c 0167 017d 0174 0374 006a  ...s.|.g.}.t.t.j
+00000490: 04a0 077c 0164 0419 00a1 0183 0153 0069  ...|.d.......S.i
+000004a0: 007d 027c 0144 005d 0c7d 0374 0374 006a  .}.|.D.].}.t.t.j
+000004b0: 04a0 077c 03a1 0183 017c 027c 033c 0071  ...|.....|.|.<.q
+000004c0: 327c 0253 0029 054e da0b 6461 7461 7365  2|.S.).N..datase
+000004d0: 745f 6964 7363 0100 0000 0000 0000 0000  t_idsc..........
+000004e0: 0000 0200 0000 0300 0000 5300 0000 7312  ..........S...s.
+000004f0: 0000 0067 007c 005d 057d 017c 016a 0091  ...g.|.].}.|.j..
+00000500: 0271 0253 0072 1600 0000 2901 da0a 6461  .q.S.r....)...da
+00000510: 7461 7365 745f 6964 2902 da02 2e30 da01  taset_id)....0..
+00000520: 6472 1600 0000 7216 0000 0072 1700 0000  dr....r....r....
+00000530: da0a 3c6c 6973 7463 6f6d 703e 3100 0000  ..<listcomp>1...
+00000540: 7302 0000 0012 007a 1f6c 6973 745f 7461  s......z.list_ta
+00000550: 626c 6573 2e3c 6c6f 6361 6c73 3e2e 3c6c  bles.<locals>.<l
+00000560: 6973 7463 6f6d 703e 7207 0000 0029 0872  istcomp>r....).r
+00000570: 0b00 0000 7202 0000 0072 1900 0000 721b  ....r....r....r.
+00000580: 0000 0072 1c00 0000 720e 0000 00da 0a69  ...r....r......i
+00000590: 7369 6e73 7461 6e63 6572 0f00 0000 2904  sinstancer....).
+000005a0: 7215 0000 0072 1d00 0000 da06 7265 7375  r....r......resu
+000005b0: 6c74 721e 0000 0072 1600 0000 7216 0000  ltr....r....r...
+000005c0: 0072 1700 0000 720f 0000 0029 0000 0073  .r....r....)...s
+000005d0: 1800 0000 0802 0601 0a02 0802 1801 0a02  ................
+000005e0: 0601 1401 0402 0801 1601 0401 720f 0000  ............r...
+000005f0: 0063 0000 0000 0000 0000 0000 0000 0400  .c..............
+00000600: 0000 0500 0000 4b00 0000 7362 0000 0074  ......K...sb...t
+00000610: 0083 0001 0074 016a 027d 017c 01a0 0364  .....t.j.}.|...d
+00000620: 0174 049b 0064 029d 03a1 01a0 05a1 007d  .t...d.........}
+00000630: 027c 00a0 0664 03a1 017d 037c 0364 0075  .|...d...}.|.d.u
+00000640: 0073 1e7c 0364 0475 0072 2f7c 0264 0519  .s.|.d.u.r/|.d..
+00000650: 00a0 0774 08a1 017c 0264 053c 0074 097c  ...t...|.d.<.t.|
+00000660: 026a 0a64 0664 078d 0183 0101 007c 0253  .j.d.d.......|.S
+00000670: 0029 084e fa40 5345 4c45 4354 2064 6174  .).N.@SELECT dat
+00000680: 6173 6574 5f6e 616d 652c 2074 6162 6c65  aset_name, table
+00000690: 5f6e 616d 652c 206e 756d 5f72 6f77 732c  _name, num_rows,
+000006a0: 206e 756d 5f63 6f6c 732c 2073 697a 6520   num_cols, size 
+000006b0: 4652 4f4d 2060 fa01 60da 0570 7269 6e74  FROM `..`..print
+000006c0: 54da 0473 697a 6546 2901 da05 696e 6465  T..sizeF)...inde
+000006d0: 7829 0bda 0c64 625f 636f 6e6e 6563 746f  x)...db_connecto
+000006e0: 7272 0b00 0000 721c 0000 0072 1300 0000  rr....r....r....
+000006f0: da09 5f5f 6462 5f69 6e66 6fda 0c74 6f5f  ..__db_info..to_
+00000700: 6461 7461 6672 616d 6572 1900 0000 5a05  dataframer....Z.
+00000710: 6170 706c 795a 1373 697a 655f 746f 5f61  applyZ.size_to_a
+00000720: 6262 7265 7661 7469 6f6e 7226 0000 005a  bbrevationr&...Z
+00000730: 0974 6f5f 7374 7269 6e67 2904 7215 0000  .to_string).r...
+00000740: 0072 1c00 0000 da02 6466 5a08 7072 696e  .r......dfZ.prin
+00000750: 745f 6974 7216 0000 0072 1600 0000 7217  t_itr....r....r.
+00000760: 0000 0072 1000 0000 3d00 0000 7310 0000  ...r....=...s...
+00000770: 0006 0206 0116 010a 0210 0112 0110 0104  ................
+00000780: 0172 1000 0000 6300 0000 0000 0000 0000  .r....c.........
+00000790: 0000 0005 0000 0005 0000 004b 0000 0073  ...........K...s
+000007a0: 8e00 0000 7c00 a000 6401 a101 7d01 7401  ....|...d...}.t.
+000007b0: 8300 0100 7402 6a03 7d02 7c01 6400 7500  ....t.j.}.|.d.u.
+000007c0: 7220 7c02 a004 6402 7405 9b00 6403 9d03  r |...d.t...d...
+000007d0: a101 a006 a100 7d03 7407 7c03 8301 0100  ......}.t.|.....
+000007e0: 6400 5300 7c02 a004 6404 7405 9b00 6405  d.S.|...d.t...d.
+000007f0: 9d03 a101 a006 a100 7d03 7c03 a008 7c03  ........}.|...|.
+00000800: 6406 1900 7c01 a009 a100 6b02 a101 a00a  d...|.....k.....
+00000810: a100 7d04 740b 7c04 8301 6407 6b01 7240  ..}.t.|...d.k.r@
+00000820: 6400 5300 740c 7c04 7c01 8302 0100 6400  d.S.t.|.|.....d.
+00000830: 5300 2908 4e5a 0764 6174 6173 6574 7a7a  S.).NZ.datasetzz
+00000840: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00000850: 2053 454c 4543 5420 6461 7461 7365 742c   SELECT dataset,
+00000860: 2064 6174 6173 6574 5f6e 616d 652c 2074   dataset_name, t
+00000870: 6162 6c65 2c20 7461 626c 655f 6e61 6d65  able, table_name
+00000880: 2c20 6e75 6d5f 726f 7773 2c20 6e75 6d5f  , num_rows, num_
+00000890: 636f 6c73 2c20 7369 7a65 2c20 7472 6565  cols, size, tree
+000008a0: 6d61 700a 2020 2020 2020 2020 2020 2020  map.            
+000008b0: 2020 2020 4652 4f4d 2060 7a3c 600a 2020      FROM `z<`.  
+000008c0: 2020 2020 2020 2020 2020 2020 2020 5748                WH
+000008d0: 4552 4520 7472 6565 6d61 702e 7368 6f77  ERE treemap.show
+000008e0: 203d 2074 7275 6520 414e 4420 6e75 6d5f   = true AND num_
+000008f0: 726f 7773 203e 2030 7224 0000 0072 2500  rows > 0r$...r%.
+00000900: 0000 5a0c 6461 7461 7365 745f 6e61 6d65  ..Z.dataset_name
+00000910: 7207 0000 0029 0d72 1900 0000 7229 0000  r....).r....r)..
+00000920: 0072 0b00 0000 721c 0000 0072 1300 0000  .r....r....r....
+00000930: 722a 0000 0072 2b00 0000 5a0d 7669 7375  r*...r+...Z.visu
+00000940: 616c 697a 655f 616c 6cda 0577 6865 7265  alize_all..where
+00000950: da05 7570 7065 72da 0664 726f 706e 61da  ..upper..dropna.
+00000960: 036c 656e 5a11 7669 7375 616c 697a 655f  .lenZ.visualize_
+00000970: 6461 7461 7365 7429 0572 1500 0000 da04  dataset).r......
+00000980: 6e61 6d65 721c 0000 0072 2c00 0000 5a06  namer....r,...Z.
+00000990: 7461 626c 6573 7216 0000 0072 1600 0000  tablesr....r....
+000009a0: 7217 0000 0072 1100 0000 4a00 0000 7320  r....r....J...s 
+000009b0: 0000 000a 0106 0206 0108 0106 0102 0208  ................
+000009c0: fe04 0302 fd08 0504 0116 011a 010c 0104  ................
+000009d0: 010e 0172 1100 0000 6300 0000 0000 0000  ...r....c.......
+000009e0: 0000 0000 0000 0000 0002 0000 0043 0000  .............C..
+000009f0: 0073 1200 0000 7400 6400 7500 7207 7401  .s....t.d.u.r.t.
+00000a00: 8300 6100 7400 5300 7212 0000 0029 0272  ..a.t.S.r....).r
+00000a10: 0b00 0000 7202 0000 0072 1600 0000 7216  ....r....r....r.
+00000a20: 0000 0072 1600 0000 7217 0000 0072 2900  ...r....r....r).
+00000a30: 0000 5e00 0000 7306 0000 0008 0206 0104  ..^...s.........
+00000a40: 0172 2900 0000 e907 0000 0046 da00 7231  .r)........F..r1
+00000a50: 0000 00da 1264 6573 7469 6e61 7469 6f6e  .....destination
+00000a60: 5f66 6f72 6d61 74da 0464 6179 73da 0a69  _format..days..i
+00000a70: 676e 6f72 655f 6869 74da 0d72 6573 706f  gnore_hit..respo
+00000a80: 6e73 655f 7479 7065 6307 0000 0000 0000  nse_typec.......
+00000a90: 0000 0000 0010 0000 000b 0000 0043 0000  .............C..
+00000aa0: 0073 c602 0000 7c05 7400 6a01 6b02 7211  .s....|.t.j.k.r.
+00000ab0: 7402 a003 7c02 a101 7402 6a04 6b02 7211  t...|...t.j.k.r.
+00000ac0: 7405 6401 8301 8201 7406 6402 7500 7219  t.d.....t.d.u.r.
+00000ad0: 7407 6403 8301 7d01 7408 a009 7c00 a00a  t.d...}.t...|...
+00000ae0: 6404 a101 a101 a00b a100 7d07 7c03 6405  d.........}.|.d.
+00000af0: 6b01 7229 6406 7d03 740c 8300 7d08 6402  k.r)d.}.t...}.d.
+00000b00: 7d09 7c04 735c 7c08 6a0d a00e 6407 a101  }.|.s\|.j...d...
+00000b10: a00f a100 7d0a 7410 7c0a 8301 6405 6b04  ....}.t.|...d.k.
+00000b20: 725c 7c0a a011 7c0a 6408 1900 7c07 6b02  r\|...|.d...|.k.
+00000b30: a101 a012 a100 6a13 6409 6701 640a 640b  ......j.d.g.d.d.
+00000b40: 8d02 7d0a 7410 7c0a 8301 6405 6b04 725c  ..}.t.|...d.k.r\
+00000b50: 7c0a 6a14 6405 1900 a015 a100 7d09 7c09  |.j.d.......}.|.
+00000b60: 6402 7501 727a 640c 7c09 640d 3c00 7c05  d.u.rzd.|.d.<.|.
+00000b70: 7400 6a16 6b02 726b 7c09 5300 7417 7c09  t.j.k.rk|.S.t.|.
+00000b80: 640e 1900 7c06 7402 a003 7c02 a101 7c09  d...|.t...|...|.
+00000b90: 640f 1900 6410 8d04 5300 7c08 6a0d a018  d...d...S.|.j...
+00000ba0: a100 7d0b 7419 a01a 6411 7c0b 6a1b 9b00  ..}.t...d.|.j...
+00000bb0: 6412 7c08 6a0d 6a1c 9b00 9d04 a101 0100  d.|.j.j.........
+00000bc0: 7c08 6a0d 6a1d 7c00 7c0b 6413 8d02 7d0c  |.j.j.|.|.d...}.
+00000bd0: 7419 a01a 6414 7c00 9b00 6415 7c0b 6a1b  t...d.|...d.|.j.
+00000be0: 9b00 9d04 a101 0100 7c02 a01e a100 7d02  ........|.....}.
+00000bf0: 7a07 7402 a003 7c02 a101 7d02 5700 6e0b  z.t...|...}.W.n.
+00000c00: 0400 741f 79b7 0100 0100 0100 7420 6416  ..t.y.......t d.
+00000c10: 8301 8201 7700 7c08 6a0d a021 7c0b 7c01  ....w.|.j..!|.|.
+00000c20: 7c02 a103 7d0d 7419 a01a 6417 7c0b 6a1b  |...}.t...d.|.j.
+00000c30: 9b00 6418 7c0b 6a1b 9b00 6419 7c01 9b00  ..d.|.j...d.|...
+00000c40: 641a 7c02 9b00 641b 9d09 a101 0100 7a47  d.|...d.......zG
+00000c50: 7c01 7c0b 6a1b 7c0d 6a22 6405 1900 7c0d  |.|.j.|.j"d...|.
+00000c60: 6a23 6405 1900 7424 a025 a100 a026 a100  j#d...t$.%...&..
+00000c70: 7424 a025 a100 7427 7c03 641c 8d01 1700  t$.%..t'|.d.....
+00000c80: a026 a100 7c00 7c07 7c0c 6a28 641d 641e  .&..|.|.|.j(d.d.
+00000c90: 9c0a 7d09 7c08 6a0d a029 742a 7c09 6701  ..}.|.j..)t*|.g.
+00000ca0: a102 7d0e 7410 7c0e 8301 6405 6b04 9001  ..}.t.|...d.k...
+00000cb0: 721a 7410 7c0e 6405 1900 641f 1900 8301  r.t.|.d...d.....
+00000cc0: 6405 6b03 9001 721a 7419 a02b 7c0e 6405  d.k...r.t..+|.d.
+00000cd0: 1900 641f 1900 a101 0100 5700 6e18 0400  ..d.......W.n...
+00000ce0: 742c 9001 7933 0100 7d0f 0100 7a0b 7419  t,..y3..}...z.t.
+00000cf0: a02b 7c0f a101 0100 5700 5900 6402 7d0f  .+|.....W.Y.d.}.
+00000d00: 7e0f 6e05 6402 7d0f 7e0f 7701 7700 7c08  ~.n.d.}.~.w.w.|.
+00000d10: 6a0d a02d 7c0b a101 0100 7419 a01a 6420  j..-|.....t...d 
+00000d20: 7c0b 6a1b 9b00 6421 7c08 6a0d 6a1c 9b00  |.j...d!|.j.j...
+00000d30: 9d04 a101 0100 640a 7c09 640d 3c00 7c05  ......d.|.d.<.|.
+00000d40: 7400 6a16 6b02 9001 7254 7c09 5300 7417  t.j.k...rT|.S.t.
+00000d50: 7c09 640e 1900 7c06 7402 a003 7c02 a101  |.d...|.t...|...
+00000d60: 7c09 640f 1900 6410 8d04 5300 2922 6104  |.d...d...S.)"a.
+00000d70: 0200 000a 2020 2020 4361 6368 6520 6120  ....    Cache a 
+00000d80: 7175 6572 7920 7265 7375 6c74 2069 6e20  query result in 
+00000d90: 476f 6f67 6c65 2043 6c6f 7564 2053 746f  Google Cloud Sto
+00000da0: 7261 6765 2028 4743 5329 0a20 2020 203a  rage (GCS).    :
+00000db0: 7061 7261 6d20 7175 6572 793a 2071 7565  param query: que
+00000dc0: 7279 2074 6f20 7275 6e20 6f6e 2062 6967  ry to run on big
+00000dd0: 7175 6572 7920 616e 6420 6361 6368 6520  query and cache 
+00000de0: 696e 2047 4353 0a20 2020 203a 7061 7261  in GCS.    :para
+00000df0: 6d20 6e61 6d65 3a20 6e61 6d65 206f 6620  m name: name of 
+00000e00: 7468 6520 6669 6c65 2074 6f20 7374 6f72  the file to stor
+00000e10: 6520 696e 2047 4353 0a20 2020 203a 7061  e in GCS.    :pa
+00000e20: 7261 6d20 6465 7374 696e 6174 696f 6e5f  ram destination_
+00000e30: 666f 726d 6174 3a20 666f 726d 6174 206f  format: format o
+00000e40: 6620 7468 6520 6669 6c65 2074 6f20 7374  f the file to st
+00000e50: 6f72 6520 696e 2047 4353 0a20 2020 203a  ore in GCS.    :
+00000e60: 7061 7261 6d20 6461 7973 3a20 6461 7973  param days: days
+00000e70: 2074 6f20 6b65 6570 2074 6865 2066 696c   to keep the fil
+00000e80: 6520 696e 2047 4353 0a20 2020 203a 7061  e in GCS.    :pa
+00000e90: 7261 6d20 6967 6e6f 7265 5f68 6974 3a20  ram ignore_hit: 
+00000ea0: 6967 6e6f 7265 2063 6163 6865 2068 6974  ignore cache hit
+00000eb0: 2061 6e64 2072 756e 2074 6865 2071 7565   and run the que
+00000ec0: 7279 2061 6761 696e 0a20 2020 203a 7061  ry again.    :pa
+00000ed0: 7261 6d20 7265 7370 6f6e 7365 5f74 7970  ram response_typ
+00000ee0: 653a 2072 6574 7572 6e20 7265 7370 6f6e  e: return respon
+00000ef0: 7365 2061 7320 6361 6368 6520 696e 666f  se as cache info
+00000f00: 206f 7220 6173 2061 2064 6174 6173 6574   or as a dataset
+00000f10: 0a20 2020 203a 7061 7261 6d20 7461 7267  .    :param targ
+00000f20: 6574 5f63 6f6c 756d 6e3a 2074 6172 6765  et_column: targe
+00000f30: 7420 636f 6c75 6d6e 2074 6f20 7573 6520  t column to use 
+00000f40: 666f 7220 7468 6520 6461 7461 7365 740a  for the dataset.
+00000f50: 2020 2020 3a72 6574 7572 6e3a 2063 6163      :return: cac
+00000f60: 6865 2069 6e66 6f20 6f72 2064 6174 6173  he info or datas
+00000f70: 6574 0a20 2020 207a 2543 616e 6e6f 7420  et.    z%Cannot 
+00000f80: 7265 7475 726e 2064 6174 6173 6574 2066  return dataset f
+00000f90: 6f72 2041 5652 4f20 666f 726d 6174 4ee9  or AVRO formatN.
+00000fa0: 0a00 0000 7a05 7574 662d 3872 0700 0000  ....z.utf-8r....
+00000fb0: 7232 0000 007a 3853 454c 4543 5420 2a20  r2...z8SELECT * 
+00000fc0: 6672 6f6d 2060 7379 7374 656d 2e67 6373  from `system.gcs
+00000fd0: 5f63 6163 6865 6020 5748 4552 4520 7374  _cache` WHERE st
+00000fe0: 6174 7573 5f63 6f64 6520 213d 202d 31da  atus_code != -1.
+00000ff0: 0468 6173 68da 0a63 7265 6174 6564 5f61  .hash..created_a
+00001000: 7446 2902 5a02 6279 5a09 6173 6365 6e64  tF).Z.byZ.ascend
+00001010: 696e 6754 5a03 6869 74da 0375 7269 da0a  ingTZ.hit..uri..
+00001020: 746f 7461 6c5f 726f 7773 2903 5a0f 7461  total_rows).Z.ta
+00001030: 7267 6574 5f63 6f6c 5f6e 616d 65da 0b66  rget_col_name..f
+00001040: 696c 655f 666f 726d 6174 7227 0000 007a  ile_formatr'...z
+00001050: 0e43 7265 6174 6564 2074 6162 6c65 207a  .Created table z
+00001060: 0420 696e 2029 0272 1300 0000 5a0b 6465  . in ).r....Z.de
+00001070: 7374 696e 6174 696f 6e7a 0d49 6e73 6572  stinationz.Inser
+00001080: 7420 7175 6572 7920 7a04 2074 6f20 7a27  t query z. to z'
+00001090: 5468 6520 6465 7374 696e 6174 696f 6e20  The destination 
+000010a0: 666f 726d 6174 2069 7320 6e6f 7420 7375  format is not su
+000010b0: 7070 6f72 7465 647a 0745 7870 6f72 7420  pportedz.Export 
+000010c0: 7a09 2074 6f20 4743 5328 2ffa 012f 7a03  z. to GCS(/../z.
+000010d0: 5f2a 2efa 0129 2901 7235 0000 0072 0100  _*...)).r5...r..
+000010e0: 0000 290a 7231 0000 00da 0666 6f6c 6465  ..).r1.....folde
+000010f0: 7272 3b00 0000 da06 6c65 6e67 7468 723a  rr;.....lengthr:
+00001100: 0000 005a 0a65 7870 6972 6564 5f61 7472  ...Z.expired_atr
+00001110: 1300 0000 7239 0000 0072 3c00 0000 5a0b  ....r9...r<...Z.
+00001120: 7374 6174 7573 5f63 6f64 65da 0665 7272  status_code..err
+00001130: 6f72 737a 0e44 656c 6574 6564 2074 6162  orsz.Deleted tab
+00001140: 6c65 207a 0620 6672 6f6d 2029 2e72 0600  le z. from ).r..
+00001150: 0000 da07 4441 5441 5345 5472 0500 0000  ....DATASETr....
+00001160: 5a09 746f 5f66 6f72 6d61 745a 0441 5652  Z.to_formatZ.AVR
+00001170: 4fda 0a56 616c 7565 4572 726f 72da 0373  O..ValueError..s
+00001180: 7472 5a11 6765 745f 7261 6e64 6f6d 5f73  trZ.get_random_s
+00001190: 7472 696e 67da 0768 6173 686c 6962 5a04  tring..hashlibZ.
+000011a0: 7368 6131 da06 656e 636f 6465 da09 6865  sha1..encode..he
+000011b0: 7864 6967 6573 7472 2900 0000 721c 0000  xdigestr)...r...
+000011c0: 0072 1300 0000 722b 0000 0072 3000 0000  .r....r+...r0...
+000011d0: 722d 0000 0072 2f00 0000 5a0b 736f 7274  r-...r/...Z.sort
+000011e0: 5f76 616c 7565 735a 0469 6c6f 635a 0774  _valuesZ.ilocZ.t
+000011f0: 6f5f 6469 6374 da0a 4341 4348 455f 494e  o_dict..CACHE_IN
+00001200: 464f 720a 0000 005a 1062 7569 6c64 5f74  FOr....Z.build_t
+00001210: 656d 705f 7461 626c 65da 036c 6f67 da05  emp_table..log..
+00001220: 6465 6275 67da 0874 6162 6c65 5f69 645a  debug..table_idZ
+00001230: 0d43 4143 4845 5f44 4154 4153 4554 5a17  .CACHE_DATASETZ.
+00001240: 7175 6572 795f 746f 5f63 6163 6865 645f  query_to_cached_
+00001250: 6461 7461 7365 7472 2e00 0000 da08 4b65  datasetr......Ke
+00001260: 7945 7272 6f72 da09 5479 7065 4572 726f  yError..TypeErro
+00001270: 725a 0d65 7870 6f72 745f 746f 5f67 6373  rZ.export_to_gcs
+00001280: 5a10 6465 7374 696e 6174 696f 6e5f 7572  Z.destination_ur
+00001290: 6973 5a1b 6465 7374 696e 6174 696f 6e5f  isZ.destination_
+000012a0: 7572 695f 6669 6c65 5f63 6f75 6e74 7372  uri_file_countsr
+000012b0: 0800 0000 da03 6e6f 77da 0969 736f 666f  ......now..isofo
+000012c0: 726d 6174 7209 0000 0072 3c00 0000 5a10  rmatr....r<...Z.
+000012d0: 696e 7365 7274 5f72 6f77 735f 6a73 6f6e  insert_rows_json
+000012e0: da0e 5f5f 6462 5f67 6373 5f63 6163 6865  ..__db_gcs_cache
+000012f0: da05 6572 726f 72da 0945 7863 6570 7469  ..error..Excepti
+00001300: 6f6e 5a0c 6465 6c65 7465 5f74 6162 6c65  onZ.delete_table
+00001310: 2910 7213 0000 0072 3100 0000 7234 0000  ).r....r1...r4..
+00001320: 0072 3500 0000 7236 0000 0072 3700 0000  .r5...r6...r7...
+00001330: 5a0d 7461 7267 6574 5f63 6f6c 756d 6e5a  Z.target_columnZ
+00001340: 0c68 6173 6865 645f 7175 6572 79da 0264  .hashed_query..d
+00001350: 62da 0372 6f77 da06 6361 6368 6564 da05  b..row..cached..
+00001360: 7461 626c 655a 0771 7265 7375 6c74 da03  tableZ.qresult..
+00001370: 7265 73da 0469 6e66 6fda 0165 7216 0000  res..info..er...
+00001380: 0072 1600 0000 7217 0000 00da 0b63 6163  .r....r......cac
+00001390: 6865 5f71 7565 7279 6500 0000 737c 0000  he_querye...s|..
+000013a0: 001a 1208 0108 0108 0114 0208 0104 0106  ................
+000013b0: 0104 0304 0110 010c 011a 0102 0106 ff0c  ................
+000013c0: 020e 0108 0108 020a 0104 010a 010e 0106  ................
+000013d0: ff0a 041c 0110 0218 0108 0202 010e 010c  ................
+000013e0: 0108 0102 ff10 0328 0102 0202 0204 0108  .......(........
+000013f0: 0108 010a 0114 0102 0102 0104 0102 0106  ................
+00001400: f610 0c24 0112 0104 8010 0116 0108 8002  ...$............
+00001410: ff0c 031c 0108 020c 0204 011e 0172 5b00  .............r[.
+00001420: 0000 2920 5a0b 5f63 6f6e 6e65 6374 696f  ..) Z._connectio
+00001430: 6e72 0200 0000 7203 0000 005a 0a5f 7669  nr....r....Z._vi
+00001440: 7375 616c 697a 655a 0a5f 636f 6e73 7461  sualizeZ._consta
+00001450: 6e74 7372 0500 0000 7206 0000 0072 0800  ntsr....r....r..
+00001460: 0000 7209 0000 005a 0b67 6373 5f64 6174  ..r....Z.gcs_dat
+00001470: 6173 6574 720a 0000 00da 076c 6f67 6769  asetr......loggi
+00001480: 6e67 724a 0000 0072 4600 0000 720b 0000  ngrJ...rF...r...
+00001490: 00da 0f5f 5f61 6e6e 6f74 6174 696f 6e73  ...__annotations
+000014a0: 5f5f 722a 0000 0072 5100 0000 da07 5f5f  __r*...rQ.....__
+000014b0: 616c 6c5f 5f72 0c00 0000 720d 0000 0072  all__r....r....r
+000014c0: 0e00 0000 720f 0000 0072 1000 0000 7211  ....r....r....r.
+000014d0: 0000 0072 2900 0000 5a03 4353 5672 4900  ...r)...Z.CSVrI.
+000014e0: 0000 7245 0000 00da 0369 6e74 da04 626f  ..rE.....int..bo
+000014f0: 6f6c 725b 0000 0072 1600 0000 7216 0000  olr[...r....r...
+00001500: 0072 1600 0000 7217 0000 00da 083c 6d6f  .r....r......<mo
+00001510: 6475 6c65 3e01 0000 0073 4400 0000 1200  dule>....sD.....
+00001520: 0801 1001 1001 0c01 0801 0801 0c03 0401  ................
+00001530: 0401 0802 0801 0809 080a 0807 0814 080d  ................
+00001540: 0814 0208 0401 0201 0201 0601 04fb 0201  ................
+00001550: 02ff 0602 02fe 0203 02fd 0204 02fc 0205  ................
+00001560: 0efb                                     ..
```

### Comparing `lib310-0.2.8/lib310/database/__pycache__/_connection.cpython-310.pyc` & `lib310-0.2.9/lib310/database/__pycache__/_connection.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `lib310-0.2.8/lib310/database/__pycache__/_constants.cpython-310.pyc` & `lib310-0.2.9/lib310/database/__pycache__/_constants.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `lib310-0.2.8/lib310/database/__pycache__/_functions.cpython-310.pyc` & `lib310-0.2.9/lib310/database/__pycache__/_functions.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `lib310-0.2.8/lib310/database/__pycache__/_visualize.cpython-310.pyc` & `lib310-0.2.9/lib310/database/__pycache__/_visualize.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `lib310-0.2.8/lib310/database/__pycache__/client.cpython-310.pyc` & `lib310-0.2.9/lib310/database/__pycache__/client.cpython-310.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Wed Nov 23 15:18:14 2022 UTC, .py size: 3787 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 6f0d 0d0a 0000 0000 b639 7e63 cb0e 0000  o........9~c....
+00000000: 6f0d 0d0a 0000 0000 4b54 9363 cb0e 0000  o.......KT.c....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0004 0000 0040 0000 0073 7a00 0000 6400  .....@...sz...d.
 00000030: 6401 6c00 6d01 5a01 0100 6400 6402 6c02  d.l.m.Z...d.d.l.
 00000040: 6d03 5a04 0100 6400 6403 6c02 6d05 5a05  m.Z...d.d.l.m.Z.
 00000050: 0100 6400 6404 6c06 6d07 5a07 6d08 5a08  ..d.d.l.m.Z.m.Z.
 00000060: 0100 6405 6406 6c09 6d0a 5a0a 0100 6405  ..d.d.l.m.Z...d.
 00000070: 6407 6c0b 6d0c 5a0c 0100 6400 6408 6c0d  d.l.m.Z...d.d.l.
```

### Comparing `lib310-0.2.8/lib310/database/__pycache__/exceptions.cpython-310.pyc` & `lib310-0.2.9/lib310/database/__pycache__/exceptions.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `lib310-0.2.8/lib310/database/_connection.py` & `lib310-0.2.9/lib310/database/_connection.py`

 * *Files identical despite different names*

### Comparing `lib310-0.2.8/lib310/database/_constants.py` & `lib310-0.2.9/lib310/database/_constants.py`

 * *Files identical despite different names*

### Comparing `lib310-0.2.8/lib310/database/_visualize.py` & `lib310-0.2.9/lib310/database/_visualize.py`

 * *Files identical despite different names*

### Comparing `lib310-0.2.8/lib310/database/charts/__pycache__/bubble_chart.cpython-310.pyc` & `lib310-0.2.9/lib310/database/charts/__pycache__/bubble_chart.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `lib310-0.2.8/lib310/database/charts/bubble_chart.py` & `lib310-0.2.9/lib310/database/charts/bubble_chart.py`

 * *Files identical despite different names*

### Comparing `lib310-0.2.8/lib310/database/client.py` & `lib310-0.2.9/lib310/database/client.py`

 * *Files identical despite different names*

### Comparing `lib310-0.2.8/lib310/lazy_loader.py` & `lib310-0.2.9/lib310/lazy_loader.py`

 * *Files identical despite different names*

### Comparing `lib310-0.2.8/lib310/machinelearning/__pycache__/_base.cpython-310.pyc` & `lib310-0.2.9/lib310/machinelearning/__pycache__/_base.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `lib310-0.2.8/lib310/machinelearning/__pycache__/_goa.cpython-310.pyc` & `lib310-0.2.9/lib310/machinelearning/__pycache__/_goa.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `lib310-0.2.8/lib310/machinelearning/__pycache__/_io.cpython-310.pyc` & `lib310-0.2.9/lib310/machinelearning/__pycache__/_io.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `lib310-0.2.8/lib310/machinelearning/__pycache__/_lm.cpython-310.pyc` & `lib310-0.2.9/lib310/machinelearning/__pycache__/_lm.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `lib310-0.2.8/lib310/machinelearning/_goa.py` & `lib310-0.2.9/lib310/machinelearning/_goa.py`

 * *Files identical despite different names*

### Comparing `lib310-0.2.8/lib310/machinelearning/_io.py` & `lib310-0.2.9/lib310/machinelearning/_io.py`

 * *Files identical despite different names*

### Comparing `lib310-0.2.8/lib310/machinelearning/_lm.py` & `lib310-0.2.9/lib310/machinelearning/_lm.py`

 * *Files identical despite different names*

### Comparing `lib310-0.2.8/lib310/tools/__pycache__/_clustering.cpython-310.pyc` & `lib310-0.2.9/lib310/tools/__pycache__/_clustering.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `lib310-0.2.8/lib310/tools/__pycache__/_pdb.cpython-310.pyc` & `lib310-0.2.9/lib310/tools/__pycache__/_pdb.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `lib310-0.2.8/lib310/tools/_pdb.py` & `lib310-0.2.9/lib310/tools/_pdb.py`

 * *Files identical despite different names*

### Comparing `lib310-0.2.8/lib310/visualization/__pycache__/_repr.cpython-310.pyc` & `lib310-0.2.9/lib310/visualization/__pycache__/_repr.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `lib310-0.2.8/lib310/visualization/_repr.py` & `lib310-0.2.9/lib310/visualization/_repr.py`

 * *Files identical despite different names*

### Comparing `lib310-0.2.8/pyproject.toml` & `lib310-0.2.9/pyproject.toml`

 * *Files 17% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "lib310"
-version = "0.2.8"
+version = "0.2.9"
 description = "lib310 Python Package"
 authors = ["Mohsen Naghipourfar <naghipourfar@berkeley.edu>", "Saman Fekri <saman@310.ai>", "Ismail Naderi <inaderi@310.ai>"]
 
 [tool.poetry.dependencies]
 python = ">=3.8"
 google-cloud = ">=0.34.0"
 google-cloud-bigquery = ">=3.2.0"
@@ -15,14 +15,16 @@
 torch = ">=1.12.0"
 pandas = ">=1.4.3"
 seaborn = ">=0.11.2"
 matplotlib = ">=3.5.2"
 plotly = ">=5.4.0"
 graphviz = ">=0.11"
 dask = ">=2022.11.0"
+distributed = ">=2022.11.0"
+dask-sql = ">=2022.11.0"
 gcsfs = ">=2022.11.0"
 
 
 [tool.poetry.dev-dependencies]
 pytest = ">7.1.2"
 
 [build-system]
```

### Comparing `lib310-0.2.8/setup.py` & `lib310-0.2.9/setup.py`

 * *Files 7% similar despite different names*

```diff
@@ -10,15 +10,17 @@
  'lib310.tools',
  'lib310.visualization']
 
 package_data = \
 {'': ['*']}
 
 install_requires = \
-['dask>=2022.11.0',
+['dask-sql>=2022.11.0',
+ 'dask>=2022.11.0',
+ 'distributed>=2022.11.0',
  'gcsfs>=2022.11.0',
  'google-cloud-bigquery>=3.2.0',
  'google-cloud>=0.34.0',
  'graphviz>=0.11',
  'matplotlib>=3.5.2',
  'numpy<1.23.0',
  'pandas>=1.4.3',
@@ -27,15 +29,15 @@
  'scanpy>=1.9.1',
  'seaborn>=0.11.2',
  'torch>=1.12.0',
  'transformers>=4.20.1']
 
 setup_kwargs = {
     'name': 'lib310',
-    'version': '0.2.8',
+    'version': '0.2.9',
     'description': 'lib310 Python Package',
     'long_description': 'None',
     'author': 'Mohsen Naghipourfar',
     'author_email': 'naghipourfar@berkeley.edu',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'None',
```

### Comparing `lib310-0.2.8/PKG-INFO` & `lib310-0.2.9/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,19 +1,21 @@
 Metadata-Version: 2.1
 Name: lib310
-Version: 0.2.8
+Version: 0.2.9
 Summary: lib310 Python Package
 Author: Mohsen Naghipourfar
 Author-email: naghipourfar@berkeley.edu
 Requires-Python: >=3.8
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Requires-Dist: dask (>=2022.11.0)
+Requires-Dist: dask-sql (>=2022.11.0)
+Requires-Dist: distributed (>=2022.11.0)
 Requires-Dist: gcsfs (>=2022.11.0)
 Requires-Dist: google-cloud (>=0.34.0)
 Requires-Dist: google-cloud-bigquery (>=3.2.0)
 Requires-Dist: graphviz (>=0.11)
 Requires-Dist: matplotlib (>=3.5.2)
 Requires-Dist: numpy (<1.23.0)
 Requires-Dist: pandas (>=1.4.3)
```

