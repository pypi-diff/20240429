# Comparing `tmp/gerrychain-0.3.1.tar.gz` & `tmp/gerrychain-0.3.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gerrychain-0.3.1.tar", last modified: Sat Mar  2 00:08:43 2024, max compression
+gzip compressed data, was "gerrychain-0.3.2.tar", last modified: Mon Apr 29 21:54:52 2024, max compression
```

## Comparing `gerrychain-0.3.1.tar` & `gerrychain-0.3.2.tar`

### file list

```diff
@@ -1,67 +1,71 @@
-drwxr-xr-x   0 peter     (1000) peter     (1000)        0 2024-03-02 00:08:43.914765 gerrychain-0.3.1/
--rw-r--r--   0 peter     (1000) peter     (1000)     1510 2024-02-23 21:29:00.000000 gerrychain-0.3.1/LICENSE
--rw-r--r--   0 peter     (1000) peter     (1000)       68 2024-02-23 21:29:00.000000 gerrychain-0.3.1/MANIFEST.in
--rw-r--r--   0 peter     (1000) peter     (1000)    13359 2024-03-02 00:08:43.914765 gerrychain-0.3.1/PKG-INFO
--rw-r--r--   0 peter     (1000) peter     (1000)    12597 2024-03-01 23:44:29.000000 gerrychain-0.3.1/README.rst
-drwxr-xr-x   0 peter     (1000) peter     (1000)        0 2024-03-02 00:08:43.911432 gerrychain-0.3.1/gerrychain/
--rw-r--r--   0 peter     (1000) peter     (1000)      949 2024-03-01 23:44:29.000000 gerrychain-0.3.1/gerrychain/__init__.py
--rw-r--r--   0 peter     (1000) peter     (1000)      497 2024-03-02 00:08:43.914765 gerrychain-0.3.1/gerrychain/_version.py
--rw-r--r--   0 peter     (1000) peter     (1000)      868 2024-02-23 21:29:00.000000 gerrychain-0.3.1/gerrychain/accept.py
--rw-r--r--   0 peter     (1000) peter     (1000)     7956 2024-02-23 21:29:00.000000 gerrychain-0.3.1/gerrychain/chain.py
-drwxr-xr-x   0 peter     (1000) peter     (1000)        0 2024-03-02 00:08:43.911432 gerrychain-0.3.1/gerrychain/constraints/
--rw-r--r--   0 peter     (1000) peter     (1000)     3590 2024-02-23 21:29:00.000000 gerrychain-0.3.1/gerrychain/constraints/__init__.py
--rw-r--r--   0 peter     (1000) peter     (1000)     6780 2024-02-23 21:29:00.000000 gerrychain-0.3.1/gerrychain/constraints/bounds.py
--rw-r--r--   0 peter     (1000) peter     (1000)     2028 2024-02-23 21:29:00.000000 gerrychain-0.3.1/gerrychain/constraints/compactness.py
--rw-r--r--   0 peter     (1000) peter     (1000)     8855 2024-02-23 21:29:00.000000 gerrychain-0.3.1/gerrychain/constraints/contiguity.py
--rw-r--r--   0 peter     (1000) peter     (1000)     6511 2024-02-23 21:29:00.000000 gerrychain-0.3.1/gerrychain/constraints/validity.py
-drwxr-xr-x   0 peter     (1000) peter     (1000)        0 2024-03-02 00:08:43.911432 gerrychain-0.3.1/gerrychain/graph/
--rw-r--r--   0 peter     (1000) peter     (1000)      806 2024-02-23 21:29:00.000000 gerrychain-0.3.1/gerrychain/graph/__init__.py
--rw-r--r--   0 peter     (1000) peter     (1000)     4750 2024-02-23 21:29:00.000000 gerrychain-0.3.1/gerrychain/graph/adjacency.py
--rw-r--r--   0 peter     (1000) peter     (1000)     3138 2024-02-23 21:29:00.000000 gerrychain-0.3.1/gerrychain/graph/geo.py
--rw-r--r--   0 peter     (1000) peter     (1000)    19565 2024-02-23 21:29:00.000000 gerrychain-0.3.1/gerrychain/graph/graph.py
--rw-r--r--   0 peter     (1000) peter     (1000)    10446 2024-02-23 21:29:00.000000 gerrychain-0.3.1/gerrychain/grid.py
-drwxr-xr-x   0 peter     (1000) peter     (1000)        0 2024-03-02 00:08:43.911432 gerrychain-0.3.1/gerrychain/meta/
--rw-r--r--   0 peter     (1000) peter     (1000)      120 2024-02-23 21:29:00.000000 gerrychain-0.3.1/gerrychain/meta/__init__.py
--rw-r--r--   0 peter     (1000) peter     (1000)     2511 2024-02-23 21:29:00.000000 gerrychain-0.3.1/gerrychain/meta/diversity.py
--rw-r--r--   0 peter     (1000) peter     (1000)     3729 2024-02-23 21:29:00.000000 gerrychain-0.3.1/gerrychain/metagraph.py
-drwxr-xr-x   0 peter     (1000) peter     (1000)        0 2024-03-02 00:08:43.911432 gerrychain-0.3.1/gerrychain/metrics/
--rw-r--r--   0 peter     (1000) peter     (1000)      297 2024-02-23 21:29:00.000000 gerrychain-0.3.1/gerrychain/metrics/__init__.py
--rw-r--r--   0 peter     (1000) peter     (1000)     1145 2024-02-23 21:29:00.000000 gerrychain-0.3.1/gerrychain/metrics/compactness.py
--rw-r--r--   0 peter     (1000) peter     (1000)     5326 2024-02-23 21:29:00.000000 gerrychain-0.3.1/gerrychain/metrics/partisan.py
-drwxr-xr-x   0 peter     (1000) peter     (1000)        0 2024-03-02 00:08:43.911432 gerrychain-0.3.1/gerrychain/partition/
--rw-r--r--   0 peter     (1000) peter     (1000)      125 2024-02-23 21:29:00.000000 gerrychain-0.3.1/gerrychain/partition/__init__.py
--rw-r--r--   0 peter     (1000) peter     (1000)     7679 2024-02-23 21:29:00.000000 gerrychain-0.3.1/gerrychain/partition/assignment.py
--rw-r--r--   0 peter     (1000) peter     (1000)      832 2024-02-23 21:29:00.000000 gerrychain-0.3.1/gerrychain/partition/geographic.py
--rw-r--r--   0 peter     (1000) peter     (1000)     8264 2024-02-23 21:29:00.000000 gerrychain-0.3.1/gerrychain/partition/partition.py
--rw-r--r--   0 peter     (1000) peter     (1000)     2105 2024-02-23 21:29:00.000000 gerrychain-0.3.1/gerrychain/partition/subgraphs.py
-drwxr-xr-x   0 peter     (1000) peter     (1000)        0 2024-03-02 00:08:43.914765 gerrychain-0.3.1/gerrychain/proposals/
--rw-r--r--   0 peter     (1000) peter     (1000)      258 2024-02-23 21:29:00.000000 gerrychain-0.3.1/gerrychain/proposals/__init__.py
--rw-r--r--   0 peter     (1000) peter     (1000)     4677 2024-02-23 21:29:00.000000 gerrychain-0.3.1/gerrychain/proposals/proposals.py
--rw-r--r--   0 peter     (1000) peter     (1000)     3020 2024-02-23 21:29:00.000000 gerrychain-0.3.1/gerrychain/proposals/spectral_proposals.py
--rw-r--r--   0 peter     (1000) peter     (1000)    10615 2024-03-01 23:44:29.000000 gerrychain-0.3.1/gerrychain/proposals/tree_proposals.py
--rw-r--r--   0 peter     (1000) peter     (1000)    45960 2024-03-01 23:44:29.000000 gerrychain-0.3.1/gerrychain/tree.py
-drwxr-xr-x   0 peter     (1000) peter     (1000)        0 2024-03-02 00:08:43.914765 gerrychain-0.3.1/gerrychain/updaters/
--rw-r--r--   0 peter     (1000) peter     (1000)      848 2024-02-23 21:29:00.000000 gerrychain-0.3.1/gerrychain/updaters/__init__.py
--rw-r--r--   0 peter     (1000) peter     (1000)     7341 2024-02-23 21:29:00.000000 gerrychain-0.3.1/gerrychain/updaters/compactness.py
--rw-r--r--   0 peter     (1000) peter     (1000)     5493 2024-02-23 21:29:00.000000 gerrychain-0.3.1/gerrychain/updaters/county_splits.py
--rw-r--r--   0 peter     (1000) peter     (1000)     3868 2024-02-23 21:29:00.000000 gerrychain-0.3.1/gerrychain/updaters/cut_edges.py
--rw-r--r--   0 peter     (1000) peter     (1000)    15915 2024-02-23 21:29:00.000000 gerrychain-0.3.1/gerrychain/updaters/election.py
--rw-r--r--   0 peter     (1000) peter     (1000)     7255 2024-02-23 21:29:00.000000 gerrychain-0.3.1/gerrychain/updaters/flows.py
--rw-r--r--   0 peter     (1000) peter     (1000)    15735 2024-02-23 21:29:00.000000 gerrychain-0.3.1/gerrychain/updaters/locality_split_scores.py
--rw-r--r--   0 peter     (1000) peter     (1000)     1225 2024-02-23 21:29:00.000000 gerrychain-0.3.1/gerrychain/updaters/spanning_trees.py
--rw-r--r--   0 peter     (1000) peter     (1000)     7681 2024-02-23 21:29:00.000000 gerrychain-0.3.1/gerrychain/updaters/tally.py
-drwxr-xr-x   0 peter     (1000) peter     (1000)        0 2024-03-02 00:08:43.914765 gerrychain-0.3.1/gerrychain/vendor/
--rw-r--r--   0 peter     (1000) peter     (1000)        0 2024-02-23 21:29:00.000000 gerrychain-0.3.1/gerrychain/vendor/__init__.py
-drwxr-xr-x   0 peter     (1000) peter     (1000)        0 2024-03-02 00:08:43.914765 gerrychain-0.3.1/gerrychain/vendor/utm/
--rw-r--r--   0 peter     (1000) peter     (1000)      173 2024-02-23 21:29:00.000000 gerrychain-0.3.1/gerrychain/vendor/utm/__init__.py
--rw-r--r--   0 peter     (1000) peter     (1000)     8663 2024-02-23 21:29:00.000000 gerrychain-0.3.1/gerrychain/vendor/utm/conversion.py
--rw-r--r--   0 peter     (1000) peter     (1000)       44 2024-02-23 21:29:00.000000 gerrychain-0.3.1/gerrychain/vendor/utm/error.py
-drwxr-xr-x   0 peter     (1000) peter     (1000)        0 2024-03-02 00:08:43.911432 gerrychain-0.3.1/gerrychain.egg-info/
--rw-r--r--   0 peter     (1000) peter     (1000)    13359 2024-03-02 00:08:43.000000 gerrychain-0.3.1/gerrychain.egg-info/PKG-INFO
--rw-r--r--   0 peter     (1000) peter     (1000)     1582 2024-03-02 00:08:43.000000 gerrychain-0.3.1/gerrychain.egg-info/SOURCES.txt
--rw-r--r--   0 peter     (1000) peter     (1000)        1 2024-03-02 00:08:43.000000 gerrychain-0.3.1/gerrychain.egg-info/dependency_links.txt
--rw-r--r--   0 peter     (1000) peter     (1000)       73 2024-03-02 00:08:43.000000 gerrychain-0.3.1/gerrychain.egg-info/requires.txt
--rw-r--r--   0 peter     (1000) peter     (1000)       11 2024-03-02 00:08:43.000000 gerrychain-0.3.1/gerrychain.egg-info/top_level.txt
--rw-r--r--   0 peter     (1000) peter     (1000)      838 2024-03-02 00:08:43.914765 gerrychain-0.3.1/setup.cfg
--rw-r--r--   0 peter     (1000) peter     (1000)     1294 2024-03-01 23:44:29.000000 gerrychain-0.3.1/setup.py
--rw-r--r--   0 peter     (1000) peter     (1000)    86677 2024-03-01 23:57:07.000000 gerrychain-0.3.1/versioneer.py
+drwxr-xr-x   0 peter     (1000) peter     (1000)        0 2024-04-29 21:54:52.374457 gerrychain-0.3.2/
+-rw-r--r--   0 peter     (1000) peter     (1000)     1510 2024-04-29 21:52:34.000000 gerrychain-0.3.2/LICENSE
+-rw-r--r--   0 peter     (1000) peter     (1000)       68 2024-04-29 21:52:34.000000 gerrychain-0.3.2/MANIFEST.in
+-rw-r--r--   0 peter     (1000) peter     (1000)    13357 2024-04-29 21:54:52.374457 gerrychain-0.3.2/PKG-INFO
+-rw-r--r--   0 peter     (1000) peter     (1000)    12595 2024-04-29 21:52:34.000000 gerrychain-0.3.2/README.rst
+drwxr-xr-x   0 peter     (1000) peter     (1000)        0 2024-04-29 21:54:52.371124 gerrychain-0.3.2/gerrychain/
+-rw-r--r--   0 peter     (1000) peter     (1000)      949 2024-04-29 21:52:34.000000 gerrychain-0.3.2/gerrychain/__init__.py
+-rw-r--r--   0 peter     (1000) peter     (1000)      497 2024-04-29 21:54:52.374457 gerrychain-0.3.2/gerrychain/_version.py
+-rw-r--r--   0 peter     (1000) peter     (1000)      868 2024-04-29 21:52:34.000000 gerrychain-0.3.2/gerrychain/accept.py
+-rw-r--r--   0 peter     (1000) peter     (1000)     7912 2024-04-29 21:52:34.000000 gerrychain-0.3.2/gerrychain/chain.py
+drwxr-xr-x   0 peter     (1000) peter     (1000)        0 2024-04-29 21:54:52.371124 gerrychain-0.3.2/gerrychain/constraints/
+-rw-r--r--   0 peter     (1000) peter     (1000)     3590 2024-04-29 21:52:34.000000 gerrychain-0.3.2/gerrychain/constraints/__init__.py
+-rw-r--r--   0 peter     (1000) peter     (1000)     6780 2024-04-29 21:52:34.000000 gerrychain-0.3.2/gerrychain/constraints/bounds.py
+-rw-r--r--   0 peter     (1000) peter     (1000)     2028 2024-04-29 21:52:34.000000 gerrychain-0.3.2/gerrychain/constraints/compactness.py
+-rw-r--r--   0 peter     (1000) peter     (1000)     8914 2024-04-29 21:52:34.000000 gerrychain-0.3.2/gerrychain/constraints/contiguity.py
+-rw-r--r--   0 peter     (1000) peter     (1000)     6511 2024-04-29 21:52:34.000000 gerrychain-0.3.2/gerrychain/constraints/validity.py
+drwxr-xr-x   0 peter     (1000) peter     (1000)        0 2024-04-29 21:54:52.371124 gerrychain-0.3.2/gerrychain/graph/
+-rw-r--r--   0 peter     (1000) peter     (1000)      806 2024-04-29 21:52:34.000000 gerrychain-0.3.2/gerrychain/graph/__init__.py
+-rw-r--r--   0 peter     (1000) peter     (1000)     4750 2024-04-29 21:52:34.000000 gerrychain-0.3.2/gerrychain/graph/adjacency.py
+-rw-r--r--   0 peter     (1000) peter     (1000)     3138 2024-04-29 21:52:34.000000 gerrychain-0.3.2/gerrychain/graph/geo.py
+-rw-r--r--   0 peter     (1000) peter     (1000)    20283 2024-04-29 21:52:34.000000 gerrychain-0.3.2/gerrychain/graph/graph.py
+-rw-r--r--   0 peter     (1000) peter     (1000)    10446 2024-04-29 21:52:34.000000 gerrychain-0.3.2/gerrychain/grid.py
+drwxr-xr-x   0 peter     (1000) peter     (1000)        0 2024-04-29 21:54:52.371124 gerrychain-0.3.2/gerrychain/meta/
+-rw-r--r--   0 peter     (1000) peter     (1000)      120 2024-04-29 21:52:34.000000 gerrychain-0.3.2/gerrychain/meta/__init__.py
+-rw-r--r--   0 peter     (1000) peter     (1000)     2511 2024-04-29 21:52:34.000000 gerrychain-0.3.2/gerrychain/meta/diversity.py
+-rw-r--r--   0 peter     (1000) peter     (1000)     3729 2024-04-29 21:52:34.000000 gerrychain-0.3.2/gerrychain/metagraph.py
+drwxr-xr-x   0 peter     (1000) peter     (1000)        0 2024-04-29 21:54:52.371124 gerrychain-0.3.2/gerrychain/metrics/
+-rw-r--r--   0 peter     (1000) peter     (1000)      297 2024-04-29 21:52:34.000000 gerrychain-0.3.2/gerrychain/metrics/__init__.py
+-rw-r--r--   0 peter     (1000) peter     (1000)     1145 2024-04-29 21:52:34.000000 gerrychain-0.3.2/gerrychain/metrics/compactness.py
+-rw-r--r--   0 peter     (1000) peter     (1000)     5326 2024-04-29 21:52:34.000000 gerrychain-0.3.2/gerrychain/metrics/partisan.py
+drwxr-xr-x   0 peter     (1000) peter     (1000)        0 2024-04-29 21:54:52.371124 gerrychain-0.3.2/gerrychain/optimization/
+-rw-r--r--   0 peter     (1000) peter     (1000)      134 2024-04-29 21:52:34.000000 gerrychain-0.3.2/gerrychain/optimization/__init__.py
+-rwxr-xr-x   0 peter     (1000) peter     (1000)    10351 2024-04-29 21:52:34.000000 gerrychain-0.3.2/gerrychain/optimization/gingleator.py
+-rw-r--r--   0 peter     (1000) peter     (1000)    23179 2024-04-29 21:52:34.000000 gerrychain-0.3.2/gerrychain/optimization/optimization.py
+drwxr-xr-x   0 peter     (1000) peter     (1000)        0 2024-04-29 21:54:52.371124 gerrychain-0.3.2/gerrychain/partition/
+-rw-r--r--   0 peter     (1000) peter     (1000)      125 2024-04-29 21:52:34.000000 gerrychain-0.3.2/gerrychain/partition/__init__.py
+-rw-r--r--   0 peter     (1000) peter     (1000)     7679 2024-04-29 21:52:34.000000 gerrychain-0.3.2/gerrychain/partition/assignment.py
+-rw-r--r--   0 peter     (1000) peter     (1000)      832 2024-04-29 21:52:34.000000 gerrychain-0.3.2/gerrychain/partition/geographic.py
+-rw-r--r--   0 peter     (1000) peter     (1000)    10357 2024-04-29 21:52:34.000000 gerrychain-0.3.2/gerrychain/partition/partition.py
+-rw-r--r--   0 peter     (1000) peter     (1000)     2105 2024-04-29 21:52:34.000000 gerrychain-0.3.2/gerrychain/partition/subgraphs.py
+drwxr-xr-x   0 peter     (1000) peter     (1000)        0 2024-04-29 21:54:52.371124 gerrychain-0.3.2/gerrychain/proposals/
+-rw-r--r--   0 peter     (1000) peter     (1000)      258 2024-04-29 21:52:34.000000 gerrychain-0.3.2/gerrychain/proposals/__init__.py
+-rw-r--r--   0 peter     (1000) peter     (1000)     4677 2024-04-29 21:52:34.000000 gerrychain-0.3.2/gerrychain/proposals/proposals.py
+-rw-r--r--   0 peter     (1000) peter     (1000)     3020 2024-04-29 21:52:34.000000 gerrychain-0.3.2/gerrychain/proposals/spectral_proposals.py
+-rw-r--r--   0 peter     (1000) peter     (1000)    10625 2024-04-29 21:52:34.000000 gerrychain-0.3.2/gerrychain/proposals/tree_proposals.py
+-rw-r--r--   0 peter     (1000) peter     (1000)    54317 2024-04-29 21:52:34.000000 gerrychain-0.3.2/gerrychain/tree.py
+drwxr-xr-x   0 peter     (1000) peter     (1000)        0 2024-04-29 21:54:52.374457 gerrychain-0.3.2/gerrychain/updaters/
+-rw-r--r--   0 peter     (1000) peter     (1000)      848 2024-04-29 21:52:34.000000 gerrychain-0.3.2/gerrychain/updaters/__init__.py
+-rw-r--r--   0 peter     (1000) peter     (1000)     7341 2024-04-29 21:52:34.000000 gerrychain-0.3.2/gerrychain/updaters/compactness.py
+-rw-r--r--   0 peter     (1000) peter     (1000)     5493 2024-04-29 21:52:34.000000 gerrychain-0.3.2/gerrychain/updaters/county_splits.py
+-rw-r--r--   0 peter     (1000) peter     (1000)     3868 2024-04-29 21:52:34.000000 gerrychain-0.3.2/gerrychain/updaters/cut_edges.py
+-rw-r--r--   0 peter     (1000) peter     (1000)    15915 2024-04-29 21:52:34.000000 gerrychain-0.3.2/gerrychain/updaters/election.py
+-rw-r--r--   0 peter     (1000) peter     (1000)     7255 2024-04-29 21:52:34.000000 gerrychain-0.3.2/gerrychain/updaters/flows.py
+-rw-r--r--   0 peter     (1000) peter     (1000)    15735 2024-04-29 21:52:34.000000 gerrychain-0.3.2/gerrychain/updaters/locality_split_scores.py
+-rw-r--r--   0 peter     (1000) peter     (1000)     1225 2024-04-29 21:52:34.000000 gerrychain-0.3.2/gerrychain/updaters/spanning_trees.py
+-rw-r--r--   0 peter     (1000) peter     (1000)     7681 2024-04-29 21:52:34.000000 gerrychain-0.3.2/gerrychain/updaters/tally.py
+drwxr-xr-x   0 peter     (1000) peter     (1000)        0 2024-04-29 21:54:52.374457 gerrychain-0.3.2/gerrychain/vendor/
+-rw-r--r--   0 peter     (1000) peter     (1000)        0 2024-04-29 21:52:34.000000 gerrychain-0.3.2/gerrychain/vendor/__init__.py
+drwxr-xr-x   0 peter     (1000) peter     (1000)        0 2024-04-29 21:54:52.374457 gerrychain-0.3.2/gerrychain/vendor/utm/
+-rw-r--r--   0 peter     (1000) peter     (1000)      173 2024-04-29 21:52:34.000000 gerrychain-0.3.2/gerrychain/vendor/utm/__init__.py
+-rw-r--r--   0 peter     (1000) peter     (1000)     8663 2024-04-29 21:52:34.000000 gerrychain-0.3.2/gerrychain/vendor/utm/conversion.py
+-rw-r--r--   0 peter     (1000) peter     (1000)       44 2024-04-29 21:52:34.000000 gerrychain-0.3.2/gerrychain/vendor/utm/error.py
+drwxr-xr-x   0 peter     (1000) peter     (1000)        0 2024-04-29 21:54:52.371124 gerrychain-0.3.2/gerrychain.egg-info/
+-rw-r--r--   0 peter     (1000) peter     (1000)    13357 2024-04-29 21:54:52.000000 gerrychain-0.3.2/gerrychain.egg-info/PKG-INFO
+-rw-r--r--   0 peter     (1000) peter     (1000)     1696 2024-04-29 21:54:52.000000 gerrychain-0.3.2/gerrychain.egg-info/SOURCES.txt
+-rw-r--r--   0 peter     (1000) peter     (1000)        1 2024-04-29 21:54:52.000000 gerrychain-0.3.2/gerrychain.egg-info/dependency_links.txt
+-rw-r--r--   0 peter     (1000) peter     (1000)       73 2024-04-29 21:54:52.000000 gerrychain-0.3.2/gerrychain.egg-info/requires.txt
+-rw-r--r--   0 peter     (1000) peter     (1000)       11 2024-04-29 21:54:52.000000 gerrychain-0.3.2/gerrychain.egg-info/top_level.txt
+-rw-r--r--   0 peter     (1000) peter     (1000)      838 2024-04-29 21:54:52.374457 gerrychain-0.3.2/setup.cfg
+-rw-r--r--   0 peter     (1000) peter     (1000)     1294 2024-04-29 21:52:34.000000 gerrychain-0.3.2/setup.py
+-rw-r--r--   0 peter     (1000) peter     (1000)    86677 2024-04-29 21:52:34.000000 gerrychain-0.3.2/versioneer.py
```

### Comparing `gerrychain-0.3.1/LICENSE` & `gerrychain-0.3.2/LICENSE`

 * *Files identical despite different names*

### Comparing `gerrychain-0.3.1/PKG-INFO` & `gerrychain-0.3.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gerrychain
-Version: 0.3.1
+Version: 0.3.2
 Summary: Use Markov chain Monte Carlo to analyze districting plans and gerrymanders
 Home-page: https://github.com/mggg/GerryChain
 Author: Metric Geometry and Gerrymandering Group
 Author-email: engineering@mggg.org
 Maintainer: Metric Geometry and Gerrymandering Group
 Maintainer-email: engineering@mggg.org
 Keywords: GerryChain
