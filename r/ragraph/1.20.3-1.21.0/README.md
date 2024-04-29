# Comparing `tmp/ragraph-1.20.3.tar.gz` & `tmp/ragraph-1.21.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ragraph-1.20.3.tar", max compression
+gzip compressed data, was "ragraph-1.21.0.tar", max compression
```

## Comparing `ragraph-1.20.3.tar` & `ragraph-1.21.0.tar`

### file list

```diff
@@ -1,160 +1,160 @@
--rw-r--r--   0        0        0    34753 2023-11-21 12:46:15.645766 ragraph-1.20.3/LICENSE-GPL
--rw-r--r--   0        0        0     2144 2023-11-21 12:46:15.645766 ragraph-1.20.3/README.md
--rw-r--r--   0        0        0     1997 2023-11-21 12:46:15.651766 ragraph-1.20.3/pyproject.toml
--rw-r--r--   0        0        0       72 2023-11-21 12:46:15.651766 ragraph-1.20.3/ragraph/__init__.py
--rw-r--r--   0        0        0      138 2023-11-21 12:46:15.651766 ragraph-1.20.3/ragraph/analysis/__init__.py
--rw-r--r--   0        0        0    19876 2023-11-21 12:46:15.651766 ragraph-1.20.3/ragraph/analysis/_classes.py
--rw-r--r--   0        0        0     7950 2023-11-21 12:46:15.651766 ragraph-1.20.3/ragraph/analysis/_utils.py
--rw-r--r--   0        0        0     1008 2023-11-21 12:46:15.651766 ragraph-1.20.3/ragraph/analysis/bus/__init__.py
--rw-r--r--   0        0        0     4020 2023-11-21 12:46:15.651766 ragraph-1.20.3/ragraph/analysis/bus/_gamma.py
--rw-r--r--   0        0        0     1376 2023-11-21 12:46:15.651766 ragraph-1.20.3/ragraph/analysis/cluster/__init__.py
--rw-r--r--   0        0        0    13980 2023-11-21 12:46:15.651766 ragraph-1.20.3/ragraph/analysis/cluster/_markov.py
--rw-r--r--   0        0        0     3470 2023-11-21 12:46:15.651766 ragraph-1.20.3/ragraph/analysis/cluster/_tarjan.py
--rw-r--r--   0        0        0     1201 2023-11-21 12:46:15.651766 ragraph-1.20.3/ragraph/analysis/comparison/__init__.py
--rw-r--r--   0        0        0     2540 2023-11-21 12:46:15.651766 ragraph-1.20.3/ragraph/analysis/comparison/_delta.py
--rw-r--r--   0        0        0     6368 2023-11-21 12:46:15.652766 ragraph-1.20.3/ragraph/analysis/comparison/_sigma.py
--rw-r--r--   0        0        0     3634 2023-11-21 12:46:15.652766 ragraph-1.20.3/ragraph/analysis/comparison/utils.py
--rw-r--r--   0        0        0    20554 2023-11-21 12:46:15.652766 ragraph-1.20.3/ragraph/analysis/compatibility/__init__.py
--rw-r--r--   0        0        0     2789 2023-11-21 12:46:15.652766 ragraph-1.20.3/ragraph/analysis/compatibility/bdd.py
--rw-r--r--   0        0        0      649 2023-11-21 12:46:15.652766 ragraph-1.20.3/ragraph/analysis/heuristics/__init__.py
--rw-r--r--   0        0        0     3351 2023-11-21 12:46:15.652766 ragraph-1.20.3/ragraph/analysis/heuristics/_johnson.py
--rw-r--r--   0        0        0     5079 2023-11-21 12:46:15.652766 ragraph-1.20.3/ragraph/analysis/heuristics/_markov_gamma.py
--rw-r--r--   0        0        0     2166 2023-11-21 12:46:15.652766 ragraph-1.20.3/ragraph/analysis/sequence/__init__.py
--rw-r--r--   0        0        0    10933 2023-11-21 12:46:15.652766 ragraph-1.20.3/ragraph/analysis/sequence/_axis.py
--rw-r--r--   0        0        0     5251 2023-11-21 12:46:15.652766 ragraph-1.20.3/ragraph/analysis/sequence/_genetic.py
--rw-r--r--   0        0        0     3025 2023-11-21 12:46:15.652766 ragraph-1.20.3/ragraph/analysis/sequence/_markov.py
--rw-r--r--   0        0        0      832 2023-11-21 12:46:15.653766 ragraph-1.20.3/ragraph/analysis/sequence/_name.py
--rw-r--r--   0        0        0     3775 2023-11-21 12:46:15.653766 ragraph-1.20.3/ragraph/analysis/sequence/_scc_tearing.py
--rw-r--r--   0        0        0     1727 2023-11-21 12:46:15.653766 ragraph-1.20.3/ragraph/analysis/sequence/_tarjan.py
--rw-r--r--   0        0        0     7130 2023-11-21 12:46:15.653766 ragraph-1.20.3/ragraph/analysis/sequence/metrics.py
--rw-r--r--   0        0        0     5245 2023-11-21 12:46:15.653766 ragraph-1.20.3/ragraph/analysis/sequence/utils.py
--rw-r--r--   0        0        0     1460 2023-11-21 12:46:15.653766 ragraph-1.20.3/ragraph/analysis/similarity/__init__.py
--rw-r--r--   0        0        0     3103 2023-11-21 12:46:15.653766 ragraph-1.20.3/ragraph/analysis/similarity/_jaccard.py
--rw-r--r--   0        0        0     9922 2023-11-21 12:46:15.653766 ragraph-1.20.3/ragraph/analysis/similarity/_similarity.py
--rw-r--r--   0        0        0     1826 2023-11-21 12:46:15.653766 ragraph-1.20.3/ragraph/analysis/similarity/utils.py
--rw-r--r--   0        0        0    10265 2023-11-21 12:46:15.653766 ragraph-1.20.3/ragraph/colors/__init__.py
--rw-r--r--   0        0        0     5447 2023-11-21 12:46:15.653766 ragraph-1.20.3/ragraph/colors/cubehelix.py
--rw-r--r--   0        0        0      769 2023-11-21 12:46:15.653766 ragraph-1.20.3/ragraph/colors/utils.py
--rw-r--r--   0        0        0     1589 2023-11-21 12:46:15.653766 ragraph-1.20.3/ragraph/datasets/__init__.py
--rw-r--r--   0        0        0      679 2023-11-21 12:46:15.654766 ragraph-1.20.3/ragraph/datasets/aircraft_engine/__init__.py
--rw-r--r--   0        0        0    28938 2023-11-21 12:46:15.654766 ragraph-1.20.3/ragraph/datasets/aircraft_engine/aircraft_engine_edges.csv
--rw-r--r--   0        0        0      977 2023-11-21 12:46:15.654766 ragraph-1.20.3/ragraph/datasets/aircraft_engine/aircraft_engine_nodes.csv
--rw-r--r--   0        0        0     1073 2023-11-21 12:46:15.654766 ragraph-1.20.3/ragraph/datasets/architecture_integral/__init__.py
--rw-r--r--   0        0        0     1364 2023-11-21 12:46:15.654766 ragraph-1.20.3/ragraph/datasets/architecture_integral/architecture_integral_edges.csv
--rw-r--r--   0        0        0      352 2023-11-21 12:46:15.654766 ragraph-1.20.3/ragraph/datasets/architecture_integral/architecture_integral_nodes.csv
--rw-r--r--   0        0        0     1083 2023-11-21 12:46:15.654766 ragraph-1.20.3/ragraph/datasets/architecture_mix/__init__.py
--rw-r--r--   0        0        0     2264 2023-11-21 12:46:15.654766 ragraph-1.20.3/ragraph/datasets/architecture_mix/architecture_mix_edges.csv
--rw-r--r--   0        0        0      352 2023-11-21 12:46:15.654766 ragraph-1.20.3/ragraph/datasets/architecture_mix/architecture_mix_nodes.csv
--rw-r--r--   0        0        0     1079 2023-11-21 12:46:15.654766 ragraph-1.20.3/ragraph/datasets/architecture_modular/__init__.py
--rw-r--r--   0        0        0     2722 2023-11-21 12:46:15.654766 ragraph-1.20.3/ragraph/datasets/architecture_modular/architecture_modular_edges.csv
--rw-r--r--   0        0        0      351 2023-11-21 12:46:15.654766 ragraph-1.20.3/ragraph/datasets/architecture_modular/architecture_modular_nodes.csv
--rw-r--r--   0        0        0      822 2023-11-21 12:46:15.654766 ragraph-1.20.3/ragraph/datasets/climate_control/__init__.py
--rw-r--r--   0        0        0     5778 2023-11-21 12:46:15.654766 ragraph-1.20.3/ragraph/datasets/climate_control/climate_control_edges.csv
--rw-r--r--   0        0        0      632 2023-11-21 12:46:15.654766 ragraph-1.20.3/ragraph/datasets/climate_control/climate_control_nodes.csv
--rw-r--r--   0        0        0      423 2023-11-21 12:46:15.655766 ragraph-1.20.3/ragraph/datasets/climate_control_mg/__init__.py
--rw-r--r--   0        0        0     5778 2023-11-21 12:46:15.655766 ragraph-1.20.3/ragraph/datasets/climate_control_mg/climate_control_mg_edges.csv
--rw-r--r--   0        0        0     1441 2023-11-21 12:46:15.655766 ragraph-1.20.3/ragraph/datasets/climate_control_mg/climate_control_mg_nodes.csv
--rw-r--r--   0        0        0      443 2023-11-21 12:46:15.655766 ragraph-1.20.3/ragraph/datasets/compatibility/__init__.py
--rw-r--r--   0        0        0      564 2023-11-21 12:46:15.655766 ragraph-1.20.3/ragraph/datasets/compatibility/compatibility_edges.csv
--rw-r--r--   0        0        0       83 2023-11-21 12:46:15.655766 ragraph-1.20.3/ragraph/datasets/compatibility/compatibility_nodes.csv
--rw-r--r--   0        0        0      469 2023-11-21 12:46:15.655766 ragraph-1.20.3/ragraph/datasets/design/__init__.py
--rw-r--r--   0        0        0      872 2023-11-21 12:46:15.655766 ragraph-1.20.3/ragraph/datasets/design/design_edges.csv
--rw-r--r--   0        0        0      384 2023-11-21 12:46:15.655766 ragraph-1.20.3/ragraph/datasets/design/design_nodes.csv
--rw-r--r--   0        0        0     1008 2023-11-21 12:46:15.655766 ragraph-1.20.3/ragraph/datasets/elevator175/__init__.py
--rw-r--r--   0        0        0   103961 2023-11-21 12:46:15.655766 ragraph-1.20.3/ragraph/datasets/elevator175/elevator175_edges.csv
--rw-r--r--   0        0        0     7255 2023-11-21 12:46:15.655766 ragraph-1.20.3/ragraph/datasets/elevator175/elevator175_nodes.csv
--rw-r--r--   0        0        0     1007 2023-11-21 12:46:15.655766 ragraph-1.20.3/ragraph/datasets/elevator45/__init__.py
--rw-r--r--   0        0        0    29033 2023-11-21 12:46:15.656766 ragraph-1.20.3/ragraph/datasets/elevator45/elevator45_edges.csv
--rw-r--r--   0        0        0     1887 2023-11-21 12:46:15.656766 ragraph-1.20.3/ragraph/datasets/elevator45/elevator45_nodes.csv
--rw-r--r--   0        0        0     1197 2023-11-21 12:46:15.656766 ragraph-1.20.3/ragraph/datasets/esl/__init__.py
--rw-r--r--   0        0        0       75 2023-11-21 12:46:15.656766 ragraph-1.20.3/ragraph/datasets/esl/pump/__init__.py
--rw-r--r--   0        0        0     3523 2023-11-21 12:46:15.656766 ragraph-1.20.3/ragraph/datasets/esl/pump/pump.esl
--rw-r--r--   0        0        0     1918 2023-11-21 12:46:15.656766 ragraph-1.20.3/ragraph/datasets/ford_hood/__init__.py
--rw-r--r--   0        0        0    30483 2023-11-21 12:46:15.656766 ragraph-1.20.3/ragraph/datasets/ford_hood/ford_hood_edges.csv
--rw-r--r--   0        0        0     3339 2023-11-21 12:46:15.656766 ragraph-1.20.3/ragraph/datasets/ford_hood/ford_hood_nodes.csv
--rw-r--r--   0        0        0     1477 2023-11-21 12:46:15.656766 ragraph-1.20.3/ragraph/datasets/kodak3d/__init__.py
--rw-r--r--   0        0        0     6660 2023-11-21 12:46:15.656766 ragraph-1.20.3/ragraph/datasets/kodak3d/kodak3d_edges.csv
--rw-r--r--   0        0        0     1134 2023-11-21 12:46:15.656766 ragraph-1.20.3/ragraph/datasets/kodak3d/kodak3d_nodes.csv
--rw-r--r--   0        0        0      202 2023-11-21 12:46:15.656766 ragraph-1.20.3/ragraph/datasets/ledsip/__init__.py
--rw-r--r--   0        0        0   210027 2023-11-21 12:46:15.657766 ragraph-1.20.3/ragraph/datasets/ledsip/ledsip_edges.csv
--rw-r--r--   0        0        0    50840 2023-11-21 12:46:15.657766 ragraph-1.20.3/ragraph/datasets/ledsip/ledsip_nodes.csv
--rw-r--r--   0        0        0       75 2023-11-21 12:46:15.657766 ragraph-1.20.3/ragraph/datasets/localbus/__init__.py
--rw-r--r--   0        0        0      723 2023-11-21 12:46:15.657766 ragraph-1.20.3/ragraph/datasets/localbus/localbus_edges.csv
--rw-r--r--   0        0        0       27 2023-11-21 12:46:15.657766 ragraph-1.20.3/ragraph/datasets/localbus/localbus_nodes.csv
--rw-r--r--   0        0        0       59 2023-11-21 12:46:15.657766 ragraph-1.20.3/ragraph/datasets/mww_lock_aspect/__init__.py
--rw-r--r--   0        0        0    93289 2023-11-21 12:46:15.658766 ragraph-1.20.3/ragraph/datasets/mww_lock_aspect/mww_lock_aspect_edges.csv
--rw-r--r--   0        0        0     9178 2023-11-21 12:46:15.658766 ragraph-1.20.3/ragraph/datasets/mww_lock_aspect/mww_lock_aspect_nodes.csv
--rw-r--r--   0        0        0      136 2023-11-21 12:46:15.658766 ragraph-1.20.3/ragraph/datasets/mww_lock_eefde/__init__.py
--rw-r--r--   0        0        0   147721 2023-11-21 12:46:15.658766 ragraph-1.20.3/ragraph/datasets/mww_lock_eefde/mww_lock_eefde_edges.csv
--rw-r--r--   0        0        0     1388 2023-11-21 12:46:15.658766 ragraph-1.20.3/ragraph/datasets/mww_lock_eefde/mww_lock_eefde_nodes.csv
--rw-r--r--   0        0        0      140 2023-11-21 12:46:15.658766 ragraph-1.20.3/ragraph/datasets/mww_lock_hansweert/__init__.py
--rw-r--r--   0        0        0    54617 2023-11-21 12:46:15.658766 ragraph-1.20.3/ragraph/datasets/mww_lock_hansweert/mww_lock_hansweert_edges.csv
--rw-r--r--   0        0        0     1144 2023-11-21 12:46:15.659766 ragraph-1.20.3/ragraph/datasets/mww_lock_hansweert/mww_lock_hansweert_nodes.csv
--rw-r--r--   0        0        0      138 2023-11-21 12:46:15.659766 ragraph-1.20.3/ragraph/datasets/mww_lock_sambeek/__init__.py
--rw-r--r--   0        0        0    53667 2023-11-21 12:46:15.659766 ragraph-1.20.3/ragraph/datasets/mww_lock_sambeek/mww_lock_sambeek_edges.csv
--rw-r--r--   0        0        0     1123 2023-11-21 12:46:15.659766 ragraph-1.20.3/ragraph/datasets/mww_lock_sambeek/mww_lock_sambeek_nodes.csv
--rw-r--r--   0        0        0      139 2023-11-21 12:46:15.659766 ragraph-1.20.3/ragraph/datasets/mww_lock_sluis15/__init__.py
--rw-r--r--   0        0        0    54995 2023-11-21 12:46:15.659766 ragraph-1.20.3/ragraph/datasets/mww_lock_sluis15/mww_lock_sluis15_edges.csv
--rw-r--r--   0        0        0     1054 2023-11-21 12:46:15.659766 ragraph-1.20.3/ragraph/datasets/mww_lock_sluis15/mww_lock_sluis15_nodes.csv
--rw-r--r--   0        0        0       55 2023-11-21 12:46:15.660766 ragraph-1.20.3/ragraph/datasets/mww_lock_volkerak/__init__.py
--rw-r--r--   0        0        0    18120 2023-11-21 12:46:15.660766 ragraph-1.20.3/ragraph/datasets/mww_lock_volkerak/mww_lock_volkerak_edges.csv
--rw-r--r--   0        0        0     1216 2023-11-21 12:46:15.660766 ragraph-1.20.3/ragraph/datasets/mww_lock_volkerak/mww_lock_volkerak_nodes.csv
--rw-r--r--   0        0        0       76 2023-11-21 12:46:15.660766 ragraph-1.20.3/ragraph/datasets/overlap/__init__.py
--rw-r--r--   0        0        0      149 2023-11-21 12:46:15.660766 ragraph-1.20.3/ragraph/datasets/overlap/overlap_edges.csv
--rw-r--r--   0        0        0       15 2023-11-21 12:46:15.660766 ragraph-1.20.3/ragraph/datasets/overlap/overlap_nodes.csv
--rw-r--r--   0        0        0     2149 2023-11-21 12:46:15.660766 ragraph-1.20.3/ragraph/datasets/pathfinder/__init__.py
--rw-r--r--   0        0        0    17741 2023-11-21 12:46:15.660766 ragraph-1.20.3/ragraph/datasets/pathfinder/pathfinder_edges.csv
--rw-r--r--   0        0        0     1084 2023-11-21 12:46:15.660766 ragraph-1.20.3/ragraph/datasets/pathfinder/pathfinder_nodes.csv
--rw-r--r--   0        0        0      353 2023-11-21 12:46:15.660766 ragraph-1.20.3/ragraph/datasets/shaja8/__init__.py
--rw-r--r--   0        0        0      243 2023-11-21 12:46:15.660766 ragraph-1.20.3/ragraph/datasets/shaja8/shaja8_edges.csv
--rw-r--r--   0        0        0       21 2023-11-21 12:46:15.660766 ragraph-1.20.3/ragraph/datasets/shaja8/shaja8_nodes.csv
--rw-r--r--   0        0        0      255 2023-11-21 12:46:15.661766 ragraph-1.20.3/ragraph/datasets/similarity/__init__.py
--rw-r--r--   0        0        0      872 2023-11-21 12:46:15.661766 ragraph-1.20.3/ragraph/datasets/similarity/similarity_edges.csv
--rw-r--r--   0        0        0      360 2023-11-21 12:46:15.661766 ragraph-1.20.3/ragraph/datasets/similarity/similarity_nodes.csv
--rw-r--r--   0        0        0      289 2023-11-21 12:46:15.661766 ragraph-1.20.3/ragraph/datasets/tarjans8/__init__.py
--rw-r--r--   0        0        0      199 2023-11-21 12:46:15.661766 ragraph-1.20.3/ragraph/datasets/tarjans8/tarjans8_edges.csv
--rw-r--r--   0        0        0       21 2023-11-21 12:46:15.661766 ragraph-1.20.3/ragraph/datasets/tarjans8/tarjans8_nodes.csv
--rw-r--r--   0        0        0     3788 2023-11-21 12:46:15.661766 ragraph-1.20.3/ragraph/datasets/tss_electric/__init__.py
--rw-r--r--   0        0        0     2805 2023-11-21 12:46:15.661766 ragraph-1.20.3/ragraph/datasets/tss_electric/tss_electric_edges.csv
--rw-r--r--   0        0        0      592 2023-11-21 12:46:15.661766 ragraph-1.20.3/ragraph/datasets/tss_electric/tss_electric_nodes.csv
--rw-r--r--   0        0        0     3893 2023-11-21 12:46:15.661766 ragraph-1.20.3/ragraph/datasets/tss_front/__init__.py
--rw-r--r--   0        0        0    29801 2023-11-21 12:46:15.661766 ragraph-1.20.3/ragraph/datasets/tss_front/tss_front_edges.csv
--rw-r--r--   0        0        0     1919 2023-11-21 12:46:15.661766 ragraph-1.20.3/ragraph/datasets/tss_front/tss_front_nodes.csv
--rw-r--r--   0        0        0     3789 2023-11-21 12:46:15.661766 ragraph-1.20.3/ragraph/datasets/tss_hydraulic/__init__.py
--rw-r--r--   0        0        0     3663 2023-11-21 12:46:15.661766 ragraph-1.20.3/ragraph/datasets/tss_hydraulic/tss_hydraulic_edges.csv
--rw-r--r--   0        0        0      863 2023-11-21 12:46:15.661766 ragraph-1.20.3/ragraph/datasets/tss_hydraulic/tss_hydraulic_nodes.csv
--rw-r--r--   0        0        0     1493 2023-11-21 12:46:15.661766 ragraph-1.20.3/ragraph/datasets/ucav/__init__.py
--rw-r--r--   0        0        0     5183 2023-11-21 12:46:15.662766 ragraph-1.20.3/ragraph/datasets/ucav/ucav_edges.csv
--rw-r--r--   0        0        0     1141 2023-11-21 12:46:15.662766 ragraph-1.20.3/ragraph/datasets/ucav/ucav_nodes.csv
--rw-r--r--   0        0        0     4410 2023-11-21 12:46:15.662766 ragraph-1.20.3/ragraph/edge.py
--rw-r--r--   0        0        0    23116 2023-11-21 12:46:15.662766 ragraph-1.20.3/ragraph/generic.py
--rw-r--r--   0        0        0    39457 2023-11-21 12:46:15.662766 ragraph-1.20.3/ragraph/graph.py
--rw-r--r--   0        0        0       76 2023-11-21 12:46:15.662766 ragraph-1.20.3/ragraph/io/__init__.py
--rw-r--r--   0        0        0    11788 2023-11-21 12:46:15.662766 ragraph-1.20.3/ragraph/io/archimate/__init__.py
--rw-r--r--   0        0        0    48350 2023-11-21 12:46:15.663766 ragraph-1.20.3/ragraph/io/archimate/archimate3_Model.xsd
--rw-r--r--   0        0        0      461 2023-11-21 12:46:15.663766 ragraph-1.20.3/ragraph/io/archimate/bare.xml
--rw-r--r--   0        0        0     8836 2023-11-21 12:46:15.663766 ragraph-1.20.3/ragraph/io/archimate/xml.xsd
--rw-r--r--   0        0        0     6747 2023-11-21 12:46:15.663766 ragraph-1.20.3/ragraph/io/canopy.py
--rw-r--r--   0        0        0    14031 2023-11-21 12:46:15.663766 ragraph-1.20.3/ragraph/io/csv.py
--rw-r--r--   0        0        0      527 2023-11-21 12:46:15.663766 ragraph-1.20.3/ragraph/io/esl.py
--rw-r--r--   0        0        0    28634 2023-11-21 12:46:15.663766 ragraph-1.20.3/ragraph/io/grip.py
--rw-r--r--   0        0        0     4136 2023-11-21 12:46:15.663766 ragraph-1.20.3/ragraph/io/json.py
--rw-r--r--   0        0        0     5150 2023-11-21 12:46:15.663766 ragraph-1.20.3/ragraph/io/matrix.py
--rw-r--r--   0        0        0     1819 2023-11-21 12:46:15.663766 ragraph-1.20.3/ragraph/io/xml/XMI-Canonical.xsd
--rw-r--r--   0        0        0     9263 2023-11-21 12:46:15.663766 ragraph-1.20.3/ragraph/io/xml/__init__.py
--rw-r--r--   0        0        0      358 2023-11-21 12:46:15.663766 ragraph-1.20.3/ragraph/io/xml/bare.xml
--rw-r--r--   0        0        0     4332 2023-11-21 12:46:15.663766 ragraph-1.20.3/ragraph/io/xml/ragraph.xsd
--rw-r--r--   0        0        0     1269 2023-11-21 12:46:15.663766 ragraph-1.20.3/ragraph/io/yaml.py
--rw-r--r--   0        0        0     7924 2023-11-21 12:46:15.664766 ragraph-1.20.3/ragraph/node.py
--rw-r--r--   0        0        0     4369 2023-11-21 12:46:15.664766 ragraph-1.20.3/ragraph/plot/__init__.py
--rw-r--r--   0        0        0      526 2023-11-21 12:46:15.664766 ragraph-1.20.3/ragraph/plot/components/__init__.py
--rw-r--r--   0        0        0     1219 2023-11-21 12:46:15.664766 ragraph-1.20.3/ragraph/plot/components/blank.py
--rw-r--r--   0        0        0     3831 2023-11-21 12:46:15.664766 ragraph-1.20.3/ragraph/plot/components/labels.py
--rw-r--r--   0        0        0     9173 2023-11-21 12:46:15.664766 ragraph-1.20.3/ragraph/plot/components/legend.py
--rw-r--r--   0        0        0    20692 2023-11-21 12:46:15.664766 ragraph-1.20.3/ragraph/plot/components/piemap.py
--rw-r--r--   0        0        0     6910 2023-11-21 12:46:15.664766 ragraph-1.20.3/ragraph/plot/components/tree.py
--rw-r--r--   0        0        0    28974 2023-11-21 12:46:15.664766 ragraph-1.20.3/ragraph/plot/generic.py
--rw-r--r--   0        0        0    10320 2023-11-21 12:46:15.664766 ragraph-1.20.3/ragraph/plot/svg.py
--rw-r--r--   0        0        0     9310 2023-11-21 12:46:15.665766 ragraph-1.20.3/ragraph/plot/utils.py
--rw-r--r--   0        0        0     3169 2023-11-21 12:46:15.665766 ragraph-1.20.3/ragraph/utils.py
--rw-r--r--   0        0        0     3344 1970-01-01 00:00:00.000000 ragraph-1.20.3/PKG-INFO
+-rw-r--r--   0        0        0    34753 2024-04-29 12:02:22.799085 ragraph-1.21.0/LICENSE-GPL
+-rw-r--r--   0        0        0     2144 2024-04-29 12:02:22.799085 ragraph-1.21.0/README.md
+-rw-r--r--   0        0        0     2003 2024-04-29 12:02:22.805086 ragraph-1.21.0/pyproject.toml
+-rw-r--r--   0        0        0       72 2024-04-29 12:02:22.805086 ragraph-1.21.0/ragraph/__init__.py
+-rw-r--r--   0        0        0      138 2024-04-29 12:02:22.805086 ragraph-1.21.0/ragraph/analysis/__init__.py
+-rw-r--r--   0        0        0    19876 2024-04-29 12:02:22.805086 ragraph-1.21.0/ragraph/analysis/_classes.py
+-rw-r--r--   0        0        0     7950 2024-04-29 12:02:22.805086 ragraph-1.21.0/ragraph/analysis/_utils.py
+-rw-r--r--   0        0        0     1008 2024-04-29 12:02:22.805086 ragraph-1.21.0/ragraph/analysis/bus/__init__.py
+-rw-r--r--   0        0        0     4020 2024-04-29 12:02:22.805086 ragraph-1.21.0/ragraph/analysis/bus/_gamma.py
+-rw-r--r--   0        0        0     1376 2024-04-29 12:02:22.805086 ragraph-1.21.0/ragraph/analysis/cluster/__init__.py
+-rw-r--r--   0        0        0    13980 2024-04-29 12:02:22.805086 ragraph-1.21.0/ragraph/analysis/cluster/_markov.py
+-rw-r--r--   0        0        0     3471 2024-04-29 12:02:22.806085 ragraph-1.21.0/ragraph/analysis/cluster/_tarjan.py
+-rw-r--r--   0        0        0     1201 2024-04-29 12:02:22.806085 ragraph-1.21.0/ragraph/analysis/comparison/__init__.py
+-rw-r--r--   0        0        0     2539 2024-04-29 12:02:22.806085 ragraph-1.21.0/ragraph/analysis/comparison/_delta.py
+-rw-r--r--   0        0        0     6462 2024-04-29 12:02:22.806085 ragraph-1.21.0/ragraph/analysis/comparison/_sigma.py
+-rw-r--r--   0        0        0     3728 2024-04-29 12:02:22.806085 ragraph-1.21.0/ragraph/analysis/comparison/utils.py
+-rw-r--r--   0        0        0    20554 2024-04-29 12:02:22.806085 ragraph-1.21.0/ragraph/analysis/compatibility/__init__.py
+-rw-r--r--   0        0        0     2790 2024-04-29 12:02:22.806085 ragraph-1.21.0/ragraph/analysis/compatibility/bdd.py
+-rw-r--r--   0        0        0      649 2024-04-29 12:02:22.806085 ragraph-1.21.0/ragraph/analysis/heuristics/__init__.py
+-rw-r--r--   0        0        0     3352 2024-04-29 12:02:22.806085 ragraph-1.21.0/ragraph/analysis/heuristics/_johnson.py
+-rw-r--r--   0        0        0     5080 2024-04-29 12:02:22.806085 ragraph-1.21.0/ragraph/analysis/heuristics/_markov_gamma.py
+-rw-r--r--   0        0        0     2166 2024-04-29 12:02:22.806085 ragraph-1.21.0/ragraph/analysis/sequence/__init__.py
+-rw-r--r--   0        0        0    10934 2024-04-29 12:02:22.806085 ragraph-1.21.0/ragraph/analysis/sequence/_axis.py
+-rw-r--r--   0        0        0     5252 2024-04-29 12:02:22.807086 ragraph-1.21.0/ragraph/analysis/sequence/_genetic.py
+-rw-r--r--   0        0        0     3026 2024-04-29 12:02:22.807086 ragraph-1.21.0/ragraph/analysis/sequence/_markov.py
+-rw-r--r--   0        0        0      833 2024-04-29 12:02:22.807086 ragraph-1.21.0/ragraph/analysis/sequence/_name.py
+-rw-r--r--   0        0        0     3776 2024-04-29 12:02:22.807086 ragraph-1.21.0/ragraph/analysis/sequence/_scc_tearing.py
+-rw-r--r--   0        0        0     1728 2024-04-29 12:02:22.807086 ragraph-1.21.0/ragraph/analysis/sequence/_tarjan.py
+-rw-r--r--   0        0        0     7130 2024-04-29 12:02:22.807086 ragraph-1.21.0/ragraph/analysis/sequence/metrics.py
+-rw-r--r--   0        0        0     5246 2024-04-29 12:02:22.807086 ragraph-1.21.0/ragraph/analysis/sequence/utils.py
+-rw-r--r--   0        0        0     1460 2024-04-29 12:02:22.807086 ragraph-1.21.0/ragraph/analysis/similarity/__init__.py
+-rw-r--r--   0        0        0     3103 2024-04-29 12:02:22.807086 ragraph-1.21.0/ragraph/analysis/similarity/_jaccard.py
+-rw-r--r--   0        0        0     9923 2024-04-29 12:02:22.807086 ragraph-1.21.0/ragraph/analysis/similarity/_similarity.py
+-rw-r--r--   0        0        0     1827 2024-04-29 12:02:22.807086 ragraph-1.21.0/ragraph/analysis/similarity/utils.py
+-rw-r--r--   0        0        0    10266 2024-04-29 12:02:22.807086 ragraph-1.21.0/ragraph/colors/__init__.py
+-rw-r--r--   0        0        0     5447 2024-04-29 12:02:22.807086 ragraph-1.21.0/ragraph/colors/cubehelix.py
+-rw-r--r--   0        0        0      770 2024-04-29 12:02:22.807086 ragraph-1.21.0/ragraph/colors/utils.py
+-rw-r--r--   0        0        0     1589 2024-04-29 12:02:22.808086 ragraph-1.21.0/ragraph/datasets/__init__.py
+-rw-r--r--   0        0        0      679 2024-04-29 12:02:22.808086 ragraph-1.21.0/ragraph/datasets/aircraft_engine/__init__.py
+-rw-r--r--   0        0        0    28938 2024-04-29 12:02:22.808086 ragraph-1.21.0/ragraph/datasets/aircraft_engine/aircraft_engine_edges.csv
+-rw-r--r--   0        0        0      977 2024-04-29 12:02:22.808086 ragraph-1.21.0/ragraph/datasets/aircraft_engine/aircraft_engine_nodes.csv
+-rw-r--r--   0        0        0     1073 2024-04-29 12:02:22.808086 ragraph-1.21.0/ragraph/datasets/architecture_integral/__init__.py
+-rw-r--r--   0        0        0     1364 2024-04-29 12:02:22.808086 ragraph-1.21.0/ragraph/datasets/architecture_integral/architecture_integral_edges.csv
+-rw-r--r--   0        0        0      352 2024-04-29 12:02:22.808086 ragraph-1.21.0/ragraph/datasets/architecture_integral/architecture_integral_nodes.csv
+-rw-r--r--   0        0        0     1083 2024-04-29 12:02:22.808086 ragraph-1.21.0/ragraph/datasets/architecture_mix/__init__.py
+-rw-r--r--   0        0        0     2264 2024-04-29 12:02:22.808086 ragraph-1.21.0/ragraph/datasets/architecture_mix/architecture_mix_edges.csv
+-rw-r--r--   0        0        0      352 2024-04-29 12:02:22.808086 ragraph-1.21.0/ragraph/datasets/architecture_mix/architecture_mix_nodes.csv
+-rw-r--r--   0        0        0     1079 2024-04-29 12:02:22.808086 ragraph-1.21.0/ragraph/datasets/architecture_modular/__init__.py
+-rw-r--r--   0        0        0     2722 2024-04-29 12:02:22.808086 ragraph-1.21.0/ragraph/datasets/architecture_modular/architecture_modular_edges.csv
+-rw-r--r--   0        0        0      351 2024-04-29 12:02:22.808086 ragraph-1.21.0/ragraph/datasets/architecture_modular/architecture_modular_nodes.csv
+-rw-r--r--   0        0        0      821 2024-04-29 12:02:22.808086 ragraph-1.21.0/ragraph/datasets/climate_control/__init__.py
+-rw-r--r--   0        0        0     5778 2024-04-29 12:02:22.808086 ragraph-1.21.0/ragraph/datasets/climate_control/climate_control_edges.csv
+-rw-r--r--   0        0        0      632 2024-04-29 12:02:22.808086 ragraph-1.21.0/ragraph/datasets/climate_control/climate_control_nodes.csv
+-rw-r--r--   0        0        0      422 2024-04-29 12:02:22.808086 ragraph-1.21.0/ragraph/datasets/climate_control_mg/__init__.py
+-rw-r--r--   0        0        0     5778 2024-04-29 12:02:22.809085 ragraph-1.21.0/ragraph/datasets/climate_control_mg/climate_control_mg_edges.csv
+-rw-r--r--   0        0        0     1441 2024-04-29 12:02:22.809085 ragraph-1.21.0/ragraph/datasets/climate_control_mg/climate_control_mg_nodes.csv
+-rw-r--r--   0        0        0      443 2024-04-29 12:02:22.809085 ragraph-1.21.0/ragraph/datasets/compatibility/__init__.py
+-rw-r--r--   0        0        0      564 2024-04-29 12:02:22.809085 ragraph-1.21.0/ragraph/datasets/compatibility/compatibility_edges.csv
+-rw-r--r--   0        0        0       83 2024-04-29 12:02:22.809085 ragraph-1.21.0/ragraph/datasets/compatibility/compatibility_nodes.csv
+-rw-r--r--   0        0        0      469 2024-04-29 12:02:22.809085 ragraph-1.21.0/ragraph/datasets/design/__init__.py
+-rw-r--r--   0        0        0      872 2024-04-29 12:02:22.809085 ragraph-1.21.0/ragraph/datasets/design/design_edges.csv
+-rw-r--r--   0        0        0      384 2024-04-29 12:02:22.809085 ragraph-1.21.0/ragraph/datasets/design/design_nodes.csv
+-rw-r--r--   0        0        0     1008 2024-04-29 12:02:22.809085 ragraph-1.21.0/ragraph/datasets/elevator175/__init__.py
+-rw-r--r--   0        0        0   103961 2024-04-29 12:02:22.809085 ragraph-1.21.0/ragraph/datasets/elevator175/elevator175_edges.csv
+-rw-r--r--   0        0        0     7255 2024-04-29 12:02:22.809085 ragraph-1.21.0/ragraph/datasets/elevator175/elevator175_nodes.csv
+-rw-r--r--   0        0        0     1007 2024-04-29 12:02:22.809085 ragraph-1.21.0/ragraph/datasets/elevator45/__init__.py
+-rw-r--r--   0        0        0    29033 2024-04-29 12:02:22.809085 ragraph-1.21.0/ragraph/datasets/elevator45/elevator45_edges.csv
+-rw-r--r--   0        0        0     1887 2024-04-29 12:02:22.809085 ragraph-1.21.0/ragraph/datasets/elevator45/elevator45_nodes.csv
+-rw-r--r--   0        0        0     1198 2024-04-29 12:02:22.810085 ragraph-1.21.0/ragraph/datasets/esl/__init__.py
+-rw-r--r--   0        0        0       75 2024-04-29 12:02:22.810085 ragraph-1.21.0/ragraph/datasets/esl/pump/__init__.py
+-rw-r--r--   0        0        0     3523 2024-04-29 12:02:22.810085 ragraph-1.21.0/ragraph/datasets/esl/pump/pump.esl
+-rw-r--r--   0        0        0     1917 2024-04-29 12:02:22.810085 ragraph-1.21.0/ragraph/datasets/ford_hood/__init__.py
+-rw-r--r--   0        0        0    30483 2024-04-29 12:02:22.810085 ragraph-1.21.0/ragraph/datasets/ford_hood/ford_hood_edges.csv
+-rw-r--r--   0        0        0     3339 2024-04-29 12:02:22.810085 ragraph-1.21.0/ragraph/datasets/ford_hood/ford_hood_nodes.csv
+-rw-r--r--   0        0        0     1476 2024-04-29 12:02:22.810085 ragraph-1.21.0/ragraph/datasets/kodak3d/__init__.py
+-rw-r--r--   0        0        0     6660 2024-04-29 12:02:22.810085 ragraph-1.21.0/ragraph/datasets/kodak3d/kodak3d_edges.csv
+-rw-r--r--   0        0        0     1134 2024-04-29 12:02:22.810085 ragraph-1.21.0/ragraph/datasets/kodak3d/kodak3d_nodes.csv
+-rw-r--r--   0        0        0      202 2024-04-29 12:02:22.810085 ragraph-1.21.0/ragraph/datasets/ledsip/__init__.py
+-rw-r--r--   0        0        0   210027 2024-04-29 12:02:22.811086 ragraph-1.21.0/ragraph/datasets/ledsip/ledsip_edges.csv
+-rw-r--r--   0        0        0    50840 2024-04-29 12:02:22.811086 ragraph-1.21.0/ragraph/datasets/ledsip/ledsip_nodes.csv
+-rw-r--r--   0        0        0       75 2024-04-29 12:02:22.811086 ragraph-1.21.0/ragraph/datasets/localbus/__init__.py
+-rw-r--r--   0        0        0      723 2024-04-29 12:02:22.811086 ragraph-1.21.0/ragraph/datasets/localbus/localbus_edges.csv
+-rw-r--r--   0        0        0       27 2024-04-29 12:02:22.811086 ragraph-1.21.0/ragraph/datasets/localbus/localbus_nodes.csv
+-rw-r--r--   0        0        0       59 2024-04-29 12:02:22.811086 ragraph-1.21.0/ragraph/datasets/mww_lock_aspect/__init__.py
+-rw-r--r--   0        0        0    93289 2024-04-29 12:02:22.811086 ragraph-1.21.0/ragraph/datasets/mww_lock_aspect/mww_lock_aspect_edges.csv
+-rw-r--r--   0        0        0     9178 2024-04-29 12:02:22.811086 ragraph-1.21.0/ragraph/datasets/mww_lock_aspect/mww_lock_aspect_nodes.csv
+-rw-r--r--   0        0        0      136 2024-04-29 12:02:22.811086 ragraph-1.21.0/ragraph/datasets/mww_lock_eefde/__init__.py
+-rw-r--r--   0        0        0   147721 2024-04-29 12:02:22.812085 ragraph-1.21.0/ragraph/datasets/mww_lock_eefde/mww_lock_eefde_edges.csv
+-rw-r--r--   0        0        0     1388 2024-04-29 12:02:22.812085 ragraph-1.21.0/ragraph/datasets/mww_lock_eefde/mww_lock_eefde_nodes.csv
+-rw-r--r--   0        0        0      140 2024-04-29 12:02:22.812085 ragraph-1.21.0/ragraph/datasets/mww_lock_hansweert/__init__.py
+-rw-r--r--   0        0        0    54617 2024-04-29 12:02:22.812085 ragraph-1.21.0/ragraph/datasets/mww_lock_hansweert/mww_lock_hansweert_edges.csv
+-rw-r--r--   0        0        0     1144 2024-04-29 12:02:22.812085 ragraph-1.21.0/ragraph/datasets/mww_lock_hansweert/mww_lock_hansweert_nodes.csv
+-rw-r--r--   0        0        0      138 2024-04-29 12:02:22.812085 ragraph-1.21.0/ragraph/datasets/mww_lock_sambeek/__init__.py
+-rw-r--r--   0        0        0    53667 2024-04-29 12:02:22.812085 ragraph-1.21.0/ragraph/datasets/mww_lock_sambeek/mww_lock_sambeek_edges.csv
+-rw-r--r--   0        0        0     1123 2024-04-29 12:02:22.812085 ragraph-1.21.0/ragraph/datasets/mww_lock_sambeek/mww_lock_sambeek_nodes.csv
+-rw-r--r--   0        0        0      139 2024-04-29 12:02:22.812085 ragraph-1.21.0/ragraph/datasets/mww_lock_sluis15/__init__.py
+-rw-r--r--   0        0        0    54995 2024-04-29 12:02:22.813085 ragraph-1.21.0/ragraph/datasets/mww_lock_sluis15/mww_lock_sluis15_edges.csv
+-rw-r--r--   0        0        0     1054 2024-04-29 12:02:22.813085 ragraph-1.21.0/ragraph/datasets/mww_lock_sluis15/mww_lock_sluis15_nodes.csv
+-rw-r--r--   0        0        0       55 2024-04-29 12:02:22.813085 ragraph-1.21.0/ragraph/datasets/mww_lock_volkerak/__init__.py
+-rw-r--r--   0        0        0    18120 2024-04-29 12:02:22.813085 ragraph-1.21.0/ragraph/datasets/mww_lock_volkerak/mww_lock_volkerak_edges.csv
+-rw-r--r--   0        0        0     1216 2024-04-29 12:02:22.813085 ragraph-1.21.0/ragraph/datasets/mww_lock_volkerak/mww_lock_volkerak_nodes.csv
+-rw-r--r--   0        0        0       76 2024-04-29 12:02:22.813085 ragraph-1.21.0/ragraph/datasets/overlap/__init__.py
+-rw-r--r--   0        0        0      149 2024-04-29 12:02:22.813085 ragraph-1.21.0/ragraph/datasets/overlap/overlap_edges.csv
+-rw-r--r--   0        0        0       15 2024-04-29 12:02:22.813085 ragraph-1.21.0/ragraph/datasets/overlap/overlap_nodes.csv
+-rw-r--r--   0        0        0     2149 2024-04-29 12:02:22.813085 ragraph-1.21.0/ragraph/datasets/pathfinder/__init__.py
+-rw-r--r--   0        0        0    17741 2024-04-29 12:02:22.814086 ragraph-1.21.0/ragraph/datasets/pathfinder/pathfinder_edges.csv
+-rw-r--r--   0        0        0     1084 2024-04-29 12:02:22.814086 ragraph-1.21.0/ragraph/datasets/pathfinder/pathfinder_nodes.csv
+-rw-r--r--   0        0        0      353 2024-04-29 12:02:22.814086 ragraph-1.21.0/ragraph/datasets/shaja8/__init__.py
+-rw-r--r--   0        0        0      243 2024-04-29 12:02:22.814086 ragraph-1.21.0/ragraph/datasets/shaja8/shaja8_edges.csv
+-rw-r--r--   0        0        0       21 2024-04-29 12:02:22.814086 ragraph-1.21.0/ragraph/datasets/shaja8/shaja8_nodes.csv
+-rw-r--r--   0        0        0      255 2024-04-29 12:02:22.814086 ragraph-1.21.0/ragraph/datasets/similarity/__init__.py
+-rw-r--r--   0        0        0      872 2024-04-29 12:02:22.814086 ragraph-1.21.0/ragraph/datasets/similarity/similarity_edges.csv
+-rw-r--r--   0        0        0      360 2024-04-29 12:02:22.814086 ragraph-1.21.0/ragraph/datasets/similarity/similarity_nodes.csv
+-rw-r--r--   0        0        0      289 2024-04-29 12:02:22.814086 ragraph-1.21.0/ragraph/datasets/tarjans8/__init__.py
+-rw-r--r--   0        0        0      199 2024-04-29 12:02:22.814086 ragraph-1.21.0/ragraph/datasets/tarjans8/tarjans8_edges.csv
+-rw-r--r--   0        0        0       21 2024-04-29 12:02:22.814086 ragraph-1.21.0/ragraph/datasets/tarjans8/tarjans8_nodes.csv
+-rw-r--r--   0        0        0     3788 2024-04-29 12:02:22.814086 ragraph-1.21.0/ragraph/datasets/tss_electric/__init__.py
+-rw-r--r--   0        0        0     2805 2024-04-29 12:02:22.814086 ragraph-1.21.0/ragraph/datasets/tss_electric/tss_electric_edges.csv
+-rw-r--r--   0        0        0      592 2024-04-29 12:02:22.814086 ragraph-1.21.0/ragraph/datasets/tss_electric/tss_electric_nodes.csv
+-rw-r--r--   0        0        0     3893 2024-04-29 12:02:22.814086 ragraph-1.21.0/ragraph/datasets/tss_front/__init__.py
+-rw-r--r--   0        0        0    29801 2024-04-29 12:02:22.814086 ragraph-1.21.0/ragraph/datasets/tss_front/tss_front_edges.csv
+-rw-r--r--   0        0        0     1919 2024-04-29 12:02:22.814086 ragraph-1.21.0/ragraph/datasets/tss_front/tss_front_nodes.csv
+-rw-r--r--   0        0        0     3789 2024-04-29 12:02:22.814086 ragraph-1.21.0/ragraph/datasets/tss_hydraulic/__init__.py
+-rw-r--r--   0        0        0     3663 2024-04-29 12:02:22.814086 ragraph-1.21.0/ragraph/datasets/tss_hydraulic/tss_hydraulic_edges.csv
+-rw-r--r--   0        0        0      863 2024-04-29 12:02:22.815086 ragraph-1.21.0/ragraph/datasets/tss_hydraulic/tss_hydraulic_nodes.csv
+-rw-r--r--   0        0        0     1493 2024-04-29 12:02:22.815086 ragraph-1.21.0/ragraph/datasets/ucav/__init__.py
+-rw-r--r--   0        0        0     5183 2024-04-29 12:02:22.815086 ragraph-1.21.0/ragraph/datasets/ucav/ucav_edges.csv
+-rw-r--r--   0        0        0     1141 2024-04-29 12:02:22.815086 ragraph-1.21.0/ragraph/datasets/ucav/ucav_nodes.csv
+-rw-r--r--   0        0        0     4410 2024-04-29 12:02:22.815086 ragraph-1.21.0/ragraph/edge.py
+-rw-r--r--   0        0        0    23718 2024-04-29 12:02:22.815086 ragraph-1.21.0/ragraph/generic.py
+-rw-r--r--   0        0        0    40322 2024-04-29 12:02:22.815086 ragraph-1.21.0/ragraph/graph.py
+-rw-r--r--   0        0        0       76 2024-04-29 12:02:22.815086 ragraph-1.21.0/ragraph/io/__init__.py
+-rw-r--r--   0        0        0    11789 2024-04-29 12:02:22.815086 ragraph-1.21.0/ragraph/io/archimate/__init__.py
+-rw-r--r--   0        0        0    48350 2024-04-29 12:02:22.816085 ragraph-1.21.0/ragraph/io/archimate/archimate3_Model.xsd
+-rw-r--r--   0        0        0      461 2024-04-29 12:02:22.816085 ragraph-1.21.0/ragraph/io/archimate/bare.xml
+-rw-r--r--   0        0        0     8836 2024-04-29 12:02:22.816085 ragraph-1.21.0/ragraph/io/archimate/xml.xsd
+-rw-r--r--   0        0        0     6745 2024-04-29 12:02:22.816085 ragraph-1.21.0/ragraph/io/canopy.py
+-rw-r--r--   0        0        0    14031 2024-04-29 12:02:22.816085 ragraph-1.21.0/ragraph/io/csv.py
+-rw-r--r--   0        0        0      527 2024-04-29 12:02:22.816085 ragraph-1.21.0/ragraph/io/esl.py
+-rw-r--r--   0        0        0    29676 2024-04-29 12:02:22.816085 ragraph-1.21.0/ragraph/io/grip.py
+-rw-r--r--   0        0        0     4137 2024-04-29 12:02:22.816085 ragraph-1.21.0/ragraph/io/json.py
+-rw-r--r--   0        0        0     6214 2024-04-29 12:02:22.816085 ragraph-1.21.0/ragraph/io/matrix.py
+-rw-r--r--   0        0        0     1819 2024-04-29 12:02:22.816085 ragraph-1.21.0/ragraph/io/xml/XMI-Canonical.xsd
+-rw-r--r--   0        0        0     9264 2024-04-29 12:02:22.816085 ragraph-1.21.0/ragraph/io/xml/__init__.py
+-rw-r--r--   0        0        0      358 2024-04-29 12:02:22.816085 ragraph-1.21.0/ragraph/io/xml/bare.xml
+-rw-r--r--   0        0        0     4332 2024-04-29 12:02:22.816085 ragraph-1.21.0/ragraph/io/xml/ragraph.xsd
+-rw-r--r--   0        0        0     1270 2024-04-29 12:02:22.816085 ragraph-1.21.0/ragraph/io/yaml.py
+-rw-r--r--   0        0        0     7924 2024-04-29 12:02:22.817086 ragraph-1.21.0/ragraph/node.py
+-rw-r--r--   0        0        0     4370 2024-04-29 12:02:22.817086 ragraph-1.21.0/ragraph/plot/__init__.py
+-rw-r--r--   0        0        0      526 2024-04-29 12:02:22.817086 ragraph-1.21.0/ragraph/plot/components/__init__.py
+-rw-r--r--   0        0        0     1219 2024-04-29 12:02:22.817086 ragraph-1.21.0/ragraph/plot/components/blank.py
+-rw-r--r--   0        0        0     3832 2024-04-29 12:02:22.817086 ragraph-1.21.0/ragraph/plot/components/labels.py
+-rw-r--r--   0        0        0     9173 2024-04-29 12:02:22.817086 ragraph-1.21.0/ragraph/plot/components/legend.py
+-rw-r--r--   0        0        0    21644 2024-04-29 12:02:22.817086 ragraph-1.21.0/ragraph/plot/components/piemap.py
+-rw-r--r--   0        0        0     6911 2024-04-29 12:02:22.817086 ragraph-1.21.0/ragraph/plot/components/tree.py
+-rw-r--r--   0        0        0    29279 2024-04-29 12:02:22.817086 ragraph-1.21.0/ragraph/plot/generic.py
+-rw-r--r--   0        0        0    10321 2024-04-29 12:02:22.817086 ragraph-1.21.0/ragraph/plot/svg.py
+-rw-r--r--   0        0        0     9487 2024-04-29 12:02:22.817086 ragraph-1.21.0/ragraph/plot/utils.py
+-rw-r--r--   0        0        0     3170 2024-04-29 12:02:22.818086 ragraph-1.21.0/ragraph/utils.py
+-rw-r--r--   0        0        0     3344 1970-01-01 00:00:00.000000 ragraph-1.21.0/PKG-INFO
```

### Comparing `ragraph-1.20.3/LICENSE-GPL` & `ragraph-1.21.0/LICENSE-GPL`

 * *Files identical despite different names*

### Comparing `ragraph-1.20.3/README.md` & `ragraph-1.21.0/README.md`

 * *Files identical despite different names*

### Comparing `ragraph-1.20.3/pyproject.toml` & `ragraph-1.21.0/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
 name = "ragraph"
