# Comparing `tmp/pepmatch-0.9.0.tar.gz` & `tmp/pepmatch-0.9.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pepmatch-0.9.0.tar", last modified: Thu Mar 30 22:03:31 2023, max compression
+gzip compressed data, was "pepmatch-0.9.1.tar", last modified: Tue May 23 23:15:53 2023, max compression
```

## Comparing `pepmatch-0.9.0.tar` & `pepmatch-0.9.1.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 dan       (1000) dan       (1000)        0 2023-03-30 22:03:31.294512 pepmatch-0.9.0/
--rw-r--r--   0 dan       (1000) dan       (1000)    11757 2021-03-17 17:44:53.000000 pepmatch-0.9.0/LICENSE
--rw-r--r--   0 dan       (1000) dan       (1000)     4847 2023-03-30 22:03:31.294512 pepmatch-0.9.0/PKG-INFO
--rw-r--r--   0 dan       (1000) dan       (1000)     4541 2023-03-30 20:51:53.000000 pepmatch-0.9.0/README.md
-drwxr-xr-x   0 dan       (1000) dan       (1000)        0 2023-03-30 22:03:31.291179 pepmatch-0.9.0/pepmatch/
--rw-r--r--   0 dan       (1000) dan       (1000)      139 2021-10-30 00:28:03.000000 pepmatch-0.9.0/pepmatch/__init__.py
--rw-r--r--   0 dan       (1000) dan       (1000)     2079 2023-01-19 01:48:10.000000 pepmatch-0.9.0/pepmatch/benchmarker.py
--rw-r--r--   0 dan       (1000) dan       (1000)     1796 2023-03-28 21:36:21.000000 pepmatch-0.9.0/pepmatch/helpers.py
--rwxr-xr-x   0 dan       (1000) dan       (1000)    27982 2023-03-30 20:22:27.000000 pepmatch-0.9.0/pepmatch/matcher.py
--rwxr-xr-x   0 dan       (1000) dan       (1000)     9208 2023-03-28 22:17:53.000000 pepmatch-0.9.0/pepmatch/preprocessor.py
--rw-r--r--   0 dan       (1000) dan       (1000)       22 2023-03-30 21:18:16.000000 pepmatch-0.9.0/pepmatch/version.py
-drwxr-xr-x   0 dan       (1000) dan       (1000)        0 2023-03-30 22:03:31.291179 pepmatch-0.9.0/pepmatch.egg-info/
--rw-r--r--   0 dan       (1000) dan       (1000)     4847 2023-03-30 22:03:31.000000 pepmatch-0.9.0/pepmatch.egg-info/PKG-INFO
--rw-r--r--   0 dan       (1000) dan       (1000)      452 2023-03-30 22:03:31.000000 pepmatch-0.9.0/pepmatch.egg-info/SOURCES.txt
--rw-r--r--   0 dan       (1000) dan       (1000)        1 2023-03-30 22:03:31.000000 pepmatch-0.9.0/pepmatch.egg-info/dependency_links.txt
--rw-r--r--   0 dan       (1000) dan       (1000)      104 2023-03-30 22:03:31.000000 pepmatch-0.9.0/pepmatch.egg-info/entry_points.txt
--rw-r--r--   0 dan       (1000) dan       (1000)        1 2021-01-26 17:40:31.000000 pepmatch-0.9.0/pepmatch.egg-info/not-zip-safe
--rw-r--r--   0 dan       (1000) dan       (1000)       80 2023-03-30 22:03:31.000000 pepmatch-0.9.0/pepmatch.egg-info/requires.txt
--rw-r--r--   0 dan       (1000) dan       (1000)        9 2023-03-30 22:03:31.000000 pepmatch-0.9.0/pepmatch.egg-info/top_level.txt
--rw-r--r--   0 dan       (1000) dan       (1000)       38 2023-03-30 22:03:31.294512 pepmatch-0.9.0/setup.cfg
--rwxr-xr-x   0 dan       (1000) dan       (1000)     1081 2022-05-06 20:37:03.000000 pepmatch-0.9.0/setup.py
-drwxr-xr-x   0 dan       (1000) dan       (1000)        0 2023-03-30 22:03:31.294512 pepmatch-0.9.0/test/
--rw-r--r--   0 dan       (1000) dan       (1000)     1746 2023-03-30 20:49:08.000000 pepmatch-0.9.0/test/test_best_match.py
--rw-r--r--   0 dan       (1000) dan       (1000)     1696 2023-03-30 18:03:55.000000 pepmatch-0.9.0/test/test_exact_match.py
--rw-r--r--   0 dan       (1000) dan       (1000)     1739 2023-03-30 18:03:55.000000 pepmatch-0.9.0/test/test_mismatch.py
+drwxr-xr-x   0 dan       (1000) dan       (1000)        0 2023-05-23 23:15:53.081408 pepmatch-0.9.1/
+-rw-r--r--   0 dan       (1000) dan       (1000)    11757 2021-03-17 17:44:53.000000 pepmatch-0.9.1/LICENSE
+-rw-r--r--   0 dan       (1000) dan       (1000)     4847 2023-05-23 23:15:53.081408 pepmatch-0.9.1/PKG-INFO
+-rw-r--r--   0 dan       (1000) dan       (1000)     4541 2023-03-30 20:51:53.000000 pepmatch-0.9.1/README.md
+drwxr-xr-x   0 dan       (1000) dan       (1000)        0 2023-05-23 23:15:53.078075 pepmatch-0.9.1/pepmatch/
+-rw-r--r--   0 dan       (1000) dan       (1000)      139 2021-10-30 00:28:03.000000 pepmatch-0.9.1/pepmatch/__init__.py
+-rw-r--r--   0 dan       (1000) dan       (1000)     2079 2023-01-19 01:48:10.000000 pepmatch-0.9.1/pepmatch/benchmarker.py
+-rw-r--r--   0 dan       (1000) dan       (1000)     1796 2023-03-28 21:36:21.000000 pepmatch-0.9.1/pepmatch/helpers.py
+-rwxr-xr-x   0 dan       (1000) dan       (1000)    28307 2023-05-23 23:14:19.000000 pepmatch-0.9.1/pepmatch/matcher.py
+-rwxr-xr-x   0 dan       (1000) dan       (1000)     9206 2023-04-11 22:13:38.000000 pepmatch-0.9.1/pepmatch/preprocessor.py
+-rw-r--r--   0 dan       (1000) dan       (1000)       22 2023-05-23 23:14:03.000000 pepmatch-0.9.1/pepmatch/version.py
+drwxr-xr-x   0 dan       (1000) dan       (1000)        0 2023-05-23 23:15:53.081408 pepmatch-0.9.1/pepmatch.egg-info/
+-rw-r--r--   0 dan       (1000) dan       (1000)     4847 2023-05-23 23:15:53.000000 pepmatch-0.9.1/pepmatch.egg-info/PKG-INFO
+-rw-r--r--   0 dan       (1000) dan       (1000)      452 2023-05-23 23:15:53.000000 pepmatch-0.9.1/pepmatch.egg-info/SOURCES.txt
+-rw-r--r--   0 dan       (1000) dan       (1000)        1 2023-05-23 23:15:53.000000 pepmatch-0.9.1/pepmatch.egg-info/dependency_links.txt
+-rw-r--r--   0 dan       (1000) dan       (1000)      104 2023-05-23 23:15:53.000000 pepmatch-0.9.1/pepmatch.egg-info/entry_points.txt
+-rw-r--r--   0 dan       (1000) dan       (1000)        1 2021-01-26 17:40:31.000000 pepmatch-0.9.1/pepmatch.egg-info/not-zip-safe
+-rw-r--r--   0 dan       (1000) dan       (1000)       80 2023-05-23 23:15:53.000000 pepmatch-0.9.1/pepmatch.egg-info/requires.txt
+-rw-r--r--   0 dan       (1000) dan       (1000)        9 2023-05-23 23:15:53.000000 pepmatch-0.9.1/pepmatch.egg-info/top_level.txt
+-rw-r--r--   0 dan       (1000) dan       (1000)       38 2023-05-23 23:15:53.081408 pepmatch-0.9.1/setup.cfg
+-rwxr-xr-x   0 dan       (1000) dan       (1000)     1081 2022-05-06 20:37:03.000000 pepmatch-0.9.1/setup.py
+drwxr-xr-x   0 dan       (1000) dan       (1000)        0 2023-05-23 23:15:53.081408 pepmatch-0.9.1/test/
+-rw-r--r--   0 dan       (1000) dan       (1000)     1765 2023-05-23 05:17:53.000000 pepmatch-0.9.1/test/test_best_match.py
+-rw-r--r--   0 dan       (1000) dan       (1000)     1713 2023-05-23 05:18:00.000000 pepmatch-0.9.1/test/test_exact_match.py
+-rw-r--r--   0 dan       (1000) dan       (1000)     1755 2023-05-23 05:18:04.000000 pepmatch-0.9.1/test/test_mismatch.py
```

### Comparing `pepmatch-0.9.0/LICENSE` & `pepmatch-0.9.1/LICENSE`

 * *Files identical despite different names*

### Comparing `pepmatch-0.9.0/PKG-INFO` & `pepmatch-0.9.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pepmatch
-Version: 0.9.0
+Version: 0.9.1
 Summary: Peptide and epitope search against a reference proteome with specified mismatches.
 Home-page: https://github.com/IEDB/PEPMatch
 Author: Daniel Marrama
 Author-email: dmarrama@lji.org
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `pepmatch-0.9.0/README.md` & `pepmatch-0.9.1/README.md`

 * *Files identical despite different names*