@@ -82,15 +82,15 @@
 
 Installation
 ============
 
 Supported Python Versions
 -------------------------
 
-The most recent version of GerryChain (as of February 2024) supports
+The most recent version of GerryChain (as of April 2024) supports
 
 - Python 3.9
 - Python 3.10
 - Python 3.11
 
 If you do not have one of these versions installed on you machine, we
 recommend that you go to the 
@@ -212,15 +212,15 @@
 If you plan on using GerryChain's GIS functions, such as computing
 adjacencies or reading in shapefiles, then run
 ``pip install gerrychain[geo]`` from the command line.
 
 This approach sometimes fails due to compatibility issues between our
 different Python GIS dependencies, like ``geopandas``, ``pyproj``,
 ``fiona``, and ``shapely``. If you run into this issue, try installing
-the dependencies using the `geo_settings.txt <https://github.com/mggg/GerryChain/raw/main/docs/geo_settings.txt>`_
+the dependencies using the `geo_settings.txt <https://github.com/mggg/GerryChain/tree/main/docs/geo_settings.txt>`_
 file. To do this, run ``pip install -r geo_settings.txt`` from the
 command line.
 
 .. note::
 
   If you plan on following through the tutorials present within the
   remainder of this documentation, you will also need to install
```

### Comparing `gerrychain-0.3.1/README.rst` & `gerrychain-0.3.2/README.rst`

 * *Files 1% similar despite different names*

```diff
@@ -62,15 +62,15 @@
 
 Installation
 ============
 
 Supported Python Versions
 -------------------------
 
