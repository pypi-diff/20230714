# Comparing `tmp/mapel-elections-2.0.5.tar.gz` & `tmp/mapel-elections-2.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mapel-elections-2.0.5.tar", last modified: Fri May 26 20:06:54 2023, max compression
+gzip compressed data, was "mapel-elections-2.0.6.tar", last modified: Fri Jul 14 09:02:41 2023, max compression
```

## Comparing `mapel-elections-2.0.5.tar` & `mapel-elections-2.0.6.tar`

### file list

```diff
@@ -1,94 +1,94 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 20:06:54.145794 mapel-elections-2.0.5/
--rw-r--r--   0 runner    (1001) docker     (123)     1081 2023-05-26 20:06:23.000000 mapel-elections-2.0.5/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)     3655 2023-05-26 20:06:54.145794 mapel-elections-2.0.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1801 2023-05-26 20:06:23.000000 mapel-elections-2.0.5/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       57 2023-05-26 20:06:23.000000 mapel-elections-2.0.5/optional_requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1042 2023-05-26 20:06:23.000000 mapel-elections-2.0.5/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-05-26 20:06:23.000000 mapel-elections-2.0.5/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-26 20:06:54.145794 mapel-elections-2.0.5/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      338 2023-05-26 20:06:23.000000 mapel-elections-2.0.5/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 20:06:54.125793 mapel-elections-2.0.5/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 20:06:54.125793 mapel-elections-2.0.5/src/mapel/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 20:06:54.129793 mapel-elections-2.0.5/src/mapel/elections/
--rw-r--r--   0 runner    (1001) docker     (123)     4097 2023-05-26 20:06:23.000000 mapel-elections-2.0.5/src/mapel/elections/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 20:06:54.133793 mapel-elections-2.0.5/src/mapel/elections/cultures/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-26 20:06:23.000000 mapel-elections-2.0.5/src/mapel/elections/cultures/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2913 2023-05-26 20:06:23.000000 mapel-elections-2.0.5/src/mapel/elections/cultures/alliances.py
--rw-r--r--   0 runner    (1001) docker     (123)      278 2023-05-26 20:06:23.000000 mapel-elections-2.0.5/src/mapel/elections/cultures/converters.py
--rw-r--r--   0 runner    (1001) docker     (123)      809 2023-05-26 20:06:23.000000 mapel-elections-2.0.5/src/mapel/elections/cultures/didi.py
--rw-r--r--   0 runner    (1001) docker     (123)    13776 2023-05-26 20:06:23.000000 mapel-elections-2.0.5/src/mapel/elections/cultures/euclidean.py
--rw-r--r--   0 runner    (1001) docker     (123)     6072 2023-05-26 20:06:23.000000 mapel-elections-2.0.5/src/mapel/elections/cultures/fake.py
--rw-r--r--   0 runner    (1001) docker     (123)     2468 2023-05-26 20:06:23.000000 mapel-elections-2.0.5/src/mapel/elections/cultures/field_experiment.py
--rw-r--r--   0 runner    (1001) docker     (123)    12638 2023-05-26 20:06:23.000000 mapel-elections-2.0.5/src/mapel/elections/cultures/group_separable.py
--rw-r--r--   0 runner    (1001) docker     (123)     1351 2023-05-26 20:06:23.000000 mapel-elections-2.0.5/src/mapel/elections/cultures/guardians.py
--rw-r--r--   0 runner    (1001) docker     (123)    11584 2023-05-26 20:06:23.000000 mapel-elections-2.0.5/src/mapel/elections/cultures/guardians_plus.py
--rw-r--r--   0 runner    (1001) docker     (123)     3153 2023-05-26 20:06:23.000000 mapel-elections-2.0.5/src/mapel/elections/cultures/impartial.py
--rw-r--r--   0 runner    (1001) docker     (123)     9216 2023-05-26 20:06:23.000000 mapel-elections-2.0.5/src/mapel/elections/cultures/mallows.py
--rw-r--r--   0 runner    (1001) docker     (123)     1738 2023-05-26 20:06:23.000000 mapel-elections-2.0.5/src/mapel/elections/cultures/noise.py
--rw-r--r--   0 runner    (1001) docker     (123)     8618 2023-05-26 20:06:23.000000 mapel-elections-2.0.5/src/mapel/elections/cultures/params.py
--rw-r--r--   0 runner    (1001) docker     (123)      472 2023-05-26 20:06:23.000000 mapel-elections-2.0.5/src/mapel/elections/cultures/parties.py
--rw-r--r--   0 runner    (1001) docker     (123)     1326 2023-05-26 20:06:23.000000 mapel-elections-2.0.5/src/mapel/elections/cultures/partylist.py
--rw-r--r--   0 runner    (1001) docker     (123)     8833 2023-05-26 20:06:23.000000 mapel-elections-2.0.5/src/mapel/elections/cultures/preflib.py
--rw-r--r--   0 runner    (1001) docker     (123)     2709 2023-05-26 20:06:23.000000 mapel-elections-2.0.5/src/mapel/elections/cultures/resampling.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 20:06:54.133793 mapel-elections-2.0.5/src/mapel/elections/cultures/sampling/
--rw-r--r--   0 runner    (1001) docker     (123)     3795 2023-05-26 20:06:23.000000 mapel-elections-2.0.5/src/mapel/elections/cultures/sampling/samplemat.py
--rw-r--r--   0 runner    (1001) docker     (123)     7168 2023-05-26 20:06:23.000000 mapel-elections-2.0.5/src/mapel/elections/cultures/single_crossing.py
--rw-r--r--   0 runner    (1001) docker     (123)     2420 2023-05-26 20:06:23.000000 mapel-elections-2.0.5/src/mapel/elections/cultures/single_peaked.py
--rw-r--r--   0 runner    (1001) docker     (123)     3372 2023-05-26 20:06:23.000000 mapel-elections-2.0.5/src/mapel/elections/cultures/sp_matrices.py
--rw-r--r--   0 runner    (1001) docker     (123)     8485 2023-05-26 20:06:23.000000 mapel-elections-2.0.5/src/mapel/elections/cultures/unused.py
--rw-r--r--   0 runner    (1001) docker     (123)     2826 2023-05-26 20:06:23.000000 mapel-elections-2.0.5/src/mapel/elections/cultures/urn.py
--rw-r--r--   0 runner    (1001) docker     (123)     9417 2023-05-26 20:06:23.000000 mapel-elections-2.0.5/src/mapel/elections/cultures_.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 20:06:54.133793 mapel-elections-2.0.5/src/mapel/elections/distances/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-26 20:06:23.000000 mapel-elections-2.0.5/src/mapel/elections/distances/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1921 2023-05-26 20:06:23.000000 mapel-elections-2.0.5/src/mapel/elections/distances/committee_distances.py
--rw-r--r--   0 runner    (1001) docker     (123)    16377 2023-05-26 20:06:23.000000 mapel-elections-2.0.5/src/mapel/elections/distances/cppdistances.cpp
--rw-r--r--   0 runner    (1001) docker     (123)    23722 2023-05-26 20:06:23.000000 mapel-elections-2.0.5/src/mapel/elections/distances/ilp_isomorphic.py
--rw-r--r--   0 runner    (1001) docker     (123)    45354 2023-05-26 20:06:23.000000 mapel-elections-2.0.5/src/mapel/elections/distances/lp.py
--rw-r--r--   0 runner    (1001) docker     (123)     9121 2023-05-26 20:06:23.000000 mapel-elections-2.0.5/src/mapel/elections/distances/main_approval_distances.py
--rw-r--r--   0 runner    (1001) docker     (123)     8942 2023-05-26 20:06:23.000000 mapel-elections-2.0.5/src/mapel/elections/distances/main_ordinal_distances.py
--rw-r--r--   0 runner    (1001) docker     (123)     8566 2023-05-26 20:06:23.000000 mapel-elections-2.0.5/src/mapel/elections/distances_.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 20:06:54.141793 mapel-elections-2.0.5/src/mapel/elections/features/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-26 20:06:23.000000 mapel-elections-2.0.5/src/mapel/elections/features/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7256 2023-05-26 20:06:23.000000 mapel-elections-2.0.5/src/mapel/elections/features/approx.py
--rw-r--r--   0 runner    (1001) docker     (123)     2435 2023-05-26 20:06:23.000000 mapel-elections-2.0.5/src/mapel/elections/features/banzhaf_cc.py
--rw-r--r--   0 runner    (1001) docker     (123)     3840 2023-05-26 20:06:23.000000 mapel-elections-2.0.5/src/mapel/elections/features/clustering.py
--rw-r--r--   0 runner    (1001) docker     (123)     5526 2023-05-26 20:06:23.000000 mapel-elections-2.0.5/src/mapel/elections/features/cohesive.py
--rw-r--r--   0 runner    (1001) docker     (123)     2818 2023-05-26 20:06:23.000000 mapel-elections-2.0.5/src/mapel/elections/features/dependent_rounding.py
--rw-r--r--   0 runner    (1001) docker     (123)      964 2023-05-26 20:06:23.000000 mapel-elections-2.0.5/src/mapel/elections/features/dimensionality.py
--rw-r--r--   0 runner    (1001) docker     (123)     7437 2023-05-26 20:06:23.000000 mapel-elections-2.0.5/src/mapel/elections/features/distortion.py
--rw-r--r--   0 runner    (1001) docker     (123)    21363 2023-05-26 20:06:23.000000 mapel-elections-2.0.5/src/mapel/elections/features/diversity.py
--rw-r--r--   0 runner    (1001) docker     (123)      556 2023-05-26 20:06:23.000000 mapel-elections-2.0.5/src/mapel/elections/features/justified_representation.py
--rw-r--r--   0 runner    (1001) docker     (123)     2514 2023-05-26 20:06:23.000000 mapel-elections-2.0.5/src/mapel/elections/features/other.py
--rw-r--r--   0 runner    (1001) docker     (123)     4591 2023-05-26 20:06:23.000000 mapel-elections-2.0.5/src/mapel/elections/features/partylist.py
--rw-r--r--   0 runner    (1001) docker     (123)     1259 2023-05-26 20:06:23.000000 mapel-elections-2.0.5/src/mapel/elections/features/power_index.py
--rw-r--r--   0 runner    (1001) docker     (123)     4833 2023-05-26 20:06:23.000000 mapel-elections-2.0.5/src/mapel/elections/features/proportionality_degree.py
--rw-r--r--   0 runner    (1001) docker     (123)     1369 2023-05-26 20:06:23.000000 mapel-elections-2.0.5/src/mapel/elections/features/ranging_cc.py
--rw-r--r--   0 runner    (1001) docker     (123)     8930 2023-05-26 20:06:23.000000 mapel-elections-2.0.5/src/mapel/elections/features/scores.py
--rw-r--r--   0 runner    (1001) docker     (123)      998 2023-05-26 20:06:23.000000 mapel-elections-2.0.5/src/mapel/elections/features/vc_diversity.py
--rw-r--r--   0 runner    (1001) docker     (123)     6675 2023-05-26 20:06:23.000000 mapel-elections-2.0.5/src/mapel/elections/features_.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 20:06:54.141793 mapel-elections-2.0.5/src/mapel/elections/objects/
--rw-r--r--   0 runner    (1001) docker     (123)    12608 2023-05-26 20:06:23.000000 mapel-elections-2.0.5/src/mapel/elections/objects/ApprovalElection.py
--rw-r--r--   0 runner    (1001) docker     (123)     9909 2023-05-26 20:06:23.000000 mapel-elections-2.0.5/src/mapel/elections/objects/ApprovalElectionExperiment.py
--rw-r--r--   0 runner    (1001) docker     (123)    18128 2023-05-26 20:06:23.000000 mapel-elections-2.0.5/src/mapel/elections/objects/Election.py
--rw-r--r--   0 runner    (1001) docker     (123)    28055 2023-05-26 20:06:23.000000 mapel-elections-2.0.5/src/mapel/elections/objects/ElectionExperiment.py
--rw-r--r--   0 runner    (1001) docker     (123)     6722 2023-05-26 20:06:23.000000 mapel-elections-2.0.5/src/mapel/elections/objects/ElectionFamily.py
--rw-r--r--   0 runner    (1001) docker     (123)    20127 2023-05-26 20:06:23.000000 mapel-elections-2.0.5/src/mapel/elections/objects/OrdinalElection.py
--rw-r--r--   0 runner    (1001) docker     (123)     2646 2023-05-26 20:06:23.000000 mapel-elections-2.0.5/src/mapel/elections/objects/OrdinalElectionExperiment.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-26 20:06:23.000000 mapel-elections-2.0.5/src/mapel/elections/objects/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 20:06:54.145794 mapel-elections-2.0.5/src/mapel/elections/other/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-26 20:06:23.000000 mapel-elections-2.0.5/src/mapel/elections/other/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2317 2023-05-26 20:06:23.000000 mapel-elections-2.0.5/src/mapel/elections/other/matrices.py
--rw-r--r--   0 runner    (1001) docker     (123)     3106 2023-05-26 20:06:23.000000 mapel-elections-2.0.5/src/mapel/elections/other/matrix2png.py
--rw-r--r--   0 runner    (1001) docker     (123)     3455 2023-05-26 20:06:23.000000 mapel-elections-2.0.5/src/mapel/elections/other/pabulib.py
--rw-r--r--   0 runner    (1001) docker     (123)     3955 2023-05-26 20:06:23.000000 mapel-elections-2.0.5/src/mapel/elections/other/rules.py
--rw-r--r--   0 runner    (1001) docker     (123)    13087 2023-05-26 20:06:23.000000 mapel-elections-2.0.5/src/mapel/elections/other/winners.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 20:06:54.145794 mapel-elections-2.0.5/src/mapel/elections/persistence/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-26 20:06:23.000000 mapel-elections-2.0.5/src/mapel/elections/persistence/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6851 2023-05-26 20:06:23.000000 mapel-elections-2.0.5/src/mapel/elections/persistence/election_exports.py
--rw-r--r--   0 runner    (1001) docker     (123)     7048 2023-05-26 20:06:23.000000 mapel-elections-2.0.5/src/mapel/elections/persistence/election_imports.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 20:06:54.145794 mapel-elections-2.0.5/src/mapel_elections.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3655 2023-05-26 20:06:54.000000 mapel-elections-2.0.5/src/mapel_elections.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3301 2023-05-26 20:06:54.000000 mapel-elections-2.0.5/src/mapel_elections.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-26 20:06:54.000000 mapel-elections-2.0.5/src/mapel_elections.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       85 2023-05-26 20:06:54.000000 mapel-elections-2.0.5/src/mapel_elections.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-05-26 20:06:54.000000 mapel-elections-2.0.5/src/mapel_elections.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 09:02:41.241595 mapel-elections-2.0.6/
+-rw-r--r--   0 runner    (1001) docker     (123)     1081 2023-07-14 09:02:16.000000 mapel-elections-2.0.6/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     3655 2023-07-14 09:02:41.241595 mapel-elections-2.0.6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1801 2023-07-14 09:02:16.000000 mapel-elections-2.0.6/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       57 2023-07-14 09:02:16.000000 mapel-elections-2.0.6/optional_requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1042 2023-07-14 09:02:16.000000 mapel-elections-2.0.6/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-07-14 09:02:16.000000 mapel-elections-2.0.6/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-14 09:02:41.241595 mapel-elections-2.0.6/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      338 2023-07-14 09:02:16.000000 mapel-elections-2.0.6/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 09:02:41.225595 mapel-elections-2.0.6/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 09:02:41.221595 mapel-elections-2.0.6/src/mapel/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 09:02:41.225595 mapel-elections-2.0.6/src/mapel/elections/
+-rw-r--r--   0 runner    (1001) docker     (123)     4857 2023-07-14 09:02:16.000000 mapel-elections-2.0.6/src/mapel/elections/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 09:02:41.233595 mapel-elections-2.0.6/src/mapel/elections/cultures/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-14 09:02:16.000000 mapel-elections-2.0.6/src/mapel/elections/cultures/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2910 2023-07-14 09:02:16.000000 mapel-elections-2.0.6/src/mapel/elections/cultures/alliances.py
+-rw-r--r--   0 runner    (1001) docker     (123)      278 2023-07-14 09:02:16.000000 mapel-elections-2.0.6/src/mapel/elections/cultures/converters.py
+-rw-r--r--   0 runner    (1001) docker     (123)      809 2023-07-14 09:02:16.000000 mapel-elections-2.0.6/src/mapel/elections/cultures/didi.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13776 2023-07-14 09:02:16.000000 mapel-elections-2.0.6/src/mapel/elections/cultures/euclidean.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6072 2023-07-14 09:02:16.000000 mapel-elections-2.0.6/src/mapel/elections/cultures/fake.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2468 2023-07-14 09:02:16.000000 mapel-elections-2.0.6/src/mapel/elections/cultures/field_experiment.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12638 2023-07-14 09:02:16.000000 mapel-elections-2.0.6/src/mapel/elections/cultures/group_separable.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1351 2023-07-14 09:02:16.000000 mapel-elections-2.0.6/src/mapel/elections/cultures/guardians.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11584 2023-07-14 09:02:16.000000 mapel-elections-2.0.6/src/mapel/elections/cultures/guardians_plus.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3083 2023-07-14 09:02:16.000000 mapel-elections-2.0.6/src/mapel/elections/cultures/impartial.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5124 2023-07-14 09:02:16.000000 mapel-elections-2.0.6/src/mapel/elections/cultures/mallows.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1738 2023-07-14 09:02:16.000000 mapel-elections-2.0.6/src/mapel/elections/cultures/noise.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8583 2023-07-14 09:02:16.000000 mapel-elections-2.0.6/src/mapel/elections/cultures/params.py
+-rw-r--r--   0 runner    (1001) docker     (123)      472 2023-07-14 09:02:16.000000 mapel-elections-2.0.6/src/mapel/elections/cultures/parties.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1326 2023-07-14 09:02:16.000000 mapel-elections-2.0.6/src/mapel/elections/cultures/partylist.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8871 2023-07-14 09:02:16.000000 mapel-elections-2.0.6/src/mapel/elections/cultures/preflib.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2521 2023-07-14 09:02:16.000000 mapel-elections-2.0.6/src/mapel/elections/cultures/resampling.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 09:02:41.233595 mapel-elections-2.0.6/src/mapel/elections/cultures/sampling/
+-rw-r--r--   0 runner    (1001) docker     (123)     3795 2023-07-14 09:02:16.000000 mapel-elections-2.0.6/src/mapel/elections/cultures/sampling/samplemat.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6813 2023-07-14 09:02:16.000000 mapel-elections-2.0.6/src/mapel/elections/cultures/single_crossing.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2420 2023-07-14 09:02:16.000000 mapel-elections-2.0.6/src/mapel/elections/cultures/single_peaked.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3372 2023-07-14 09:02:16.000000 mapel-elections-2.0.6/src/mapel/elections/cultures/sp_matrices.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8485 2023-07-14 09:02:16.000000 mapel-elections-2.0.6/src/mapel/elections/cultures/unused.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2821 2023-07-14 09:02:16.000000 mapel-elections-2.0.6/src/mapel/elections/cultures/urn.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9418 2023-07-14 09:02:16.000000 mapel-elections-2.0.6/src/mapel/elections/cultures_.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 09:02:41.233595 mapel-elections-2.0.6/src/mapel/elections/distances/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-14 09:02:16.000000 mapel-elections-2.0.6/src/mapel/elections/distances/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1921 2023-07-14 09:02:16.000000 mapel-elections-2.0.6/src/mapel/elections/distances/committee_distances.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16377 2023-07-14 09:02:16.000000 mapel-elections-2.0.6/src/mapel/elections/distances/cppdistances.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)    23722 2023-07-14 09:02:16.000000 mapel-elections-2.0.6/src/mapel/elections/distances/ilp_isomorphic.py
+-rw-r--r--   0 runner    (1001) docker     (123)    45354 2023-07-14 09:02:16.000000 mapel-elections-2.0.6/src/mapel/elections/distances/lp.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1382 2023-07-14 09:02:16.000000 mapel-elections-2.0.6/src/mapel/elections/distances/main_approval_distances.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8985 2023-07-14 09:02:16.000000 mapel-elections-2.0.6/src/mapel/elections/distances/main_ordinal_distances.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7713 2023-07-14 09:02:16.000000 mapel-elections-2.0.6/src/mapel/elections/distances_.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 09:02:41.237595 mapel-elections-2.0.6/src/mapel/elections/features/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-14 09:02:16.000000 mapel-elections-2.0.6/src/mapel/elections/features/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7366 2023-07-14 09:02:16.000000 mapel-elections-2.0.6/src/mapel/elections/features/approx.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2461 2023-07-14 09:02:16.000000 mapel-elections-2.0.6/src/mapel/elections/features/banzhaf_cc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3840 2023-07-14 09:02:16.000000 mapel-elections-2.0.6/src/mapel/elections/features/clustering.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5526 2023-07-14 09:02:16.000000 mapel-elections-2.0.6/src/mapel/elections/features/cohesive.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2819 2023-07-14 09:02:16.000000 mapel-elections-2.0.6/src/mapel/elections/features/dependent_rounding.py
+-rw-r--r--   0 runner    (1001) docker     (123)      962 2023-07-14 09:02:16.000000 mapel-elections-2.0.6/src/mapel/elections/features/dimensionality.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7437 2023-07-14 09:02:16.000000 mapel-elections-2.0.6/src/mapel/elections/features/distortion.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19937 2023-07-14 09:02:16.000000 mapel-elections-2.0.6/src/mapel/elections/features/diversity.py
+-rw-r--r--   0 runner    (1001) docker     (123)      556 2023-07-14 09:02:16.000000 mapel-elections-2.0.6/src/mapel/elections/features/justified_representation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2514 2023-07-14 09:02:16.000000 mapel-elections-2.0.6/src/mapel/elections/features/other.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4591 2023-07-14 09:02:16.000000 mapel-elections-2.0.6/src/mapel/elections/features/partylist.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1259 2023-07-14 09:02:16.000000 mapel-elections-2.0.6/src/mapel/elections/features/power_index.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4833 2023-07-14 09:02:16.000000 mapel-elections-2.0.6/src/mapel/elections/features/proportionality_degree.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1407 2023-07-14 09:02:16.000000 mapel-elections-2.0.6/src/mapel/elections/features/ranging_cc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9193 2023-07-14 09:02:16.000000 mapel-elections-2.0.6/src/mapel/elections/features/scores.py
+-rw-r--r--   0 runner    (1001) docker     (123)      912 2023-07-14 09:02:16.000000 mapel-elections-2.0.6/src/mapel/elections/features/vc_diversity.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6676 2023-07-14 09:02:16.000000 mapel-elections-2.0.6/src/mapel/elections/features_.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 09:02:41.237595 mapel-elections-2.0.6/src/mapel/elections/objects/
+-rw-r--r--   0 runner    (1001) docker     (123)     8932 2023-07-14 09:02:16.000000 mapel-elections-2.0.6/src/mapel/elections/objects/ApprovalElection.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9516 2023-07-14 09:02:16.000000 mapel-elections-2.0.6/src/mapel/elections/objects/ApprovalElectionExperiment.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15109 2023-07-14 09:02:16.000000 mapel-elections-2.0.6/src/mapel/elections/objects/Election.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25957 2023-07-14 09:02:16.000000 mapel-elections-2.0.6/src/mapel/elections/objects/ElectionExperiment.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6363 2023-07-14 09:02:16.000000 mapel-elections-2.0.6/src/mapel/elections/objects/ElectionFamily.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21780 2023-07-14 09:02:16.000000 mapel-elections-2.0.6/src/mapel/elections/objects/OrdinalElection.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2535 2023-07-14 09:02:16.000000 mapel-elections-2.0.6/src/mapel/elections/objects/OrdinalElectionExperiment.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-14 09:02:16.000000 mapel-elections-2.0.6/src/mapel/elections/objects/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 09:02:41.241595 mapel-elections-2.0.6/src/mapel/elections/other/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-14 09:02:16.000000 mapel-elections-2.0.6/src/mapel/elections/other/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2317 2023-07-14 09:02:16.000000 mapel-elections-2.0.6/src/mapel/elections/other/matrices.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3106 2023-07-14 09:02:16.000000 mapel-elections-2.0.6/src/mapel/elections/other/matrix2png.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3455 2023-07-14 09:02:16.000000 mapel-elections-2.0.6/src/mapel/elections/other/pabulib.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3955 2023-07-14 09:02:16.000000 mapel-elections-2.0.6/src/mapel/elections/other/rules.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13087 2023-07-14 09:02:16.000000 mapel-elections-2.0.6/src/mapel/elections/other/winners.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 09:02:41.241595 mapel-elections-2.0.6/src/mapel/elections/persistence/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-14 09:02:16.000000 mapel-elections-2.0.6/src/mapel/elections/persistence/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6754 2023-07-14 09:02:16.000000 mapel-elections-2.0.6/src/mapel/elections/persistence/election_exports.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6952 2023-07-14 09:02:16.000000 mapel-elections-2.0.6/src/mapel/elections/persistence/election_imports.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 09:02:41.241595 mapel-elections-2.0.6/src/mapel_elections.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3655 2023-07-14 09:02:41.000000 mapel-elections-2.0.6/src/mapel_elections.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3301 2023-07-14 09:02:41.000000 mapel-elections-2.0.6/src/mapel_elections.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-14 09:02:41.000000 mapel-elections-2.0.6/src/mapel_elections.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       85 2023-07-14 09:02:41.000000 mapel-elections-2.0.6/src/mapel_elections.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-07-14 09:02:41.000000 mapel-elections-2.0.6/src/mapel_elections.egg-info/top_level.txt
```

### Comparing `mapel-elections-2.0.5/LICENSE.txt` & `mapel-elections-2.0.6/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `mapel-elections-2.0.5/PKG-INFO` & `mapel-elections-2.0.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mapel-elections
-Version: 2.0.5
+Version: 2.0.6
 Summary: Map of Elections
 Author-email: Stanislaw Szufa <s.szufa@gmail.com>, Niclas Boehmer <niclas.boehmer@tu-berlin.de>, Piotr Faliszewski <faliszew@agh.edu.pl>, Lukasz Janeczko <lukij1997@gmail.com>, Andrzej Kaczmarczyk <andrzej.kaczmarczyk@agh.edu.pl>, Tomasz Was <tomasz.t.was@gmail.com>
 License: Copyright (c) 2018-2022 Stanislaw Szufa and contributors
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
         of this software and associated documentation files (the "Software"), to deal
         in the Software without restriction, including without limitation the rights
```