### Comparing `pepmatch-0.9.0/pepmatch/benchmarker.py` & `pepmatch-0.9.1/pepmatch/benchmarker.py`

 * *Files identical despite different names*

### Comparing `pepmatch-0.9.0/pepmatch/helpers.py` & `pepmatch-0.9.1/pepmatch/helpers.py`

 * *Files identical despite different names*

### Comparing `pepmatch-0.9.0/pepmatch/matcher.py` & `pepmatch-0.9.1/pepmatch/matcher.py`

 * *Files 1% similar despite different names*

```diff
@@ -224,16 +224,16 @@
     for peptide in self.query:
       
       if len(peptide) < self.k:
         continue
 
       # split peptide into kmers - only use kmers necessary that overlap entire peptide
       all_kmers = split_sequence(peptide, self.k)
-      target_kmers = all_kmers if self.k == len(peptide) else [all_kmers[i] for i in range(0, len(all_kmers), self.k)] + [all_kmers[-1]]
-      
+      target_kmers = self._get_target_kmers(all_kmers)
+
       # SQL fetch
       sql_placeholders = ', '.join('?' * len(target_kmers))
       sql_query = f'SELECT kmer, idx FROM "{kmers_table_name}" WHERE kmer IN ({sql_placeholders})'
       cursor.execute(sql_query, target_kmers)
       kmer_indexes = cursor.fetchall()
 
       kmer_hit_list = []
@@ -250,14 +250,24 @@
       all_matches.extend(processed_matches)
 
     cursor.close()
     conn.close()
 
     return all_matches
 
+  def _get_target_kmers(self, all_kmers):
+    """Return the target kmers that overlap the entire peptide."""
+    if len(all_kmers) == self.k:
+        return all_kmers
+
+    target_kmers = all_kmers[::self.k]
+    if all_kmers[-1] != target_kmers[-1]:
+        target_kmers.append(all_kmers[-1])
+    return target_kmers
+
   def _process_exact_matches(self, peptide, peptide_matches, cursor, metadata_table_name):
     """Extract all metadata for the exact matches and return as a list of tuples."""
     all_matches = []
     if not peptide_matches:
       all_matches.append((peptide,) + (np.nan,) * 13)
     else:
       for match in peptide_matches:
@@ -489,21 +499,21 @@
       for match in peptide_matches:
         match_data = (
           peptide,                                                         # query peptide
           match[0],                                                        # matched peptide
           metadata_dict[(match[2] - (match[2] % 1000000)) // 1000000][0],  # protein ID
           metadata_dict[(match[2] - (match[2] % 1000000)) // 1000000][1],  # protein name
           metadata_dict[(match[2] - (match[2] % 1000000)) // 1000000][2],  # species
-          metadata_dict[(match[2] - (match[2] % 1000000)) // 1000000][3],  # taxon ID
+          int(metadata_dict[(match[2] - (match[2] % 1000000)) // 1000000][3]), # taxon ID
           metadata_dict[(match[2] - (match[2] % 1000000)) // 1000000][4],  # gene symbol
-          match[1],                                                        # mismatches count
+          int(match[1]),                                                   # mismatches count
           [i+1 for i in range(len(peptide)) if peptide[i] != match[0][i]], # mutated positions
-          (match[2] % 1000000) + 1,                                        # index start
-          (match[2] % 1000000) + len(peptide),                             # index end
-          metadata_dict[(match[2] - (match[2] % 1000000)) // 1000000][5],  # protein existence level
+          int((match[2] % 1000000) + 1),                                   # index start
+          int((match[2] % 1000000) + len(peptide)),                        # index end
+          int(metadata_dict[(match[2] - (match[2] % 1000000)) // 1000000][5]), # protein existence level
           metadata_dict[(match[2] - (match[2] % 1000000)) // 1000000][6],  # sequence version
           metadata_dict[(match[2] - (match[2] % 1000000)) // 1000000][7])  # gene priority flag
         
         all_matches.append(match_data)
 
     return all_matches
 
@@ -638,16 +648,17 @@
     df['Sequence Version'] = df['Sequence Version'].apply(lambda x: f'.{int(x)}' if not pd.isna(x) else '')   
     df['Protein ID'] = df['Protein ID'] + df['Sequence Version']
     
     # drop "Sequence Version" and "Gene Priority" columns
     df.drop(columns=['Sequence Version'], inplace=True)
     df.drop(columns=['Gene Priority'], inplace=True)
 
-    # replace whitespace with NaNs
-    df.replace(r'^\s*$', np.nan, regex=True, inplace=True)
+    # force integers on some columns
+    int_cols = ['Taxon ID', 'Mismatches', 'Index start', 'Index end', 'Protein Existence Level']
+    df[int_cols] = df[int_cols].astype('Int64')
 
     return df
 
   def _output_matches(self, df):
     """Write Pandas dataframe to format that is specified"""
     if self.output_format == 'csv':
       return df.to_csv(f'{self.preprocessed_files_path}/{self.output_name}.csv', index=False)
```

