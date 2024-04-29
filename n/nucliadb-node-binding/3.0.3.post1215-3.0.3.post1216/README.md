# Comparing `tmp/nucliadb_node_binding-3.0.3.post1215.tar.gz` & `tmp/nucliadb_node_binding-3.0.3.post1216.tar.gz`

## Comparing `nucliadb_node_binding-3.0.3.post1215.tar` & `nucliadb_node_binding-3.0.3.post1216.tar`

### file list

```diff
@@ -1,283 +1,283 @@
--rw-r--r--   0        0        0      399 1970-01-01 00:00:00.000000 nucliadb_node_binding-3.0.3.post1215/local_dependencies/nucliadb_texts2/Cargo.toml
--rw-r--r--   0     1001      127      931 2024-04-29 09:36:44.000000 nucliadb_node_binding-3.0.3.post1215/local_dependencies/nucliadb_texts2/src/lib.rs
--rw-r--r--   0     1001      127     2755 2024-04-29 09:36:44.000000 nucliadb_node_binding-3.0.3.post1215/local_dependencies/nucliadb_texts2/src/query_io.rs
--rw-r--r--   0     1001      127    22721 2024-04-29 09:36:44.000000 nucliadb_node_binding-3.0.3.post1215/local_dependencies/nucliadb_texts2/src/reader.rs
--rw-r--r--   0     1001      127     3105 2024-04-29 09:36:44.000000 nucliadb_node_binding-3.0.3.post1215/local_dependencies/nucliadb_texts2/src/schema.rs
--rw-r--r--   0     1001      127     8682 2024-04-29 09:36:44.000000 nucliadb_node_binding-3.0.3.post1215/local_dependencies/nucliadb_texts2/src/search_query.rs
--rw-r--r--   0     1001      127    10109 2024-04-29 09:36:44.000000 nucliadb_node_binding-3.0.3.post1215/local_dependencies/nucliadb_texts2/src/writer.rs
--rw-r--r--   0     1001      127     3396 2024-04-29 09:36:44.000000 nucliadb_node_binding-3.0.3.post1215/local_dependencies/nucliadb_texts2/tests/common/mod.rs
--rw-r--r--   0     1001      127     2068 2024-04-29 09:36:44.000000 nucliadb_node_binding-3.0.3.post1215/local_dependencies/nucliadb_texts2/tests/test_reader.rs
--rw-r--r--   0     1001      127     9567 2024-04-29 09:36:44.000000 nucliadb_node_binding-3.0.3.post1215/local_dependencies/nucliadb_texts2/tests/test_search.rs
--rw-r--r--   0     1001      127     1249 2024-04-29 09:36:44.000000 nucliadb_node_binding-3.0.3.post1215/local_dependencies/nucliadb_texts2/tests/test_streaming.rs
--rw-r--r--   0     1001      127     3469 2024-04-29 09:36:44.000000 nucliadb_node_binding-3.0.3.post1215/local_dependencies/nucliadb_texts2/tests/test_writer.rs
--rw-r--r--   0        0        0      629 1970-01-01 00:00:00.000000 nucliadb_node_binding-3.0.3.post1215/local_dependencies/nucliadb_paragraphs3/Cargo.toml
--rw-r--r--   0     1001      127     7796 2024-04-29 09:36:44.000000 nucliadb_node_binding-3.0.3.post1215/local_dependencies/nucliadb_paragraphs3/src/fuzzy_query.rs
--rw-r--r--   0     1001      127     1024 2024-04-29 09:36:44.000000 nucliadb_node_binding-3.0.3.post1215/local_dependencies/nucliadb_paragraphs3/src/lib.rs
--rw-r--r--   0     1001      127     2780 2024-04-29 09:36:44.000000 nucliadb_node_binding-3.0.3.post1215/local_dependencies/nucliadb_paragraphs3/src/query_io.rs
--rw-r--r--   0     1001      127    42885 2024-04-29 09:36:44.000000 nucliadb_node_binding-3.0.3.post1215/local_dependencies/nucliadb_paragraphs3/src/reader.rs
--rw-r--r--   0     1001      127     4407 2024-04-29 09:36:44.000000 nucliadb_node_binding-3.0.3.post1215/local_dependencies/nucliadb_paragraphs3/src/schema.rs
--rw-r--r--   0     1001      127    21349 2024-04-29 09:36:44.000000 nucliadb_node_binding-3.0.3.post1215/local_dependencies/nucliadb_paragraphs3/src/search_query.rs
--rw-r--r--   0     1001      127    11723 2024-04-29 09:36:44.000000 nucliadb_node_binding-3.0.3.post1215/local_dependencies/nucliadb_paragraphs3/src/search_response.rs
--rw-r--r--   0     1001      127     2846 2024-04-29 09:36:44.000000 nucliadb_node_binding-3.0.3.post1215/local_dependencies/nucliadb_paragraphs3/src/set_query.rs
--rw-r--r--   0     1001      127     4090 2024-04-29 09:36:44.000000 nucliadb_node_binding-3.0.3.post1215/local_dependencies/nucliadb_paragraphs3/src/stop_words.rs
--rw-r--r--   0     1001      127    17057 2024-04-29 09:36:44.000000 nucliadb_node_binding-3.0.3.post1215/local_dependencies/nucliadb_paragraphs3/src/writer.rs
--rw-r--r--   0     1001      127       88 2024-04-29 09:36:44.000000 nucliadb_node_binding-3.0.3.post1215/local_dependencies/nucliadb_paragraphs3/stop_words/README.md
--rw-r--r--   0     1001      127    19791 2024-04-29 09:36:44.000000 nucliadb_node_binding-3.0.3.post1215/local_dependencies/nucliadb_paragraphs3/stop_words/ar.json
--rw-r--r--   0     1001      127     1923 2024-04-29 09:36:44.000000 nucliadb_node_binding-3.0.3.post1215/local_dependencies/nucliadb_paragraphs3/stop_words/az.json
--rw-r--r--   0     1001      127    11684 2024-04-29 09:36:44.000000 nucliadb_node_binding-3.0.3.post1215/local_dependencies/nucliadb_paragraphs3/stop_words/bn.json
--rw-r--r--   0     1001      127     2513 2024-04-29 09:36:44.000000 nucliadb_node_binding-3.0.3.post1215/local_dependencies/nucliadb_paragraphs3/stop_words/ca.json
--rw-r--r--   0     1001      127    12802 2024-04-29 09:36:44.000000 nucliadb_node_binding-3.0.3.post1215/local_dependencies/nucliadb_paragraphs3/stop_words/ch.json
--rw-r--r--   0     1001      127      730 2024-04-29 09:36:44.000000 nucliadb_node_binding-3.0.3.post1215/local_dependencies/nucliadb_paragraphs3/stop_words/da.json
--rw-r--r--   0     1001      127     2090 2024-04-29 09:36:44.000000 nucliadb_node_binding-3.0.3.post1215/local_dependencies/nucliadb_paragraphs3/stop_words/de.json
--rw-r--r--   0     1001      127     6284 2024-04-29 09:36:44.000000 nucliadb_node_binding-3.0.3.post1215/local_dependencies/nucliadb_paragraphs3/stop_words/el.json
--rw-r--r--   0     1001      127     1473 2024-04-29 09:36:44.000000 nucliadb_node_binding-3.0.3.post1215/local_dependencies/nucliadb_paragraphs3/stop_words/en.json
--rw-r--r--   0     1001      127     3451 2024-04-29 09:36:44.000000 nucliadb_node_binding-3.0.3.post1215/local_dependencies/nucliadb_paragraphs3/stop_words/es.json
--rw-r--r--   0     1001      127     3182 2024-04-29 09:36:44.000000 nucliadb_node_binding-3.0.3.post1215/local_dependencies/nucliadb_paragraphs3/stop_words/eu.json
--rw-r--r--   0     1001      127     2126 2024-04-29 09:36:44.000000 nucliadb_node_binding-3.0.3.post1215/local_dependencies/nucliadb_paragraphs3/stop_words/extract.py
--rw-r--r--   0     1001      127     2748 2024-04-29 09:36:44.000000 nucliadb_node_binding-3.0.3.post1215/local_dependencies/nucliadb_paragraphs3/stop_words/fi.json
--rw-r--r--   0     1001      127     1388 2024-04-29 09:36:44.000000 nucliadb_node_binding-3.0.3.post1215/local_dependencies/nucliadb_paragraphs3/stop_words/fr.json
--rw-r--r--   0     1001      127     5716 2024-04-29 09:36:44.000000 nucliadb_node_binding-3.0.3.post1215/local_dependencies/nucliadb_paragraphs3/stop_words/he.json
--rw-r--r--   0     1001      127     2108 2024-04-29 09:36:44.000000 nucliadb_node_binding-3.0.3.post1215/local_dependencies/nucliadb_paragraphs3/stop_words/hu.json
--rw-r--r--   0     1001      127     8721 2024-04-29 09:36:44.000000 nucliadb_node_binding-3.0.3.post1215/local_dependencies/nucliadb_paragraphs3/stop_words/id.json
--rw-r--r--   0     1001      127     2535 2024-04-29 09:36:44.000000 nucliadb_node_binding-3.0.3.post1215/local_dependencies/nucliadb_paragraphs3/stop_words/it.json
--rw-r--r--   0     1001      127    11737 2024-04-29 09:36:44.000000 nucliadb_node_binding-3.0.3.post1215/local_dependencies/nucliadb_paragraphs3/stop_words/kk.json
--rw-r--r--   0     1001      127     7730 2024-04-29 09:36:44.000000 nucliadb_node_binding-3.0.3.post1215/local_dependencies/nucliadb_paragraphs3/stop_words/ne.json
--rw-r--r--   0     1001      127      756 2024-04-29 09:36:44.000000 nucliadb_node_binding-3.0.3.post1215/local_dependencies/nucliadb_paragraphs3/stop_words/nl.json
--rw-r--r--   0     1001      127     1447 2024-04-29 09:36:44.000000 nucliadb_node_binding-3.0.3.post1215/local_dependencies/nucliadb_paragraphs3/stop_words/no.json
--rw-r--r--   0     1001      127     2055 2024-04-29 09:36:44.000000 nucliadb_node_binding-3.0.3.post1215/local_dependencies/nucliadb_paragraphs3/stop_words/pt.json
--rw-r--r--   0     1001      127     3327 2024-04-29 09:36:44.000000 nucliadb_node_binding-3.0.3.post1215/local_dependencies/nucliadb_paragraphs3/stop_words/ro.json
--rw-r--r--   0     1001      127     3856 2024-04-29 09:36:44.000000 nucliadb_node_binding-3.0.3.post1215/local_dependencies/nucliadb_paragraphs3/stop_words/ru.json
--rw-r--r--   0     1001      127    23032 2024-04-29 09:36:44.000000 nucliadb_node_binding-3.0.3.post1215/local_dependencies/nucliadb_paragraphs3/stop_words/sl.json
--rw-r--r--   0     1001      127      993 2024-04-29 09:36:44.000000 nucliadb_node_binding-3.0.3.post1215/local_dependencies/nucliadb_paragraphs3/stop_words/sv.json
--rw-r--r--   0     1001      127     5424 2024-04-29 09:36:44.000000 nucliadb_node_binding-3.0.3.post1215/local_dependencies/nucliadb_paragraphs3/stop_words/tg.json
--rw-r--r--   0     1001      127      491 2024-04-29 09:36:44.000000 nucliadb_node_binding-3.0.3.post1215/local_dependencies/nucliadb_paragraphs3/stop_words/tr.json
--rw-r--r--   0        0        0      742 1970-01-01 00:00:00.000000 nucliadb_node_binding-3.0.3.post1215/local_dependencies/nucliadb_vectors/Cargo.toml
--rw-r--r--   0     1001      127       69 2024-04-29 09:36:44.000000 nucliadb_node_binding-3.0.3.post1215/local_dependencies/nucliadb_vectors/README.md
--rw-r--r--   0     1001      127       43 2024-04-29 09:36:44.000000 nucliadb_node_binding-3.0.3.post1215/local_dependencies/nucliadb_vectors/docs/README.md
--rw-r--r--   0     1001      127    25718 2024-04-29 09:36:44.000000 nucliadb_node_binding-3.0.3.post1215/local_dependencies/nucliadb_vectors/docs/labels.drawio.svg
--rw-r--r--   0     1001      127    12340 2024-04-29 09:36:44.000000 nucliadb_node_binding-3.0.3.post1215/local_dependencies/nucliadb_vectors/src/data_point/disk_hnsw.rs
--rw-r--r--   0     1001      127    24470 2024-04-29 09:36:44.000000 nucliadb_node_binding-3.0.3.post1215/local_dependencies/nucliadb_vectors/src/data_point/mod.rs
--rw-r--r--   0     1001      127    11214 2024-04-29 09:36:44.000000 nucliadb_node_binding-3.0.3.post1215/local_dependencies/nucliadb_vectors/src/data_point/node.rs
--rw-r--r--   0     1001      127    14639 2024-04-29 09:36:44.000000 nucliadb_node_binding-3.0.3.post1215/local_dependencies/nucliadb_vectors/src/data_point/ops_hnsw.rs
--rw-r--r--   0     1001      127     1642 2024-04-29 09:36:44.000000 nucliadb_node_binding-3.0.3.post1215/local_dependencies/nucliadb_vectors/src/data_point/params.rs
--rw-r--r--   0     1001      127     3952 2024-04-29 09:36:44.000000 nucliadb_node_binding-3.0.3.post1215/local_dependencies/nucliadb_vectors/src/data_point/ram_hnsw.rs
--rw-r--r--   0     1001      127    14175 2024-04-29 09:36:44.000000 nucliadb_node_binding-3.0.3.post1215/local_dependencies/nucliadb_vectors/src/data_point/tests.rs
--rw-r--r--   0     1001      127     5798 2024-04-29 09:36:44.000000 nucliadb_node_binding-3.0.3.post1215/local_dependencies/nucliadb_vectors/src/data_point_provider/garbage_collector.rs
--rw-r--r--   0     1001      127     2777 2024-04-29 09:36:44.000000 nucliadb_node_binding-3.0.3.post1215/local_dependencies/nucliadb_vectors/src/data_point_provider/mod.rs
--rw-r--r--   0     1001      127    10613 2024-04-29 09:36:44.000000 nucliadb_node_binding-3.0.3.post1215/local_dependencies/nucliadb_vectors/src/data_point_provider/reader.rs
--rw-r--r--   0     1001      127     2304 2024-04-29 09:36:44.000000 nucliadb_node_binding-3.0.3.post1215/local_dependencies/nucliadb_vectors/src/data_point_provider/replication.rs
--rw-r--r--   0     1001      127     5288 2024-04-29 09:36:44.000000 nucliadb_node_binding-3.0.3.post1215/local_dependencies/nucliadb_vectors/src/data_point_provider/state.rs
--rw-r--r--   0     1001      127    20587 2024-04-29 09:36:44.000000 nucliadb_node_binding-3.0.3.post1215/local_dependencies/nucliadb_vectors/src/data_point_provider/writer.rs
--rw-r--r--   0     1001      127    23710 2024-04-29 09:36:44.000000 nucliadb_node_binding-3.0.3.post1215/local_dependencies/nucliadb_vectors/src/data_types/data_store.rs
--rw-r--r--   0     1001      127     6916 2024-04-29 09:36:44.000000 nucliadb_node_binding-3.0.3.post1215/local_dependencies/nucliadb_vectors/src/data_types/dtrie_ram.rs
--rw-r--r--   0     1001      127     1959 2024-04-29 09:36:44.000000 nucliadb_node_binding-3.0.3.post1215/local_dependencies/nucliadb_vectors/src/data_types/mod.rs
--rw-r--r--   0     1001      127     6143 2024-04-29 09:36:44.000000 nucliadb_node_binding-3.0.3.post1215/local_dependencies/nucliadb_vectors/src/data_types/trie.rs
--rw-r--r--   0     1001      127     2904 2024-04-29 09:36:44.000000 nucliadb_node_binding-3.0.3.post1215/local_dependencies/nucliadb_vectors/src/data_types/trie_ram.rs
--rw-r--r--   0     1001      127     4433 2024-04-29 09:36:44.000000 nucliadb_node_binding-3.0.3.post1215/local_dependencies/nucliadb_vectors/src/data_types/vector.rs
--rw-r--r--   0     1001      127    10472 2024-04-29 09:36:44.000000 nucliadb_node_binding-3.0.3.post1215/local_dependencies/nucliadb_vectors/src/formula/mod.rs
--rw-r--r--   0     1001      127     2165 2024-04-29 09:36:44.000000 nucliadb_node_binding-3.0.3.post1215/local_dependencies/nucliadb_vectors/src/lib.rs
--rw-r--r--   0     1001      127     1278 2024-04-29 09:36:44.000000 nucliadb_node_binding-3.0.3.post1215/local_dependencies/nucliadb_vectors/src/service/mod.rs
--rw-r--r--   0     1001      127     1897 2024-04-29 09:36:44.000000 nucliadb_node_binding-3.0.3.post1215/local_dependencies/nucliadb_vectors/src/service/query_io.rs
--rw-r--r--   0     1001      127    17192 2024-04-29 09:36:44.000000 nucliadb_node_binding-3.0.3.post1215/local_dependencies/nucliadb_vectors/src/service/reader.rs
--rw-r--r--   0     1001      127    15294 2024-04-29 09:36:44.000000 nucliadb_node_binding-3.0.3.post1215/local_dependencies/nucliadb_vectors/src/service/writer.rs
--rw-r--r--   0     1001      127     1668 2024-04-29 09:36:44.000000 nucliadb_node_binding-3.0.3.post1215/local_dependencies/nucliadb_vectors/src/utils.rs
--rw-r--r--   0     1001      127     2884 2024-04-29 09:36:44.000000 nucliadb_node_binding-3.0.3.post1215/local_dependencies/nucliadb_vectors/tests/test_merge.rs
--rw-r--r--   0        0        0      361 1970-01-01 00:00:00.000000 nucliadb_node_binding-3.0.3.post1215/local_dependencies/nucliadb_procs/Cargo.toml
--rw-r--r--   0     1001      127     3409 2024-04-29 09:36:44.000000 nucliadb_node_binding-3.0.3.post1215/local_dependencies/nucliadb_procs/src/lib.rs
--rw-r--r--   0     1001      127     2885 2024-04-29 09:36:44.000000 nucliadb_node_binding-3.0.3.post1215/local_dependencies/nucliadb_procs/src/measure.rs
--rw-r--r--   0     1001      127     1081 2024-04-29 09:36:44.000000 nucliadb_node_binding-3.0.3.post1215/local_dependencies/nucliadb_procs/tests/dont_compile/actor_defined_twice.rs
--rw-r--r--   0     1001      127      222 2024-04-29 09:36:44.000000 nucliadb_node_binding-3.0.3.post1215/local_dependencies/nucliadb_procs/tests/dont_compile/actor_defined_twice.stderr
--rw-r--r--   0     1001      127     1038 2024-04-29 09:36:44.000000 nucliadb_node_binding-3.0.3.post1215/local_dependencies/nucliadb_procs/tests/dont_compile/actor_not_defined.rs
--rw-r--r--   0     1001      127      327 2024-04-29 09:36:44.000000 nucliadb_node_binding-3.0.3.post1215/local_dependencies/nucliadb_procs/tests/dont_compile/actor_not_defined.stderr
--rw-r--r--   0     1001      127     1086 2024-04-29 09:36:44.000000 nucliadb_node_binding-3.0.3.post1215/local_dependencies/nucliadb_procs/tests/dont_compile/metric_defined_twice.rs
--rw-r--r--   0     1001      127      249 2024-04-29 09:36:44.000000 nucliadb_node_binding-3.0.3.post1215/local_dependencies/nucliadb_procs/tests/dont_compile/metric_defined_twice.stderr
--rw-r--r--   0     1001      127     1046 2024-04-29 09:36:44.000000 nucliadb_node_binding-3.0.3.post1215/local_dependencies/nucliadb_procs/tests/dont_compile/wrong_actor.rs
--rw-r--r--   0     1001      127     1303 2024-04-29 09:36:44.000000 nucliadb_node_binding-3.0.3.post1215/local_dependencies/nucliadb_procs/tests/dont_compile/wrong_actor.stderr
--rw-r--r--   0     1001      127     1408 2024-04-29 09:36:44.000000 nucliadb_node_binding-3.0.3.post1215/local_dependencies/nucliadb_procs/tests/test_measure.rs
--rw-r--r--   0        0        0      629 1970-01-01 00:00:00.000000 nucliadb_node_binding-3.0.3.post1215/local_dependencies/nucliadb_paragraphs2/Cargo.toml
--rw-r--r--   0     1001      127     7796 2024-04-29 09:36:44.000000 nucliadb_node_binding-3.0.3.post1215/local_dependencies/nucliadb_paragraphs2/src/fuzzy_query.rs
--rw-r--r--   0     1001      127     1009 2024-04-29 09:36:44.000000 nucliadb_node_binding-3.0.3.post1215/local_dependencies/nucliadb_paragraphs2/src/lib.rs
--rw-r--r--   0     1001      127     2780 2024-04-29 09:36:44.000000 nucliadb_node_binding-3.0.3.post1215/local_dependencies/nucliadb_paragraphs2/src/query_io.rs
--rw-r--r--   0     1001      127    42940 2024-04-29 09:36:44.000000 nucliadb_node_binding-3.0.3.post1215/local_dependencies/nucliadb_paragraphs2/src/reader.rs
--rw-r--r--   0     1001      127     4808 2024-04-29 09:36:44.000000 nucliadb_node_binding-3.0.3.post1215/local_dependencies/nucliadb_paragraphs2/src/schema.rs
--rw-r--r--   0     1001      127    22494 2024-04-29 09:36:44.000000 nucliadb_node_binding-3.0.3.post1215/local_dependencies/nucliadb_paragraphs2/src/search_query.rs
--rw-r--r--   0     1001      127    11391 2024-04-29 09:36:44.000000 nucliadb_node_binding-3.0.3.post1215/local_dependencies/nucliadb_paragraphs2/src/search_response.rs
--rw-r--r--   0     1001      127     4090 2024-04-29 09:36:44.000000 nucliadb_node_binding-3.0.3.post1215/local_dependencies/nucliadb_paragraphs2/src/stop_words.rs
--rw-r--r--   0     1001      127    17965 2024-04-29 09:36:44.000000 nucliadb_node_binding-3.0.3.post1215/local_dependencies/nucliadb_paragraphs2/src/writer.rs
--rw-r--r--   0     1001      127       88 2024-04-29 09:36:44.000000 nucliadb_node_binding-3.0.3.post1215/local_dependencies/nucliadb_paragraphs2/stop_words/README.md
--rw-r--r--   0     1001      127    19791 2024-04-29 09:36:44.000000 nucliadb_node_binding-3.0.3.post1215/local_dependencies/nucliadb_paragraphs2/stop_words/ar.json
--rw-r--r--   0     1001      127     1923 2024-04-29 09:36:44.000000 nucliadb_node_binding-3.0.3.post1215/local_dependencies/nucliadb_paragraphs2/stop_words/az.json
--rw-r--r--   0     1001      127    11684 2024-04-29 09:36:44.000000 nucliadb_node_binding-3.0.3.post1215/local_dependencies/nucliadb_paragraphs2/stop_words/bn.json
--rw-r--r--   0     1001      127     2513 2024-04-29 09:36:44.000000 nucliadb_node_binding-3.0.3.post1215/local_dependencies/nucliadb_paragraphs2/stop_words/ca.json
--rw-r--r--   0     1001      127    12802 2024-04-29 09:36:44.000000 nucliadb_node_binding-3.0.3.post1215/local_dependencies/nucliadb_paragraphs2/stop_words/ch.json
--rw-r--r--   0     1001      127      730 2024-04-29 09:36:44.000000 nucliadb_node_binding-3.0.3.post1215/local_dependencies/nucliadb_paragraphs2/stop_words/da.json
--rw-r--r--   0     1001      127     2090 2024-04-29 09:36:44.000000 nucliadb_node_binding-3.0.3.post1215/local_dependencies/nucliadb_paragraphs2/stop_words/de.json
--rw-r--r--   0     1001      127     6284 2024-04-29 09:36:44.000000 nucliadb_node_binding-3.0.3.post1215/local_dependencies/nucliadb_paragraphs2/stop_words/el.json
--rw-r--r--   0     1001      127     1473 2024-04-29 09:36:44.000000 nucliadb_node_binding-3.0.3.post1215/local_dependencies/nucliadb_paragraphs2/stop_words/en.json
--rw-r--r--   0     1001      127     3451 2024-04-29 09:36:44.000000 nucliadb_node_binding-3.0.3.post1215/local_dependencies/nucliadb_paragraphs2/stop_words/es.json
--rw-r--r--   0     1001      127     3182 2024-04-29 09:36:44.000000 nucliadb_node_binding-3.0.3.post1215/local_dependencies/nucliadb_paragraphs2/stop_words/eu.json
--rw-r--r--   0     1001      127     2126 2024-04-29 09:36:44.000000 nucliadb_node_binding-3.0.3.post1215/local_dependencies/nucliadb_paragraphs2/stop_words/extract.py
--rw-r--r--   0     1001      127     2748 2024-04-29 09:36:44.000000 nucliadb_node_binding-3.0.3.post1215/local_dependencies/nucliadb_paragraphs2/stop_words/fi.json
--rw-r--r--   0     1001      127     1388 2024-04-29 09:36:44.000000 nucliadb_node_binding-3.0.3.post1215/local_dependencies/nucliadb_paragraphs2/stop_words/fr.json
--rw-r--r--   0     1001      127     5716 2024-04-29 09:36:44.000000 nucliadb_node_binding-3.0.3.post1215/local_dependencies/nucliadb_paragraphs2/stop_words/he.json
--rw-r--r--   0     1001      127     2108 2024-04-29 09:36:44.000000 nucliadb_node_binding-3.0.3.post1215/local_dependencies/nucliadb_paragraphs2/stop_words/hu.json
--rw-r--r--   0     1001      127     8721 2024-04-29 09:36:44.000000 nucliadb_node_binding-3.0.3.post1215/local_dependencies/nucliadb_paragraphs2/stop_words/id.json
--rw-r--r--   0     1001      127     2535 2024-04-29 09:36:44.000000 nucliadb_node_binding-3.0.3.post1215/local_dependencies/nucliadb_paragraphs2/stop_words/it.json
--rw-r--r--   0     1001      127    11737 2024-04-29 09:36:44.000000 nucliadb_node_binding-3.0.3.post1215/local_dependencies/nucliadb_paragraphs2/stop_words/kk.json
--rw-r--r--   0     1001      127     7730 2024-04-29 09:36:44.000000 nucliadb_node_binding-3.0.3.post1215/local_dependencies/nucliadb_paragraphs2/stop_words/ne.json
--rw-r--r--   0     1001      127      756 2024-04-29 09:36:44.000000 nucliadb_node_binding-3.0.3.post1215/local_dependencies/nucliadb_paragraphs2/stop_words/nl.json
--rw-r--r--   0     1001      127     1447 2024-04-29 09:36:44.000000 nucliadb_node_binding-3.0.3.post1215/local_dependencies/nucliadb_paragraphs2/stop_words/no.json
--rw-r--r--   0     1001      127     2055 2024-04-29 09:36:44.000000 nucliadb_node_binding-3.0.3.post1215/local_dependencies/nucliadb_paragraphs2/stop_words/pt.json
--rw-r--r--   0     1001      127     3327 2024-04-29 09:36:44.000000 nucliadb_node_binding-3.0.3.post1215/local_dependencies/nucliadb_paragraphs2/stop_words/ro.json
--rw-r--r--   0     1001      127     3856 2024-04-29 09:36:44.000000 nucliadb_node_binding-3.0.3.post1215/local_dependencies/nucliadb_paragraphs2/stop_words/ru.json
--rw-r--r--   0     1001      127    23032 2024-04-29 09:36:44.000000 nucliadb_node_binding-3.0.3.post1215/local_dependencies/nucliadb_paragraphs2/stop_words/sl.json
--rw-r--r--   0     1001      127      993 2024-04-29 09:36:44.000000 nucliadb_node_binding-3.0.3.post1215/local_dependencies/nucliadb_paragraphs2/stop_words/sv.json
--rw-r--r--   0     1001      127     5424 2024-04-29 09:36:44.000000 nucliadb_node_binding-3.0.3.post1215/local_dependencies/nucliadb_paragraphs2/stop_words/tg.json
--rw-r--r--   0     1001      127      491 2024-04-29 09:36:44.000000 nucliadb_node_binding-3.0.3.post1215/local_dependencies/nucliadb_paragraphs2/stop_words/tr.json
--rw-r--r--   0        0        0      931 1970-01-01 00:00:00.000000 nucliadb_node_binding-3.0.3.post1215/local_dependencies/nucliadb_core/Cargo.toml
--rw-r--r--   0     1001      127     5872 2024-04-29 09:36:44.000000 nucliadb_node_binding-3.0.3.post1215/local_dependencies/nucliadb_core/src/fs_state.rs
--rw-r--r--   0     1001      127     2681 2024-04-29 09:36:44.000000 nucliadb_node_binding-3.0.3.post1215/local_dependencies/nucliadb_core/src/lib.rs
--rw-r--r--   0     1001      127     2295 2024-04-29 09:36:44.000000 nucliadb_node_binding-3.0.3.post1215/local_dependencies/nucliadb_core/src/merge.rs
--rw-r--r--   0     1001      127      906 2024-04-29 09:36:44.000000 nucliadb_node_binding-3.0.3.post1215/local_dependencies/nucliadb_core/src/metrics/meters/mod.rs
--rw-r--r--   0     1001      127     4869 2024-04-29 09:36:44.000000 nucliadb_node_binding-3.0.3.post1215/local_dependencies/nucliadb_core/src/metrics/meters/prometheus.rs
--rw-r--r--   0     1001      127     1702 2024-04-29 09:36:44.000000 nucliadb_node_binding-3.0.3.post1215/local_dependencies/nucliadb_core/src/metrics/metric/grpc_ops.rs
--rw-r--r--   0     1001      127     1442 2024-04-29 09:36:44.000000 nucliadb_node_binding-3.0.3.post1215/local_dependencies/nucliadb_core/src/metrics/metric/mod.rs
--rw-r--r--   0     1001      127     1950 2024-04-29 09:36:44.000000 nucliadb_node_binding-3.0.3.post1215/local_dependencies/nucliadb_core/src/metrics/metric/replication.rs
--rw-r--r--   0     1001      127     2626 2024-04-29 09:36:44.000000 nucliadb_node_binding-3.0.3.post1215/local_dependencies/nucliadb_core/src/metrics/metric/request_time.rs
--rw-r--r--   0     1001      127     1644 2024-04-29 09:36:44.000000 nucliadb_node_binding-3.0.3.post1215/local_dependencies/nucliadb_core/src/metrics/metric/shard_cache.rs
--rw-r--r--   0     1001      127    21641 2024-04-29 09:36:44.000000 nucliadb_node_binding-3.0.3.post1215/local_dependencies/nucliadb_core/src/metrics/metric/tokio_runtime.rs
--rw-r--r--   0     1001      127    16736 2024-04-29 09:36:44.000000 nucliadb_node_binding-3.0.3.post1215/local_dependencies/nucliadb_core/src/metrics/metric/tokio_tasks.rs
--rw-r--r--   0     1001      127     3415 2024-04-29 09:36:44.000000 nucliadb_node_binding-3.0.3.post1215/local_dependencies/nucliadb_core/src/metrics/metric/vectors.rs
--rw-r--r--   0     1001      127     1324 2024-04-29 09:36:44.000000 nucliadb_node_binding-3.0.3.post1215/local_dependencies/nucliadb_core/src/metrics/mod.rs
--rw-r--r--   0     1001      127     3074 2024-04-29 09:36:44.000000 nucliadb_node_binding-3.0.3.post1215/local_dependencies/nucliadb_core/src/metrics/task_monitor.rs
--rw-r--r--   0     1001      127     3920 2024-04-29 09:36:44.000000 nucliadb_node_binding-3.0.3.post1215/local_dependencies/nucliadb_core/src/metrics/tests.rs
--rw-r--r--   0     1001      127     2990 2024-04-29 09:36:44.000000 nucliadb_node_binding-3.0.3.post1215/local_dependencies/nucliadb_core/src/paragraphs.rs
--rw-r--r--   0     1001      127    17305 2024-04-29 09:36:44.000000 nucliadb_node_binding-3.0.3.post1215/local_dependencies/nucliadb_core/src/query_language/mod.rs
--rw-r--r--   0     1001      127    15367 2024-04-29 09:36:44.000000 nucliadb_node_binding-3.0.3.post1215/local_dependencies/nucliadb_core/src/query_planner.rs
--rw-r--r--   0     1001      127     2069 2024-04-29 09:36:44.000000 nucliadb_node_binding-3.0.3.post1215/local_dependencies/nucliadb_core/src/relations.rs
--rw-r--r--   0     1001      127     8250 2024-04-29 09:36:44.000000 nucliadb_node_binding-3.0.3.post1215/local_dependencies/nucliadb_core/src/tantivy_replica.rs
--rw-r--r--   0     1001      127     2603 2024-04-29 09:36:44.000000 nucliadb_node_binding-3.0.3.post1215/local_dependencies/nucliadb_core/src/texts.rs
--rw-r--r--   0     1001      127     3559 2024-04-29 09:36:44.000000 nucliadb_node_binding-3.0.3.post1215/local_dependencies/nucliadb_core/src/vectors.rs
--rw-r--r--   0        0        0     3212 1970-01-01 00:00:00.000000 nucliadb_node_binding-3.0.3.post1215/local_dependencies/nucliadb_node/Cargo.toml
--rw-r--r--   0     1001      127     1045 2024-04-29 09:36:44.000000 nucliadb_node_binding-3.0.3.post1215/local_dependencies/nucliadb_node/.rustc_info.json
--rw-r--r--   0     1001      127      877 2024-04-29 09:36:44.000000 nucliadb_node_binding-3.0.3.post1215/local_dependencies/nucliadb_node/Makefile
--rw-r--r--   0     1001      127     1500 2024-04-29 09:36:44.000000 nucliadb_node_binding-3.0.3.post1215/local_dependencies/nucliadb_node/README.md
--rw-r--r--   0     1001      127     1757 2024-04-29 09:36:44.000000 nucliadb_node_binding-3.0.3.post1215/local_dependencies/nucliadb_node/nucliadb_node/__init__.py
--rw-r--r--   0     1001      127     3957 2024-04-29 09:36:44.000000 nucliadb_node_binding-3.0.3.post1215/local_dependencies/nucliadb_node/nucliadb_node/app.py
--rw-r--r--   0     1001      127    17752 2024-04-29 09:36:44.000000 nucliadb_node_binding-3.0.3.post1215/local_dependencies/nucliadb_node/nucliadb_node/indexer.py
--rw-r--r--   0     1001      127      890 2024-04-29 09:36:44.000000 nucliadb_node_binding-3.0.3.post1215/local_dependencies/nucliadb_node/nucliadb_node/listeners/__init__.py
--rw-r--r--   0     1001      127     2424 2024-04-29 09:36:44.000000 nucliadb_node_binding-3.0.3.post1215/local_dependencies/nucliadb_node/nucliadb_node/listeners/indexed_publisher.py
--rw-r--r--   0     1001      127     4015 2024-04-29 09:36:44.000000 nucliadb_node_binding-3.0.3.post1215/local_dependencies/nucliadb_node/nucliadb_node/pull.py
--rw-r--r--   0     1001      127     1535 2024-04-29 09:36:44.000000 nucliadb_node_binding-3.0.3.post1215/local_dependencies/nucliadb_node/nucliadb_node/service.py
--rw-r--r--   0     1001      127     1487 2024-04-29 09:36:44.000000 nucliadb_node_binding-3.0.3.post1215/local_dependencies/nucliadb_node/nucliadb_node/settings.py
--rw-r--r--   0     1001      127     1133 2024-04-29 09:36:44.000000 nucliadb_node_binding-3.0.3.post1215/local_dependencies/nucliadb_node/nucliadb_node/signals.py
--rw-r--r--   0     1001      127      835 2024-04-29 09:36:44.000000 nucliadb_node_binding-3.0.3.post1215/local_dependencies/nucliadb_node/nucliadb_node/tests/__init__.py
--rw-r--r--   0     1001      127     1092 2024-04-29 09:36:44.000000 nucliadb_node_binding-3.0.3.post1215/local_dependencies/nucliadb_node/nucliadb_node/tests/conftest.py
--rw-r--r--   0     1001      127    10810 2024-04-29 09:36:44.000000 nucliadb_node_binding-3.0.3.post1215/local_dependencies/nucliadb_node/nucliadb_node/tests/fixtures.py
--rw-r--r--   0     1001      127    13788 2024-04-29 09:36:44.000000 nucliadb_node_binding-3.0.3.post1215/local_dependencies/nucliadb_node/nucliadb_node/tests/integration/test_indexing.py
--rw-r--r--   0     1001      127     2289 2024-04-29 09:36:44.000000 nucliadb_node_binding-3.0.3.post1215/local_dependencies/nucliadb_node/nucliadb_node/tests/unit/test_app.py
--rw-r--r--   0     1001      127     2361 2024-04-29 09:36:44.000000 nucliadb_node_binding-3.0.3.post1215/local_dependencies/nucliadb_node/nucliadb_node/tests/unit/test_indexed_publisher.py
--rw-r--r--   0     1001      127    12553 2024-04-29 09:36:44.000000 nucliadb_node_binding-3.0.3.post1215/local_dependencies/nucliadb_node/nucliadb_node/tests/unit/test_indexer.py
--rw-r--r--   0     1001      127     3379 2024-04-29 09:36:44.000000 nucliadb_node_binding-3.0.3.post1215/local_dependencies/nucliadb_node/nucliadb_node/tests/unit/test_pull.py
--rw-r--r--   0     1001      127     2323 2024-04-29 09:36:44.000000 nucliadb_node_binding-3.0.3.post1215/local_dependencies/nucliadb_node/nucliadb_node/writer.py
--rw-r--r--   0     1001      127      101 2024-04-29 09:36:44.000000 nucliadb_node_binding-3.0.3.post1215/local_dependencies/nucliadb_node/requirements-sources.txt
--rw-r--r--   0     1001      127      276 2024-04-29 09:36:44.000000 nucliadb_node_binding-3.0.3.post1215/local_dependencies/nucliadb_node/requirements.txt
--rw-r--r--   0     1001      127      249 2024-04-29 09:36:44.000000 nucliadb_node_binding-3.0.3.post1215/local_dependencies/nucliadb_node/setup.cfg
--rw-r--r--   0     1001      127     1405 2024-04-29 09:36:44.000000 nucliadb_node_binding-3.0.3.post1215/local_dependencies/nucliadb_node/setup.py
--rw-r--r--   0     1001      127     2518 2024-04-29 09:36:44.000000 nucliadb_node_binding-3.0.3.post1215/local_dependencies/nucliadb_node/src/analytics/blocking.rs
--rw-r--r--   0     1001      127     1219 2024-04-29 09:36:44.000000 nucliadb_node_binding-3.0.3.post1215/local_dependencies/nucliadb_node/src/analytics/mod.rs
--rw-r--r--   0     1001      127     4931 2024-04-29 09:36:44.000000 nucliadb_node_binding-3.0.3.post1215/local_dependencies/nucliadb_node/src/analytics/payload.rs
--rw-r--r--   0     1001      127    12828 2024-04-29 09:36:44.000000 nucliadb_node_binding-3.0.3.post1215/local_dependencies/nucliadb_node/src/analytics/sender.rs
--rw-r--r--   0     1001      127     3085 2024-04-29 09:36:44.000000 nucliadb_node_binding-3.0.3.post1215/local_dependencies/nucliadb_node/src/analytics/sink.rs
--rw-r--r--   0     1001      127     1900 2024-04-29 09:36:44.000000 nucliadb_node_binding-3.0.3.post1215/local_dependencies/nucliadb_node/src/analytics/sync.rs
--rw-r--r--   0     1001      127     5045 2024-04-29 09:36:44.000000 nucliadb_node_binding-3.0.3.post1215/local_dependencies/nucliadb_node/src/bin/reader.rs
--rw-r--r--   0     1001      127     8050 2024-04-29 09:36:44.000000 nucliadb_node_binding-3.0.3.post1215/local_dependencies/nucliadb_node/src/bin/writer.rs
--rw-r--r--   0     1001      127     1345 2024-04-29 09:36:44.000000 nucliadb_node_binding-3.0.3.post1215/local_dependencies/nucliadb_node/src/cache/mod.rs
--rw-r--r--   0     1001      127     3035 2024-04-29 09:36:44.000000 nucliadb_node_binding-3.0.3.post1215/local_dependencies/nucliadb_node/src/cache/reader_cache.rs
--rw-r--r--   0     1001      127    14199 2024-04-29 09:36:44.000000 nucliadb_node_binding-3.0.3.post1215/local_dependencies/nucliadb_node/src/cache/resource_cache.rs
--rw-r--r--   0     1001      127    11029 2024-04-29 09:36:44.000000 nucliadb_node_binding-3.0.3.post1215/local_dependencies/nucliadb_node/src/cache/writer_cache.rs
--rw-r--r--   0     1001      127     1771 2024-04-29 09:36:44.000000 nucliadb_node_binding-3.0.3.post1215/local_dependencies/nucliadb_node/src/disk_structure.rs
--rw-r--r--   0     1001      127     1111 2024-04-29 09:36:44.000000 nucliadb_node_binding-3.0.3.post1215/local_dependencies/nucliadb_node/src/errors.rs
--rw-r--r--   0     1001      127     2656 2024-04-29 09:36:44.000000 nucliadb_node_binding-3.0.3.post1215/local_dependencies/nucliadb_node/src/grpc/collect_garbage.rs
--rw-r--r--   0     1001      127    18813 2024-04-29 09:36:44.000000 nucliadb_node_binding-3.0.3.post1215/local_dependencies/nucliadb_node/src/grpc/grpc_reader.rs
--rw-r--r--   0     1001      127    13722 2024-04-29 09:36:44.000000 nucliadb_node_binding-3.0.3.post1215/local_dependencies/nucliadb_node/src/grpc/grpc_writer.rs
--rw-r--r--   0     1001      127     3186 2024-04-29 09:36:44.000000 nucliadb_node_binding-3.0.3.post1215/local_dependencies/nucliadb_node/src/grpc/middleware/debug.rs
--rw-r--r--   0     1001      127     3440 2024-04-29 09:36:44.000000 nucliadb_node_binding-3.0.3.post1215/local_dependencies/nucliadb_node/src/grpc/middleware/metrics.rs
--rw-r--r--   0     1001      127     1009 2024-04-29 09:36:44.000000 nucliadb_node_binding-3.0.3.post1215/local_dependencies/nucliadb_node/src/grpc/middleware/mod.rs
--rw-r--r--   0     1001      127     4158 2024-04-29 09:36:44.000000 nucliadb_node_binding-3.0.3.post1215/local_dependencies/nucliadb_node/src/grpc/middleware/telemetry.rs
--rw-r--r--   0     1001      127     1283 2024-04-29 09:36:44.000000 nucliadb_node_binding-3.0.3.post1215/local_dependencies/nucliadb_node/src/grpc/mod.rs
--rw-r--r--   0     1001      127     2581 2024-04-29 09:36:44.000000 nucliadb_node_binding-3.0.3.post1215/local_dependencies/nucliadb_node/src/grpc/update.rs
--rw-r--r--   0     1001      127     1173 2024-04-29 09:36:44.000000 nucliadb_node_binding-3.0.3.post1215/local_dependencies/nucliadb_node/src/http_server/metrics_service.rs
--rw-r--r--   0     1001      127     1465 2024-04-29 09:36:44.000000 nucliadb_node_binding-3.0.3.post1215/local_dependencies/nucliadb_node/src/http_server/mod.rs
--rw-r--r--   0     1001      127     1943 2024-04-29 09:36:44.000000 nucliadb_node_binding-3.0.3.post1215/local_dependencies/nucliadb_node/src/http_server/traces_service.rs
--rw-r--r--   0     1001      127     1504 2024-04-29 09:36:44.000000 nucliadb_node_binding-3.0.3.post1215/local_dependencies/nucliadb_node/src/lib.rs
--rw-r--r--   0     1001      127     2757 2024-04-29 09:36:44.000000 nucliadb_node_binding-3.0.3.post1215/local_dependencies/nucliadb_node/src/lifecycle.rs
--rw-r--r--   0     1001      127     1778 2024-04-29 09:36:44.000000 nucliadb_node_binding-3.0.3.post1215/local_dependencies/nucliadb_node/src/merge/global.rs
--rw-r--r--   0     1001      127     1089 2024-04-29 09:36:44.000000 nucliadb_node_binding-3.0.3.post1215/local_dependencies/nucliadb_node/src/merge/mod.rs
--rw-r--r--   0     1001      127    13672 2024-04-29 09:36:44.000000 nucliadb_node_binding-3.0.3.post1215/local_dependencies/nucliadb_node/src/merge/scheduler.rs
--rw-r--r--   0     1001      127     3677 2024-04-29 09:36:44.000000 nucliadb_node_binding-3.0.3.post1215/local_dependencies/nucliadb_node/src/merge/work.rs
--rw-r--r--   0     1001      127     1935 2024-04-29 09:36:44.000000 nucliadb_node_binding-3.0.3.post1215/local_dependencies/nucliadb_node/src/node_metadata.rs
--rw-r--r--   0     1001      127     2417 2024-04-29 09:36:44.000000 nucliadb_node_binding-3.0.3.post1215/local_dependencies/nucliadb_node/src/replication/health.rs
--rw-r--r--   0     1001      127     1070 2024-04-29 09:36:44.000000 nucliadb_node_binding-3.0.3.post1215/local_dependencies/nucliadb_node/src/replication/mod.rs
--rw-r--r--   0     1001      127    14103 2024-04-29 09:36:44.000000 nucliadb_node_binding-3.0.3.post1215/local_dependencies/nucliadb_node/src/replication/replicator.rs
--rw-r--r--   0     1001      127    11755 2024-04-29 09:36:44.000000 nucliadb_node_binding-3.0.3.post1215/local_dependencies/nucliadb_node/src/replication/service.rs
--rw-r--r--   0     1001      127    11615 2024-04-29 09:36:44.000000 nucliadb_node_binding-3.0.3.post1215/local_dependencies/nucliadb_node/src/settings.rs
--rw-r--r--   0     1001      127     1111 2024-04-29 09:36:44.000000 nucliadb_node_binding-3.0.3.post1215/local_dependencies/nucliadb_node/src/shards/errors.rs
--rw-r--r--   0     1001      127    11409 2024-04-29 09:36:44.000000 nucliadb_node_binding-3.0.3.post1215/local_dependencies/nucliadb_node/src/shards/metadata.rs
--rw-r--r--   0     1001      127     1127 2024-04-29 09:36:44.000000 nucliadb_node_binding-3.0.3.post1215/local_dependencies/nucliadb_node/src/shards/mod.rs
--rw-r--r--   0     1001      127    27149 2024-04-29 09:36:44.000000 nucliadb_node_binding-3.0.3.post1215/local_dependencies/nucliadb_node/src/shards/shard_reader.rs
--rw-r--r--   0     1001      127    23537 2024-04-29 09:36:44.000000 nucliadb_node_binding-3.0.3.post1215/local_dependencies/nucliadb_node/src/shards/shard_writer.rs
--rw-r--r--   0     1001      127     1887 2024-04-29 09:36:44.000000 nucliadb_node_binding-3.0.3.post1215/local_dependencies/nucliadb_node/src/shards/versioning.rs
--rw-r--r--   0     1001      127    10170 2024-04-29 09:36:44.000000 nucliadb_node_binding-3.0.3.post1215/local_dependencies/nucliadb_node/src/telemetry.rs
--rw-r--r--   0     1001      127     6396 2024-04-29 09:36:44.000000 nucliadb_node_binding-3.0.3.post1215/local_dependencies/nucliadb_node/src/utils.rs
--rw-r--r--   0     1001      127       42 2024-04-29 09:36:44.000000 nucliadb_node_binding-3.0.3.post1215/local_dependencies/nucliadb_node/test.sh
--rw-r--r--   0     1001      127     1115 2024-04-29 09:36:44.000000 nucliadb_node_binding-3.0.3.post1215/local_dependencies/nucliadb_node/tests/common/mod.rs
--rw-r--r--   0     1001      127    12731 2024-04-29 09:36:44.000000 nucliadb_node_binding-3.0.3.post1215/local_dependencies/nucliadb_node/tests/common/node_services.rs
--rw-r--r--   0     1001      127     7823 2024-04-29 09:36:44.000000 nucliadb_node_binding-3.0.3.post1215/local_dependencies/nucliadb_node/tests/common/resources.rs
--rw-r--r--   0     1001      127     8173 2024-04-29 09:36:44.000000 nucliadb_node_binding-3.0.3.post1215/local_dependencies/nucliadb_node/tests/test_date_range_search.rs
--rw-r--r--   0     1001      127     4089 2024-04-29 09:36:44.000000 nucliadb_node_binding-3.0.3.post1215/local_dependencies/nucliadb_node/tests/test_download.rs
--rw-r--r--   0     1001      127     1684 2024-04-29 09:36:44.000000 nucliadb_node_binding-3.0.3.post1215/local_dependencies/nucliadb_node/tests/test_merge.rs
--rw-r--r--   0     1001      127     6003 2024-04-29 09:36:44.000000 nucliadb_node_binding-3.0.3.post1215/local_dependencies/nucliadb_node/tests/test_replication.rs
--rw-r--r--   0     1001      127    22494 2024-04-29 09:36:44.000000 nucliadb_node_binding-3.0.3.post1215/local_dependencies/nucliadb_node/tests/test_search_relations.rs
--rw-r--r--   0     1001      127     6958 2024-04-29 09:36:44.000000 nucliadb_node_binding-3.0.3.post1215/local_dependencies/nucliadb_node/tests/test_search_sorting.rs
--rw-r--r--   0     1001      127     7044 2024-04-29 09:36:44.000000 nucliadb_node_binding-3.0.3.post1215/local_dependencies/nucliadb_node/tests/test_security_search.rs
--rw-r--r--   0     1001      127     6862 2024-04-29 09:36:44.000000 nucliadb_node_binding-3.0.3.post1215/local_dependencies/nucliadb_node/tests/test_shards.rs
--rw-r--r--   0     1001      127    10698 2024-04-29 09:36:44.000000 nucliadb_node_binding-3.0.3.post1215/local_dependencies/nucliadb_node/tests/test_suggest.rs
--rw-r--r--   0     1001      127     5438 2024-04-29 09:36:44.000000 nucliadb_node_binding-3.0.3.post1215/local_dependencies/nucliadb_node/tests/test_vector_normalization.rs
--rw-r--r--   0        0        0      501 1970-01-01 00:00:00.000000 nucliadb_node_binding-3.0.3.post1215/local_dependencies/nucliadb_protos/Cargo.toml
--rw-r--r--   0     1001      127     2155 2024-04-29 09:36:44.000000 nucliadb_node_binding-3.0.3.post1215/local_dependencies/nucliadb_protos/build.rs
--rw-r--r--   0     1001      127    26110 2024-04-29 09:36:44.000000 nucliadb_node_binding-3.0.3.post1215/local_dependencies/nucliadb_protos/src/fdbwriter.rs
--rw-r--r--   0     1001      127        0 2024-04-29 09:36:44.000000 nucliadb_node_binding-3.0.3.post1215/local_dependencies/nucliadb_protos/src/google.protobuf.rs
--rw-r--r--   0     1001      127     9795 2024-04-29 09:36:44.000000 nucliadb_node_binding-3.0.3.post1215/local_dependencies/nucliadb_protos/src/knowledgebox.rs
--rw-r--r--   0     1001      127     1256 2024-04-29 09:36:44.000000 nucliadb_node_binding-3.0.3.post1215/local_dependencies/nucliadb_protos/src/lib.rs
--rw-r--r--   0     1001      127    77311 2024-04-29 09:36:44.000000 nucliadb_node_binding-3.0.3.post1215/local_dependencies/nucliadb_protos/src/nodereader.rs
--rw-r--r--   0     1001      127    10240 2024-04-29 09:36:44.000000 nucliadb_node_binding-3.0.3.post1215/local_dependencies/nucliadb_protos/src/noderesources.rs
--rw-r--r--   0     1001      127    43352 2024-04-29 09:36:44.000000 nucliadb_node_binding-3.0.3.post1215/local_dependencies/nucliadb_protos/src/nodewriter.rs
--rw-r--r--   0     1001      127    19010 2024-04-29 09:36:44.000000 nucliadb_node_binding-3.0.3.post1215/local_dependencies/nucliadb_protos/src/replication.rs
--rw-r--r--   0     1001      127    33352 2024-04-29 09:36:44.000000 nucliadb_node_binding-3.0.3.post1215/local_dependencies/nucliadb_protos/src/resources.rs
--rw-r--r--   0     1001      127     5528 2024-04-29 09:36:44.000000 nucliadb_node_binding-3.0.3.post1215/local_dependencies/nucliadb_protos/src/utils.rs
--rw-r--r--   0        0        0      708 1970-01-01 00:00:00.000000 nucliadb_node_binding-3.0.3.post1215/local_dependencies/nucliadb_relations2/Cargo.toml
--rw-r--r--   0     1001      127     3593 2024-04-29 09:36:44.000000 nucliadb_node_binding-3.0.3.post1215/local_dependencies/nucliadb_relations2/src/io_maps.rs
--rw-r--r--   0     1001      127      916 2024-04-29 09:36:44.000000 nucliadb_node_binding-3.0.3.post1215/local_dependencies/nucliadb_relations2/src/lib.rs
--rw-r--r--   0     1001      127    17039 2024-04-29 09:36:44.000000 nucliadb_node_binding-3.0.3.post1215/local_dependencies/nucliadb_relations2/src/reader.rs
--rw-r--r--   0     1001      127     7123 2024-04-29 09:36:44.000000 nucliadb_node_binding-3.0.3.post1215/local_dependencies/nucliadb_relations2/src/schema.rs
--rw-r--r--   0     1001      127     8007 2024-04-29 09:36:44.000000 nucliadb_node_binding-3.0.3.post1215/local_dependencies/nucliadb_relations2/src/writer.rs
--rw-r--r--   0     1001      127     1802 2024-04-29 09:36:44.000000 nucliadb_node_binding-3.0.3.post1215/local_dependencies/nucliadb_relations2/tests/common/mod.rs
--rw-r--r--   0     1001      127     9445 2024-04-29 09:36:44.000000 nucliadb_node_binding-3.0.3.post1215/local_dependencies/nucliadb_relations2/tests/test_reader.rs
--rw-r--r--   0     1001      127     3297 2024-04-29 09:36:44.000000 nucliadb_node_binding-3.0.3.post1215/local_dependencies/nucliadb_relations2/tests/test_writer.rs
--rw-r--r--   0        0        0      943 1970-01-01 00:00:00.000000 nucliadb_node_binding-3.0.3.post1215/Cargo.toml
--rw-r--r--   0     1001      127     1553 2024-04-29 09:36:44.000000 nucliadb_node_binding-3.0.3.post1215/CHANGELOG.md
--rw-r--r--   0     1001      127      895 2024-04-29 09:36:44.000000 nucliadb_node_binding-3.0.3.post1215/Makefile
--rw-r--r--   0     1001      127       52 2024-04-29 09:36:44.000000 nucliadb_node_binding-3.0.3.post1215/README.md
--rwxr-xr-x   0     1001      127      978 2024-04-29 09:36:44.000000 nucliadb_node_binding-3.0.3.post1215/cov.sh
--rw-r--r--   0     1001      127     1309 2024-04-29 09:36:44.000000 nucliadb_node_binding-3.0.3.post1215/pyproject.toml
--rw-r--r--   0     1001      127     2195 2024-04-29 09:36:44.000000 nucliadb_node_binding-3.0.3.post1215/src/collect_garbage.rs
--rw-r--r--   0     1001      127     1212 2024-04-29 09:36:44.000000 nucliadb_node_binding-3.0.3.post1215/src/errors.rs
--rw-r--r--   0     1001      127     2337 2024-04-29 09:36:44.000000 nucliadb_node_binding-3.0.3.post1215/src/lib.rs
--rw-r--r--   0     1001      127     9405 2024-04-29 09:36:44.000000 nucliadb_node_binding-3.0.3.post1215/src/reader.rs
--rw-r--r--   0     1001      127     2154 2024-04-29 09:36:44.000000 nucliadb_node_binding-3.0.3.post1215/src/update.rs
--rw-r--r--   0     1001      127     9162 2024-04-29 09:36:44.000000 nucliadb_node_binding-3.0.3.post1215/src/writer.rs
--rw-r--r--   0     1001      127      835 2024-04-29 09:36:44.000000 nucliadb_node_binding-3.0.3.post1215/tests/__init__.py
--rw-r--r--   0     1001      127      892 2024-04-29 09:36:44.000000 nucliadb_node_binding-3.0.3.post1215/tests/conftest.py
--rw-r--r--   0     1001      127     3903 2024-04-29 09:36:44.000000 nucliadb_node_binding-3.0.3.post1215/tests/integration/test_indexing.py
--rw-r--r--   0        0        0      401 1970-01-01 00:00:00.000000 nucliadb_node_binding-3.0.3.post1215/PKG-INFO
+-rw-r--r--   0        0        0     3212 1970-01-01 00:00:00.000000 nucliadb_node_binding-3.0.3.post1216/local_dependencies/nucliadb_node/Cargo.toml
+-rw-r--r--   0     1001      127     1045 2024-04-29 09:43:04.000000 nucliadb_node_binding-3.0.3.post1216/local_dependencies/nucliadb_node/.rustc_info.json
+-rw-r--r--   0     1001      127      877 2024-04-29 09:43:04.000000 nucliadb_node_binding-3.0.3.post1216/local_dependencies/nucliadb_node/Makefile
+-rw-r--r--   0     1001      127     1500 2024-04-29 09:43:04.000000 nucliadb_node_binding-3.0.3.post1216/local_dependencies/nucliadb_node/README.md
+-rw-r--r--   0     1001      127     1757 2024-04-29 09:43:04.000000 nucliadb_node_binding-3.0.3.post1216/local_dependencies/nucliadb_node/nucliadb_node/__init__.py
+-rw-r--r--   0     1001      127     3957 2024-04-29 09:43:04.000000 nucliadb_node_binding-3.0.3.post1216/local_dependencies/nucliadb_node/nucliadb_node/app.py
+-rw-r--r--   0     1001      127    17752 2024-04-29 09:43:04.000000 nucliadb_node_binding-3.0.3.post1216/local_dependencies/nucliadb_node/nucliadb_node/indexer.py
+-rw-r--r--   0     1001      127      890 2024-04-29 09:43:04.000000 nucliadb_node_binding-3.0.3.post1216/local_dependencies/nucliadb_node/nucliadb_node/listeners/__init__.py
+-rw-r--r--   0     1001      127     2424 2024-04-29 09:43:04.000000 nucliadb_node_binding-3.0.3.post1216/local_dependencies/nucliadb_node/nucliadb_node/listeners/indexed_publisher.py
+-rw-r--r--   0     1001      127     4015 2024-04-29 09:43:04.000000 nucliadb_node_binding-3.0.3.post1216/local_dependencies/nucliadb_node/nucliadb_node/pull.py
+-rw-r--r--   0     1001      127     1535 2024-04-29 09:43:04.000000 nucliadb_node_binding-3.0.3.post1216/local_dependencies/nucliadb_node/nucliadb_node/service.py
+-rw-r--r--   0     1001      127     1487 2024-04-29 09:43:04.000000 nucliadb_node_binding-3.0.3.post1216/local_dependencies/nucliadb_node/nucliadb_node/settings.py
+-rw-r--r--   0     1001      127     1133 2024-04-29 09:43:04.000000 nucliadb_node_binding-3.0.3.post1216/local_dependencies/nucliadb_node/nucliadb_node/signals.py
+-rw-r--r--   0     1001      127      835 2024-04-29 09:43:04.000000 nucliadb_node_binding-3.0.3.post1216/local_dependencies/nucliadb_node/nucliadb_node/tests/__init__.py
+-rw-r--r--   0     1001      127     1092 2024-04-29 09:43:04.000000 nucliadb_node_binding-3.0.3.post1216/local_dependencies/nucliadb_node/nucliadb_node/tests/conftest.py
+-rw-r--r--   0     1001      127    10810 2024-04-29 09:43:04.000000 nucliadb_node_binding-3.0.3.post1216/local_dependencies/nucliadb_node/nucliadb_node/tests/fixtures.py
+-rw-r--r--   0     1001      127    13788 2024-04-29 09:43:04.000000 nucliadb_node_binding-3.0.3.post1216/local_dependencies/nucliadb_node/nucliadb_node/tests/integration/test_indexing.py
+-rw-r--r--   0     1001      127     2289 2024-04-29 09:43:04.000000 nucliadb_node_binding-3.0.3.post1216/local_dependencies/nucliadb_node/nucliadb_node/tests/unit/test_app.py
+-rw-r--r--   0     1001      127     2361 2024-04-29 09:43:04.000000 nucliadb_node_binding-3.0.3.post1216/local_dependencies/nucliadb_node/nucliadb_node/tests/unit/test_indexed_publisher.py
+-rw-r--r--   0     1001      127    12553 2024-04-29 09:43:04.000000 nucliadb_node_binding-3.0.3.post1216/local_dependencies/nucliadb_node/nucliadb_node/tests/unit/test_indexer.py
+-rw-r--r--   0     1001      127     3379 2024-04-29 09:43:04.000000 nucliadb_node_binding-3.0.3.post1216/local_dependencies/nucliadb_node/nucliadb_node/tests/unit/test_pull.py
+-rw-r--r--   0     1001      127     2323 2024-04-29 09:43:04.000000 nucliadb_node_binding-3.0.3.post1216/local_dependencies/nucliadb_node/nucliadb_node/writer.py
+-rw-r--r--   0     1001      127      101 2024-04-29 09:43:04.000000 nucliadb_node_binding-3.0.3.post1216/local_dependencies/nucliadb_node/requirements-sources.txt
+-rw-r--r--   0     1001      127      276 2024-04-29 09:43:04.000000 nucliadb_node_binding-3.0.3.post1216/local_dependencies/nucliadb_node/requirements.txt
+-rw-r--r--   0     1001      127      249 2024-04-29 09:43:04.000000 nucliadb_node_binding-3.0.3.post1216/local_dependencies/nucliadb_node/setup.cfg
+-rw-r--r--   0     1001      127     1405 2024-04-29 09:43:04.000000 nucliadb_node_binding-3.0.3.post1216/local_dependencies/nucliadb_node/setup.py
+-rw-r--r--   0     1001      127     2518 2024-04-29 09:43:04.000000 nucliadb_node_binding-3.0.3.post1216/local_dependencies/nucliadb_node/src/analytics/blocking.rs
+-rw-r--r--   0     1001      127     1219 2024-04-29 09:43:04.000000 nucliadb_node_binding-3.0.3.post1216/local_dependencies/nucliadb_node/src/analytics/mod.rs
+-rw-r--r--   0     1001      127     4931 2024-04-29 09:43:04.000000 nucliadb_node_binding-3.0.3.post1216/local_dependencies/nucliadb_node/src/analytics/payload.rs
+-rw-r--r--   0     1001      127    12828 2024-04-29 09:43:04.000000 nucliadb_node_binding-3.0.3.post1216/local_dependencies/nucliadb_node/src/analytics/sender.rs
+-rw-r--r--   0     1001      127     3085 2024-04-29 09:43:04.000000 nucliadb_node_binding-3.0.3.post1216/local_dependencies/nucliadb_node/src/analytics/sink.rs
+-rw-r--r--   0     1001      127     1900 2024-04-29 09:43:04.000000 nucliadb_node_binding-3.0.3.post1216/local_dependencies/nucliadb_node/src/analytics/sync.rs
+-rw-r--r--   0     1001      127     5045 2024-04-29 09:43:04.000000 nucliadb_node_binding-3.0.3.post1216/local_dependencies/nucliadb_node/src/bin/reader.rs
+-rw-r--r--   0     1001      127     8050 2024-04-29 09:43:04.000000 nucliadb_node_binding-3.0.3.post1216/local_dependencies/nucliadb_node/src/bin/writer.rs
+-rw-r--r--   0     1001      127     1345 2024-04-29 09:43:04.000000 nucliadb_node_binding-3.0.3.post1216/local_dependencies/nucliadb_node/src/cache/mod.rs
+-rw-r--r--   0     1001      127     3035 2024-04-29 09:43:04.000000 nucliadb_node_binding-3.0.3.post1216/local_dependencies/nucliadb_node/src/cache/reader_cache.rs
+-rw-r--r--   0     1001      127    14199 2024-04-29 09:43:04.000000 nucliadb_node_binding-3.0.3.post1216/local_dependencies/nucliadb_node/src/cache/resource_cache.rs
+-rw-r--r--   0     1001      127    11265 2024-04-29 09:43:04.000000 nucliadb_node_binding-3.0.3.post1216/local_dependencies/nucliadb_node/src/cache/writer_cache.rs
+-rw-r--r--   0     1001      127     1771 2024-04-29 09:43:04.000000 nucliadb_node_binding-3.0.3.post1216/local_dependencies/nucliadb_node/src/disk_structure.rs
+-rw-r--r--   0     1001      127     1111 2024-04-29 09:43:04.000000 nucliadb_node_binding-3.0.3.post1216/local_dependencies/nucliadb_node/src/errors.rs
+-rw-r--r--   0     1001      127     2656 2024-04-29 09:43:04.000000 nucliadb_node_binding-3.0.3.post1216/local_dependencies/nucliadb_node/src/grpc/collect_garbage.rs
+-rw-r--r--   0     1001      127    18813 2024-04-29 09:43:04.000000 nucliadb_node_binding-3.0.3.post1216/local_dependencies/nucliadb_node/src/grpc/grpc_reader.rs
+-rw-r--r--   0     1001      127    13710 2024-04-29 09:43:04.000000 nucliadb_node_binding-3.0.3.post1216/local_dependencies/nucliadb_node/src/grpc/grpc_writer.rs
+-rw-r--r--   0     1001      127     3186 2024-04-29 09:43:04.000000 nucliadb_node_binding-3.0.3.post1216/local_dependencies/nucliadb_node/src/grpc/middleware/debug.rs
+-rw-r--r--   0     1001      127     3440 2024-04-29 09:43:04.000000 nucliadb_node_binding-3.0.3.post1216/local_dependencies/nucliadb_node/src/grpc/middleware/metrics.rs
+-rw-r--r--   0     1001      127     1009 2024-04-29 09:43:04.000000 nucliadb_node_binding-3.0.3.post1216/local_dependencies/nucliadb_node/src/grpc/middleware/mod.rs
+-rw-r--r--   0     1001      127     4158 2024-04-29 09:43:04.000000 nucliadb_node_binding-3.0.3.post1216/local_dependencies/nucliadb_node/src/grpc/middleware/telemetry.rs
+-rw-r--r--   0     1001      127     1283 2024-04-29 09:43:04.000000 nucliadb_node_binding-3.0.3.post1216/local_dependencies/nucliadb_node/src/grpc/mod.rs
+-rw-r--r--   0     1001      127     2581 2024-04-29 09:43:04.000000 nucliadb_node_binding-3.0.3.post1216/local_dependencies/nucliadb_node/src/grpc/update.rs
+-rw-r--r--   0     1001      127     1173 2024-04-29 09:43:04.000000 nucliadb_node_binding-3.0.3.post1216/local_dependencies/nucliadb_node/src/http_server/metrics_service.rs
+-rw-r--r--   0     1001      127     1465 2024-04-29 09:43:04.000000 nucliadb_node_binding-3.0.3.post1216/local_dependencies/nucliadb_node/src/http_server/mod.rs
+-rw-r--r--   0     1001      127     1943 2024-04-29 09:43:04.000000 nucliadb_node_binding-3.0.3.post1216/local_dependencies/nucliadb_node/src/http_server/traces_service.rs
+-rw-r--r--   0     1001      127     1504 2024-04-29 09:43:04.000000 nucliadb_node_binding-3.0.3.post1216/local_dependencies/nucliadb_node/src/lib.rs
+-rw-r--r--   0     1001      127     2757 2024-04-29 09:43:04.000000 nucliadb_node_binding-3.0.3.post1216/local_dependencies/nucliadb_node/src/lifecycle.rs
+-rw-r--r--   0     1001      127     1778 2024-04-29 09:43:04.000000 nucliadb_node_binding-3.0.3.post1216/local_dependencies/nucliadb_node/src/merge/global.rs
+-rw-r--r--   0     1001      127     1089 2024-04-29 09:43:04.000000 nucliadb_node_binding-3.0.3.post1216/local_dependencies/nucliadb_node/src/merge/mod.rs
+-rw-r--r--   0     1001      127    13672 2024-04-29 09:43:04.000000 nucliadb_node_binding-3.0.3.post1216/local_dependencies/nucliadb_node/src/merge/scheduler.rs
+-rw-r--r--   0     1001      127     3677 2024-04-29 09:43:04.000000 nucliadb_node_binding-3.0.3.post1216/local_dependencies/nucliadb_node/src/merge/work.rs
+-rw-r--r--   0     1001      127     1935 2024-04-29 09:43:04.000000 nucliadb_node_binding-3.0.3.post1216/local_dependencies/nucliadb_node/src/node_metadata.rs
+-rw-r--r--   0     1001      127     2417 2024-04-29 09:43:04.000000 nucliadb_node_binding-3.0.3.post1216/local_dependencies/nucliadb_node/src/replication/health.rs
+-rw-r--r--   0     1001      127     1070 2024-04-29 09:43:04.000000 nucliadb_node_binding-3.0.3.post1216/local_dependencies/nucliadb_node/src/replication/mod.rs
+-rw-r--r--   0     1001      127    14144 2024-04-29 09:43:04.000000 nucliadb_node_binding-3.0.3.post1216/local_dependencies/nucliadb_node/src/replication/replicator.rs
+-rw-r--r--   0     1001      127    11803 2024-04-29 09:43:04.000000 nucliadb_node_binding-3.0.3.post1216/local_dependencies/nucliadb_node/src/replication/service.rs
+-rw-r--r--   0     1001      127    11615 2024-04-29 09:43:04.000000 nucliadb_node_binding-3.0.3.post1216/local_dependencies/nucliadb_node/src/settings.rs
+-rw-r--r--   0     1001      127     1111 2024-04-29 09:43:04.000000 nucliadb_node_binding-3.0.3.post1216/local_dependencies/nucliadb_node/src/shards/errors.rs
+-rw-r--r--   0     1001      127    11052 2024-04-29 09:43:04.000000 nucliadb_node_binding-3.0.3.post1216/local_dependencies/nucliadb_node/src/shards/metadata.rs
+-rw-r--r--   0     1001      127     1127 2024-04-29 09:43:04.000000 nucliadb_node_binding-3.0.3.post1216/local_dependencies/nucliadb_node/src/shards/mod.rs
+-rw-r--r--   0     1001      127    27129 2024-04-29 09:43:04.000000 nucliadb_node_binding-3.0.3.post1216/local_dependencies/nucliadb_node/src/shards/shard_reader.rs
+-rw-r--r--   0     1001      127    23537 2024-04-29 09:43:04.000000 nucliadb_node_binding-3.0.3.post1216/local_dependencies/nucliadb_node/src/shards/shard_writer.rs
+-rw-r--r--   0     1001      127     1887 2024-04-29 09:43:04.000000 nucliadb_node_binding-3.0.3.post1216/local_dependencies/nucliadb_node/src/shards/versioning.rs
+-rw-r--r--   0     1001      127    10170 2024-04-29 09:43:04.000000 nucliadb_node_binding-3.0.3.post1216/local_dependencies/nucliadb_node/src/telemetry.rs
+-rw-r--r--   0     1001      127     6396 2024-04-29 09:43:04.000000 nucliadb_node_binding-3.0.3.post1216/local_dependencies/nucliadb_node/src/utils.rs
+-rw-r--r--   0     1001      127       42 2024-04-29 09:43:04.000000 nucliadb_node_binding-3.0.3.post1216/local_dependencies/nucliadb_node/test.sh
+-rw-r--r--   0     1001      127     1115 2024-04-29 09:43:04.000000 nucliadb_node_binding-3.0.3.post1216/local_dependencies/nucliadb_node/tests/common/mod.rs
+-rw-r--r--   0     1001      127    12731 2024-04-29 09:43:04.000000 nucliadb_node_binding-3.0.3.post1216/local_dependencies/nucliadb_node/tests/common/node_services.rs
+-rw-r--r--   0     1001      127     7823 2024-04-29 09:43:04.000000 nucliadb_node_binding-3.0.3.post1216/local_dependencies/nucliadb_node/tests/common/resources.rs
+-rw-r--r--   0     1001      127     8173 2024-04-29 09:43:04.000000 nucliadb_node_binding-3.0.3.post1216/local_dependencies/nucliadb_node/tests/test_date_range_search.rs
+-rw-r--r--   0     1001      127     4089 2024-04-29 09:43:04.000000 nucliadb_node_binding-3.0.3.post1216/local_dependencies/nucliadb_node/tests/test_download.rs
+-rw-r--r--   0     1001      127     1684 2024-04-29 09:43:04.000000 nucliadb_node_binding-3.0.3.post1216/local_dependencies/nucliadb_node/tests/test_merge.rs
+-rw-r--r--   0     1001      127     6003 2024-04-29 09:43:04.000000 nucliadb_node_binding-3.0.3.post1216/local_dependencies/nucliadb_node/tests/test_replication.rs
+-rw-r--r--   0     1001      127    22494 2024-04-29 09:43:04.000000 nucliadb_node_binding-3.0.3.post1216/local_dependencies/nucliadb_node/tests/test_search_relations.rs
+-rw-r--r--   0     1001      127     6958 2024-04-29 09:43:04.000000 nucliadb_node_binding-3.0.3.post1216/local_dependencies/nucliadb_node/tests/test_search_sorting.rs
+-rw-r--r--   0     1001      127     7044 2024-04-29 09:43:04.000000 nucliadb_node_binding-3.0.3.post1216/local_dependencies/nucliadb_node/tests/test_security_search.rs
+-rw-r--r--   0     1001      127     6862 2024-04-29 09:43:04.000000 nucliadb_node_binding-3.0.3.post1216/local_dependencies/nucliadb_node/tests/test_shards.rs
+-rw-r--r--   0     1001      127    10698 2024-04-29 09:43:04.000000 nucliadb_node_binding-3.0.3.post1216/local_dependencies/nucliadb_node/tests/test_suggest.rs
+-rw-r--r--   0     1001      127     5438 2024-04-29 09:43:04.000000 nucliadb_node_binding-3.0.3.post1216/local_dependencies/nucliadb_node/tests/test_vector_normalization.rs
+-rw-r--r--   0        0        0      501 1970-01-01 00:00:00.000000 nucliadb_node_binding-3.0.3.post1216/local_dependencies/nucliadb_protos/Cargo.toml
+-rw-r--r--   0     1001      127     2155 2024-04-29 09:43:04.000000 nucliadb_node_binding-3.0.3.post1216/local_dependencies/nucliadb_protos/build.rs
+-rw-r--r--   0     1001      127    26110 2024-04-29 09:43:04.000000 nucliadb_node_binding-3.0.3.post1216/local_dependencies/nucliadb_protos/src/fdbwriter.rs
+-rw-r--r--   0     1001      127        0 2024-04-29 09:43:04.000000 nucliadb_node_binding-3.0.3.post1216/local_dependencies/nucliadb_protos/src/google.protobuf.rs
+-rw-r--r--   0     1001      127     9795 2024-04-29 09:43:04.000000 nucliadb_node_binding-3.0.3.post1216/local_dependencies/nucliadb_protos/src/knowledgebox.rs
+-rw-r--r--   0     1001      127     1256 2024-04-29 09:43:04.000000 nucliadb_node_binding-3.0.3.post1216/local_dependencies/nucliadb_protos/src/lib.rs
+-rw-r--r--   0     1001      127    77311 2024-04-29 09:43:04.000000 nucliadb_node_binding-3.0.3.post1216/local_dependencies/nucliadb_protos/src/nodereader.rs
+-rw-r--r--   0     1001      127    10240 2024-04-29 09:43:04.000000 nucliadb_node_binding-3.0.3.post1216/local_dependencies/nucliadb_protos/src/noderesources.rs
+-rw-r--r--   0     1001      127    43352 2024-04-29 09:43:04.000000 nucliadb_node_binding-3.0.3.post1216/local_dependencies/nucliadb_protos/src/nodewriter.rs
+-rw-r--r--   0     1001      127    19106 2024-04-29 09:43:04.000000 nucliadb_node_binding-3.0.3.post1216/local_dependencies/nucliadb_protos/src/replication.rs
+-rw-r--r--   0     1001      127    33352 2024-04-29 09:43:04.000000 nucliadb_node_binding-3.0.3.post1216/local_dependencies/nucliadb_protos/src/resources.rs
+-rw-r--r--   0     1001      127     5528 2024-04-29 09:43:04.000000 nucliadb_node_binding-3.0.3.post1216/local_dependencies/nucliadb_protos/src/utils.rs
+-rw-r--r--   0        0        0      361 1970-01-01 00:00:00.000000 nucliadb_node_binding-3.0.3.post1216/local_dependencies/nucliadb_procs/Cargo.toml
+-rw-r--r--   0     1001      127     3409 2024-04-29 09:43:04.000000 nucliadb_node_binding-3.0.3.post1216/local_dependencies/nucliadb_procs/src/lib.rs
+-rw-r--r--   0     1001      127     2885 2024-04-29 09:43:04.000000 nucliadb_node_binding-3.0.3.post1216/local_dependencies/nucliadb_procs/src/measure.rs
+-rw-r--r--   0     1001      127     1081 2024-04-29 09:43:04.000000 nucliadb_node_binding-3.0.3.post1216/local_dependencies/nucliadb_procs/tests/dont_compile/actor_defined_twice.rs
+-rw-r--r--   0     1001      127      222 2024-04-29 09:43:04.000000 nucliadb_node_binding-3.0.3.post1216/local_dependencies/nucliadb_procs/tests/dont_compile/actor_defined_twice.stderr
+-rw-r--r--   0     1001      127     1038 2024-04-29 09:43:04.000000 nucliadb_node_binding-3.0.3.post1216/local_dependencies/nucliadb_procs/tests/dont_compile/actor_not_defined.rs
+-rw-r--r--   0     1001      127      327 2024-04-29 09:43:04.000000 nucliadb_node_binding-3.0.3.post1216/local_dependencies/nucliadb_procs/tests/dont_compile/actor_not_defined.stderr
+-rw-r--r--   0     1001      127     1086 2024-04-29 09:43:04.000000 nucliadb_node_binding-3.0.3.post1216/local_dependencies/nucliadb_procs/tests/dont_compile/metric_defined_twice.rs
+-rw-r--r--   0     1001      127      249 2024-04-29 09:43:04.000000 nucliadb_node_binding-3.0.3.post1216/local_dependencies/nucliadb_procs/tests/dont_compile/metric_defined_twice.stderr
+-rw-r--r--   0     1001      127     1046 2024-04-29 09:43:04.000000 nucliadb_node_binding-3.0.3.post1216/local_dependencies/nucliadb_procs/tests/dont_compile/wrong_actor.rs
+-rw-r--r--   0     1001      127     1303 2024-04-29 09:43:04.000000 nucliadb_node_binding-3.0.3.post1216/local_dependencies/nucliadb_procs/tests/dont_compile/wrong_actor.stderr
+-rw-r--r--   0     1001      127     1408 2024-04-29 09:43:04.000000 nucliadb_node_binding-3.0.3.post1216/local_dependencies/nucliadb_procs/tests/test_measure.rs
+-rw-r--r--   0        0        0      629 1970-01-01 00:00:00.000000 nucliadb_node_binding-3.0.3.post1216/local_dependencies/nucliadb_paragraphs2/Cargo.toml
+-rw-r--r--   0     1001      127     7796 2024-04-29 09:43:04.000000 nucliadb_node_binding-3.0.3.post1216/local_dependencies/nucliadb_paragraphs2/src/fuzzy_query.rs
+-rw-r--r--   0     1001      127     1009 2024-04-29 09:43:04.000000 nucliadb_node_binding-3.0.3.post1216/local_dependencies/nucliadb_paragraphs2/src/lib.rs
+-rw-r--r--   0     1001      127     2780 2024-04-29 09:43:04.000000 nucliadb_node_binding-3.0.3.post1216/local_dependencies/nucliadb_paragraphs2/src/query_io.rs
+-rw-r--r--   0     1001      127    42940 2024-04-29 09:43:04.000000 nucliadb_node_binding-3.0.3.post1216/local_dependencies/nucliadb_paragraphs2/src/reader.rs
+-rw-r--r--   0     1001      127     4808 2024-04-29 09:43:04.000000 nucliadb_node_binding-3.0.3.post1216/local_dependencies/nucliadb_paragraphs2/src/schema.rs
+-rw-r--r--   0     1001      127    22494 2024-04-29 09:43:04.000000 nucliadb_node_binding-3.0.3.post1216/local_dependencies/nucliadb_paragraphs2/src/search_query.rs
+-rw-r--r--   0     1001      127    11391 2024-04-29 09:43:04.000000 nucliadb_node_binding-3.0.3.post1216/local_dependencies/nucliadb_paragraphs2/src/search_response.rs
+-rw-r--r--   0     1001      127     4090 2024-04-29 09:43:04.000000 nucliadb_node_binding-3.0.3.post1216/local_dependencies/nucliadb_paragraphs2/src/stop_words.rs
+-rw-r--r--   0     1001      127    17965 2024-04-29 09:43:04.000000 nucliadb_node_binding-3.0.3.post1216/local_dependencies/nucliadb_paragraphs2/src/writer.rs
+-rw-r--r--   0     1001      127       88 2024-04-29 09:43:04.000000 nucliadb_node_binding-3.0.3.post1216/local_dependencies/nucliadb_paragraphs2/stop_words/README.md
+-rw-r--r--   0     1001      127    19791 2024-04-29 09:43:04.000000 nucliadb_node_binding-3.0.3.post1216/local_dependencies/nucliadb_paragraphs2/stop_words/ar.json
+-rw-r--r--   0     1001      127     1923 2024-04-29 09:43:04.000000 nucliadb_node_binding-3.0.3.post1216/local_dependencies/nucliadb_paragraphs2/stop_words/az.json
+-rw-r--r--   0     1001      127    11684 2024-04-29 09:43:04.000000 nucliadb_node_binding-3.0.3.post1216/local_dependencies/nucliadb_paragraphs2/stop_words/bn.json
+-rw-r--r--   0     1001      127     2513 2024-04-29 09:43:04.000000 nucliadb_node_binding-3.0.3.post1216/local_dependencies/nucliadb_paragraphs2/stop_words/ca.json
+-rw-r--r--   0     1001      127    12802 2024-04-29 09:43:04.000000 nucliadb_node_binding-3.0.3.post1216/local_dependencies/nucliadb_paragraphs2/stop_words/ch.json
+-rw-r--r--   0     1001      127      730 2024-04-29 09:43:04.000000 nucliadb_node_binding-3.0.3.post1216/local_dependencies/nucliadb_paragraphs2/stop_words/da.json
+-rw-r--r--   0     1001      127     2090 2024-04-29 09:43:04.000000 nucliadb_node_binding-3.0.3.post1216/local_dependencies/nucliadb_paragraphs2/stop_words/de.json
+-rw-r--r--   0     1001      127     6284 2024-04-29 09:43:04.000000 nucliadb_node_binding-3.0.3.post1216/local_dependencies/nucliadb_paragraphs2/stop_words/el.json
+-rw-r--r--   0     1001      127     1473 2024-04-29 09:43:04.000000 nucliadb_node_binding-3.0.3.post1216/local_dependencies/nucliadb_paragraphs2/stop_words/en.json
+-rw-r--r--   0     1001      127     3451 2024-04-29 09:43:04.000000 nucliadb_node_binding-3.0.3.post1216/local_dependencies/nucliadb_paragraphs2/stop_words/es.json
+-rw-r--r--   0     1001      127     3182 2024-04-29 09:43:04.000000 nucliadb_node_binding-3.0.3.post1216/local_dependencies/nucliadb_paragraphs2/stop_words/eu.json
+-rw-r--r--   0     1001      127     2126 2024-04-29 09:43:04.000000 nucliadb_node_binding-3.0.3.post1216/local_dependencies/nucliadb_paragraphs2/stop_words/extract.py
+-rw-r--r--   0     1001      127     2748 2024-04-29 09:43:04.000000 nucliadb_node_binding-3.0.3.post1216/local_dependencies/nucliadb_paragraphs2/stop_words/fi.json
+-rw-r--r--   0     1001      127     1388 2024-04-29 09:43:04.000000 nucliadb_node_binding-3.0.3.post1216/local_dependencies/nucliadb_paragraphs2/stop_words/fr.json
+-rw-r--r--   0     1001      127     5716 2024-04-29 09:43:04.000000 nucliadb_node_binding-3.0.3.post1216/local_dependencies/nucliadb_paragraphs2/stop_words/he.json
+-rw-r--r--   0     1001      127     2108 2024-04-29 09:43:04.000000 nucliadb_node_binding-3.0.3.post1216/local_dependencies/nucliadb_paragraphs2/stop_words/hu.json
+-rw-r--r--   0     1001      127     8721 2024-04-29 09:43:04.000000 nucliadb_node_binding-3.0.3.post1216/local_dependencies/nucliadb_paragraphs2/stop_words/id.json
+-rw-r--r--   0     1001      127     2535 2024-04-29 09:43:04.000000 nucliadb_node_binding-3.0.3.post1216/local_dependencies/nucliadb_paragraphs2/stop_words/it.json
+-rw-r--r--   0     1001      127    11737 2024-04-29 09:43:04.000000 nucliadb_node_binding-3.0.3.post1216/local_dependencies/nucliadb_paragraphs2/stop_words/kk.json
+-rw-r--r--   0     1001      127     7730 2024-04-29 09:43:04.000000 nucliadb_node_binding-3.0.3.post1216/local_dependencies/nucliadb_paragraphs2/stop_words/ne.json
+-rw-r--r--   0     1001      127      756 2024-04-29 09:43:04.000000 nucliadb_node_binding-3.0.3.post1216/local_dependencies/nucliadb_paragraphs2/stop_words/nl.json
+-rw-r--r--   0     1001      127     1447 2024-04-29 09:43:04.000000 nucliadb_node_binding-3.0.3.post1216/local_dependencies/nucliadb_paragraphs2/stop_words/no.json
+-rw-r--r--   0     1001      127     2055 2024-04-29 09:43:04.000000 nucliadb_node_binding-3.0.3.post1216/local_dependencies/nucliadb_paragraphs2/stop_words/pt.json
+-rw-r--r--   0     1001      127     3327 2024-04-29 09:43:04.000000 nucliadb_node_binding-3.0.3.post1216/local_dependencies/nucliadb_paragraphs2/stop_words/ro.json
+-rw-r--r--   0     1001      127     3856 2024-04-29 09:43:04.000000 nucliadb_node_binding-3.0.3.post1216/local_dependencies/nucliadb_paragraphs2/stop_words/ru.json
+-rw-r--r--   0     1001      127    23032 2024-04-29 09:43:04.000000 nucliadb_node_binding-3.0.3.post1216/local_dependencies/nucliadb_paragraphs2/stop_words/sl.json
+-rw-r--r--   0     1001      127      993 2024-04-29 09:43:04.000000 nucliadb_node_binding-3.0.3.post1216/local_dependencies/nucliadb_paragraphs2/stop_words/sv.json
+-rw-r--r--   0     1001      127     5424 2024-04-29 09:43:04.000000 nucliadb_node_binding-3.0.3.post1216/local_dependencies/nucliadb_paragraphs2/stop_words/tg.json
+-rw-r--r--   0     1001      127      491 2024-04-29 09:43:04.000000 nucliadb_node_binding-3.0.3.post1216/local_dependencies/nucliadb_paragraphs2/stop_words/tr.json
+-rw-r--r--   0        0        0      629 1970-01-01 00:00:00.000000 nucliadb_node_binding-3.0.3.post1216/local_dependencies/nucliadb_paragraphs3/Cargo.toml
+-rw-r--r--   0     1001      127     7796 2024-04-29 09:43:04.000000 nucliadb_node_binding-3.0.3.post1216/local_dependencies/nucliadb_paragraphs3/src/fuzzy_query.rs
+-rw-r--r--   0     1001      127     1024 2024-04-29 09:43:04.000000 nucliadb_node_binding-3.0.3.post1216/local_dependencies/nucliadb_paragraphs3/src/lib.rs
+-rw-r--r--   0     1001      127     2780 2024-04-29 09:43:04.000000 nucliadb_node_binding-3.0.3.post1216/local_dependencies/nucliadb_paragraphs3/src/query_io.rs
+-rw-r--r--   0     1001      127    42885 2024-04-29 09:43:04.000000 nucliadb_node_binding-3.0.3.post1216/local_dependencies/nucliadb_paragraphs3/src/reader.rs
+-rw-r--r--   0     1001      127     4407 2024-04-29 09:43:04.000000 nucliadb_node_binding-3.0.3.post1216/local_dependencies/nucliadb_paragraphs3/src/schema.rs
+-rw-r--r--   0     1001      127    21349 2024-04-29 09:43:04.000000 nucliadb_node_binding-3.0.3.post1216/local_dependencies/nucliadb_paragraphs3/src/search_query.rs
+-rw-r--r--   0     1001      127    11723 2024-04-29 09:43:04.000000 nucliadb_node_binding-3.0.3.post1216/local_dependencies/nucliadb_paragraphs3/src/search_response.rs
+-rw-r--r--   0     1001      127     2846 2024-04-29 09:43:04.000000 nucliadb_node_binding-3.0.3.post1216/local_dependencies/nucliadb_paragraphs3/src/set_query.rs
+-rw-r--r--   0     1001      127     4090 2024-04-29 09:43:04.000000 nucliadb_node_binding-3.0.3.post1216/local_dependencies/nucliadb_paragraphs3/src/stop_words.rs
+-rw-r--r--   0     1001      127    17057 2024-04-29 09:43:04.000000 nucliadb_node_binding-3.0.3.post1216/local_dependencies/nucliadb_paragraphs3/src/writer.rs
+-rw-r--r--   0     1001      127       88 2024-04-29 09:43:04.000000 nucliadb_node_binding-3.0.3.post1216/local_dependencies/nucliadb_paragraphs3/stop_words/README.md
+-rw-r--r--   0     1001      127    19791 2024-04-29 09:43:04.000000 nucliadb_node_binding-3.0.3.post1216/local_dependencies/nucliadb_paragraphs3/stop_words/ar.json
+-rw-r--r--   0     1001      127     1923 2024-04-29 09:43:04.000000 nucliadb_node_binding-3.0.3.post1216/local_dependencies/nucliadb_paragraphs3/stop_words/az.json
+-rw-r--r--   0     1001      127    11684 2024-04-29 09:43:04.000000 nucliadb_node_binding-3.0.3.post1216/local_dependencies/nucliadb_paragraphs3/stop_words/bn.json
+-rw-r--r--   0     1001      127     2513 2024-04-29 09:43:04.000000 nucliadb_node_binding-3.0.3.post1216/local_dependencies/nucliadb_paragraphs3/stop_words/ca.json
+-rw-r--r--   0     1001      127    12802 2024-04-29 09:43:04.000000 nucliadb_node_binding-3.0.3.post1216/local_dependencies/nucliadb_paragraphs3/stop_words/ch.json
+-rw-r--r--   0     1001      127      730 2024-04-29 09:43:04.000000 nucliadb_node_binding-3.0.3.post1216/local_dependencies/nucliadb_paragraphs3/stop_words/da.json
+-rw-r--r--   0     1001      127     2090 2024-04-29 09:43:04.000000 nucliadb_node_binding-3.0.3.post1216/local_dependencies/nucliadb_paragraphs3/stop_words/de.json
+-rw-r--r--   0     1001      127     6284 2024-04-29 09:43:04.000000 nucliadb_node_binding-3.0.3.post1216/local_dependencies/nucliadb_paragraphs3/stop_words/el.json
+-rw-r--r--   0     1001      127     1473 2024-04-29 09:43:04.000000 nucliadb_node_binding-3.0.3.post1216/local_dependencies/nucliadb_paragraphs3/stop_words/en.json
+-rw-r--r--   0     1001      127     3451 2024-04-29 09:43:04.000000 nucliadb_node_binding-3.0.3.post1216/local_dependencies/nucliadb_paragraphs3/stop_words/es.json
+-rw-r--r--   0     1001      127     3182 2024-04-29 09:43:04.000000 nucliadb_node_binding-3.0.3.post1216/local_dependencies/nucliadb_paragraphs3/stop_words/eu.json
+-rw-r--r--   0     1001      127     2126 2024-04-29 09:43:04.000000 nucliadb_node_binding-3.0.3.post1216/local_dependencies/nucliadb_paragraphs3/stop_words/extract.py
+-rw-r--r--   0     1001      127     2748 2024-04-29 09:43:04.000000 nucliadb_node_binding-3.0.3.post1216/local_dependencies/nucliadb_paragraphs3/stop_words/fi.json
+-rw-r--r--   0     1001      127     1388 2024-04-29 09:43:04.000000 nucliadb_node_binding-3.0.3.post1216/local_dependencies/nucliadb_paragraphs3/stop_words/fr.json
+-rw-r--r--   0     1001      127     5716 2024-04-29 09:43:04.000000 nucliadb_node_binding-3.0.3.post1216/local_dependencies/nucliadb_paragraphs3/stop_words/he.json
+-rw-r--r--   0     1001      127     2108 2024-04-29 09:43:04.000000 nucliadb_node_binding-3.0.3.post1216/local_dependencies/nucliadb_paragraphs3/stop_words/hu.json
+-rw-r--r--   0     1001      127     8721 2024-04-29 09:43:04.000000 nucliadb_node_binding-3.0.3.post1216/local_dependencies/nucliadb_paragraphs3/stop_words/id.json
+-rw-r--r--   0     1001      127     2535 2024-04-29 09:43:04.000000 nucliadb_node_binding-3.0.3.post1216/local_dependencies/nucliadb_paragraphs3/stop_words/it.json
+-rw-r--r--   0     1001      127    11737 2024-04-29 09:43:04.000000 nucliadb_node_binding-3.0.3.post1216/local_dependencies/nucliadb_paragraphs3/stop_words/kk.json
+-rw-r--r--   0     1001      127     7730 2024-04-29 09:43:04.000000 nucliadb_node_binding-3.0.3.post1216/local_dependencies/nucliadb_paragraphs3/stop_words/ne.json
+-rw-r--r--   0     1001      127      756 2024-04-29 09:43:04.000000 nucliadb_node_binding-3.0.3.post1216/local_dependencies/nucliadb_paragraphs3/stop_words/nl.json
+-rw-r--r--   0     1001      127     1447 2024-04-29 09:43:04.000000 nucliadb_node_binding-3.0.3.post1216/local_dependencies/nucliadb_paragraphs3/stop_words/no.json
+-rw-r--r--   0     1001      127     2055 2024-04-29 09:43:04.000000 nucliadb_node_binding-3.0.3.post1216/local_dependencies/nucliadb_paragraphs3/stop_words/pt.json
+-rw-r--r--   0     1001      127     3327 2024-04-29 09:43:04.000000 nucliadb_node_binding-3.0.3.post1216/local_dependencies/nucliadb_paragraphs3/stop_words/ro.json
+-rw-r--r--   0     1001      127     3856 2024-04-29 09:43:04.000000 nucliadb_node_binding-3.0.3.post1216/local_dependencies/nucliadb_paragraphs3/stop_words/ru.json
+-rw-r--r--   0     1001      127    23032 2024-04-29 09:43:04.000000 nucliadb_node_binding-3.0.3.post1216/local_dependencies/nucliadb_paragraphs3/stop_words/sl.json
+-rw-r--r--   0     1001      127      993 2024-04-29 09:43:04.000000 nucliadb_node_binding-3.0.3.post1216/local_dependencies/nucliadb_paragraphs3/stop_words/sv.json
+-rw-r--r--   0     1001      127     5424 2024-04-29 09:43:04.000000 nucliadb_node_binding-3.0.3.post1216/local_dependencies/nucliadb_paragraphs3/stop_words/tg.json
+-rw-r--r--   0     1001      127      491 2024-04-29 09:43:04.000000 nucliadb_node_binding-3.0.3.post1216/local_dependencies/nucliadb_paragraphs3/stop_words/tr.json
+-rw-r--r--   0        0        0      399 1970-01-01 00:00:00.000000 nucliadb_node_binding-3.0.3.post1216/local_dependencies/nucliadb_texts2/Cargo.toml
+-rw-r--r--   0     1001      127      931 2024-04-29 09:43:04.000000 nucliadb_node_binding-3.0.3.post1216/local_dependencies/nucliadb_texts2/src/lib.rs
+-rw-r--r--   0     1001      127     2755 2024-04-29 09:43:04.000000 nucliadb_node_binding-3.0.3.post1216/local_dependencies/nucliadb_texts2/src/query_io.rs
+-rw-r--r--   0     1001      127    22721 2024-04-29 09:43:04.000000 nucliadb_node_binding-3.0.3.post1216/local_dependencies/nucliadb_texts2/src/reader.rs
+-rw-r--r--   0     1001      127     3105 2024-04-29 09:43:04.000000 nucliadb_node_binding-3.0.3.post1216/local_dependencies/nucliadb_texts2/src/schema.rs
+-rw-r--r--   0     1001      127     8682 2024-04-29 09:43:04.000000 nucliadb_node_binding-3.0.3.post1216/local_dependencies/nucliadb_texts2/src/search_query.rs
+-rw-r--r--   0     1001      127    10109 2024-04-29 09:43:04.000000 nucliadb_node_binding-3.0.3.post1216/local_dependencies/nucliadb_texts2/src/writer.rs
+-rw-r--r--   0     1001      127     3396 2024-04-29 09:43:04.000000 nucliadb_node_binding-3.0.3.post1216/local_dependencies/nucliadb_texts2/tests/common/mod.rs
+-rw-r--r--   0     1001      127     2068 2024-04-29 09:43:04.000000 nucliadb_node_binding-3.0.3.post1216/local_dependencies/nucliadb_texts2/tests/test_reader.rs
+-rw-r--r--   0     1001      127     9567 2024-04-29 09:43:04.000000 nucliadb_node_binding-3.0.3.post1216/local_dependencies/nucliadb_texts2/tests/test_search.rs
+-rw-r--r--   0     1001      127     1249 2024-04-29 09:43:04.000000 nucliadb_node_binding-3.0.3.post1216/local_dependencies/nucliadb_texts2/tests/test_streaming.rs
+-rw-r--r--   0     1001      127     3469 2024-04-29 09:43:04.000000 nucliadb_node_binding-3.0.3.post1216/local_dependencies/nucliadb_texts2/tests/test_writer.rs
+-rw-r--r--   0        0        0      742 1970-01-01 00:00:00.000000 nucliadb_node_binding-3.0.3.post1216/local_dependencies/nucliadb_vectors/Cargo.toml
+-rw-r--r--   0     1001      127       69 2024-04-29 09:43:04.000000 nucliadb_node_binding-3.0.3.post1216/local_dependencies/nucliadb_vectors/README.md
+-rw-r--r--   0     1001      127       43 2024-04-29 09:43:04.000000 nucliadb_node_binding-3.0.3.post1216/local_dependencies/nucliadb_vectors/docs/README.md
+-rw-r--r--   0     1001      127    25718 2024-04-29 09:43:04.000000 nucliadb_node_binding-3.0.3.post1216/local_dependencies/nucliadb_vectors/docs/labels.drawio.svg
+-rw-r--r--   0     1001      127    12340 2024-04-29 09:43:04.000000 nucliadb_node_binding-3.0.3.post1216/local_dependencies/nucliadb_vectors/src/data_point/disk_hnsw.rs
+-rw-r--r--   0     1001      127    24470 2024-04-29 09:43:04.000000 nucliadb_node_binding-3.0.3.post1216/local_dependencies/nucliadb_vectors/src/data_point/mod.rs
+-rw-r--r--   0     1001      127    11214 2024-04-29 09:43:04.000000 nucliadb_node_binding-3.0.3.post1216/local_dependencies/nucliadb_vectors/src/data_point/node.rs
+-rw-r--r--   0     1001      127    14639 2024-04-29 09:43:04.000000 nucliadb_node_binding-3.0.3.post1216/local_dependencies/nucliadb_vectors/src/data_point/ops_hnsw.rs
+-rw-r--r--   0     1001      127     1642 2024-04-29 09:43:04.000000 nucliadb_node_binding-3.0.3.post1216/local_dependencies/nucliadb_vectors/src/data_point/params.rs
+-rw-r--r--   0     1001      127     3952 2024-04-29 09:43:04.000000 nucliadb_node_binding-3.0.3.post1216/local_dependencies/nucliadb_vectors/src/data_point/ram_hnsw.rs
+-rw-r--r--   0     1001      127    14175 2024-04-29 09:43:04.000000 nucliadb_node_binding-3.0.3.post1216/local_dependencies/nucliadb_vectors/src/data_point/tests.rs
+-rw-r--r--   0     1001      127     5798 2024-04-29 09:43:04.000000 nucliadb_node_binding-3.0.3.post1216/local_dependencies/nucliadb_vectors/src/data_point_provider/garbage_collector.rs
+-rw-r--r--   0     1001      127     2777 2024-04-29 09:43:04.000000 nucliadb_node_binding-3.0.3.post1216/local_dependencies/nucliadb_vectors/src/data_point_provider/mod.rs
+-rw-r--r--   0     1001      127    10613 2024-04-29 09:43:04.000000 nucliadb_node_binding-3.0.3.post1216/local_dependencies/nucliadb_vectors/src/data_point_provider/reader.rs
+-rw-r--r--   0     1001      127     2304 2024-04-29 09:43:04.000000 nucliadb_node_binding-3.0.3.post1216/local_dependencies/nucliadb_vectors/src/data_point_provider/replication.rs
+-rw-r--r--   0     1001      127     5288 2024-04-29 09:43:04.000000 nucliadb_node_binding-3.0.3.post1216/local_dependencies/nucliadb_vectors/src/data_point_provider/state.rs
+-rw-r--r--   0     1001      127    20587 2024-04-29 09:43:04.000000 nucliadb_node_binding-3.0.3.post1216/local_dependencies/nucliadb_vectors/src/data_point_provider/writer.rs
+-rw-r--r--   0     1001      127    23710 2024-04-29 09:43:04.000000 nucliadb_node_binding-3.0.3.post1216/local_dependencies/nucliadb_vectors/src/data_types/data_store.rs
+-rw-r--r--   0     1001      127     6916 2024-04-29 09:43:04.000000 nucliadb_node_binding-3.0.3.post1216/local_dependencies/nucliadb_vectors/src/data_types/dtrie_ram.rs
+-rw-r--r--   0     1001      127     1959 2024-04-29 09:43:04.000000 nucliadb_node_binding-3.0.3.post1216/local_dependencies/nucliadb_vectors/src/data_types/mod.rs
+-rw-r--r--   0     1001      127     6143 2024-04-29 09:43:04.000000 nucliadb_node_binding-3.0.3.post1216/local_dependencies/nucliadb_vectors/src/data_types/trie.rs
+-rw-r--r--   0     1001      127     2904 2024-04-29 09:43:04.000000 nucliadb_node_binding-3.0.3.post1216/local_dependencies/nucliadb_vectors/src/data_types/trie_ram.rs
+-rw-r--r--   0     1001      127     4433 2024-04-29 09:43:04.000000 nucliadb_node_binding-3.0.3.post1216/local_dependencies/nucliadb_vectors/src/data_types/vector.rs
+-rw-r--r--   0     1001      127    10472 2024-04-29 09:43:04.000000 nucliadb_node_binding-3.0.3.post1216/local_dependencies/nucliadb_vectors/src/formula/mod.rs
+-rw-r--r--   0     1001      127     2165 2024-04-29 09:43:04.000000 nucliadb_node_binding-3.0.3.post1216/local_dependencies/nucliadb_vectors/src/lib.rs
+-rw-r--r--   0     1001      127     1278 2024-04-29 09:43:04.000000 nucliadb_node_binding-3.0.3.post1216/local_dependencies/nucliadb_vectors/src/service/mod.rs
+-rw-r--r--   0     1001      127     1897 2024-04-29 09:43:04.000000 nucliadb_node_binding-3.0.3.post1216/local_dependencies/nucliadb_vectors/src/service/query_io.rs
+-rw-r--r--   0     1001      127    17192 2024-04-29 09:43:04.000000 nucliadb_node_binding-3.0.3.post1216/local_dependencies/nucliadb_vectors/src/service/reader.rs
+-rw-r--r--   0     1001      127    15294 2024-04-29 09:43:04.000000 nucliadb_node_binding-3.0.3.post1216/local_dependencies/nucliadb_vectors/src/service/writer.rs
+-rw-r--r--   0     1001      127     1668 2024-04-29 09:43:04.000000 nucliadb_node_binding-3.0.3.post1216/local_dependencies/nucliadb_vectors/src/utils.rs
+-rw-r--r--   0     1001      127     2884 2024-04-29 09:43:04.000000 nucliadb_node_binding-3.0.3.post1216/local_dependencies/nucliadb_vectors/tests/test_merge.rs
+-rw-r--r--   0        0        0      708 1970-01-01 00:00:00.000000 nucliadb_node_binding-3.0.3.post1216/local_dependencies/nucliadb_relations2/Cargo.toml
+-rw-r--r--   0     1001      127     3593 2024-04-29 09:43:04.000000 nucliadb_node_binding-3.0.3.post1216/local_dependencies/nucliadb_relations2/src/io_maps.rs
+-rw-r--r--   0     1001      127      916 2024-04-29 09:43:04.000000 nucliadb_node_binding-3.0.3.post1216/local_dependencies/nucliadb_relations2/src/lib.rs
+-rw-r--r--   0     1001      127    17039 2024-04-29 09:43:04.000000 nucliadb_node_binding-3.0.3.post1216/local_dependencies/nucliadb_relations2/src/reader.rs
+-rw-r--r--   0     1001      127     7123 2024-04-29 09:43:04.000000 nucliadb_node_binding-3.0.3.post1216/local_dependencies/nucliadb_relations2/src/schema.rs
+-rw-r--r--   0     1001      127     8007 2024-04-29 09:43:04.000000 nucliadb_node_binding-3.0.3.post1216/local_dependencies/nucliadb_relations2/src/writer.rs
+-rw-r--r--   0     1001      127     1802 2024-04-29 09:43:04.000000 nucliadb_node_binding-3.0.3.post1216/local_dependencies/nucliadb_relations2/tests/common/mod.rs
+-rw-r--r--   0     1001      127     9445 2024-04-29 09:43:04.000000 nucliadb_node_binding-3.0.3.post1216/local_dependencies/nucliadb_relations2/tests/test_reader.rs
+-rw-r--r--   0     1001      127     3297 2024-04-29 09:43:04.000000 nucliadb_node_binding-3.0.3.post1216/local_dependencies/nucliadb_relations2/tests/test_writer.rs
+-rw-r--r--   0        0        0      931 1970-01-01 00:00:00.000000 nucliadb_node_binding-3.0.3.post1216/local_dependencies/nucliadb_core/Cargo.toml
+-rw-r--r--   0     1001      127     5872 2024-04-29 09:43:04.000000 nucliadb_node_binding-3.0.3.post1216/local_dependencies/nucliadb_core/src/fs_state.rs
+-rw-r--r--   0     1001      127     2969 2024-04-29 09:43:04.000000 nucliadb_node_binding-3.0.3.post1216/local_dependencies/nucliadb_core/src/lib.rs
+-rw-r--r--   0     1001      127     2295 2024-04-29 09:43:04.000000 nucliadb_node_binding-3.0.3.post1216/local_dependencies/nucliadb_core/src/merge.rs
+-rw-r--r--   0     1001      127      906 2024-04-29 09:43:04.000000 nucliadb_node_binding-3.0.3.post1216/local_dependencies/nucliadb_core/src/metrics/meters/mod.rs
+-rw-r--r--   0     1001      127     4869 2024-04-29 09:43:04.000000 nucliadb_node_binding-3.0.3.post1216/local_dependencies/nucliadb_core/src/metrics/meters/prometheus.rs
+-rw-r--r--   0     1001      127     1702 2024-04-29 09:43:04.000000 nucliadb_node_binding-3.0.3.post1216/local_dependencies/nucliadb_core/src/metrics/metric/grpc_ops.rs
+-rw-r--r--   0     1001      127     1442 2024-04-29 09:43:04.000000 nucliadb_node_binding-3.0.3.post1216/local_dependencies/nucliadb_core/src/metrics/metric/mod.rs
+-rw-r--r--   0     1001      127     1950 2024-04-29 09:43:04.000000 nucliadb_node_binding-3.0.3.post1216/local_dependencies/nucliadb_core/src/metrics/metric/replication.rs
+-rw-r--r--   0     1001      127     2626 2024-04-29 09:43:04.000000 nucliadb_node_binding-3.0.3.post1216/local_dependencies/nucliadb_core/src/metrics/metric/request_time.rs
+-rw-r--r--   0     1001      127     1644 2024-04-29 09:43:04.000000 nucliadb_node_binding-3.0.3.post1216/local_dependencies/nucliadb_core/src/metrics/metric/shard_cache.rs
+-rw-r--r--   0     1001      127    21641 2024-04-29 09:43:04.000000 nucliadb_node_binding-3.0.3.post1216/local_dependencies/nucliadb_core/src/metrics/metric/tokio_runtime.rs
+-rw-r--r--   0     1001      127    16736 2024-04-29 09:43:04.000000 nucliadb_node_binding-3.0.3.post1216/local_dependencies/nucliadb_core/src/metrics/metric/tokio_tasks.rs
+-rw-r--r--   0     1001      127     3415 2024-04-29 09:43:04.000000 nucliadb_node_binding-3.0.3.post1216/local_dependencies/nucliadb_core/src/metrics/metric/vectors.rs
+-rw-r--r--   0     1001      127     1324 2024-04-29 09:43:04.000000 nucliadb_node_binding-3.0.3.post1216/local_dependencies/nucliadb_core/src/metrics/mod.rs
+-rw-r--r--   0     1001      127     3074 2024-04-29 09:43:04.000000 nucliadb_node_binding-3.0.3.post1216/local_dependencies/nucliadb_core/src/metrics/task_monitor.rs
+-rw-r--r--   0     1001      127     3920 2024-04-29 09:43:04.000000 nucliadb_node_binding-3.0.3.post1216/local_dependencies/nucliadb_core/src/metrics/tests.rs
+-rw-r--r--   0     1001      127     2990 2024-04-29 09:43:04.000000 nucliadb_node_binding-3.0.3.post1216/local_dependencies/nucliadb_core/src/paragraphs.rs
+-rw-r--r--   0     1001      127    17305 2024-04-29 09:43:04.000000 nucliadb_node_binding-3.0.3.post1216/local_dependencies/nucliadb_core/src/query_language/mod.rs
+-rw-r--r--   0     1001      127    15367 2024-04-29 09:43:04.000000 nucliadb_node_binding-3.0.3.post1216/local_dependencies/nucliadb_core/src/query_planner.rs
+-rw-r--r--   0     1001      127     2069 2024-04-29 09:43:04.000000 nucliadb_node_binding-3.0.3.post1216/local_dependencies/nucliadb_core/src/relations.rs
+-rw-r--r--   0     1001      127     8250 2024-04-29 09:43:04.000000 nucliadb_node_binding-3.0.3.post1216/local_dependencies/nucliadb_core/src/tantivy_replica.rs
+-rw-r--r--   0     1001      127     2603 2024-04-29 09:43:04.000000 nucliadb_node_binding-3.0.3.post1216/local_dependencies/nucliadb_core/src/texts.rs
+-rw-r--r--   0     1001      127     3559 2024-04-29 09:43:04.000000 nucliadb_node_binding-3.0.3.post1216/local_dependencies/nucliadb_core/src/vectors.rs
+-rw-r--r--   0        0        0      943 1970-01-01 00:00:00.000000 nucliadb_node_binding-3.0.3.post1216/Cargo.toml
+-rw-r--r--   0     1001      127     1553 2024-04-29 09:43:04.000000 nucliadb_node_binding-3.0.3.post1216/CHANGELOG.md
+-rw-r--r--   0     1001      127      895 2024-04-29 09:43:04.000000 nucliadb_node_binding-3.0.3.post1216/Makefile
+-rw-r--r--   0     1001      127       52 2024-04-29 09:43:04.000000 nucliadb_node_binding-3.0.3.post1216/README.md
+-rwxr-xr-x   0     1001      127      978 2024-04-29 09:43:04.000000 nucliadb_node_binding-3.0.3.post1216/cov.sh
+-rw-r--r--   0     1001      127     1309 2024-04-29 09:43:04.000000 nucliadb_node_binding-3.0.3.post1216/pyproject.toml
+-rw-r--r--   0     1001      127     2195 2024-04-29 09:43:04.000000 nucliadb_node_binding-3.0.3.post1216/src/collect_garbage.rs
+-rw-r--r--   0     1001      127     1212 2024-04-29 09:43:04.000000 nucliadb_node_binding-3.0.3.post1216/src/errors.rs
+-rw-r--r--   0     1001      127     2337 2024-04-29 09:43:04.000000 nucliadb_node_binding-3.0.3.post1216/src/lib.rs
+-rw-r--r--   0     1001      127     9405 2024-04-29 09:43:04.000000 nucliadb_node_binding-3.0.3.post1216/src/reader.rs
+-rw-r--r--   0     1001      127     2154 2024-04-29 09:43:04.000000 nucliadb_node_binding-3.0.3.post1216/src/update.rs
+-rw-r--r--   0     1001      127     9150 2024-04-29 09:43:04.000000 nucliadb_node_binding-3.0.3.post1216/src/writer.rs
+-rw-r--r--   0     1001      127      835 2024-04-29 09:43:04.000000 nucliadb_node_binding-3.0.3.post1216/tests/__init__.py
+-rw-r--r--   0     1001      127      892 2024-04-29 09:43:04.000000 nucliadb_node_binding-3.0.3.post1216/tests/conftest.py
+-rw-r--r--   0     1001      127     3903 2024-04-29 09:43:04.000000 nucliadb_node_binding-3.0.3.post1216/tests/integration/test_indexing.py
+-rw-r--r--   0        0        0      401 1970-01-01 00:00:00.000000 nucliadb_node_binding-3.0.3.post1216/PKG-INFO
```

