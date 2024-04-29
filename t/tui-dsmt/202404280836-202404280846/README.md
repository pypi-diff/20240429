# Comparing `tmp/tui_dsmt-202404280836.tar.gz` & `tmp/tui_dsmt-202404280846.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tui_dsmt-202404280836.tar", last modified: Sun Apr 28 08:36:08 2024, max compression
+gzip compressed data, was "tui_dsmt-202404280846.tar", last modified: Sun Apr 28 08:46:09 2024, max compression
```

## Comparing `tui_dsmt-202404280836.tar` & `tui_dsmt-202404280846.tar`

### file list

```diff
@@ -1,65 +1,65 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-28 08:36:08.281006 tui_dsmt-202404280836/
--rw-r--r--   0 root         (0) root         (0)      835 2024-04-28 08:36:08.281006 tui_dsmt-202404280836/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)       38 2024-04-28 08:36:08.285006 tui_dsmt-202404280836/setup.cfg
--rwxrwxrwx   0 root         (0) root         (0)     1237 2024-04-25 10:30:29.000000 tui_dsmt-202404280836/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-28 08:36:08.257005 tui_dsmt-202404280836/src/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-28 08:36:08.257005 tui_dsmt-202404280836/src/tui_dsmt/
--rw-rw-rw-   0 root         (0) root         (0)      780 2024-04-25 10:30:29.000000 tui_dsmt-202404280836/src/tui_dsmt/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-28 08:36:08.261005 tui_dsmt-202404280836/src/tui_dsmt/clustering/
--rw-rw-rw-   0 root         (0) root         (0)     5223 2024-04-25 10:30:29.000000 tui_dsmt-202404280836/src/tui_dsmt/clustering/PAM.py
--rw-rw-rw-   0 root         (0) root         (0)      309 2024-04-25 10:30:29.000000 tui_dsmt-202404280836/src/tui_dsmt/clustering/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     2691 2024-04-25 10:30:29.000000 tui_dsmt-202404280836/src/tui_dsmt/clustering/animation.py
--rw-rw-rw-   0 root         (0) root         (0)    19467 2024-04-25 10:30:29.000000 tui_dsmt-202404280836/src/tui_dsmt/clustering/datasets.py
--rw-rw-rw-   0 root         (0) root         (0)      260 2024-04-25 10:30:29.000000 tui_dsmt-202404280836/src/tui_dsmt/clustering/draw.py
--rw-rw-rw-   0 root         (0) root         (0)     2141 2024-04-28 07:42:19.000000 tui_dsmt-202404280836/src/tui_dsmt/clustering/evaluation.py
--rw-rw-rw-   0 root         (0) root         (0)     4488 2024-04-25 10:30:29.000000 tui_dsmt-202404280836/src/tui_dsmt/clustering/hierarchical.py
--rw-rw-rw-   0 root         (0) root         (0)      945 2024-04-25 10:30:29.000000 tui_dsmt-202404280836/src/tui_dsmt/clustering/interactive.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-28 08:36:08.265005 tui_dsmt-202404280836/src/tui_dsmt/fpm/
--rw-rw-rw-   0 root         (0) root         (0)    14098 2024-04-25 10:30:29.000000 tui_dsmt-202404280836/src/tui_dsmt/fpm/BruteForceFI.py
--rw-rw-rw-   0 root         (0) root         (0)     4055 2024-04-25 10:30:29.000000 tui_dsmt-202404280836/src/tui_dsmt/fpm/ConditionalFPTree.py
--rw-rw-rw-   0 root         (0) root         (0)     5837 2024-04-25 10:30:29.000000 tui_dsmt-202404280836/src/tui_dsmt/fpm/ConditionalPatternBase.py
--rw-rw-rw-   0 root         (0) root         (0)    11867 2024-04-25 10:30:29.000000 tui_dsmt-202404280836/src/tui_dsmt/fpm/FPTree.py
--rw-rw-rw-   0 root         (0) root         (0)    18908 2024-04-25 10:30:29.000000 tui_dsmt-202404280836/src/tui_dsmt/fpm/HashTree.py
--rw-rw-rw-   0 root         (0) root         (0)     1462 2024-04-25 10:30:29.000000 tui_dsmt-202404280836/src/tui_dsmt/fpm/Itemset.py
--rw-rw-rw-   0 root         (0) root         (0)     3036 2024-04-25 10:30:29.000000 tui_dsmt-202404280836/src/tui_dsmt/fpm/ItemsetGrid.py
--rw-rw-rw-   0 root         (0) root         (0)     5942 2024-04-25 10:30:29.000000 tui_dsmt-202404280836/src/tui_dsmt/fpm/ItemsetGridApriori.py
--rw-rw-rw-   0 root         (0) root         (0)     5865 2024-04-25 10:30:29.000000 tui_dsmt-202404280836/src/tui_dsmt/fpm/ItemsetGridECLAT.py
--rw-rw-rw-   0 root         (0) root         (0)     1262 2024-04-28 07:42:19.000000 tui_dsmt-202404280836/src/tui_dsmt/fpm/SequentialDatabase.py
--rw-rw-rw-   0 root         (0) root         (0)     1129 2024-04-25 10:30:29.000000 tui_dsmt-202404280836/src/tui_dsmt/fpm/SequentialItemset.py
--rw-rw-rw-   0 root         (0) root         (0)     1181 2024-04-25 10:30:29.000000 tui_dsmt-202404280836/src/tui_dsmt/fpm/TransactionDatabase.py
--rw-rw-rw-   0 root         (0) root         (0)   112423 2024-04-28 07:42:19.000000 tui_dsmt-202404280836/src/tui_dsmt/fpm/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-28 08:36:08.277006 tui_dsmt-202404280836/src/tui_dsmt/graph/
--rw-rw-rw-   0 root         (0) root         (0)     3894 2024-04-25 10:30:29.000000 tui_dsmt-202404280836/src/tui_dsmt/graph/BFS.py
--rw-rw-rw-   0 root         (0) root         (0)     1585 2024-04-25 10:30:29.000000 tui_dsmt-202404280836/src/tui_dsmt/graph/BipartiteFlow.py
--rw-rw-rw-   0 root         (0) root         (0)     3478 2024-04-25 10:30:29.000000 tui_dsmt-202404280836/src/tui_dsmt/graph/DFS.py
--rw-rw-rw-   0 root         (0) root         (0)     5843 2024-04-25 10:30:29.000000 tui_dsmt-202404280836/src/tui_dsmt/graph/Dijkstra.py
--rw-rw-rw-   0 root         (0) root         (0)      175 2024-04-25 10:30:29.000000 tui_dsmt-202404280836/src/tui_dsmt/graph/EdmondsKarp.py
--rw-rw-rw-   0 root         (0) root         (0)     4747 2024-04-25 10:30:29.000000 tui_dsmt-202404280836/src/tui_dsmt/graph/FordFulkerson.py
--rw-rw-rw-   0 root         (0) root         (0)     4461 2024-04-25 10:30:29.000000 tui_dsmt-202404280836/src/tui_dsmt/graph/Hall.py
--rw-rw-rw-   0 root         (0) root         (0)     2095 2024-04-25 10:30:29.000000 tui_dsmt-202404280836/src/tui_dsmt/graph/InteractiveGraph.py
--rw-rw-rw-   0 root         (0) root         (0)     3142 2024-04-25 10:30:29.000000 tui_dsmt-202404280836/src/tui_dsmt/graph/Kruskal.py
--rw-rw-rw-   0 root         (0) root         (0)     4877 2024-04-25 10:30:29.000000 tui_dsmt-202404280836/src/tui_dsmt/graph/LabelPropagation.py
--rw-rw-rw-   0 root         (0) root         (0)       39 2024-04-25 10:30:29.000000 tui_dsmt-202404280836/src/tui_dsmt/graph/MarkovClusterAlgorithm.py
--rw-rw-rw-   0 root         (0) root         (0)     2234 2024-04-25 10:30:29.000000 tui_dsmt-202404280836/src/tui_dsmt/graph/MaximumFlow.py
--rw-rw-rw-   0 root         (0) root         (0)     2705 2024-04-25 10:30:29.000000 tui_dsmt-202404280836/src/tui_dsmt/graph/RandomWalk.py
--rw-rw-rw-   0 root         (0) root         (0)   420228 2024-04-25 10:30:29.000000 tui_dsmt-202404280836/src/tui_dsmt/graph/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     5267 2024-04-25 10:30:29.000000 tui_dsmt-202404280836/src/tui_dsmt/graph/game.py
--rw-rw-rw-   0 root         (0) root         (0)     5766 2024-04-25 10:30:29.000000 tui_dsmt-202404280836/src/tui_dsmt/graph/html.py
--rw-rw-rw-   0 root         (0) root         (0)      870 2024-04-25 10:30:29.000000 tui_dsmt-202404280836/src/tui_dsmt/graph/representation.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-28 08:36:08.277006 tui_dsmt-202404280836/src/tui_dsmt/jpanim/
--rw-rw-rw-   0 root         (0) root         (0)     2935 2024-04-25 10:30:29.000000 tui_dsmt-202404280836/src/tui_dsmt/jpanim/JupyterAnimation.py
--rw-rw-rw-   0 root         (0) root         (0)       47 2024-04-25 10:30:29.000000 tui_dsmt-202404280836/src/tui_dsmt/jpanim/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-28 08:36:08.281006 tui_dsmt-202404280836/src/tui_dsmt/jpanim/resources/
--rw-rw-rw-   0 root         (0) root         (0)     2002 2024-04-25 10:30:29.000000 tui_dsmt-202404280836/src/tui_dsmt/jpanim/resources/controls-ff.html
--rw-rw-rw-   0 root         (0) root         (0)      797 2024-04-25 10:30:29.000000 tui_dsmt-202404280836/src/tui_dsmt/jpanim/resources/controls.html
--rw-rw-rw-   0 root         (0) root         (0)      743 2024-04-25 10:30:29.000000 tui_dsmt-202404280836/src/tui_dsmt/jpanim/resources/script.js
--rw-rw-rw-   0 root         (0) root         (0)      193 2024-04-25 10:30:29.000000 tui_dsmt-202404280836/src/tui_dsmt/jpanim/resources/style.css
--rw-rw-rw-   0 root         (0) root         (0)   147897 2024-04-25 10:30:29.000000 tui_dsmt-202404280836/src/tui_dsmt/jpanim/resources/vue-3.4.24.js
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-28 08:36:08.281006 tui_dsmt-202404280836/src/tui_dsmt/util/
--rw-rw-rw-   0 root         (0) root         (0)       92 2024-04-25 10:30:29.000000 tui_dsmt-202404280836/src/tui_dsmt/util/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-28 08:36:08.281006 tui_dsmt-202404280836/src/tui_dsmt.egg-info/
--rw-r--r--   0 root         (0) root         (0)      835 2024-04-28 08:36:08.000000 tui_dsmt-202404280836/src/tui_dsmt.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1828 2024-04-28 08:36:08.000000 tui_dsmt-202404280836/src/tui_dsmt.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-04-28 08:36:08.000000 tui_dsmt-202404280836/src/tui_dsmt.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      162 2024-04-28 08:36:08.000000 tui_dsmt-202404280836/src/tui_dsmt.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        9 2024-04-28 08:36:08.000000 tui_dsmt-202404280836/src/tui_dsmt.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-28 08:46:09.824292 tui_dsmt-202404280846/
+-rw-r--r--   0 root         (0) root         (0)      835 2024-04-28 08:46:09.824292 tui_dsmt-202404280846/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)       38 2024-04-28 08:46:09.824292 tui_dsmt-202404280846/setup.cfg
+-rwxrwxrwx   0 root         (0) root         (0)     1237 2024-04-25 10:30:29.000000 tui_dsmt-202404280846/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-28 08:46:09.808292 tui_dsmt-202404280846/src/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-28 08:46:09.808292 tui_dsmt-202404280846/src/tui_dsmt/
+-rw-rw-rw-   0 root         (0) root         (0)      780 2024-04-25 10:30:29.000000 tui_dsmt-202404280846/src/tui_dsmt/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-28 08:46:09.812292 tui_dsmt-202404280846/src/tui_dsmt/clustering/
+-rw-rw-rw-   0 root         (0) root         (0)     5223 2024-04-25 10:30:29.000000 tui_dsmt-202404280846/src/tui_dsmt/clustering/PAM.py
+-rw-rw-rw-   0 root         (0) root         (0)      309 2024-04-25 10:30:29.000000 tui_dsmt-202404280846/src/tui_dsmt/clustering/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     2691 2024-04-25 10:30:29.000000 tui_dsmt-202404280846/src/tui_dsmt/clustering/animation.py
+-rw-rw-rw-   0 root         (0) root         (0)    19467 2024-04-25 10:30:29.000000 tui_dsmt-202404280846/src/tui_dsmt/clustering/datasets.py
+-rw-rw-rw-   0 root         (0) root         (0)      260 2024-04-25 10:30:29.000000 tui_dsmt-202404280846/src/tui_dsmt/clustering/draw.py
+-rw-rw-rw-   0 root         (0) root         (0)     2141 2024-04-28 07:42:19.000000 tui_dsmt-202404280846/src/tui_dsmt/clustering/evaluation.py
+-rw-rw-rw-   0 root         (0) root         (0)     4488 2024-04-25 10:30:29.000000 tui_dsmt-202404280846/src/tui_dsmt/clustering/hierarchical.py
+-rw-rw-rw-   0 root         (0) root         (0)      945 2024-04-25 10:30:29.000000 tui_dsmt-202404280846/src/tui_dsmt/clustering/interactive.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-28 08:46:09.816292 tui_dsmt-202404280846/src/tui_dsmt/fpm/
+-rw-rw-rw-   0 root         (0) root         (0)    14098 2024-04-25 10:30:29.000000 tui_dsmt-202404280846/src/tui_dsmt/fpm/BruteForceFI.py
+-rw-rw-rw-   0 root         (0) root         (0)     4055 2024-04-25 10:30:29.000000 tui_dsmt-202404280846/src/tui_dsmt/fpm/ConditionalFPTree.py
+-rw-rw-rw-   0 root         (0) root         (0)     5837 2024-04-25 10:30:29.000000 tui_dsmt-202404280846/src/tui_dsmt/fpm/ConditionalPatternBase.py
+-rw-rw-rw-   0 root         (0) root         (0)    11867 2024-04-25 10:30:29.000000 tui_dsmt-202404280846/src/tui_dsmt/fpm/FPTree.py
+-rw-rw-rw-   0 root         (0) root         (0)    18908 2024-04-25 10:30:29.000000 tui_dsmt-202404280846/src/tui_dsmt/fpm/HashTree.py
+-rw-rw-rw-   0 root         (0) root         (0)     1462 2024-04-25 10:30:29.000000 tui_dsmt-202404280846/src/tui_dsmt/fpm/Itemset.py
+-rw-rw-rw-   0 root         (0) root         (0)     3036 2024-04-25 10:30:29.000000 tui_dsmt-202404280846/src/tui_dsmt/fpm/ItemsetGrid.py
+-rw-rw-rw-   0 root         (0) root         (0)     5942 2024-04-25 10:30:29.000000 tui_dsmt-202404280846/src/tui_dsmt/fpm/ItemsetGridApriori.py
+-rw-rw-rw-   0 root         (0) root         (0)     5865 2024-04-25 10:30:29.000000 tui_dsmt-202404280846/src/tui_dsmt/fpm/ItemsetGridECLAT.py
+-rw-rw-rw-   0 root         (0) root         (0)     1309 2024-04-28 08:46:02.000000 tui_dsmt-202404280846/src/tui_dsmt/fpm/SequentialDatabase.py
+-rw-rw-rw-   0 root         (0) root         (0)     1129 2024-04-25 10:30:29.000000 tui_dsmt-202404280846/src/tui_dsmt/fpm/SequentialItemset.py
+-rw-rw-rw-   0 root         (0) root         (0)     1181 2024-04-25 10:30:29.000000 tui_dsmt-202404280846/src/tui_dsmt/fpm/TransactionDatabase.py
+-rw-rw-rw-   0 root         (0) root         (0)   112752 2024-04-28 08:46:02.000000 tui_dsmt-202404280846/src/tui_dsmt/fpm/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-28 08:46:09.820292 tui_dsmt-202404280846/src/tui_dsmt/graph/
+-rw-rw-rw-   0 root         (0) root         (0)     3894 2024-04-25 10:30:29.000000 tui_dsmt-202404280846/src/tui_dsmt/graph/BFS.py
+-rw-rw-rw-   0 root         (0) root         (0)     1585 2024-04-25 10:30:29.000000 tui_dsmt-202404280846/src/tui_dsmt/graph/BipartiteFlow.py
+-rw-rw-rw-   0 root         (0) root         (0)     3478 2024-04-25 10:30:29.000000 tui_dsmt-202404280846/src/tui_dsmt/graph/DFS.py
+-rw-rw-rw-   0 root         (0) root         (0)     5843 2024-04-25 10:30:29.000000 tui_dsmt-202404280846/src/tui_dsmt/graph/Dijkstra.py
+-rw-rw-rw-   0 root         (0) root         (0)      175 2024-04-25 10:30:29.000000 tui_dsmt-202404280846/src/tui_dsmt/graph/EdmondsKarp.py
+-rw-rw-rw-   0 root         (0) root         (0)     4747 2024-04-25 10:30:29.000000 tui_dsmt-202404280846/src/tui_dsmt/graph/FordFulkerson.py
+-rw-rw-rw-   0 root         (0) root         (0)     4461 2024-04-25 10:30:29.000000 tui_dsmt-202404280846/src/tui_dsmt/graph/Hall.py
+-rw-rw-rw-   0 root         (0) root         (0)     2095 2024-04-25 10:30:29.000000 tui_dsmt-202404280846/src/tui_dsmt/graph/InteractiveGraph.py
+-rw-rw-rw-   0 root         (0) root         (0)     3142 2024-04-25 10:30:29.000000 tui_dsmt-202404280846/src/tui_dsmt/graph/Kruskal.py
+-rw-rw-rw-   0 root         (0) root         (0)     4877 2024-04-25 10:30:29.000000 tui_dsmt-202404280846/src/tui_dsmt/graph/LabelPropagation.py
+-rw-rw-rw-   0 root         (0) root         (0)       39 2024-04-25 10:30:29.000000 tui_dsmt-202404280846/src/tui_dsmt/graph/MarkovClusterAlgorithm.py
+-rw-rw-rw-   0 root         (0) root         (0)     2234 2024-04-25 10:30:29.000000 tui_dsmt-202404280846/src/tui_dsmt/graph/MaximumFlow.py
+-rw-rw-rw-   0 root         (0) root         (0)     2705 2024-04-25 10:30:29.000000 tui_dsmt-202404280846/src/tui_dsmt/graph/RandomWalk.py
+-rw-rw-rw-   0 root         (0) root         (0)   420228 2024-04-25 10:30:29.000000 tui_dsmt-202404280846/src/tui_dsmt/graph/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     5267 2024-04-25 10:30:29.000000 tui_dsmt-202404280846/src/tui_dsmt/graph/game.py
+-rw-rw-rw-   0 root         (0) root         (0)     5766 2024-04-25 10:30:29.000000 tui_dsmt-202404280846/src/tui_dsmt/graph/html.py
+-rw-rw-rw-   0 root         (0) root         (0)      870 2024-04-25 10:30:29.000000 tui_dsmt-202404280846/src/tui_dsmt/graph/representation.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-28 08:46:09.824292 tui_dsmt-202404280846/src/tui_dsmt/jpanim/
+-rw-rw-rw-   0 root         (0) root         (0)     2935 2024-04-25 10:30:29.000000 tui_dsmt-202404280846/src/tui_dsmt/jpanim/JupyterAnimation.py
+-rw-rw-rw-   0 root         (0) root         (0)       47 2024-04-25 10:30:29.000000 tui_dsmt-202404280846/src/tui_dsmt/jpanim/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-28 08:46:09.824292 tui_dsmt-202404280846/src/tui_dsmt/jpanim/resources/
+-rw-rw-rw-   0 root         (0) root         (0)     2002 2024-04-25 10:30:29.000000 tui_dsmt-202404280846/src/tui_dsmt/jpanim/resources/controls-ff.html
+-rw-rw-rw-   0 root         (0) root         (0)      797 2024-04-25 10:30:29.000000 tui_dsmt-202404280846/src/tui_dsmt/jpanim/resources/controls.html
+-rw-rw-rw-   0 root         (0) root         (0)      743 2024-04-25 10:30:29.000000 tui_dsmt-202404280846/src/tui_dsmt/jpanim/resources/script.js
+-rw-rw-rw-   0 root         (0) root         (0)      193 2024-04-25 10:30:29.000000 tui_dsmt-202404280846/src/tui_dsmt/jpanim/resources/style.css
+-rw-rw-rw-   0 root         (0) root         (0)   147897 2024-04-25 10:30:29.000000 tui_dsmt-202404280846/src/tui_dsmt/jpanim/resources/vue-3.4.24.js
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-28 08:46:09.824292 tui_dsmt-202404280846/src/tui_dsmt/util/
+-rw-rw-rw-   0 root         (0) root         (0)       92 2024-04-25 10:30:29.000000 tui_dsmt-202404280846/src/tui_dsmt/util/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-28 08:46:09.824292 tui_dsmt-202404280846/src/tui_dsmt.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      835 2024-04-28 08:46:09.000000 tui_dsmt-202404280846/src/tui_dsmt.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1828 2024-04-28 08:46:09.000000 tui_dsmt-202404280846/src/tui_dsmt.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-04-28 08:46:09.000000 tui_dsmt-202404280846/src/tui_dsmt.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      162 2024-04-28 08:46:09.000000 tui_dsmt-202404280846/src/tui_dsmt.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        9 2024-04-28 08:46:09.000000 tui_dsmt-202404280846/src/tui_dsmt.egg-info/top_level.txt
```

### Comparing `tui_dsmt-202404280836/PKG-INFO` & `tui_dsmt-202404280846/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tui_dsmt
-Version: 202404280836
+Version: 202404280846
 Summary: everything you need for our jupyter notebooks
 Home-page: https://dbgit.prakinf.tu-ilmenau.de/lectures/data-science-methoden-und-techniken
 Author: Eric Tröbs
 Author-email: eric.troebs@tu-ilmenau.de
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `tui_dsmt-202404280836/setup.py` & `tui_dsmt-202404280846/setup.py`

 * *Files identical despite different names*

