# Comparing `tmp/mapel-elections-2.0.3.dev6.tar.gz` & `tmp/mapel-elections-2.0.3.dev7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mapel-elections-2.0.3.dev6.tar", last modified: Wed May 24 14:40:59 2023, max compression
+gzip compressed data, was "mapel-elections-2.0.3.dev7.tar", last modified: Wed May 24 17:34:53 2023, max compression
```

## Comparing `mapel-elections-2.0.3.dev6.tar` & `mapel-elections-2.0.3.dev7.tar`

### file list

```diff
@@ -1,94 +1,94 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 14:40:59.979500 mapel-elections-2.0.3.dev6/
--rw-r--r--   0 runner    (1001) docker     (123)     1081 2023-05-24 14:40:30.000000 mapel-elections-2.0.3.dev6/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)     3660 2023-05-24 14:40:59.979500 mapel-elections-2.0.3.dev6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1801 2023-05-24 14:40:30.000000 mapel-elections-2.0.3.dev6/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       57 2023-05-24 14:40:30.000000 mapel-elections-2.0.3.dev6/optional_requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1047 2023-05-24 14:40:30.000000 mapel-elections-2.0.3.dev6/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-05-24 14:40:30.000000 mapel-elections-2.0.3.dev6/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-24 14:40:59.979500 mapel-elections-2.0.3.dev6/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      338 2023-05-24 14:40:30.000000 mapel-elections-2.0.3.dev6/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 14:40:59.963500 mapel-elections-2.0.3.dev6/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 14:40:59.959500 mapel-elections-2.0.3.dev6/src/mapel/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 14:40:59.963500 mapel-elections-2.0.3.dev6/src/mapel/elections/
--rw-r--r--   0 runner    (1001) docker     (123)     4115 2023-05-24 14:40:30.000000 mapel-elections-2.0.3.dev6/src/mapel/elections/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 14:40:59.967501 mapel-elections-2.0.3.dev6/src/mapel/elections/cultures/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 14:40:30.000000 mapel-elections-2.0.3.dev6/src/mapel/elections/cultures/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2913 2023-05-24 14:40:30.000000 mapel-elections-2.0.3.dev6/src/mapel/elections/cultures/alliances.py
--rw-r--r--   0 runner    (1001) docker     (123)      278 2023-05-24 14:40:30.000000 mapel-elections-2.0.3.dev6/src/mapel/elections/cultures/converters.py
--rw-r--r--   0 runner    (1001) docker     (123)      809 2023-05-24 14:40:30.000000 mapel-elections-2.0.3.dev6/src/mapel/elections/cultures/didi.py
--rw-r--r--   0 runner    (1001) docker     (123)    13776 2023-05-24 14:40:30.000000 mapel-elections-2.0.3.dev6/src/mapel/elections/cultures/euclidean.py
--rw-r--r--   0 runner    (1001) docker     (123)     6072 2023-05-24 14:40:30.000000 mapel-elections-2.0.3.dev6/src/mapel/elections/cultures/fake.py
--rw-r--r--   0 runner    (1001) docker     (123)     2468 2023-05-24 14:40:30.000000 mapel-elections-2.0.3.dev6/src/mapel/elections/cultures/field_experiment.py
--rw-r--r--   0 runner    (1001) docker     (123)    12638 2023-05-24 14:40:30.000000 mapel-elections-2.0.3.dev6/src/mapel/elections/cultures/group_separable.py
--rw-r--r--   0 runner    (1001) docker     (123)     1351 2023-05-24 14:40:30.000000 mapel-elections-2.0.3.dev6/src/mapel/elections/cultures/guardians.py
--rw-r--r--   0 runner    (1001) docker     (123)    11584 2023-05-24 14:40:30.000000 mapel-elections-2.0.3.dev6/src/mapel/elections/cultures/guardians_plus.py
--rw-r--r--   0 runner    (1001) docker     (123)     3153 2023-05-24 14:40:30.000000 mapel-elections-2.0.3.dev6/src/mapel/elections/cultures/impartial.py
--rw-r--r--   0 runner    (1001) docker     (123)     9216 2023-05-24 14:40:30.000000 mapel-elections-2.0.3.dev6/src/mapel/elections/cultures/mallows.py
--rw-r--r--   0 runner    (1001) docker     (123)     1738 2023-05-24 14:40:30.000000 mapel-elections-2.0.3.dev6/src/mapel/elections/cultures/noise.py
--rw-r--r--   0 runner    (1001) docker     (123)     8618 2023-05-24 14:40:30.000000 mapel-elections-2.0.3.dev6/src/mapel/elections/cultures/params.py
--rw-r--r--   0 runner    (1001) docker     (123)      472 2023-05-24 14:40:30.000000 mapel-elections-2.0.3.dev6/src/mapel/elections/cultures/parties.py
--rw-r--r--   0 runner    (1001) docker     (123)     1326 2023-05-24 14:40:30.000000 mapel-elections-2.0.3.dev6/src/mapel/elections/cultures/partylist.py
--rw-r--r--   0 runner    (1001) docker     (123)     8833 2023-05-24 14:40:30.000000 mapel-elections-2.0.3.dev6/src/mapel/elections/cultures/preflib.py
--rw-r--r--   0 runner    (1001) docker     (123)     2709 2023-05-24 14:40:30.000000 mapel-elections-2.0.3.dev6/src/mapel/elections/cultures/resampling.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 14:40:59.971500 mapel-elections-2.0.3.dev6/src/mapel/elections/cultures/sampling/
--rw-r--r--   0 runner    (1001) docker     (123)     3795 2023-05-24 14:40:30.000000 mapel-elections-2.0.3.dev6/src/mapel/elections/cultures/sampling/samplemat.py
--rw-r--r--   0 runner    (1001) docker     (123)     7168 2023-05-24 14:40:30.000000 mapel-elections-2.0.3.dev6/src/mapel/elections/cultures/single_crossing.py
--rw-r--r--   0 runner    (1001) docker     (123)     2420 2023-05-24 14:40:30.000000 mapel-elections-2.0.3.dev6/src/mapel/elections/cultures/single_peaked.py
--rw-r--r--   0 runner    (1001) docker     (123)     3372 2023-05-24 14:40:30.000000 mapel-elections-2.0.3.dev6/src/mapel/elections/cultures/sp_matrices.py
--rw-r--r--   0 runner    (1001) docker     (123)     8485 2023-05-24 14:40:30.000000 mapel-elections-2.0.3.dev6/src/mapel/elections/cultures/unused.py
--rw-r--r--   0 runner    (1001) docker     (123)     2826 2023-05-24 14:40:30.000000 mapel-elections-2.0.3.dev6/src/mapel/elections/cultures/urn.py
--rw-r--r--   0 runner    (1001) docker     (123)     9417 2023-05-24 14:40:30.000000 mapel-elections-2.0.3.dev6/src/mapel/elections/cultures_.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 14:40:59.971500 mapel-elections-2.0.3.dev6/src/mapel/elections/distances/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 14:40:30.000000 mapel-elections-2.0.3.dev6/src/mapel/elections/distances/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1945 2023-05-24 14:40:30.000000 mapel-elections-2.0.3.dev6/src/mapel/elections/distances/committee_distances.py
--rw-r--r--   0 runner    (1001) docker     (123)    16377 2023-05-24 14:40:30.000000 mapel-elections-2.0.3.dev6/src/mapel/elections/distances/cppdistances.cpp
--rw-r--r--   0 runner    (1001) docker     (123)    23722 2023-05-24 14:40:30.000000 mapel-elections-2.0.3.dev6/src/mapel/elections/distances/ilp_isomorphic.py
--rw-r--r--   0 runner    (1001) docker     (123)    50211 2023-05-24 14:40:30.000000 mapel-elections-2.0.3.dev6/src/mapel/elections/distances/lp.py
--rw-r--r--   0 runner    (1001) docker     (123)     9107 2023-05-24 14:40:30.000000 mapel-elections-2.0.3.dev6/src/mapel/elections/distances/main_approval_distances.py
--rw-r--r--   0 runner    (1001) docker     (123)     8644 2023-05-24 14:40:30.000000 mapel-elections-2.0.3.dev6/src/mapel/elections/distances/main_ordinal_distances.py
--rw-r--r--   0 runner    (1001) docker     (123)     8265 2023-05-24 14:40:30.000000 mapel-elections-2.0.3.dev6/src/mapel/elections/distances_.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 14:40:59.975500 mapel-elections-2.0.3.dev6/src/mapel/elections/features/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 14:40:30.000000 mapel-elections-2.0.3.dev6/src/mapel/elections/features/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7256 2023-05-24 14:40:30.000000 mapel-elections-2.0.3.dev6/src/mapel/elections/features/approx.py
--rw-r--r--   0 runner    (1001) docker     (123)     2435 2023-05-24 14:40:30.000000 mapel-elections-2.0.3.dev6/src/mapel/elections/features/banzhaf_cc.py
--rw-r--r--   0 runner    (1001) docker     (123)     3840 2023-05-24 14:40:30.000000 mapel-elections-2.0.3.dev6/src/mapel/elections/features/clustering.py
--rw-r--r--   0 runner    (1001) docker     (123)     5526 2023-05-24 14:40:30.000000 mapel-elections-2.0.3.dev6/src/mapel/elections/features/cohesive.py
--rw-r--r--   0 runner    (1001) docker     (123)     2818 2023-05-24 14:40:30.000000 mapel-elections-2.0.3.dev6/src/mapel/elections/features/dependent_rounding.py
--rw-r--r--   0 runner    (1001) docker     (123)      964 2023-05-24 14:40:30.000000 mapel-elections-2.0.3.dev6/src/mapel/elections/features/dimensionality.py
--rw-r--r--   0 runner    (1001) docker     (123)     7437 2023-05-24 14:40:30.000000 mapel-elections-2.0.3.dev6/src/mapel/elections/features/distortion.py
--rw-r--r--   0 runner    (1001) docker     (123)    21363 2023-05-24 14:40:30.000000 mapel-elections-2.0.3.dev6/src/mapel/elections/features/diversity.py
--rw-r--r--   0 runner    (1001) docker     (123)      556 2023-05-24 14:40:30.000000 mapel-elections-2.0.3.dev6/src/mapel/elections/features/justified_representation.py
--rw-r--r--   0 runner    (1001) docker     (123)     2514 2023-05-24 14:40:30.000000 mapel-elections-2.0.3.dev6/src/mapel/elections/features/other.py
--rw-r--r--   0 runner    (1001) docker     (123)     4591 2023-05-24 14:40:30.000000 mapel-elections-2.0.3.dev6/src/mapel/elections/features/partylist.py
--rw-r--r--   0 runner    (1001) docker     (123)     1259 2023-05-24 14:40:30.000000 mapel-elections-2.0.3.dev6/src/mapel/elections/features/power_index.py
--rw-r--r--   0 runner    (1001) docker     (123)     4833 2023-05-24 14:40:30.000000 mapel-elections-2.0.3.dev6/src/mapel/elections/features/proportionality_degree.py
--rw-r--r--   0 runner    (1001) docker     (123)     1369 2023-05-24 14:40:30.000000 mapel-elections-2.0.3.dev6/src/mapel/elections/features/ranging_cc.py
--rw-r--r--   0 runner    (1001) docker     (123)     8930 2023-05-24 14:40:30.000000 mapel-elections-2.0.3.dev6/src/mapel/elections/features/scores.py
--rw-r--r--   0 runner    (1001) docker     (123)      998 2023-05-24 14:40:30.000000 mapel-elections-2.0.3.dev6/src/mapel/elections/features/vc_diversity.py
--rw-r--r--   0 runner    (1001) docker     (123)     6675 2023-05-24 14:40:30.000000 mapel-elections-2.0.3.dev6/src/mapel/elections/features_.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 14:40:59.975500 mapel-elections-2.0.3.dev6/src/mapel/elections/objects/
--rw-r--r--   0 runner    (1001) docker     (123)    12608 2023-05-24 14:40:30.000000 mapel-elections-2.0.3.dev6/src/mapel/elections/objects/ApprovalElection.py
--rw-r--r--   0 runner    (1001) docker     (123)     9909 2023-05-24 14:40:30.000000 mapel-elections-2.0.3.dev6/src/mapel/elections/objects/ApprovalElectionExperiment.py
--rw-r--r--   0 runner    (1001) docker     (123)    18128 2023-05-24 14:40:30.000000 mapel-elections-2.0.3.dev6/src/mapel/elections/objects/Election.py
--rw-r--r--   0 runner    (1001) docker     (123)    28015 2023-05-24 14:40:30.000000 mapel-elections-2.0.3.dev6/src/mapel/elections/objects/ElectionExperiment.py
--rw-r--r--   0 runner    (1001) docker     (123)     6722 2023-05-24 14:40:30.000000 mapel-elections-2.0.3.dev6/src/mapel/elections/objects/ElectionFamily.py
--rw-r--r--   0 runner    (1001) docker     (123)    20127 2023-05-24 14:40:30.000000 mapel-elections-2.0.3.dev6/src/mapel/elections/objects/OrdinalElection.py
--rw-r--r--   0 runner    (1001) docker     (123)     2646 2023-05-24 14:40:30.000000 mapel-elections-2.0.3.dev6/src/mapel/elections/objects/OrdinalElectionExperiment.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 14:40:30.000000 mapel-elections-2.0.3.dev6/src/mapel/elections/objects/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 14:40:59.979500 mapel-elections-2.0.3.dev6/src/mapel/elections/other/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 14:40:30.000000 mapel-elections-2.0.3.dev6/src/mapel/elections/other/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2317 2023-05-24 14:40:30.000000 mapel-elections-2.0.3.dev6/src/mapel/elections/other/matrices.py
--rw-r--r--   0 runner    (1001) docker     (123)     3106 2023-05-24 14:40:30.000000 mapel-elections-2.0.3.dev6/src/mapel/elections/other/matrix2png.py
--rw-r--r--   0 runner    (1001) docker     (123)     3455 2023-05-24 14:40:30.000000 mapel-elections-2.0.3.dev6/src/mapel/elections/other/pabulib.py
--rw-r--r--   0 runner    (1001) docker     (123)     3955 2023-05-24 14:40:30.000000 mapel-elections-2.0.3.dev6/src/mapel/elections/other/rules.py
--rw-r--r--   0 runner    (1001) docker     (123)    13087 2023-05-24 14:40:30.000000 mapel-elections-2.0.3.dev6/src/mapel/elections/other/winners.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 14:40:59.979500 mapel-elections-2.0.3.dev6/src/mapel/elections/persistence/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 14:40:30.000000 mapel-elections-2.0.3.dev6/src/mapel/elections/persistence/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6851 2023-05-24 14:40:30.000000 mapel-elections-2.0.3.dev6/src/mapel/elections/persistence/election_exports.py
--rw-r--r--   0 runner    (1001) docker     (123)     7048 2023-05-24 14:40:30.000000 mapel-elections-2.0.3.dev6/src/mapel/elections/persistence/election_imports.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 14:40:59.979500 mapel-elections-2.0.3.dev6/src/mapel_elections.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3660 2023-05-24 14:40:59.000000 mapel-elections-2.0.3.dev6/src/mapel_elections.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3301 2023-05-24 14:40:59.000000 mapel-elections-2.0.3.dev6/src/mapel_elections.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-24 14:40:59.000000 mapel-elections-2.0.3.dev6/src/mapel_elections.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       85 2023-05-24 14:40:59.000000 mapel-elections-2.0.3.dev6/src/mapel_elections.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-05-24 14:40:59.000000 mapel-elections-2.0.3.dev6/src/mapel_elections.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 17:34:53.820635 mapel-elections-2.0.3.dev7/
+-rw-r--r--   0 runner    (1001) docker     (123)     1081 2023-05-24 17:34:28.000000 mapel-elections-2.0.3.dev7/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     3660 2023-05-24 17:34:53.820635 mapel-elections-2.0.3.dev7/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1801 2023-05-24 17:34:28.000000 mapel-elections-2.0.3.dev7/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       57 2023-05-24 17:34:28.000000 mapel-elections-2.0.3.dev7/optional_requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1047 2023-05-24 17:34:28.000000 mapel-elections-2.0.3.dev7/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-05-24 17:34:28.000000 mapel-elections-2.0.3.dev7/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-24 17:34:53.820635 mapel-elections-2.0.3.dev7/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      338 2023-05-24 17:34:28.000000 mapel-elections-2.0.3.dev7/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 17:34:53.812635 mapel-elections-2.0.3.dev7/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 17:34:53.812635 mapel-elections-2.0.3.dev7/src/mapel/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 17:34:53.812635 mapel-elections-2.0.3.dev7/src/mapel/elections/
+-rw-r--r--   0 runner    (1001) docker     (123)     4115 2023-05-24 17:34:28.000000 mapel-elections-2.0.3.dev7/src/mapel/elections/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 17:34:53.816635 mapel-elections-2.0.3.dev7/src/mapel/elections/cultures/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 17:34:28.000000 mapel-elections-2.0.3.dev7/src/mapel/elections/cultures/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2913 2023-05-24 17:34:28.000000 mapel-elections-2.0.3.dev7/src/mapel/elections/cultures/alliances.py
+-rw-r--r--   0 runner    (1001) docker     (123)      278 2023-05-24 17:34:28.000000 mapel-elections-2.0.3.dev7/src/mapel/elections/cultures/converters.py
+-rw-r--r--   0 runner    (1001) docker     (123)      809 2023-05-24 17:34:28.000000 mapel-elections-2.0.3.dev7/src/mapel/elections/cultures/didi.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13776 2023-05-24 17:34:28.000000 mapel-elections-2.0.3.dev7/src/mapel/elections/cultures/euclidean.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6072 2023-05-24 17:34:28.000000 mapel-elections-2.0.3.dev7/src/mapel/elections/cultures/fake.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2468 2023-05-24 17:34:28.000000 mapel-elections-2.0.3.dev7/src/mapel/elections/cultures/field_experiment.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12638 2023-05-24 17:34:28.000000 mapel-elections-2.0.3.dev7/src/mapel/elections/cultures/group_separable.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1351 2023-05-24 17:34:28.000000 mapel-elections-2.0.3.dev7/src/mapel/elections/cultures/guardians.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11584 2023-05-24 17:34:28.000000 mapel-elections-2.0.3.dev7/src/mapel/elections/cultures/guardians_plus.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3153 2023-05-24 17:34:28.000000 mapel-elections-2.0.3.dev7/src/mapel/elections/cultures/impartial.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9216 2023-05-24 17:34:28.000000 mapel-elections-2.0.3.dev7/src/mapel/elections/cultures/mallows.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1738 2023-05-24 17:34:29.000000 mapel-elections-2.0.3.dev7/src/mapel/elections/cultures/noise.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8618 2023-05-24 17:34:29.000000 mapel-elections-2.0.3.dev7/src/mapel/elections/cultures/params.py
+-rw-r--r--   0 runner    (1001) docker     (123)      472 2023-05-24 17:34:29.000000 mapel-elections-2.0.3.dev7/src/mapel/elections/cultures/parties.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1326 2023-05-24 17:34:29.000000 mapel-elections-2.0.3.dev7/src/mapel/elections/cultures/partylist.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8833 2023-05-24 17:34:29.000000 mapel-elections-2.0.3.dev7/src/mapel/elections/cultures/preflib.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2709 2023-05-24 17:34:29.000000 mapel-elections-2.0.3.dev7/src/mapel/elections/cultures/resampling.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 17:34:53.816635 mapel-elections-2.0.3.dev7/src/mapel/elections/cultures/sampling/
+-rw-r--r--   0 runner    (1001) docker     (123)     3795 2023-05-24 17:34:29.000000 mapel-elections-2.0.3.dev7/src/mapel/elections/cultures/sampling/samplemat.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7168 2023-05-24 17:34:29.000000 mapel-elections-2.0.3.dev7/src/mapel/elections/cultures/single_crossing.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2420 2023-05-24 17:34:29.000000 mapel-elections-2.0.3.dev7/src/mapel/elections/cultures/single_peaked.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3372 2023-05-24 17:34:29.000000 mapel-elections-2.0.3.dev7/src/mapel/elections/cultures/sp_matrices.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8485 2023-05-24 17:34:29.000000 mapel-elections-2.0.3.dev7/src/mapel/elections/cultures/unused.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2826 2023-05-24 17:34:29.000000 mapel-elections-2.0.3.dev7/src/mapel/elections/cultures/urn.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9417 2023-05-24 17:34:29.000000 mapel-elections-2.0.3.dev7/src/mapel/elections/cultures_.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 17:34:53.816635 mapel-elections-2.0.3.dev7/src/mapel/elections/distances/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 17:34:29.000000 mapel-elections-2.0.3.dev7/src/mapel/elections/distances/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1945 2023-05-24 17:34:29.000000 mapel-elections-2.0.3.dev7/src/mapel/elections/distances/committee_distances.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16377 2023-05-24 17:34:29.000000 mapel-elections-2.0.3.dev7/src/mapel/elections/distances/cppdistances.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)    23722 2023-05-24 17:34:29.000000 mapel-elections-2.0.3.dev7/src/mapel/elections/distances/ilp_isomorphic.py
+-rw-r--r--   0 runner    (1001) docker     (123)    50211 2023-05-24 17:34:29.000000 mapel-elections-2.0.3.dev7/src/mapel/elections/distances/lp.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9107 2023-05-24 17:34:29.000000 mapel-elections-2.0.3.dev7/src/mapel/elections/distances/main_approval_distances.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8644 2023-05-24 17:34:29.000000 mapel-elections-2.0.3.dev7/src/mapel/elections/distances/main_ordinal_distances.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8265 2023-05-24 17:34:29.000000 mapel-elections-2.0.3.dev7/src/mapel/elections/distances_.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 17:34:53.820635 mapel-elections-2.0.3.dev7/src/mapel/elections/features/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 17:34:29.000000 mapel-elections-2.0.3.dev7/src/mapel/elections/features/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7256 2023-05-24 17:34:29.000000 mapel-elections-2.0.3.dev7/src/mapel/elections/features/approx.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2435 2023-05-24 17:34:29.000000 mapel-elections-2.0.3.dev7/src/mapel/elections/features/banzhaf_cc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3840 2023-05-24 17:34:29.000000 mapel-elections-2.0.3.dev7/src/mapel/elections/features/clustering.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5526 2023-05-24 17:34:29.000000 mapel-elections-2.0.3.dev7/src/mapel/elections/features/cohesive.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2818 2023-05-24 17:34:29.000000 mapel-elections-2.0.3.dev7/src/mapel/elections/features/dependent_rounding.py
+-rw-r--r--   0 runner    (1001) docker     (123)      964 2023-05-24 17:34:29.000000 mapel-elections-2.0.3.dev7/src/mapel/elections/features/dimensionality.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7437 2023-05-24 17:34:29.000000 mapel-elections-2.0.3.dev7/src/mapel/elections/features/distortion.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21363 2023-05-24 17:34:29.000000 mapel-elections-2.0.3.dev7/src/mapel/elections/features/diversity.py
+-rw-r--r--   0 runner    (1001) docker     (123)      556 2023-05-24 17:34:29.000000 mapel-elections-2.0.3.dev7/src/mapel/elections/features/justified_representation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2514 2023-05-24 17:34:29.000000 mapel-elections-2.0.3.dev7/src/mapel/elections/features/other.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4591 2023-05-24 17:34:29.000000 mapel-elections-2.0.3.dev7/src/mapel/elections/features/partylist.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1259 2023-05-24 17:34:29.000000 mapel-elections-2.0.3.dev7/src/mapel/elections/features/power_index.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4833 2023-05-24 17:34:29.000000 mapel-elections-2.0.3.dev7/src/mapel/elections/features/proportionality_degree.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1369 2023-05-24 17:34:29.000000 mapel-elections-2.0.3.dev7/src/mapel/elections/features/ranging_cc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8930 2023-05-24 17:34:29.000000 mapel-elections-2.0.3.dev7/src/mapel/elections/features/scores.py
+-rw-r--r--   0 runner    (1001) docker     (123)      998 2023-05-24 17:34:29.000000 mapel-elections-2.0.3.dev7/src/mapel/elections/features/vc_diversity.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6675 2023-05-24 17:34:29.000000 mapel-elections-2.0.3.dev7/src/mapel/elections/features_.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 17:34:53.820635 mapel-elections-2.0.3.dev7/src/mapel/elections/objects/
+-rw-r--r--   0 runner    (1001) docker     (123)    12608 2023-05-24 17:34:29.000000 mapel-elections-2.0.3.dev7/src/mapel/elections/objects/ApprovalElection.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9909 2023-05-24 17:34:29.000000 mapel-elections-2.0.3.dev7/src/mapel/elections/objects/ApprovalElectionExperiment.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18128 2023-05-24 17:34:29.000000 mapel-elections-2.0.3.dev7/src/mapel/elections/objects/Election.py
+-rw-r--r--   0 runner    (1001) docker     (123)    28015 2023-05-24 17:34:29.000000 mapel-elections-2.0.3.dev7/src/mapel/elections/objects/ElectionExperiment.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6722 2023-05-24 17:34:29.000000 mapel-elections-2.0.3.dev7/src/mapel/elections/objects/ElectionFamily.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20127 2023-05-24 17:34:29.000000 mapel-elections-2.0.3.dev7/src/mapel/elections/objects/OrdinalElection.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2646 2023-05-24 17:34:29.000000 mapel-elections-2.0.3.dev7/src/mapel/elections/objects/OrdinalElectionExperiment.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 17:34:29.000000 mapel-elections-2.0.3.dev7/src/mapel/elections/objects/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 17:34:53.820635 mapel-elections-2.0.3.dev7/src/mapel/elections/other/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 17:34:29.000000 mapel-elections-2.0.3.dev7/src/mapel/elections/other/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2317 2023-05-24 17:34:29.000000 mapel-elections-2.0.3.dev7/src/mapel/elections/other/matrices.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3106 2023-05-24 17:34:29.000000 mapel-elections-2.0.3.dev7/src/mapel/elections/other/matrix2png.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3455 2023-05-24 17:34:29.000000 mapel-elections-2.0.3.dev7/src/mapel/elections/other/pabulib.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3955 2023-05-24 17:34:29.000000 mapel-elections-2.0.3.dev7/src/mapel/elections/other/rules.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13087 2023-05-24 17:34:29.000000 mapel-elections-2.0.3.dev7/src/mapel/elections/other/winners.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 17:34:53.820635 mapel-elections-2.0.3.dev7/src/mapel/elections/persistence/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 17:34:29.000000 mapel-elections-2.0.3.dev7/src/mapel/elections/persistence/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6851 2023-05-24 17:34:29.000000 mapel-elections-2.0.3.dev7/src/mapel/elections/persistence/election_exports.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7048 2023-05-24 17:34:29.000000 mapel-elections-2.0.3.dev7/src/mapel/elections/persistence/election_imports.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 17:34:53.820635 mapel-elections-2.0.3.dev7/src/mapel_elections.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3660 2023-05-24 17:34:53.000000 mapel-elections-2.0.3.dev7/src/mapel_elections.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3301 2023-05-24 17:34:53.000000 mapel-elections-2.0.3.dev7/src/mapel_elections.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-24 17:34:53.000000 mapel-elections-2.0.3.dev7/src/mapel_elections.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       85 2023-05-24 17:34:53.000000 mapel-elections-2.0.3.dev7/src/mapel_elections.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-05-24 17:34:53.000000 mapel-elections-2.0.3.dev7/src/mapel_elections.egg-info/top_level.txt
```

### Comparing `mapel-elections-2.0.3.dev6/LICENSE.txt` & `mapel-elections-2.0.3.dev7/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `mapel-elections-2.0.3.dev6/PKG-INFO` & `mapel-elections-2.0.3.dev7/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mapel-elections
-Version: 2.0.3.dev6
+Version: 2.0.3.dev7
 Summary: Map of Elections
 Author-email: Stanislaw Szufa <s.szufa@gmail.com>, Niclas Boehmer <niclas.boehmer@tu-berlin.de>, Piotr Faliszewski <faliszew@agh.edu.pl>, Lukasz Janeczko <lukij1997@gmail.com>, Andrzej Kaczmarczyk <andrzej.kaczmarczyk@agh.edu.pl>, Tomasz Was <tomasz.t.was@gmail.com>
 License: Copyright (c) 2018-2022 Stanislaw Szufa and contributors
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
         of this software and associated documentation files (the "Software"), to deal
         in the Software without restriction, including without limitation the rights
```