-version = "1.20.3"
+version = "1.21.0"
 description = "Ratio graph handling in Python."
 authors = ["Ratio Innovations B.V. <info@ratio-case.nl>"]
 license = "GPL-3.0-or-later"
 documentation = "https://ragraph.ratio-case.nl"
 readme = "README.md"
 repository = "https://gitlab.com/ratio-case-os/python/ragraph"
 homepage = "https://ragraph.ratio-case.nl"
@@ -16,15 +16,15 @@
 [tool.poetry.dependencies]
 python = "^3.9"
 dd = { version = "^0.5" }
 lxml = { version = "^4" }
 numpy = { version = "^1" }
 plotly = { version = "^5" }
 "ruamel.yaml" = "*"
-strenum = { version = "*", python = "<3.11"}
+strenum = { version = "*", python = "<3.11" }
 kaleido = { version = "0.2.1", optional = true }
 raesl = { version = "^0", optional = true }
 ratio-genetic-py = "^0.3"
 
 [tool.poetry.extras]
 esl = ["raesl"]
 plot = ["kaleido"]
@@ -74,12 +74,12 @@
 
 [tool.raver]
 ref = "origin/main"
 changelog = "./docs/CHANGELOG.md"
 
 [tool.ruff]
 line-length = 100
-select = [
+lint.select = [
     "E", # pycodestyle
     "F", # pyflakes
 ]
 target-version = "py39"
```

### Comparing `ragraph-1.20.3/ragraph/analysis/_classes.py` & `ragraph-1.21.0/ragraph/analysis/_classes.py`

 * *Files identical despite different names*

### Comparing `ragraph-1.20.3/ragraph/analysis/_utils.py` & `ragraph-1.21.0/ragraph/analysis/_utils.py`

 * *Files identical despite different names*

### Comparing `ragraph-1.20.3/ragraph/analysis/bus/__init__.py` & `ragraph-1.21.0/ragraph/analysis/bus/__init__.py`

 * *Files identical despite different names*

### Comparing `ragraph-1.20.3/ragraph/analysis/bus/_gamma.py` & `ragraph-1.21.0/ragraph/analysis/bus/_gamma.py`

 * *Files identical despite different names*

### Comparing `ragraph-1.20.3/ragraph/analysis/cluster/__init__.py` & `ragraph-1.21.0/ragraph/analysis/cluster/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -14,15 +14,15 @@
   graph or provided a deepcopy of the graph with only the leaf nodes, their edges and
   newly created cluster nodes.
 
 ## Available algorithms
 
 - [`markov`][ragraph.analysis.cluster.markov]
 - [`hierarchical_markov`][ragraph.analysis.cluster.hierarchical_markov]
-- ['tarjans_scc`][ragraph.analysis.cluster.tarjans_scc]
+- [`tarjans_scc`][ragraph.analysis.cluster.tarjans_scc]
 """
 
 from ragraph.analysis.cluster._markov import (
     MarkovFlow,
     MarkovRelative,
     calculate_tpm,
     create_clusters,
```

### Comparing `ragraph-1.20.3/ragraph/analysis/cluster/_markov.py` & `ragraph-1.21.0/ragraph/analysis/cluster/_markov.py`

 * *Files identical despite different names*

### Comparing `ragraph-1.20.3/ragraph/analysis/cluster/_tarjan.py` & `ragraph-1.21.0/ragraph/analysis/cluster/_tarjan.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 # Tarjan's strongly connected components algorithm.
 
 Reference:
     Tarjan, R. (1972). Depth-First Search and Linear Graph Algorithms.
     SIAM Journal on Computing, 1(2), 146-160.
     [DOI: 10.1137/0201010] (https://doi.org/10.1137/0201010)
 """
+
 from textwrap import dedent
 from typing import Dict, List, Optional, Tuple, Union
 
 from ragraph.analysis._classes import ClusterAnalysis
 from ragraph.analysis._utils import create_parent
 from ragraph.graph import Graph
 from ragraph.node import Node
```

### Comparing `ragraph-1.20.3/ragraph/analysis/comparison/__init__.py` & `ragraph-1.21.0/ragraph/analysis/comparison/__init__.py`

 * *Files identical despite different names*

### Comparing `ragraph-1.20.3/ragraph/analysis/comparison/_delta.py` & `ragraph-1.21.0/ragraph/analysis/comparison/_delta.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,9 @@
 """# Delta analysis"""
 
-
 from typing import Type
 
 from ragraph.analysis.comparison.utils import (
     EdgeDescriptor,
     EdgeDescriptorLike,
     NodeDescriptor,
     NodeDescriptorLike,
```

### Comparing `ragraph-1.20.3/ragraph/analysis/comparison/_sigma.py` & `ragraph-1.21.0/ragraph/analysis/comparison/_sigma.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,22 +1,26 @@
 """# Sigma analysis"""
 
 import enum
 from copy import deepcopy
-from typing import Iterable
+from typing import TYPE_CHECKING, Iterable
 
 from ragraph.edge import Edge
 from ragraph.generic import Metadata
 from ragraph.graph import Graph
 from ragraph.node import Node
 
 try:
     StrEnum = enum.StrEnum
 except Exception:
-    from strenum import StrEnum
+    from strenum import StrEnum  # type: ignore
+finally:
+    if TYPE_CHECKING:
+        StrEnum = enum.StrEnum
+
 
 class SigmaMode(StrEnum):
     """Aggregation mode for sigma analysis, absolute counted occurrences or an average per graph."""
 
     ABSOLUTE = enum.auto()
     AVERAGE = enum.auto()
```

### Comparing `ragraph-1.20.3/ragraph/analysis/comparison/utils.py` & `ragraph-1.21.0/ragraph/analysis/comparison/utils.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,22 +1,26 @@
 """# Comparison analysis utilities"""
+
 import enum
 from abc import ABC, abstractmethod
 from dataclasses import dataclass
-from typing import FrozenSet, Tuple
+from typing import TYPE_CHECKING, FrozenSet, Tuple
 
 from ragraph.edge import Edge
 from ragraph.generic import Metadata
 from ragraph.graph import Graph
 from ragraph.node import Node
 
 try:
     StrEnum = enum.StrEnum
 except Exception:
-    from strenum import StrEnum
+    from strenum import StrEnum  # type: ignore
+finally:
+    if TYPE_CHECKING:
+        StrEnum = enum.StrEnum
 
 
 class NodeDescriptorLike(ABC):
     """A class that takes a node and describes it by returning a fixed (hashable) output.
 
     Hashable means that the description can be used to determine uniqueness by set operations.
     """
```

### Comparing `ragraph-1.20.3/ragraph/analysis/compatibility/__init__.py` & `ragraph-1.21.0/ragraph/analysis/compatibility/__init__.py`

 * *Files identical despite different names*

### Comparing `ragraph-1.20.3/ragraph/analysis/compatibility/bdd.py` & `ragraph-1.21.0/ragraph/analysis/compatibility/bdd.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 """# Binary Decision Diagram compatibility calculation
 
 Binary Decision Diagram (BDD) implementation of the compatibility problem.
 """
+
 from typing import Generator, List, Tuple, Union
 
 import dd.autoref as _bdd
 import numpy as np
 
 
 def _yield_ranges(nums: List[int], start: int = 0) -> Generator[range, None, None]:
```

### Comparing `ragraph-1.20.3/ragraph/analysis/heuristics/__init__.py` & `ragraph-1.21.0/ragraph/analysis/heuristics/__init__.py`

 * *Files identical despite different names*

### Comparing `ragraph-1.20.3/ragraph/analysis/heuristics/_johnson.py` & `ragraph-1.21.0/ragraph/analysis/heuristics/_johnson.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """# Donald B. Johnson's nested circuit finding algorithm"""
+
 from collections import defaultdict
 from typing import Dict, Generator, List, Optional, Set, Union
 
 from ragraph.analysis.cluster._tarjan import tarjans_scc_algorithm
 from ragraph.graph import Graph
 from ragraph.node import Node
```

### Comparing `ragraph-1.20.3/ragraph/analysis/heuristics/_markov_gamma.py` & `ragraph-1.21.0/ragraph/analysis/heuristics/_markov_gamma.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """# Hierarchical Markov Clustering (HMC) with Gamma bus detection."""
+
 from textwrap import dedent
 from typing import List, Optional, Tuple, Union
 
 from ragraph.analysis import _utils
 from ragraph.analysis._classes import ClusterAnalysis, Parameter
 from ragraph.analysis.bus._gamma import gamma_bus_detection, gamma_params
 from ragraph.analysis.cluster._markov import (
```

### Comparing `ragraph-1.20.3/ragraph/analysis/sequence/__init__.py` & `ragraph-1.21.0/ragraph/analysis/sequence/__init__.py`

 * *Files identical despite different names*

### Comparing `ragraph-1.20.3/ragraph/analysis/sequence/_axis.py` & `ragraph-1.21.0/ragraph/analysis/sequence/_axis.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """Sort nodes in a typical axis-ready format."""
+
 from textwrap import dedent
 from typing import Any, Dict, Iterable, List, Optional, Tuple, Union
 
 from ragraph.analysis._classes import Cast, Parameter, SequenceAnalysis
 from ragraph.graph import Graph
 from ragraph.node import Node
```

### Comparing `ragraph-1.20.3/ragraph/analysis/sequence/_genetic.py` & `ragraph-1.21.0/ragraph/analysis/sequence/_genetic.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """Genetic algorithms for sequencing purposes."""
+
 from typing import List, Optional, Tuple, Union
 
 from ratio_genetic_py import (
     ConvergenceKinds,
     CrossoverKinds,
     EvaluatorKinds,
     EvaluatorMatrix,
```

### Comparing `ragraph-1.20.3/ragraph/analysis/sequence/_markov.py` & `ragraph-1.21.0/ragraph/analysis/sequence/_markov.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 """Sorting algorithm based on the node dependency/influence in a Markov chain.
 """
+
 from textwrap import dedent
 from typing import List, Optional, Tuple, Union
 
 import numpy as np
 
 from ragraph.analysis._classes import Bound, Parameter, SequenceAnalysis
 from ragraph.analysis.sequence.metrics import net_markov_flow_adjacency
```

### Comparing `ragraph-1.20.3/ragraph/analysis/sequence/_name.py` & `ragraph-1.21.0/ragraph/analysis/sequence/_name.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """Sequence nodes by name."""
+
 from typing import List, Optional, Tuple, Union
 
 from ragraph.analysis._classes import SequenceAnalysis
 from ragraph.graph import Graph, Node
 
 sort_by_name_analysis = SequenceAnalysis("Sort by name")
```

### Comparing `ragraph-1.20.3/ragraph/analysis/sequence/_scc_tearing.py` & `ragraph-1.21.0/ragraph/analysis/sequence/_scc_tearing.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 """A sequencing algorithm for cyclic graphs that tears cycles based on a metric
 (penalty) function. By default we use the metric that the Markov sequencing algorithm
 uses to sort all nodes straight away.
 """
+
 from textwrap import dedent
 from typing import Any, Callable, Dict, Generator, List, Optional, Tuple, Union
 
 from ragraph.analysis._classes import MethodCast, Parameter, SequenceAnalysis
 from ragraph.analysis.cluster._tarjan import tarjans_scc_algorithm
 from ragraph.analysis.sequence.utils import markov_decision
 from ragraph.graph import Graph
```

### Comparing `ragraph-1.20.3/ragraph/analysis/sequence/_tarjan.py` & `ragraph-1.21.0/ragraph/analysis/sequence/_tarjan.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """Tarjan's Depth First Search Algorithm."""
+
 from typing import Dict, List, Optional, Tuple, Union
 
 from ragraph.analysis._classes import SequenceAnalysis
 from ragraph.graph import Graph
 from ragraph.node import Node
 
 tarjans_dfs_analysis = SequenceAnalysis(
```

### Comparing `ragraph-1.20.3/ragraph/analysis/sequence/metrics.py` & `ragraph-1.21.0/ragraph/analysis/sequence/metrics.py`

 * *Files identical despite different names*

### Comparing `ragraph-1.20.3/ragraph/analysis/sequence/utils.py` & `ragraph-1.21.0/ragraph/analysis/sequence/utils.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """Sequencing utils."""
+
 from typing import Any, Callable, Dict, List, Optional, Tuple, Union
 
 import numpy as np
 
 from ragraph.analysis import logger
 from ragraph.analysis._classes import BranchsortAnalysis
 from ragraph.analysis.sequence.metrics import net_markov_flow_adjacency
```

### Comparing `ragraph-1.20.3/ragraph/analysis/similarity/__init__.py` & `ragraph-1.21.0/ragraph/analysis/similarity/__init__.py`

 * *Files identical despite different names*

### Comparing `ragraph-1.20.3/ragraph/analysis/similarity/_jaccard.py` & `ragraph-1.21.0/ragraph/analysis/similarity/_jaccard.py`

 * *Files identical despite different names*

### Comparing `ragraph-1.20.3/ragraph/analysis/similarity/_similarity.py` & `ragraph-1.21.0/ragraph/analysis/similarity/_similarity.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """# Similarity analysis"""
+
 from typing import Any, Callable, List, Tuple
 
 import numpy as np
 
 from ragraph.analysis import cluster, similarity
 from ragraph.edge import Edge
 from ragraph.graph import Graph
```

### Comparing `ragraph-1.20.3/ragraph/analysis/similarity/utils.py` & `ragraph-1.21.0/ragraph/analysis/similarity/utils.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """#Similarity analysis utilities"""
+
 from typing import Any, Callable, List
 
 
 def on_hasattrs(attrs: List[str]) -> Callable[[Any], List[bool]]:
     """Get an object description function that checks whether an instance possesses certain
     attributes. It does not check the values thereof!
```

### Comparing `ragraph-1.20.3/ragraph/colors/__init__.py` & `ragraph-1.21.0/ragraph/colors/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -10,14 +10,15 @@
 [`get_hue`][ragraph.colors.get_hue] is a great way to get a sequential color palette for any hue
 where the hue value corresponds to anything between red (1.0), green (2.0) or blue (3.0).
 
 In our plots, these colors are *not* interpolated. This opens up an easy way to visualize your
 colors in a discrete fashion, since you merely need to supply a list with less colors (e.g. the
 desired number of discrete steps).
 """
+
 from typing import Any, Dict, List
 
 from ragraph.colors.cubehelix import cubehelix_palette
 
 
 def get_categorical(n_colors: int = 10, **kwargs) -> List[str]:
     """Get a color palette suitable for categorical data.
```

### Comparing `ragraph-1.20.3/ragraph/colors/cubehelix.py` & `ragraph-1.21.0/ragraph/colors/cubehelix.py`

 * *Files identical despite different names*

### Comparing `ragraph-1.20.3/ragraph/colors/utils.py` & `ragraph-1.21.0/ragraph/colors/utils.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """# Color utilities"""
+
 from typing import Tuple
 
 
 def rgb1_to_rgb(r: float, g: float, b: float) -> Tuple[int, int, int]:
     """Convert [0.0-1.0] scaled RGB to [0-255]."""
     return round(r * 255), round(g * 255), round(b * 255)
```

### Comparing `ragraph-1.20.3/ragraph/datasets/__init__.py` & `ragraph-1.21.0/ragraph/datasets/__init__.py`

 * *Files identical despite different names*

### Comparing `ragraph-1.20.3/ragraph/datasets/aircraft_engine/__init__.py` & `ragraph-1.21.0/ragraph/datasets/aircraft_engine/__init__.py`

 * *Files identical despite different names*

### Comparing `ragraph-1.20.3/ragraph/datasets/aircraft_engine/aircraft_engine_edges.csv` & `ragraph-1.21.0/ragraph/datasets/aircraft_engine/aircraft_engine_edges.csv`

 * *Files identical despite different names*

### Comparing `ragraph-1.20.3/ragraph/datasets/aircraft_engine/aircraft_engine_nodes.csv` & `ragraph-1.21.0/ragraph/datasets/aircraft_engine/aircraft_engine_nodes.csv`

 * *Files identical despite different names*

### Comparing `ragraph-1.20.3/ragraph/datasets/architecture_integral/__init__.py` & `ragraph-1.21.0/ragraph/datasets/architecture_integral/__init__.py`

 * *Files identical despite different names*

### Comparing `ragraph-1.20.3/ragraph/datasets/architecture_integral/architecture_integral_edges.csv` & `ragraph-1.21.0/ragraph/datasets/architecture_integral/architecture_integral_edges.csv`

 * *Files identical despite different names*

### Comparing `ragraph-1.20.3/ragraph/datasets/architecture_mix/__init__.py` & `ragraph-1.21.0/ragraph/datasets/architecture_mix/__init__.py`

 * *Files identical despite different names*

### Comparing `ragraph-1.20.3/ragraph/datasets/architecture_mix/architecture_mix_edges.csv` & `ragraph-1.21.0/ragraph/datasets/architecture_mix/architecture_mix_edges.csv`

 * *Files identical despite different names*

### Comparing `ragraph-1.20.3/ragraph/datasets/architecture_modular/__init__.py` & `ragraph-1.21.0/ragraph/datasets/architecture_modular/__init__.py`

 * *Files identical despite different names*

### Comparing `ragraph-1.20.3/ragraph/datasets/architecture_modular/architecture_modular_edges.csv` & `ragraph-1.21.0/ragraph/datasets/architecture_modular/architecture_modular_edges.csv`

 * *Files identical despite different names*

### Comparing `ragraph-1.20.3/ragraph/datasets/climate_control/__init__.py` & `ragraph-1.21.0/ragraph/datasets/climate_control/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -15,15 +15,14 @@
 components.
 
 Reference:
     Pimmler, T. U., & Eppinger, S. D. (1994). Integration Analysis of Product Decompositions. ASME
     Design Theory and Methodology Conference.
 """
 
-
 edge_weights = [
     "adjacency",
     "spatial",
     "energy flow",
     "information flow",
     "material flow",
 ]
```

### Comparing `ragraph-1.20.3/ragraph/datasets/climate_control/climate_control_edges.csv` & `ragraph-1.21.0/ragraph/datasets/climate_control/climate_control_edges.csv`

 * *Files identical despite different names*

### Comparing `ragraph-1.20.3/ragraph/datasets/climate_control/climate_control_nodes.csv` & `ragraph-1.21.0/ragraph/datasets/climate_control/climate_control_nodes.csv`

 * *Files identical despite different names*

### Comparing `ragraph-1.20.3/ragraph/datasets/climate_control_mg/climate_control_mg_edges.csv` & `ragraph-1.21.0/ragraph/datasets/climate_control_mg/climate_control_mg_edges.csv`

 * *Files identical despite different names*

### Comparing `ragraph-1.20.3/ragraph/datasets/climate_control_mg/climate_control_mg_nodes.csv` & `ragraph-1.21.0/ragraph/datasets/climate_control_mg/climate_control_mg_nodes.csv`

 * *Files identical despite different names*

### Comparing `ragraph-1.20.3/ragraph/datasets/compatibility/compatibility_edges.csv` & `ragraph-1.21.0/ragraph/datasets/compatibility/compatibility_edges.csv`

 * *Files identical despite different names*

### Comparing `ragraph-1.20.3/ragraph/datasets/design/design_edges.csv` & `ragraph-1.21.0/ragraph/datasets/design/design_edges.csv`

 * *Files identical despite different names*

### Comparing `ragraph-1.20.3/ragraph/datasets/elevator175/__init__.py` & `ragraph-1.21.0/ragraph/datasets/elevator175/__init__.py`

 * *Files identical despite different names*

### Comparing `ragraph-1.20.3/ragraph/datasets/elevator175/elevator175_edges.csv` & `ragraph-1.21.0/ragraph/datasets/elevator175/elevator175_edges.csv`

 * *Files identical despite different names*

### Comparing `ragraph-1.20.3/ragraph/datasets/elevator175/elevator175_nodes.csv` & `ragraph-1.21.0/ragraph/datasets/elevator175/elevator175_nodes.csv`

 * *Files identical despite different names*

### Comparing `ragraph-1.20.3/ragraph/datasets/elevator45/__init__.py` & `ragraph-1.21.0/ragraph/datasets/elevator45/__init__.py`

 * *Files identical despite different names*

### Comparing `ragraph-1.20.3/ragraph/datasets/elevator45/elevator45_edges.csv` & `ragraph-1.21.0/ragraph/datasets/elevator45/elevator45_edges.csv`

 * *Files identical despite different names*

### Comparing `ragraph-1.20.3/ragraph/datasets/elevator45/elevator45_nodes.csv` & `ragraph-1.21.0/ragraph/datasets/elevator45/elevator45_nodes.csv`

 * *Files identical despite different names*

### Comparing `ragraph-1.20.3/ragraph/datasets/esl/__init__.py` & `ragraph-1.21.0/ragraph/datasets/esl/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """# Elephant Specification Language datasets"""
+
 import importlib
 from pathlib import Path
 from typing import List
 
 HERE = Path(__file__).parent
```

### Comparing `ragraph-1.20.3/ragraph/datasets/esl/pump/pump.esl` & `ragraph-1.21.0/ragraph/datasets/esl/pump/pump.esl`

 * *Files identical despite different names*

### Comparing `ragraph-1.20.3/ragraph/datasets/ford_hood/__init__.py` & `ragraph-1.21.0/ragraph/datasets/ford_hood/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -34,15 +34,14 @@
 
 Reference:
     Yassine, Ali A., Daniel E. Whitney, and Tony P. Zambito. 2001. Assessment of Rework
     Probabilities for Simulating Product Development Processes Using the Design Structure Matrix
     (DSM). ASME Design Engineering Technical Conferences, DTM-21693.
 """
 
-
 node_weights = [
     "EC(i) ($000)",
     "EC(r) ($000)",
     "ED(i) (days)",
     "ED(r) (% of ED (i))",
     "information variability",
 ]
```

### Comparing `ragraph-1.20.3/ragraph/datasets/ford_hood/ford_hood_edges.csv` & `ragraph-1.21.0/ragraph/datasets/ford_hood/ford_hood_edges.csv`

 * *Files identical despite different names*

### Comparing `ragraph-1.20.3/ragraph/datasets/ford_hood/ford_hood_nodes.csv` & `ragraph-1.21.0/ragraph/datasets/ford_hood/ford_hood_nodes.csv`

 * *Files identical despite different names*

### Comparing `ragraph-1.20.3/ragraph/datasets/kodak3d/__init__.py` & `ragraph-1.21.0/ragraph/datasets/kodak3d/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -27,9 +27,8 @@
 
 Reference:
     Alizon, Fabrice, Seung K. Moon, Steven B. Shooter, and Timothy W. Simpson. 2007,
     September 4--7. Three Dimensional Design Structure Matrix-DSM3D. ASME Design Engineering
     Technical Conferences, DETCZ007-34510, Las Vegas, NV, pp. 941-948.
 """
 
-
 edge_weights = ["adjacency"]
```

### Comparing `ragraph-1.20.3/ragraph/datasets/kodak3d/kodak3d_edges.csv` & `ragraph-1.21.0/ragraph/datasets/kodak3d/kodak3d_edges.csv`

 * *Files identical despite different names*

### Comparing `ragraph-1.20.3/ragraph/datasets/kodak3d/kodak3d_nodes.csv` & `ragraph-1.21.0/ragraph/datasets/kodak3d/kodak3d_nodes.csv`

 * *Files identical despite different names*

### Comparing `ragraph-1.20.3/ragraph/datasets/ledsip/ledsip_edges.csv` & `ragraph-1.21.0/ragraph/datasets/ledsip/ledsip_edges.csv`

 * *Files identical despite different names*

### Comparing `ragraph-1.20.3/ragraph/datasets/ledsip/ledsip_nodes.csv` & `ragraph-1.21.0/ragraph/datasets/ledsip/ledsip_nodes.csv`

 * *Files identical despite different names*

### Comparing `ragraph-1.20.3/ragraph/datasets/localbus/localbus_edges.csv` & `ragraph-1.21.0/ragraph/datasets/localbus/localbus_edges.csv`

 * *Files identical despite different names*

### Comparing `ragraph-1.20.3/ragraph/datasets/mww_lock_aspect/mww_lock_aspect_edges.csv` & `ragraph-1.21.0/ragraph/datasets/mww_lock_aspect/mww_lock_aspect_edges.csv`

 * *Files identical despite different names*

### Comparing `ragraph-1.20.3/ragraph/datasets/mww_lock_aspect/mww_lock_aspect_nodes.csv` & `ragraph-1.21.0/ragraph/datasets/mww_lock_aspect/mww_lock_aspect_nodes.csv`

 * *Files identical despite different names*

### Comparing `ragraph-1.20.3/ragraph/datasets/mww_lock_eefde/mww_lock_eefde_edges.csv` & `ragraph-1.21.0/ragraph/datasets/mww_lock_eefde/mww_lock_eefde_edges.csv`

 * *Files identical despite different names*

### Comparing `ragraph-1.20.3/ragraph/datasets/mww_lock_eefde/mww_lock_eefde_nodes.csv` & `ragraph-1.21.0/ragraph/datasets/mww_lock_eefde/mww_lock_eefde_nodes.csv`

 * *Files identical despite different names*

### Comparing `ragraph-1.20.3/ragraph/datasets/mww_lock_hansweert/mww_lock_hansweert_edges.csv` & `ragraph-1.21.0/ragraph/datasets/mww_lock_hansweert/mww_lock_hansweert_edges.csv`

 * *Files identical despite different names*

### Comparing `ragraph-1.20.3/ragraph/datasets/mww_lock_hansweert/mww_lock_hansweert_nodes.csv` & `ragraph-1.21.0/ragraph/datasets/mww_lock_hansweert/mww_lock_hansweert_nodes.csv`

 * *Files identical despite different names*

### Comparing `ragraph-1.20.3/ragraph/datasets/mww_lock_sambeek/mww_lock_sambeek_edges.csv` & `ragraph-1.21.0/ragraph/datasets/mww_lock_sambeek/mww_lock_sambeek_edges.csv`

 * *Files identical despite different names*

### Comparing `ragraph-1.20.3/ragraph/datasets/mww_lock_sambeek/mww_lock_sambeek_nodes.csv` & `ragraph-1.21.0/ragraph/datasets/mww_lock_sambeek/mww_lock_sambeek_nodes.csv`

 * *Files identical despite different names*

### Comparing `ragraph-1.20.3/ragraph/datasets/mww_lock_sluis15/mww_lock_sluis15_edges.csv` & `ragraph-1.21.0/ragraph/datasets/mww_lock_sluis15/mww_lock_sluis15_edges.csv`

 * *Files identical despite different names*

### Comparing `ragraph-1.20.3/ragraph/datasets/mww_lock_sluis15/mww_lock_sluis15_nodes.csv` & `ragraph-1.21.0/ragraph/datasets/mww_lock_sluis15/mww_lock_sluis15_nodes.csv`

 * *Files identical despite different names*

### Comparing `ragraph-1.20.3/ragraph/datasets/mww_lock_volkerak/mww_lock_volkerak_edges.csv` & `ragraph-1.21.0/ragraph/datasets/mww_lock_volkerak/mww_lock_volkerak_edges.csv`

 * *Files identical despite different names*

### Comparing `ragraph-1.20.3/ragraph/datasets/mww_lock_volkerak/mww_lock_volkerak_nodes.csv` & `ragraph-1.21.0/ragraph/datasets/mww_lock_volkerak/mww_lock_volkerak_nodes.csv`

 * *Files identical despite different names*

### Comparing `ragraph-1.20.3/ragraph/datasets/pathfinder/__init__.py` & `ragraph-1.21.0/ragraph/datasets/pathfinder/__init__.py`

 * *Files identical despite different names*

### Comparing `ragraph-1.20.3/ragraph/datasets/pathfinder/pathfinder_edges.csv` & `ragraph-1.21.0/ragraph/datasets/pathfinder/pathfinder_edges.csv`

 * *Files identical despite different names*

### Comparing `ragraph-1.20.3/ragraph/datasets/pathfinder/pathfinder_nodes.csv` & `ragraph-1.21.0/ragraph/datasets/pathfinder/pathfinder_nodes.csv`

 * *Files identical despite different names*

### Comparing `ragraph-1.20.3/ragraph/datasets/similarity/similarity_edges.csv` & `ragraph-1.21.0/ragraph/datasets/similarity/similarity_edges.csv`

 * *Files identical despite different names*

### Comparing `ragraph-1.20.3/ragraph/datasets/tss_electric/__init__.py` & `ragraph-1.21.0/ragraph/datasets/tss_electric/__init__.py`

 * *Files identical despite different names*

### Comparing `ragraph-1.20.3/ragraph/datasets/tss_electric/tss_electric_edges.csv` & `ragraph-1.21.0/ragraph/datasets/tss_electric/tss_electric_edges.csv`

 * *Files identical despite different names*

### Comparing `ragraph-1.20.3/ragraph/datasets/tss_electric/tss_electric_nodes.csv` & `ragraph-1.21.0/ragraph/datasets/tss_electric/tss_electric_nodes.csv`

 * *Files identical despite different names*

### Comparing `ragraph-1.20.3/ragraph/datasets/tss_front/__init__.py` & `ragraph-1.21.0/ragraph/datasets/tss_front/__init__.py`

 * *Files identical despite different names*

### Comparing `ragraph-1.20.3/ragraph/datasets/tss_front/tss_front_edges.csv` & `ragraph-1.21.0/ragraph/datasets/tss_front/tss_front_edges.csv`

 * *Files identical despite different names*

### Comparing `ragraph-1.20.3/ragraph/datasets/tss_front/tss_front_nodes.csv` & `ragraph-1.21.0/ragraph/datasets/tss_front/tss_front_nodes.csv`

 * *Files identical despite different names*

### Comparing `ragraph-1.20.3/ragraph/datasets/tss_hydraulic/__init__.py` & `ragraph-1.21.0/ragraph/datasets/tss_hydraulic/__init__.py`

 * *Files identical despite different names*

### Comparing `ragraph-1.20.3/ragraph/datasets/tss_hydraulic/tss_hydraulic_edges.csv` & `ragraph-1.21.0/ragraph/datasets/tss_hydraulic/tss_hydraulic_edges.csv`

 * *Files identical despite different names*

### Comparing `ragraph-1.20.3/ragraph/datasets/tss_hydraulic/tss_hydraulic_nodes.csv` & `ragraph-1.21.0/ragraph/datasets/tss_hydraulic/tss_hydraulic_nodes.csv`

 * *Files identical despite different names*

### Comparing `ragraph-1.20.3/ragraph/datasets/ucav/__init__.py` & `ragraph-1.21.0/ragraph/datasets/ucav/__init__.py`

 * *Files identical despite different names*

### Comparing `ragraph-1.20.3/ragraph/datasets/ucav/ucav_edges.csv` & `ragraph-1.21.0/ragraph/datasets/ucav/ucav_edges.csv`

 * *Files identical despite different names*

### Comparing `ragraph-1.20.3/ragraph/datasets/ucav/ucav_nodes.csv` & `ragraph-1.21.0/ragraph/datasets/ucav/ucav_nodes.csv`

 * *Files identical despite different names*

### Comparing `ragraph-1.20.3/ragraph/edge.py` & `ragraph-1.21.0/ragraph/edge.py`

 * *Files identical despite different names*

### Comparing `ragraph-1.20.3/ragraph/generic.py` & `ragraph-1.21.0/ragraph/generic.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,19 +1,55 @@
 """Generic purpose classes and methods such as metadata models.
 
 Metadata includes the kinds, labels, weights and annotations that we assign to our data
 objects. Standardizing this enables a more predictable experience.
 """
+
+import enum
 import uuid as _uuid
 from collections import defaultdict
 from copy import deepcopy
-from typing import Any, Callable, Dict, Generator, Iterable, List, Optional, Set, Union
+from typing import (
+    TYPE_CHECKING,
+    Any,
+    Callable,
+    Dict,
+    Generator,
+    Iterable,
+    List,
+    Optional,
+    Set,
+    Union,
+)
 from warnings import warn
 
 
+try:
+    StrEnum = enum.StrEnum
+except Exception:
+    from strenum import StrEnum  # type: ignore
+finally:
+    if TYPE_CHECKING:
+        StrEnum = enum.StrEnum
+
+
+class Convention(StrEnum):
+    """Convention for matrix conversion to follow. Either:
+
+    - Inputs in rows, feedback above diagonal (IR_FAD)
+    - Inputs in columns, feedback below diagonal (IC_FBD)
+    """
+
+    IR_FAD = enum.auto()
+    """Inputs in rows, feedback above diagonal."""
+
+    IC_FBD = enum.auto()
+    """Inputs in columns, feedback below diagonal."""
+
+
 class MappingValidationError(Exception):
     pass
 
 
 def field(fget: Callable):
     """A [`Mapping`][ragraph.generic.Mapping] `field` is a property that utilizes the
     [`Mapping`][ragraph.generic.Mapping]'s data.
```

### Comparing `ragraph-1.20.3/ragraph/graph.py` & `ragraph-1.21.0/ragraph/graph.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,21 +1,34 @@
 """# Graph class module
 
 The [`Graph`][ragraph.graph.Graph] class is the core of this package. It is the internal storage
 format that facilitates all conversions. These class definitions are designed to
 accommodate a wide range of graph formats.
 """
+
 from collections import OrderedDict, defaultdict
 from copy import deepcopy
-from typing import Any, Callable, Dict, Generator, Iterable, List, Optional, Set, Tuple, Union
+from typing import (
+    Any,
+    Callable,
+    Dict,
+    Generator,
+    Iterable,
+    List,
+    Optional,
+    Set,
+    Tuple,
+    Union,
+)
 from uuid import UUID
 
 from ragraph import utils
 from ragraph.edge import Edge
 from ragraph.generic import Annotations, Metadata
+from ragraph.generic import Convention
 from ragraph.node import Node
 
 try:
     import numpy as np
 
 except ImportError:
     np = None  # type: ignore
@@ -638,14 +651,15 @@
 
     def get_adjacency_matrix(
         self,
         nodes: Optional[Union[List[Node], List[str]]] = None,
         inherit: bool = False,
         loops: bool = False,
         only: Optional[List[str]] = None,
+        convention: Convention = Convention.IR_FAD,
     ) -> Union["np.ndarray", List[List[float]]]:
         """Convert graph data into a numerical adjacency matrix.
 
         Arguments:
             nodes: Optional list of nodes for which to get the adjacency matrix.
             inherit: Whether to count weights between children of the given nodes.
             loops: Whether to calculate self-loops from a node to itself.
@@ -654,23 +668,32 @@
 
         Returns:
             Adjacency matrix as a 2D numpy array if numpy is present. Otherwise it will
             return a 2D nested list.
         """
         from ragraph.io.matrix import to_matrix
 
-        return to_matrix(self, rows=nodes, cols=nodes, inherit=inherit, loops=loops, only=only)
+        return to_matrix(
+            self,
+            rows=nodes,
+            cols=nodes,
+            inherit=inherit,
+            loops=loops,
+            only=only,
+            convention=convention,
+        )
 
     def get_mapping_matrix(
         self,
         rows: Optional[Union[List[Node], List[str]]] = None,
         cols: Optional[Union[List[Node], List[str]]] = None,
         inherit: bool = False,
         loops: bool = False,
         only: Optional[List[str]] = None,
+        convention: Convention = Convention.IR_FAD,
     ) -> Union["np.ndarray", List[List[float]]]:
         """Convert graph data into a numerical mapping matrix.
 
         Arguments:
             rows: Nodes representing the matrix rows.
             cols: Nodes representing the matrix columns if different from the rows.
             inherit: Whether to count weights between children of the given nodes.
@@ -680,22 +703,31 @@
 
         Returns:
             Adjacency matrix as a 2D numpy array if numpy is present. Otherwise it will
             return a 2D nested list.
         """
         from ragraph.io.matrix import to_matrix
 
-        return to_matrix(self, rows=rows, cols=cols, inherit=inherit, loops=loops, only=only)
+        return to_matrix(
+            self,
+            rows=rows,
+            cols=cols,
+            inherit=inherit,
+            loops=loops,
+            only=only,
+            convention=convention,
+        )
 
     def get_ascii_art(
         self,
         nodes: Optional[List[Node]] = None,
         edge: str = "X",
         diag: str = "\u25A0",
         show: bool = False,
+        convention: Convention = Convention.IR_FAD,
     ) -> Optional[str]:
         """Get a unicode ASCII art representation of a binary adjacency matrix for a
         given set of nodes.
 
         Arguments:
             nodes: Nodes to include in the art.
             edge: Mark to use when there's an edge between nodes. (X by default)
@@ -720,23 +752,32 @@
         # Grid lines
         topline = pad + "\u250C" + (dim - 1) * (ddd + "\u252C") + ddd + "\u2510"
         sepline = pad + "\u251C" + (dim - 1) * (ddd + "\u253C") + ddd + "\u2524"
         endline = pad + "\u2514" + (dim - 1) * (ddd + "\u2534") + ddd + "\u2518"
 
         lines = [topline]
 
-        for i, tgt in enumerate(nodes):
-            line = (maxlen - namelens[i]) * " " + tgt.name + "\u2525"
-            for j, src in enumerate(nodes):
+        for i, row in enumerate(nodes):
+            line = (maxlen - namelens[i]) * " " + row.name + "\u2525"
+            for j, col in enumerate(nodes):
                 if i == j:
                     mark = diag
-                elif self._directed_edges.get(src.name, dict()).get(tgt.name, False):
-                    mark = edge
                 else:
-                    mark = " "
+                    if convention == Convention.IR_FAD:
+                        src = col
+                        tgt = row
+                    elif convention == Convention.IC_FBD:
+                        src = row
+                        tgt = col
+                    else:
+                        raise ValueError("Unknown matrix convention type.")
+                    if self._directed_edges.get(src.name, dict()).get(tgt.name, False):
+                        mark = edge
+                    else:
+                        mark = " "
                 line += " {} \u2502".format(mark)
 
             lines.append(line)
             lines.append(sepline)
         lines[-1] = endline
         txt = "\n".join(lines)
         if show:
```

### Comparing `ragraph-1.20.3/ragraph/io/archimate/__init__.py` & `ragraph-1.21.0/ragraph/io/archimate/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 """XML format support using The Open Group ArchiMate® Model Exchange File Format.
 
 Reference:
     https://www.opengroup.org/xsd/archimate/
 """
+
 import shutil
 from pathlib import Path
 from typing import Any, Dict, Generator, Optional, Union
 
 from lxml import etree
 from lxml.builder import ElementMaker
```

### Comparing `ragraph-1.20.3/ragraph/io/archimate/archimate3_Model.xsd` & `ragraph-1.21.0/ragraph/io/archimate/archimate3_Model.xsd`

 * *Files identical despite different names*

### Comparing `ragraph-1.20.3/ragraph/io/archimate/xml.xsd` & `ragraph-1.21.0/ragraph/io/archimate/xml.xsd`

 * *Files identical despite different names*

### Comparing `ragraph-1.20.3/ragraph/io/canopy.py` & `ragraph-1.21.0/ragraph/io/canopy.py`

 * *Files 1% similar despite different names*

```diff
@@ -50,15 +50,15 @@
 
     return graphs
 
 
 def to_canopy(
     graph: Graph,
     path: Optional[Union[Path, str]] = None,
-    fmt: str = "session",
+    fmt: str = "graph",
 ) -> Optional[str]:
     """Save graph as a Canopy dataset.
 
     Arguments:
         graph: Graph to save.
         path: Path to write to.
         fmt: One of 'session' or 'graph'.
```

### Comparing `ragraph-1.20.3/ragraph/io/csv.py` & `ragraph-1.21.0/ragraph/io/csv.py`

 * *Files identical despite different names*

### Comparing `ragraph-1.20.3/ragraph/io/esl.py` & `ragraph-1.21.0/ragraph/io/esl.py`

 * *Files identical despite different names*

### Comparing `ragraph-1.20.3/ragraph/io/grip.py` & `ragraph-1.21.0/ragraph/io/grip.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """# GRIP format support"""
+
 from datetime import datetime
 from pathlib import Path
 from typing import Optional, Union
 from uuid import UUID, uuid4
 
 from lxml import etree
 
@@ -61,14 +62,15 @@
     "Onderhoudsproducten": ["ID", "User", "Type_uitwisseling"],
     "Proceseisen": ["ID", "User", "Type_uitwisseling"],
     "Onderhoudsactiviteiten": ["ID", "User", "Type_uitwisseling"],
 }
 
 
 OBJECT_KIND = "object"
+OBJECTTYPE_KIND = "objecttype"
 FUNCTIE_KIND = "functie"
 SYSTEEMEIS_KIND = "systeemeis"
 SCOPE_KIND = "scope"
 RAAKVLAK_KIND = "raakvlak"
 PARAMETER_KIND = "param"
 
 
@@ -91,14 +93,17 @@
         annotations=dict(root.attrib),
     )
     parse_params(graph, root)
 
     parse_collection(graph, root, "Objecten", "Object", OBJECT_KIND)
     parse_objectenboom(graph, root)
 
+    parse_collection(graph, root, "Objecttypen", "Objecttype", OBJECTTYPE_KIND)
+    parse_objecttypenboom(graph, root)
+
     parse_collection(graph, root, "Functies", "Functie", FUNCTIE_KIND)
     parse_collection(graph, root, "Systeemeisen", "Systeemeis", SYSTEEMEIS_KIND)
     parse_collection(graph, root, "Scope", "Scope", SCOPE_KIND)
     parse_collection(graph, root, "Raakvlakken", "Raakvlak", RAAKVLAK_KIND)
 
     parse_systeemeis_edges(graph, root)
     parse_object_edges(graph, root)
@@ -272,14 +277,24 @@
         parent = graph[UUID(el.attrib.get("GUID"))]
         for sub in el.iterfind("SI_Onderliggend"):
             for obj in sub.iterfind("ObjectOnderliggend"):
                 child_id = UUID(obj.attrib.get("GUID"))
                 graph[child_id].parent = parent
 
 
+def parse_objecttypenboom(graph: Graph, root: etree.Element):
+    collection = root.find("Objecttypen")
+    for el in collection.iterfind("Objecttype"):
+        parent = graph[UUID(el.attrib.get("GUID"))]
+        for sub in el.iterfind("SI_Onderliggende"):
+            for obj in sub.iterfind("Objecttype"):
+                child_id = UUID(obj.attrib.get("GUID"))
+                graph[child_id].parent = parent
+
+
 def parse_systeemeis_edges(graph: Graph, root: etree.Element):
     elems = root.find("Systeemeisen").iterfind("Systeemeis")
     for el in elems:
         source = graph[UUID(el.attrib.get("GUID"))]
 
         for me_eis in el.iterfind("CI_MEEisObject"):
             eis_obj = me_eis.find("EisObject")
@@ -307,14 +322,22 @@
             annotations = dict(RootRef=sub.attrib["RootRef"])
             for functie in sub.iterfind("Functie"):
                 functie_id = UUID(functie.attrib.get("GUID"))
                 target = graph[functie_id]
                 graph.add_edge(Edge(source, target, kind=OBJECT_KIND, annotations=annotations))
                 graph.add_edge(Edge(target, source, kind=OBJECT_KIND, annotations=annotations))
 
+        for sub in el.iterfind("SI_Objecttype"):
+            annotations = dict(RootRef=sub.attrib["RootRef"])
+            for objecttype in sub.iterfind("Objecttype"):
+                objecttype_id = UUID(objecttype.attrib.get("GUID"))
+                target = graph[objecttype_id]
+                graph.add_edge(Edge(source, target, kind=OBJECT_KIND, annotations=annotations))
+                graph.add_edge(Edge(target, source, kind=OBJECT_KIND, annotations=annotations))
+
 
 def parse_scope_edges(graph: Graph, root: etree.Element):
     elems = root.find("Scope").iterfind("Scope")
     for el in elems:
         source = graph[UUID(el.attrib.get("GUID"))]
 
         for eis in el.iterfind("SI_Systeemeis"):
```

### Comparing `ragraph-1.20.3/ragraph/io/json.py` & `ragraph-1.21.0/ragraph/io/json.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """# JSON format support"""
+
 import json
 from pathlib import Path
 from typing import Any, Dict, Optional, Union
 from uuid import UUID
 
 from ragraph.edge import Edge
 from ragraph.generic import Annotations
```

### Comparing `ragraph-1.20.3/ragraph/io/matrix.py` & `ragraph-1.21.0/ragraph/io/matrix.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,28 +1,29 @@
 """# Adjacency and mapping matrices support"""
 
 from typing import Any, Dict, List, Optional, Union
 
 from ragraph.edge import Edge
 from ragraph.graph import Graph
 from ragraph.node import Node
+from ragraph.generic import Convention
 
 try:
     import numpy as np
-
 except ImportError:
     np = None
 
 
 def from_matrix(
     matrix: Union["np.ndarray", List[List[int]], List[List[float]]],
     rows: Optional[Union[List[Node], List[str]]] = None,
     cols: Optional[Union[List[Node], List[str]]] = None,
     weight_label: str = "default",
     empty: Optional[Union[int, float]] = 0.0,
+    convention: Convention = Convention.IR_FAD,
     **graph_args: Dict[str, Any],
 ) -> Graph:
     """Create a graph from an adjacency or mapping matrix.
 
     Arguments:
         matrix: Matrix to convert into a graph.
         rows: Nodes or node labels corresponding to the rows of the matrix.
@@ -40,15 +41,15 @@
         If no column labels are provided, they are assumed to be equal to the rows.
         For non-square matrices, you should provide node labels!
     """
 
     rows = [Node(f"node{i}") for i in range(len(matrix))] if rows is None else rows
 
     # init empty graph
-    graph = Graph(**graph_args)
+    graph = Graph(**graph_args)  # type: ignore
 
     # Parse row labels and create new nodes.
     node_rows = _parse_labels(graph, rows)
 
     # Init nodes from provided labels.
     if cols is None:
         node_cols = node_rows
@@ -58,37 +59,54 @@
     # Dimension check of matrix and labels.
     dim = (len(matrix), len(matrix[0]))
     labdim = (len(node_rows), len(node_cols))
     if dim != labdim:
         raise ValueError(f"Matrix dimensions {dim} do not agree with label dimensions {labdim}.")
 
     # Generate edges and return.
-    edges = [
-        Edge(
-            source,
-            target,
-            name=f"{source.name}->{target.name}",
-            weights={weight_label: matrix[row][col]},
-        )
-        for row, target in enumerate(node_rows)
-        for col, source in enumerate(node_cols)
-        if matrix[row][col] != empty
-    ]
+    if convention == Convention.IR_FAD:
+        edges = [
+            Edge(
+                source,
+                target,
+                name=f"{source.name}->{target.name}",
+                weights={weight_label: matrix[row][col]},
+            )
+            for row, target in enumerate(node_rows)
+            for col, source in enumerate(node_cols)
+            if matrix[row][col] != empty
+        ]
+    elif convention == Convention.IC_FBD:
+        edges = [
+            Edge(
+                source,
+                target,
+                name=f"{source.name}->{target.name}",
+                weights={weight_label: matrix[row][col]},
+            )
+            for row, source in enumerate(node_rows)
+            for col, target in enumerate(node_cols)
+            if matrix[row][col] != empty
+        ]
+    else:
+        raise ValueError("Unknown convention for matrix conversion.")
+
     graph.edges = edges
     return graph
 
 
 def to_matrix(
     graph: Graph,
     rows: Optional[Union[List[Node], List[str]]] = None,
     cols: Optional[Union[List[Node], List[str]]] = None,
     inherit: bool = False,
     loops: bool = False,
     only: Optional[List[str]] = None,
-) -> Union[np.ndarray, List[List[float]]]:
+    convention: Convention = Convention.IR_FAD,
+) -> Union["np.ndarray", List[List[float]]]:
     """Convert graph data into a directed numerical adjacency or mapping matrix.
 
     Arguments:
         graph: Graph to fetch data from.
         rows: Nodes representing the matrix rows.
         cols: Nodes representing the matrix columns if different from the rows.
         inherit: Whether to count weights between children of the given nodes.
@@ -115,21 +133,31 @@
 
     dim = (len(rows), len(cols))
     if np:
         matrix = np.zeros(dim, dtype=float)
     else:
         matrix = [[0.0 for j in range(dim[1])] for i in range(dim[0])]
 
-    for col, source in enumerate(cols):
-        for row, target in enumerate(rows):
-            if source == target and not loops:
+    for col, col_node in enumerate(cols):
+        for row, row_node in enumerate(rows):
+            if col_node == row_node and not loops:
                 continue
 
+            if convention == Convention.IR_FAD:
+                source = col_node
+                target = row_node
+            elif convention == Convention.IC_FBD:
+                source = row_node
+                target = col_node
+            else:
+                raise ValueError("Unknown convention for matrix conversion.")
+
             sources = [source]
             targets = [target]
+
             if inherit:
                 sources.extend(source.descendants)
                 targets.extend(target.descendants)
 
             weight = sum(
                 [_get_weight(e, only=only) for e in graph.edges_between_all(sources, targets)]
             )
```

### Comparing `ragraph-1.20.3/ragraph/io/xml/XMI-Canonical.xsd` & `ragraph-1.21.0/ragraph/io/xml/XMI-Canonical.xsd`

 * *Files identical despite different names*

### Comparing `ragraph-1.20.3/ragraph/io/xml/__init__.py` & `ragraph-1.21.0/ragraph/io/xml/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """XML format support using the XML Metadata Interchange (XMI) standard."""
+
 import shutil
 import uuid as _uuid
 from pathlib import Path
 from typing import Any, Callable, Dict, Iterable, List, Optional, Union
 
 from lxml import etree
```

### Comparing `ragraph-1.20.3/ragraph/io/xml/ragraph.xsd` & `ragraph-1.21.0/ragraph/io/xml/ragraph.xsd`

 * *Files identical despite different names*

### Comparing `ragraph-1.20.3/ragraph/io/yaml.py` & `ragraph-1.21.0/ragraph/io/yaml.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """# YAML format support"""
+
 from pathlib import Path
 from typing import Optional, Union
 
 from ragraph.graph import Graph
 from ragraph.io.json import graph_from_json_dict
 
 try:
```

### Comparing `ragraph-1.20.3/ragraph/node.py` & `ragraph-1.21.0/ragraph/node.py`

 * *Files identical despite different names*

### Comparing `ragraph-1.20.3/ragraph/plot/__init__.py` & `ragraph-1.21.0/ragraph/plot/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """# RaGraph plotting module"""
+
 from typing import Any, Dict, Iterable, List, Optional
 
 from plotly import graph_objects as go
 
 from ragraph.edge import Edge
 from ragraph.graph import Graph
 from ragraph.node import Node
```

### Comparing `ragraph-1.20.3/ragraph/plot/components/__init__.py` & `ragraph-1.21.0/ragraph/plot/components/__init__.py`

 * *Files identical despite different names*

### Comparing `ragraph-1.20.3/ragraph/plot/components/blank.py` & `ragraph-1.21.0/ragraph/plot/components/blank.py`

 * *Files identical despite different names*

### Comparing `ragraph-1.20.3/ragraph/plot/components/labels.py` & `ragraph-1.21.0/ragraph/plot/components/labels.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """# Labels list plot component"""
+
 from copy import deepcopy
 from typing import List
 
 from ragraph.node import Node
 from ragraph.plot.generic import Component, Style
```

### Comparing `ragraph-1.20.3/ragraph/plot/components/legend.py` & `ragraph-1.21.0/ragraph/plot/components/legend.py`

 * *Files identical despite different names*

### Comparing `ragraph-1.20.3/ragraph/plot/components/piemap.py` & `ragraph-1.21.0/ragraph/plot/components/piemap.py`

 * *Files 5% similar despite different names*

```diff
@@ -10,23 +10,25 @@
 well as other metrics. The node hierarchy is included using squares drawn around the
 diagonal.
 
 Furthermore, bus nodes have their respective row and column in a shaded background
 color. This sets apart the buses' "highly integrative" edges from the regular edges
 between nodes.
 """
+
 from collections import OrderedDict, defaultdict
 from copy import deepcopy
 from math import cos, pi, prod, sin
 from typing import Any, Dict, List, Tuple
 
 import plotly.graph_objs as go
 
 from ragraph import colors
 from ragraph.edge import Edge
+from ragraph.generic import Convention
 from ragraph.node import Node
 from ragraph.plot import svg
 from ragraph.plot.generic import Component, Style
 
 
 class PieMap(Component):
     """A map of piecharts plot component.
@@ -229,16 +231,30 @@
 
     # Get fields dict.
     fields_dict, field_lower, field_upper = _get_fields_dict(bundle_dict, fields, style)
 
     # Calculate actual traces and shapes.
     traces = []
     shapes = []
-    for i, source in enumerate(cols):
-        for j, target in enumerate(rows):
+    for i, col in enumerate(cols):
+        if style.convention == Convention.IR_FAD:
+            source = col
+        elif style.convention == Convention.IC_FBD:
+            target = col
+        else:
+            raise ValueError("Unknown matrix convention.")
+
+        for j, row in enumerate(rows):
+            if style.convention == Convention.IR_FAD:
+                target = row
+            elif style.convention == Convention.IC_FBD:
+                source = row
+            else:
+                raise ValueError("Unknown matrix convention.")
+
             bundle = bundle_dict[source.name, target.name]
             if not bundle:
                 continue  # No edges here.
             field_values = fields_dict[source.name, target.name]
 
             # Equal angles if calculated else calculate relative ones.
             field_angles = (
@@ -285,16 +301,30 @@
 
     # Without inheritance, this edge dict is just the result we want.
     if not style.piemap.inherit:
         return edge_dict
 
     # Calculate edge bundles:
     bundle_dict: Dict[Tuple[str, str], List[Edge]] = defaultdict(list)
-    for i, source in enumerate(cols):
-        for j, target in enumerate(rows):
+    for col in cols:
+        if style.convention == Convention.IR_FAD:
+            source = col
+        elif style.convention == Convention.IC_FBD:
+            target = col
+        else:
+            raise ValueError("Unknown matrix convention.")
+
+        for row in rows:
+            if style.convention == Convention.IR_FAD:
+                target = row
+            elif style.convention == Convention.IC_FBD:
+                source = row
+            else:
+                raise ValueError("Unknown matrix convention.")
+
             bundle = edge_dict[source.name, target.name]
             bundle.extend(
                 e
                 for s in source.descendant_gen
                 for t in target.descendant_gen
                 for e in edge_dict[s.name, t.name]
             )
```

### Comparing `ragraph-1.20.3/ragraph/plot/components/tree.py` & `ragraph-1.21.0/ragraph/plot/components/tree.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 """# Hierarchy tree plot component
 
 This module contains the [`Tree` component][ragraph.plot.components.tree.Tree] which produces a
 [`Component`][ragraph.plot.generic.Component] for the hierarchy tree of a vertical list of leaf
 nodes up to their roots which are put on their left.
 """
+
 from collections import OrderedDict
 from copy import deepcopy
 from typing import Any, Dict, List, Set, Tuple, Union
 
 import plotly.graph_objs as go
 
 from ragraph.node import Node
```

### Comparing `ragraph-1.20.3/ragraph/plot/generic.py` & `ragraph-1.21.0/ragraph/plot/generic.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,17 @@
 """# RaGraph generic plotting classes"""
+
 from copy import deepcopy
 from typing import Any, Callable, Dict, List, Optional, Tuple, Union
 
 from plotly import graph_objs as go
 from plotly.basedatatypes import BaseTraceType
 
 from ragraph import colors
-from ragraph.generic import Mapping, field
+from ragraph.generic import Convention, Mapping, field
 from ragraph.plot import svg
 
 MODEBAR_BUTTONS = {
     "toImage",
     "sendDataToCloud",
     "editInChartStudio",
     "zoom2d",
@@ -649,16 +650,15 @@
 
     @field
     def fontaspectratio(self) -> float:  # type: ignore
         """Font width per fontsize ratio."""
 
     @field
     def height(self) -> int:  # type: ignore
-        """Height of the swatch plot in number of box sizes when plotting a
-        numerical legend."""
+        """Height of the swatch plot in number of box sizes when plotting a numerical legend."""
 
     @field
     def n_ticks(self) -> int:  # type: ignore
         """Number of ticks in the swatch plot when plotting a numerical legend."""
 
     @field
     def xaxis(self) -> go.layout.XAxis:  # type: ignore
@@ -669,14 +669,15 @@
         """Plotly Y-axis settings."""
 
 
 class Style(Mapping):
     """RaGraph plot style mapping.
 
     Arguments:
+        convention: Convention to use when drawing edges.
         boxsize: Size in pixels per row or column.
         config: Plotly Figure.show() config.
         highlight_annotation: Annotation key of instances that should be highlighted.
             Value should be True-ish. Set key to `None` to disable.
         highlight_color: Default color to use for highlights.
         labels: Labels plot style.
         layout: Layout options.
@@ -687,14 +688,15 @@
         show_legend: Bool to display legend.
         row_col_numbers: Bool to display row and column numbers.
         xstep: Axis increment per row or column in plots (usually 1).
         ystep: Axis increment per row or column in plots (usually 1).
     """
 
     _defaults = dict(
+        convention=Convention.IR_FAD,
         boxsize=20,
         config=dict(
             displaylogo=False,
             modeBarButtonsToRemove=list(
                 MODEBAR_BUTTONS - {"resetScale2d", "toImage", "toggleSpikelines"}
             ),
             responsive=False,
@@ -719,14 +721,15 @@
         row_col_numbers=True,
         xstep=1,
         ystep=1,
     )
 
     def __init__(
         self,
+        convention: Optional[Convention] = None,
         boxsize: Optional[int] = None,
         config: Optional[Dict[str, Any]] = None,
         highlight_annotation: Optional[str] = None,
         highlight_color: Optional[str] = None,
         labels: Optional[Union[LabelsStyle, Dict[str, Any]]] = None,
         layout: Optional[Union[go.Layout, Dict[str, Any]]] = None,
         palettes: Optional[Palettes] = None,
@@ -735,14 +738,15 @@
         legend: Optional[Union[LegendStyle, Dict[str, Any]]] = None,
         show_legend: Optional[bool] = None,
         row_col_numbers: Optional[bool] = None,
         xstep: Optional[str] = None,
         ystep: Optional[str] = None,
     ):
         super().__init__(
+            convention=convention,
             boxsize=boxsize,
             config=config,
             highlight_annotation=highlight_annotation,
             highlight_color=highlight_color,
             labels=labels,
             layout=layout,
             palettes=palettes,
@@ -752,14 +756,18 @@
             show_legend=show_legend,
             row_col_numbers=row_col_numbers,
             xstep=xstep,
             ystep=ystep,
         )
 
     @field
+    def convention(self) -> Convention:  # type: ignore
+        """Convention to use when drawing edges."""
+
+    @field
     def boxsize(self) -> int:  # type: ignore
         """Size in pixels per row or column."""
 
     @field
     def config(self) -> Dict[str, Any]:  # type: ignore
         """Plotly Figure.show() config."""
```

### Comparing `ragraph-1.20.3/ragraph/plot/svg.py` & `ragraph-1.21.0/ragraph/plot/svg.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 """# SVG shapes
 
 This module contains two base classes, being the [`Line`][ragraph.plot.svg.Line] options for SVG
 shapes and an [`SVG`][ragraph.plot.svg.SVG] mapping for the shapes themselves. You will also find
 several methods to obtain several basic shapes conveniently.
 """
+
 from math import cos, pi, sin
 from typing import Any, Dict, Optional, Union
 
 from ragraph.generic import Mapping, field
 
 
 class Line(Mapping):
```

### Comparing `ragraph-1.20.3/ragraph/plot/utils.py` & `ragraph-1.21.0/ragraph/plot/utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """RaGraph plot utilities."""
+
 from typing import Dict, Iterable, List, Optional, Union
 
 from plotly import graph_objects as go
 from plotly.subplots import make_subplots
 
 from ragraph.analysis.sequence._axis import get_axis_sequence  # noqa
 from ragraph.edge import Edge
@@ -26,53 +27,61 @@
     """
     rows = len(components)
 
     components_t = list(zip(*components))  # Transpose helper matrix.
     cols = len(components_t)
 
     min_x_ranges = [
-        min(
-            [comp.xaxis.range[0] for comp in col if comp and comp.xaxis.range],
-            default=0,
+        (
+            min(
+                [comp.xaxis.range[0] for comp in col if comp and comp.xaxis.range],
+                default=0,
+            )
+            if any(col)
+            else 0
         )
-        if any(col)
-        else 0
         for col in components_t
         if components_t
     ]
 
     max_x_ranges = [
-        max(
-            [comp.xaxis.range[1] for comp in col if comp and comp.xaxis.range],
-            default=1,
+        (
+            max(
+                [comp.xaxis.range[1] for comp in col if comp and comp.xaxis.range],
+                default=1,
+            )
+            if any(col)
+            else 1
         )
-        if any(col)
-        else 1
         for col in components_t
     ]
 
     widths = [(x_max - x_min) * style.boxsize for (x_max, x_min) in zip(max_x_ranges, min_x_ranges)]
 
     min_y_ranges = [
-        min(
-            [comp.yaxis.range[0] for comp in row if comp and comp.yaxis.range],
-            default=0,
+        (
+            min(
+                [comp.yaxis.range[0] for comp in row if comp and comp.yaxis.range],
+                default=0,
+            )
+            if any(row)
+            else 0
         )
-        if any(row)
-        else 0
         for row in components
     ]
 
     max_y_ranges = [
-        max(
-            [comp.yaxis.range[1] for comp in row if comp and comp.yaxis.range],
-            default=1,
+        (
+            max(
+                [comp.yaxis.range[1] for comp in row if comp and comp.yaxis.range],
+                default=1,
+            )
+            if any(row)
+            else 1
         )
-        if any(row)
-        else 1
         for row in components
     ]
 
     heights = [
         (y_max - y_min) * style.boxsize for (y_max, y_min) in zip(max_y_ranges, min_y_ranges)
     ]
```

### Comparing `ragraph-1.20.3/ragraph/utils.py` & `ragraph-1.21.0/ragraph/utils.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """# Graph handling utilities"""
+
 from typing import TYPE_CHECKING, Generator, List, Set
 
 if TYPE_CHECKING:
     from ragraph.graph import Graph
     from ragraph.node import Node
```

### Comparing `ragraph-1.20.3/PKG-INFO` & `ragraph-1.21.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ragraph
-Version: 1.20.3
+Version: 1.21.0
 Summary: Ratio graph handling in Python.
 Home-page: https://ragraph.ratio-case.nl
 License: GPL-3.0-or-later
 Author: Ratio Innovations B.V.
 Author-email: info@ratio-case.nl
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
```