### Comparing `tui_dsmt-202404280836/src/tui_dsmt/__init__.py` & `tui_dsmt-202404280846/src/tui_dsmt/__init__.py`

 * *Files identical despite different names*

### Comparing `tui_dsmt-202404280836/src/tui_dsmt/clustering/PAM.py` & `tui_dsmt-202404280846/src/tui_dsmt/clustering/PAM.py`

 * *Files identical despite different names*

### Comparing `tui_dsmt-202404280836/src/tui_dsmt/clustering/animation.py` & `tui_dsmt-202404280846/src/tui_dsmt/clustering/animation.py`

 * *Files identical despite different names*

### Comparing `tui_dsmt-202404280836/src/tui_dsmt/clustering/datasets.py` & `tui_dsmt-202404280846/src/tui_dsmt/clustering/datasets.py`

 * *Files identical despite different names*

### Comparing `tui_dsmt-202404280836/src/tui_dsmt/clustering/evaluation.py` & `tui_dsmt-202404280846/src/tui_dsmt/clustering/evaluation.py`

 * *Files identical despite different names*

### Comparing `tui_dsmt-202404280836/src/tui_dsmt/clustering/hierarchical.py` & `tui_dsmt-202404280846/src/tui_dsmt/clustering/hierarchical.py`

 * *Files identical despite different names*