### Comparing `mapel-elections-2.0.5/README.md` & `mapel-elections-2.0.6/README.md`

 * *Files identical despite different names*

### Comparing `mapel-elections-2.0.5/pyproject.toml` & `mapel-elections-2.0.6/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=65", "wheel", "pybind11>=2.6.1"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "mapel-elections"
-version = "2.0.5"
+version = "2.0.6"
 authors = [
  {name = "Stanislaw Szufa", email = "s.szufa@gmail.com"},
  {name = "Niclas Boehmer", email = "niclas.boehmer@tu-berlin.de"},
  {name = "Piotr Faliszewski", email = "faliszew@agh.edu.pl"},
  {name = "Lukasz Janeczko", email = "lukij1997@gmail.com"},
  {name = "Andrzej Kaczmarczyk", email = "andrzej.kaczmarczyk@agh.edu.pl"},
  {name = "Tomasz Was", email = "tomasz.t.was@gmail.com"},
```

### Comparing `mapel-elections-2.0.5/src/mapel/elections/cultures/alliances.py` & `mapel-elections-2.0.6/src/mapel/elections/cultures/alliances.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import numpy as np
 
 from mapel.elections.cultures.impartial import generate_ordinal_ic_votes
 from mapel.elections.cultures.urn import generate_urn_votes
-from mapel.elections.cultures.mallows import generate_mallows_votes, phi_from_relphi
+from mapel.core.features.mallows import generate_mallows_votes, phi_from_normphi
 
 
 def generate_ordinal_alliance_ic_votes(num_voters: int = None,
                                        num_candidates: int = None,
                                        params: dict = None):
     """ Return: ordinal votes from Impartial Culture with alliances """
     votes = generate_ordinal_ic_votes(num_voters, num_candidates)
@@ -27,15 +27,15 @@
 
     return np.array(votes), alliances
 
 
 def generate_ordinal_alliance_norm_mallows_votes(num_voters: int = None,
                                         num_candidates: int = None,
                                         params: dict = None):
-    params['phi'] = phi_from_relphi(num_candidates, params['normphi'])
+    params['phi'] = phi_from_normphi(num_candidates, params['normphi'])
     votes = generate_mallows_votes(num_voters, num_candidates, params)
 
     alliances = np.random.choice([i for i in range(params['num_alliances'])],
                                  size=num_candidates, replace=True)
 
     return np.array(votes), alliances
```

### Comparing `mapel-elections-2.0.5/src/mapel/elections/cultures/didi.py` & `mapel-elections-2.0.6/src/mapel/elections/cultures/didi.py`

 * *Files identical despite different names*

### Comparing `mapel-elections-2.0.5/src/mapel/elections/cultures/euclidean.py` & `mapel-elections-2.0.6/src/mapel/elections/cultures/euclidean.py`

 * *Files identical despite different names*

### Comparing `mapel-elections-2.0.5/src/mapel/elections/cultures/fake.py` & `mapel-elections-2.0.6/src/mapel/elections/cultures/fake.py`

 * *Files identical despite different names*

### Comparing `mapel-elections-2.0.5/src/mapel/elections/cultures/field_experiment.py` & `mapel-elections-2.0.6/src/mapel/elections/cultures/field_experiment.py`

 * *Files identical despite different names*

### Comparing `mapel-elections-2.0.5/src/mapel/elections/cultures/group_separable.py` & `mapel-elections-2.0.6/src/mapel/elections/cultures/group_separable.py`

 * *Files identical despite different names*

### Comparing `mapel-elections-2.0.5/src/mapel/elections/cultures/guardians.py` & `mapel-elections-2.0.6/src/mapel/elections/cultures/guardians.py`

 * *Files identical despite different names*

### Comparing `mapel-elections-2.0.5/src/mapel/elections/cultures/guardians_plus.py` & `mapel-elections-2.0.6/src/mapel/elections/cultures/guardians_plus.py`

 * *Files identical despite different names*

### Comparing `mapel-elections-2.0.5/src/mapel/elections/cultures/impartial.py` & `mapel-elections-2.0.6/src/mapel/elections/cultures/impartial.py`

 * *Files 5% similar despite different names*

```diff
@@ -43,19 +43,18 @@
                                num_candidates: int = None,
                                p: float = 0.5) -> list:
     """ Return: approval votes from impartial culture
         Params: there is a single 'p' parameter which defines the ratio
                 of candidates approves by each candidate (default p=0.5) """
     if p > 1 or p < 0:
         logging.warning(f'Incorrect value of p: {p}. Value should be in [0,1]')