### Comparing `nucliadb_node_binding-3.0.3.post1215/local_dependencies/nucliadb_texts2/src/lib.rs` & `nucliadb_node_binding-3.0.3.post1216/local_dependencies/nucliadb_texts2/src/lib.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.0.3.post1215/local_dependencies/nucliadb_texts2/src/query_io.rs` & `nucliadb_node_binding-3.0.3.post1216/local_dependencies/nucliadb_texts2/src/query_io.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.0.3.post1215/local_dependencies/nucliadb_texts2/src/reader.rs` & `nucliadb_node_binding-3.0.3.post1216/local_dependencies/nucliadb_texts2/src/reader.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.0.3.post1215/local_dependencies/nucliadb_texts2/src/schema.rs` & `nucliadb_node_binding-3.0.3.post1216/local_dependencies/nucliadb_texts2/src/schema.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.0.3.post1215/local_dependencies/nucliadb_texts2/src/search_query.rs` & `nucliadb_node_binding-3.0.3.post1216/local_dependencies/nucliadb_texts2/src/search_query.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.0.3.post1215/local_dependencies/nucliadb_texts2/src/writer.rs` & `nucliadb_node_binding-3.0.3.post1216/local_dependencies/nucliadb_texts2/src/writer.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.0.3.post1215/local_dependencies/nucliadb_texts2/tests/common/mod.rs` & `nucliadb_node_binding-3.0.3.post1216/local_dependencies/nucliadb_texts2/tests/common/mod.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.0.3.post1215/local_dependencies/nucliadb_texts2/tests/test_reader.rs` & `nucliadb_node_binding-3.0.3.post1216/local_dependencies/nucliadb_texts2/tests/test_reader.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.0.3.post1215/local_dependencies/nucliadb_texts2/tests/test_search.rs` & `nucliadb_node_binding-3.0.3.post1216/local_dependencies/nucliadb_texts2/tests/test_search.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.0.3.post1215/local_dependencies/nucliadb_texts2/tests/test_streaming.rs` & `nucliadb_node_binding-3.0.3.post1216/local_dependencies/nucliadb_texts2/tests/test_streaming.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.0.3.post1215/local_dependencies/nucliadb_texts2/tests/test_writer.rs` & `nucliadb_node_binding-3.0.3.post1216/local_dependencies/nucliadb_texts2/tests/test_writer.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.0.3.post1215/local_dependencies/nucliadb_paragraphs3/Cargo.toml` & `nucliadb_node_binding-3.0.3.post1216/local_dependencies/nucliadb_paragraphs3/Cargo.toml`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.0.3.post1215/local_dependencies/nucliadb_paragraphs3/src/fuzzy_query.rs` & `nucliadb_node_binding-3.0.3.post1216/local_dependencies/nucliadb_paragraphs2/src/fuzzy_query.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.0.3.post1215/local_dependencies/nucliadb_paragraphs3/src/lib.rs` & `nucliadb_node_binding-3.0.3.post1216/local_dependencies/nucliadb_paragraphs3/src/lib.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.0.3.post1215/local_dependencies/nucliadb_paragraphs3/src/query_io.rs` & `nucliadb_node_binding-3.0.3.post1216/local_dependencies/nucliadb_paragraphs2/src/query_io.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.0.3.post1215/local_dependencies/nucliadb_paragraphs3/src/reader.rs` & `nucliadb_node_binding-3.0.3.post1216/local_dependencies/nucliadb_paragraphs3/src/reader.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.0.3.post1215/local_dependencies/nucliadb_paragraphs3/src/schema.rs` & `nucliadb_node_binding-3.0.3.post1216/local_dependencies/nucliadb_paragraphs3/src/schema.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.0.3.post1215/local_dependencies/nucliadb_paragraphs3/src/search_query.rs` & `nucliadb_node_binding-3.0.3.post1216/local_dependencies/nucliadb_paragraphs3/src/search_query.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.0.3.post1215/local_dependencies/nucliadb_paragraphs3/src/search_response.rs` & `nucliadb_node_binding-3.0.3.post1216/local_dependencies/nucliadb_paragraphs3/src/search_response.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.0.3.post1215/local_dependencies/nucliadb_paragraphs3/src/set_query.rs` & `nucliadb_node_binding-3.0.3.post1216/local_dependencies/nucliadb_paragraphs3/src/set_query.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.0.3.post1215/local_dependencies/nucliadb_paragraphs3/src/stop_words.rs` & `nucliadb_node_binding-3.0.3.post1216/local_dependencies/nucliadb_paragraphs2/src/stop_words.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.0.3.post1215/local_dependencies/nucliadb_paragraphs3/src/writer.rs` & `nucliadb_node_binding-3.0.3.post1216/local_dependencies/nucliadb_paragraphs3/src/writer.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.0.3.post1215/local_dependencies/nucliadb_paragraphs3/stop_words/ar.json` & `nucliadb_node_binding-3.0.3.post1216/local_dependencies/nucliadb_paragraphs2/stop_words/ar.json`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.0.3.post1215/local_dependencies/nucliadb_paragraphs3/stop_words/az.json` & `nucliadb_node_binding-3.0.3.post1216/local_dependencies/nucliadb_paragraphs2/stop_words/az.json`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.0.3.post1215/local_dependencies/nucliadb_paragraphs3/stop_words/bn.json` & `nucliadb_node_binding-3.0.3.post1216/local_dependencies/nucliadb_paragraphs2/stop_words/bn.json`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.0.3.post1215/local_dependencies/nucliadb_paragraphs3/stop_words/ca.json` & `nucliadb_node_binding-3.0.3.post1216/local_dependencies/nucliadb_paragraphs2/stop_words/ca.json`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.0.3.post1215/local_dependencies/nucliadb_paragraphs3/stop_words/ch.json` & `nucliadb_node_binding-3.0.3.post1216/local_dependencies/nucliadb_paragraphs2/stop_words/ch.json`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.0.3.post1215/local_dependencies/nucliadb_paragraphs3/stop_words/da.json` & `nucliadb_node_binding-3.0.3.post1216/local_dependencies/nucliadb_paragraphs2/stop_words/da.json`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.0.3.post1215/local_dependencies/nucliadb_paragraphs3/stop_words/de.json` & `nucliadb_node_binding-3.0.3.post1216/local_dependencies/nucliadb_paragraphs2/stop_words/de.json`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.0.3.post1215/local_dependencies/nucliadb_paragraphs3/stop_words/el.json` & `nucliadb_node_binding-3.0.3.post1216/local_dependencies/nucliadb_paragraphs2/stop_words/el.json`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.0.3.post1215/local_dependencies/nucliadb_paragraphs3/stop_words/en.json` & `nucliadb_node_binding-3.0.3.post1216/local_dependencies/nucliadb_paragraphs2/stop_words/en.json`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.0.3.post1215/local_dependencies/nucliadb_paragraphs3/stop_words/es.json` & `nucliadb_node_binding-3.0.3.post1216/local_dependencies/nucliadb_paragraphs2/stop_words/es.json`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.0.3.post1215/local_dependencies/nucliadb_paragraphs3/stop_words/eu.json` & `nucliadb_node_binding-3.0.3.post1216/local_dependencies/nucliadb_paragraphs2/stop_words/eu.json`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.0.3.post1215/local_dependencies/nucliadb_paragraphs3/stop_words/extract.py` & `nucliadb_node_binding-3.0.3.post1216/local_dependencies/nucliadb_paragraphs2/stop_words/extract.py`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.0.3.post1215/local_dependencies/nucliadb_paragraphs3/stop_words/fi.json` & `nucliadb_node_binding-3.0.3.post1216/local_dependencies/nucliadb_paragraphs2/stop_words/fi.json`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.0.3.post1215/local_dependencies/nucliadb_paragraphs3/stop_words/fr.json` & `nucliadb_node_binding-3.0.3.post1216/local_dependencies/nucliadb_paragraphs2/stop_words/fr.json`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.0.3.post1215/local_dependencies/nucliadb_paragraphs3/stop_words/he.json` & `nucliadb_node_binding-3.0.3.post1216/local_dependencies/nucliadb_paragraphs2/stop_words/he.json`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.0.3.post1215/local_dependencies/nucliadb_paragraphs3/stop_words/hu.json` & `nucliadb_node_binding-3.0.3.post1216/local_dependencies/nucliadb_paragraphs2/stop_words/hu.json`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.0.3.post1215/local_dependencies/nucliadb_paragraphs3/stop_words/id.json` & `nucliadb_node_binding-3.0.3.post1216/local_dependencies/nucliadb_paragraphs2/stop_words/id.json`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.0.3.post1215/local_dependencies/nucliadb_paragraphs3/stop_words/it.json` & `nucliadb_node_binding-3.0.3.post1216/local_dependencies/nucliadb_paragraphs2/stop_words/it.json`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.0.3.post1215/local_dependencies/nucliadb_paragraphs3/stop_words/kk.json` & `nucliadb_node_binding-3.0.3.post1216/local_dependencies/nucliadb_paragraphs2/stop_words/kk.json`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.0.3.post1215/local_dependencies/nucliadb_paragraphs3/stop_words/ne.json` & `nucliadb_node_binding-3.0.3.post1216/local_dependencies/nucliadb_paragraphs2/stop_words/ne.json`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.0.3.post1215/local_dependencies/nucliadb_paragraphs3/stop_words/nl.json` & `nucliadb_node_binding-3.0.3.post1216/local_dependencies/nucliadb_paragraphs2/stop_words/nl.json`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.0.3.post1215/local_dependencies/nucliadb_paragraphs3/stop_words/no.json` & `nucliadb_node_binding-3.0.3.post1216/local_dependencies/nucliadb_paragraphs2/stop_words/no.json`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.0.3.post1215/local_dependencies/nucliadb_paragraphs3/stop_words/pt.json` & `nucliadb_node_binding-3.0.3.post1216/local_dependencies/nucliadb_paragraphs2/stop_words/pt.json`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.0.3.post1215/local_dependencies/nucliadb_paragraphs3/stop_words/ro.json` & `nucliadb_node_binding-3.0.3.post1216/local_dependencies/nucliadb_paragraphs2/stop_words/ro.json`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.0.3.post1215/local_dependencies/nucliadb_paragraphs3/stop_words/ru.json` & `nucliadb_node_binding-3.0.3.post1216/local_dependencies/nucliadb_paragraphs2/stop_words/ru.json`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.0.3.post1215/local_dependencies/nucliadb_paragraphs3/stop_words/sl.json` & `nucliadb_node_binding-3.0.3.post1216/local_dependencies/nucliadb_paragraphs2/stop_words/sl.json`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.0.3.post1215/local_dependencies/nucliadb_paragraphs3/stop_words/sv.json` & `nucliadb_node_binding-3.0.3.post1216/local_dependencies/nucliadb_paragraphs2/stop_words/sv.json`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.0.3.post1215/local_dependencies/nucliadb_paragraphs3/stop_words/tg.json` & `nucliadb_node_binding-3.0.3.post1216/local_dependencies/nucliadb_paragraphs2/stop_words/tg.json`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.0.3.post1215/local_dependencies/nucliadb_vectors/Cargo.toml` & `nucliadb_node_binding-3.0.3.post1216/local_dependencies/nucliadb_vectors/Cargo.toml`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.0.3.post1215/local_dependencies/nucliadb_vectors/docs/labels.drawio.svg` & `nucliadb_node_binding-3.0.3.post1216/local_dependencies/nucliadb_vectors/docs/labels.drawio.svg`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.0.3.post1215/local_dependencies/nucliadb_vectors/src/data_point/disk_hnsw.rs` & `nucliadb_node_binding-3.0.3.post1216/local_dependencies/nucliadb_vectors/src/data_point/disk_hnsw.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.0.3.post1215/local_dependencies/nucliadb_vectors/src/data_point/mod.rs` & `nucliadb_node_binding-3.0.3.post1216/local_dependencies/nucliadb_vectors/src/data_point/mod.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.0.3.post1215/local_dependencies/nucliadb_vectors/src/data_point/node.rs` & `nucliadb_node_binding-3.0.3.post1216/local_dependencies/nucliadb_vectors/src/data_point/node.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.0.3.post1215/local_dependencies/nucliadb_vectors/src/data_point/ops_hnsw.rs` & `nucliadb_node_binding-3.0.3.post1216/local_dependencies/nucliadb_vectors/src/data_point/ops_hnsw.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.0.3.post1215/local_dependencies/nucliadb_vectors/src/data_point/params.rs` & `nucliadb_node_binding-3.0.3.post1216/local_dependencies/nucliadb_vectors/src/data_point/params.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.0.3.post1215/local_dependencies/nucliadb_vectors/src/data_point/ram_hnsw.rs` & `nucliadb_node_binding-3.0.3.post1216/local_dependencies/nucliadb_vectors/src/data_point/ram_hnsw.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.0.3.post1215/local_dependencies/nucliadb_vectors/src/data_point/tests.rs` & `nucliadb_node_binding-3.0.3.post1216/local_dependencies/nucliadb_vectors/src/data_point/tests.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.0.3.post1215/local_dependencies/nucliadb_vectors/src/data_point_provider/garbage_collector.rs` & `nucliadb_node_binding-3.0.3.post1216/local_dependencies/nucliadb_vectors/src/data_point_provider/garbage_collector.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.0.3.post1215/local_dependencies/nucliadb_vectors/src/data_point_provider/mod.rs` & `nucliadb_node_binding-3.0.3.post1216/local_dependencies/nucliadb_vectors/src/data_point_provider/mod.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.0.3.post1215/local_dependencies/nucliadb_vectors/src/data_point_provider/reader.rs` & `nucliadb_node_binding-3.0.3.post1216/local_dependencies/nucliadb_vectors/src/data_point_provider/reader.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.0.3.post1215/local_dependencies/nucliadb_vectors/src/data_point_provider/replication.rs` & `nucliadb_node_binding-3.0.3.post1216/local_dependencies/nucliadb_vectors/src/data_point_provider/replication.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.0.3.post1215/local_dependencies/nucliadb_vectors/src/data_point_provider/state.rs` & `nucliadb_node_binding-3.0.3.post1216/local_dependencies/nucliadb_vectors/src/data_point_provider/state.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.0.3.post1215/local_dependencies/nucliadb_vectors/src/data_point_provider/writer.rs` & `nucliadb_node_binding-3.0.3.post1216/local_dependencies/nucliadb_vectors/src/data_point_provider/writer.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.0.3.post1215/local_dependencies/nucliadb_vectors/src/data_types/data_store.rs` & `nucliadb_node_binding-3.0.3.post1216/local_dependencies/nucliadb_vectors/src/data_types/data_store.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.0.3.post1215/local_dependencies/nucliadb_vectors/src/data_types/dtrie_ram.rs` & `nucliadb_node_binding-3.0.3.post1216/local_dependencies/nucliadb_vectors/src/data_types/dtrie_ram.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.0.3.post1215/local_dependencies/nucliadb_vectors/src/data_types/mod.rs` & `nucliadb_node_binding-3.0.3.post1216/local_dependencies/nucliadb_vectors/src/data_types/mod.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.0.3.post1215/local_dependencies/nucliadb_vectors/src/data_types/trie.rs` & `nucliadb_node_binding-3.0.3.post1216/local_dependencies/nucliadb_vectors/src/data_types/trie.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.0.3.post1215/local_dependencies/nucliadb_vectors/src/data_types/trie_ram.rs` & `nucliadb_node_binding-3.0.3.post1216/local_dependencies/nucliadb_vectors/src/data_types/trie_ram.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.0.3.post1215/local_dependencies/nucliadb_vectors/src/data_types/vector.rs` & `nucliadb_node_binding-3.0.3.post1216/local_dependencies/nucliadb_vectors/src/data_types/vector.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.0.3.post1215/local_dependencies/nucliadb_vectors/src/formula/mod.rs` & `nucliadb_node_binding-3.0.3.post1216/local_dependencies/nucliadb_vectors/src/formula/mod.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.0.3.post1215/local_dependencies/nucliadb_vectors/src/lib.rs` & `nucliadb_node_binding-3.0.3.post1216/local_dependencies/nucliadb_vectors/src/lib.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.0.3.post1215/local_dependencies/nucliadb_vectors/src/service/mod.rs` & `nucliadb_node_binding-3.0.3.post1216/local_dependencies/nucliadb_vectors/src/service/mod.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.0.3.post1215/local_dependencies/nucliadb_vectors/src/service/query_io.rs` & `nucliadb_node_binding-3.0.3.post1216/local_dependencies/nucliadb_vectors/src/service/query_io.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.0.3.post1215/local_dependencies/nucliadb_vectors/src/service/reader.rs` & `nucliadb_node_binding-3.0.3.post1216/local_dependencies/nucliadb_vectors/src/service/reader.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.0.3.post1215/local_dependencies/nucliadb_vectors/src/service/writer.rs` & `nucliadb_node_binding-3.0.3.post1216/local_dependencies/nucliadb_vectors/src/service/writer.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.0.3.post1215/local_dependencies/nucliadb_vectors/src/utils.rs` & `nucliadb_node_binding-3.0.3.post1216/local_dependencies/nucliadb_vectors/src/utils.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.0.3.post1215/local_dependencies/nucliadb_vectors/tests/test_merge.rs` & `nucliadb_node_binding-3.0.3.post1216/local_dependencies/nucliadb_vectors/tests/test_merge.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.0.3.post1215/local_dependencies/nucliadb_procs/src/lib.rs` & `nucliadb_node_binding-3.0.3.post1216/local_dependencies/nucliadb_procs/src/lib.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.0.3.post1215/local_dependencies/nucliadb_procs/src/measure.rs` & `nucliadb_node_binding-3.0.3.post1216/local_dependencies/nucliadb_procs/src/measure.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.0.3.post1215/local_dependencies/nucliadb_procs/tests/dont_compile/actor_defined_twice.rs` & `nucliadb_node_binding-3.0.3.post1216/local_dependencies/nucliadb_procs/tests/dont_compile/actor_defined_twice.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.0.3.post1215/local_dependencies/nucliadb_procs/tests/dont_compile/actor_not_defined.rs` & `nucliadb_node_binding-3.0.3.post1216/local_dependencies/nucliadb_procs/tests/dont_compile/actor_not_defined.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.0.3.post1215/local_dependencies/nucliadb_procs/tests/dont_compile/metric_defined_twice.rs` & `nucliadb_node_binding-3.0.3.post1216/local_dependencies/nucliadb_procs/tests/dont_compile/metric_defined_twice.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.0.3.post1215/local_dependencies/nucliadb_procs/tests/dont_compile/wrong_actor.rs` & `nucliadb_node_binding-3.0.3.post1216/local_dependencies/nucliadb_procs/tests/dont_compile/wrong_actor.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.0.3.post1215/local_dependencies/nucliadb_procs/tests/dont_compile/wrong_actor.stderr` & `nucliadb_node_binding-3.0.3.post1216/local_dependencies/nucliadb_procs/tests/dont_compile/wrong_actor.stderr`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.0.3.post1215/local_dependencies/nucliadb_procs/tests/test_measure.rs` & `nucliadb_node_binding-3.0.3.post1216/local_dependencies/nucliadb_procs/tests/test_measure.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.0.3.post1215/local_dependencies/nucliadb_paragraphs2/Cargo.toml` & `nucliadb_node_binding-3.0.3.post1216/local_dependencies/nucliadb_paragraphs2/Cargo.toml`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.0.3.post1215/local_dependencies/nucliadb_paragraphs2/src/fuzzy_query.rs` & `nucliadb_node_binding-3.0.3.post1216/local_dependencies/nucliadb_paragraphs3/src/fuzzy_query.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.0.3.post1215/local_dependencies/nucliadb_paragraphs2/src/lib.rs` & `nucliadb_node_binding-3.0.3.post1216/local_dependencies/nucliadb_paragraphs2/src/lib.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.0.3.post1215/local_dependencies/nucliadb_paragraphs2/src/query_io.rs` & `nucliadb_node_binding-3.0.3.post1216/local_dependencies/nucliadb_paragraphs3/src/query_io.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.0.3.post1215/local_dependencies/nucliadb_paragraphs2/src/reader.rs` & `nucliadb_node_binding-3.0.3.post1216/local_dependencies/nucliadb_paragraphs2/src/reader.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.0.3.post1215/local_dependencies/nucliadb_paragraphs2/src/schema.rs` & `nucliadb_node_binding-3.0.3.post1216/local_dependencies/nucliadb_paragraphs2/src/schema.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.0.3.post1215/local_dependencies/nucliadb_paragraphs2/src/search_query.rs` & `nucliadb_node_binding-3.0.3.post1216/local_dependencies/nucliadb_paragraphs2/src/search_query.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.0.3.post1215/local_dependencies/nucliadb_paragraphs2/src/search_response.rs` & `nucliadb_node_binding-3.0.3.post1216/local_dependencies/nucliadb_paragraphs2/src/search_response.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.0.3.post1215/local_dependencies/nucliadb_paragraphs2/src/stop_words.rs` & `nucliadb_node_binding-3.0.3.post1216/local_dependencies/nucliadb_paragraphs3/src/stop_words.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.0.3.post1215/local_dependencies/nucliadb_paragraphs2/src/writer.rs` & `nucliadb_node_binding-3.0.3.post1216/local_dependencies/nucliadb_paragraphs2/src/writer.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.0.3.post1215/local_dependencies/nucliadb_paragraphs2/stop_words/ar.json` & `nucliadb_node_binding-3.0.3.post1216/local_dependencies/nucliadb_paragraphs3/stop_words/ar.json`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.0.3.post1215/local_dependencies/nucliadb_paragraphs2/stop_words/az.json` & `nucliadb_node_binding-3.0.3.post1216/local_dependencies/nucliadb_paragraphs3/stop_words/az.json`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.0.3.post1215/local_dependencies/nucliadb_paragraphs2/stop_words/bn.json` & `nucliadb_node_binding-3.0.3.post1216/local_dependencies/nucliadb_paragraphs3/stop_words/bn.json`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.0.3.post1215/local_dependencies/nucliadb_paragraphs2/stop_words/ca.json` & `nucliadb_node_binding-3.0.3.post1216/local_dependencies/nucliadb_paragraphs3/stop_words/ca.json`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.0.3.post1215/local_dependencies/nucliadb_paragraphs2/stop_words/ch.json` & `nucliadb_node_binding-3.0.3.post1216/local_dependencies/nucliadb_paragraphs3/stop_words/ch.json`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.0.3.post1215/local_dependencies/nucliadb_paragraphs2/stop_words/da.json` & `nucliadb_node_binding-3.0.3.post1216/local_dependencies/nucliadb_paragraphs3/stop_words/da.json`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.0.3.post1215/local_dependencies/nucliadb_paragraphs2/stop_words/de.json` & `nucliadb_node_binding-3.0.3.post1216/local_dependencies/nucliadb_paragraphs3/stop_words/de.json`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.0.3.post1215/local_dependencies/nucliadb_paragraphs2/stop_words/el.json` & `nucliadb_node_binding-3.0.3.post1216/local_dependencies/nucliadb_paragraphs3/stop_words/el.json`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.0.3.post1215/local_dependencies/nucliadb_paragraphs2/stop_words/en.json` & `nucliadb_node_binding-3.0.3.post1216/local_dependencies/nucliadb_paragraphs3/stop_words/en.json`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.0.3.post1215/local_dependencies/nucliadb_paragraphs2/stop_words/es.json` & `nucliadb_node_binding-3.0.3.post1216/local_dependencies/nucliadb_paragraphs3/stop_words/es.json`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.0.3.post1215/local_dependencies/nucliadb_paragraphs2/stop_words/eu.json` & `nucliadb_node_binding-3.0.3.post1216/local_dependencies/nucliadb_paragraphs3/stop_words/eu.json`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.0.3.post1215/local_dependencies/nucliadb_paragraphs2/stop_words/extract.py` & `nucliadb_node_binding-3.0.3.post1216/local_dependencies/nucliadb_paragraphs3/stop_words/extract.py`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.0.3.post1215/local_dependencies/nucliadb_paragraphs2/stop_words/fi.json` & `nucliadb_node_binding-3.0.3.post1216/local_dependencies/nucliadb_paragraphs3/stop_words/fi.json`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.0.3.post1215/local_dependencies/nucliadb_paragraphs2/stop_words/fr.json` & `nucliadb_node_binding-3.0.3.post1216/local_dependencies/nucliadb_paragraphs3/stop_words/fr.json`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.0.3.post1215/local_dependencies/nucliadb_paragraphs2/stop_words/he.json` & `nucliadb_node_binding-3.0.3.post1216/local_dependencies/nucliadb_paragraphs3/stop_words/he.json`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.0.3.post1215/local_dependencies/nucliadb_paragraphs2/stop_words/hu.json` & `nucliadb_node_binding-3.0.3.post1216/local_dependencies/nucliadb_paragraphs3/stop_words/hu.json`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.0.3.post1215/local_dependencies/nucliadb_paragraphs2/stop_words/id.json` & `nucliadb_node_binding-3.0.3.post1216/local_dependencies/nucliadb_paragraphs3/stop_words/id.json`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.0.3.post1215/local_dependencies/nucliadb_paragraphs2/stop_words/it.json` & `nucliadb_node_binding-3.0.3.post1216/local_dependencies/nucliadb_paragraphs3/stop_words/it.json`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.0.3.post1215/local_dependencies/nucliadb_paragraphs2/stop_words/kk.json` & `nucliadb_node_binding-3.0.3.post1216/local_dependencies/nucliadb_paragraphs3/stop_words/kk.json`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.0.3.post1215/local_dependencies/nucliadb_paragraphs2/stop_words/ne.json` & `nucliadb_node_binding-3.0.3.post1216/local_dependencies/nucliadb_paragraphs3/stop_words/ne.json`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.0.3.post1215/local_dependencies/nucliadb_paragraphs2/stop_words/nl.json` & `nucliadb_node_binding-3.0.3.post1216/local_dependencies/nucliadb_paragraphs3/stop_words/nl.json`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.0.3.post1215/local_dependencies/nucliadb_paragraphs2/stop_words/no.json` & `nucliadb_node_binding-3.0.3.post1216/local_dependencies/nucliadb_paragraphs3/stop_words/no.json`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.0.3.post1215/local_dependencies/nucliadb_paragraphs2/stop_words/pt.json` & `nucliadb_node_binding-3.0.3.post1216/local_dependencies/nucliadb_paragraphs3/stop_words/pt.json`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.0.3.post1215/local_dependencies/nucliadb_paragraphs2/stop_words/ro.json` & `nucliadb_node_binding-3.0.3.post1216/local_dependencies/nucliadb_paragraphs3/stop_words/ro.json`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.0.3.post1215/local_dependencies/nucliadb_paragraphs2/stop_words/ru.json` & `nucliadb_node_binding-3.0.3.post1216/local_dependencies/nucliadb_paragraphs3/stop_words/ru.json`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.0.3.post1215/local_dependencies/nucliadb_paragraphs2/stop_words/sl.json` & `nucliadb_node_binding-3.0.3.post1216/local_dependencies/nucliadb_paragraphs3/stop_words/sl.json`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.0.3.post1215/local_dependencies/nucliadb_paragraphs2/stop_words/sv.json` & `nucliadb_node_binding-3.0.3.post1216/local_dependencies/nucliadb_paragraphs3/stop_words/sv.json`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.0.3.post1215/local_dependencies/nucliadb_paragraphs2/stop_words/tg.json` & `nucliadb_node_binding-3.0.3.post1216/local_dependencies/nucliadb_paragraphs3/stop_words/tg.json`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.0.3.post1215/local_dependencies/nucliadb_core/Cargo.toml` & `nucliadb_node_binding-3.0.3.post1216/local_dependencies/nucliadb_core/Cargo.toml`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.0.3.post1215/local_dependencies/nucliadb_core/src/fs_state.rs` & `nucliadb_node_binding-3.0.3.post1216/local_dependencies/nucliadb_core/src/fs_state.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.0.3.post1215/local_dependencies/nucliadb_core/src/lib.rs` & `nucliadb_node_binding-3.0.3.post1216/local_dependencies/nucliadb_core/src/lib.rs`

 * *Files 8% similar despite different names*