-The most recent version of GerryChain (as of February 2024) supports
+The most recent version of GerryChain (as of April 2024) supports
 
 - Python 3.9
 - Python 3.10
 - Python 3.11
 
 If you do not have one of these versions installed on you machine, we
 recommend that you go to the 
@@ -192,15 +192,15 @@
 If you plan on using GerryChain's GIS functions, such as computing
 adjacencies or reading in shapefiles, then run
 ``pip install gerrychain[geo]`` from the command line.
 
 This approach sometimes fails due to compatibility issues between our
 different Python GIS dependencies, like ``geopandas``, ``pyproj``,
 ``fiona``, and ``shapely``. If you run into this issue, try installing
-the dependencies using the `geo_settings.txt <https://github.com/mggg/GerryChain/raw/main/docs/geo_settings.txt>`_
+the dependencies using the `geo_settings.txt <https://github.com/mggg/GerryChain/tree/main/docs/geo_settings.txt>`_
 file. To do this, run ``pip install -r geo_settings.txt`` from the
 command line.
 
 .. note::
 
   If you plan on following through the tutorials present within the
   remainder of this documentation, you will also need to install
```

### Comparing `gerrychain-0.3.1/gerrychain/__init__.py` & `gerrychain-0.3.2/gerrychain/__init__.py`

 * *Files identical despite different names*

### Comparing `gerrychain-0.3.1/gerrychain/accept.py` & `gerrychain-0.3.2/gerrychain/accept.py`

 * *Files identical despite different names*

### Comparing `gerrychain-0.3.1/gerrychain/chain.py` & `gerrychain-0.3.2/gerrychain/chain.py`

 * *Files 1% similar despite different names*

```diff
@@ -20,18 +20,17 @@
 Dependencies:
 
 - typing: Used for type hints.
 
 Last Updated: 11 Jan 2024
 """
 
-from .constraints import Validator
 from typing import Union, Iterable, Callable, Optional
 
-from gerrychain.constraints import Bounds
+from gerrychain.constraints import Validator, Bounds
 from gerrychain.partition import Partition
 
 
 class MarkovChain:
     """
     MarkovChain is a class that creates an iterator for iterating over the states
     of a Markov chain run in a gerrymandering analysis context.