### Comparing `pepmatch-0.9.0/pepmatch/preprocessor.py` & `pepmatch-0.9.1/pepmatch/preprocessor.py`

 * *Files 0% similar despite different names*

```diff
@@ -120,15 +120,15 @@
     db_path = os.path.join(self.preprocessed_files_path, f'{self.proteome_name}.db')
     with sqlite3.connect(db_path) as conn:
       cursor = conn.cursor()
 
       # check if kmers table already exists and exit if it does
       # for some reason writing to the same table multiple times messes up results
       if cursor.execute(f'SELECT name FROM sqlite_master WHERE type="table" AND name="{kmers_table}";').fetchone():
-          return
+        return
 
       self._create_tables(cursor, kmers_table, metadata_table)
       self._insert_kmers(cursor, kmers_table, k)
       self._insert_metadata(cursor, metadata_table)
       self._create_indexes(cursor, kmers_table, metadata_table)
 
       conn.commit()
```

### Comparing `pepmatch-0.9.0/pepmatch.egg-info/PKG-INFO` & `pepmatch-0.9.1/pepmatch.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pepmatch
-Version: 0.9.0
+Version: 0.9.1
 Summary: Peptide and epitope search against a reference proteome with specified mismatches.
 Home-page: https://github.com/IEDB/PEPMatch
 Author: Daniel Marrama
 Author-email: dmarrama@lji.org
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `pepmatch-0.9.0/setup.py` & `pepmatch-0.9.1/setup.py`

 * *Files identical despite different names*