```diff
@@ -47,14 +47,15 @@
     pub use crate::{node_error, read_rw_lock, write_rw_lock, Context, NodeResult};
 }
 
 use std::collections::HashMap;
 use std::sync::{RwLock, RwLockReadGuard, RwLockWriteGuard};
 
 pub use anyhow::{anyhow as node_error, Context, Error};
+use nucliadb_protos::utils::ReleaseChannel;
 use serde::{Deserialize, Serialize};
 
 use crate::tantivy_replica::TantivyReplicaState;
 pub type NodeResult<O> = anyhow::Result<O>;
 
 #[derive(Clone, Copy, Serialize, Deserialize, Debug, PartialEq, Eq, Default)]
 pub enum Channel {
@@ -68,14 +69,23 @@
         match value {
             1 => Channel::EXPERIMENTAL,
             _ => Channel::STABLE,
         }
     }
 }
 
+impl From<Channel> for i32 {
+    fn from(value: Channel) -> Self {
+        match value {
+            Channel::STABLE => ReleaseChannel::Stable as i32,
+            Channel::EXPERIMENTAL => ReleaseChannel::Experimental as i32,
+        }
+    }
+}
+
 #[derive(Debug, Default)]
 pub struct RawReplicaState {
     pub metadata_files: HashMap<String, Vec<u8>>,
     pub files: Vec<String>,
 }
 
 impl RawReplicaState {
```