-    votes = [set() for _ in range(num_voters)]
-    for i in range(num_voters):
-        for j in range(num_candidates):
-            if np.random.random() <= p:
-                votes[i].add(j)
+
+    votes = [set(j for j in range(num_candidates) if np.random.random() <= p)
+             for _ in range(num_voters)]
+
     return votes
 
 
 def generate_approval_id_votes(num_voters: int = None,
                                num_candidates: int = None,
                                p: float = 0.5) -> list:
     """ Return: approval votes from identity culture
```

### Comparing `mapel-elections-2.0.5/src/mapel/elections/cultures/mallows.py` & `mapel-elections-2.0.6/src/mapel/elections/cultures/unused.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,296 +1,264 @@
-import copy
-import os
-import pickle
-import random
-
 import numpy as np
-import logging
+from mapel.elections.cultures.single_peaked import generate_ordinal_sp_conitzer_votes, generate_ordinal_sp_walsh_votes
 
 
-# Given the number m of candidates and a phi\in [0,1] function computes the expected number of swaps
-# in a vote sampled from Mallows culture_id
-def calculateExpectedNumberSwaps(num_candidates, phi):
-    res = phi * num_candidates / (1 - phi)
-    for j in range(1, num_candidates + 1):
-        res = res + (j * (phi ** j)) / ((phi ** j) - 1)
-    return res
-
-
-# Given the number m of candidates and a absolute number of expected swaps exp_abs, this function
-# returns a value of phi such that in a vote sampled from Mallows culture_id with this parameter
-# the expected number of swaps is exp_abs
-def phi_from_relphi(num_candidates, relphi=None):
-    if relphi is None:
-        logging.warning('normphi is not defined')
-        return -1
-    if relphi == 1:
-        return 1
-    if relphi > 2 or relphi < 0:
-        logging.warning("Incorrect normphi value")
-    if relphi > 1:
-        return 2-relphi
-    exp_abs = relphi * (num_candidates * (num_candidates - 1)) / 4
-    low = 0
-    high = 1
-    while low <= high:
-        mid = (high + low) / 2
-        cur = calculateExpectedNumberSwaps(num_candidates, mid)
-        if abs(cur - exp_abs) < 1e-5:
-            return mid
-        # If x is greater, ignore left half
-        if cur < exp_abs:
-            low = mid
-
-        # If x is smaller, ignore right half
-        elif cur > exp_abs:
-            high = mid
-
-    # If we reach here, then the element was not present
-    return -1
-
-
-def phi_from_normphi(num_candidates=10, normphi=None):
-    return phi_from_relphi(num_candidates, relphi=normphi)
-
-def computeInsertionProbas(i, phi):
-    probas = (i + 1) * [0]
-    for j in range(i + 1):
-        probas[j] = pow(phi, (i + 1) - (j + 1))
-    return probas
-
-
-def weighted_choice(choices):
-    total = 0
-    for w in choices:
-        total = total + w
-    r = np.random.uniform(0, total)
-    upto = 0.0
-    for i, w in enumerate(choices):
-        if upto + w >= r:
-            return i
-        upto = upto + w
-    assert False, "Shouldn't get here"
-
-
-def mallowsVote(m, insertion_probabilites_list):
-    vote = [0]
-    for i in range(1, m):
-        index = weighted_choice(insertion_probabilites_list[i - 1])
-        vote.insert(index, i)
-    return vote
-
-
-def generate_mallows_votes(num_voters, num_candidates, phi=None, weight=0, **kwargs):
-    if phi is None:
-        logging.warning('phi is not defined')
-    insertion_probabilites_list = []
-    for i in range(1, num_candidates):
-        insertion_probabilites_list.append(computeInsertionProbas(i, phi))
-    V = []
-    for i in range(num_voters):
-        vote = mallowsVote(num_candidates, insertion_probabilites_list)
-        if weight > 0:
-            probability = np.random.random()
-            if probability <= weight:
-                vote.reverse()
-        V += [vote]
-    return V
-
-
-def generate_norm_mallows_mixture_votes(num_voters, num_candidates, params):
-    phi_1 = phi_from_normphi(num_candidates, float(params['normphi_1']))
-    params_1 = {'weight': 0, 'phi': phi_1}
-    votes_1 = generate_mallows_votes(num_voters, num_candidates, params_1)
-
-
-    phi_2 = phi_from_normphi(num_candidates, float(params['normphi_2']))
-    params_2 = {'weight': 1, 'phi': phi_2}
-    votes_2 = generate_mallows_votes(num_voters, num_candidates, params_2)
+def generate_ic_party(num_voters: int = None, params: dict = None) -> list:
+    """ Return: party votes from Impartial Culture"""
+    num_parties = params['num_parties']
+    party_size = params['num_winners']
 
-    votes = []
-    size_1 = int((1-float(params['weight']))*num_voters)
-    for i in range(size_1):
-        votes.append(votes_1[i])
-    for i in range(size_1, num_voters):
-        votes.append(votes_2[i])
+    votes = np.zeros([num_voters, num_parties], dtype=int)
 
-    return votes
+    for j in range(num_voters):
+        votes[j] = np.random.permutation(num_parties)
 
+    new_votes = [[] for _ in range(num_voters)]
+    for i in range(num_voters):
+        for j in range(num_parties):
+            for w in range(party_size):
+                _id = votes[i][j] * party_size + w
+                new_votes[i].append(_id)
+    return new_votes
 
-def calculateZpoly(m):
-    res = [1]
-    for i in range(1, m + 1):
-        mult = [1] * i
-        res2 = [0] * (len(res) + len(mult) - 1)
-        for o1, i1 in enumerate(res):
-            for o2, i2 in enumerate(mult):
-                res2[o1 + o2] += i1 * i2
-        res = res2
-    return res
-
-
-def evaluatePolynomial(coeff, x):
-    res = 0
-    for i, c in enumerate(coeff):
-        res += c * (x ** i)
-    return res
-
-
-def calculateZ(m, phi):
-    coeff = calculateZpoly(m)
-    return evaluatePolynomial(coeff, phi)
-
-
-# mat[i][j] is the probability with which candidate i ends up in position j
-def mallowsMatrix(num_candidates, lphi, pos, normalize=True):
-    mat = np.zeros([num_candidates, num_candidates])
-    if normalize:
-        phi = phi_from_relphi(num_candidates, lphi)
-    else:
-        phi = lphi
-    Z = calculateZ(num_candidates, phi)
-    for i in range(num_candidates):
+
+def generate_weighted_stratification_votes(num_voters: int = None, num_candidates: int = None,
+                                           params=None):
+    if params is None:
+        params = {}
+
+    w = params.get('w', 0.5)
+
+    return [list(np.random.permutation(int(w*num_candidates))) +
+             list(np.random.permutation([j for j in range(int(w*num_candidates), num_candidates)]))
+            for _ in range(num_voters)]
+
+
+def generate_sp_party(model=None, num_voters=None, num_candidates=None, params=None) -> np.ndarray:
+    candidates = [[] for _ in range(num_candidates)]
+    _ids = [i for i in range(num_candidates)]
+
+    for j in range(params['num_parties']):
+        for w in range(params['num_winners']):
+            _id = j * params['num_winners'] + w
+            candidates[_id] = [np.random.normal(params['party'][j][0], params['var'])]
+
+    mapping = [x for _, x in sorted(zip(candidates, _ids))]
+
+    if model == 'conitzer_party':
+        votes = generate_ordinal_sp_conitzer_votes(num_voters=num_voters,
+                                                   num_candidates=num_candidates)
+    elif model == 'walsh_party':
+        votes = generate_ordinal_sp_walsh_votes(num_voters=num_voters,
+                                                num_candidates=num_candidates)
+    for i in range(num_voters):
         for j in range(num_candidates):
-            freqs = [pos[k][i][j] for k in
-                     range(1 + int(num_candidates * (num_candidates - 1) / 2))]
-            unnormal_prob = evaluatePolynomial(freqs, phi)
-            mat[i][j] = unnormal_prob / Z
-    return mat
+            votes[i][j] = mapping[votes[i][j]]
 
+    return votes
 
-def get_mallows_matrix(num_candidates, params, normalize=True):
-    lphi = params['normphi']
-    if 'weight' not in params:
-        weight = 0
-    else:
-        weight = params['weight']
 
-    if 'sec_normphi' not in params:
-        lphi_2 = lphi
-    else:
-        lphi_2 = params['sec_normphi']
 
-    try:
-        path = os.path.join(os.getcwd(), 'mapel', 'elections', 'cultures', 'mallows_positionmatrices',
-                            str(num_candidates) + "_matrix.txt")
-        with open(path, "r") as file:
-            pos = pickle.load(file)
-    except FileNotFoundError:
-        print("Mallows matrix only supported for up to 30 candidates")
-    mat1 = mallowsMatrix(num_candidates, lphi, pos, normalize)
-    mat2 = mallowsMatrix(num_candidates, lphi_2, pos, normalize)
-    res = np.zeros([num_candidates, num_candidates])
-    for i in range(num_candidates):
-        for j in range(num_candidates):
-            res[i][j] = (1.-weight) * mat1[i][j] + (weight) * mat2[i][num_candidates - 1 - j]
-    return res
+def generate_approval_urn_votes(num_voters: int = None,
+                                num_candidates: int = None,
+                                params: dict = None) -> list:
+    """ Return: approval votes from an approval variant of Polya-Eggenberger urn culture """
 
+    votes = []
+    urn_size = 1.
+    for j in range(num_voters):
+        rho = np.random.uniform(0, urn_size)
+        if rho <= 1.:
+            vote = set()
+            for c in range(num_candidates):
+                if np.random.random() <= params['p']:
+                    vote.add(c)
+            votes.append(vote)
+        else:
+            votes.append(votes[np.random.randint(0, j)])
+        urn_size += params['alpha']
 
-def get_mallows_vectors(num_candidates, fake_param):
-    return get_mallows_matrix(num_candidates, fake_param).transpose()
+    return votes
 
 
-def generate_mallows_party(num_voters=None, num_candidates=None,
-                           election_model=None, params=None):
-    num_parties = params['num_parties']
-    num_winners = params['num_winners']
-    party_size = num_winners
+def generate_approval_simplex_resampling_votes(num_voters=None, num_candidates=None,
+                                                    params=None):
+        if 'phi' not in params:
+            phi = np.random.random()
+        else:
+            phi = params['phi']
+
+        if 'g' not in params:
+            num_groups = 2
+        else:
+            num_groups = params['g']
+
+        if 'max_range' not in params:
+            params['max_range'] = 1.
+
+        sizes_c = [0.1, 0.1, 0.1, 0.1, 0.1, 0.1, 0.1]
+        # sizes_c = runif_in_simplex(num_groups)
+        sizes_c = np.concatenate(([0], sizes_c))
+        sizes_c = np.cumsum(sizes_c)
+        print(sizes_c)
+
+        sum = 71 + 5*8
+
+        sizes_v = [71/sum, 8/sum, 8/sum, 8/sum, 8/sum, 8/sum]
+        # sizes_v = runif_in_simplex(num_groups)
+        sizes_v = np.concatenate(([0], sizes_v))
+        sizes_v = np.cumsum(sizes_v)
+        print(sizes_v)
+
+        votes = [set() for _ in range(num_voters)]
+
+        for g in range(num_groups):
+
+            central_vote = {i for i in range(int(sizes_c[g] * num_candidates),
+                                             int(sizes_c[g+1] * num_candidates))}
+
+            for v in range(int(sizes_v[g] * num_voters), int(sizes_v[g + 1] * num_voters)):
+                vote = set()
+                for c in range(num_candidates):
+                    if np.random.random() <= phi:
+                        if np.random.random() <= params['p']:
+                            vote.add(c)
+                    else:
+                        if c in central_vote:
+                            vote.add(c)
+                votes[v] = vote
+
+            # sum_p = sum([sum(vote) for vote in votes])
+            # avg_p = sum_p / (num_voters * num_candidates)
+            # print(avg_p, params['max_range'])
+            # if avg_p < params['max_range']:
+            #     break
 
-    params['phi'] = phi_from_relphi(num_parties, relphi=params['main-phi'])
-    mapping = generate_mallows_votes(num_voters, num_parties, params)[0]
+        return votes
 
-    params['phi'] = phi_from_relphi(num_parties, relphi=params['normphi'])
-    votes = generate_mallows_votes(num_voters, num_parties, params)
+def approval_anti_pjr_votes(num_voters=None, num_candidates=None, params=None):
 
-    for i in range(num_voters):
-        for j in range(num_parties):
-            votes[i][j] = mapping[votes[i][j]]
+    if 'p' not in params:
+        p = np.random.random()
+    else:
+        p = params['p']
 
-    new_votes = [[] for _ in range(num_voters)]
+    if 'phi' not in params:
+        phi = np.random.random()
+    else:
+        phi = params['phi']
 
-    for i in range(num_voters):
-        for j in range(num_parties):
-            for w in range(party_size):
-                _id = votes[i][j] * party_size + w
-                new_votes[i].append(_id)
+    if 'g' not in params:
+        num_groups = 2
+    else:
+        num_groups = params['g']
 
-    return new_votes
+    c_group_size = int(num_candidates/num_groups)
+    v_group_size = int(num_voters/num_groups)
+    size = int(p * num_candidates)
 
+    votes = []
+    for g in range(num_groups):
 
+        core = {g * c_group_size + i for i in range(c_group_size)}
+        rest = set(list(range(num_candidates))) - core
 
+        if size <= c_group_size:
+            central_vote = set(np.random.choice(list(core), size=size))
+        else:
+            central_vote = set(np.random.choice(list(rest), size=size-c_group_size))
+            central_vote = central_vote.union(core)
+
+        for v in range(v_group_size):
+            vote = set()
+            for c in range(num_candidates):
+                if np.random.random() <= phi:
+                    if np.random.random() <= p:
+                        vote.add(c)
+                else:
+                    if c in central_vote:
+                        vote.add(c)
+            votes.append(vote)
 
+    return votes
 
-# def generate_approval_hamming_noise_model_votes(num_voters=None, num_candidates=None, params=None):
-#     k = int(params['p'] * num_candidates)
-#     central_vote = {i for i in range(k)}
-#
-#     votes = [set() for _ in range(num_voters)]
-#     for v in range(num_voters):
-#         vote = set()
-#         for c in range(num_candidates):
-#             if c in central_vote:
-#                 if np.random.random() <= 1 - params['phi']:
-#                     vote.add(c)
-#             else:
-#                 if np.random.random() < params['phi']:
-#                     vote.add(c)
-#         votes[v] = vote
-#
-#     return votes
 
+def approval_partylist_votes_old(num_voters=None, num_candidates=None, params=None):
 
-def generate_approval_truncated_mallows_votes(num_voters=None, num_candidates=None, max_range=1,
-                                              normphi=None, weight=None):
+    if 'g' not in params:
+        num_groups = 2
+    else:
+        num_groups = params['g']
 
-    phi = phi_from_relphi(num_candidates, relphi=normphi)
+    if 'is_shifted' not in params:
+        shift = False
+    else:
+        shift = True
 
-    ordinal_votes = generate_mallows_votes(num_voters, num_candidates, phi=phi, weight=weight)
+    if 'm' not in params:
+        m = 0
+    else:
+        m = params['m']
 
+    c_group_size = int(num_candidates/num_groups)
+    v_group_size = int(num_voters/num_groups)
 
     votes = []
-    k = np.random.randint(low=1., high=int(max_range * num_candidates))
-    for v in range(num_voters):
-        votes.append(set(ordinal_votes[v][0:k]))
+    if not shift:
+        for g in range(num_groups):
+            for v in range(v_group_size):
+                vote = set()
+                for c in range(c_group_size):
+                    c += g*c_group_size
+                    vote.add(c)
+                for _ in range(m):
+                    el = random.sample(vote, 1)[0]
+                    vote.remove(el)
+                votes.append(vote)
+    else:
+        shift = int(c_group_size/2)
+        for g in range(num_groups):
+            for v in range(int(v_group_size/2)):
+                vote = set()
+                for c in range(c_group_size):
+                    c += g*c_group_size
+                    vote.add(c)
+                for _ in range(m):
+                    el = random.sample(vote, 1)[0]
+                    vote.remove(el)
+                votes.append(vote)
+
+            for v in range(int(v_group_size/2), v_group_size):
+                vote = set()
+                for c in range(c_group_size):
+                    c += g*c_group_size + shift
+                    c %= num_candidates
+                    vote.add(c)
+                for _ in range(m):
+                    el = random.sample(vote, 1)[0]
+                    vote.remove(el)
+                votes.append(vote)
 
     return votes
 
 
-def runif_in_simplex(n):
-  ''' Return uniformly random vector in the n-simplex '''
-
-  k = np.random.exponential(scale=1.0, size=n)
-  return k / sum(k)
-
-
+def generate_approval_exp_partylist_votes(num_voters=None, num_candidates=None, params=None):
 
+    if params is None:
+        params = {}
 
-def mallows_vote(vote, phi):
-    num_candidates = len(vote)
-    raw_vote = generate_mallows_votes(1, num_candidates, phi)[0]
-    new_vote = [0] * len(vote)
-    for i in range(num_candidates):
-        new_vote[raw_vote[i]] = vote[i]
-    return new_vote
+    num_groups = params.get('g', 5)
+    exp = params.get('exp', 2.)
 
+    sizes = np.array([1./exp**(i+1) for i in range(num_groups)])
+    sizes = sizes / np.sum(sizes)
+    party_votes = np.random.choice([i for i in range(num_groups)], num_voters, p=sizes)
 
-def mallows_votes(votes, phi):
-    for i in range(len(votes)):
-        votes[i] = mallows_vote(votes[i], phi)
-    return votes
-
-
-def generate_norm_mallows_with_walls_votes(num_voters, num_candidates, params):
+    party_size = int(num_candidates/num_groups)
     votes = []
-    upper_half_size = int(num_candidates*params['p'])
-    if upper_half_size == 0 or upper_half_size == num_candidates:
-        return np.array(generate_mallows_votes(num_voters, num_candidates, params))
-
-    lower_half_size = num_candidates - upper_half_size
-    upper_half_votes = np.array(generate_mallows_votes(num_voters, upper_half_size, params))
-    lower_half_votes = np.array(generate_mallows_votes(num_voters, lower_half_size, params)) \
-                       + upper_half_size
+
     for i in range(num_voters):
-        v = np.concatenate([upper_half_votes[i], lower_half_votes[i]])
-        votes.append(v)
-    return votes
+        shift = party_votes[i]*party_size
+        vote = set([int(c+shift) for c in range(party_size)])
+        votes.append(vote)
 
+    return votes
```

### Comparing `mapel-elections-2.0.5/src/mapel/elections/cultures/noise.py` & `mapel-elections-2.0.6/src/mapel/elections/cultures/noise.py`

 * *Files identical despite different names*

### Comparing `mapel-elections-2.0.5/src/mapel/elections/cultures/params.py` & `mapel-elections-2.0.6/src/mapel/elections/cultures/params.py`

 * *Files 2% similar despite different names*

```diff
@@ -8,38 +8,37 @@
 
 # Ordinal
 def update_params_ordinal_mallows(params):
     if 'phi' in params and type(params['phi']) is list:
         params['phi'] = np.random.uniform(low=params['phi'][0], high=params['phi'][1])
     elif 'phi' not in params:
         params['phi'] = np.random.random()
-    # params['alpha'] = params['phi']
 
 
 def update_params_ordinal_norm_mallows(params, num_candidates):
     if 'normphi' not in params:
         params['normphi'] = np.random.random()
-    params['phi'] = mallows.phi_from_relphi(num_candidates, relphi=params['normphi'])
+    params['phi'] = mallows.phi_from_normphi(num_candidates, relphi=params['normphi'])
     if 'weight' not in params:
         params['weight'] = 0.
 
 
 def update_params_ordinal_urn_model(params):
     if 'alpha' not in params:
         params['alpha'] = gamma.rvs(0.8)
 
 
 def update_params_ordinal_mallows_matrix_path(params, num_candidates):
     params['normphi'] = params['alpha']
-    params['phi'] = mallows.phi_from_relphi(num_candidates, relphi=params['normphi'])
+    params['phi'] = mallows.phi_from_normphi(num_candidates, relphi=params['normphi'])
 
 
 def update_params_ordinal_mallows_triangle(params, num_candidates):
     params['normphi'] = 1 - np.sqrt(np.random.uniform())
-    params['phi'] = mallows.phi_from_relphi(num_candidates, relphi=params['normphi'])
+    params['phi'] = mallows.phi_from_normphi(num_candidates, relphi=params['normphi'])
     params['weight'] = np.random.uniform(0, 0.5)
     params['alpha'] = params['normphi']
     params['tint'] = params['weight']  # for tint on plots
 
 
 def update_params_ordinal_alpha(printing_params):
     if 'alpha' not in printing_params:
```

### Comparing `mapel-elections-2.0.5/src/mapel/elections/cultures/partylist.py` & `mapel-elections-2.0.6/src/mapel/elections/cultures/partylist.py`

 * *Files identical despite different names*

### Comparing `mapel-elections-2.0.5/src/mapel/elections/cultures/preflib.py` & `mapel-elections-2.0.6/src/mapel/elections/cultures/preflib.py`

 * *Files 0% similar despite different names*

```diff
@@ -64,15 +64,16 @@
 
     for j in range(original_num_voters):
         value = file_votes.readline().strip().split(',')
         for k in range(original_num_candidates):
             original_votes[j][k] = int(value[k])
 
     file_votes.close()
-    print(model, len(original_votes), len(np.unique(original_votes, axis=0)))
+    # print(model, len(original_votes), len(np.unique(original_votes, axis=0)))
+    return np.array(original_votes)
 
     for j in range(num_voters):
         r = np.random.randint(0, original_num_voters - 1)
         for k in range(original_num_candidates):
             votes[j][k] = original_votes[r][k]
 
     for i in range(num_voters):
```

### Comparing `mapel-elections-2.0.5/src/mapel/elections/cultures/resampling.py` & `mapel-elections-2.0.6/src/mapel/elections/cultures/resampling.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,28 +1,19 @@
 import numpy as np
 import copy
 
 
 def generate_approval_resampling_votes(num_voters=None, num_candidates=None,
                                        phi=0.5, p=0.5):
-
     k = int(p * num_candidates)
     central_vote = {i for i in range(k)}
 
-    votes = [set() for _ in range(num_voters)]
-    for v in range(num_voters):
-        vote = set()
-        for c in range(num_candidates):
-            if np.random.random() <= phi:
-                if np.random.random() <= p:
-                    vote.add(c)
-            else:
-                if c in central_vote:
-                    vote.add(c)
-        votes[v] = vote
+    votes = [{c for c in range(num_candidates) if
+              (np.random.random() <= phi and np.random.random() <= p) or c in central_vote}
+             for _ in range(num_voters)]
 
     return votes
 
 
 def generate_approval_disjoint_resampling_votes(num_voters=None, num_candidates=None,
                                                 phi=0.5, p=0.5, g=2):
     num_groups = g
```

### Comparing `mapel-elections-2.0.5/src/mapel/elections/cultures/sampling/samplemat.py` & `mapel-elections-2.0.6/src/mapel/elections/cultures/sampling/samplemat.py`

 * *Files identical despite different names*

### Comparing `mapel-elections-2.0.5/src/mapel/elections/cultures/single_crossing.py` & `mapel-elections-2.0.6/src/mapel/elections/cultures/single_crossing.py`

 * *Files 4% similar despite different names*

```diff
@@ -2,88 +2,62 @@
 
 from random import *
 
 import numpy as np
 
 
 def generate_ordinal_single_crossing_votes(num_voters: int = None,
-                                           num_candidates: int = None,
-                                           domain_id: str = 'naive') -> np.ndarray:
+                                           num_candidates: int = None) -> np.ndarray:
     """ helper function: generate simple single-crossing elections"""
 
     votes = np.zeros([num_voters, num_candidates])
 
-    # GENERATE DOMAIN
-    if domain_id == 'naive':
+    domain_size = int(num_candidates * (num_candidates - 1) / 2 + 1)
+    domain = [list(range(num_candidates)) for _ in range(domain_size)]
 
-        domain_size = int(num_candidates * (num_candidates - 1) / 2 + 1)
-
-        domain = [[i for i in range(num_candidates)] for _ in range(domain_size)]
-
-        for line in range(1, domain_size):
-
-            poss = []
-            for i in range(num_candidates - 1):
-                if domain[line - 1][i] < domain[line - 1][i + 1]:
-                    poss.append([domain[line - 1][i], domain[line - 1][i + 1]])
-
-            r = np.random.randint(0, len(poss))  # random swap
-
-            for i in range(num_candidates):
-
-                domain[line][i] = domain[line - 1][i]
-
-                if domain[line][i] == poss[r][0]:
-                    domain[line][i] = poss[r][1]
-
-                elif domain[line][i] == poss[r][1]:
-                    domain[line][i] = poss[r][0]
-
-    # elif domain_id == 'naive_pf':
-    #     domain = naive_sampler.sample()
-    elif domain_id == 'uniform':
-        return uniform_sampler.sampleElection()
-    else:
-        print('No such domain!')
-        domain = []
-
-    domain_size = len(domain)
-
-    # GENERATE VOTES
+    for line in range(1, domain_size):
+        swap_candidates = [(i, i + 1) for i in range(num_candidates - 1) if
+                           domain[line - 1][i] < domain[line - 1][i + 1]]
+        swap_indices = swap_candidates[np.random.randint(0, len(swap_candidates))]
+
+        domain[line] = domain[line - 1].copy()
+        domain[line][swap_indices[0]], domain[line][swap_indices[1]] = domain[line][
+                                                                           swap_indices[1]], \
+                                                                       domain[line][
+                                                                           swap_indices[0]]
 
     for j in range(num_voters):
         r = np.random.randint(0, domain_size)
         votes[j] = list(domain[r])
 
     return votes
 
 
 def get_single_crossing_matrix(num_candidates: int) -> np.ndarray:
     return get_single_crossing_vectors(num_candidates).transpose()
 
 
 def get_single_crossing_vectors(num_candidates: int) -> np.ndarray:
-
     matrix = np.zeros([num_candidates, num_candidates])
 
     for i in range(num_candidates):
-        for j in range(num_candidates-i):
-            matrix[i][j] = i+j
+        for j in range(num_candidates - i):
+            matrix[i][j] = i + j
 
     for i in range(num_candidates):
         for j in range(i):
             matrix[i][j] += 1
 
     sums = [1]
     for i in range(num_candidates):
-        sums.append(sums[i]+i)
+        sums.append(sums[i] + i)
 
     for i in range(num_candidates):
         matrix[i][i] += sums[i]
-        matrix[i][num_candidates-i-1] -= i
+        matrix[i][num_candidates - i - 1] -= i
 
     for i in range(num_candidates):
         denominator = sum(matrix[i])
         for j in range(num_candidates):
             matrix[i][j] /= denominator
 
     return matrix
@@ -246,9 +220,7 @@
 
 class scDomainNaiveSampler:
     def __init__(self, m):
         self.node = getSCDomainSampler(m)
 
     def sample(self):
         return self.node.sample_domain_naive()
-
-
```

### Comparing `mapel-elections-2.0.5/src/mapel/elections/cultures/single_peaked.py` & `mapel-elections-2.0.6/src/mapel/elections/cultures/single_peaked.py`

 * *Files identical despite different names*

### Comparing `mapel-elections-2.0.5/src/mapel/elections/cultures/sp_matrices.py` & `mapel-elections-2.0.6/src/mapel/elections/cultures/sp_matrices.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from random import *
 
 import numpy as np
-from mapel.elections.cultures.mallows import phi_from_relphi, mallows_votes
+from mapel.core.features.mallows import phi_from_normphi, mallows_votes
 from scipy.special import binom
 
 
 ### MATRICES ###
 
 # WALSH
 
@@ -128,24 +128,24 @@
         for t in range(m):
             P[i][t] = probW(m, i + 1, t + 1)
     return P
 
 
 ########  MALLOWS SP  ########
 def generate_conitzer_mallows_votes(num_voters, num_candidates, params):
-    params['phi'] = phi_from_relphi(num_candidates, relphi=params['normphi'])
+    params['phi'] = phi_from_normphi(num_candidates, normphi=params['normphi'])
 
     votes = generate_ordinal_sp_conitzer_votes(num_voters=num_voters, num_candidates=num_candidates)
 
     votes = mallows_votes(votes, params['phi'])
 
     return votes
 
 
 def generate_walsh_mallows_votes(num_voters, num_candidates, params):
-    params['phi'] = phi_from_relphi(num_candidates, relphi=params['normphi'])
+    params['phi'] = phi_from_normphi(num_candidates, normphi=params['normphi'])
 
     votes = generate_ordinal_sp_walsh_votes(num_voters=num_voters, num_candidates=num_candidates)
 
     votes = mallows_votes(votes, params['phi'])
 
     return votes
```

### Comparing `mapel-elections-2.0.5/src/mapel/elections/cultures/urn.py` & `mapel-elections-2.0.6/src/mapel/elections/cultures/urn.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 #!/usr/bin/env python
 import logging
 
 import numpy as np
 
-from mapel.elections.cultures.mallows import mallows_votes
+from mapel.core.features.mallows import mallows_votes
 
 
 ###########
 # ORDINAL #
 ###########
 def generate_urn_votes(num_voters: int = None,
                        num_candidates: int = None,
```

### Comparing `mapel-elections-2.0.5/src/mapel/elections/cultures_.py` & `mapel-elections-2.0.6/src/mapel/elections/cultures_.py`

 * *Files 0% similar despite different names*

```diff
@@ -110,14 +110,15 @@
 
 
 def generate_ordinal_votes(culture_id: str = None,
                            num_candidates: int = None,
                            num_voters: int = None,
                            params: dict = None,
                            **kwargs) -> Union[list, np.ndarray]:
+
     if culture_id in LIST_OF_PREFLIB_MODELS:
         return generate_preflib_votes(culture_id=culture_id,
                                       num_candidates=num_candidates,
                                       num_voters=num_voters,
                                       params=params)
 
     elif culture_id in registered_ordinal_cultures:
```

### Comparing `mapel-elections-2.0.5/src/mapel/elections/distances/committee_distances.py` & `mapel-elections-2.0.6/src/mapel/elections/distances/committee_distances.py`

 * *Files identical despite different names*

### Comparing `mapel-elections-2.0.5/src/mapel/elections/distances/cppdistances.cpp` & `mapel-elections-2.0.6/src/mapel/elections/distances/cppdistances.cpp`

 * *Files identical despite different names*

### Comparing `mapel-elections-2.0.5/src/mapel/elections/distances/ilp_isomorphic.py` & `mapel-elections-2.0.6/src/mapel/elections/distances/ilp_isomorphic.py`

 * *Files identical despite different names*

### Comparing `mapel-elections-2.0.5/src/mapel/elections/distances/lp.py` & `mapel-elections-2.0.6/src/mapel/elections/distances/lp.py`

 * *Files identical despite different names*

### Comparing `mapel-elections-2.0.5/src/mapel/elections/distances/main_ordinal_distances.py` & `mapel-elections-2.0.6/src/mapel/elections/distances/main_ordinal_distances.py`

 * *Files 0% similar despite different names*

```diff
@@ -5,14 +5,16 @@
 
 from mapel.core.matchings import *
 from mapel.elections.objects.OrdinalElection import OrdinalElection
 import mapel.core.utils as utils
 from mapel.core.inner_distances import swap_distance
 import mapel.elections.distances.ilp_isomorphic as ilp_iso
 
+import mapel.elections.distances.lp as lp
+
 try:
     import mapel.elections.distances.cppdistances as cppd
 except:
     logging.warning("The quick C++ procedures for computing the swap and "
                     "Spearman distance is unavailable: using the (slow) python one instead")
```

### Comparing `mapel-elections-2.0.5/src/mapel/elections/distances_.py` & `mapel-elections-2.0.6/src/mapel/elections/distances_.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,35 +1,30 @@
 #!/usr/bin/env python
 import logging
 from time import time
 from typing import Callable
 from tqdm import tqdm
 
 import copy
-import os
-import csv
 import numpy as np
 
 from mapel.elections.distances import main_approval_distances as mad
 from mapel.elections.distances import main_ordinal_distances as mod
 from mapel.core.inner_distances import map_str_to_func
 from mapel.elections.objects.ApprovalElection import ApprovalElection
 from mapel.elections.objects.OrdinalElection import OrdinalElection
 from mapel.core.objects.Experiment import Experiment
 
+import mapel.core.persistence.experiment_exports as exports
+
 
 registered_approval_distances = {
     'approvalwise': mad.compute_approvalwise,
 
     'hamming': mad.compute_hamming,  # unsupported distance
-    'flow': mad.compute_flow,  # unsupported distance
-    'coapproval_frequency': mad.compute_coapproval_frequency_vectors,  # unsupported distance
-    'pairwise': mad.compute_pairwise,  # unsupported distance
-    'voterlikeness': mad.compute_voterlikeness,  # unsupported distance
-    'candidatelikeness': mad.compute_candidatelikeness,  # unsupported distance
 }
 
 registered_ordinal_distances = {
     'positionwise': mod.compute_positionwise_distance,
     'bordawise': mod.compute_bordawise_distance,
     'pairwise': mod.compute_pairwise_distance,
     'discrete': mod.compute_discrete_distance,
@@ -116,16 +111,19 @@
         inner_distance = map_str_to_func(inner_distance)
     else:
         main_distance = distance_id
         inner_distance = None
     return inner_distance, main_distance
 
 
-def run_single_process(exp: Experiment, instances_ids: list,
-                       distances: dict, times: dict, matchings: dict,
+def run_single_process(exp: Experiment,
+                       instances_ids: list,
+                       distances: dict,
+                       times: dict,
+                       matchings: dict,
                        safe_mode=False) -> None:
     """ Single process for computing distances """
 
     for instance_id_1, instance_id_2 in tqdm(instances_ids, desc='Computing distances'):
         start_time = time()
         if safe_mode:
             distance = get_distance(copy.deepcopy(exp.instances[instance_id_1]),
@@ -142,16 +140,19 @@
             matchings[instance_id_2][instance_id_1] = np.argsort(matching)
         distances[instance_id_1][instance_id_2] = distance
         distances[instance_id_2][instance_id_1] = distances[instance_id_1][instance_id_2]
         times[instance_id_1][instance_id_2] = time() - start_time
         times[instance_id_2][instance_id_1] = times[instance_id_1][instance_id_2]
 
 
-def run_multiple_processes(exp: Experiment, instances_ids: list,
-                           distances: dict, times: dict, matchings: dict,
+def run_multiple_processes(exp: Experiment,
+                           instances_ids: list,
+                           distances: dict,
+                           times: dict,
+                           matchings: dict,
                            t) -> None:
     """ Single process for computing distances """
 
     for instance_id_1, instance_id_2 in tqdm(instances_ids,
                                              desc=f'Computing distances of thread {t}'):
         start_time = time()
         distance = get_distance(copy.deepcopy(exp.instances[instance_id_1]),
@@ -164,26 +165,15 @@
             matchings[instance_id_2][instance_id_1] = np.argsort(matching)
         distances[instance_id_1][instance_id_2] = distance
         distances[instance_id_2][instance_id_1] = distances[instance_id_1][instance_id_2]
         times[instance_id_1][instance_id_2] = time() - start_time
         times[instance_id_2][instance_id_1] = times[instance_id_1][instance_id_2]
 
     if exp.is_exported:
-        _store_distances(exp, instances_ids, distances, times, t)
-
+        exports.export_distances_helper(exp, instances_ids, distances, times, t)
 
-def _store_distances(exp, instances_ids, distances, times, t):
-    """ Store distances to csv file """
-    file_name = f'{exp.distance_id}_p{t}.csv'
-    path = os.path.join(os.getcwd(), "experiments", exp.experiment_id, "distances", file_name)
-    with open(path, 'w', newline='') as csv_file:
-        writer = csv.writer(csv_file, delimiter=';')
-        writer.writerow(["instance_id_1", "instance_id_2", "distance", "time"])
-        for election_id_1, election_id_2 in instances_ids:
-            distance = float(distances[election_id_1][election_id_2])
-            time_ = float(times[election_id_1][election_id_2])
-            writer.writerow([election_id_1, election_id_2, distance, time_])
 
 
 # # # # # # # # # # # # # # # #
-# LAST CLEANUP ON: 17.08.2022 #
+# LAST CLEANUP ON: 11.07.2023 #
 # # # # # # # # # # # # # # # #
+
```

### Comparing `mapel-elections-2.0.5/src/mapel/elections/features/approx.py` & `mapel-elections-2.0.6/src/mapel/elections/features/approx.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,15 +2,16 @@
 from mapel.elections.distances.lp import solve_rand_approx_pav
 from mapel.elections.features.scores import get_score, get_dissat
 
 
 # NEW LP
 def get_rand_approx_pav_score(election, committee_size=1):
     if election.fake:
-        return 'None'
+        return {'value': None}
+
     W = [1 / (i + 1) for i in range(election.num_candidates)]
 
     C = np.zeros([election.num_voters, election.num_candidates])
     for i, vote in enumerate(election.votes):
         for j, c in enumerate(vote):
             C[i][c] = j
     # is C equivalent to potes?
@@ -29,17 +30,18 @@
 
 def get_greedy_approx_pav_score(election, committee_size=1):
     return get_greedy_approx_score(election, 'pav', committee_size=committee_size)
 
 
 def get_greedy_approx_score(election, rule, committee_size=1):
     if election.fake:
-        return 'None', 'None'
+        return {'value': None, 'dissat': None}
     winners = get_winners_approx_greedy(election, committee_size, rule)
-    return get_score(election, winners, rule), get_dissat(election, winners, rule)
+    return {'value': get_score(election, winners, rule),
+            'dissat': get_dissat(election, winners, rule)}
 
 
 def get_winners_approx_greedy(election, committee_size, rule):
     """ universal function """
 
     owa_vector, scoring_vector = get_vectors(election, rule, committee_size)
 
@@ -119,18 +121,19 @@
 
 def get_removal_approx_pav_score(election, committee_size=1):
     return get_removal_approx_score(election, "pav", committee_size=committee_size)
 
 
 def get_removal_approx_score(election, rule, committee_size=1):
     if election.fake:
-        return 'None', 'None'
+        return {'value': None, 'dissat': None}
     winners = get_winners_approx_removal(election, committee_size, rule)
 
-    return get_score(election, winners, rule), get_dissat(election, winners, rule)
+    return {'value': get_score(election, winners, rule),
+            'dissat': get_dissat(election, winners, rule)}
 
 
 def get_winners_approx_removal(election, committee_size, rule):
 
     owa_vector, scoring_vector = get_vectors(election, rule, committee_size)
 
     def simple(active, vote, target, owa_vector, scoring_vector):
```

### Comparing `mapel-elections-2.0.5/src/mapel/elections/features/banzhaf_cc.py` & `mapel-elections-2.0.6/src/mapel/elections/features/banzhaf_cc.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,17 +1,16 @@
 
 import scipy.special
 
 from mapel.elections.features.scores import get_cc_score, get_cc_dissat
-import time
 
 
 def get_banzhaf_cc_score(election, committee_size=1):
     if election.fake:
-        return 'None', 'None'
+        return {'value': None, 'dissat': None}
 
     winners = set()
     BASE = {}
     BINOM = {}
 
     for _ in range(committee_size):
         highest_c = 0
@@ -22,15 +21,15 @@
             candidate_score = sum([voter_score(BASE, BINOM, election, v, c, committee_size, winners)
                                    for v in range(election.num_voters)])
             if candidate_score > highest_score:
                 highest_score = candidate_score
                 highest_c = c
         winners.add(highest_c)
 
-    return get_cc_score(election, winners), get_cc_dissat(election, winners)
+    return {'value': get_cc_score(election, winners), 'dissat': get_cc_dissat(election, winners)}
 
 
 def voter_score(BASE, BINOM, election, v, c, committee_size, winners):
 
     potes = election.get_potes()
     m = election.num_candidates
```

### Comparing `mapel-elections-2.0.5/src/mapel/elections/features/clustering.py` & `mapel-elections-2.0.6/src/mapel/elections/features/clustering.py`

 * *Files identical despite different names*

### Comparing `mapel-elections-2.0.5/src/mapel/elections/features/cohesive.py` & `mapel-elections-2.0.6/src/mapel/elections/features/cohesive.py`

 * *Files identical despite different names*

### Comparing `mapel-elections-2.0.5/src/mapel/elections/features/dependent_rounding.py` & `mapel-elections-2.0.6/src/mapel/elections/features/dependent_rounding.py`

 * *Files 0% similar despite different names*

```diff
@@ -94,14 +94,15 @@
             else:
                 node.children[1].value = 0
                 node.election_id = node.children[0].election_id
 
         if a+b == 1.:
             node.value = None
 
+
 def _get_final_values_from_tree(node, values):
     if node.value is not None and node.election_id not in values:
         values[node.election_id] = int(node.value)
     for child in node.children:
         _get_final_values_from_tree(child, values)
```

### Comparing `mapel-elections-2.0.5/src/mapel/elections/features/dimensionality.py` & `mapel-elections-2.0.6/src/mapel/elections/features/dimensionality.py`

 * *Files 14% similar despite different names*

```diff
@@ -5,15 +5,15 @@
     import pandas as pd
 except:
     pass
 
 
 def min_dim(election):
     if election.fake:
-        return 'None'
+        return None
 
     election.set_default_object_type('vote')
     election.compute_distances(distance_id='swap')
 
     df = election.distances['vote']
     df = pd.DataFrame(df, columns=[str(i) for i in range(election.num_voters)])
```

### Comparing `mapel-elections-2.0.5/src/mapel/elections/features/distortion.py` & `mapel-elections-2.0.6/src/mapel/elections/features/distortion.py`

 * *Files identical despite different names*

### Comparing `mapel-elections-2.0.5/src/mapel/elections/features/diversity.py` & `mapel-elections-2.0.6/src/mapel/elections/features/diversity.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,327 +1,345 @@
 import math
 
 import numpy as np
 import itertools
-# AUXILIARY FUNCTIONS
-from mapel.core.glossary import LIST_OF_FAKE_MODELS
-
 
 def kemeny_ranking(election):
     m = election.num_candidates
     wmg = election.votes_to_pairwise_matrix()
     best_d = np.infty
     for test_ranking in itertools.permutations(list(range(m))):
         dist = 0
         for i in range(m):
-            for j in range(i+1,m):
-                dist = dist + wmg[test_ranking[j],test_ranking[i]]
+            for j in range(i + 1, m):
+                dist = dist + wmg[test_ranking[j], test_ranking[i]]
             if dist > best_d:
                 break
         if dist < best_d:
             best = test_ranking
             best_d = dist
     return best, best_d
 
+
 def gini_coef(x):
     # Mean absolute difference
     mad = np.abs(np.subtract.outer(x, x)).mean()
     return (mad / x.mean() / 2)
 
+
 def geom_mean(x):
     x = np.log(x)
     return np.exp(x.mean())
 
+
 def swap_distance_between_potes(pote_1: list, pote_2: list) -> int:
     """ Return: Swap distance between two potes """
     swap_distance = 0
     for i, j in itertools.combinations(pote_1, 2):
         if (pote_1[i] > pote_1[j] and
             pote_2[i] < pote_2[j]) or \
                 (pote_1[i] < pote_1[j] and
                  pote_2[i] > pote_2[j]):
             swap_distance += 1
     return swap_distance
 
+
 def remove_diag(mtrx):
     """ Return: Input matrix with diagonal removed (shape[1] - 1) """
     res = np.zeros((mtrx.shape[0], mtrx.shape[1] - 1))
     for i in range(mtrx.shape[0]):
         for j in range(mtrx.shape[0]):
             if j < i:
-                res[i,j] = mtrx[i,j]
+                res[i, j] = mtrx[i, j]
             elif j > i:
-                res[i,j-1] = mtrx[i,j]
+                res[i, j - 1] = mtrx[i, j]
     return res
 
+
 def calculate_borda_scores(election):
     m = election.num_candidates
     borda = np.zeros(m, int)
     for v in election.votes:
         for i, c in enumerate(v):
             borda[c] = borda[c] + m - i - 1
     return borda
 
+
 def calculate_cand_dom_dist(election):
     distances = election.votes_to_pairwise_matrix()
     distances = np.abs(distances - 0.5)
     np.fill_diagonal(distances, 0)
     return distances
 
+
 def calculate_cand_pos_dist(election):
     election.compute_potes()
     distances = np.zeros([election.num_candidates, election.num_candidates])
     for c1 in range(election.num_candidates):
         for c2 in range(election.num_candidates):
             dist = 0
             for pote in election.potes:
                 dist += abs(pote[c1] - pote[c2])
             distances[c1][c2] = dist
     return distances
 
+
 def calculate_vote_swap_dist(election):
     election.compute_potes()
     distances = np.zeros([election.num_voters, election.num_voters])
     for v1 in range(election.num_voters):
         for v2 in range(election.num_voters):
             distances[v1][v2] = swap_distance_between_potes(
                 election.potes[v1], election.potes[v2])
     return distances
 
+
 # DIVERSITY INDICES
 
 def borda_gini(election):
     if election.fake:
-        return 'None'
+        return None
     all_scores = calculate_borda_scores(election)
     return gini_coef(all_scores)
 
+
 def borda_meandev(election):
     if election.fake:
-        return 'None'
+        return None
     all_scores = calculate_borda_scores(election)
     all_scores = np.abs(all_scores - all_scores.mean())
     return all_scores.mean()
 
+
 def borda_std(election):
     if election.fake:
-        return 'None'
+        return None
     all_scores = calculate_borda_scores(election)
     return all_scores.std()
 
+
 # FROM other.py
 # def borda_std(election):
 #     all_scores = np.zeros(election.num_candidates)
 #     vectors = election.votes_to_positionwise_matrix()
 #     for i in range(election.num_candidates):
 #         for j in range(election.num_candidates):
 #             all_scores[i] += vectors[i][j] * (election.num_candidates - j - 1)
 #     return np.std(all_scores)
 
 def borda_range(election):
     if election.fake:
-        return 'None'
+        return None
     all_scores = calculate_borda_scores(election)
     return (np.max(all_scores) - np.min(all_scores))
 
+
 def cand_dom_dist_mean(election):
     if election.fake:
-        return 'None'
+        return None
     distances = calculate_cand_dom_dist(election)
     return distances.sum() / (election.num_candidates - 1) / election.num_candidates * 2
 
+
 def agreement_index(election):
     if election.fake:
-        return 'None'
+        return None
     distances = calculate_cand_dom_dist(election)
     return distances.sum() / (election.num_candidates - 1) / election.num_candidates * 2
 
+
 def cand_dom_dist_std(election):
     if election.fake:
-        return 'None'
+        return None
     distances = calculate_cand_dom_dist(election)
     distances = remove_diag(distances)
     return distances.std()
 
-# def cand_pos_dist_mean(election):
-#     if election.fake:
-#         return 'None'
-#     distances = np.zeros([election.num_candidates, election.num_candidates])
-#     for c1 in range(election.num_candidates):
-#         for c2 in range(election.num_candidates):
-#             dist = 0
-#             for pote in election.potes:
-#                 dist += abs(pote[c1] - pote[c2])
-#             distances[c1][c2] = dist
-#     print(election.culture_id)
-#     print(distances)
-#     return distances.sum() / (election.num_candidates - 1) / election.num_candidates
-# NO SENSE – ALWAYS CONSTANT
 
 def cand_pos_dist_std(election):
     if election.fake:
-        return 'None'
+        return None
     distances = calculate_cand_pos_dist(election)
     distances = remove_diag(distances)
     return distances.std()
 
+
 def cand_pos_dist_meandev(election):
     if election.fake:
-        return 'None'
+        return None
     distances = calculate_cand_pos_dist(election)
     distances = remove_diag(distances)
     distances = np.abs(distances - distances.mean())
     return distances.mean()
 
+
 def cand_pos_dist_gini(election):
     if election.fake:
-        return 'None'
+        return None
     distances = calculate_cand_pos_dist(election)
     distances = remove_diag(distances)
     return gini_coef(distances)
 
+
 def med_cands_summed(election):
     if election.fake:
-        return 'None'
+        return None
     m = election.num_candidates
     distances = calculate_cand_pos_dist(election)
     res = [0] * m
-    for i in range(1,m):
+    for i in range(1, m):
         best_d = np.inf
-        for comb in itertools.combinations(range(m),i):
+        for comb in itertools.combinations(range(m), i):
             d_total = 0
             for c1 in range(m):
                 min_d = np.inf
                 for c2 in comb:
-                    d_cand = distances[c1,c2]
+                    d_cand = distances[c1, c2]
                     if d_cand < min_d:
                         min_d = d_cand
                 d_total = d_total + min_d
             if d_total < best_d:
                 best_d = d_total
         res[i] = best_d
     return sum(res)
 
+
 def vote_dist_mean(election):
     if election.fake:
-        return 'None'
+        return None
     distances = calculate_vote_swap_dist(election)
     return distances.sum() / election.num_voters / (election.num_voters - 1)
 
+
 def vote_dist_max(election):
     if election.fake:
-        return 'None'
+        return None
     distances = calculate_vote_swap_dist(election)
     return distances.max()
 
+
 def vote_dist_med(election):
     if election.fake:
-        return 'None'
+        return None
     distances = calculate_vote_swap_dist(election)
     distances = remove_diag(distances)
     return np.median(distances)
 
+
 def vote_dist_gini(election):
     if election.fake:
-        return 'None'
+        return None
     distances = calculate_vote_swap_dist(election)
     distances = remove_diag(distances)
     return gini_coef(distances)
 
+
 def vote_sqr_dist_mean(election):
     if election.fake:
-        return 'None'
+        return None
     distances = calculate_vote_swap_dist(election)
     distances = remove_diag(distances)
     distances = np.sqrt(distances)
     return distances.mean()
 
+
 def vote_sqr_dist_med(election):
     if election.fake:
-        return 'None'
+        return None
     distances = calculate_vote_swap_dist(election)
     distances = remove_diag(distances)
     distances = np.sqrt(distances)
     return np.median(distances)
 
+
 def vote_diversity_Karpov(election):
     if election.fake:
-        return 'None'
+        return None
     distances = calculate_vote_swap_dist(election)
     distances = remove_diag(distances)
     distances = distances + 0.5
     distances[distances == 0.5] = 1
     return geom_mean(distances)
 
+
 def dist_sqr_to_Kemeny_mean(election):
     if election.fake:
-        return 'None'
-    return 'None'
+        return None
+    return None
+
 
 def dist_to_Kemeny_mean(election):
     if election.fake:
-        return 'None'
+        return None
     _, dist = kemeny_ranking(election)
     return dist / election.num_voters
 
+
 def dist_to_Kemeny_med(election):
     if election.fake:
-        return 'None'
-    return 'None'
+        return None
+    return None
+
 
 def dist_to_Borda_mean(election):
     if election.fake:
-        return 'None'
+        return None
     m = election.num_candidates
     borda = calculate_borda_scores(election)
     ranking = np.argsort(-borda)
     wmg = election.votes_to_pairwise_matrix()
     dist = 0
     for i in range(m):
         for j in range(i + 1, m):
             dist = dist + wmg[ranking[j], ranking[i]]
     return dist / election.num_voters
 
+
 def lexi_diversity(election):
     if election.fake:
-        return 'None'
-    return 'None'
+        return None
+    return None
+
 
 def greedy_kKemenys_summed(election):
     if election.fake:
-        return 'None'
+        return None
     res = [0] * election.num_voters
     distances = calculate_vote_swap_dist(election)
     best = np.argmin(distances.sum(axis=1))
     best_vec = distances[best]
     res[0] = best_vec.sum()
-    distances = np.vstack((distances[:best], distances[best+1:]))
+    distances = np.vstack((distances[:best], distances[best + 1:]))
 
-    for i in range(1,election.num_voters):
+    for i in range(1, election.num_voters):
         relatives = distances - best_vec
-        relatives = relatives*(relatives < 0)
+        relatives = relatives * (relatives < 0)
         best = np.argmin(relatives.sum(axis=1))
         best_vec = best_vec + relatives[best]
         res[i] = best_vec.sum()
-        distances = np.vstack((distances[:best], distances[best+1:]))
+        distances = np.vstack((distances[:best], distances[best + 1:]))
 
     return sum(res)
     max_dist = (election.num_candidates) * (election.num_candidates - 1) / 2
     return sum(res) / election.num_voters / max_dist
 
+
 def restore_order(x):
     for i in range(len(x)):
         for j in range(len(x) - i, len(x)):
             if x[j] >= x[-i - 1]:
                 x[j] += 1
     return x
+
+
 def distances_to_rankings(rankings, distances):
     dists = distances[rankings]
     return np.sum(dists.min(axis=0))
 
+
 def find_improvement(distances, d, starting, rest, n, k, l):
     for cut in itertools.combinations(range(k), l):
         # print(cut)
         for paste in itertools.combinations(rest, l):
             ranks = []
             j = 0
             for i in range(k):
@@ -334,38 +352,40 @@
             if len(set(ranks)) == len(ranks):
                 # check if better
                 d_new = distances_to_rankings(ranks, distances)
                 if d > d_new:
                     return ranks, d_new, True
     return starting, d, False
 
+
 def local_search_kKemeny_single_k(election, k, l, starting=None):
     if starting is None:
         starting = list(range(k))
     distances = calculate_vote_swap_dist(election)
 
     n = election.num_voters
 
     d = distances_to_rankings(starting, distances)
     iter = 0
     check = True
-    while(check):
+    while (check):
         # print(iter)
         # print(starting)
         # print(d)
         # print()
         iter = iter + 1
         rest = [i for i in range(n) if i not in starting]
         for j in range(l):
-            starting, d, check = find_improvement(distances, d, starting, rest, n, k, j+1)
+            starting, d, check = find_improvement(distances, d, starting, rest, n, k, j + 1)
             if check:
                 break
         # print()
     return d
 
+
 def local_search_kKemeny(election, l, starting=None):
     max_dist = election.num_candidates * (election.num_candidates - 1) / 2
     res = []
     for k in range(1, election.num_voters):
         # print(k)
         if starting is None:
             d = local_search_kKemeny_single_k(election, k, l)
@@ -377,120 +397,125 @@
         else:
             break
     for k in range(len(res), election.num_voters):
         res.append(0)
 
     return res
 
+
 def diversity_index(election):
     if election.fake:
-        return 'None'
+        return None
     max_dist = election.num_candidates * (election.num_candidates - 1) / 2
     res = [0] * election.num_voters
     chosen_votes = []
     distances = calculate_vote_swap_dist(election)
     best = np.argmin(distances.sum(axis=1))
     chosen_votes.append(best)
     best_vec = distances[best]
     res[0] = best_vec.sum() / max_dist / election.num_voters
-    distances = np.vstack((distances[:best],distances[best+1:]))
+    distances = np.vstack((distances[:best], distances[best + 1:]))
 
-    for i in range(1,election.num_voters):
+    for i in range(1, election.num_voters):
         relatives = distances - best_vec
-        relatives = relatives*(relatives < 0)
+        relatives = relatives * (relatives < 0)
         best = np.argmin(relatives.sum(axis=1))
         chosen_votes.append(best)
         best_vec = best_vec + relatives[best]
         res[i] = best_vec.sum() / max_dist / election.num_voters
-        distances = np.vstack((distances[:best], distances[best+1:]))
+        distances = np.vstack((distances[:best], distances[best + 1:]))
 
     chosen_votes = restore_order(chosen_votes)
 
     res_1 = local_search_kKemeny(election, 1, chosen_votes)
     res_2 = local_search_kKemeny(election, 1)
     res = [min(d_1, d_2) for d_1, d_2 in zip(res_1, res_2)]
 
-    return sum([x / (i+1) for i, x in enumerate(res)])
+    return sum([x / (i + 1) for i, x in enumerate(res)])
+
 
 def greedy_kKemenys_divk_summed(election):
     if election.fake:
-        return 'None'
+        return None
     res = [0] * election.num_voters
     distances = calculate_vote_swap_dist(election)
     best = np.argmin(distances.sum(axis=1))
     best_vec = distances[best]
     res[0] = best_vec.sum()
-    distances = np.vstack((distances[:best], distances[best+1:]))
+    distances = np.vstack((distances[:best], distances[best + 1:]))
 
     for i in range(1, election.num_voters):
         relatives = distances - best_vec
-        relatives = relatives*(relatives < 0)
+        relatives = relatives * (relatives < 0)
         best = np.argmin(relatives.sum(axis=1))
         best_vec = best_vec + relatives[best]
         res[i] = best_vec.sum() / (i + 1)
-        distances = np.vstack((distances[:best], distances[best+1:]))
+        distances = np.vstack((distances[:best], distances[best + 1:]))
 
     # res[0] = 0 # for disregarding one Kemeny (AN = ID)
     max_dist = (election.num_candidates) * (election.num_candidates - 1) / 2
     return sum(res) / election.num_voters / max_dist
 
+
 def greedy_2kKemenys_summed(election):
     if election.fake:
-        return 'None'
+        return None
     res = []
     distances = calculate_vote_swap_dist(election)
     best = np.argmin(distances.sum(axis=1))
     best_vec = distances[best]
     res.append(best_vec.sum())
-    distances = np.vstack((distances[:best], distances[best+1:]))
+    distances = np.vstack((distances[:best], distances[best + 1:]))
 
     k = 2
     for i in range(1, election.num_voters):
         relatives = distances - best_vec
-        relatives = relatives*(relatives < 0)
+        relatives = relatives * (relatives < 0)
         best = np.argmin(relatives.sum(axis=1))
         best_vec = best_vec + relatives[best]
         if (i + 1) == k:
             res.append(best_vec.sum())
             k = k * 2
-        distances = np.vstack((distances[:best], distances[best+1:]))
+        distances = np.vstack((distances[:best], distances[best + 1:]))
 
     # res[0] = 0 # for disregarding one Kemeny (AN = ID)
     max_dist = (election.num_candidates) * (election.num_candidates - 1) / 2
     return sum(res) / election.num_voters / max_dist / 2
 
+
 def polarization_1by2Kemenys(election):
     if election.fake:
-        return 'None'
+        return None
     distances = calculate_vote_swap_dist(election)
     best = np.argmin(distances.sum(axis=1))
     best_vec = distances[best]
     first_kemeny = best_vec.sum()
-    distances = np.vstack((distances[:best],distances[best+1:]))
+    distances = np.vstack((distances[:best], distances[best + 1:]))
 
     relatives = distances - best_vec
-    relatives = relatives*(relatives < 0)
+    relatives = relatives * (relatives < 0)
     best = np.argmin(relatives.sum(axis=1))
     best_vec = best_vec + relatives[best]
     second_kemeny = best_vec.sum()
 
     max_dist = (election.num_candidates) * (election.num_candidates - 1) / 2
     return (first_kemeny - second_kemeny) / election.num_voters / max_dist
 
+
 def polarization_index(election):
     if election.fake:
-        return 'None'
+        return None
     distances = calculate_vote_swap_dist(election)
     best_1 = np.argmin(distances.sum(axis=1))
     best_vec = distances[best_1]
     first_kemeny = best_vec.sum()
-    distances = np.vstack((distances[:best_1], distances[best_1+1:]))
+    distances = np.vstack((distances[:best_1], distances[best_1 + 1:]))
 
     relatives = distances - best_vec
-    relatives = relatives*(relatives < 0)
+    relatives = relatives * (relatives < 0)
     best_2 = np.argmin(relatives.sum(axis=1))
 
     if best_1 <= best_2:
         best_2 = best_2 + 1
 
     chosen = [best_1, best_2]
     chosen.sort()
@@ -498,182 +523,162 @@
     second_kemeny_1 = local_search_kKemeny_single_k(election, 2, 1, starting=chosen)
     second_kemeny_2 = local_search_kKemeny_single_k(election, 2, 1)
     second_kemeny = min(second_kemeny_1, second_kemeny_2)
 
     max_dist = (election.num_candidates) * (election.num_candidates - 1) / 2
     return 2 * (first_kemeny - second_kemeny) / election.num_voters / max_dist
 
+
 def greedy_kmeans_summed(election):
     if election.fake:
-        return 'None'
+        return None
     res = [0] * election.num_voters
     distances = calculate_vote_swap_dist(election)
     distances = distances * distances
     best = np.argmin(distances.sum(axis=1))
     best_vec = distances[best]
     res[0] = best_vec.sum()
-    distances = np.vstack((distances[:best],distances[best+1:]))
+    distances = np.vstack((distances[:best], distances[best + 1:]))
 
-    for i in range(1,election.num_voters):
+    for i in range(1, election.num_voters):
         relatives = distances - best_vec
-        relatives = relatives*(relatives < 0)
+        relatives = relatives * (relatives < 0)
         best = np.argmin(relatives.sum(axis=1))
         best_vec = best_vec + relatives[best]
         res[i] = best_vec.sum()
-        distances = np.vstack((distances[:best],distances[best+1:]))
+        distances = np.vstack((distances[:best], distances[best + 1:]))
 
     return sum(res)
 
+
 def support_diversity(election, tuple_len):
     if election.fake:
-        return 'None'
+        return None
     m = election.num_candidates
     res = 0
     for subset in itertools.combinations(range(m), tuple_len):
         support = []
         for v in election.votes:
             trimmed_v = []
             for c in v:
                 if c in subset:
                     trimmed_v.append(c)
-            if not(trimmed_v in support):
+            if not (trimmed_v in support):
                 support.append(trimmed_v)
         res = res + len(support)
     return res
 
+
 def support_diversity_normed(election, tuple_len):
     if election.fake:
-        return 'None'
+        return None
     m = election.num_candidates
     res = 0
     count = 0
     for subset in itertools.combinations(range(m), tuple_len):
         count = count + 1
         support = []
         for v in election.votes:
             trimmed_v = []
             for c in v:
                 if c in subset:
                     trimmed_v.append(c)
-            if not(trimmed_v in support):
+            if not (trimmed_v in support):
                 support.append(trimmed_v)
         res = res + len(support)
     return res / count
 
+
 def support_diversity_normed2(election, tuple_len):
     if election.fake:
-        return 'None'
+        return None
     m = election.num_candidates
     res = 0
     count = 0
     for subset in itertools.combinations(range(m), tuple_len):
         count = count + 1
         support = []
         for v in election.votes:
             trimmed_v = []
             for c in v:
                 if c in subset:
                     trimmed_v.append(c)
-            if not(trimmed_v in support):
+            if not (trimmed_v in support):
                 support.append(trimmed_v)
         res = res + len(support)
     return res / count / math.factorial(tuple_len)
 
+
 def support_diversity_normed3(election, tuple_len):
     if election.fake:
-        return 'None'
+        return None
     m = election.num_candidates
     res = 0
     count = 0
     for subset in itertools.combinations(range(m), tuple_len):
         count = count + 1
         support = []
         for v in election.votes:
             trimmed_v = []
             for c in v:
                 if c in subset:
                     trimmed_v.append(c)
-            if not(trimmed_v in support):
+            if not (trimmed_v in support):
                 support.append(trimmed_v)
         res = res + len(support)
-    max_times = min(math.factorial(tuple_len),election.num_voters)
+    max_times = min(math.factorial(tuple_len), election.num_voters)
     return res / count / max_times
 
+
 def support_pairs(election):
-    return support_diversity(election,2)
+    return support_diversity(election, 2)
+
 
 def support_triplets(election):
-    return support_diversity(election,3)
+    return support_diversity(election, 3)
+
 
 def support_votes(election):
     if election.fake:
-        return 'None'
+        return None
     m = election.num_candidates
-    return support_diversity(election,m)
+    return support_diversity(election, m)
+
 
 def support_diversity_summed(election):
     if election.fake:
-        return 'None'
+        return None
     m = election.num_candidates
     res = 0
-    for i in range(2,m+1):
+    for i in range(2, m + 1):
         res = res + support_diversity(election, i)
     return res
 
+
 def support_diversity_normed_summed(election):
     if election.fake:
-        return 'None'
+        return None
     m = election.num_candidates
     res = 0
-    for i in range(2,m+1):
+    for i in range(2, m + 1):
         res = res + support_diversity_normed(election, i)
     return res
 
+
 def support_diversity_normed2_summed(election):
     if election.fake:
-        return 'None'
+        return None
     m = election.num_candidates
     res = 0
-    for i in range(2,m+1):
+    for i in range(2, m + 1):
         res = res + support_diversity_normed2(election, i)
     return res
 
+
 def support_diversity_normed3_summed(election):
     if election.fake:
-        return 'None'
+        return None
     m = election.num_candidates
     res = 0
-    for i in range(2,m+1):
+    for i in range(2, m + 1):
         res = res + support_diversity_normed3(election, i)
     return res
-
-# FROM vc_diversity.py
-# def num_of_diff_votes(election):
-#     if election.fake:
-#         return 'None'
-#     str_votes = [str(vote) for vote in election.votes]
-#     return len(set(str_votes))
-#
-#
-# def voterlikeness_sqrt(election):
-#     if election.fake:
-#         return 'None'
-#     vectors = election.votes_to_voterlikeness_vectors()
-#     score = 0.
-#     for vector in vectors:
-#         for value in vector:
-#             score += value**0.5
-#     return score
-#
-#
-# def voterlikeness_harmonic(election):
-#     if election.fake:
-#         return 'None'
-#     vectors = election.votes_to_voterlikeness_vectors()
-#     score = 0.
-#     for vector in vectors:
-#         vector = sorted(vector)
-#         for pos, value in enumerate(vector):
-#             score += 1/(pos+2)*value
-#     return score
-#
-#
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `mapel-elections-2.0.5/src/mapel/elections/features/justified_representation.py` & `mapel-elections-2.0.6/src/mapel/elections/features/justified_representation.py`

 * *Files identical despite different names*

### Comparing `mapel-elections-2.0.5/src/mapel/elections/features/other.py` & `mapel-elections-2.0.6/src/mapel/elections/features/other.py`

 * *Files identical despite different names*

### Comparing `mapel-elections-2.0.5/src/mapel/elections/features/partylist.py` & `mapel-elections-2.0.6/src/mapel/elections/features/partylist.py`

 * *Files identical despite different names*

### Comparing `mapel-elections-2.0.5/src/mapel/elections/features/power_index.py` & `mapel-elections-2.0.6/src/mapel/elections/features/power_index.py`

 * *Files identical despite different names*

### Comparing `mapel-elections-2.0.5/src/mapel/elections/features/proportionality_degree.py` & `mapel-elections-2.0.6/src/mapel/elections/features/proportionality_degree.py`

 * *Files identical despite different names*

### Comparing `mapel-elections-2.0.5/src/mapel/elections/features/ranging_cc.py` & `mapel-elections-2.0.6/src/mapel/elections/features/ranging_cc.py`

 * *Files 14% similar despite different names*

```diff
@@ -3,27 +3,27 @@
 import numpy as np
 
 from mapel.elections.features.scores import get_cc_score, get_cc_dissat
 
 
 def get_ranging_cc_score(election, committee_size=1):
     if election.fake:
-        return 'None', 'None'
+        return {'value': None, 'dissat': None}
 
     x = election.num_candidates * scipy.special.lambertw(committee_size).real / committee_size
 
     best_score = 0
     best_dissat = 0
     for threshold in range(1, int(x)):
         score, dissat = get_algorithm_p_committee(election, committee_size, x)
         if score > best_score:
             best_score = score
             best_dissat = dissat
 
-    return best_score, best_dissat
+    return {'value': best_score, 'dissat': best_dissat}
 
 
 def get_algorithm_p_committee(election, committee_size, x):
 
     winners = set()
 
     active = [True for _ in range(election.num_voters)]
```

### Comparing `mapel-elections-2.0.5/src/mapel/elections/features/scores.py` & `mapel-elections-2.0.6/src/mapel/elections/features/scores.py`

 * *Files 10% similar despite different names*

```diff
@@ -22,33 +22,37 @@
 
 from mapel.core.glossary import *
 from mapel.elections.distances import lp
 from mapel.elections.other import winners as win
 
 
 # MAIN FUNCTIONS
-def highest_borda_score(election) -> int:
+def highest_borda_score(election):
     """ Compute highest BORDA score of a given election """
+    if election.culture_id in LIST_OF_FAKE_MODELS:
+        return {'value': None}
     c = election.num_candidates
     vectors = election.get_vectors()
     borda = [sum([vectors[i][pos] * (c - pos - 1) for pos in range(c)])
              for i in range(c)]
     return max(borda) * election.num_voters
 
 
-def highest_plurality_score(election) -> int:
+def highest_plurality_score(election):
     """ compute highest PLURALITY score of a given election"""
+    if election.culture_id in LIST_OF_FAKE_MODELS:
+        return {'value': None}
     first_pos = election.get_matrix()[0]
     return max(first_pos) * election.num_voters
 
 
-def highest_copeland_score(election) -> Union[int, str]:
+def highest_copeland_score(election):
     """ compute highest COPELAND score of a given election """
     if election.culture_id in LIST_OF_FAKE_MODELS:
-        return 'None'
+        return {'value': None}
 
     election.compute_potes()
     scores = np.zeros([election.num_candidates])
 
     for i in range(election.num_candidates):
         for j in range(i + 1, election.num_candidates):
             result = 0
@@ -65,15 +69,15 @@
 
     return max(scores)
 
 
 def lowest_dodgson_score(election):
     """ compute lowest DODGSON score of a given election """
     if election.culture_id in LIST_OF_FAKE_MODELS:
-        return 'None'
+        return {'value': None}
 
     min_score = math.inf
 
     for target_id in range(election.num_candidates):
 
         # PREPARE N
         unique_potes, N = _potes_to_unique_potes(election.get_potes())
@@ -118,40 +122,40 @@
             min_score = score
 
     return min_score
 
 
 def highest_cc_score(election, committee_size=1):
     if election.culture_id in LIST_OF_FAKE_MODELS:
-        return 'None', 'None'
+        return {'value': None, 'dissat': None}
     winners, total_time = win.generate_winners(election=election,
                                              num_winners=committee_size,
                                              ballot="ordinal",
                                              type='borda_owa', name='cc')
-    return get_cc_score(election, winners), get_cc_dissat(election, winners)
+    return {'value': get_cc_score(election, winners), 'dissat': get_cc_dissat(election, winners)}
 
 
 def highest_hb_score(election, committee_size=1):
     if election.culture_id in LIST_OF_FAKE_MODELS:
-        return 'None', 'None'
+        return {'value': None, 'dissat': None}
     winners, total_time = win.generate_winners(election=election,
                                              num_winners=committee_size,
                                              ballot="ordinal",
                                              type='borda_owa', name='hb')
-    return get_hb_score(election, winners), get_hb_dissat(election, winners)
+    return {'value': get_hb_score(election, winners), 'dissat': get_hb_dissat(election, winners)}
 
 
 def highest_pav_score(election, committee_size=1):
     if election.culture_id in LIST_OF_FAKE_MODELS:
-        return 'None', 'None'
+        return {'value': None, 'dissat': None}
     winners, total_time = win.generate_winners(election=election,
                                              num_winners=committee_size,
                                              ballot="ordinal",
                                              type='bloc_owa', name='hb')
-    return get_pav_score(election, winners), get_pav_dissat(election, winners)
+    return {'value': get_pav_score(election, winners), 'dissat': get_pav_dissat(election, winners)}
 
 
 # HELPER FUNCTIONS
 def _potes_to_unique_potes(potes):
     """ Remove repetitions from potes (positional votes) """
     unique_potes = []
     n = []
```

### Comparing `mapel-elections-2.0.5/src/mapel/elections/features/vc_diversity.py` & `mapel-elections-2.0.6/src/mapel/elections/features/vc_diversity.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,40 +1,42 @@
-from mapel.core.glossary import LIST_OF_FAKE_MODELS
 import numpy as np
 
 
 def num_of_diff_votes(election):
     if election.fake:
-        return 'None'
+        return None
+
     str_votes = [str(vote) for vote in election.votes]
     return len(set(str_votes))
 
 
 def voterlikeness_sqrt(election):
     if election.fake:
-        return 'None'
+        return None
+
     vectors = election.votes_to_voterlikeness_vectors()
     score = 0.
     for vector in vectors:
         for value in vector:
             score += value**0.5
     return score
 
 
 def voterlikeness_harmonic(election):
     if election.fake:
-        return 'None'
+        return None
+
     vectors = election.votes_to_voterlikeness_vectors()
     score = 0.
     for vector in vectors:
         vector = sorted(vector)
         for pos, value in enumerate(vector):
             score += 1/(pos+2)*value
     return score
 
 
 def borda_diversity(election):
-    if election.culture_id in LIST_OF_FAKE_MODELS:
-        return 'None'
+    if election.fake:
+        return None
 
     vector = np.array(election.votes_to_bordawise_vector())
     return np.std(vector)
```

### Comparing `mapel-elections-2.0.5/src/mapel/elections/features_.py` & `mapel-elections-2.0.6/src/mapel/elections/features_.py`

 * *Files 2% similar despite different names*

```diff
@@ -98,14 +98,15 @@
     'pav_time': partylist.pav_time,  # unsupported feature
     'justified_ratio': other.justified_ratio,  # unsupported feature
     'rand_approx_pav_score': approx.get_rand_approx_pav_score,  # unsupported feature
     'min_dim': dimensionality.min_dim,  # unsupported feature
 }
 
 
+
 def get_global_feature(feature_id):
     """ Global feature depends on all instances """
     if feature_id in MAIN_GLOBAL_FEATUERS:
         return get_main_global_feature(feature_id)
 
     return {'clustering': clustering.clustering_v1,
             'clustering_kmeans': clustering.clustering_kmeans,
@@ -132,9 +133,9 @@
     registered_approval_features[name] = function
 
 
 def add_ordinal_feature(name, function):
     registered_ordinal_features[name] = function
 
 # # # # # # # # # # # # # # # #
-# LAST CLEANUP ON: 10.05.2022 #
+# LAST CLEANUP ON: 11.07.2023 #
 # # # # # # # # # # # # # # # #
```

### Comparing `mapel-elections-2.0.5/src/mapel/elections/objects/ApprovalElection.py` & `mapel-elections-2.0.6/src/mapel/elections/objects/ApprovalElection.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,166 +1,82 @@
 #!/usr/bin/env python
+from abc import ABC
 
 from matplotlib import pyplot as plt
 from mapel.elections.cultures_ import generate_approval_votes
 from mapel.elections.objects.Election import Election
 from mapel.core.inner_distances import hamming
 from mapel.core.utils import *
 import mapel.elections.persistence.election_imports as imports
 import mapel.elections.persistence.election_exports as exports
 from mapel.elections.cultures.params import *
 
 
-class ApprovalElection(Election):
+class ApprovalElection(Election, ABC):
 
     def __init__(self,
-                 experiment_id,
-                 election_id,
+                 experiment_id=None,
+                 election_id=None,
                  culture_id=None,
                  num_candidates=None,
-                 is_imported: bool = False,
-                 is_shifted: bool = False,
                  params=None,
                  variable=None,
                  **kwargs):
 
-        super().__init__(experiment_id,
-                         election_id,
+        super().__init__(experiment_id=experiment_id,
+                         election_id=election_id,
                          culture_id=culture_id,
                          num_candidates=num_candidates,
                          **kwargs)
 
         self.params = params
         self.variable = variable
 
         self.approvalwise_vector = []
-        self.coapproval_frequency_vectors = []
-        self.voterlikeness_vectors = []
-        self.pairwise_matrix = []
-        self.candidatelikeness_original_vectors = []
-        self.candidatelikeness_sorted_vectors = []
-        self.hamming_candidates = []
         self.reverse_approvals = []
 
-        if is_imported and experiment_id != 'virtual':
+        self.import_approval_election()
+
+    def import_approval_election(self):
+        if self.is_imported and self.experiment_id is not None:
             try:
-                fake = imports.check_if_fake(experiment_id, election_id, 'app')
+                fake = imports.check_if_fake(self.experiment_id, self.election_id, 'app')
                 if fake:
                     self.culture_id, self.params, self.num_voters, self.num_candidates = \
-                        imports.import_fake_app_election(experiment_id, election_id)
+                        imports.import_fake_app_election(self.experiment_id, self.election_id)
                 else:
                     self.votes, self.num_voters, self.num_candidates, self.params, \
-                    self.culture_id = imports.import_real_app_election(experiment_id,
-                                                                       election_id,
-                                                                       is_shifted)
+                    self.culture_id = imports.import_real_app_election(self.experiment_id,
+                                                                       self.election_id,
+                                                                       self.is_shifted)
             except:
                 pass
 
         if self.params is None:
             self.params = {}
 
-        if culture_id is not None:
+        if self.culture_id is not None:
             self.params, self.printing_params = update_params_approval(self.params,
-                                                                                   self.printing_params,
-                                                                                   self.variable,
-                                                                                   self.culture_id,
-                                                                                   self.num_candidates)
+                                                                       self.printing_params,
+                                                                       self.variable,
+                                                                       self.culture_id,
+                                                                       self.num_candidates)
 
     def votes_to_approvalwise_vector(self) -> None:
         """ Convert votes to approvalwise vectors """
-        approvalwise_vector = np.zeros([self.num_candidates])
-        for vote in self.votes:
-            for c in vote:
-                approvalwise_vector[c] += 1
+        vote_indices = np.concatenate(self.votes)
+        approvalwise_vector = np.bincount(vote_indices, minlength=self.num_candidates)
         approvalwise_vector = approvalwise_vector / self.num_voters
         self.approvalwise_vector = np.sort(approvalwise_vector)
 
-    def votes_to_coapproval_frequency_vectors(self, vector_type='A') -> None:
-        """ Convert votes to frequency vectors """
-        vectors = np.zeros([self.num_candidates, self.num_candidates * 2])
-        for vote in self.votes:
-            size = len(vote)
-            for c in range(self.num_candidates):
-                if c in vote:
-                    if vector_type in ['A', 'B']:
-                        vectors[c][size - 1] += 1
-                    elif vector_type == 'C':
-                        vectors[c][2 * size - 1] += 1
-                    elif vector_type in ['D', 'E']:
-                        vectors[c][self.num_candidates + size - 1] += 1
-                else:
-                    if vector_type == 'A':
-                        vectors[c][self.num_candidates + size] += 1
-                    elif vector_type == 'B':
-                        vectors[c][2 * self.num_candidates - size - 1] += 1
-                    elif vector_type == 'C':
-                        vectors[c][2 * size] += 1
-                    elif vector_type == 'D':
-                        vectors[c][size] += 1
-                    elif vector_type == 'E':
-                        vectors[c][self.num_candidates - size - 1] += 1
-        vectors = vectors / self.num_voters
-        self.coapproval_frequency_vectors = vectors
-
-    def votes_to_pairwise_matrix(self) -> None:
-        """ Convert votes to pairwise matrix """
-        matrix = np.zeros([self.num_candidates, self.num_candidates])
-
-        for c_1 in range(self.num_candidates):
-            for c_2 in range(self.num_candidates):
-                for vote in self.votes:
-                    if (c_1 in vote and c_2 in vote) or (c_1 not in vote and c_2 not in vote):
-                        matrix[c_1][c_2] += 1
-        matrix = matrix / self.num_voters
-        self.pairwise_matrix = matrix
-
-    def votes_to_candidatelikeness_original_vectors(self) -> None:
-        """ Convert votes to ... """
-        matrix = np.zeros([self.num_candidates, self.num_candidates])
-
-        for c_1 in range(self.num_candidates):
-            for c_2 in range(self.num_candidates):
-                for vote in self.votes:
-                    if (c_1 in vote and c_2 not in vote) or (c_1 not in vote and c_2 in vote):
-                        matrix[c_1][c_2] += 1
-        matrix = matrix / self.num_voters
-        self.candidatelikeness_original_vectors = matrix
-
-    def votes_to_candidatelikeness_sorted_vectors(self) -> None:
-        """ Convert votes to ... """
-        self.votes_to_candidatelikeness_original_vectors()
-        self.candidatelikeness_sorted_vectors = np.sort(self.candidatelikeness_original_vectors)
-
-    def votes_to_voterlikeness_vectors(self, vector_type='hamming') -> None:
-        """ Convert votes to ... """
-
-        vectors = np.zeros([self.num_voters, self.num_voters])
-
-        for i in range(self.num_voters):
-            for j in range(self.num_voters):
-                set_a = self.votes[i]
-                set_b = self.votes[j]
-                if vector_type == 'hamming':
-                    vectors[i][j] = hamming(set_a, set_b)
-                elif vector_type == 'to_be_deleted':
-                    vectors[i][j] = len(set_a.intersection(set_b)) - len(set_a)
-            vectors[i] = sorted(vectors[i])
-
-        self.voterlikeness_vectors = vectors
-
     def compute_reverse_approvals(self):
-        reverse_approvals = [set() for _ in range(self.num_candidates)]
-        for i, vote in enumerate(self.votes):
-            for c in vote:
-                reverse_approvals[int(c)].add(i)
-
-        self.reverse_approvals = reverse_approvals
+        self.reverse_approvals = [set(i for i, vote in enumerate(self.votes) if c in vote)
+                                  for c in range(self.num_candidates)]
 
     def prepare_instance(self, is_exported=None, is_aggregated=True):
-
         self.votes = generate_approval_votes(culture_id=self.culture_id,
                                              num_candidates=self.num_candidates,
                                              num_voters=self.num_voters,
                                              params=self.params)
         if is_exported:
             exports.export_approval_election(self, is_aggregated=is_aggregated)
 
@@ -182,15 +98,15 @@
 
         if self.is_exported:
             exports.export_distances(self, object_type='vote')
 
         return distances
 
     def compute_distances_between_candidates(self, distance_id='hamming'):
-        #
+
         distances = np.zeros([self.num_candidates, self.num_candidates])
         for c1 in range(self.num_candidates):
             for c2 in range(self.num_candidates):
                 if distance_id == 'hamming':
                     distances[c1][c2] = hamming(self.reverse_approvals[c1],
                                                 self.reverse_approvals[c2])
                 elif distance_id == 'jaccard':
@@ -201,15 +117,15 @@
                             self.reverse_approvals[c1].intersection(self.reverse_approvals[c2])) \
                                             / len(
                             self.reverse_approvals[c1].union(self.reverse_approvals[c2]))
 
         self.distances['candidate'] = distances
 
         if self.is_exported:
-            self.export_distances(object_type='candidate')
+            exports.export_distances(self, object_type='candidate')
 
     def print_map(self, show=True, radius=None, name=None, alpha=0.1, s=30, circles=False,
                   object_type=None, double_gradient=False, saveas=None, color='blue',
                   marker='o', title_size=20, annotate=False):
 
         if object_type == 'vote':
             length = self.num_voters
@@ -219,15 +135,14 @@
             self.compute_reverse_approvals()
             votes = self.reverse_approvals
 
         if object_type is None:
             object_type = self.object_type
 
         plt.figure(figsize=(6.4, 6.4))
-        # = plt.subplots()
 
         X = []
         Y = []
         for elem in self.coordinates[object_type]:
             X.append(elem[0])
             Y.append(elem[1])
```

### Comparing `mapel-elections-2.0.5/src/mapel/elections/objects/ApprovalElectionExperiment.py` & `mapel-elections-2.0.6/src/mapel/elections/objects/ApprovalElectionExperiment.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 #!/usr/bin/env python
+from abc import ABC
 
 from mapel.core.matchings import solve_matching_vectors
 from mapel.elections.objects.ElectionExperiment import ElectionExperiment
 from mapel.elections.other import pabulib
 from mapel.core.utils import *
 import numpy as np
 import csv
@@ -23,15 +24,15 @@
     TSNE = None
     SpectralEmbedding = None
     LocallyLinearEmbedding = None
     Isomap = None
     print(error)
 
 
-class ApprovalElectionExperiment(ElectionExperiment):
+class ApprovalElectionExperiment(ElectionExperiment, ABC):
     """ Abstract set of approval elections."""
 
     def __init__(self, **kwargs):
         super().__init__(**kwargs)
 
     def add_culture(self, name, function):
         cultures.add_approval_culture(name, function)
@@ -178,41 +179,28 @@
                     if ctr == 0:
                         avg_value = -1
                     else:
                         avg_value = round(total_value / ctr, 2)
                     results[model][rule] = avg_value
             all_results[f'{feature_id}_{column_id}'] = results
 
-        # print("\\toprule")
-        # print("rule", end=" ")
-        # for model in list_of_models:
-        #     # print(f'& {nice_model[model]}', end=" ")
-        #     print(f'& {model}', end=" ")
-        # # print("")
-        # print("\\\\ \\midrule")
-
         for rule in list_of_rules:
             print(rule, end=" ")
             for model in list_of_models:
                 print(f'&', end=" ")
                 for feature_id, column_id in zip(features_id, columns_id):
                     print(f'{all_results[f"{feature_id}_{column_id}"][model][rule]}', end=" \ ")
-            # print("")
             print("\\\\ \\midrule")
 
     def add_folders_to_experiment(self) -> None:
 
-        if not os.path.isdir("experiments/"):
-            os.mkdir(os.path.join(os.getcwd(), "experiments"))
-
-        if not os.path.isdir("images/"):
-            os.mkdir(os.path.join(os.getcwd(), "images"))
-
-        if not os.path.isdir("trash/"):
-            os.mkdir(os.path.join(os.getcwd(), "trash"))
+        dirs = ["experiments", "images", "trash"]
+        for dir in dirs:
+            if not os.path.isdir(dir):
+                os.mkdir(os.path.join(os.getcwd(), dir))
 
         if not os.path.isdir(os.path.join(os.getcwd(), "experiments", self.experiment_id)):
             os.mkdir(os.path.join(os.getcwd(), "experiments", self.experiment_id))
 
         list_of_folders = ['distances',
                            'features',
                            'coordinates',
```

### Comparing `mapel-elections-2.0.5/src/mapel/elections/objects/Election.py` & `mapel-elections-2.0.6/src/mapel/elections/objects/Election.py`

 * *Files 18% similar despite different names*

```diff
@@ -25,56 +25,63 @@
 
 OBJECT_TYPES = ['vote', 'candidate']
 
 
 class Election(Instance):
 
     def __init__(self,
-                 experiment_id,
-                 election_id,
+                 experiment_id=None,
+                 election_id=None,
                  culture_id=None,
                  votes=None,
                  ballot_type: str = 'ordinal',
                  num_voters: int = None,
                  num_candidates: int = None,
                  label=None,
                  fast_import=False,
                  is_shifted=False,
+                 is_imported=False,
                  **kwargs):
 
-        super().__init__(experiment_id,
-                         election_id,
+        super().__init__(experiment_id=experiment_id,
+                         instance_id=election_id,
                          culture_id=culture_id,
                          **kwargs)
 
         self.election_id = election_id
         self.ballot_type = ballot_type
         self.label = label
         self.num_voters = num_voters
         self.num_candidates = num_candidates
         self.votes = votes
-
         self.is_exported = True
         self.winners = None
         self.alternative_winners = {}
         self.fake = culture_id in LIST_OF_FAKE_MODELS
         self.potes = None
         self.features = {}
         self.object_type = 'vote'
         self.points = {}
         self.is_shifted = is_shifted
+        self.is_imported = is_imported
+        self.fast_import = fast_import
+
+        self.import_distances()
+        self.import_coordinates()
 
+    def import_distances(self):
         self.distances = {}
-        if not fast_import:
+        if not self.fast_import:
             for object_type in OBJECT_TYPES:
                 try:
                     self.distances[object_type] = imports.import_distances(self, object_type)
                 except:
                     pass
 
+    def import_coordinates(self):
         self.coordinates = {}
         for object_type in OBJECT_TYPES:
             try:
                 self.coordinates[object_type] = imports.import_coordinates(self, object_type)
             except:
                 pass
 
@@ -184,141 +191,43 @@
         file_name = os.path.join(os.getcwd(), "images", name, f'{saveas}.png')
         plt.savefig(file_name, bbox_inches='tight', dpi=100)
         if show:
             plt.show()
         else:
             plt.clf()
 
-    #DIV-MERGE # TO DELETE?
-    def print_map_verfity(self, show=True, radius=None, name=None, alpha=0.1, s=30, circles=False,
-                  object_type=None, double_gradient=False, saveas=None):
-
-        if object_type is None:
-            object_type = self.object_type
-
-        plt.figure(figsize=(6.4, 6.4))
-
-        X = []
-        Y = []
-        for elem in self.coordinates[object_type]:
-            X.append(elem[0])
-            Y.append(elem[1])
-
-        if circles:
-            weighted_points = {}
-            Xs = {}
-            Ys = {}
-            for i in range(self.num_voters):
-                str_elem = str(self.votes[i])
-                if str_elem in weighted_points:
-                    weighted_points[str_elem] += 1
-                else:
-                    weighted_points[str_elem] = 1
-                    Xs[str_elem] = X[i]
-                    Ys[str_elem] = Y[i]
-
-            for str_elem in weighted_points:
-                if weighted_points[str_elem] > 10:
-                    plt.scatter(Xs[str_elem], Ys[str_elem],
-                                color='purple',
-                                s=10 * weighted_points[str_elem],
-                                alpha=0.2)
-
-        if double_gradient:
-            for i in range(self.num_voters):
-                x = float(self.points['voters'][i][0])
-                y = float(self.points['voters'][i][1])
-                plt.scatter(X[i], Y[i], color=[0,y,x], s=s, alpha=alpha)
-        else:
-            plt.scatter(X, Y, color='blue', s=s, alpha=alpha)
-
-        if radius:
-            plt.xlim([-radius, radius])
-            plt.ylim([-radius, radius])
-        plt.title(self.label, size=38)
-        plt.axis('off')
-
-        if saveas is None:
-            saveas = f'{self.label}_euc'
-
-        file_name = os.path.join(os.getcwd(), "images", name, f'{saveas}.png')
-        plt.savefig(file_name, bbox_inches='tight', dpi=100)
-        if show:
-            plt.show()
-        else:
-            plt.clf()
-
-    # def online_mini_map(self):
-    #
-    #     self.compute_potes()
-    #
-    #     distances = np.zeros([len(self.potes), len(self.potes)])
-    #     for v1 in range(len(self.potes)):
-    #         for v2 in range(len(self.potes)):
-    #             swap_distance = 0
-    #             for i, j in itertools.combinations(self.potes[0], 2):
-    #                 if (self.potes[v1][i] > self.potes[v1][j] and
-    #                     self.potes[v2][i] < self.potes[v2][j]) or \
-    #                         (self.potes[v1][i] < self.potes[v1][j] and
-    #                          self.potes[v2][i] > self.potes[v2][j]):
-    #                     swap_distance += 1
-    #             distances[v1][v2] = swap_distance
-    #
-    #     # my_pos = KamadaKawai().embed(
-    #     #     distances=distances,
-    #     # )
-    #     my_pos = MDS(n_components=2, dissimilarity='precomputed').fit_transform(distances)
-    #     X = []
-    #     Y = []
-    #     for elem in my_pos:
-    #         X.append(elem[0])
-    #         Y.append(elem[1])
-    #     plt.scatter(X, Y, color='blue', s=12, alpha=0.3)
-    #     plt.xlim([-100, 100])
-    #     plt.ylim([-100, 100])
-    #     plt.title(self.label, size=26)
-    #     plt.axis('off')
-    #
-    #     file_name = os.path.join(os.getcwd(), "images", "mini_maps", f'{self.label}.png')
-    #     plt.savefig(file_name, bbox_inches='tight', dpi=250)
-    #     # plt.clf()
-    #     # plt.savefig(file_name, bbox_inches=bbox_inches, dpi=250)
-    #     plt.show()
-
 
     @abstractmethod
     def compute_distances(self):
         pass
 
     #DIV-MERGE
     def embed(self, algorithm='MDS', object_type=None, virtual=False):
 
         if object_type is None:
             object_type = self.object_type
 
-        # election.coordinates[object_type] = KamadaKawai().embed(
-        #     distances=election.distances[object_type],
-        # )
         MDS_object = MDS(n_components=2, dissimilarity='precomputed',
 
             # max_iter=1000,
             # n_init=20,
             # eps=1e-6,
             )
 
         #DIV-MERGE
         if algorithm == 'PCA':
             self.coordinates[object_type] = pca(self.distances[object_type])
         else:
             self.coordinates[object_type] = MDS_object.fit_transform(self.distances[object_type])
 
         if object_type == 'vote':
-            length = self.num_voters
+            length = self.num_options
         elif object_type == 'candidate':
-            length = self.num_candidates
+            # length = experiment_id.num_candidates
+            pass
         else:
             logging.warning('No such type of object!')
             length = None
 
         # ADJUST
         # find max dist
         # if (not ('identity' in election.culture_id.lower() and object_type=='vote')) \
@@ -371,16 +280,23 @@
 
                 if left_ctr < right_ctr:
                     self.rotate(math.pi, object_type)
 
             except Exception:
                 pass
 
+
+        if object_type == 'vote':
+            length = self.num_options
+        elif object_type == 'candidate':
+            length = self.num_candidates
+            pass
+
         if self.is_exported and not virtual:
-            exports.export_coordinates(self, object_type=object_type)
+            exports.export_coordinates(self, object_type=object_type, length=length)
 
     def all_dist_zeros(self, object_type):
         if np.abs(self.distances[object_type]).sum():
             return False
         else:
             return True
 
@@ -405,18 +321,22 @@
 
     def compute_feature(self, feature_id, feature_long_id=None, **kwargs):
         if feature_long_id is None:
             feature_long_id = feature_id
         feature = get_local_feature(feature_id)
         self.features[feature_long_id] = feature(self, **kwargs)
 
-    def get_feature(self, feature_id, feature_long_id=None, **kwargs):
+    def get_feature(self,
+                    feature_id,
+                    feature_long_id=None,
+                    overwrite=False,
+                    **kwargs):
         if feature_long_id is None:
             feature_long_id = feature_id
-        if feature_id not in self.features:
+        if feature_id not in self.features or overwrite:
             self.compute_feature(feature_id, feature_long_id, **kwargs)
         return self.features[feature_long_id]
 
 
 def map_the_votes(election, party_id, party_size) -> Election:
     new_votes = [[] for _ in range(election.num_voters)]
     for i in range(election.num_voters):
```

### Comparing `mapel-elections-2.0.5/src/mapel/elections/objects/ElectionExperiment.py` & `mapel-elections-2.0.6/src/mapel/elections/objects/ElectionExperiment.py`

 * *Files 6% similar despite different names*

```diff
@@ -15,14 +15,16 @@
 import mapel.elections.other.rules as rules
 import mapel.elections.features_ as features
 from mapel.core.objects.Experiment import Experiment
 import mapel.core.printing as pr
 from mapel.core.utils import *
 from mapel.core.glossary import *
 
+import mapel.core.persistence.experiment_exports as exports
+
 try:
     from sklearn.manifold import MDS
     from sklearn.manifold import TSNE
     from sklearn.manifold import SpectralEmbedding
     from sklearn.manifold import LocallyLinearEmbedding
     from sklearn.manifold import Isomap
 except ImportError as error:
@@ -54,21 +56,22 @@
     def add_feature(self, name, function):
         pass
 
     @abstractmethod
     def add_culture(self, name, function):
         pass
 
-    def __init__(self, shift=False, **kwargs):
-        super().__init__(**kwargs)
-        self.shift = shift
+    def __init__(self, is_shifted=False, instance_type=None, **kwargs):
+        self.instance_type = instance_type
+        self.is_shifted = is_shifted
         self.default_num_candidates = 10
         self.default_num_voters = 100
         self.default_committee_size = 1
         self.all_winning_committees = {}
+        super().__init__(**kwargs)
 
     def __getattr__(self, attr):
         if attr == 'elections':
             return self.instances
         elif attr == 'num_elections':
             return self.num_instances
         else:
@@ -102,27 +105,28 @@
                     writer.writerow(row)
 
     def add_instances_to_experiment(self):
         instances = {}
 
         for family_id in self.families:
             single = self.families[family_id].single
-
             ids = []
             for j in range(self.families[family_id].size):
                 instance_id = get_instance_id(single, family_id, j)
                 if self.instance_type == 'ordinal':
                     instance = OrdinalElection(self.experiment_id, instance_id,
                                                is_imported=True,
                                                fast_import=self.fast_import,
-                                               with_matrix=self.with_matrix)
+                                               with_matrix=self.with_matrix,
+                                               label=self.families[family_id].label)
                 elif self.instance_type == 'approval':
                     instance = ApprovalElection(self.experiment_id, instance_id,
                                                 is_imported=True,
-                                                fast_import=self.fast_import)
+                                                fast_import=self.fast_import,
+                                                label=self.families[family_id].label)
                 else:
                     instance = None
 
                 instances[instance_id] = instance
                 ids.append(str(instance_id))
 
             self.families[family_id].election_ids = ids
@@ -215,15 +219,14 @@
                 family_id += '_' + str(float(params['phi']))
             elif culture_id in {'norm-mallows', 'norm-mallows_matrix'} \
                     and params['normphi'] is not None:
                 family_id += '_' + str(float(params['normphi']))
 
         elif label is None:
             label = family_id
-
         self.families[family_id] = ElectionFamily(culture_id=culture_id,
                                                   family_id=family_id,
                                                   params=params,
                                                   label=label,
                                                   color=color,
                                                   alpha=alpha,
                                                   show=show,
@@ -239,15 +242,16 @@
 
         self.num_families = len(self.families)
         self.num_elections = sum([self.families[family_id].size for family_id in self.families])
         self.main_order = [i for i in range(self.num_elections)]
 
         new_instances = self.families[family_id].prepare_family(
             is_exported=self.is_exported,
-            experiment_id=self.experiment_id)
+            experiment_id=self.experiment_id,
+            instance_type=self.instance_type)
 
         for instance_id in new_instances:
             self.instances[instance_id] = new_instances[instance_id]
 
         self.families[family_id].instance_ids = list(new_instances.keys())
 
         return list(new_instances.keys())
@@ -261,15 +265,14 @@
                          marker: str = 'o',
                          num_candidates: int = None,
                          num_voters: int = None,
                          family_id: str = None):
 
         if label is None:
             label = family_id
-
         self.families[family_id] = ElectionFamily(culture_id=culture_id,
                                                   family_id=family_id,
                                                   label=label,
                                                   color=color,
                                                   alpha=alpha,
                                                   show=show,
                                                   size=0,
@@ -295,15 +298,17 @@
 
         for family_id in tqdm(self.families, desc="Preparing instances"):
 
             new_instances = self.families[family_id].prepare_family(
                 is_exported=self.is_exported,
                 experiment_id=self.experiment_id,
                 store_points=store_points,
-                is_aggregated=is_aggregated)
+                is_aggregated=is_aggregated,
+                instance_type=self.instance_type,
+            )
 
             for instance_id in new_instances:
                 self.instances[instance_id] = new_instances[instance_id]
 
     def compute_winners(self, method=None, num_winners=1):
         for election_id in self.elections:
             self.elections[election_id].compute_winners(method=method, num_winners=num_winners)
@@ -376,52 +381,40 @@
                 processes.append(process)
 
             for process in processes:
                 process.join()
 
             distances = {instance_id: {} for instance_id in self.instances}
             times = {instance_id: {} for instance_id in self.instances}
+
             for t in range(num_processes):
 
                 file_name = f'{distance_id}_p{t}.csv'
-                path = os.path.join(os.getcwd(), "experiments", self.experiment_id, "distances",
+                path = os.path.join(os.getcwd(),
+                                    "experiments",
+                                    self.experiment_id,
+                                    "distances",
                                     file_name)
 
                 with open(path, 'r', newline='') as csv_file:
                     reader = csv.DictReader(csv_file, delimiter=';')
 
                     for row in reader:
-                        distances[row['instance_id_1']][row['instance_id_2']] = float(
-                            row['distance'])
-                        times[row['instance_id_1']][row['instance_id_2']] = float(row['time'])
+                        distances[row['instance_id_1']][row['instance_id_2']] = \
+                            float(row['distance'])
+                        times[row['instance_id_1']][row['instance_id_2']] = \
+                            float(row['time'])
 
         if self.is_exported:
-            self._store_distances_to_file(distance_id, distances, times, self_distances)
+            exports.export_distances_to_file(self, distance_id, distances, times, self_distances)
 
         self.distances = distances
         self.times = times
         self.matchings = matchings
 
-    def _store_distances_to_file(self, distance_id, distances, times, self_distances):
-
-        path_to_folder = os.path.join(os.getcwd(), "experiments", self.experiment_id, "distances")
-        make_folder_if_do_not_exist(path_to_folder)
-        path = os.path.join(path_to_folder, f'{distance_id}.csv')
-
-        with open(path, 'w', newline='') as csv_file:
-            writer = csv.writer(csv_file, delimiter=';')
-            writer.writerow(["instance_id_1", "instance_id_2", "distance", "time"])
-
-            for i, election_1 in enumerate(self.elections):
-                for j, election_2 in enumerate(self.elections):
-                    if i < j or (i == j and self_distances):
-                        distance = str(distances[election_1][election_2])
-                        time_ = str(times[election_1][election_2])
-                        writer.writerow([election_1, election_2, distance, time_])
-
     def get_election_id_from_model_name(self, culture_id: str) -> str:
         for family_id in self.families:
             if self.families[family_id].culture_id == culture_id:
                 return family_id
 
     def print_matrix(self, **kwargs):
         pr.print_matrix(experiment=self, **kwargs)
@@ -502,31 +495,35 @@
                                                      show=show,
                                                      size=size,
                                                      marker=marker,
                                                      starting_from=starting_from,
                                                      num_candidates=num_candidates,
                                                      num_voters=num_voters,
                                                      path=path,
-                                                     single=single,
-                                                     instance_type=self.instance_type)
+                                                     single=single)
                 starting_from += size
 
                 all_num_candidates.append(num_candidates)
                 all_num_voters.append(num_voters)
 
             check_if_all_equal(all_num_candidates, 'num_candidates')
             check_if_all_equal(all_num_voters, 'num_voters')
 
             self.num_families = len(families)
             self.num_elections = sum([families[family_id].size for family_id in families])
             self.main_order = [i for i in range(self.num_elections)]
 
         return families
 
-    def compute_feature(self, feature_id: str = None, feature_params=None, **kwargs) -> dict:
+    def compute_feature(self,
+                        feature_id: str = None,
+                        feature_params=None,
+                        overwrite=False,
+                        saveas=None,
+                        **kwargs) -> dict:
 
         if feature_params is None:
             feature_params = {}
 
         if feature_id in ['priceability', 'core', 'ejr']:
             feature_long_id = f'{feature_id}_{feature_params["rule"]}'
         elif feature_id in ['distortion', 'monotonicity']:
@@ -536,37 +533,38 @@
 
         num_iterations = 1
         if 'num_interations' in feature_params:
             num_iterations = feature_params['num_interations']
 
         if feature_id == 'ejr':
             feature_dict = {'value': {}, 'time': {}, 'ejr': {}, 'pjr': {}, 'jr': {}, 'pareto': {}}
-        elif feature_id in FEATURES_WITH_DISSAT:
-            feature_dict = {'value': {}, 'time': {}, 'dissat': {}}
         else:
             feature_dict = {'value': {}, 'time': {}}
 
         if feature_id in MAIN_GLOBAL_FEATUERS or feature_id in ELECTION_GLOBAL_FEATURES:
 
             feature = features.get_global_feature(feature_id)
 
             values = feature(self, election_ids=list(self.instances), **kwargs)
 
-            for instance_id in tqdm(self.instances):
+            for instance_id in tqdm(self.instances, desc='Computing feature'):
                 feature_dict['value'][instance_id] = values[instance_id]
-                feature_dict['time'][instance_id] = 0
+                if values[instance_id] is None:
+                    feature_dict['time'][instance_id] = None
+                else:
+                    feature_dict['time'][instance_id] = 0
 
         else:
             feature = features.get_local_feature(feature_id)
 
             for instance_id in tqdm(self.instances):
                 instance = self.elections[instance_id]
 
                 start = time.time()
-
+                solution = None
                 for _ in range(num_iterations):
 
                     if feature_id in ['monotonicity_1', 'monotonicity_triplets']:
                         value = feature(self, instance)
 
                     elif feature_id in {'avg_distortion_from_guardians',
                                         'worst_distortion_from_guardians',
@@ -574,90 +572,60 @@
                                         'distortion_from_top_100'}:
                         value = feature(self, instance_id)
                     elif feature_id in ['ejr', 'core', 'pareto', 'priceability',
                                         'cohesiveness']:
                         value = instance.get_feature(feature_id, feature_long_id,
                                                      feature_params=feature_params)
                     else:
-                        value = instance.get_feature(feature_id, feature_long_id, **kwargs)
-
+                        solution = instance.get_feature(feature_id, feature_long_id,
+                                                        overwrite=overwrite, **kwargs)
                 total_time = time.time() - start
                 total_time /= num_iterations
 
-                if feature_id == 'ejr':
-                    feature_dict['ejr'][instance_id] = int(value['ejr'])
-                    feature_dict['pjr'][instance_id] = int(value['pjr'])
-                    feature_dict['jr'][instance_id] = int(value['jr'])
-                    feature_dict['pareto'][instance_id] = int(value['pareto'])
-                    feature_dict['time'][instance_id] = total_time
-
-                elif feature_id in FEATURES_WITH_DISSAT:
-                    feature_dict['value'][instance_id] = value[0]
+                if solution is not None:
+                    if type(solution) is dict:
+                        for key in solution:
+                            if key not in feature_dict:
+                                feature_dict[key] = {}
+                            feature_dict[key][instance_id] = solution[key]
+                    else:
+                        feature_dict['value'][instance_id] = solution
                     feature_dict['time'][instance_id] = total_time
-                    feature_dict['dissat'][instance_id] = value[1]
                 else:
                     feature_dict['value'][instance_id] = value
                     feature_dict['time'][instance_id] = total_time
 
+        if saveas is None:
+            saveas = feature_long_id
+
         if self.is_exported:
-            self._store_election_feature(feature_id, feature_long_id, feature_dict)
+            exports.export_feature_to_file(self,
+                                           feature_id,
+                                           saveas,
+                                           feature_dict)
 
-        self.features[feature_long_id] = feature_dict
+        self.features[saveas] = feature_dict
         return feature_dict
 
-    def _store_election_feature(self, feature_id, feature_long_id, feature_dict):
-
-        path_to_folder = os.path.join(os.getcwd(), "experiments", self.experiment_id, "features")
-        make_folder_if_do_not_exist(path_to_folder)
-
-        if feature_id in EMBEDDING_RELATED_FEATURE:
-            path = os.path.join(os.getcwd(), "experiments", self.experiment_id,
-                                "features", f'{feature_id}_{self.embedding_id}.csv')
-        else:
-            path = os.path.join(os.getcwd(), "experiments", self.experiment_id,
-                                "features", f'{feature_long_id}.csv')
-
-        with open(path, 'w', newline='') as csv_file:
-            writer = csv.writer(csv_file, delimiter=';')
-            if feature_id == 'ejr':
-                writer.writerow(["instance_id", "ejr", "pjr", "jr", "pareto", "time"])
-                for key in feature_dict['ejr']:
-                    writer.writerow([key, feature_dict['ejr'][key],
-                                     feature_dict['pjr'][key],
-                                     feature_dict['jr'][key],
-                                     feature_dict['pareto'][key],
-                                     feature_dict['time'][key]])
-            elif feature_id in {'partylist'}:
-                writer.writerow(["instance_id", "value", "bound", "num_large_parties"])
-                for key in feature_dict:
-                    writer.writerow([key, feature_dict[key][0], feature_dict[key][1],
-                                     feature_dict[key][2]])
-            elif feature_id in FEATURES_WITH_DISSAT:
-                writer.writerow(["instance_id", "value", 'time', 'dissat'])
-                for key in feature_dict['value']:
-                    writer.writerow(
-                        [key, feature_dict['value'][key], feature_dict['time'][key],
-                         feature_dict['dissat'][key]])
-            else:
-                writer.writerow(["instance_id", "value", "time"])
-                for key in feature_dict['value']:
-                    writer.writerow([key, feature_dict['value'][key], feature_dict['time'][key]])
-
-    def compute_rules(self, list_of_rules, committee_size: int = 10,
+    def compute_rules(self, list_of_rules,
+                      committee_size: int = 10,
                       resolute: bool = False) -> None:
         for rule_name in list_of_rules:
             print('Computing', rule_name)
             if rule_name in NOT_ABCVOTING_RULES:
-                rules.compute_not_abcvoting_rule(experiment=self, rule_name=rule_name,
-                                                 committee_size=committee_size, resolute=resolute)
+                rules.compute_not_abcvoting_rule(experiment=self,
+                                                 rule_name=rule_name,
+                                                 committee_size=committee_size,
+                                                 resolute=resolute)
             else:
                 rules.compute_abcvoting_rule(experiment=self, rule_name=rule_name,
-                                             committee_size=committee_size, resolute=resolute)
+                                             committee_size=committee_size,
+                                             resolute=resolute)
 
-    def import_committees(self, list_of_rules) -> None:
+    def import_committees(self, list_of_rules):
         for rule_name in list_of_rules:
             self.all_winning_committees[rule_name] = rules.import_committees_from_file(
                 experiment_id=self.experiment_id, rule_name=rule_name)
 
     def add_election_to_family(self, election=None, family_id=None):
         self.instances[election.instance_id] = election
         self.families[family_id].add_election(election)
```

### Comparing `mapel-elections-2.0.5/src/mapel/elections/objects/ElectionFamily.py` & `mapel-elections-2.0.6/src/mapel/elections/objects/ElectionFamily.py`

 * *Files 5% similar despite different names*

```diff
@@ -3,40 +3,39 @@
 import copy
 import logging
 
 from mapel.core.objects.Family import Family
 from mapel.elections.objects.OrdinalElection import OrdinalElection
 from mapel.elections.objects.ApprovalElection import ApprovalElection
 from mapel.core.utils import *
-import mapel.elections.cultures.mallows as mallows
 from mapel.elections.cultures.params import *
 
 
 class ElectionFamily(Family):
     """ Family of elections: a set of elections from the same election culture_id """
 
     def __init__(self,
                  culture_id: str = None,
-                 family_id='none',
+                 family_id: str = 'none',
                  params: dict = None,
                  size: int = 1,
                  label: str = None,
                  color: str = "black",
                  alpha: float = 1.,
                  ms: int = 20,
-                 show=True,
-                 marker='o',
+                 show: bool = True,
+                 marker: str = 'o',
                  starting_from: int = 0,
                  path: dict = None,
                  single: bool = False,
 
-                 num_candidates=None,
-                 num_voters=None,
+                 instance_type = None,
+                 num_candidates: int = None,
+                 num_voters: int = None,
                  election_ids=None,
-                 instance_type: str = 'ordinal',
                  **kwargs):
 
         super().__init__(culture_id=culture_id,
                          family_id=family_id,
                          params=params,
                          size=size,
                          label=label,
@@ -51,28 +50,33 @@
                          instance_ids=election_ids,
                          **kwargs)
 
         self.num_candidates = num_candidates
         self.num_voters = num_voters
         self.instance_type = instance_type
 
+
     def __getattr__(self, attr):
         if attr == 'election_ids':
             return self.instance_ids
         else:
             return self.__dict__[attr]
 
     def __setattr__(self, name, value):
         if name == "election_ids":
             return setattr(self, 'instance_ids', value)
         else:
             self.__dict__[name] = value
 
     def prepare_family(self, experiment_id=None, is_exported=True,
-                       store_points=False, is_aggregated=True):
+                       store_points=False, is_aggregated=True,
+                       instance_type=None):
+
+        if instance_type is not None:
+            self.instance_type = instance_type
 
         if self.instance_type == 'ordinal':
 
             elections = {}
             _keys = []
             for j in range(self.size):
 
@@ -82,33 +86,24 @@
                 path = self.path
                 if path is not None and 'variable' in path:
                     new_params, variable = get_params_for_paths(self, j)
                     if params is None:
                         params = {}
                     params = {**params, **new_params}
 
-                # if params is not None and 'normphi' in params:
-                #     params['phi'] = mallows.phi_from_relphi(
-                #         self.num_candidates, relphi=params['normphi'])
-
-                # if self.culture_id in {'all_votes'}:
-                #     params['iter_id'] = j
-
-                # if self.culture_id in {'crate'}:
-                #     new_params = get_params_for_crate(j)
-                #     params = {**params, **new_params}
-
                 election_id = get_instance_id(self.single, self.family_id, j)
 
-                election = OrdinalElection(experiment_id, election_id, culture_id=self.culture_id,
-                                           num_voters=self.num_voters, label=self.label,
+                election = OrdinalElection(experiment_id, election_id,
+                                           culture_id=self.culture_id,
+                                           num_voters=self.num_voters,
+                                           label=self.label,
                                            num_candidates=self.num_candidates,
-                                           params=copy.deepcopy(params), ballot_type=self.instance_type,
-                                           variable=variable, is_imported=False,
-                                           # printing_params=printing_params,
+                                           params=copy.deepcopy(params),
+                                           variable=variable,
+                                           is_imported=False,
                                            )
 
                 election.prepare_instance(is_exported=is_exported, is_aggregated=is_aggregated)
 
                 if store_points:
                     try:
                         election.points['voters'] = election.import_ideal_points('voters')
@@ -174,14 +169,12 @@
 
         return elections
 
     def add_election(self, election):
         self.size += 1
         self.election_ids.append(election.instance_id)
 
-        pass
-
 
 
 # # # # # # # # # # # # # # # #
 # LAST CLEANUP ON: 12.10.2021 #
 # # # # # # # # # # # # # # # #
```

### Comparing `mapel-elections-2.0.5/src/mapel/elections/objects/OrdinalElection.py` & `mapel-elections-2.0.6/src/mapel/elections/objects/OrdinalElection.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,7 +1,10 @@
+import logging
+from collections import Counter
+
 from matplotlib import pyplot as plt
 
 import csv
 
 from mapel.elections.cultures.group_separable import get_gs_caterpillar_vectors
 from mapel.elections.cultures.preflib import get_sushi_vectors
 from mapel.elections.cultures.single_crossing import get_single_crossing_vectors
@@ -20,76 +23,75 @@
 from mapel.elections.cultures.fake import *
 from mapel.elections.other.winners import get_borda_points
 
 
 class OrdinalElection(Election):
 
     def __init__(self,
-                 experiment_id,
-                 election_id,
+                 experiment_id=None,
+                 election_id=None,
                  culture_id=None,
                  votes=None,
-                 with_matrix=False,
                  params=None,
                  label=None,
-                 ballot_type: str = 'ordinal',
                  num_voters: int = None,
                  num_candidates: int = None,
-                 is_imported: bool = False,
-                 is_shifted: bool = False,
                  variable=None,
                  fast_import=False,
                  **kwargs):
 
-        super().__init__(experiment_id,
-                         election_id,
+        super().__init__(experiment_id=experiment_id,
+                         election_id=election_id,
                          culture_id=culture_id,
                          votes=votes,
-                         ballot_type=ballot_type,
                          label=label,
                          num_voters=num_voters,
                          num_candidates=num_candidates,
                          fast_import=fast_import,
                          **kwargs)
 
         self.params = params
         self.variable = variable
-
         self.vectors = []
         self.matrix = []
-        self.borda_points = []
         self.potes = None
         self.condorcet = None
         self.points = {}
         self.alliances = {}
 
-        if is_imported and experiment_id != 'virtual':
+        self.import_ordinal_election()
+
+    def import_ordinal_election(self):
+        if self.is_imported and self.experiment_id != 'virtual':
             try:
-                if votes is not None:
-                    self.culture_id = culture_id
-                    if str(votes[0]) in LIST_OF_FAKE_MODELS:
+                if self.votes is not None:
+                    self.culture_id = self.culture_id
+                    if str(self.votes[0]) in LIST_OF_FAKE_MODELS:
                         self.fake = True
-                        self.votes = votes[0]
-                        self.num_candidates = votes[1]
-                        self.num_voters = votes[2]
+                        self.votes = self.votes[0]
+                        self.num_candidates = self.votes[1]
+                        self.num_voters = self.votes[2]
                     else:
-                        self.votes = votes
-                        self.num_candidates = len(votes[0])
-                        self.num_voters = len(votes)
+                        self.votes = self.votes
+                        self.num_candidates = len(self.votes[0])
+                        self.num_voters = len(self.votes)
                         self.compute_potes()
                 else:
-                    self.fake = imports.check_if_fake(experiment_id, election_id, 'soc')
+                    self.fake = imports.check_if_fake(self.experiment_id, self.election_id, 'soc')
                     if self.fake:
                         self.culture_id, self.params, self.num_voters, \
-                        self.num_candidates = imports.import_fake_soc_election(experiment_id,
-                                                                               election_id)
+                        self.num_candidates = imports.import_fake_soc_election(self.experiment_id,
+                                                                               self.election_id)
                     else:
+
                         self.votes, self.num_voters, self.num_candidates, self.params, \
-                        self.culture_id, self.alliances = imports.import_real_soc_election(
-                            experiment_id, election_id, is_shifted)
+                        self.culture_id, self.alliances, \
+                        self.num_options, self.quantites = imports.import_real_soc_election(
+                            self.experiment_id, self.election_id, self.is_shifted)
+
                         try:
                             self.points['voters'] = self.import_ideal_points('voters')
                             self.points['candidates'] = self.import_ideal_points('candidates')
                         except:
                             pass
 
                         try:
@@ -98,21 +100,18 @@
                                 self.alpha = self.params['alpha']
                         except KeyError:
                             print("Error")
                             pass
 
                 self.candidatelikeness_original_vectors = {}
 
-                if with_matrix:
-                    self.matrix = self.import_matrix()
-                    self.vectors = self.matrix.transpose()
-                else:
-                    if not fast_import:
-                        self.votes_to_positionwise_vectors()
+                if not self.fast_import:
+                    self.votes_to_positionwise_vectors()
             except:
+                self.is_correct = False
                 pass
 
         if self.params is None:
             self.params = {}
 
         try:
             self.params, self.printing_params = update_params_ordinal(
@@ -192,16 +191,19 @@
     def votes_to_pairwise_matrix(self) -> np.ndarray:
         """ convert VOTES to pairwise MATRIX """
         matrix = np.zeros([self.num_candidates, self.num_candidates])
         if self.fake:
             if self.culture_id in {'identity', 'uniformity', 'antagonism', 'stratification'}:
                 matrix = get_fake_matrix_single(self.culture_id, self.num_candidates)
             elif self.culture_id in PATHS:
-                matrix = get_fake_convex(self.culture_id, self.num_candidates, self.num_voters,
-                                         self.fake_param, get_fake_matrix_single)
+                matrix = get_fake_convex(self.culture_id,
+                                         self.num_candidates,
+                                         self.num_voters,
+                                         self.fake_param,
+                                         get_fake_matrix_single)
 
         else:
             for v in range(self.num_voters):
                 for c1 in range(self.num_candidates):
                     for c2 in range(c1 + 1, self.num_candidates):
                         matrix[int(self.votes[v][c1])][
                             int(self.votes[v][c2])] += 1
@@ -215,16 +217,18 @@
         """ convert VOTES to Borda vector """
         borda_vector = np.zeros([self.num_candidates])
         if self.fake:
             if self.culture_id in {'identity', 'uniformity', 'antagonism', 'stratification'}:
                 borda_vector = get_fake_borda_vector(self.culture_id, self.num_candidates,
                                                      self.num_voters)
             elif self.culture_id in PATHS:
-                borda_vector = get_fake_convex(self.culture_id, self.num_candidates,
-                                               self.num_voters, self.params,
+                borda_vector = get_fake_convex(self.culture_id,
+                                               self.num_candidates,
+                                               self.num_voters,
+                                               self.params,
                                                get_fake_borda_vector)
         else:
             c = self.num_candidates
             v = self.num_voters
             vectors = self.votes_to_positionwise_vectors()
             borda_vector = [sum([vectors[i][j] * (c - j - 1) for j in range(c)]) * v for i in
                             range(self.num_candidates)]
@@ -248,28 +252,28 @@
         vectors = self.votes_to_positionwise_matrix()
         return [self.vector_to_interval(vectors[i], precision=precision)
                 for i in range(len(vectors))]
 
     def votes_to_voterlikeness_vectors(self) -> np.ndarray:
         return self.votes_to_voterlikeness_matrix()
 
-    def votes_to_voterlikeness_matrix(self) -> np.ndarray:
+    def votes_to_voterlikeness_matrix(self, vote_distance='swap') -> np.ndarray:
         """ convert VOTES to voter-likeness MATRIX """
         matrix = np.zeros([self.num_voters, self.num_voters])
         self.compute_potes()
 
         for v1 in range(self.num_voters):
             for v2 in range(self.num_voters):
-                matrix[v1][v2] = swap_distance_between_potes(self.potes[v1], self.potes[v2])
-                # matrix[v1][v2] = spearman_distance_between_potes(election.potes[v1], election.potes[v2])
+                if vote_distance == 'swap':
+                    matrix[v1][v2] = swap_distance_between_potes(self.potes[v1], self.potes[v2])
+                elif vote_distance == 'spearman':
+                    matrix[v1][v2] = spearman_distance_between_potes(self.potes[v1], self.potes[v2])
 
-        # VOTERLIKENESS IS SYMMETRIC
         for i in range(self.num_voters):
             for j in range(i + 1, self.num_voters):
-                # matrix[i][j] **= 0.5
                 matrix[j][i] = matrix[i][j]
 
         return matrix
 
     def votes_to_agg_voterlikeness_vector(self):
         """ convert VOTES to Borda vector """
 
@@ -300,66 +304,87 @@
             self.winners = compute_borda_winners(election=self, num_winners=num_winners)
         if method == 'stv':
             self.winners = compute_stv_winners(election=self, num_winners=num_winners)
         if method in {'approx_cc', 'approx_hb', 'approx_pav'}:
             self.winners = generate_winners(election=self, num_winners=num_winners)
 
     def prepare_instance(self, is_exported=None, is_aggregated=True):
-        # election.params['exp_id'] = election.experiment_id
-        # election.params['ele_id'] = election.election_id
-        # election.params['is_aggregated'] = is_aggregated
         if 'num_alliances' in self.params:
             self.votes, self.alliances = generate_ordinal_alliance_votes(
                 culture_id=self.culture_id,
                 num_candidates=self.num_candidates,
                 num_voters=self.num_voters,
                 params=self.params)
         else:
             self.votes = generate_ordinal_votes(culture_id=self.culture_id,
                                                 num_candidates=self.num_candidates,
                                                 num_voters=self.num_voters,
                                                 params=self.params)
 
+        c = Counter(map(tuple, self.votes))
+        counted_votes = [[count, list(row)] for row, count in c.items()]
+        counted_votes = sorted(counted_votes, reverse=True)
+        self.quantites = [a[0] for a in counted_votes]
+        self.num_options = len(counted_votes)
+
         if is_exported:
             exports.export_ordinal_election(self, is_aggregated=is_aggregated)
 
+    def get_distinct_votes(self):
+        import itertools
+        votes = self.votes
+        votes = votes.tolist()
+        votes.sort()
+        return list(k for k, _ in itertools.groupby(votes))
+
     def compute_distances(self, distance_id='swap', object_type=None):
         """ Return: distances between votes """
         if object_type is None:
             object_type = self.object_type
 
+        self.distinct_votes = self.get_distinct_votes()
+        self.distinct_potes = convert_votes_to_potes(self.distinct_votes)
+        self.num_dist_votes = len(self.distinct_votes)
+
         if object_type == 'vote':
-            self.compute_potes()
-            distances = np.zeros([self.num_voters, self.num_voters])
-            for v1 in range(self.num_voters):
-                for v2 in range(self.num_voters):
+            distances = np.zeros([self.num_dist_votes, self.num_dist_votes])
+            for v1 in range(self.num_dist_votes):
+                for v2 in range(self.num_dist_votes):
                     if distance_id == 'swap':
                         distances[v1][v2] = swap_distance_between_potes(
-                            self.potes[v1], self.potes[v2])
+                            self.distinct_potes[v1], self.distinct_potes[v2])
                     elif distance_id == 'spearman':
                         distances[v1][v2] = spearman_distance_between_potes(
-                            self.potes[v1], self.potes[v2])
+                            self.distinct_potes[v1], self.distinct_potes[v2])
         elif object_type == 'candidate':
             self.compute_potes()
             if distance_id == 'domination':
                 distances = self.votes_to_pairwise_matrix()
                 distances = np.abs(distances - 0.5) * self.num_voters
                 np.fill_diagonal(distances, 0)
             elif distance_id == 'position':
                 distances = np.zeros([self.num_candidates, self.num_candidates])
                 for c1 in range(self.num_candidates):
                     for c2 in range(self.num_candidates):
                         dist = 0
                         for pote in self.potes:
                             dist += abs(pote[c1] - pote[c2])
                         distances[c1][c2] = dist
+        else:
+            logging.warning('incorrect object_type')
+
         self.distances[object_type] = distances
 
+        if object_type == 'vote':
+            length = self.num_dist_votes
+        elif object_type == 'candidate':
+            length = self.num_candidates
+
         if self.is_exported:
-            exports.export_distances(self, object_type=object_type)
+            exports.export_distances(self, object_type=object_type, length=length)
 
     def is_condorcet(self):
         """ Check if election witness Condorcet winner"""
         if self.condorcet is None:
             self.condorcet = is_condorcet(self)
         return self.condorcet
 
@@ -396,14 +421,16 @@
                   object_type=None, double_gradient=False, saveas=None, color='blue',
                   marker='o', title_size=20):
 
         if object_type == 'vote':
             length = self.num_voters
         elif object_type == 'candidate':
             length = self.num_candidates
+        else:
+            logging.warning(f'Incorrect object type: {object_type}')
 
         if object_type is None:
             object_type = self.object_type
 
         plt.figure(figsize=(6.4, 6.4))
 
         X = []
@@ -416,54 +443,72 @@
         if start:
             plt.scatter(X[0], Y[0],
                         color='sienna',
                         s=1000,
                         alpha=1,
                         marker='X')
 
-        if double_gradient:
-            for i in range(length):
-                x = float(self.points['voters'][i][0])
-                y = float(self.points['voters'][i][1])
-                plt.scatter(X[i], Y[i], color=[0, y, x], s=s, alpha=alpha)
-        else:
-            plt.scatter(X, Y, color=color, s=s, alpha=alpha, marker=marker)
+        if object_type == 'vote':
+            if double_gradient:
+                for i in range(length):
+                    x = float(self.points['voters'][i][0])
+                    y = float(self.points['voters'][i][1])
+                    plt.scatter(X[i], Y[i], color=[0, y, x], s=s, alpha=alpha)
+            else:
+                for i in range(len(X)):
+                    plt.scatter(X[i], Y[i], color=color, alpha=alpha, marker=marker,
+                                s=self.quantites[i] * s)
+
+        elif object_type == 'candidate':
+            for i in range(len(X)):
+                plt.scatter(X[i], Y[i], color=color, alpha=alpha, marker=marker,
+                            s=s)
+
+        #
+        # if circles:  # works only for votes
+        #     weighted_points = {}
+        #     Xs = {}
+        #     Ys = {}
+        #     for i in range(length):
+        #         str_elem = str(experiment_id.votes[i])
+        #         if str_elem in weighted_points:
+        #             weighted_points[str_elem] += 1
+        #         else:
+        #             weighted_points[str_elem] = 1
+        #             Xs[str_elem] = X[i]
+        #             Ys[str_elem] = Y[i]
+        #     for str_elem in weighted_points:
+        #         if weighted_points[str_elem] > 10 and str_elem != 'set()':
+        #             plt.scatter(Xs[str_elem], Ys[str_elem],
+        #                         color='purple',
+        #                         s=10 * weighted_points[str_elem],
+        #                         alpha=0.2)
 
-        if circles:  # works only for votes
-            weighted_points = {}
-            Xs = {}
-            Ys = {}
-            for i in range(length):
-                str_elem = str(self.votes[i])
-                if str_elem in weighted_points:
-                    weighted_points[str_elem] += 1
-                else:
-                    weighted_points[str_elem] = 1
-                    Xs[str_elem] = X[i]
-                    Ys[str_elem] = Y[i]
-            for str_elem in weighted_points:
-                if weighted_points[str_elem] > 10 and str_elem != 'set()':
-                    plt.scatter(Xs[str_elem], Ys[str_elem],
-                                color='purple',
-                                s=10 * weighted_points[str_elem],
-                                alpha=0.2)
         avg_x = np.mean(X)
         avg_y = np.mean(Y)
 
         if radius:
             plt.xlim([avg_x - radius, avg_x + radius])
             plt.ylim([avg_y - radius, avg_y + radius])
         # plt.title(election.label, size=38)
+
         plt.title(self.texify_label(self.label), size=title_size)
+
         # plt.title(election.texify_label(election.label), size=38, y=0.94)
         # plt.title(election.label, size=title_size)
         plt.axis('off')
 
         if saveas is None:
-            saveas = f'{self.label}'
+            saveas = f'{self.label}_{object_type}'
 
         file_name = os.path.join(os.getcwd(), "images", name, f'{saveas}.png')
         plt.savefig(file_name, bbox_inches='tight', dpi=100)
         if show:
             plt.show()
         else:
             plt.clf()
+
+
+def convert_votes_to_potes(votes):
+    """ Convert votes to positional votes (called potes) """
+    return np.array([[list(vote).index(i) for i, _ in enumerate(vote)]
+                     for vote in votes])
```

### Comparing `mapel-elections-2.0.5/src/mapel/elections/objects/OrdinalElectionExperiment.py` & `mapel-elections-2.0.6/src/mapel/elections/objects/OrdinalElectionExperiment.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 #!/usr/bin/env python
 import os
+from abc import ABC
 
 from mapel.elections.objects.ElectionExperiment import ElectionExperiment
 import mapel.elections.cultures_ as cultures
 import mapel.elections.features_ as features
 import mapel.elections.distances_ as distances
 
 try:
@@ -17,15 +18,15 @@
     TSNE = None
     SpectralEmbedding = None
     LocallyLinearEmbedding = None
     Isomap = None
     print(error)
 
 
-class OrdinalElectionExperiment(ElectionExperiment):
+class OrdinalElectionExperiment(ElectionExperiment, ABC):
     """Abstract set of elections."""
 
     def __init__(self, **kwargs):
         super().__init__(**kwargs)
 
     def add_culture(self, name, function):
         cultures.add_ordinal_culture(name, function)
@@ -34,22 +35,18 @@
         features.add_ordinal_feature(name, function)
 
     def add_distance(self, name, function):
         distances.add_ordinal_distance(name, function)
 
     def add_folders_to_experiment(self) -> None:
 
-        if not os.path.isdir("experiments/"):
-            os.mkdir(os.path.join(os.getcwd(), "experiments"))
-
-        if not os.path.isdir("images/"):
-            os.mkdir(os.path.join(os.getcwd(), "images"))
-
-        if not os.path.isdir("trash/"):
-            os.mkdir(os.path.join(os.getcwd(), "trash"))
+        dirs = ["experiments", "images", "trash"]
+        for dir in dirs:
+            if not os.path.isdir(dir):
+                os.mkdir(os.path.join(os.getcwd(), dir))
 
         if not os.path.isdir(os.path.join(os.getcwd(), "experiments", self.experiment_id)):
             os.mkdir(os.path.join(os.getcwd(), "experiments", self.experiment_id))
 
         list_of_folders = ['distances',
                            'features',
                            'coordinates',
```

### Comparing `mapel-elections-2.0.5/src/mapel/elections/other/matrices.py` & `mapel-elections-2.0.6/src/mapel/elections/other/matrices.py`

 * *Files identical despite different names*

### Comparing `mapel-elections-2.0.5/src/mapel/elections/other/matrix2png.py` & `mapel-elections-2.0.6/src/mapel/elections/other/matrix2png.py`

 * *Files identical despite different names*

### Comparing `mapel-elections-2.0.5/src/mapel/elections/other/pabulib.py` & `mapel-elections-2.0.6/src/mapel/elections/other/pabulib.py`

 * *Files identical despite different names*

### Comparing `mapel-elections-2.0.5/src/mapel/elections/other/rules.py` & `mapel-elections-2.0.6/src/mapel/elections/other/rules.py`

 * *Files identical despite different names*

### Comparing `mapel-elections-2.0.5/src/mapel/elections/other/winners.py` & `mapel-elections-2.0.6/src/mapel/elections/other/winners.py`

 * *Files identical despite different names*

### Comparing `mapel-elections-2.0.5/src/mapel/elections/persistence/election_exports.py` & `mapel-elections-2.0.6/src/mapel/elections/persistence/election_exports.py`

 * *Files 6% similar despite different names*

```diff
@@ -104,15 +104,15 @@
     else:
         export_votes_to_file(election,
                              election.culture_id,
                              election.num_candidates,
                              election.num_voters,
                              election.params,
                              path_to_file,
-                             election.ballot_type,
+                             ballot_type='approval',
                              votes=election.votes,
                              is_aggregated=is_aggregated)
 
 
 def export_ordinal_election(election, is_aggregated=True):
     """ Store ordinal election in a .soc file """
 
@@ -123,43 +123,43 @@
     if election.culture_id in LIST_OF_FAKE_MODELS:
         file_ = open(path_to_file, 'w')
         file_.write(f'$ {election.culture_id} {election.params} \n')
         file_.write(str(election.num_candidates) + '\n')
         file_.write(str(election.num_voters) + '\n')
         file_.close()
     else:
-        export_votes_to_file(election, election.culture_id, election.num_candidates, election.num_voters,
-                             election.params, path_to_file, election.ballot_type, votes=election.votes,
-                             is_aggregated=is_aggregated, alliances=election.alliances)
+        export_votes_to_file(election,
+                             election.culture_id,
+                             election.num_candidates,
+                             election.num_voters,
+                             election.params,
+                             path_to_file,
+                             ballot_type='ordinal',
+                             votes=election.votes,
+                             is_aggregated=is_aggregated,
+                             alliances=election.alliances)
 
 
-def export_distances(experiment, object_type='vote'):
+def export_distances(experiment, object_type='vote', length=None):
     file_name = f'{experiment.election_id}_{object_type}.csv'
     path = os.path.join(os.getcwd(), "experiments", experiment.experiment_id, "distances", file_name)
     with open(path, 'w', newline='') as csv_file:
         writer = csv.writer(csv_file, delimiter=';')
         writer.writerow(["v1", "v2", "distance"])
-        if object_type == 'vote':
-            length = experiment.num_voters
-        elif object_type == 'candidate':
-            length = experiment.num_candidates
         for v1 in range(length):
             for v2 in range(length):
                 distance = str(experiment.distances[object_type][v1][v2])
                 writer.writerow([v1, v2, distance])
 
 
-def export_coordinates(experiment, object_type='vote'):
+def export_coordinates(experiment, object_type='vote', length=None):
     file_name = f'{experiment.election_id}_{object_type}.csv'
     path = os.path.join(os.getcwd(), "experiments", experiment.experiment_id, "coordinates",
                         file_name)
     with open(path, 'w', newline='') as csv_file:
         writer = csv.writer(csv_file, delimiter=';')
         writer.writerow(["vote_id", "x", "y"])
-        if object_type == 'vote':
-            length = experiment.num_voters
-        elif object_type == 'candidate':
-            length = experiment.num_candidates
         for vote_id in range(length):
             x = str(experiment.coordinates[object_type][vote_id][0])
             y = str(experiment.coordinates[object_type][vote_id][1])
             writer.writerow([vote_id, x, y])
+
```

### Comparing `mapel-elections-2.0.5/src/mapel/elections/persistence/election_imports.py` & `mapel-elections-2.0.6/src/mapel/elections/persistence/election_imports.py`

 * *Files 2% similar despite different names*

```diff
@@ -41,30 +41,30 @@
 
     line = my_file.readline().rstrip("\n").split(',')
     num_voters = int(line[0])
     num_options = int(line[2])
     votes = [[0 for _ in range(num_candidates)] for _ in range(num_voters)]
 
     it = 0
+    quantites = []
     for j in range(num_options):
-        line = my_file.readline().rstrip("\n").split(',')
-        quantity = int(line[0])
+        line = list(map(int, my_file.readline().rstrip("\n").split(',')))
+        quantity = line[0]
+        quantites.append(quantity)
 
         for k in range(quantity):
-            for el in range(num_candidates):
-                votes[it][el] = int(line[el + 1])
+            votes[it] = line[1:num_candidates + 1]
             it += 1
 
     if is_shifted:
-        for i in range(num_voters):
-            for j in range(num_candidates):
-                votes[i][j] -= 1
+        votes = [[vote - 1 for vote in voter] for voter in votes]
     my_file.close()
 
-    return np.array(votes), num_voters, num_candidates, params, model_name, alliances
+    return np.array(votes), num_voters, num_candidates, params, model_name, alliances, \
+           num_options, quantites
 
 
 def import_fake_soc_election(experiment_id, name):
     """ Import fake ordinal election form .soc file """
 
     file_name = f'{name}.soc'
     path = os.path.join(os.getcwd(), "experiments", experiment_id, "elections", file_name)
@@ -128,19 +128,15 @@
                 it += 1
 
     if culture_id in NICE_NAME.values():
         rev_dict = dict(zip(NICE_NAME.values(), NICE_NAME.keys()))
         culture_id = rev_dict[culture_id]
 
     if is_shifted:
-        for i, vote in enumerate(votes):
-            new_vote = set()
-            for c in vote:
-                new_vote.add(c - 1)
-            votes[i] = new_vote
+        votes = [{c - 1 for c in vote} for vote in votes]
     my_file.close()
 
     return votes, num_voters, num_candidates, params, culture_id
 
 
 def import_fake_app_election(experiment_id: str, name: str):
     """ Import fake approval election from .app file """
```

### Comparing `mapel-elections-2.0.5/src/mapel_elections.egg-info/PKG-INFO` & `mapel-elections-2.0.6/src/mapel_elections.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mapel-elections
-Version: 2.0.5
+Version: 2.0.6
 Summary: Map of Elections
 Author-email: Stanislaw Szufa <s.szufa@gmail.com>, Niclas Boehmer <niclas.boehmer@tu-berlin.de>, Piotr Faliszewski <faliszew@agh.edu.pl>, Lukasz Janeczko <lukij1997@gmail.com>, Andrzej Kaczmarczyk <andrzej.kaczmarczyk@agh.edu.pl>, Tomasz Was <tomasz.t.was@gmail.com>
 License: Copyright (c) 2018-2022 Stanislaw Szufa and contributors
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
         of this software and associated documentation files (the "Software"), to deal
         in the Software without restriction, including without limitation the rights
```

### Comparing `mapel-elections-2.0.5/src/mapel_elections.egg-info/SOURCES.txt` & `mapel-elections-2.0.6/src/mapel_elections.egg-info/SOURCES.txt`

 * *Files identical despite different names*