### Comparing `pepmatch-0.9.0/test/test_exact_match.py` & `pepmatch-0.9.1/test/test_exact_match.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,50 +1,49 @@
 #!/usr/bin/env python3
 
-import unittest
 import os
 
 import pandas as pd
 import pandas.testing as pdt
 
 from pepmatch import Preprocessor, Matcher
 
-class TestExactMatch(unittest.TestCase):
-  def test_exact_match(self):
 
-    # paths
-    test_script_dir = os.path.dirname(os.path.realpath(__file__))
-    proteome_fasta = os.path.join(test_script_dir, '../benchmarking/proteomes/human.fasta')
-    query_fasta = os.path.join(test_script_dir, '../benchmarking/queries/mhc_ligands_test.fasta')
-    expected_csv = os.path.join(test_script_dir, '../benchmarking/expected/mhc_ligands_expected.csv')
-
-    # preprocess human proteome
-    k=9
-    Preprocessor(proteome_fasta).sql_proteome(k)
-
-    # match MHC ligands (9-mers) to human proteome
-    df = Matcher(
-      query=query_fasta,
-      proteome_file=proteome_fasta,
-      max_mismatches=0,
-      k=k,
-      output_format='dataframe').match()
-
-    # remove preprocessed file
-    os.remove('human.db')
-
-    # load the expected data
-    expected_df = pd.read_csv(expected_csv)
-
-    # select only the necessary columns to test for
-    df = df[['Query Sequence', 'Matched Sequence', 'Protein ID', 'Index start']]
-    expected_df = expected_df[['Query Sequence', 'Matched Sequence', 'Protein ID', 'Index start']]
-
-    # sort dataframes by Query Sequence, Protein ID, and Index start
-    df = df.sort_values(by=['Query Sequence', 'Protein ID', 'Index start']).reset_index(drop=True)
-    expected_df = expected_df.sort_values(by=['Query Sequence', 'Protein ID', 'Index start']).reset_index(drop=True)
+def test_exact_match():
+  # paths
+  test_script_dir = os.path.dirname(os.path.realpath(__file__))
+  proteome_fasta = os.path.join(test_script_dir, '../benchmarking/proteomes/human.fasta')
+  query_fasta = os.path.join(test_script_dir, '../benchmarking/queries/mhc_ligands_test.fasta')
+  expected_csv = os.path.join(test_script_dir, '../benchmarking/expected/mhc_ligands_expected.csv')
+
+  # preprocess human proteome
+  k=9
+  Preprocessor(proteome_fasta).sql_proteome(k)
+
+  # match MHC ligands (9-mers) to human proteome
+  df = Matcher(
+    query=query_fasta,
+    proteome_file=proteome_fasta,
+    max_mismatches=0,
+    k=k,
+    output_format='dataframe').match()
+
+  # remove preprocessed file
+  os.remove('human.db')
+
+  # load the expected data
+  expected_df = pd.read_csv(expected_csv)
+
+  # select only the necessary columns to test for
+  df = df[['Query Sequence', 'Matched Sequence', 'Protein ID', 'Index start']]
+  expected_df = expected_df[['Query Sequence', 'Matched Sequence', 'Protein ID', 'Index start']]
+
+  # convert Index start to int64 for comparison
+  df['Index start'] = df['Index start'].astype('int64')
+  expected_df['Index start'] = expected_df['Index start'].astype('int64')
+
+  # sort dataframes by Query Sequence, Protein ID, and Index start
+  df = df.sort_values(by=['Query Sequence', 'Protein ID', 'Index start']).reset_index(drop=True)
+  expected_df = expected_df.sort_values(by=['Query Sequence', 'Protein ID', 'Index start']).reset_index(drop=True)
 