### Comparing `nucliadb_node_binding-3.0.3.post1215/local_dependencies/nucliadb_core/src/merge.rs` & `nucliadb_node_binding-3.0.3.post1216/local_dependencies/nucliadb_core/src/merge.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.0.3.post1215/local_dependencies/nucliadb_core/src/metrics/meters/mod.rs` & `nucliadb_node_binding-3.0.3.post1216/local_dependencies/nucliadb_core/src/metrics/meters/mod.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.0.3.post1215/local_dependencies/nucliadb_core/src/metrics/meters/prometheus.rs` & `nucliadb_node_binding-3.0.3.post1216/local_dependencies/nucliadb_core/src/metrics/meters/prometheus.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.0.3.post1215/local_dependencies/nucliadb_core/src/metrics/metric/grpc_ops.rs` & `nucliadb_node_binding-3.0.3.post1216/local_dependencies/nucliadb_core/src/metrics/metric/grpc_ops.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.0.3.post1215/local_dependencies/nucliadb_core/src/metrics/metric/mod.rs` & `nucliadb_node_binding-3.0.3.post1216/local_dependencies/nucliadb_core/src/metrics/metric/mod.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.0.3.post1215/local_dependencies/nucliadb_core/src/metrics/metric/replication.rs` & `nucliadb_node_binding-3.0.3.post1216/local_dependencies/nucliadb_core/src/metrics/metric/replication.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.0.3.post1215/local_dependencies/nucliadb_core/src/metrics/metric/request_time.rs` & `nucliadb_node_binding-3.0.3.post1216/local_dependencies/nucliadb_core/src/metrics/metric/request_time.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.0.3.post1215/local_dependencies/nucliadb_core/src/metrics/metric/shard_cache.rs` & `nucliadb_node_binding-3.0.3.post1216/local_dependencies/nucliadb_core/src/metrics/metric/shard_cache.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.0.3.post1215/local_dependencies/nucliadb_core/src/metrics/metric/tokio_runtime.rs` & `nucliadb_node_binding-3.0.3.post1216/local_dependencies/nucliadb_core/src/metrics/metric/tokio_runtime.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.0.3.post1215/local_dependencies/nucliadb_core/src/metrics/metric/tokio_tasks.rs` & `nucliadb_node_binding-3.0.3.post1216/local_dependencies/nucliadb_core/src/metrics/metric/tokio_tasks.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.0.3.post1215/local_dependencies/nucliadb_core/src/metrics/metric/vectors.rs` & `nucliadb_node_binding-3.0.3.post1216/local_dependencies/nucliadb_core/src/metrics/metric/vectors.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.0.3.post1215/local_dependencies/nucliadb_core/src/metrics/mod.rs` & `nucliadb_node_binding-3.0.3.post1216/local_dependencies/nucliadb_core/src/metrics/mod.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.0.3.post1215/local_dependencies/nucliadb_core/src/metrics/task_monitor.rs` & `nucliadb_node_binding-3.0.3.post1216/local_dependencies/nucliadb_core/src/metrics/task_monitor.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.0.3.post1215/local_dependencies/nucliadb_core/src/metrics/tests.rs` & `nucliadb_node_binding-3.0.3.post1216/local_dependencies/nucliadb_core/src/metrics/tests.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.0.3.post1215/local_dependencies/nucliadb_core/src/paragraphs.rs` & `nucliadb_node_binding-3.0.3.post1216/local_dependencies/nucliadb_core/src/paragraphs.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.0.3.post1215/local_dependencies/nucliadb_core/src/query_language/mod.rs` & `nucliadb_node_binding-3.0.3.post1216/local_dependencies/nucliadb_core/src/query_language/mod.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.0.3.post1215/local_dependencies/nucliadb_core/src/query_planner.rs` & `nucliadb_node_binding-3.0.3.post1216/local_dependencies/nucliadb_core/src/query_planner.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.0.3.post1215/local_dependencies/nucliadb_core/src/relations.rs` & `nucliadb_node_binding-3.0.3.post1216/local_dependencies/nucliadb_core/src/relations.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.0.3.post1215/local_dependencies/nucliadb_core/src/tantivy_replica.rs` & `nucliadb_node_binding-3.0.3.post1216/local_dependencies/nucliadb_core/src/tantivy_replica.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.0.3.post1215/local_dependencies/nucliadb_core/src/texts.rs` & `nucliadb_node_binding-3.0.3.post1216/local_dependencies/nucliadb_core/src/texts.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.0.3.post1215/local_dependencies/nucliadb_core/src/vectors.rs` & `nucliadb_node_binding-3.0.3.post1216/local_dependencies/nucliadb_core/src/vectors.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.0.3.post1215/local_dependencies/nucliadb_node/Cargo.toml` & `nucliadb_node_binding-3.0.3.post1216/local_dependencies/nucliadb_node/Cargo.toml`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.0.3.post1215/local_dependencies/nucliadb_node/.rustc_info.json` & `nucliadb_node_binding-3.0.3.post1216/local_dependencies/nucliadb_node/.rustc_info.json`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.0.3.post1215/local_dependencies/nucliadb_node/Makefile` & `nucliadb_node_binding-3.0.3.post1216/local_dependencies/nucliadb_node/Makefile`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.0.3.post1215/local_dependencies/nucliadb_node/README.md` & `nucliadb_node_binding-3.0.3.post1216/local_dependencies/nucliadb_node/README.md`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.0.3.post1215/local_dependencies/nucliadb_node/nucliadb_node/__init__.py` & `nucliadb_node_binding-3.0.3.post1216/local_dependencies/nucliadb_node/nucliadb_node/__init__.py`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.0.3.post1215/local_dependencies/nucliadb_node/nucliadb_node/app.py` & `nucliadb_node_binding-3.0.3.post1216/local_dependencies/nucliadb_node/nucliadb_node/app.py`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.0.3.post1215/local_dependencies/nucliadb_node/nucliadb_node/indexer.py` & `nucliadb_node_binding-3.0.3.post1216/local_dependencies/nucliadb_node/nucliadb_node/indexer.py`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.0.3.post1215/local_dependencies/nucliadb_node/nucliadb_node/listeners/__init__.py` & `nucliadb_node_binding-3.0.3.post1216/local_dependencies/nucliadb_node/nucliadb_node/listeners/__init__.py`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.0.3.post1215/local_dependencies/nucliadb_node/nucliadb_node/listeners/indexed_publisher.py` & `nucliadb_node_binding-3.0.3.post1216/local_dependencies/nucliadb_node/nucliadb_node/listeners/indexed_publisher.py`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.0.3.post1215/local_dependencies/nucliadb_node/nucliadb_node/pull.py` & `nucliadb_node_binding-3.0.3.post1216/local_dependencies/nucliadb_node/nucliadb_node/pull.py`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.0.3.post1215/local_dependencies/nucliadb_node/nucliadb_node/service.py` & `nucliadb_node_binding-3.0.3.post1216/local_dependencies/nucliadb_node/nucliadb_node/service.py`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.0.3.post1215/local_dependencies/nucliadb_node/nucliadb_node/settings.py` & `nucliadb_node_binding-3.0.3.post1216/local_dependencies/nucliadb_node/nucliadb_node/settings.py`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.0.3.post1215/local_dependencies/nucliadb_node/nucliadb_node/signals.py` & `nucliadb_node_binding-3.0.3.post1216/local_dependencies/nucliadb_node/nucliadb_node/signals.py`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.0.3.post1215/local_dependencies/nucliadb_node/nucliadb_node/tests/__init__.py` & `nucliadb_node_binding-3.0.3.post1216/local_dependencies/nucliadb_node/nucliadb_node/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.0.3.post1215/local_dependencies/nucliadb_node/nucliadb_node/tests/conftest.py` & `nucliadb_node_binding-3.0.3.post1216/local_dependencies/nucliadb_node/nucliadb_node/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.0.3.post1215/local_dependencies/nucliadb_node/nucliadb_node/tests/fixtures.py` & `nucliadb_node_binding-3.0.3.post1216/local_dependencies/nucliadb_node/nucliadb_node/tests/fixtures.py`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.0.3.post1215/local_dependencies/nucliadb_node/nucliadb_node/tests/integration/test_indexing.py` & `nucliadb_node_binding-3.0.3.post1216/local_dependencies/nucliadb_node/nucliadb_node/tests/integration/test_indexing.py`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.0.3.post1215/local_dependencies/nucliadb_node/nucliadb_node/tests/unit/test_app.py` & `nucliadb_node_binding-3.0.3.post1216/local_dependencies/nucliadb_node/nucliadb_node/tests/unit/test_app.py`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.0.3.post1215/local_dependencies/nucliadb_node/nucliadb_node/tests/unit/test_indexed_publisher.py` & `nucliadb_node_binding-3.0.3.post1216/local_dependencies/nucliadb_node/nucliadb_node/tests/unit/test_indexed_publisher.py`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.0.3.post1215/local_dependencies/nucliadb_node/nucliadb_node/tests/unit/test_indexer.py` & `nucliadb_node_binding-3.0.3.post1216/local_dependencies/nucliadb_node/nucliadb_node/tests/unit/test_indexer.py`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.0.3.post1215/local_dependencies/nucliadb_node/nucliadb_node/tests/unit/test_pull.py` & `nucliadb_node_binding-3.0.3.post1216/local_dependencies/nucliadb_node/nucliadb_node/tests/unit/test_pull.py`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.0.3.post1215/local_dependencies/nucliadb_node/nucliadb_node/writer.py` & `nucliadb_node_binding-3.0.3.post1216/local_dependencies/nucliadb_node/nucliadb_node/writer.py`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.0.3.post1215/local_dependencies/nucliadb_node/setup.py` & `nucliadb_node_binding-3.0.3.post1216/local_dependencies/nucliadb_node/setup.py`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.0.3.post1215/local_dependencies/nucliadb_node/src/analytics/blocking.rs` & `nucliadb_node_binding-3.0.3.post1216/local_dependencies/nucliadb_node/src/analytics/blocking.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.0.3.post1215/local_dependencies/nucliadb_node/src/analytics/mod.rs` & `nucliadb_node_binding-3.0.3.post1216/local_dependencies/nucliadb_node/src/analytics/mod.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.0.3.post1215/local_dependencies/nucliadb_node/src/analytics/payload.rs` & `nucliadb_node_binding-3.0.3.post1216/local_dependencies/nucliadb_node/src/analytics/payload.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.0.3.post1215/local_dependencies/nucliadb_node/src/analytics/sender.rs` & `nucliadb_node_binding-3.0.3.post1216/local_dependencies/nucliadb_node/src/analytics/sender.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.0.3.post1215/local_dependencies/nucliadb_node/src/analytics/sink.rs` & `nucliadb_node_binding-3.0.3.post1216/local_dependencies/nucliadb_node/src/analytics/sink.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.0.3.post1215/local_dependencies/nucliadb_node/src/analytics/sync.rs` & `nucliadb_node_binding-3.0.3.post1216/local_dependencies/nucliadb_node/src/analytics/sync.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.0.3.post1215/local_dependencies/nucliadb_node/src/bin/reader.rs` & `nucliadb_node_binding-3.0.3.post1216/local_dependencies/nucliadb_node/src/bin/reader.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.0.3.post1215/local_dependencies/nucliadb_node/src/bin/writer.rs` & `nucliadb_node_binding-3.0.3.post1216/local_dependencies/nucliadb_node/src/bin/writer.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.0.3.post1215/local_dependencies/nucliadb_node/src/cache/mod.rs` & `nucliadb_node_binding-3.0.3.post1216/local_dependencies/nucliadb_node/src/cache/mod.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.0.3.post1215/local_dependencies/nucliadb_node/src/cache/reader_cache.rs` & `nucliadb_node_binding-3.0.3.post1216/local_dependencies/nucliadb_node/src/cache/reader_cache.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.0.3.post1215/local_dependencies/nucliadb_node/src/cache/resource_cache.rs` & `nucliadb_node_binding-3.0.3.post1216/local_dependencies/nucliadb_node/src/cache/resource_cache.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.0.3.post1215/local_dependencies/nucliadb_node/src/cache/writer_cache.rs` & `nucliadb_node_binding-3.0.3.post1216/local_dependencies/nucliadb_node/src/cache/writer_cache.rs`

 * *Files 2% similar despite different names*

