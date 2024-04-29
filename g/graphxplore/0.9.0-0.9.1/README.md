# Comparing `tmp/graphxplore-0.9.0.tar.gz` & `tmp/graphxplore-0.9.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "graphxplore-0.9.0.tar", last modified: Thu Apr 18 14:17:06 2024, max compression
+gzip compressed data, was "graphxplore-0.9.1.tar", last modified: Mon Apr 29 14:19:56 2024, max compression
```

## Comparing `graphxplore-0.9.0.tar` & `graphxplore-0.9.1.tar`

### file list

```diff
@@ -1,57 +1,58 @@
-drwxrwxrwx   0 lbellmann  (1000) lbellmann  (1000)        0 2024-04-18 14:17:06.859144 graphxplore-0.9.0/
--rwxrwxrwx   0 lbellmann  (1000) lbellmann  (1000)     1104 2024-04-11 12:13:02.000000 graphxplore-0.9.0/LICENSE
--rwxrwxrwx   0 lbellmann  (1000) lbellmann  (1000)      355 2024-04-18 14:17:06.853177 graphxplore-0.9.0/PKG-INFO
--rwxrwxrwx   0 lbellmann  (1000) lbellmann  (1000)     2114 2024-04-11 12:20:38.000000 graphxplore-0.9.0/README.md
-drwxrwxrwx   0 lbellmann  (1000) lbellmann  (1000)        0 2024-04-18 14:17:06.313133 graphxplore-0.9.0/graphxplore/
-drwxrwxrwx   0 lbellmann  (1000) lbellmann  (1000)        0 2024-04-18 14:17:06.395619 graphxplore-0.9.0/graphxplore/Basis/
-drwxrwxrwx   0 lbellmann  (1000) lbellmann  (1000)        0 2024-04-18 14:17:06.426349 graphxplore-0.9.0/graphxplore/Basis/AttributeAssociationGraph/
--rwxrwxrwx   0 lbellmann  (1000) lbellmann  (1000)      533 2024-04-11 12:20:39.000000 graphxplore-0.9.0/graphxplore/Basis/AttributeAssociationGraph/__init__.py
--rwxrwxrwx   0 lbellmann  (1000) lbellmann  (1000)    25975 2024-04-11 12:20:39.000000 graphxplore-0.9.0/graphxplore/Basis/AttributeAssociationGraph/attribute_association_graph_classes.py
-drwxrwxrwx   0 lbellmann  (1000) lbellmann  (1000)        0 2024-04-18 14:17:06.457814 graphxplore-0.9.0/graphxplore/Basis/BaseGraph/
--rwxrwxrwx   0 lbellmann  (1000) lbellmann  (1000)      294 2024-04-11 12:20:39.000000 graphxplore-0.9.0/graphxplore/Basis/BaseGraph/__init__.py
--rwxrwxrwx   0 lbellmann  (1000) lbellmann  (1000)    13043 2024-04-11 12:20:39.000000 graphxplore-0.9.0/graphxplore/Basis/BaseGraph/base_classes.py
--rwxrwxrwx   0 lbellmann  (1000) lbellmann  (1000)      480 2024-04-11 12:20:39.000000 graphxplore-0.9.0/graphxplore/Basis/__init__.py
--rwxrwxrwx   0 lbellmann  (1000) lbellmann  (1000)      684 2024-04-11 12:20:39.000000 graphxplore-0.9.0/graphxplore/Basis/graph_classes.py
--rwxrwxrwx   0 lbellmann  (1000) lbellmann  (1000)    42586 2024-04-11 12:20:39.000000 graphxplore-0.9.0/graphxplore/Basis/graph_io_handlers.py
--rwxrwxrwx   0 lbellmann  (1000) lbellmann  (1000)    17261 2024-04-11 12:20:39.000000 graphxplore-0.9.0/graphxplore/Basis/utils.py
-drwxrwxrwx   0 lbellmann  (1000) lbellmann  (1000)        0 2024-04-18 14:17:06.500497 graphxplore-0.9.0/graphxplore/Dashboard/
--rwxrwxrwx   0 lbellmann  (1000) lbellmann  (1000)      223 2024-04-11 12:20:39.000000 graphxplore-0.9.0/graphxplore/Dashboard/__init__.py
--rwxrwxrwx   0 lbellmann  (1000) lbellmann  (1000)    18273 2024-04-11 12:20:39.000000 graphxplore-0.9.0/graphxplore/Dashboard/dashboard_buider.py
--rwxrwxrwx   0 lbellmann  (1000) lbellmann  (1000)     3231 2024-04-11 12:20:39.000000 graphxplore-0.9.0/graphxplore/Dashboard/meta_distribution_plotter.py
-drwxrwxrwx   0 lbellmann  (1000) lbellmann  (1000)        0 2024-04-18 14:17:06.610656 graphxplore-0.9.0/graphxplore/DataMapping/
-drwxrwxrwx   0 lbellmann  (1000) lbellmann  (1000)        0 2024-04-18 14:17:06.639851 graphxplore-0.9.0/graphxplore/DataMapping/Conclusions/
--rwxrwxrwx   0 lbellmann  (1000) lbellmann  (1000)      227 2024-04-11 12:20:39.000000 graphxplore-0.9.0/graphxplore/DataMapping/Conclusions/__init__.py
--rwxrwxrwx   0 lbellmann  (1000) lbellmann  (1000)     8812 2024-04-11 12:20:39.000000 graphxplore-0.9.0/graphxplore/DataMapping/Conclusions/conclusions.py
-drwxrwxrwx   0 lbellmann  (1000) lbellmann  (1000)        0 2024-04-18 14:17:06.670415 graphxplore-0.9.0/graphxplore/DataMapping/Conditionals/
--rwxrwxrwx   0 lbellmann  (1000) lbellmann  (1000)      599 2024-04-11 12:20:39.000000 graphxplore-0.9.0/graphxplore/DataMapping/Conditionals/__init__.py
--rwxrwxrwx   0 lbellmann  (1000) lbellmann  (1000)    28315 2024-04-11 12:20:39.000000 graphxplore-0.9.0/graphxplore/DataMapping/Conditionals/logic_operators.py
--rwxrwxrwx   0 lbellmann  (1000) lbellmann  (1000)      911 2024-04-11 12:20:39.000000 graphxplore-0.9.0/graphxplore/DataMapping/__init__.py
--rwxrwxrwx   0 lbellmann  (1000) lbellmann  (1000)    20705 2024-04-11 12:20:39.000000 graphxplore-0.9.0/graphxplore/DataMapping/data_aggregator.py
--rwxrwxrwx   0 lbellmann  (1000) lbellmann  (1000)    33662 2024-04-11 12:20:39.000000 graphxplore-0.9.0/graphxplore/DataMapping/data_mapping.py
--rwxrwxrwx   0 lbellmann  (1000) lbellmann  (1000)    25598 2024-04-11 12:20:39.000000 graphxplore-0.9.0/graphxplore/DataMapping/data_structure_transformer.py
--rwxrwxrwx   0 lbellmann  (1000) lbellmann  (1000)    13482 2024-04-11 12:20:39.000000 graphxplore-0.9.0/graphxplore/DataMapping/data_transformation.py
--rwxrwxrwx   0 lbellmann  (1000) lbellmann  (1000)    12941 2024-04-11 12:20:39.000000 graphxplore-0.9.0/graphxplore/DataMapping/mapping_utils.py
--rwxrwxrwx   0 lbellmann  (1000) lbellmann  (1000)    14679 2024-04-11 12:20:39.000000 graphxplore-0.9.0/graphxplore/DataMapping/meta_lattice.py
--rwxrwxrwx   0 lbellmann  (1000) lbellmann  (1000)     7100 2024-04-11 12:20:39.000000 graphxplore-0.9.0/graphxplore/DataMapping/variable_mapping.py
-drwxrwxrwx   0 lbellmann  (1000) lbellmann  (1000)        0 2024-04-18 14:17:06.739846 graphxplore-0.9.0/graphxplore/GraphDataScience/
--rwxrwxrwx   0 lbellmann  (1000) lbellmann  (1000)     1037 2024-04-11 12:20:39.000000 graphxplore-0.9.0/graphxplore/GraphDataScience/__init__.py
--rwxrwxrwx   0 lbellmann  (1000) lbellmann  (1000)    25496 2024-04-11 12:20:39.000000 graphxplore-0.9.0/graphxplore/GraphDataScience/attribute_association_graph_generator.py
--rwxrwxrwx   0 lbellmann  (1000) lbellmann  (1000)    14298 2024-04-11 12:20:39.000000 graphxplore-0.9.0/graphxplore/GraphDataScience/group_selector.py
--rwxrwxrwx   0 lbellmann  (1000) lbellmann  (1000)    23114 2024-04-11 12:20:39.000000 graphxplore-0.9.0/graphxplore/GraphDataScience/post_filter.py
--rwxrwxrwx   0 lbellmann  (1000) lbellmann  (1000)     7563 2024-04-11 12:20:39.000000 graphxplore-0.9.0/graphxplore/GraphDataScience/pre_filter.py
-drwxrwxrwx   0 lbellmann  (1000) lbellmann  (1000)        0 2024-04-18 14:17:06.768422 graphxplore-0.9.0/graphxplore/GraphTranslation/
--rwxrwxrwx   0 lbellmann  (1000) lbellmann  (1000)       76 2024-04-11 12:20:39.000000 graphxplore-0.9.0/graphxplore/GraphTranslation/__init__.py
--rwxrwxrwx   0 lbellmann  (1000) lbellmann  (1000)    16473 2024-04-11 12:20:39.000000 graphxplore-0.9.0/graphxplore/GraphTranslation/graph_translator.py
-drwxrwxrwx   0 lbellmann  (1000) lbellmann  (1000)        0 2024-04-18 14:17:06.832844 graphxplore-0.9.0/graphxplore/MetaDataHandling/
--rwxrwxrwx   0 lbellmann  (1000) lbellmann  (1000)      436 2024-04-11 12:20:39.000000 graphxplore-0.9.0/graphxplore/MetaDataHandling/__init__.py
--rwxrwxrwx   0 lbellmann  (1000) lbellmann  (1000)    21218 2024-04-11 12:20:39.000000 graphxplore-0.9.0/graphxplore/MetaDataHandling/meta_data.py
--rwxrwxrwx   0 lbellmann  (1000) lbellmann  (1000)    13448 2024-04-11 12:20:39.000000 graphxplore-0.9.0/graphxplore/MetaDataHandling/meta_data_generator.py
--rwxrwxrwx   0 lbellmann  (1000) lbellmann  (1000)    23983 2024-04-11 12:20:39.000000 graphxplore-0.9.0/graphxplore/MetaDataHandling/variable_info.py
--rwxrwxrwx   0 lbellmann  (1000) lbellmann  (1000)        0 2024-04-11 12:20:39.000000 graphxplore-0.9.0/graphxplore/__init__.py
-drwxrwxrwx   0 lbellmann  (1000) lbellmann  (1000)        0 2024-04-18 14:17:06.847571 graphxplore-0.9.0/graphxplore.egg-info/
--rwxrwxrwx   0 lbellmann  (1000) lbellmann  (1000)      355 2024-04-18 14:17:06.000000 graphxplore-0.9.0/graphxplore.egg-info/PKG-INFO
--rwxrwxrwx   0 lbellmann  (1000) lbellmann  (1000)     1736 2024-04-18 14:17:06.000000 graphxplore-0.9.0/graphxplore.egg-info/SOURCES.txt
--rwxrwxrwx   0 lbellmann  (1000) lbellmann  (1000)        1 2024-04-18 14:17:06.000000 graphxplore-0.9.0/graphxplore.egg-info/dependency_links.txt
--rwxrwxrwx   0 lbellmann  (1000) lbellmann  (1000)       12 2024-04-18 14:17:06.000000 graphxplore-0.9.0/graphxplore.egg-info/top_level.txt
--rwxrwxrwx   0 lbellmann  (1000) lbellmann  (1000)       38 2024-04-18 14:17:06.859325 graphxplore-0.9.0/setup.cfg
--rwxrwxrwx   0 lbellmann  (1000) lbellmann  (1000)      467 2024-04-18 13:52:44.000000 graphxplore-0.9.0/setup.py
+drwxrwxrwx   0 lbellmann  (1000) lbellmann  (1000)        0 2024-04-29 14:19:56.380930 graphxplore-0.9.1/
+-rwxrwxrwx   0 lbellmann  (1000) lbellmann  (1000)     1104 2024-04-11 12:13:02.000000 graphxplore-0.9.1/LICENSE
+-rwxrwxrwx   0 lbellmann  (1000) lbellmann  (1000)     4227 2024-04-29 14:19:56.375613 graphxplore-0.9.1/PKG-INFO
+-rwxrwxrwx   0 lbellmann  (1000) lbellmann  (1000)     2375 2024-04-29 12:37:05.000000 graphxplore-0.9.1/README.md
+drwxrwxrwx   0 lbellmann  (1000) lbellmann  (1000)        0 2024-04-29 14:19:55.835412 graphxplore-0.9.1/graphxplore/
+drwxrwxrwx   0 lbellmann  (1000) lbellmann  (1000)        0 2024-04-29 14:19:55.946296 graphxplore-0.9.1/graphxplore/Basis/
+drwxrwxrwx   0 lbellmann  (1000) lbellmann  (1000)        0 2024-04-29 14:19:55.980944 graphxplore-0.9.1/graphxplore/Basis/AttributeAssociationGraph/
+-rwxrwxrwx   0 lbellmann  (1000) lbellmann  (1000)      533 2024-04-25 13:48:29.000000 graphxplore-0.9.1/graphxplore/Basis/AttributeAssociationGraph/__init__.py
+-rwxrwxrwx   0 lbellmann  (1000) lbellmann  (1000)    25975 2024-04-25 13:48:29.000000 graphxplore-0.9.1/graphxplore/Basis/AttributeAssociationGraph/attribute_association_graph_classes.py
+drwxrwxrwx   0 lbellmann  (1000) lbellmann  (1000)        0 2024-04-29 14:19:56.011277 graphxplore-0.9.1/graphxplore/Basis/BaseGraph/
+-rwxrwxrwx   0 lbellmann  (1000) lbellmann  (1000)      294 2024-04-25 13:48:29.000000 graphxplore-0.9.1/graphxplore/Basis/BaseGraph/__init__.py
+-rwxrwxrwx   0 lbellmann  (1000) lbellmann  (1000)    13043 2024-04-25 13:48:29.000000 graphxplore-0.9.1/graphxplore/Basis/BaseGraph/base_classes.py
+-rwxrwxrwx   0 lbellmann  (1000) lbellmann  (1000)      480 2024-04-25 13:48:29.000000 graphxplore-0.9.1/graphxplore/Basis/__init__.py
+-rwxrwxrwx   0 lbellmann  (1000) lbellmann  (1000)      684 2024-04-25 13:48:29.000000 graphxplore-0.9.1/graphxplore/Basis/graph_classes.py
+-rwxrwxrwx   0 lbellmann  (1000) lbellmann  (1000)    42586 2024-04-25 13:48:29.000000 graphxplore-0.9.1/graphxplore/Basis/graph_io_handlers.py
+-rwxrwxrwx   0 lbellmann  (1000) lbellmann  (1000)    17261 2024-04-25 13:48:29.000000 graphxplore-0.9.1/graphxplore/Basis/utils.py
+drwxrwxrwx   0 lbellmann  (1000) lbellmann  (1000)        0 2024-04-29 14:19:56.048882 graphxplore-0.9.1/graphxplore/Dashboard/
+-rwxrwxrwx   0 lbellmann  (1000) lbellmann  (1000)      223 2024-04-25 13:48:29.000000 graphxplore-0.9.1/graphxplore/Dashboard/__init__.py
+-rwxrwxrwx   0 lbellmann  (1000) lbellmann  (1000)    18273 2024-04-25 13:48:29.000000 graphxplore-0.9.1/graphxplore/Dashboard/dashboard_buider.py
+-rwxrwxrwx   0 lbellmann  (1000) lbellmann  (1000)     3231 2024-04-25 13:48:29.000000 graphxplore-0.9.1/graphxplore/Dashboard/meta_distribution_plotter.py
+drwxrwxrwx   0 lbellmann  (1000) lbellmann  (1000)        0 2024-04-29 14:19:56.150478 graphxplore-0.9.1/graphxplore/DataMapping/
+drwxrwxrwx   0 lbellmann  (1000) lbellmann  (1000)        0 2024-04-29 14:19:56.177821 graphxplore-0.9.1/graphxplore/DataMapping/Conclusions/
+-rwxrwxrwx   0 lbellmann  (1000) lbellmann  (1000)      227 2024-04-25 13:48:29.000000 graphxplore-0.9.1/graphxplore/DataMapping/Conclusions/__init__.py
+-rwxrwxrwx   0 lbellmann  (1000) lbellmann  (1000)     8812 2024-04-25 13:48:29.000000 graphxplore-0.9.1/graphxplore/DataMapping/Conclusions/conclusions.py
+drwxrwxrwx   0 lbellmann  (1000) lbellmann  (1000)        0 2024-04-29 14:19:56.208143 graphxplore-0.9.1/graphxplore/DataMapping/Conditionals/
+-rwxrwxrwx   0 lbellmann  (1000) lbellmann  (1000)      599 2024-04-25 13:48:29.000000 graphxplore-0.9.1/graphxplore/DataMapping/Conditionals/__init__.py
+-rwxrwxrwx   0 lbellmann  (1000) lbellmann  (1000)    28315 2024-04-25 13:48:29.000000 graphxplore-0.9.1/graphxplore/DataMapping/Conditionals/logic_operators.py
+-rwxrwxrwx   0 lbellmann  (1000) lbellmann  (1000)      911 2024-04-25 13:48:29.000000 graphxplore-0.9.1/graphxplore/DataMapping/__init__.py
+-rwxrwxrwx   0 lbellmann  (1000) lbellmann  (1000)    20705 2024-04-25 13:48:29.000000 graphxplore-0.9.1/graphxplore/DataMapping/data_aggregator.py
+-rwxrwxrwx   0 lbellmann  (1000) lbellmann  (1000)    33662 2024-04-25 13:48:29.000000 graphxplore-0.9.1/graphxplore/DataMapping/data_mapping.py
+-rwxrwxrwx   0 lbellmann  (1000) lbellmann  (1000)    25598 2024-04-25 13:48:29.000000 graphxplore-0.9.1/graphxplore/DataMapping/data_structure_transformer.py
+-rwxrwxrwx   0 lbellmann  (1000) lbellmann  (1000)    13482 2024-04-25 13:48:29.000000 graphxplore-0.9.1/graphxplore/DataMapping/data_transformation.py
+-rwxrwxrwx   0 lbellmann  (1000) lbellmann  (1000)    12941 2024-04-25 13:48:29.000000 graphxplore-0.9.1/graphxplore/DataMapping/mapping_utils.py
+-rwxrwxrwx   0 lbellmann  (1000) lbellmann  (1000)    14679 2024-04-25 13:48:29.000000 graphxplore-0.9.1/graphxplore/DataMapping/meta_lattice.py
+-rwxrwxrwx   0 lbellmann  (1000) lbellmann  (1000)     7100 2024-04-25 13:48:29.000000 graphxplore-0.9.1/graphxplore/DataMapping/variable_mapping.py
+drwxrwxrwx   0 lbellmann  (1000) lbellmann  (1000)        0 2024-04-29 14:19:56.274060 graphxplore-0.9.1/graphxplore/GraphDataScience/
+-rwxrwxrwx   0 lbellmann  (1000) lbellmann  (1000)     1037 2024-04-25 13:48:29.000000 graphxplore-0.9.1/graphxplore/GraphDataScience/__init__.py
+-rwxrwxrwx   0 lbellmann  (1000) lbellmann  (1000)    25496 2024-04-25 13:48:29.000000 graphxplore-0.9.1/graphxplore/GraphDataScience/attribute_association_graph_generator.py
+-rwxrwxrwx   0 lbellmann  (1000) lbellmann  (1000)    14298 2024-04-25 13:48:29.000000 graphxplore-0.9.1/graphxplore/GraphDataScience/group_selector.py
+-rwxrwxrwx   0 lbellmann  (1000) lbellmann  (1000)    23114 2024-04-25 13:48:29.000000 graphxplore-0.9.1/graphxplore/GraphDataScience/post_filter.py
+-rwxrwxrwx   0 lbellmann  (1000) lbellmann  (1000)     7563 2024-04-25 13:48:29.000000 graphxplore-0.9.1/graphxplore/GraphDataScience/pre_filter.py
+drwxrwxrwx   0 lbellmann  (1000) lbellmann  (1000)        0 2024-04-29 14:19:56.301854 graphxplore-0.9.1/graphxplore/GraphTranslation/
+-rwxrwxrwx   0 lbellmann  (1000) lbellmann  (1000)       76 2024-04-25 13:48:29.000000 graphxplore-0.9.1/graphxplore/GraphTranslation/__init__.py
+-rwxrwxrwx   0 lbellmann  (1000) lbellmann  (1000)    16473 2024-04-25 13:48:29.000000 graphxplore-0.9.1/graphxplore/GraphTranslation/graph_translator.py
+drwxrwxrwx   0 lbellmann  (1000) lbellmann  (1000)        0 2024-04-29 14:19:56.354439 graphxplore-0.9.1/graphxplore/MetaDataHandling/
+-rwxrwxrwx   0 lbellmann  (1000) lbellmann  (1000)      436 2024-04-25 13:48:29.000000 graphxplore-0.9.1/graphxplore/MetaDataHandling/__init__.py
+-rwxrwxrwx   0 lbellmann  (1000) lbellmann  (1000)    21218 2024-04-25 13:48:29.000000 graphxplore-0.9.1/graphxplore/MetaDataHandling/meta_data.py
+-rwxrwxrwx   0 lbellmann  (1000) lbellmann  (1000)    13448 2024-04-25 13:48:29.000000 graphxplore-0.9.1/graphxplore/MetaDataHandling/meta_data_generator.py
+-rwxrwxrwx   0 lbellmann  (1000) lbellmann  (1000)    23983 2024-04-25 13:48:29.000000 graphxplore-0.9.1/graphxplore/MetaDataHandling/variable_info.py
+-rwxrwxrwx   0 lbellmann  (1000) lbellmann  (1000)        0 2024-04-25 13:48:29.000000 graphxplore-0.9.1/graphxplore/__init__.py
+drwxrwxrwx   0 lbellmann  (1000) lbellmann  (1000)        0 2024-04-29 14:19:56.370582 graphxplore-0.9.1/graphxplore.egg-info/
+-rwxrwxrwx   0 lbellmann  (1000) lbellmann  (1000)     4227 2024-04-29 14:19:55.000000 graphxplore-0.9.1/graphxplore.egg-info/PKG-INFO
+-rwxrwxrwx   0 lbellmann  (1000) lbellmann  (1000)     1776 2024-04-29 14:19:55.000000 graphxplore-0.9.1/graphxplore.egg-info/SOURCES.txt
+-rwxrwxrwx   0 lbellmann  (1000) lbellmann  (1000)        1 2024-04-29 14:19:55.000000 graphxplore-0.9.1/graphxplore.egg-info/dependency_links.txt
+-rwxrwxrwx   0 lbellmann  (1000) lbellmann  (1000)       28 2024-04-29 14:19:55.000000 graphxplore-0.9.1/graphxplore.egg-info/requires.txt
+-rwxrwxrwx   0 lbellmann  (1000) lbellmann  (1000)       12 2024-04-29 14:19:55.000000 graphxplore-0.9.1/graphxplore.egg-info/top_level.txt
+-rwxrwxrwx   0 lbellmann  (1000) lbellmann  (1000)      920 2024-04-29 11:49:19.000000 graphxplore-0.9.1/pyproject.toml
+-rwxrwxrwx   0 lbellmann  (1000) lbellmann  (1000)       38 2024-04-29 14:19:56.380930 graphxplore-0.9.1/setup.cfg
```

### Comparing `graphxplore-0.9.0/LICENSE` & `graphxplore-0.9.1/LICENSE`

 * *Files identical despite different names*

### Comparing `graphxplore-0.9.0/README.md` & `graphxplore-0.9.1/README.md`

 * *Files 23% similar despite different names*

```diff
@@ -1,33 +1,35 @@
 # GraphXplore: Visual exploration and easy preprocessing of data
 
 [![unittest workflow](https://github.com/UKEIAM/graphxplore/actions/workflows/unittest.yml/badge.svg)](https://github.com/UKEIAM/graphxplore/actions/workflows/unittest.yml)
+[![Documentation Status](https://readthedocs.org/projects/graphxplore/badge/?version=latest)](https://graphxplore.readthedocs.io/en/latest/?badge=latest)
 
-<img src="./frontend/GraphXplore/graphxplore_icon.png" alt="drawing" width="100"/>
+<img src="https://ukeiam.github.io/graphxplore/graphxplore_icon.png" alt="drawing" width="100"/>
 
 ## About
 
 GraphXplore is a tool for visually exploring, cleaning and transforming your data, as well as defining and sharing 
 metadata and mappings with others. You can access GraphXplore as a Python package, or use its graphical user interface 
 application. The app can either be run as a local webserver or a standalone desktop app.
 GraphXplore does not require advanced knowledge about statistics or data science and the app can be used without prior 
 coding/scripting skills. The tool was designed with the application to the medical research domain in mind, but can be 
 generally used with any data source. 
 
 ## Installation
 
-- Python package: Install from PyPi with `pip install graphxplore`, or checkout versions at ( :hammer: TODO insert pypi link)
+- Python package: Install from PyPi with `pip install graphxplore`, or checkout versions at the 
+  [PyPI GraphXplore project site](https://pypi.org/project/graphxplore/)
   - Alternatively, you can clone this repository, checkout a specific commit and use that version via `sys.path`,
     `pip install -e` or `conda develop`
-- Desktop app: Download the installer for a specific release from ( :hammer: TODO insert release link)
+- Desktop app: [Download the installer](https://github.com/UKEIAM/graphxplore/releases)
   - Alternatively, you can clone this repository, checkout a specific commit, use [NPM](https://www.npmjs.com/) and run 
     the [installation script](./frontend/build_release.sh)
 - Local webserver: Clone this repository, install streamlit with `pip install streamlit`, navigate to 
   `frontend/GraphXplore` and run `streamlit run streamlit_app.py`
 
 ## Documentation
 
-You can find detailed information about the data-related tasks that you can work in with GraphXplore, as well as its 
-functionalities at ( :hammer: TODO insert GitHub pages link). Additionally, the same information is given in the app via various 
-how-to pages and tooltips.
+In the [GraphXplore user guide](https://ukeiam.github.io/graphxplore/) you can find detailed information about the 
+data-related tasks that you can work in with GraphXplore, as well as its functionalities. Additionally, the same 
+information is given in the app via various how-to pages and tooltips.
 
-To read the Python package code documentation navigate to ( :hammer: TODO insert readthedocs link)
+For information on coding with GraphXplore, read the [Python package code documentation](https://graphxplore.readthedocs.io/en/latest/).
```

### Comparing `graphxplore-0.9.0/graphxplore/Basis/AttributeAssociationGraph/__init__.py` & `graphxplore-0.9.1/graphxplore/Basis/AttributeAssociationGraph/__init__.py`

 * *Files identical despite different names*

### Comparing `graphxplore-0.9.0/graphxplore/Basis/AttributeAssociationGraph/attribute_association_graph_classes.py` & `graphxplore-0.9.1/graphxplore/Basis/AttributeAssociationGraph/attribute_association_graph_classes.py`

 * *Files identical despite different names*

### Comparing `graphxplore-0.9.0/graphxplore/Basis/BaseGraph/base_classes.py` & `graphxplore-0.9.1/graphxplore/Basis/BaseGraph/base_classes.py`

 * *Files identical despite different names*

### Comparing `graphxplore-0.9.0/graphxplore/Basis/graph_classes.py` & `graphxplore-0.9.1/graphxplore/Basis/graph_classes.py`

 * *Files identical despite different names*

### Comparing `graphxplore-0.9.0/graphxplore/Basis/graph_io_handlers.py` & `graphxplore-0.9.1/graphxplore/Basis/graph_io_handlers.py`

 * *Files identical despite different names*

### Comparing `graphxplore-0.9.0/graphxplore/Basis/utils.py` & `graphxplore-0.9.1/graphxplore/Basis/utils.py`

 * *Files identical despite different names*

### Comparing `graphxplore-0.9.0/graphxplore/Dashboard/dashboard_buider.py` & `graphxplore-0.9.1/graphxplore/Dashboard/dashboard_buider.py`

 * *Files identical despite different names*

### Comparing `graphxplore-0.9.0/graphxplore/Dashboard/meta_distribution_plotter.py` & `graphxplore-0.9.1/graphxplore/Dashboard/meta_distribution_plotter.py`

 * *Files identical despite different names*

### Comparing `graphxplore-0.9.0/graphxplore/DataMapping/Conclusions/conclusions.py` & `graphxplore-0.9.1/graphxplore/DataMapping/Conclusions/conclusions.py`

 * *Files identical despite different names*

### Comparing `graphxplore-0.9.0/graphxplore/DataMapping/Conditionals/__init__.py` & `graphxplore-0.9.1/graphxplore/DataMapping/Conditionals/__init__.py`

 * *Files identical despite different names*

### Comparing `graphxplore-0.9.0/graphxplore/DataMapping/Conditionals/logic_operators.py` & `graphxplore-0.9.1/graphxplore/DataMapping/Conditionals/logic_operators.py`

 * *Files identical despite different names*

### Comparing `graphxplore-0.9.0/graphxplore/DataMapping/__init__.py` & `graphxplore-0.9.1/graphxplore/DataMapping/__init__.py`

 * *Files identical despite different names*

### Comparing `graphxplore-0.9.0/graphxplore/DataMapping/data_aggregator.py` & `graphxplore-0.9.1/graphxplore/DataMapping/data_aggregator.py`

 * *Files identical despite different names*

### Comparing `graphxplore-0.9.0/graphxplore/DataMapping/data_mapping.py` & `graphxplore-0.9.1/graphxplore/DataMapping/data_mapping.py`

 * *Files identical despite different names*

### Comparing `graphxplore-0.9.0/graphxplore/DataMapping/data_structure_transformer.py` & `graphxplore-0.9.1/graphxplore/DataMapping/data_structure_transformer.py`

 * *Files identical despite different names*

### Comparing `graphxplore-0.9.0/graphxplore/DataMapping/data_transformation.py` & `graphxplore-0.9.1/graphxplore/DataMapping/data_transformation.py`

 * *Files identical despite different names*

### Comparing `graphxplore-0.9.0/graphxplore/DataMapping/mapping_utils.py` & `graphxplore-0.9.1/graphxplore/DataMapping/mapping_utils.py`

 * *Files identical despite different names*

### Comparing `graphxplore-0.9.0/graphxplore/DataMapping/meta_lattice.py` & `graphxplore-0.9.1/graphxplore/DataMapping/meta_lattice.py`

 * *Files identical despite different names*

### Comparing `graphxplore-0.9.0/graphxplore/DataMapping/variable_mapping.py` & `graphxplore-0.9.1/graphxplore/DataMapping/variable_mapping.py`

 * *Files identical despite different names*

### Comparing `graphxplore-0.9.0/graphxplore/GraphDataScience/__init__.py` & `graphxplore-0.9.1/graphxplore/GraphDataScience/__init__.py`

 * *Files identical despite different names*

### Comparing `graphxplore-0.9.0/graphxplore/GraphDataScience/attribute_association_graph_generator.py` & `graphxplore-0.9.1/graphxplore/GraphDataScience/attribute_association_graph_generator.py`

 * *Files identical despite different names*

### Comparing `graphxplore-0.9.0/graphxplore/GraphDataScience/group_selector.py` & `graphxplore-0.9.1/graphxplore/GraphDataScience/group_selector.py`

 * *Files identical despite different names*

### Comparing `graphxplore-0.9.0/graphxplore/GraphDataScience/post_filter.py` & `graphxplore-0.9.1/graphxplore/GraphDataScience/post_filter.py`

 * *Files identical despite different names*

### Comparing `graphxplore-0.9.0/graphxplore/GraphDataScience/pre_filter.py` & `graphxplore-0.9.1/graphxplore/GraphDataScience/pre_filter.py`

 * *Files identical despite different names*

### Comparing `graphxplore-0.9.0/graphxplore/GraphTranslation/graph_translator.py` & `graphxplore-0.9.1/graphxplore/GraphTranslation/graph_translator.py`

 * *Files identical despite different names*

### Comparing `graphxplore-0.9.0/graphxplore/MetaDataHandling/meta_data.py` & `graphxplore-0.9.1/graphxplore/MetaDataHandling/meta_data.py`

 * *Files identical despite different names*

### Comparing `graphxplore-0.9.0/graphxplore/MetaDataHandling/meta_data_generator.py` & `graphxplore-0.9.1/graphxplore/MetaDataHandling/meta_data_generator.py`

 * *Files identical despite different names*

### Comparing `graphxplore-0.9.0/graphxplore/MetaDataHandling/variable_info.py` & `graphxplore-0.9.1/graphxplore/MetaDataHandling/variable_info.py`

 * *Files identical despite different names*

### Comparing `graphxplore-0.9.0/graphxplore.egg-info/SOURCES.txt` & `graphxplore-0.9.1/graphxplore.egg-info/SOURCES.txt`

 * *Files 8% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 LICENSE
 README.md
-setup.py
+pyproject.toml
 graphxplore/__init__.py
 graphxplore.egg-info/PKG-INFO
 graphxplore.egg-info/SOURCES.txt
 graphxplore.egg-info/dependency_links.txt
+graphxplore.egg-info/requires.txt
 graphxplore.egg-info/top_level.txt
 graphxplore/Basis/__init__.py
 graphxplore/Basis/graph_classes.py
 graphxplore/Basis/graph_io_handlers.py
 graphxplore/Basis/utils.py
 graphxplore/Basis/AttributeAssociationGraph/__init__.py
 graphxplore/Basis/AttributeAssociationGraph/attribute_association_graph_classes.py
```