@@ -50,30 +49,30 @@
     """
 
     def __init__(
         self,
         proposal: Callable,
         constraints: Union[Iterable[Callable], Validator, Iterable[Bounds], Callable],
         accept: Callable,
-        initial_state: Optional[Partition],
+        initial_state: Partition,
         total_steps: int,
     ) -> None:
         """
         :param proposal: Function proposing the next state from the current state.
         :type proposal: Callable
         :param constraints: A function with signature ``Partition -> bool`` determining whether
             the proposed next state is valid (passes all binary constraints). Usually
             this is a :class:`~gerrychain.constraints.Validator` class instance.
         :type constraints: Union[Iterable[Callable], Validator, Iterable[Bounds], Callable]
         :param accept: Function accepting or rejecting the proposed state. In the most basic
             use case, this always returns ``True``. But if the user wanted to use a
             Metropolis-Hastings acceptance rule, this is where you would implement it.
         :type accept: Callable
         :param initial_state: Initial :class:`gerrychain.partition.Partition` class.
-        :type initial_state: Optional[Partition]
+        :type initial_state: Partition
         :param total_steps: Number of steps to run.
         :type total_steps: int
 
         :returns: None
 
         :raises ValueError: If the initial_state is not valid according to the constraints.
         """
```

### Comparing `gerrychain-0.3.1/gerrychain/constraints/__init__.py` & `gerrychain-0.3.2/gerrychain/constraints/__init__.py`

 * *Files identical despite different names*

### Comparing `gerrychain-0.3.1/gerrychain/constraints/bounds.py` & `gerrychain-0.3.2/gerrychain/constraints/bounds.py`

 * *Files identical despite different names*

### Comparing `gerrychain-0.3.1/gerrychain/constraints/compactness.py` & `gerrychain-0.3.2/gerrychain/constraints/compactness.py`

 * *Files identical despite different names*

### Comparing `gerrychain-0.3.1/gerrychain/constraints/contiguity.py` & `gerrychain-0.3.2/gerrychain/constraints/contiguity.py`

 * *Files 0% similar despite different names*

```diff
@@ -151,14 +151,17 @@
     """
     flips = partition.flips
     parent = partition.parent
 
     if flips is None:
         return partition.parts
 
+    if parent is None:
+        return set(flips.values())
+
     affected = set()
     for node, part in flips.items():
         affected.add(part)
         affected.add(parent.assignment.mapping[node])
 
     return affected
```

### Comparing `gerrychain-0.3.1/gerrychain/constraints/validity.py` & `gerrychain-0.3.2/gerrychain/constraints/validity.py`

 * *Files identical despite different names*

### Comparing `gerrychain-0.3.1/gerrychain/graph/__init__.py` & `gerrychain-0.3.2/gerrychain/graph/__init__.py`

 * *Files identical despite different names*

### Comparing `gerrychain-0.3.1/gerrychain/graph/adjacency.py` & `gerrychain-0.3.2/gerrychain/graph/adjacency.py`

 * *Files identical despite different names*

### Comparing `gerrychain-0.3.1/gerrychain/graph/geo.py` & `gerrychain-0.3.2/gerrychain/graph/geo.py`

 * *Files identical despite different names*

### Comparing `gerrychain-0.3.1/gerrychain/graph/graph.py` & `gerrychain-0.3.2/gerrychain/graph/graph.py`

 * *Files 1% similar despite different names*

```diff
@@ -178,14 +178,15 @@
     def from_geodataframe(
         cls,
         dataframe: pd.DataFrame,
         adjacency: str = "rook",
         cols_to_add: Optional[List[str]] = None,
         reproject: bool = False,
         ignore_errors: bool = False,
+        crs_override: Optional[str | int] = None,
     ) -> "Graph":
         """
         Creates the adjacency :class:`Graph` of geometries described by `dataframe`.
         The areas of the polygons are included as node attributes (with key `area`).
         The shared perimeter of neighboring polygons are included as edge attributes
         (with key `shared_perim`).
         Nodes corresponding to polygons on the boundary of the union of all the geometries
@@ -210,14 +211,17 @@
         :type cols_to_add: Optional[List[str]], optional
         :param reproject: Whether to reproject to a UTM projection before
             creating the graph. Default is ``False``.
         :type reproject: bool, optional
         :param ignore_errors: Whether to ignore all invalid geometries and
             attept to create the graph anyway. Default is ``False``.
         :type ignore_errors: bool, optional
+        :param crs_override: Value to override the CRS of the GeoDataFrame.
+            Default is None.
+        :type crs_override: Optional[str | int], optional
 
         :returns: The adjacency graph of the geometries from `dataframe`.
         :rtype: Graph
         """
         # Validate geometries before reprojection
         if not ignore_errors:
             invalid = invalid_geometries(dataframe)
@@ -259,15 +263,29 @@
         add_boundary_perimeters(graph, df.geometry)
 
         # Add area data to the nodes
         areas = df.geometry.area.to_dict()
         networkx.set_node_attributes(graph, name="area", values=areas)
 
         graph.add_data(df, columns=cols_to_add)
-        graph.graph["crs"] = df.crs.to_json()
+
+        if crs_override is not None:
+            df.set_crs(crs_override, inplace=True)
+
+        if df.crs is None:
+            warnings.warn(
+                "GeoDataFrame has no CRS. Did you forget to set it? "
+                "If you're sure this is correct, you can ignore this warning. "
+                "Otherwise, please set the CRS using the `crs_override` parameter. "
+                "Attempting to proceed without a CRS."
+            )
+            graph.graph["crs"] = None
+        else:
+            graph.graph["crs"] = df.crs.to_json()
+
         return graph
 
     def lookup(self, node: Any, field: Any) -> Any:
         """
         Lookup a node/field attribute.
 
         :param node: Node to look up.
```

### Comparing `gerrychain-0.3.1/gerrychain/grid.py` & `gerrychain-0.3.2/gerrychain/grid.py`

 * *Files identical despite different names*

### Comparing `gerrychain-0.3.1/gerrychain/meta/diversity.py` & `gerrychain-0.3.2/gerrychain/meta/diversity.py`

 * *Files identical despite different names*

### Comparing `gerrychain-0.3.1/gerrychain/metagraph.py` & `gerrychain-0.3.2/gerrychain/metagraph.py`

 * *Files identical despite different names*

### Comparing `gerrychain-0.3.1/gerrychain/metrics/compactness.py` & `gerrychain-0.3.2/gerrychain/metrics/compactness.py`

 * *Files identical despite different names*

### Comparing `gerrychain-0.3.1/gerrychain/metrics/partisan.py` & `gerrychain-0.3.2/gerrychain/metrics/partisan.py`

 * *Files identical despite different names*

### Comparing `gerrychain-0.3.1/gerrychain/partition/assignment.py` & `gerrychain-0.3.2/gerrychain/partition/assignment.py`

 * *Files identical despite different names*

### Comparing `gerrychain-0.3.1/gerrychain/partition/geographic.py` & `gerrychain-0.3.2/gerrychain/partition/geographic.py`

 * *Files identical despite different names*

### Comparing `gerrychain-0.3.1/gerrychain/partition/partition.py` & `gerrychain-0.3.2/gerrychain/partition/partition.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 import json
 import networkx
 
 from gerrychain.graph.graph import FrozenGraph, Graph
 from ..updaters import compute_edge_flows, flows_from_changes, cut_edges
 from .assignment import get_assignment
 from .subgraphs import SubgraphView
+from ..tree import recursive_tree_part
 from typing import Any, Callable, Dict, Optional, Tuple
 
 
 class Partition:
     """
     Partition represents a partition of the nodes of the graph. It will perform
     the first layer of computations at each step in the Markov chain - basic
@@ -59,14 +60,69 @@
             self._first_time(graph, assignment, updaters, use_default_updaters)
         else:
             self._from_parent(parent, flips)
 
         self._cache = dict()
         self.subgraphs = SubgraphView(self.graph, self.parts)
 