```diff
@@ -231,14 +231,15 @@
 mod tests {
     use std::fs;
     use std::sync::Arc;
     use std::thread::sleep;
     use std::time::Duration;
 
     use crossbeam_utils::thread::scope;
+    use nucliadb_core::Channel;
     use tempfile::tempdir;
 
     use super::ShardWriterCache;
     use crate::settings::{EnvSettings, Settings};
     use crate::shards::metadata::{ShardMetadata, Similarity};
     use crate::shards::ShardId;
 
@@ -252,16 +253,22 @@
         .into();
         let cache = Arc::new(ShardWriterCache::new(settings.clone()));
 
         let shard_id_0 = ShardId::from("shard_id_0");
         let shard_0_path = settings.shards_path().join(shard_id_0.clone());
         fs::create_dir(settings.shards_path()).unwrap();
 
-        let shard_meta =
-            ShardMetadata::new(shard_0_path.clone(), shard_id_0.clone(), None, Similarity::Cosine, None, false);
+        let shard_meta = ShardMetadata::new(
+            shard_0_path.clone(),
+            shard_id_0.clone(),
+            "kbid".to_string(),
+            Similarity::Cosine,
+            Channel::EXPERIMENTAL,
+            false,
+        );
         cache.create(shard_meta).unwrap();
 
         let shard_0 = cache.get(&shard_id_0).unwrap();
 
         scope(|scope| {
             let cache_clone = cache.clone();
             let shard_id_0_clone = shard_id_0.clone();
@@ -293,14 +300,20 @@
         })
         .unwrap();
 
         // Shard is deleted, getting it should fail to load
         assert!(cache.get(&shard_id_0).is_err());
 
         // Recreating the shard should work (i.e: it's not stuck in the deletion state)
-        let shard_meta =
-            ShardMetadata::new(shard_0_path.clone(), shard_id_0.clone(), None, Similarity::Cosine, None, false);
+        let shard_meta = ShardMetadata::new(
+            shard_0_path.clone(),
+            shard_id_0.clone(),
+            "kbid".to_string(),
+            Similarity::Cosine,
+            Channel::EXPERIMENTAL,
+            false,
+        );
         cache.create(shard_meta).unwrap();
 
         assert!(cache.get(&shard_id_0).is_ok());
     }
 }
```