### Comparing `tui_dsmt-202404280836/src/tui_dsmt/clustering/interactive.py` & `tui_dsmt-202404280846/src/tui_dsmt/clustering/interactive.py`

 * *Files identical despite different names*

### Comparing `tui_dsmt-202404280836/src/tui_dsmt/fpm/BruteForceFI.py` & `tui_dsmt-202404280846/src/tui_dsmt/fpm/BruteForceFI.py`

 * *Files identical despite different names*

### Comparing `tui_dsmt-202404280836/src/tui_dsmt/fpm/ConditionalFPTree.py` & `tui_dsmt-202404280846/src/tui_dsmt/fpm/ConditionalFPTree.py`

 * *Files identical despite different names*

### Comparing `tui_dsmt-202404280836/src/tui_dsmt/fpm/ConditionalPatternBase.py` & `tui_dsmt-202404280846/src/tui_dsmt/fpm/ConditionalPatternBase.py`

 * *Files identical despite different names*

### Comparing `tui_dsmt-202404280836/src/tui_dsmt/fpm/FPTree.py` & `tui_dsmt-202404280846/src/tui_dsmt/fpm/FPTree.py`

 * *Files identical despite different names*

### Comparing `tui_dsmt-202404280836/src/tui_dsmt/fpm/HashTree.py` & `tui_dsmt-202404280846/src/tui_dsmt/fpm/HashTree.py`

 * *Files identical despite different names*