+    @classmethod
+    def from_random_assignment(
+        cls,
+        graph: Graph,
+        n_parts: int,
+        epsilon: float,
+        pop_col: str,
+        updaters: Optional[Dict[str, Callable]] = None,
+        use_default_updaters: bool = True,
+        flips: Optional[Dict] = None,
+        method: Callable = recursive_tree_part,
+    ) -> "Partition":
+        """
+        Create a Partition with a random assignment of nodes to districts.
+
+        :param graph: The graph to create the Partition from.
+        :type graph: :class:`~gerrychain.Graph`
+        :param n_parts: The number of districts to divide the nodes into.
+        :type n_parts: int
+        :param epsilon: The maximum relative population deviation from the ideal
+        :type epsilon: float
+            population. Should be in [0,1].
+        :param pop_col: The column of the graph's node data that holds the population data.
+        :type pop_col: str
+        :param updaters: Dictionary of updaters
+        :type updaters: Optional[Dict[str, Callable]], optional
+        :param use_default_updaters: If `False`, do not include default updaters.
+        :type use_default_updaters: bool, optional
+        :param flips: Dictionary assigning nodes of the graph to their new districts.
+        :type flips: Optional[Dict], optional
+        :param method: The function to use to partition the graph into ``n_parts``. Defaults to
+            :func:`~gerrychain.tree.recursive_tree_part`.
+        :type method: Callable, optional
+
+        :returns: The partition created with a random assignment
+        :rtype: Partition
+        """
+        total_pop = sum(graph.nodes[n][pop_col] for n in graph)
+        ideal_pop = total_pop / n_parts
+
+        assignment = method(
+            graph=graph,
+            parts=range(n_parts),
+            pop_target=ideal_pop,
+            pop_col=pop_col,
+            epsilon=epsilon,
+        )
+
+        return cls(
+            graph,
+            assignment,
+            updaters,
+            use_default_updaters=use_default_updaters,
+        )
+
     def _first_time(self, graph, assignment, updaters, use_default_updaters):
         if isinstance(graph, Graph):
             self.graph = FrozenGraph(graph)
         elif isinstance(graph, networkx.Graph):
             graph = Graph.from_networkx(graph)
             self.graph = FrozenGraph(graph)
         elif isinstance(graph, FrozenGraph):
```

### Comparing `gerrychain-0.3.1/gerrychain/partition/subgraphs.py` & `gerrychain-0.3.2/gerrychain/partition/subgraphs.py`

 * *Files identical despite different names*

### Comparing `gerrychain-0.3.1/gerrychain/proposals/proposals.py` & `gerrychain-0.3.2/gerrychain/proposals/proposals.py`

 * *Files identical despite different names*

### Comparing `gerrychain-0.3.1/gerrychain/proposals/spectral_proposals.py` & `gerrychain-0.3.2/gerrychain/proposals/spectral_proposals.py`

 * *Files identical despite different names*

### Comparing `gerrychain-0.3.1/gerrychain/proposals/tree_proposals.py` & `gerrychain-0.3.2/gerrychain/proposals/tree_proposals.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from functools import partial
 from inspect import signature
 import random
 
 from gerrychain.partition import Partition
 from ..tree import (
-    recursive_tree_part,
+    epsilon_tree_bipartition,
     bipartition_tree,
     bipartition_tree_random,
     _bipartition_tree_random_all,
     uniform_spanning_tree,
     find_balanced_edge_cuts_memoization,
     ReselectException,
 )
@@ -115,15 +115,15 @@
                 if tuple(parts_to_merge) not in bad_district_pairs:
                     break
 
             subgraph = partition.graph.subgraph(
                 partition.parts[parts_to_merge[0]] | partition.parts[parts_to_merge[1]]
             )
 