### Comparing `nucliadb_node_binding-3.0.3.post1215/local_dependencies/nucliadb_node/src/disk_structure.rs` & `nucliadb_node_binding-3.0.3.post1216/local_dependencies/nucliadb_node/src/disk_structure.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.0.3.post1215/local_dependencies/nucliadb_node/src/errors.rs` & `nucliadb_node_binding-3.0.3.post1216/local_dependencies/nucliadb_node/src/errors.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.0.3.post1215/local_dependencies/nucliadb_node/src/grpc/collect_garbage.rs` & `nucliadb_node_binding-3.0.3.post1216/local_dependencies/nucliadb_node/src/grpc/collect_garbage.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.0.3.post1215/local_dependencies/nucliadb_node/src/grpc/grpc_reader.rs` & `nucliadb_node_binding-3.0.3.post1216/local_dependencies/nucliadb_node/src/grpc/grpc_reader.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.0.3.post1215/local_dependencies/nucliadb_node/src/grpc/grpc_writer.rs` & `nucliadb_node_binding-3.0.3.post1216/local_dependencies/nucliadb_node/src/grpc/grpc_writer.rs`

 * *Files 1% similar despite different names*

```diff
@@ -116,17 +116,17 @@
         send_analytics_event(AnalyticsEvent::Create).await;
         let request = request.into_inner();
         let kbid = request.kbid.clone();
         let shard_id = uuid::Uuid::new_v4().to_string();
         let metadata = ShardMetadata::new(
             self.shards.shards_path.join(shard_id.clone()),
             shard_id,
-            Some(kbid),
+            kbid,
             request.similarity().into(),
-            Some(Channel::from(request.release_channel)),
+            Channel::from(request.release_channel),
             request.normalize_vectors,
         );
 
         let shards = Arc::clone(&self.shards);
         let new_shard = tokio::task::spawn_blocking(move || shards.create(metadata))
             .await
             .map_err(|error| tonic::Status::internal(format!("Error creating shard: {error:?}")))?;
```