### Comparing `mapel-elections-2.0.3.dev6/README.md` & `mapel-elections-2.0.3.dev7/README.md`

 * *Files identical despite different names*

### Comparing `mapel-elections-2.0.3.dev6/pyproject.toml` & `mapel-elections-2.0.3.dev7/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=65", "wheel", "pybind11>=2.6.1"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "mapel-elections"
-version = "2.0.3.dev6"
+version = "2.0.3.dev7"
 authors = [
  {name = "Stanislaw Szufa", email = "s.szufa@gmail.com"},
  {name = "Niclas Boehmer", email = "niclas.boehmer@tu-berlin.de"},
  {name = "Piotr Faliszewski", email = "faliszew@agh.edu.pl"},
  {name = "Lukasz Janeczko", email = "lukij1997@gmail.com"},
  {name = "Andrzej Kaczmarczyk", email = "andrzej.kaczmarczyk@agh.edu.pl"},
  {name = "Tomasz Was", email = "tomasz.t.was@gmail.com"},
```

### Comparing `mapel-elections-2.0.3.dev6/src/mapel/elections/__init__.py` & `mapel-elections-2.0.3.dev7/src/mapel/elections/__init__.py`

 * *Files identical despite different names*

### Comparing `mapel-elections-2.0.3.dev6/src/mapel/elections/cultures/alliances.py` & `mapel-elections-2.0.3.dev7/src/mapel/elections/cultures/alliances.py`

 * *Files identical despite different names*

### Comparing `mapel-elections-2.0.3.dev6/src/mapel/elections/cultures/didi.py` & `mapel-elections-2.0.3.dev7/src/mapel/elections/cultures/didi.py`

 * *Files identical despite different names*

### Comparing `mapel-elections-2.0.3.dev6/src/mapel/elections/cultures/euclidean.py` & `mapel-elections-2.0.3.dev7/src/mapel/elections/cultures/euclidean.py`

 * *Files identical despite different names*

### Comparing `mapel-elections-2.0.3.dev6/src/mapel/elections/cultures/fake.py` & `mapel-elections-2.0.3.dev7/src/mapel/elections/cultures/fake.py`

 * *Files identical despite different names*

### Comparing `mapel-elections-2.0.3.dev6/src/mapel/elections/cultures/field_experiment.py` & `mapel-elections-2.0.3.dev7/src/mapel/elections/cultures/field_experiment.py`

 * *Files identical despite different names*

### Comparing `mapel-elections-2.0.3.dev6/src/mapel/elections/cultures/group_separable.py` & `mapel-elections-2.0.3.dev7/src/mapel/elections/cultures/group_separable.py`

 * *Files identical despite different names*

### Comparing `mapel-elections-2.0.3.dev6/src/mapel/elections/cultures/guardians.py` & `mapel-elections-2.0.3.dev7/src/mapel/elections/cultures/guardians.py`

 * *Files identical despite different names*

### Comparing `mapel-elections-2.0.3.dev6/src/mapel/elections/cultures/guardians_plus.py` & `mapel-elections-2.0.3.dev7/src/mapel/elections/cultures/guardians_plus.py`

 * *Files identical despite different names*

### Comparing `mapel-elections-2.0.3.dev6/src/mapel/elections/cultures/impartial.py` & `mapel-elections-2.0.3.dev7/src/mapel/elections/cultures/impartial.py`

 * *Files identical despite different names*

### Comparing `mapel-elections-2.0.3.dev6/src/mapel/elections/cultures/mallows.py` & `mapel-elections-2.0.3.dev7/src/mapel/elections/cultures/mallows.py`

 * *Files identical despite different names*

### Comparing `mapel-elections-2.0.3.dev6/src/mapel/elections/cultures/noise.py` & `mapel-elections-2.0.3.dev7/src/mapel/elections/cultures/noise.py`

 * *Files identical despite different names*

### Comparing `mapel-elections-2.0.3.dev6/src/mapel/elections/cultures/params.py` & `mapel-elections-2.0.3.dev7/src/mapel/elections/cultures/params.py`

 * *Files identical despite different names*

### Comparing `mapel-elections-2.0.3.dev6/src/mapel/elections/cultures/partylist.py` & `mapel-elections-2.0.3.dev7/src/mapel/elections/cultures/partylist.py`

 * *Files identical despite different names*

### Comparing `mapel-elections-2.0.3.dev6/src/mapel/elections/cultures/preflib.py` & `mapel-elections-2.0.3.dev7/src/mapel/elections/cultures/preflib.py`

 * *Files identical despite different names*

### Comparing `mapel-elections-2.0.3.dev6/src/mapel/elections/cultures/resampling.py` & `mapel-elections-2.0.3.dev7/src/mapel/elections/cultures/resampling.py`

 * *Files identical despite different names*

### Comparing `mapel-elections-2.0.3.dev6/src/mapel/elections/cultures/sampling/samplemat.py` & `mapel-elections-2.0.3.dev7/src/mapel/elections/cultures/sampling/samplemat.py`

 * *Files identical despite different names*

### Comparing `mapel-elections-2.0.3.dev6/src/mapel/elections/cultures/single_crossing.py` & `mapel-elections-2.0.3.dev7/src/mapel/elections/cultures/single_crossing.py`

 * *Files identical despite different names*

### Comparing `mapel-elections-2.0.3.dev6/src/mapel/elections/cultures/single_peaked.py` & `mapel-elections-2.0.3.dev7/src/mapel/elections/cultures/single_peaked.py`

 * *Files identical despite different names*

### Comparing `mapel-elections-2.0.3.dev6/src/mapel/elections/cultures/sp_matrices.py` & `mapel-elections-2.0.3.dev7/src/mapel/elections/cultures/sp_matrices.py`

 * *Files identical despite different names*

### Comparing `mapel-elections-2.0.3.dev6/src/mapel/elections/cultures/unused.py` & `mapel-elections-2.0.3.dev7/src/mapel/elections/cultures/unused.py`

 * *Files identical despite different names*

### Comparing `mapel-elections-2.0.3.dev6/src/mapel/elections/cultures/urn.py` & `mapel-elections-2.0.3.dev7/src/mapel/elections/cultures/urn.py`

 * *Files identical despite different names*

### Comparing `mapel-elections-2.0.3.dev6/src/mapel/elections/cultures_.py` & `mapel-elections-2.0.3.dev7/src/mapel/elections/cultures_.py`

 * *Files identical despite different names*

### Comparing `mapel-elections-2.0.3.dev6/src/mapel/elections/distances/committee_distances.py` & `mapel-elections-2.0.3.dev7/src/mapel/elections/distances/committee_distances.py`

 * *Files identical despite different names*

### Comparing `mapel-elections-2.0.3.dev6/src/mapel/elections/distances/cppdistances.cpp` & `mapel-elections-2.0.3.dev7/src/mapel/elections/distances/cppdistances.cpp`

 * *Files identical despite different names*

### Comparing `mapel-elections-2.0.3.dev6/src/mapel/elections/distances/ilp_isomorphic.py` & `mapel-elections-2.0.3.dev7/src/mapel/elections/distances/ilp_isomorphic.py`

 * *Files identical despite different names*

### Comparing `mapel-elections-2.0.3.dev6/src/mapel/elections/distances/lp.py` & `mapel-elections-2.0.3.dev7/src/mapel/elections/distances/lp.py`

 * *Files identical despite different names*

### Comparing `mapel-elections-2.0.3.dev6/src/mapel/elections/distances/main_approval_distances.py` & `mapel-elections-2.0.3.dev7/src/mapel/elections/distances/main_approval_distances.py`

 * *Files identical despite different names*

### Comparing `mapel-elections-2.0.3.dev6/src/mapel/elections/distances/main_ordinal_distances.py` & `mapel-elections-2.0.3.dev7/src/mapel/elections/distances/main_ordinal_distances.py`

 * *Files identical despite different names*

### Comparing `mapel-elections-2.0.3.dev6/src/mapel/elections/distances_.py` & `mapel-elections-2.0.3.dev7/src/mapel/elections/distances_.py`

 * *Files identical despite different names*

### Comparing `mapel-elections-2.0.3.dev6/src/mapel/elections/features/approx.py` & `mapel-elections-2.0.3.dev7/src/mapel/elections/features/approx.py`

 * *Files identical despite different names*

### Comparing `mapel-elections-2.0.3.dev6/src/mapel/elections/features/banzhaf_cc.py` & `mapel-elections-2.0.3.dev7/src/mapel/elections/features/banzhaf_cc.py`

 * *Files identical despite different names*

### Comparing `mapel-elections-2.0.3.dev6/src/mapel/elections/features/clustering.py` & `mapel-elections-2.0.3.dev7/src/mapel/elections/features/clustering.py`

 * *Files identical despite different names*

### Comparing `mapel-elections-2.0.3.dev6/src/mapel/elections/features/cohesive.py` & `mapel-elections-2.0.3.dev7/src/mapel/elections/features/cohesive.py`

 * *Files identical despite different names*

### Comparing `mapel-elections-2.0.3.dev6/src/mapel/elections/features/dependent_rounding.py` & `mapel-elections-2.0.3.dev7/src/mapel/elections/features/dependent_rounding.py`

 * *Files identical despite different names*

### Comparing `mapel-elections-2.0.3.dev6/src/mapel/elections/features/dimensionality.py` & `mapel-elections-2.0.3.dev7/src/mapel/elections/features/dimensionality.py`

 * *Files identical despite different names*

### Comparing `mapel-elections-2.0.3.dev6/src/mapel/elections/features/distortion.py` & `mapel-elections-2.0.3.dev7/src/mapel/elections/features/distortion.py`

 * *Files identical despite different names*

### Comparing `mapel-elections-2.0.3.dev6/src/mapel/elections/features/diversity.py` & `mapel-elections-2.0.3.dev7/src/mapel/elections/features/diversity.py`

 * *Files identical despite different names*

### Comparing `mapel-elections-2.0.3.dev6/src/mapel/elections/features/justified_representation.py` & `mapel-elections-2.0.3.dev7/src/mapel/elections/features/justified_representation.py`

 * *Files identical despite different names*

### Comparing `mapel-elections-2.0.3.dev6/src/mapel/elections/features/other.py` & `mapel-elections-2.0.3.dev7/src/mapel/elections/features/other.py`

 * *Files identical despite different names*

### Comparing `mapel-elections-2.0.3.dev6/src/mapel/elections/features/partylist.py` & `mapel-elections-2.0.3.dev7/src/mapel/elections/features/partylist.py`

 * *Files identical despite different names*

### Comparing `mapel-elections-2.0.3.dev6/src/mapel/elections/features/power_index.py` & `mapel-elections-2.0.3.dev7/src/mapel/elections/features/power_index.py`

 * *Files identical despite different names*

### Comparing `mapel-elections-2.0.3.dev6/src/mapel/elections/features/proportionality_degree.py` & `mapel-elections-2.0.3.dev7/src/mapel/elections/features/proportionality_degree.py`

 * *Files identical despite different names*

### Comparing `mapel-elections-2.0.3.dev6/src/mapel/elections/features/ranging_cc.py` & `mapel-elections-2.0.3.dev7/src/mapel/elections/features/ranging_cc.py`

 * *Files identical despite different names*

### Comparing `mapel-elections-2.0.3.dev6/src/mapel/elections/features/scores.py` & `mapel-elections-2.0.3.dev7/src/mapel/elections/features/scores.py`

 * *Files identical despite different names*

### Comparing `mapel-elections-2.0.3.dev6/src/mapel/elections/features/vc_diversity.py` & `mapel-elections-2.0.3.dev7/src/mapel/elections/features/vc_diversity.py`

 * *Files identical despite different names*

### Comparing `mapel-elections-2.0.3.dev6/src/mapel/elections/features_.py` & `mapel-elections-2.0.3.dev7/src/mapel/elections/features_.py`

 * *Files identical despite different names*

### Comparing `mapel-elections-2.0.3.dev6/src/mapel/elections/objects/ApprovalElection.py` & `mapel-elections-2.0.3.dev7/src/mapel/elections/objects/ApprovalElection.py`

 * *Files identical despite different names*

### Comparing `mapel-elections-2.0.3.dev6/src/mapel/elections/objects/ApprovalElectionExperiment.py` & `mapel-elections-2.0.3.dev7/src/mapel/elections/objects/ApprovalElectionExperiment.py`

 * *Files identical despite different names*

### Comparing `mapel-elections-2.0.3.dev6/src/mapel/elections/objects/Election.py` & `mapel-elections-2.0.3.dev7/src/mapel/elections/objects/Election.py`

 * *Files identical despite different names*

### Comparing `mapel-elections-2.0.3.dev6/src/mapel/elections/objects/ElectionExperiment.py` & `mapel-elections-2.0.3.dev7/src/mapel/elections/objects/ElectionExperiment.py`

 * *Files identical despite different names*

### Comparing `mapel-elections-2.0.3.dev6/src/mapel/elections/objects/ElectionFamily.py` & `mapel-elections-2.0.3.dev7/src/mapel/elections/objects/ElectionFamily.py`

 * *Files identical despite different names*

### Comparing `mapel-elections-2.0.3.dev6/src/mapel/elections/objects/OrdinalElection.py` & `mapel-elections-2.0.3.dev7/src/mapel/elections/objects/OrdinalElection.py`

 * *Files identical despite different names*

### Comparing `mapel-elections-2.0.3.dev6/src/mapel/elections/objects/OrdinalElectionExperiment.py` & `mapel-elections-2.0.3.dev7/src/mapel/elections/objects/OrdinalElectionExperiment.py`

 * *Files identical despite different names*

### Comparing `mapel-elections-2.0.3.dev6/src/mapel/elections/other/matrices.py` & `mapel-elections-2.0.3.dev7/src/mapel/elections/other/matrices.py`

 * *Files identical despite different names*

### Comparing `mapel-elections-2.0.3.dev6/src/mapel/elections/other/matrix2png.py` & `mapel-elections-2.0.3.dev7/src/mapel/elections/other/matrix2png.py`

 * *Files identical despite different names*

### Comparing `mapel-elections-2.0.3.dev6/src/mapel/elections/other/pabulib.py` & `mapel-elections-2.0.3.dev7/src/mapel/elections/other/pabulib.py`

 * *Files identical despite different names*

### Comparing `mapel-elections-2.0.3.dev6/src/mapel/elections/other/rules.py` & `mapel-elections-2.0.3.dev7/src/mapel/elections/other/rules.py`

 * *Files identical despite different names*

### Comparing `mapel-elections-2.0.3.dev6/src/mapel/elections/other/winners.py` & `mapel-elections-2.0.3.dev7/src/mapel/elections/other/winners.py`

 * *Files identical despite different names*

### Comparing `mapel-elections-2.0.3.dev6/src/mapel/elections/persistence/election_exports.py` & `mapel-elections-2.0.3.dev7/src/mapel/elections/persistence/election_exports.py`

 * *Files identical despite different names*

### Comparing `mapel-elections-2.0.3.dev6/src/mapel/elections/persistence/election_imports.py` & `mapel-elections-2.0.3.dev7/src/mapel/elections/persistence/election_imports.py`

 * *Files identical despite different names*

### Comparing `mapel-elections-2.0.3.dev6/src/mapel_elections.egg-info/PKG-INFO` & `mapel-elections-2.0.3.dev7/src/mapel_elections.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mapel-elections
-Version: 2.0.3.dev6
+Version: 2.0.3.dev7
 Summary: Map of Elections
 Author-email: Stanislaw Szufa <s.szufa@gmail.com>, Niclas Boehmer <niclas.boehmer@tu-berlin.de>, Piotr Faliszewski <faliszew@agh.edu.pl>, Lukasz Janeczko <lukij1997@gmail.com>, Andrzej Kaczmarczyk <andrzej.kaczmarczyk@agh.edu.pl>, Tomasz Was <tomasz.t.was@gmail.com>
 License: Copyright (c) 2018-2022 Stanislaw Szufa and contributors
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
         of this software and associated documentation files (the "Software"), to deal
         in the Software without restriction, including without limitation the rights
```

### Comparing `mapel-elections-2.0.3.dev6/src/mapel_elections.egg-info/SOURCES.txt` & `mapel-elections-2.0.3.dev7/src/mapel_elections.egg-info/SOURCES.txt`

 * *Files identical despite different names*