### Comparing `tui_dsmt-202404280836/src/tui_dsmt/fpm/Itemset.py` & `tui_dsmt-202404280846/src/tui_dsmt/fpm/Itemset.py`

 * *Files identical despite different names*

### Comparing `tui_dsmt-202404280836/src/tui_dsmt/fpm/ItemsetGrid.py` & `tui_dsmt-202404280846/src/tui_dsmt/fpm/ItemsetGrid.py`

 * *Files identical despite different names*

### Comparing `tui_dsmt-202404280836/src/tui_dsmt/fpm/ItemsetGridApriori.py` & `tui_dsmt-202404280846/src/tui_dsmt/fpm/ItemsetGridApriori.py`

 * *Files identical despite different names*

### Comparing `tui_dsmt-202404280836/src/tui_dsmt/fpm/ItemsetGridECLAT.py` & `tui_dsmt-202404280846/src/tui_dsmt/fpm/ItemsetGridECLAT.py`

 * *Files identical despite different names*

### Comparing `tui_dsmt-202404280836/src/tui_dsmt/fpm/SequentialDatabase.py` & `tui_dsmt-202404280846/src/tui_dsmt/fpm/SequentialDatabase.py`

 * *Files 14% similar despite different names*

```diff
@@ -28,20 +28,21 @@
     def max_length(self) -> int:
         return max(
             len(transaction)
             for _, transaction in self
         )
 
     @property
-    def powerset(self) -> 'SequentialDatabase':
+    def item_powerset(self) -> 'SequentialDatabase':
         items = list(self.items)
 
         def generate(l: int):
             if l == 0:
                 return
 
             for i in items:
                 yield i
                 for k in generate(l - 1):
-                    yield i + k
+                    if i[0] not in k:
+                        yield i + k
 
         return SequentialDatabase(*enumerate(sorted(generate(self.max_length))))
```