### Comparing `nucliadb_node_binding-3.0.3.post1215/local_dependencies/nucliadb_node/src/grpc/middleware/debug.rs` & `nucliadb_node_binding-3.0.3.post1216/local_dependencies/nucliadb_node/src/grpc/middleware/debug.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.0.3.post1215/local_dependencies/nucliadb_node/src/grpc/middleware/metrics.rs` & `nucliadb_node_binding-3.0.3.post1216/local_dependencies/nucliadb_node/src/grpc/middleware/metrics.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.0.3.post1215/local_dependencies/nucliadb_node/src/grpc/middleware/mod.rs` & `nucliadb_node_binding-3.0.3.post1216/local_dependencies/nucliadb_node/src/grpc/middleware/mod.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.0.3.post1215/local_dependencies/nucliadb_node/src/grpc/middleware/telemetry.rs` & `nucliadb_node_binding-3.0.3.post1216/local_dependencies/nucliadb_node/src/grpc/middleware/telemetry.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.0.3.post1215/local_dependencies/nucliadb_node/src/grpc/mod.rs` & `nucliadb_node_binding-3.0.3.post1216/local_dependencies/nucliadb_node/src/grpc/mod.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.0.3.post1215/local_dependencies/nucliadb_node/src/grpc/update.rs` & `nucliadb_node_binding-3.0.3.post1216/local_dependencies/nucliadb_node/src/grpc/update.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.0.3.post1215/local_dependencies/nucliadb_node/src/http_server/metrics_service.rs` & `nucliadb_node_binding-3.0.3.post1216/local_dependencies/nucliadb_node/src/http_server/metrics_service.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.0.3.post1215/local_dependencies/nucliadb_node/src/http_server/mod.rs` & `nucliadb_node_binding-3.0.3.post1216/local_dependencies/nucliadb_node/src/http_server/mod.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.0.3.post1215/local_dependencies/nucliadb_node/src/http_server/traces_service.rs` & `nucliadb_node_binding-3.0.3.post1216/local_dependencies/nucliadb_node/src/http_server/traces_service.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.0.3.post1215/local_dependencies/nucliadb_node/src/lib.rs` & `nucliadb_node_binding-3.0.3.post1216/local_dependencies/nucliadb_node/src/lib.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.0.3.post1215/local_dependencies/nucliadb_node/src/lifecycle.rs` & `nucliadb_node_binding-3.0.3.post1216/local_dependencies/nucliadb_node/src/lifecycle.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.0.3.post1215/local_dependencies/nucliadb_node/src/merge/global.rs` & `nucliadb_node_binding-3.0.3.post1216/local_dependencies/nucliadb_node/src/merge/global.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.0.3.post1215/local_dependencies/nucliadb_node/src/merge/mod.rs` & `nucliadb_node_binding-3.0.3.post1216/local_dependencies/nucliadb_node/src/merge/mod.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.0.3.post1215/local_dependencies/nucliadb_node/src/merge/scheduler.rs` & `nucliadb_node_binding-3.0.3.post1216/local_dependencies/nucliadb_node/src/merge/scheduler.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.0.3.post1215/local_dependencies/nucliadb_node/src/merge/work.rs` & `nucliadb_node_binding-3.0.3.post1216/local_dependencies/nucliadb_node/src/merge/work.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.0.3.post1215/local_dependencies/nucliadb_node/src/node_metadata.rs` & `nucliadb_node_binding-3.0.3.post1216/local_dependencies/nucliadb_node/src/node_metadata.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.0.3.post1215/local_dependencies/nucliadb_node/src/replication/health.rs` & `nucliadb_node_binding-3.0.3.post1216/local_dependencies/nucliadb_node/src/replication/health.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.0.3.post1215/local_dependencies/nucliadb_node/src/replication/mod.rs` & `nucliadb_node_binding-3.0.3.post1216/local_dependencies/nucliadb_node/src/replication/mod.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.0.3.post1215/local_dependencies/nucliadb_node/src/replication/replicator.rs` & `nucliadb_node_binding-3.0.3.post1216/local_dependencies/nucliadb_node/src/replication/replicator.rs`

 * *Files 1% similar despite different names*