-    # assert dataframes are equal
-    pdt.assert_frame_equal(df, expected_df, check_dtype=False, check_exact=True)
-
-if __name__ == '__main__':
-  unittest.main()
+  # assert dataframes are equal
+  pdt.assert_frame_equal(df, expected_df, check_dtype=False, check_exact=True)
```

### Comparing `pepmatch-0.9.0/test/test_mismatch.py` & `pepmatch-0.9.1/test/test_mismatch.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,51 +1,49 @@
 #!/usr/bin/env python3
 
-import unittest
 import os
 
 import pandas as pd
 import pandas.testing as pdt
 
 from pepmatch import Preprocessor, Matcher
   
-class TestMismatch(unittest.TestCase):
-  def test_mismatch(self):
+def test_mismatch():
+  # paths
+  test_script_dir = os.path.dirname(os.path.realpath(__file__))
+  proteome_fasta = os.path.join(test_script_dir, '../benchmarking/proteomes/human.fasta')
+  query_fasta = os.path.join(test_script_dir, '../benchmarking/queries/neoepitopes_test.fasta')
+  expected_csv = os.path.join(test_script_dir, '../benchmarking/expected/neoepitopes_expected.csv')
+
+  # preprocess human proteome
+  k = 3
+  Preprocessor(proteome_fasta).pickle_proteome(k)
+
+  # match neoepitopes to human proteome
+  df = Matcher(
+    query=query_fasta,
+    proteome_file=proteome_fasta,
+    max_mismatches=3,
+    k=k,
+    output_format='dataframe').match()
+
+  # remove preprocessed files
+  os.remove('human_3mers.pickle')
+  os.remove('human_metadata.pickle')
+
+  # load the expected data
+  expected_df = pd.read_csv(expected_csv)
+
+  # select only the necessary columns to test for
+  df = df[['Query Sequence', 'Matched Sequence', 'Protein ID', 'Index start']]
+  expected_df = expected_df[['Query Sequence', 'Matched Sequence', 'Protein ID', 'Index start']]
+
+  # convert Index start to int64 for comparison
+  df['Index start'] = df['Index start'].astype('int64')
+  expected_df['Index start'] = expected_df['Index start'].astype('int64')
+
+  # sort dataframes by Query Sequence, Protein ID, and Index start
+  df = df.sort_values(by=['Query Sequence', 'Protein ID', 'Index start']).reset_index(drop=True)
+  expected_df = expected_df.sort_values(by=['Query Sequence', 'Protein ID', 'Index start']).reset_index(drop=True)
 