-            flips = recursive_tree_part(
+            flips = epsilon_tree_bipartition(
                 subgraph.graph,
                 parts_to_merge,
                 pop_col=pop_col,
                 pop_target=pop_target,
                 epsilon=epsilon,
                 node_repeats=node_repeats,
                 method=method,
```

### Comparing `gerrychain-0.3.1/gerrychain/tree.py` & `gerrychain-0.3.2/gerrychain/tree.py`

 * *Files 7% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 
 Dependencies:
 
 - networkx: Used for graph data structure and algorithms.
 - random: Provides random number generation for probabilistic approaches.
 - typing: Used for type hints.
 
-Last Updated: 30 Jan 2024
+Last Updated: 25 April 2024
 """
 
 import networkx as nx
 from networkx.algorithms import tree
 
 from functools import partial
 from inspect import signature
@@ -74,17 +74,19 @@
     """
     if region_surcharge is None:
         region_surcharge = dict()
 
     for edge in graph.edges():
         weight = random.random()
         for key, value in region_surcharge.items():
+            # We surcharge edges that cross regions and those that are not in any region
             if (
                 graph.nodes[edge[0]][key] != graph.nodes[edge[1]][key]
-                and graph.nodes[edge[0]][key] is not None
+                or graph.nodes[edge[0]][key] is None
+                or graph.nodes[edge[1]][key] is None
             ):
                 weight += value
 
         graph.edges[edge]["random_weight"] = weight
 
     spanning_tree = tree.minimum_spanning_tree(
         graph, algorithm="kruskal", weight="random_weight"
@@ -182,17 +184,40 @@
         return self._degrees[node]
 
     def contract_node(self, node, parent) -> None:
         self.population[parent] += self.population[node]
         self.subsets[parent] |= self.subsets[node]
         self._degrees[parent] -= 1
 
-    def has_ideal_population(self, node) -> bool:
+    def has_ideal_population(self, node, one_sided_cut: bool = False) -> bool:
+        """
+        Checks if a node has an ideal population within the graph up to epsilon.
+
+        :param node: The node to check.
+        :type node: Any
+        :param one_sided_cut: Whether or not we are cutting off a single district. When
+            set to False, we check if the node we are cutting and the remaining graph
+            are both within epsilon of the ideal population. When set to True, we only
+            check if the node we are cutting is within epsilon of the ideal population.
+            Defaults to False.
+        :type one_sided_cut: bool, optional
+
+        :returns: True if the node has an ideal population within the graph up to epsilon.
+        :rtype: bool
+        """
+        if one_sided_cut:
+            return (
+                abs(self.population[node] - self.ideal_pop)
+                < self.epsilon * self.ideal_pop
+            )
+
         return (
-            abs(self.population[node] - self.ideal_pop) < self.epsilon * self.ideal_pop
+            abs(self.population[node] - self.ideal_pop) <= self.epsilon * self.ideal_pop
+            and abs((self.tot_pop - self.population[node]) - self.ideal_pop)
+            <= self.epsilon * self.ideal_pop
         )
 
     def __repr__(self) -> str:
         graph_info = (
             f"Graph(nodes={len(self.graph.nodes)}, edges={len(self.graph.edges)})"
         )
         return (
@@ -206,25 +231,33 @@
 
 # Tuple that is used in the find_balanced_edge_cuts function
 Cut = namedtuple("Cut", "edge weight subset")
 Cut.__new__.__defaults__ = (None, None, None)
 Cut.__doc__ = "Represents a cut in a graph."
 Cut.edge.__doc__ = "The edge where the cut is made. Defaults to None."
 Cut.weight.__doc__ = "The weight assigned to the edge (if any). Defaults to None."
-Cut.subset.__doc__ = "The (frozen) subset of nodes on one side of the cut. Defaults to None."
+Cut.subset.__doc__ = (
+    "The (frozen) subset of nodes on one side of the cut. Defaults to None."
+)
 
 
 def find_balanced_edge_cuts_contraction(
-    h: PopulatedGraph, choice: Callable = random.choice
+    h: PopulatedGraph, one_sided_cut: bool = False, choice: Callable = random.choice
 ) -> List[Cut]:
     """
     Find balanced edge cuts using contraction.
 
     :param h: The populated graph.
     :type h: PopulatedGraph
+    :param one_sided_cut: Whether or not we are cutting off a single district. When
+        set to False, we check if the node we are cutting and the remaining graph
+        are both within epsilon of the ideal population. When set to True, we only
+        check if the node we are cutting is within epsilon of the ideal population.
+        Defaults to False.
+    :type one_sided_cut: bool, optional
     :param choice: The function used to make random choices.
     :type choice: Callable, optional
 
     :returns: A list of balanced edge cuts.
     :rtype: List[Cut]
     """
 
@@ -232,21 +265,21 @@
     # BFS predecessors for iteratively contracting leaves
     pred = predecessors(h.graph, root)
 
     cuts = []
     leaves = deque(x for x in h if h.degree(x) == 1)
     while len(leaves) > 0:
         leaf = leaves.popleft()
-        if h.has_ideal_population(leaf):
+        if h.has_ideal_population(leaf, one_sided_cut=one_sided_cut):
             e = (leaf, pred[leaf])
             cuts.append(
                 Cut(
                     edge=e,
                     weight=h.graph.edges[e].get("random_weight", random.random()),
-                    subset=frozenset(h.subsets[leaf].copy())
+                    subset=frozenset(h.subsets[leaf].copy()),
                 )
             )
         # Contract the leaf:
         parent = pred[leaf]
         h.contract_node(leaf, parent)
         if h.degree(parent) == 1 and parent != root:
             leaves.append(parent)
@@ -312,26 +345,32 @@
                 for c in succ[next_node]:
                     if c not in nodes:
                         queue.append(c)
     return nodes
 
 
 def find_balanced_edge_cuts_memoization(
-    h: PopulatedGraph, choice: Callable = random.choice
+    h: PopulatedGraph, one_sided_cut: bool = False, choice: Callable = random.choice
 ) -> List[Cut]:
     """
     Find balanced edge cuts using memoization.
 
     This function takes a PopulatedGraph object and a choice function as input and returns a list
     of balanced edge cuts. A balanced edge cut is defined as a cut that divides the graph into
     two subsets, such that the population of each subset is close to the ideal population
     defined by the PopulatedGraph object.
 
     :param h: The PopulatedGraph object representing the graph.
     :type h: PopulatedGraph
+    :param one_sided_cut: Whether or not we are cutting off a single district. When
+        set to False, we check if the node we are cutting and the remaining graph
+        are both within epsilon of the ideal population. When set to True, we only
+        check if the node we are cutting is within epsilon of the ideal population.
+        Defaults to False.
+    :type one_sided_cut: bool, optional
     :param choice: The choice function used to select the root node.
     :type choice: Callable, optional
 
     :returns: A list of balanced edge cuts.
     :rtype: List[Cut]
     """
 
@@ -339,26 +378,44 @@
     pred = predecessors(h.graph, root)
     succ = successors(h.graph, root)
     total_pop = h.tot_pop
 
     subtree_pops = _calc_pops(succ, root, h)
 
     cuts = []
-    for node, tree_pop in subtree_pops.items():
-        if abs(tree_pop - h.ideal_pop) <= h.ideal_pop * h.epsilon:
-            e = (node, pred[node])
-            wt = random.random()
-            cuts.append(
-                Cut(
-                    edge=e,
-                    weight=h.graph.edges[e].get("random_weight", wt),
-                    subset=frozenset(_part_nodes(node, succ))
+
+    if one_sided_cut:
+        for node, tree_pop in subtree_pops.items():
+            if abs(tree_pop - h.ideal_pop) <= h.ideal_pop * h.epsilon:
+                e = (node, pred[node])
+                wt = random.random()
+                cuts.append(
+                    Cut(
+                        edge=e,
+                        weight=h.graph.edges[e].get("random_weight", wt),
+                        subset=frozenset(_part_nodes(node, succ)),
+                    )
                 )
-            )
-        elif abs((total_pop - tree_pop) - h.ideal_pop) <= h.ideal_pop * h.epsilon:
+            elif abs((total_pop - tree_pop) - h.ideal_pop) <= h.ideal_pop * h.epsilon:
+                e = (node, pred[node])
+                wt = random.random()
+                cuts.append(
+                    Cut(
+                        edge=e,
+                        weight=h.graph.edges[e].get("random_weight", wt),
+                        subset=frozenset(set(h.graph.nodes) - _part_nodes(node, succ)),
+                    )
+                )
+
+        return cuts
+
+    for node, tree_pop in subtree_pops.items():
+        if (abs(tree_pop - h.ideal_pop) <= h.ideal_pop * h.epsilon) and (
+            abs((total_pop - tree_pop) - h.ideal_pop) <= h.ideal_pop * h.epsilon
+        ):
             e = (node, pred[node])
             wt = random.random()
             cuts.append(
                 Cut(
                     edge=e,
                     weight=h.graph.edges[e].get("random_weight", wt),
                     subset=frozenset(set(h.graph.nodes) - _part_nodes(node, succ)),
@@ -382,17 +439,15 @@
     user has allowed the algorithm to reselect the pair of
     districts from parent graph to try and recombine.
     """
 
     pass
 
 
-def _max_weight_choice(
-    cut_edge_list: List[Cut]
-) -> Cut:
+def _max_weight_choice(cut_edge_list: List[Cut]) -> Cut:
     """
     Each Cut object in the list is assigned a random weight.
     This random weight is either assigned during the call to
     the minimum spanning tree algorithm (Kruskal's) algorithm
     or it is generated during the selection of the balanced edges
     (cf. :meth:`find_balanced_edge_cuts_memoization` and
     :meth:`find_balanced_edge_cuts_contraction`).
@@ -423,38 +478,32 @@
         return random.choice(cut_edge_list)
 
     return max(cut_edge_list, key=lambda cut: cut.weight)
 
 
 def _power_set_sorted_by_size_then_sum(d):
     power_set = [
-        s
-        for i in range(1, len(d) + 1)
-        for s in itertools.combinations(d.keys(), i)
+        s for i in range(1, len(d) + 1) for s in itertools.combinations(d.keys(), i)
     ]
 
     # Sort the subsets in descending order based on
     # the sum of their corresponding values in the dictionary
     sorted_power_set = sorted(
-        power_set,
-        key=lambda s: (len(s), sum(d[i] for i in s)),
-        reverse=True
+        power_set, key=lambda s: (len(s), sum(d[i] for i in s)), reverse=True
     )
 
     return sorted_power_set
 
 
 # Note that the populated graph and the region surcharge are passed
 # by object reference. This means that a copy is not made since we
 # are not modifying the object in the function, and the speed of
 # this randomized selection will not suffer for it.
 def _region_preferred_max_weight_choice(
-    populated_graph: PopulatedGraph,
-    region_surcharge: Dict,
-    cut_edge_list: List[Cut]
+    populated_graph: PopulatedGraph, region_surcharge: Dict, cut_edge_list: List[Cut]
 ) -> Cut:
     """
     This function is used in the case of a region-aware chain. It
     is similar to the as :meth:`_max_weight_choice` function except
     that it will preferentially select one of the cuts that has the
     highest surcharge. So, if we have a weight dict of the form
     ``{region1: wt1, region2: wt2}`` , then this function first looks
@@ -498,27 +547,30 @@
     # Early return for simple cases
     if len(region_surcharge) < 1 or len(region_surcharge) > 3:
         return _max_weight_choice(cut_edge_list)
 
     # Prepare data for efficient access
     edge_region_info = {
         cut: {
-            key: (populated_graph.graph.nodes[cut.edge[0]].get(key),
-                  populated_graph.graph.nodes[cut.edge[1]].get(key))
+            key: (
+                populated_graph.graph.nodes[cut.edge[0]].get(key),
+                populated_graph.graph.nodes[cut.edge[1]].get(key),
+            )
             for key in region_surcharge
         }
         for cut in cut_edge_list
     }
 
     # Generate power set sorted by surcharge, then filter cuts based
     # on region matching
     power_set = _power_set_sorted_by_size_then_sum(region_surcharge)
     for region_combination in power_set:
         suitable_cuts = [
-            cut for cut in cut_edge_list
+            cut
+            for cut in cut_edge_list
             if all(
                 edge_region_info[cut][key][0] != edge_region_info[cut][key][1]
                 for key in region_combination
             )
         ]
         if suitable_cuts:
             return _max_weight_choice(suitable_cuts)
@@ -532,19 +584,20 @@
     pop_target: Union[int, float],
     epsilon: float,
     node_repeats: int = 1,
     spanning_tree: Optional[nx.Graph] = None,
     spanning_tree_fn: Callable = random_spanning_tree,
     region_surcharge: Optional[Dict] = None,
     balance_edge_fn: Callable = find_balanced_edge_cuts_memoization,
+    one_sided_cut: bool = False,
     choice: Callable = random.choice,
     max_attempts: Optional[int] = 100000,
     warn_attempts: int = 1000,
     allow_pair_reselection: bool = False,
-    cut_choice: Callable = _region_preferred_max_weight_choice
+    cut_choice: Callable = _region_preferred_max_weight_choice,
 ) -> Set:
     """
     This function finds a balanced 2 partition of a graph by drawing a
     spanning tree and finding an edge to cut that leaves at most an epsilon
     imbalance between the populations of the parts. If a root fails, new roots
     are tried until node_repeats in which case a new tree is drawn.
 
@@ -571,14 +624,21 @@
     :type spanning_tree_fn: Callable, optional
     :param region_surcharge: A dictionary of surcharges for the spanning tree algorithm.
         Defaults to None.
     :type region_surcharge: Optional[Dict], optional
     :param balance_edge_fn: The function to find balanced edge cuts. Defaults to
         :func:`find_balanced_edge_cuts_memoization`.
     :type balance_edge_fn: Callable, optional
+    :param one_sided_cut: Passed to the ``balance_edge_fn``. Determines whether or not we are
+        cutting off a single district when partitioning the tree. When
+        set to False, we check if the node we are cutting and the remaining graph
+        are both within epsilon of the ideal population. When set to True, we only
+        check if the node we are cutting is within epsilon of the ideal population.
+        Defaults to False.
+    :type one_sided_cut: bool, optional
     :param choice: The function to make a random choice of root node for the population
         tree. Passed to ``balance_edge_fn``. Can be substituted for testing.
         Defaults to :func:`random.random()`.
     :type choice: Callable, optional
     :param max_attempts: The maximum number of attempts that should be made to bipartition.
         Defaults to 10000.
     :type max_attempts: Optional[int], optional
@@ -600,14 +660,17 @@
     :raises RuntimeError: If a possible cut cannot be found after the maximum number of attempts
         given by ``max_attempts``.
     """
     # Try to add the region-aware in if the spanning_tree_fn accepts a surcharge dictionary
     if "region_surcharge" in signature(spanning_tree_fn).parameters:
         spanning_tree_fn = partial(spanning_tree_fn, region_surcharge=region_surcharge)
 
+    if "one_sided_cut" in signature(balance_edge_fn).parameters:
+        balance_edge_fn = partial(balance_edge_fn, one_sided_cut=one_sided_cut)
+
     populations = {node: graph.nodes[node][pop_col] for node in graph.node_indices}
 
     possible_cuts: List[Cut] = []
     if spanning_tree is None:
         spanning_tree = spanning_tree_fn(graph)
 
     restarts = 0
@@ -738,14 +801,15 @@
     pop_target: Union[int, float],
     epsilon: float,
     node_repeats: int = 1,
     repeat_until_valid: bool = True,
     spanning_tree: Optional[nx.Graph] = None,
     spanning_tree_fn: Callable = random_spanning_tree,
     balance_edge_fn: Callable = find_balanced_edge_cuts_memoization,
+    one_sided_cut: bool = False,
     choice: Callable = random.choice,
     max_attempts: Optional[int] = 100000,
 ) -> Union[Set[Any], None]:
     """
     This is like :func:`bipartition_tree` except it chooses a random balanced
     cut, rather than the first cut it finds.
 
@@ -753,22 +817,22 @@
     spanning tree and finding an edge to cut that leaves at most an epsilon
     imbalance between the populations of the parts. If a root fails, new roots
     are tried until node_repeats in which case a new tree is drawn.
 
     Builds up a connected subgraph with a connected complement whose population
     is ``epsilon * pop_target`` away from ``pop_target``.
 
-    :param graph: The graph to partition
+    :param graph: The graph to partition.
     :type graph: nx.Graph
-    :param pop_col: The node attribute holding the population of each node
+    :param pop_col: The node attribute holding the population of each node.
     :type pop_col: str
-    :param pop_target: The target population for the returned subset of nodes
+    :param pop_target: The target population for the returned subset of nodes.
     :type pop_target: Union[int, float]
     :param epsilon: The allowable deviation from  ``pop_target`` (as a percentage of
-        ``pop_target``) for the subgraph's population
+        ``pop_target``) for the subgraph's population.
     :type epsilon: float
     :param node_repeats: A parameter for the algorithm: how many different choices
         of root to use before drawing a new spanning tree. Defaults to 1.
     :type node_repeats: int
     :param repeat_until_valid: Determines whether to keep drawing spanning trees
         until a tree with a balanced cut is found. If `True`, a set of nodes will
         always be returned; if `False`, `None` will be returned if a valid spanning
@@ -779,25 +843,35 @@
     :type spanning_tree: Optional[nx.Graph], optional
     :param spanning_tree_fn: The random spanning tree algorithm to use if a spanning
         tree is not provided. Defaults to :func:`random_spanning_tree`.
     :type spanning_tree_fn: Callable, optional
     :param balance_edge_fn: The algorithm used to find balanced cut edges. Defaults to
         :func:`find_balanced_edge_cuts_memoization`.
     :type balance_edge_fn: Callable, optional
+    :param one_sided_cut: Passed to the ``balance_edge_fn``. Determines whether or not we are
+        cutting off a single district when partitioning the tree. When
+        set to False, we check if the node we are cutting and the remaining graph
+        are both within epsilon of the ideal population. When set to True, we only
+        check if the node we are cutting is within epsilon of the ideal population.
+        Defaults to False.
+    :type one_sided_cut: bool, optional
     :param choice: The random choice function. Can be substituted for testing. Defaults
         to :func:`random.choice`.
     :type choice: Callable, optional
     :param max_attempts: The max number of attempts that should be made to bipartition.
         Defaults to None.
     :type max_attempts: Optional[int], optional
 
     :returns: A subset of nodes of ``graph`` (whose induced subgraph is connected) or None if a
         valid spanning tree is not found.
     :rtype: Union[Set[Any], None]
     """
+    if "one_sided_cut" in signature(balance_edge_fn).parameters:
+        balance_edge_fn = partial(balance_edge_fn, one_sided_cut=True)
+
     possible_cuts = _bipartition_tree_random_all(
         graph=graph,
         pop_col=pop_col,
         pop_target=pop_target,
         epsilon=epsilon,
         node_repeats=node_repeats,
         repeat_until_valid=repeat_until_valid,
@@ -807,38 +881,121 @@
         choice=choice,
         max_attempts=max_attempts,
     )
     if possible_cuts:
         return choice(possible_cuts).subset
 
 
+def epsilon_tree_bipartition(
+    graph: nx.Graph,
+    parts: Sequence,
+    pop_target: Union[float, int],
+    pop_col: str,
+    epsilon: float,
+    node_repeats: int = 1,
+    method: Callable = partial(bipartition_tree, max_attempts=10000),
+) -> Dict:
+    """
+    Uses :func:`~gerrychain.tree.bipartition_tree` to partition a tree into
+    two parts of population ``pop_target`` (within ``epsilon``).
+
+    :param graph: The graph to partition into two :math:`\varepsilon`-balanced parts.
+    :type graph: nx.Graph
+    :param parts: Iterable of part (district) labels (like ``[0,1,2]`` or ``range(4)``).
+    :type parts: Sequence
+    :param pop_target: Target population for each part of the partition.
+    :type pop_target: Union[float, int]
+    :param pop_col: Node attribute key holding population data.
+    :type pop_col: str
+    :param epsilon: How far (as a percentage of ``pop_target``) from ``pop_target`` the parts
+        of the partition can be.
+    :type epsilon: float
+    :param node_repeats: Parameter for :func:`~gerrychain.tree_methods.bipartition_tree` to use.
+        Defaults to 1.
+    :type node_repeats: int, optional
+    :param method: The partition method to use. Defaults to
+        `partial(bipartition_tree, max_attempts=10000)`.
+    :type method: Callable, optional
+
+    :returns: New assignments for the nodes of ``graph``.
+    :rtype: dict
+    """
+    if len(parts) != 2:
+        raise ValueError(
+            "This function only supports bipartitioning. Please ensure that there"
+            + " are exactly 2 parts in the parts list."
+        )
+
+    flips = {}
+    remaining_nodes = graph.node_indices
+
+    lb_pop = pop_target * (1 - epsilon)
+    ub_pop = pop_target * (1 + epsilon)
+    check_pop = lambda x: lb_pop <= x <= ub_pop
+
+    nodes = method(
+        graph.subgraph(remaining_nodes),
+        pop_col=pop_col,
+        pop_target=pop_target,
+        epsilon=epsilon,
+        node_repeats=node_repeats,
+        one_sided_cut=False,
+    )
+
+    if nodes is None:
+        raise BalanceError()
+
+    part_pop = 0
+    for node in nodes:
+        flips[node] = parts[-2]
+        part_pop += graph.nodes[node][pop_col]
+
+    if not check_pop(part_pop):
+        raise PopulationBalanceError()
+
+    remaining_nodes -= nodes
+
+    # All of the remaining nodes go in the last part
+    part_pop = 0
+    for node in remaining_nodes:
+        flips[node] = parts[-1]
+        part_pop += graph.nodes[node][pop_col]
+
+    if not check_pop(part_pop):
+        raise PopulationBalanceError()
+
+    return flips
+
+
+# TODO: Move these recursive partition functions to their own module. They are not
+# central to the operation of the recom function despite being tree methods.
 def recursive_tree_part(
     graph: nx.Graph,
     parts: Sequence,
     pop_target: Union[float, int],
     pop_col: str,
     epsilon: float,
     node_repeats: int = 1,
     method: Callable = partial(bipartition_tree, max_attempts=10000),
 ) -> Dict:
     """
     Uses :func:`~gerrychain.tree.bipartition_tree` recursively to partition a tree into
     ``len(parts)`` parts of population ``pop_target`` (within ``epsilon``). Can be used to
     generate initial seed plans or to implement ReCom-like "merge walk" proposals.
 
-    :param graph: The graph
+    :param graph: The graph to partition into ``len(parts)`` :math:`\varepsilon`-balanced parts.
     :type graph: nx.Graph
-    :param parts: Iterable of part labels (like ``[0,1,2]`` or ``range(4)``)
+    :param parts: Iterable of part (district) labels (like ``[0,1,2]`` or ``range(4)``).
     :type parts: Sequence
-    :param pop_target: Target population for each part of the partition
+    :param pop_target: Target population for each part of the partition.
     :type pop_target: Union[float, int]
-    :param pop_col: Node attribute key holding population data
+    :param pop_col: Node attribute key holding population data.
     :type pop_col: str
     :param epsilon: How far (as a percentage of ``pop_target``) from ``pop_target`` the parts
-        of the partition can be
+        of the partition can be.
     :type epsilon: float
     :param node_repeats: Parameter for :func:`~gerrychain.tree_methods.bipartition_tree` to use.
         Defaluts to 1.
     :type node_repeats: int, optional
     :param method: The partition method to use. Defaults to
         `partial(bipartition_tree, max_attempts=10000)`.
     :type method: Callable, optional
@@ -853,44 +1010,81 @@
     # basis such that every partition, including the last partition, has a
     # population within +/-``epsilon`` of the target population.
     # For instance, if district n's population exceeds the target by 2%
     # with a +/-2% epsilon, then district n+1's population should be between
     # 98% of the target population and the target population.
     debt: Union[int, float] = 0
 
-    for part in parts[:-1]:
+    lb_pop = pop_target * (1 - epsilon)
+    ub_pop = pop_target * (1 + epsilon)
+    check_pop = lambda x: lb_pop <= x <= ub_pop
+
+    for part in parts[:-2]:
         min_pop = max(pop_target * (1 - epsilon), pop_target * (1 - epsilon) - debt)
         max_pop = min(pop_target * (1 + epsilon), pop_target * (1 + epsilon) - debt)
         new_pop_target = (min_pop + max_pop) / 2
 
         try:
             nodes = method(
                 graph.subgraph(remaining_nodes),
                 pop_col=pop_col,
                 pop_target=new_pop_target,
                 epsilon=(max_pop - min_pop) / (2 * new_pop_target),
                 node_repeats=node_repeats,
+                one_sided_cut=True,
             )
         except Exception:
             raise
 
         if nodes is None:
             raise BalanceError()
 
         part_pop = 0
         for node in nodes:
             flips[node] = part
             part_pop += graph.nodes[node][pop_col]
 
+        if not check_pop(part_pop):
+            raise PopulationBalanceError()
+
         debt += part_pop - pop_target
         remaining_nodes -= nodes
 
+    # After making n-2 districts, we need to make sure that the last
+    # two districts are both balanced.
+    nodes = method(
+        graph.subgraph(remaining_nodes),
+        pop_col=pop_col,
+        pop_target=pop_target,
+        epsilon=epsilon,
+        node_repeats=node_repeats,
+        one_sided_cut=False,
+    )
+
+    if nodes is None:
+        raise BalanceError()
+
+    part_pop = 0
+    for node in nodes:
+        flips[node] = parts[-2]
+        part_pop += graph.nodes[node][pop_col]
+
+    if not check_pop(part_pop):
+        raise PopulationBalanceError()
+
+    remaining_nodes -= nodes
+
     # All of the remaining nodes go in the last part
+    part_pop = 0
     for node in remaining_nodes:
         flips[node] = parts[-1]
+        part_pop += graph.nodes[node][pop_col]
+
+    if not check_pop(part_pop):
+        raise PopulationBalanceError()
 
     return flips
 
 
 def get_seed_chunks(
     graph: nx.Graph,
     num_chunks: int,
@@ -999,15 +1193,15 @@
 
     return list(chunks.values())
 
 
 def get_max_prime_factor_less_than(n: int, ceil: int) -> Optional[int]:
     """
     Helper function for recursive_seed_part_inner. Returns the largest prime factor of ``n``
-        less than ``ceil``, or None if all are greater than ceil.
+    less than ``ceil``, or None if all are greater than ceil.
 
     :param n: The number to find the largest prime factor for.
     :type n: int
     :param ceil: The upper limit for the largest prime factor.
     :type ceil: int
 
     :returns: The largest prime factor of ``n`` less than ``ceil``, or None if all are greater
@@ -1091,15 +1285,15 @@
     :param ceil: Either a positive integer (at least 2) or None. Relevant only if n is None.
         If ``ceil`` is a positive integer then finds the largest factor of ``num_dists`` less
         than or equal to ``ceil``, and recursively splits graph into that number of chunks, or
         bites off a district if that number is 1. Defaults to None.
     :type ceil: Optional[int], optional
 
     :returns: New assignments for the nodes of ``graph``.
-    :rtype: List of lists, each list is a district
+    :rtype: List of sets, each set is a district
     """
 
     # Chooses num_chunks
     if n is None:
         if ceil is None:
             num_chunks = get_max_prime_factor_less_than(num_dists, num_dists)
         elif ceil >= 2:
@@ -1111,23 +1305,36 @@
     else:
         raise ValueError("n must be None or a positive integer")
 
     # base case
     if num_dists == 1:
         return [set(graph.nodes)]
 
+    if num_dists == 2:
+        nodes = method(
+            graph,
+            pop_col=pop_col,
+            pop_target=pop_target,
+            epsilon=epsilon,
+            node_repeats=node_repeats,
+            one_sided_cut=False,
+        )
+
+        return [set(nodes), set(graph.nodes) - set(nodes)]
+
     # bite off a district and recurse into the remaining subgraph
     elif num_chunks is None or num_dists % num_chunks != 0:
         remaining_nodes = set(graph.nodes)
         nodes = method(
             graph.subgraph(remaining_nodes),
             pop_col=pop_col,
             pop_target=pop_target,
             epsilon=epsilon,
             node_repeats=node_repeats,
+            one_sided_cut=True,
         )
         remaining_nodes -= nodes
         assignment = [nodes] + recursive_seed_part_inner(
             graph.subgraph(remaining_nodes),
             num_dists - 1,
             pop_target,
             pop_col,
@@ -1136,15 +1343,21 @@
             n=n,
             ceil=ceil,
         )
 
     # split graph into num_chunks chunks, and recurse into each chunk
     elif num_dists % num_chunks == 0:
         chunks = get_seed_chunks(
-            graph, num_chunks, num_dists, pop_target, pop_col, epsilon, method=method
+            graph,
+            num_chunks,
+            num_dists,
+            pop_target,
+            pop_col,
+            epsilon,
+            method=partial(method, one_sided_cut=True),
         )
 
         assignment = []
         for chunk in chunks:
             chunk_assignment = recursive_seed_part_inner(
                 graph.subgraph(chunk),
                 num_dists // num_chunks,
@@ -1223,7 +1436,11 @@
         for node in assignment[i]:
             flips[node] = parts[i]
     return flips
 
 
 class BalanceError(Exception):
     """Raised when a balanced cut cannot be found."""
+
+
+class PopulationBalanceError(Exception):
+    """Raised when the population of a district is outside the acceptable epsilon range."""
```

### Comparing `gerrychain-0.3.1/gerrychain/updaters/__init__.py` & `gerrychain-0.3.2/gerrychain/updaters/__init__.py`

 * *Files identical despite different names*

### Comparing `gerrychain-0.3.1/gerrychain/updaters/compactness.py` & `gerrychain-0.3.2/gerrychain/updaters/compactness.py`

 * *Files identical despite different names*

### Comparing `gerrychain-0.3.1/gerrychain/updaters/county_splits.py` & `gerrychain-0.3.2/gerrychain/updaters/county_splits.py`

 * *Files identical despite different names*

### Comparing `gerrychain-0.3.1/gerrychain/updaters/cut_edges.py` & `gerrychain-0.3.2/gerrychain/updaters/cut_edges.py`

 * *Files identical despite different names*

### Comparing `gerrychain-0.3.1/gerrychain/updaters/election.py` & `gerrychain-0.3.2/gerrychain/updaters/election.py`

 * *Files identical despite different names*

### Comparing `gerrychain-0.3.1/gerrychain/updaters/flows.py` & `gerrychain-0.3.2/gerrychain/updaters/flows.py`

 * *Files identical despite different names*

### Comparing `gerrychain-0.3.1/gerrychain/updaters/locality_split_scores.py` & `gerrychain-0.3.2/gerrychain/updaters/locality_split_scores.py`

 * *Files identical despite different names*

### Comparing `gerrychain-0.3.1/gerrychain/updaters/spanning_trees.py` & `gerrychain-0.3.2/gerrychain/updaters/spanning_trees.py`

 * *Files identical despite different names*

### Comparing `gerrychain-0.3.1/gerrychain/updaters/tally.py` & `gerrychain-0.3.2/gerrychain/updaters/tally.py`

 * *Files identical despite different names*

### Comparing `gerrychain-0.3.1/gerrychain/vendor/utm/conversion.py` & `gerrychain-0.3.2/gerrychain/vendor/utm/conversion.py`

 * *Files identical despite different names*

### Comparing `gerrychain-0.3.1/gerrychain.egg-info/PKG-INFO` & `gerrychain-0.3.2/gerrychain.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gerrychain
-Version: 0.3.1
+Version: 0.3.2
 Summary: Use Markov chain Monte Carlo to analyze districting plans and gerrymanders
 Home-page: https://github.com/mggg/GerryChain
 Author: Metric Geometry and Gerrymandering Group
 Author-email: engineering@mggg.org
 Maintainer: Metric Geometry and Gerrymandering Group
 Maintainer-email: engineering@mggg.org
 Keywords: GerryChain
@@ -82,15 +82,15 @@
 
 Installation
 ============
 
 Supported Python Versions
 -------------------------
 
-The most recent version of GerryChain (as of February 2024) supports
+The most recent version of GerryChain (as of April 2024) supports
 
 - Python 3.9
 - Python 3.10
 - Python 3.11
 
 If you do not have one of these versions installed on you machine, we
 recommend that you go to the 
@@ -212,15 +212,15 @@
 If you plan on using GerryChain's GIS functions, such as computing
 adjacencies or reading in shapefiles, then run
 ``pip install gerrychain[geo]`` from the command line.
 
 This approach sometimes fails due to compatibility issues between our
 different Python GIS dependencies, like ``geopandas``, ``pyproj``,
 ``fiona``, and ``shapely``. If you run into this issue, try installing
-the dependencies using the `geo_settings.txt <https://github.com/mggg/GerryChain/raw/main/docs/geo_settings.txt>`_
+the dependencies using the `geo_settings.txt <https://github.com/mggg/GerryChain/tree/main/docs/geo_settings.txt>`_
 file. To do this, run ``pip install -r geo_settings.txt`` from the
 command line.
 
 .. note::
 
   If you plan on following through the tutorials present within the
   remainder of this documentation, you will also need to install
```

### Comparing `gerrychain-0.3.1/gerrychain.egg-info/SOURCES.txt` & `gerrychain-0.3.2/gerrychain.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -26,14 +26,17 @@
 gerrychain/graph/geo.py
 gerrychain/graph/graph.py
 gerrychain/meta/__init__.py
 gerrychain/meta/diversity.py
 gerrychain/metrics/__init__.py
 gerrychain/metrics/compactness.py
 gerrychain/metrics/partisan.py
+gerrychain/optimization/__init__.py
+gerrychain/optimization/gingleator.py
+gerrychain/optimization/optimization.py
 gerrychain/partition/__init__.py
 gerrychain/partition/assignment.py
 gerrychain/partition/geographic.py
 gerrychain/partition/partition.py
 gerrychain/partition/subgraphs.py
 gerrychain/proposals/__init__.py
 gerrychain/proposals/proposals.py
```

### Comparing `gerrychain-0.3.1/setup.cfg` & `gerrychain-0.3.2/setup.cfg`

 * *Files identical despite different names*

### Comparing `gerrychain-0.3.1/setup.py` & `gerrychain-0.3.2/setup.py`

 * *Files identical despite different names*

### Comparing `gerrychain-0.3.1/versioneer.py` & `gerrychain-0.3.2/versioneer.py`

 * *Files identical despite different names*