```diff
@@ -20,15 +20,15 @@
 use std::fs;
 use std::sync::atomic::AtomicBool;
 use std::sync::Arc;
 
 use futures::Future;
 use nucliadb_core::metrics::replication as replication_metrics;
 use nucliadb_core::tracing::{debug, error, info, warn};
-use nucliadb_core::{metrics, Error, NodeResult};
+use nucliadb_core::{metrics, Channel, Error, NodeResult};
 use nucliadb_protos::prelude::EmptyQuery;
 use nucliadb_protos::replication;
 use tokio::io::AsyncWriteExt;
 use tokio::sync::Semaphore;
 use tokio::time::Duration; // Import the Future trait
 use tonic::Request;
 
@@ -260,17 +260,17 @@
                 let shard_cache_clone = shard_cache.clone();
                 let shard_id_clone = shard_id.clone();
                 shard_lookup = tokio::task::spawn_blocking(move || shard_cache_clone.get(&shard_id_clone)).await?;
             } else {
                 let metadata = ShardMetadata::new(
                     shards_path.join(shard_id.clone()),
                     shard_state.shard_id.clone(),
-                    Some(shard_state.kbid.clone()),
+                    shard_state.kbid.clone(),
                     shard_state.similarity.clone().into(),
-                    None,
+                    Channel::from(shard_state.release_channel),
                     shard_state.normalize_vectors,
                 );
                 let shard_cache_clone = Arc::clone(&shard_cache);
 
                 warn!("Creating shard to replicate: {shard_id}");
                 let shard_create = tokio::task::spawn_blocking(move || shard_cache_clone.create(metadata)).await?;
                 if shard_create.is_err() {
```

### Comparing `nucliadb_node_binding-3.0.3.post1215/local_dependencies/nucliadb_node/src/replication/service.rs` & `nucliadb_node_binding-3.0.3.post1216/local_dependencies/nucliadb_node/src/replication/service.rs`

 * *Files 2% similar despite different names*

```diff
@@ -223,17 +223,18 @@
                     .unwrap_or(true);
                 if shard_changed_or_not_present {
                     let similarity: Similarity = metadata.similarity().into();
 
                     resp_shard_states.push(replication::PrimaryShardReplicationState {
                         shard_id,
                         generation_id: gen_id,
-                        kbid: metadata.kbid().unwrap_or_default(),
+                        kbid: metadata.kbid(),
                         similarity: similarity.to_string(),
                         normalize_vectors: metadata.normalize_vectors(),
+                        release_channel: metadata.channel().into(),
                     });
                 }
             } else {
                 warn!("Shard {} metadata not found", shard_id);
             }
         }
```

### Comparing `nucliadb_node_binding-3.0.3.post1215/local_dependencies/nucliadb_node/src/settings.rs` & `nucliadb_node_binding-3.0.3.post1216/local_dependencies/nucliadb_node/src/settings.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.0.3.post1215/local_dependencies/nucliadb_node/src/shards/errors.rs` & `nucliadb_node_binding-3.0.3.post1216/local_dependencies/nucliadb_node/src/shards/errors.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.0.3.post1215/local_dependencies/nucliadb_node/src/shards/metadata.rs` & `nucliadb_node_binding-3.0.3.post1216/local_dependencies/nucliadb_node/src/shards/metadata.rs`

 * *Files 9% similar despite different names*

```diff
@@ -67,70 +67,68 @@
             Similarity::Dot => protos::VectorSimilarity::Dot,
         }
     }
 }
 
 #[derive(Serialize, Deserialize, Default, Clone, Debug)]
 pub struct ShardMetadataFile {
-    pub kbid: Option<String>,
-    pub similarity: Option<Similarity>,
-    pub id: Option<String>,
-    #[serde(default)]
-    pub channel: Option<Channel>,
-    pub normalize_vectors: Option<bool>,
+    pub kbid: String,
+    pub id: String,
+    pub channel: Channel,
+    pub similarity: Similarity,
+    pub normalize_vectors: bool,
 }
 
 #[derive(Default, Debug)]
 pub struct ShardMetadata {
     shard_path: PathBuf,
     id: String,
-    kbid: Option<String>,
-    similarity: Option<Similarity>,
-    channel: Option<Channel>,
+    kbid: String,
+    similarity: Similarity,
+    channel: Channel,
     normalize_vectors: bool,
     // A generation id is a way to track if a shard has changed.
     // A new id means that something in the shard has changed.
     // This is used by replication to track which shards have changed
     // and to efficiently replicate them.
     generation_id: RwLock<Option<String>>,
 }
 
 impl ShardMetadata {
     pub fn open(shard_path: PathBuf) -> NodeResult<ShardMetadata> {
         let metadata_path = shard_path.join(disk_structure::METADATA_FILE);
         if !metadata_path.exists() {
             return Err(node_error!("Shard metadata file does not exist"));
         }
-        let requested_shard_id = shard_path.file_name().unwrap().to_str().unwrap().to_string();
 
         let mut reader = BufReader::new(File::open(metadata_path)?);
         let metadata: ShardMetadataFile = serde_json::from_reader(&mut reader)?;
         Ok(ShardMetadata {
             shard_path,
             kbid: metadata.kbid,
             similarity: metadata.similarity,
-            id: metadata.id.unwrap_or(requested_shard_id),
+            id: metadata.id,
             channel: metadata.channel,
-            normalize_vectors: metadata.normalize_vectors.unwrap_or(false),
+            normalize_vectors: metadata.normalize_vectors,
             generation_id: RwLock::new(None),
         })
     }
 
     pub fn new(
         shard_path: PathBuf,
         id: String,
-        kbid: Option<String>,
+        kbid: String,
         similarity: Similarity,
-        channel: Option<Channel>,
+        channel: Channel,
         normalize_vectors: bool,
     ) -> ShardMetadata {
         ShardMetadata {
             shard_path,
             kbid,
-            similarity: Some(similarity),
+            similarity,
             id,
             channel,
             normalize_vectors,
             generation_id: RwLock::new(None),
         }
     }
 
@@ -145,17 +143,17 @@
 
         let mut writer = BufWriter::new(File::create(temp_metadata_path.clone())?);
         serde_json::to_writer(
             &mut writer,
             &ShardMetadataFile {
                 kbid: self.kbid.clone(),
                 similarity: self.similarity,
-                id: Some(self.id.clone()),
+                id: self.id.clone(),
                 channel: self.channel,
-                normalize_vectors: Some(self.normalize_vectors),
+                normalize_vectors: self.normalize_vectors,
             },
         )?;
         writer.flush()?;
 
         std::fs::rename(temp_metadata_path, metadata_path)?;
 
         self.new_generation_id();
@@ -163,24 +161,24 @@
         Ok(())
     }
 
     pub fn shard_path(&self) -> PathBuf {
         self.shard_path.clone()
     }
 
-    pub fn kbid(&self) -> Option<String> {
+    pub fn kbid(&self) -> String {
         self.kbid.clone()
     }
 
     pub fn similarity(&self) -> protos::VectorSimilarity {
-        self.similarity.unwrap_or(Similarity::Cosine).into()
+        self.similarity.into()
     }
 
     pub fn channel(&self) -> Channel {
-        self.channel.unwrap_or_default()
+        self.channel
     }
 
     pub fn normalize_vectors(&self) -> bool {
         self.normalize_vectors
     }
 
     pub fn id(&self) -> String {
@@ -272,17 +270,17 @@
     use super::*;
     #[test]
     fn create() {
         let dir = TempDir::new().unwrap();
         let meta = ShardMetadata::new(
             dir.path().to_path_buf(),
             "ID".to_string(),
-            Some("KB".to_string()),
+            "KB".to_string(),
             Similarity::Cosine,
-            Some(Channel::EXPERIMENTAL),
+            Channel::EXPERIMENTAL,
             false,
         );
         meta.serialize_metadata().unwrap();
         let meta_disk = ShardMetadata::open(dir.path().to_path_buf()).unwrap();
         assert_eq!(meta.kbid, meta_disk.kbid);
         assert_eq!(meta.similarity, meta_disk.similarity);
         assert_eq!(meta.id, meta_disk.id);
@@ -314,17 +312,17 @@
 
     #[test]
     fn test_cache_generation_id() {
         let dir = TempDir::new().unwrap();
         let meta = ShardMetadata::new(
             dir.path().to_path_buf(),
             "ID".to_string(),
-            Some("KB".to_string()),
+            "KB".to_string(),
             Similarity::Cosine,
-            Some(Channel::EXPERIMENTAL),
+            Channel::EXPERIMENTAL,
             false,
         );
         let gen_id = meta.get_generation_id();
         assert_eq!(gen_id, meta.get_generation_id());
         // assert!(meta.generation_id.read().unwrap().is_none());
         // let gen_id = meta.get_generation_id();
         // assert_eq!(
```

### Comparing `nucliadb_node_binding-3.0.3.post1215/local_dependencies/nucliadb_node/src/shards/mod.rs` & `nucliadb_node_binding-3.0.3.post1216/local_dependencies/nucliadb_node/src/shards/mod.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.0.3.post1215/local_dependencies/nucliadb_node/src/shards/shard_reader.rs` & `nucliadb_node_binding-3.0.3.post1216/local_dependencies/nucliadb_node/src/shards/shard_reader.rs`

 * *Files 1% similar despite different names*

```diff
@@ -216,15 +216,15 @@
             s.spawn(|_| paragraph_result = paragraph_task());
             s.spawn(|_| vector_result = vector_task());
         })
         .expect("Failed to join threads");
 
         Ok(Shard {
             metadata: Some(protos::ShardMetadata {
-                kbid: self.metadata.kbid().unwrap_or_default(),
+                kbid: self.metadata.kbid(),
                 release_channel: self.metadata.channel() as i32,
             }),
             shard_id: self.id.clone(),
             // naming issue here, this is not number of resource
             // but more like number of fields
             fields: text_result? as u64,
             paragraphs: paragraph_result? as u64,
```

### Comparing `nucliadb_node_binding-3.0.3.post1215/local_dependencies/nucliadb_node/src/shards/shard_writer.rs` & `nucliadb_node_binding-3.0.3.post1216/local_dependencies/nucliadb_node/src/shards/shard_writer.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.0.3.post1215/local_dependencies/nucliadb_node/src/shards/versioning.rs` & `nucliadb_node_binding-3.0.3.post1216/local_dependencies/nucliadb_node/src/shards/versioning.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.0.3.post1215/local_dependencies/nucliadb_node/src/telemetry.rs` & `nucliadb_node_binding-3.0.3.post1216/local_dependencies/nucliadb_node/src/telemetry.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.0.3.post1215/local_dependencies/nucliadb_node/src/utils.rs` & `nucliadb_node_binding-3.0.3.post1216/local_dependencies/nucliadb_node/src/utils.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.0.3.post1215/local_dependencies/nucliadb_node/tests/common/mod.rs` & `nucliadb_node_binding-3.0.3.post1216/local_dependencies/nucliadb_node/tests/common/mod.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.0.3.post1215/local_dependencies/nucliadb_node/tests/common/node_services.rs` & `nucliadb_node_binding-3.0.3.post1216/local_dependencies/nucliadb_node/tests/common/node_services.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.0.3.post1215/local_dependencies/nucliadb_node/tests/common/resources.rs` & `nucliadb_node_binding-3.0.3.post1216/local_dependencies/nucliadb_node/tests/common/resources.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.0.3.post1215/local_dependencies/nucliadb_node/tests/test_date_range_search.rs` & `nucliadb_node_binding-3.0.3.post1216/local_dependencies/nucliadb_node/tests/test_date_range_search.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.0.3.post1215/local_dependencies/nucliadb_node/tests/test_download.rs` & `nucliadb_node_binding-3.0.3.post1216/local_dependencies/nucliadb_node/tests/test_download.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.0.3.post1215/local_dependencies/nucliadb_node/tests/test_merge.rs` & `nucliadb_node_binding-3.0.3.post1216/local_dependencies/nucliadb_node/tests/test_merge.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.0.3.post1215/local_dependencies/nucliadb_node/tests/test_replication.rs` & `nucliadb_node_binding-3.0.3.post1216/local_dependencies/nucliadb_node/tests/test_replication.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.0.3.post1215/local_dependencies/nucliadb_node/tests/test_search_relations.rs` & `nucliadb_node_binding-3.0.3.post1216/local_dependencies/nucliadb_node/tests/test_search_relations.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.0.3.post1215/local_dependencies/nucliadb_node/tests/test_search_sorting.rs` & `nucliadb_node_binding-3.0.3.post1216/local_dependencies/nucliadb_node/tests/test_search_sorting.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.0.3.post1215/local_dependencies/nucliadb_node/tests/test_security_search.rs` & `nucliadb_node_binding-3.0.3.post1216/local_dependencies/nucliadb_node/tests/test_security_search.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.0.3.post1215/local_dependencies/nucliadb_node/tests/test_shards.rs` & `nucliadb_node_binding-3.0.3.post1216/local_dependencies/nucliadb_node/tests/test_shards.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.0.3.post1215/local_dependencies/nucliadb_node/tests/test_suggest.rs` & `nucliadb_node_binding-3.0.3.post1216/local_dependencies/nucliadb_node/tests/test_suggest.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.0.3.post1215/local_dependencies/nucliadb_node/tests/test_vector_normalization.rs` & `nucliadb_node_binding-3.0.3.post1216/local_dependencies/nucliadb_node/tests/test_vector_normalization.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.0.3.post1215/local_dependencies/nucliadb_protos/build.rs` & `nucliadb_node_binding-3.0.3.post1216/local_dependencies/nucliadb_protos/build.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.0.3.post1215/local_dependencies/nucliadb_protos/src/fdbwriter.rs` & `nucliadb_node_binding-3.0.3.post1216/local_dependencies/nucliadb_protos/src/fdbwriter.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.0.3.post1215/local_dependencies/nucliadb_protos/src/knowledgebox.rs` & `nucliadb_node_binding-3.0.3.post1216/local_dependencies/nucliadb_protos/src/knowledgebox.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.0.3.post1215/local_dependencies/nucliadb_protos/src/lib.rs` & `nucliadb_node_binding-3.0.3.post1216/local_dependencies/nucliadb_protos/src/lib.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.0.3.post1215/local_dependencies/nucliadb_protos/src/nodereader.rs` & `nucliadb_node_binding-3.0.3.post1216/local_dependencies/nucliadb_protos/src/nodereader.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.0.3.post1215/local_dependencies/nucliadb_protos/src/noderesources.rs` & `nucliadb_node_binding-3.0.3.post1216/local_dependencies/nucliadb_protos/src/noderesources.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.0.3.post1215/local_dependencies/nucliadb_protos/src/nodewriter.rs` & `nucliadb_node_binding-3.0.3.post1216/local_dependencies/nucliadb_protos/src/nodewriter.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.0.3.post1215/local_dependencies/nucliadb_protos/src/replication.rs` & `nucliadb_node_binding-3.0.3.post1216/local_dependencies/nucliadb_protos/src/replication.rs`

 * *Files 1% similar despite different names*

```diff
@@ -8,14 +8,16 @@
     pub generation_id: ::prost::alloc::string::String,
     #[prost(string, tag="3")]
     pub kbid: ::prost::alloc::string::String,
     #[prost(string, tag="4")]
     pub similarity: ::prost::alloc::string::String,
     #[prost(bool, tag="5")]
     pub normalize_vectors: bool,
+    #[prost(enumeration="super::utils::ReleaseChannel", tag="6")]
+    pub release_channel: i32,
 }
 #[derive(Clone, PartialEq, ::prost::Message)]
 pub struct SecondaryShardReplicationState {
     #[prost(string, tag="1")]
     pub shard_id: ::prost::alloc::string::String,
     /// ID to identify the generation of the shard to know
     /// if there is a new version of the shard available to download
```

### Comparing `nucliadb_node_binding-3.0.3.post1215/local_dependencies/nucliadb_protos/src/resources.rs` & `nucliadb_node_binding-3.0.3.post1216/local_dependencies/nucliadb_protos/src/resources.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.0.3.post1215/local_dependencies/nucliadb_protos/src/utils.rs` & `nucliadb_node_binding-3.0.3.post1216/local_dependencies/nucliadb_protos/src/utils.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.0.3.post1215/local_dependencies/nucliadb_relations2/Cargo.toml` & `nucliadb_node_binding-3.0.3.post1216/local_dependencies/nucliadb_relations2/Cargo.toml`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.0.3.post1215/local_dependencies/nucliadb_relations2/src/io_maps.rs` & `nucliadb_node_binding-3.0.3.post1216/local_dependencies/nucliadb_relations2/src/io_maps.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.0.3.post1215/local_dependencies/nucliadb_relations2/src/lib.rs` & `nucliadb_node_binding-3.0.3.post1216/local_dependencies/nucliadb_relations2/src/lib.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.0.3.post1215/local_dependencies/nucliadb_relations2/src/reader.rs` & `nucliadb_node_binding-3.0.3.post1216/local_dependencies/nucliadb_relations2/src/reader.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.0.3.post1215/local_dependencies/nucliadb_relations2/src/schema.rs` & `nucliadb_node_binding-3.0.3.post1216/local_dependencies/nucliadb_relations2/src/schema.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.0.3.post1215/local_dependencies/nucliadb_relations2/src/writer.rs` & `nucliadb_node_binding-3.0.3.post1216/local_dependencies/nucliadb_relations2/src/writer.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.0.3.post1215/local_dependencies/nucliadb_relations2/tests/common/mod.rs` & `nucliadb_node_binding-3.0.3.post1216/local_dependencies/nucliadb_relations2/tests/common/mod.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.0.3.post1215/local_dependencies/nucliadb_relations2/tests/test_reader.rs` & `nucliadb_node_binding-3.0.3.post1216/local_dependencies/nucliadb_relations2/tests/test_reader.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.0.3.post1215/local_dependencies/nucliadb_relations2/tests/test_writer.rs` & `nucliadb_node_binding-3.0.3.post1216/local_dependencies/nucliadb_relations2/tests/test_writer.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.0.3.post1215/Cargo.toml` & `nucliadb_node_binding-3.0.3.post1216/Cargo.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [package]
 name = "nucliadb_node_binding"
-version = "3.0.3-post1215"
+version = "3.0.3-post1216"
 edition = "2021"
 
 # See more keys and their definitions at https://doc.rust-lang.org/cargo/reference/manifest.html
 [lib]
 name = "nucliadb_node_binding"
 crate-type = ["cdylib"]
```

### Comparing `nucliadb_node_binding-3.0.3.post1215/CHANGELOG.md` & `nucliadb_node_binding-3.0.3.post1216/CHANGELOG.md`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.0.3.post1215/Makefile` & `nucliadb_node_binding-3.0.3.post1216/Makefile`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.0.3.post1215/cov.sh` & `nucliadb_node_binding-3.0.3.post1216/cov.sh`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.0.3.post1215/pyproject.toml` & `nucliadb_node_binding-3.0.3.post1216/pyproject.toml`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.0.3.post1215/src/collect_garbage.rs` & `nucliadb_node_binding-3.0.3.post1216/src/collect_garbage.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.0.3.post1215/src/errors.rs` & `nucliadb_node_binding-3.0.3.post1216/src/errors.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.0.3.post1215/src/lib.rs` & `nucliadb_node_binding-3.0.3.post1216/src/lib.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.0.3.post1215/src/reader.rs` & `nucliadb_node_binding-3.0.3.post1216/src/reader.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.0.3.post1215/src/update.rs` & `nucliadb_node_binding-3.0.3.post1216/src/update.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.0.3.post1215/src/writer.rs` & `nucliadb_node_binding-3.0.3.post1216/src/writer.rs`

 * *Files 0% similar despite different names*

```diff
@@ -96,17 +96,17 @@
 
         let request = NewShardRequest::decode(&mut Cursor::new(metadata)).expect("Error decoding arguments");
         let shard_id = uuid::Uuid::new_v4().to_string();
         let similarity = VectorSimilarity::from_i32(request.similarity).unwrap();
         let metadata = ShardMetadata::new(
             self.shards_path.join(shard_id.clone()),
             shard_id,
-            Some(request.kbid),
+            request.kbid,
             similarity.into(),
-            Some(Channel::from(request.release_channel)),
+            Channel::from(request.release_channel),
             request.normalize_vectors,
         );
         let new_shard = self.shards.create(metadata);
         match new_shard {
             Ok(new_shard) => Ok(PyList::new(
                 py,
                 ShardCreated {
```

### Comparing `nucliadb_node_binding-3.0.3.post1215/tests/__init__.py` & `nucliadb_node_binding-3.0.3.post1216/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.0.3.post1215/tests/conftest.py` & `nucliadb_node_binding-3.0.3.post1216/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.0.3.post1215/tests/integration/test_indexing.py` & `nucliadb_node_binding-3.0.3.post1216/tests/integration/test_indexing.py`

 * *Files identical despite different names*