-    # paths
-    test_script_dir = os.path.dirname(os.path.realpath(__file__))
-    proteome_fasta = os.path.join(test_script_dir, '../benchmarking/proteomes/human.fasta')
-    query_fasta = os.path.join(test_script_dir, '../benchmarking/queries/neoepitopes_test.fasta')
-    expected_csv = os.path.join(test_script_dir, '../benchmarking/expected/neoepitopes_expected.csv')
-
-    # preprocess human proteome
-    k = 3
-    Preprocessor(proteome_fasta).pickle_proteome(k)
-
-    # match neoepitopes to human proteome
-    df = Matcher(
-      query=query_fasta,
-      proteome_file=proteome_fasta,
-      max_mismatches=3,
-      k=k,
-      output_format='dataframe').match()
-
-    # remove preprocessed files
-    os.remove('human_3mers.pickle')
-    os.remove('human_metadata.pickle')
-
-    # load the expected data
-    expected_df = pd.read_csv(expected_csv)
-
-    # select only the necessary columns to test for
-    df = df[['Query Sequence', 'Matched Sequence', 'Protein ID', 'Index start']]
-    expected_df = expected_df[['Query Sequence', 'Matched Sequence', 'Protein ID', 'Index start']]
-
-    # sort dataframes by Query Sequence, Protein ID, and Index start
-    df = df.sort_values(by=['Query Sequence', 'Protein ID', 'Index start']).reset_index(drop=True)
-    expected_df = expected_df.sort_values(by=['Query Sequence', 'Protein ID', 'Index start']).reset_index(drop=True)
-
-    # assert dataframes are equal
-    pdt.assert_frame_equal(df, expected_df, check_dtype=False, check_exact=True)
-
-if __name__ == '__main__':
-  unittest.main()
+  # assert dataframes are equal
+  pdt.assert_frame_equal(df, expected_df, check_dtype=False, check_exact=True)
```