### Comparing `tui_dsmt-202404280836/src/tui_dsmt/fpm/SequentialItemset.py` & `tui_dsmt-202404280846/src/tui_dsmt/fpm/SequentialItemset.py`

 * *Files identical despite different names*

### Comparing `tui_dsmt-202404280836/src/tui_dsmt/fpm/TransactionDatabase.py` & `tui_dsmt-202404280846/src/tui_dsmt/fpm/TransactionDatabase.py`

 * *Files identical despite different names*

### Comparing `tui_dsmt-202404280836/src/tui_dsmt/fpm/__init__.py` & `tui_dsmt-202404280846/src/tui_dsmt/fpm/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -22,18 +22,24 @@
     (2, Itemset('Butter', 'Mehl', 'Milch', 'Zucker')),
     (3, Itemset('Butter', 'Eier', 'Milch', 'Salz')),
     (4, Itemset('Eier')),
     (5, Itemset('Butter', 'Mehl', 'Milch', 'Salz', 'Zucker')),
 )
 
 sequential_receipts = SequentialDatabase(
-    (1, SequentialItemset('Brot', 'Milch', 'Eier')),
-    (2, SequentialItemset('Milch', 'Eier')),
+    (1, SequentialItemset('Eier', 'Brot', 'Milch', 'Käse')),
+    (2, SequentialItemset('Milch', 'Eier', 'Butter')),
     (3, SequentialItemset('Brot', 'Butter', 'Eier')),
-    (4, SequentialItemset('Brot', 'Milch'))
+    (4, SequentialItemset('Brot', 'Milch', 'Käse')),
+    (5, SequentialItemset('Brot', 'Eier', 'Milch')),
+    (6, SequentialItemset('Brot', 'Eier'))
+    # (1, SequentialItemset('Brot', 'Milch', 'Eier')),
+    # (2, SequentialItemset('Milch', 'Eier')),
+    # (3, SequentialItemset('Brot', 'Butter', 'Eier')),
+    # (4, SequentialItemset('Brot', 'Milch'))
 )
 
 numbers = TransactionDatabase(
     (100, Itemset(1, 3, 4)),
     (200, Itemset(2, 3, 5)),
     (300, Itemset(1, 2, 3, 5)),
     (400, Itemset(2, 5)),
```

### Comparing `tui_dsmt-202404280836/src/tui_dsmt/graph/BFS.py` & `tui_dsmt-202404280846/src/tui_dsmt/graph/BFS.py`

 * *Files identical despite different names*

### Comparing `tui_dsmt-202404280836/src/tui_dsmt/graph/BipartiteFlow.py` & `tui_dsmt-202404280846/src/tui_dsmt/graph/BipartiteFlow.py`

 * *Files identical despite different names*

### Comparing `tui_dsmt-202404280836/src/tui_dsmt/graph/DFS.py` & `tui_dsmt-202404280846/src/tui_dsmt/graph/DFS.py`

 * *Files identical despite different names*

### Comparing `tui_dsmt-202404280836/src/tui_dsmt/graph/Dijkstra.py` & `tui_dsmt-202404280846/src/tui_dsmt/graph/Dijkstra.py`

 * *Files identical despite different names*

### Comparing `tui_dsmt-202404280836/src/tui_dsmt/graph/FordFulkerson.py` & `tui_dsmt-202404280846/src/tui_dsmt/graph/FordFulkerson.py`

 * *Files identical despite different names*

### Comparing `tui_dsmt-202404280836/src/tui_dsmt/graph/Hall.py` & `tui_dsmt-202404280846/src/tui_dsmt/graph/Hall.py`

 * *Files identical despite different names*

### Comparing `tui_dsmt-202404280836/src/tui_dsmt/graph/InteractiveGraph.py` & `tui_dsmt-202404280846/src/tui_dsmt/graph/InteractiveGraph.py`

 * *Files identical despite different names*

### Comparing `tui_dsmt-202404280836/src/tui_dsmt/graph/Kruskal.py` & `tui_dsmt-202404280846/src/tui_dsmt/graph/Kruskal.py`

 * *Files identical despite different names*

### Comparing `tui_dsmt-202404280836/src/tui_dsmt/graph/LabelPropagation.py` & `tui_dsmt-202404280846/src/tui_dsmt/graph/LabelPropagation.py`

 * *Files identical despite different names*

### Comparing `tui_dsmt-202404280836/src/tui_dsmt/graph/MaximumFlow.py` & `tui_dsmt-202404280846/src/tui_dsmt/graph/MaximumFlow.py`

 * *Files identical despite different names*

### Comparing `tui_dsmt-202404280836/src/tui_dsmt/graph/RandomWalk.py` & `tui_dsmt-202404280846/src/tui_dsmt/graph/RandomWalk.py`

 * *Files identical despite different names*

### Comparing `tui_dsmt-202404280836/src/tui_dsmt/graph/__init__.py` & `tui_dsmt-202404280846/src/tui_dsmt/graph/__init__.py`

 * *Files identical despite different names*

### Comparing `tui_dsmt-202404280836/src/tui_dsmt/graph/game.py` & `tui_dsmt-202404280846/src/tui_dsmt/graph/game.py`

 * *Files identical despite different names*

### Comparing `tui_dsmt-202404280836/src/tui_dsmt/graph/html.py` & `tui_dsmt-202404280846/src/tui_dsmt/graph/html.py`

 * *Files identical despite different names*

### Comparing `tui_dsmt-202404280836/src/tui_dsmt/graph/representation.py` & `tui_dsmt-202404280846/src/tui_dsmt/graph/representation.py`

 * *Files identical despite different names*

### Comparing `tui_dsmt-202404280836/src/tui_dsmt/jpanim/JupyterAnimation.py` & `tui_dsmt-202404280846/src/tui_dsmt/jpanim/JupyterAnimation.py`

 * *Files identical despite different names*

### Comparing `tui_dsmt-202404280836/src/tui_dsmt/jpanim/resources/controls-ff.html` & `tui_dsmt-202404280846/src/tui_dsmt/jpanim/resources/controls-ff.html`

 * *Files identical despite different names*

### Comparing `tui_dsmt-202404280836/src/tui_dsmt/jpanim/resources/controls.html` & `tui_dsmt-202404280846/src/tui_dsmt/jpanim/resources/controls.html`

 * *Files identical despite different names*

### Comparing `tui_dsmt-202404280836/src/tui_dsmt/jpanim/resources/script.js` & `tui_dsmt-202404280846/src/tui_dsmt/jpanim/resources/script.js`

 * *Files identical despite different names*

### Comparing `tui_dsmt-202404280836/src/tui_dsmt/jpanim/resources/vue-3.4.24.js` & `tui_dsmt-202404280846/src/tui_dsmt/jpanim/resources/vue-3.4.24.js`

 * *Files identical despite different names*

### Comparing `tui_dsmt-202404280836/src/tui_dsmt.egg-info/PKG-INFO` & `tui_dsmt-202404280846/src/tui_dsmt.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tui_dsmt
-Version: 202404280836
+Version: 202404280846
 Summary: everything you need for our jupyter notebooks
 Home-page: https://dbgit.prakinf.tu-ilmenau.de/lectures/data-science-methoden-und-techniken
 Author: Eric Tröbs
 Author-email: eric.troebs@tu-ilmenau.de
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `tui_dsmt-202404280836/src/tui_dsmt.egg-info/SOURCES.txt` & `tui_dsmt-202404280846/src/tui_dsmt.egg-info/SOURCES.txt`

 * *Files identical despite different names*

