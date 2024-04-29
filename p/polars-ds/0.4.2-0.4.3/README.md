# Comparing `tmp/polars_ds-0.4.2.tar.gz` & `tmp/polars_ds-0.4.3.tar.gz`

## Comparing `polars_ds-0.4.2.tar` & `polars_ds-0.4.3.tar`

### file list

```diff
@@ -1,98 +1,99 @@
--rw-r--r--   0        0        0     1451 1970-01-01 00:00:00.000000 polars_ds-0.4.2/Cargo.toml
--rw-r--r--   0     1001      127     4742 2024-04-19 02:51:18.000000 polars_ds-0.4.2/.github/workflows/CI.yml
--rw-r--r--   0     1001      127      897 2024-04-19 02:51:18.000000 polars_ds-0.4.2/.gitignore
--rw-r--r--   0     1001      127      268 2024-04-19 02:51:18.000000 polars_ds-0.4.2/.pre-commit-config.yaml
--rw-r--r--   0     1001      127      442 2024-04-19 02:51:18.000000 polars_ds-0.4.2/.readthedocs.yaml
--rw-r--r--   0     1001      127     2312 2024-04-19 02:51:18.000000 polars_ds-0.4.2/CONTRIBUTING.md
--rw-r--r--   0     1001      127     1063 2024-04-19 02:51:18.000000 polars_ds-0.4.2/LICENSE.txt
--rw-r--r--   0     1001      127      715 2024-04-19 02:51:18.000000 polars_ds-0.4.2/Makefile
--rw-r--r--   0     1001      127     8927 2024-04-19 02:51:18.000000 polars_ds-0.4.2/README.md
--rw-r--r--   0     1001      127       55 2024-04-19 02:51:18.000000 polars_ds-0.4.2/docs/complex.md
--rw-r--r--   0     1001      127       58 2024-04-19 02:51:18.000000 polars_ds-0.4.2/docs/graph.md
--rw-r--r--   0     1001      127     8531 2024-04-19 02:51:18.000000 polars_ds-0.4.2/docs/index.md
--rw-r--r--   0     1001      127       57 2024-04-19 02:51:18.000000 polars_ds-0.4.2/docs/metrics.md
--rw-r--r--   0     1001      127       81 2024-04-19 02:51:18.000000 polars_ds-0.4.2/docs/num.md
--rw-r--r--   0     1001      127      144 2024-04-19 02:51:18.000000 polars_ds-0.4.2/docs/polars_ds.md
--rw-r--r--   0     1001      127      123 2024-04-19 02:51:18.000000 polars_ds-0.4.2/docs/requirements-docs.txt
--rw-r--r--   0     1001      127       67 2024-04-19 02:51:18.000000 polars_ds-0.4.2/docs/stats.md
--rw-r--r--   0     1001      127       68 2024-04-19 02:51:18.000000 polars_ds-0.4.2/docs/str2.md
--rw-r--r--   0     1001      127   125731 2024-04-19 02:51:18.000000 polars_ds-0.4.2/examples/basics.ipynb
--rw-r--r--   0     1001      127  1764254 2024-04-19 02:51:18.000000 polars_ds-0.4.2/examples/dependency.parquet
--rw-r--r--   0     1001      127   386350 2024-04-19 02:51:18.000000 polars_ds-0.4.2/examples/diagnosis.ipynb
--rw-r--r--   0     1001      127    31063 2024-04-19 02:51:18.000000 polars_ds-0.4.2/examples/sample_and_split.ipynb
--rw-r--r--   0     1001      127      609 2024-04-19 02:51:18.000000 polars_ds-0.4.2/mkdocs.yml
--rw-r--r--   0     1001      127     3230 2024-04-19 02:51:18.000000 polars_ds-0.4.2/python/polars_ds/__init__.py
--rw-r--r--   0     1001      127     1243 2024-04-19 02:51:18.000000 polars_ds-0.4.2/python/polars_ds/_utils.py
--rw-r--r--   0     1001      127     7324 2024-04-19 02:51:18.000000 polars_ds-0.4.2/python/polars_ds/complex.py
--rw-r--r--   0     1001      127    20305 2024-04-19 02:51:18.000000 polars_ds-0.4.2/python/polars_ds/diagnosis.py
--rw-r--r--   0     1001      127     7188 2024-04-19 02:51:18.000000 polars_ds-0.4.2/python/polars_ds/graph.py
--rw-r--r--   0     1001      127    13270 2024-04-19 02:51:18.000000 polars_ds-0.4.2/python/polars_ds/metrics.py
--rw-r--r--   0     1001      127    49302 2024-04-19 02:51:18.000000 polars_ds-0.4.2/python/polars_ds/num.py
--rw-r--r--   0     1001      127     6080 2024-04-19 02:51:18.000000 polars_ds-0.4.2/python/polars_ds/sample.py
--rw-r--r--   0     1001      127    30893 2024-04-19 02:51:18.000000 polars_ds-0.4.2/python/polars_ds/stats.py
--rw-r--r--   0     1001      127    31957 2024-04-19 02:51:18.000000 polars_ds-0.4.2/python/polars_ds/str2.py
--rw-r--r--   0     1001      127     1133 2024-04-19 02:51:18.000000 polars_ds-0.4.2/python/polars_ds/type_alias.py
--rw-r--r--   0     1001      127       83 2024-04-19 02:51:18.000000 polars_ds-0.4.2/requirements.txt
--rw-r--r--   0     1001      127       42 2024-04-19 02:51:18.000000 polars_ds-0.4.2/rust-toolchain.toml
--rw-r--r--   0     1001      127     2089 2024-04-19 02:51:18.000000 polars_ds-0.4.2/src/graph/degree.rs
--rw-r--r--   0     1001      127     4158 2024-04-19 02:51:18.000000 polars_ds-0.4.2/src/graph/eigen_centrality.rs
--rw-r--r--   0     1001      127     3146 2024-04-19 02:51:18.000000 polars_ds-0.4.2/src/graph/mod.rs
--rw-r--r--   0     1001      127     8711 2024-04-19 02:51:18.000000 polars_ds-0.4.2/src/graph/shortest_path.rs
--rw-r--r--   0     1001      127      430 2024-04-19 02:51:18.000000 polars_ds-0.4.2/src/lib.rs
--rw-r--r--   0     1001      127      967 2024-04-19 02:51:18.000000 polars_ds-0.4.2/src/num/cond_entropy.rs
--rw-r--r--   0     1001      127     4186 2024-04-19 02:51:18.000000 polars_ds-0.4.2/src/num/convolve.rs
--rw-r--r--   0     1001      127     7150 2024-04-19 02:51:18.000000 polars_ds-0.4.2/src/num/entrophies.rs
--rw-r--r--   0     1001      127     2536 2024-04-19 02:51:18.000000 polars_ds-0.4.2/src/num/fft.rs
--rw-r--r--   0     1001      127     9462 2024-04-19 02:51:18.000000 polars_ds-0.4.2/src/num/float_extras.rs
--rw-r--r--   0     1001      127     1383 2024-04-19 02:51:18.000000 polars_ds-0.4.2/src/num/gcd_lcm.rs
--rw-r--r--   0     1001      127     2734 2024-04-19 02:51:18.000000 polars_ds-0.4.2/src/num/haversine.rs
--rw-r--r--   0     1001      127     8843 2024-04-19 02:51:18.000000 polars_ds-0.4.2/src/num/jaccard.rs
--rw-r--r--   0     1001      127    18850 2024-04-19 02:51:18.000000 polars_ds-0.4.2/src/num/knn.rs
--rw-r--r--   0     1001      127      808 2024-04-19 02:51:18.000000 polars_ds-0.4.2/src/num/lempel_ziv.rs
--rw-r--r--   0     1001      127     3126 2024-04-19 02:51:18.000000 polars_ds-0.4.2/src/num/mod.rs
--rw-r--r--   0     1001      127     9656 2024-04-19 02:51:18.000000 polars_ds-0.4.2/src/num/ols.rs
--rw-r--r--   0     1001      127     5714 2024-04-19 02:51:18.000000 polars_ds-0.4.2/src/num/pca.rs
--rw-r--r--   0     1001      127     3707 2024-04-19 02:51:18.000000 polars_ds-0.4.2/src/num/psi.rs
--rw-r--r--   0     1001      127     2064 2024-04-19 02:51:18.000000 polars_ds-0.4.2/src/num/target_encode.rs
--rw-r--r--   0     1001      127     5764 2024-04-19 02:51:18.000000 polars_ds-0.4.2/src/num/tp_fp.rs
--rw-r--r--   0     1001      127     1422 2024-04-19 02:51:18.000000 polars_ds-0.4.2/src/num/trapz.rs
--rw-r--r--   0     1001      127     2659 2024-04-19 02:51:18.000000 polars_ds-0.4.2/src/num/woe_iv.rs
--rw-r--r--   0     1001      127     2251 2024-04-19 02:51:18.000000 polars_ds-0.4.2/src/stats/chi2.rs
--rw-r--r--   0     1001      127     3630 2024-04-19 02:51:18.000000 polars_ds-0.4.2/src/stats/fstats.rs
--rw-r--r--   0     1001      127     2817 2024-04-19 02:51:18.000000 polars_ds-0.4.2/src/stats/ks.rs
--rw-r--r--   0     1001      127     1111 2024-04-19 02:51:18.000000 polars_ds-0.4.2/src/stats/mod.rs
--rw-r--r--   0     1001      127     3383 2024-04-19 02:51:18.000000 polars_ds-0.4.2/src/stats/normal_test.rs
--rw-r--r--   0     1001      127    15502 2024-04-19 02:51:18.000000 polars_ds-0.4.2/src/stats/sample.rs
--rw-r--r--   0     1001      127     6054 2024-04-19 02:51:18.000000 polars_ds-0.4.2/src/stats/t_test.rs
--rw-r--r--   0     1001      127     1594 2024-04-19 02:51:18.000000 polars_ds-0.4.2/src/stats/xi_corr.rs
--rw-r--r--   0     1001      127     4235 2024-04-19 02:51:18.000000 polars_ds-0.4.2/src/stats_utils/beta.rs
--rw-r--r--   0     1001      127     6734 2024-04-19 02:51:18.000000 polars_ds-0.4.2/src/stats_utils/gamma.rs
--rw-r--r--   0     1001      127      895 2024-04-19 02:51:18.000000 polars_ds-0.4.2/src/stats_utils/mod.rs
--rw-r--r--   0     1001      127    18992 2024-04-19 02:51:18.000000 polars_ds-0.4.2/src/stats_utils/normal.rs
--rw-r--r--   0     1001      127     2221 2024-04-19 02:51:18.000000 polars_ds-0.4.2/src/str2/consts.rs
--rw-r--r--   0     1001      127     3082 2024-04-19 02:51:18.000000 polars_ds-0.4.2/src/str2/fuzz.rs
--rw-r--r--   0     1001      127    11287 2024-04-19 02:51:18.000000 polars_ds-0.4.2/src/str2/hamming.rs
--rw-r--r--   0     1001      127     1066 2024-04-19 02:51:18.000000 polars_ds-0.4.2/src/str2/inflections.rs
--rw-r--r--   0     1001      127      483 2024-04-19 02:51:18.000000 polars_ds-0.4.2/src/str2/is_stopword.rs
--rw-r--r--   0     1001      127     5723 2024-04-19 02:51:18.000000 polars_ds-0.4.2/src/str2/jaro.rs
--rw-r--r--   0     1001      127     7937 2024-04-19 02:51:18.000000 polars_ds-0.4.2/src/str2/knn_strs.rs
--rw-r--r--   0     1001      127    13628 2024-04-19 02:51:18.000000 polars_ds-0.4.2/src/str2/levenshtein.rs
--rw-r--r--   0     1001      127     1159 2024-04-19 02:51:18.000000 polars_ds-0.4.2/src/str2/mod.rs
--rw-r--r--   0     1001      127     5731 2024-04-19 02:51:18.000000 polars_ds-0.4.2/src/str2/osa.rs
--rw-r--r--   0     1001      127     3051 2024-04-19 02:51:18.000000 polars_ds-0.4.2/src/str2/overlap.rs
--rw-r--r--   0     1001      127    24197 2024-04-19 02:51:18.000000 polars_ds-0.4.2/src/str2/snowball/algorithms/english_stemmer.rs
--rw-r--r--   0     1001      127      110 2024-04-19 02:51:18.000000 polars_ds-0.4.2/src/str2/snowball/algorithms/mod.rs
--rw-r--r--   0     1001      127      198 2024-04-19 02:51:18.000000 polars_ds-0.4.2/src/str2/snowball/among.rs
--rw-r--r--   0     1001      127     1371 2024-04-19 02:51:18.000000 polars_ds-0.4.2/src/str2/snowball/mod.rs
--rw-r--r--   0     1001      127    12885 2024-04-19 02:51:18.000000 polars_ds-0.4.2/src/str2/snowball/snowball_env.rs
--rw-r--r--   0     1001      127      870 2024-04-19 02:51:18.000000 polars_ds-0.4.2/src/str2/snowball_stem.rs
--rw-r--r--   0     1001      127     3059 2024-04-19 02:51:18.000000 polars_ds-0.4.2/src/str2/sorensen_dice.rs
--rw-r--r--   0     1001      127     3050 2024-04-19 02:51:18.000000 polars_ds-0.4.2/src/str2/str_jaccard.rs
--rw-r--r--   0     1001      127     3461 2024-04-19 02:51:18.000000 polars_ds-0.4.2/src/str2/tversky.rs
--rw-r--r--   0     1001      127     2447 2024-04-19 02:51:18.000000 polars_ds-0.4.2/src/utils/mod.rs
--rw-r--r--   0     1001      127      121 2024-04-19 02:51:18.000000 polars_ds-0.4.2/tests/requirements-test.txt
--rw-r--r--   0     1001      127     2685 2024-04-19 02:51:18.000000 polars_ds-0.4.2/tests/test.ipynb
--rw-r--r--   0     1001      127    39271 2024-04-19 02:51:18.000000 polars_ds-0.4.2/tests/test_correctness.py
--rw-r--r--   0     1001      127    73361 2024-04-19 02:51:18.000000 polars_ds-0.4.2/Cargo.lock
--rw-r--r--   0     1001      127     1050 2024-04-19 02:51:18.000000 polars_ds-0.4.2/pyproject.toml
--rw-r--r--   0        0        0     9693 1970-01-01 00:00:00.000000 polars_ds-0.4.2/PKG-INFO
+-rw-r--r--   0        0        0     1451 1970-01-01 00:00:00.000000 polars_ds-0.4.3/Cargo.toml
+-rw-r--r--   0     1001      127     4764 2024-04-28 23:44:00.000000 polars_ds-0.4.3/.github/workflows/CI.yml
+-rw-r--r--   0     1001      127      897 2024-04-28 23:44:00.000000 polars_ds-0.4.3/.gitignore
+-rw-r--r--   0     1001      127      268 2024-04-28 23:44:00.000000 polars_ds-0.4.3/.pre-commit-config.yaml
+-rw-r--r--   0     1001      127      442 2024-04-28 23:44:00.000000 polars_ds-0.4.3/.readthedocs.yaml
+-rw-r--r--   0     1001      127     2312 2024-04-28 23:44:00.000000 polars_ds-0.4.3/CONTRIBUTING.md
+-rw-r--r--   0     1001      127     1063 2024-04-28 23:44:00.000000 polars_ds-0.4.3/LICENSE.txt
+-rw-r--r--   0     1001      127      715 2024-04-28 23:44:00.000000 polars_ds-0.4.3/Makefile
+-rw-r--r--   0     1001      127     9792 2024-04-28 23:44:00.000000 polars_ds-0.4.3/README.md
+-rw-r--r--   0     1001      127       55 2024-04-28 23:44:00.000000 polars_ds-0.4.3/docs/complex.md
+-rw-r--r--   0     1001      127       58 2024-04-28 23:44:00.000000 polars_ds-0.4.3/docs/graph.md
+-rw-r--r--   0     1001      127     9596 2024-04-28 23:44:00.000000 polars_ds-0.4.3/docs/index.md
+-rw-r--r--   0     1001      127       57 2024-04-28 23:44:00.000000 polars_ds-0.4.3/docs/metrics.md
+-rw-r--r--   0     1001      127       81 2024-04-28 23:44:00.000000 polars_ds-0.4.3/docs/num.md
+-rw-r--r--   0     1001      127      144 2024-04-28 23:44:00.000000 polars_ds-0.4.3/docs/polars_ds.md
+-rw-r--r--   0     1001      127      123 2024-04-28 23:44:00.000000 polars_ds-0.4.3/docs/requirements-docs.txt
+-rw-r--r--   0     1001      127       67 2024-04-28 23:44:00.000000 polars_ds-0.4.3/docs/stats.md
+-rw-r--r--   0     1001      127       68 2024-04-28 23:44:00.000000 polars_ds-0.4.3/docs/str2.md
+-rw-r--r--   0     1001      127   125841 2024-04-28 23:44:00.000000 polars_ds-0.4.3/examples/basics.ipynb
+-rw-r--r--   0     1001      127  1764254 2024-04-28 23:44:00.000000 polars_ds-0.4.3/examples/dependency.parquet
+-rw-r--r--   0     1001      127   718268 2024-04-28 23:44:00.000000 polars_ds-0.4.3/examples/diagnosis.ipynb
+-rw-r--r--   0     1001      127    31063 2024-04-28 23:44:00.000000 polars_ds-0.4.3/examples/sample_and_split.ipynb
+-rw-r--r--   0     1001      127      609 2024-04-28 23:44:00.000000 polars_ds-0.4.3/mkdocs.yml
+-rw-r--r--   0     1001      127     3230 2024-04-28 23:44:00.000000 polars_ds-0.4.3/python/polars_ds/__init__.py
+-rw-r--r--   0     1001      127     1243 2024-04-28 23:44:00.000000 polars_ds-0.4.3/python/polars_ds/_utils.py
+-rw-r--r--   0     1001      127     7324 2024-04-28 23:44:00.000000 polars_ds-0.4.3/python/polars_ds/complex.py
+-rw-r--r--   0     1001      127    26784 2024-04-28 23:44:00.000000 polars_ds-0.4.3/python/polars_ds/diagnosis.py
+-rw-r--r--   0     1001      127     7188 2024-04-28 23:44:00.000000 polars_ds-0.4.3/python/polars_ds/graph.py
+-rw-r--r--   0     1001      127    13270 2024-04-28 23:44:00.000000 polars_ds-0.4.3/python/polars_ds/metrics.py
+-rw-r--r--   0     1001      127    50144 2024-04-28 23:44:00.000000 polars_ds-0.4.3/python/polars_ds/num.py
+-rw-r--r--   0     1001      127     6080 2024-04-28 23:44:00.000000 polars_ds-0.4.3/python/polars_ds/sample.py
+-rw-r--r--   0     1001      127    32460 2024-04-28 23:44:00.000000 polars_ds-0.4.3/python/polars_ds/stats.py
+-rw-r--r--   0     1001      127    31957 2024-04-28 23:44:00.000000 polars_ds-0.4.3/python/polars_ds/str2.py
+-rw-r--r--   0     1001      127     1256 2024-04-28 23:44:00.000000 polars_ds-0.4.3/python/polars_ds/type_alias.py
+-rw-r--r--   0     1001      127       83 2024-04-28 23:44:00.000000 polars_ds-0.4.3/requirements.txt
+-rw-r--r--   0     1001      127       42 2024-04-28 23:44:00.000000 polars_ds-0.4.3/rust-toolchain.toml
+-rw-r--r--   0     1001      127     2089 2024-04-28 23:44:00.000000 polars_ds-0.4.3/src/graph/degree.rs
+-rw-r--r--   0     1001      127     4158 2024-04-28 23:44:00.000000 polars_ds-0.4.3/src/graph/eigen_centrality.rs
+-rw-r--r--   0     1001      127     3146 2024-04-28 23:44:00.000000 polars_ds-0.4.3/src/graph/mod.rs
+-rw-r--r--   0     1001      127     8711 2024-04-28 23:44:00.000000 polars_ds-0.4.3/src/graph/shortest_path.rs
+-rw-r--r--   0     1001      127      430 2024-04-28 23:44:00.000000 polars_ds-0.4.3/src/lib.rs
+-rw-r--r--   0     1001      127      967 2024-04-28 23:44:00.000000 polars_ds-0.4.3/src/num/cond_entropy.rs
+-rw-r--r--   0     1001      127     6279 2024-04-28 23:44:00.000000 polars_ds-0.4.3/src/num/convolve.rs
+-rw-r--r--   0     1001      127     7150 2024-04-28 23:44:00.000000 polars_ds-0.4.3/src/num/entrophies.rs
+-rw-r--r--   0     1001      127     2536 2024-04-28 23:44:00.000000 polars_ds-0.4.3/src/num/fft.rs
+-rw-r--r--   0     1001      127     9546 2024-04-28 23:44:00.000000 polars_ds-0.4.3/src/num/float_extras.rs
+-rw-r--r--   0     1001      127     1383 2024-04-28 23:44:00.000000 polars_ds-0.4.3/src/num/gcd_lcm.rs
+-rw-r--r--   0     1001      127     2734 2024-04-28 23:44:00.000000 polars_ds-0.4.3/src/num/haversine.rs
+-rw-r--r--   0     1001      127     8843 2024-04-28 23:44:00.000000 polars_ds-0.4.3/src/num/jaccard.rs
+-rw-r--r--   0     1001      127    18898 2024-04-28 23:44:00.000000 polars_ds-0.4.3/src/num/knn.rs
+-rw-r--r--   0     1001      127      808 2024-04-28 23:44:00.000000 polars_ds-0.4.3/src/num/lempel_ziv.rs
+-rw-r--r--   0     1001      127     3126 2024-04-28 23:44:00.000000 polars_ds-0.4.3/src/num/mod.rs
+-rw-r--r--   0     1001      127     9846 2024-04-28 23:44:00.000000 polars_ds-0.4.3/src/num/ols.rs
+-rw-r--r--   0     1001      127     5714 2024-04-28 23:44:00.000000 polars_ds-0.4.3/src/num/pca.rs
+-rw-r--r--   0     1001      127     3749 2024-04-28 23:44:00.000000 polars_ds-0.4.3/src/num/psi.rs
+-rw-r--r--   0     1001      127     2064 2024-04-28 23:44:00.000000 polars_ds-0.4.3/src/num/target_encode.rs
+-rw-r--r--   0     1001      127     5764 2024-04-28 23:44:00.000000 polars_ds-0.4.3/src/num/tp_fp.rs
+-rw-r--r--   0     1001      127     1422 2024-04-28 23:44:00.000000 polars_ds-0.4.3/src/num/trapz.rs
+-rw-r--r--   0     1001      127     2659 2024-04-28 23:44:00.000000 polars_ds-0.4.3/src/num/woe_iv.rs
+-rw-r--r--   0     1001      127     2251 2024-04-28 23:44:00.000000 polars_ds-0.4.3/src/stats/chi2.rs
+-rw-r--r--   0     1001      127     3630 2024-04-28 23:44:00.000000 polars_ds-0.4.3/src/stats/fstats.rs
+-rw-r--r--   0     1001      127     4289 2024-04-28 23:44:00.000000 polars_ds-0.4.3/src/stats/kendall_tau.rs
+-rw-r--r--   0     1001      127     2817 2024-04-28 23:44:00.000000 polars_ds-0.4.3/src/stats/ks.rs
+-rw-r--r--   0     1001      127     1128 2024-04-28 23:44:00.000000 polars_ds-0.4.3/src/stats/mod.rs
+-rw-r--r--   0     1001      127     3383 2024-04-28 23:44:00.000000 polars_ds-0.4.3/src/stats/normal_test.rs
+-rw-r--r--   0     1001      127    15502 2024-04-28 23:44:00.000000 polars_ds-0.4.3/src/stats/sample.rs
+-rw-r--r--   0     1001      127     6054 2024-04-28 23:44:00.000000 polars_ds-0.4.3/src/stats/t_test.rs
+-rw-r--r--   0     1001      127     1594 2024-04-28 23:44:00.000000 polars_ds-0.4.3/src/stats/xi_corr.rs
+-rw-r--r--   0     1001      127     4235 2024-04-28 23:44:00.000000 polars_ds-0.4.3/src/stats_utils/beta.rs
+-rw-r--r--   0     1001      127     6734 2024-04-28 23:44:00.000000 polars_ds-0.4.3/src/stats_utils/gamma.rs
+-rw-r--r--   0     1001      127      895 2024-04-28 23:44:00.000000 polars_ds-0.4.3/src/stats_utils/mod.rs
+-rw-r--r--   0     1001      127    18992 2024-04-28 23:44:00.000000 polars_ds-0.4.3/src/stats_utils/normal.rs
+-rw-r--r--   0     1001      127     2221 2024-04-28 23:44:00.000000 polars_ds-0.4.3/src/str2/consts.rs
+-rw-r--r--   0     1001      127     3082 2024-04-28 23:44:00.000000 polars_ds-0.4.3/src/str2/fuzz.rs
+-rw-r--r--   0     1001      127    11287 2024-04-28 23:44:00.000000 polars_ds-0.4.3/src/str2/hamming.rs
+-rw-r--r--   0     1001      127     1066 2024-04-28 23:44:00.000000 polars_ds-0.4.3/src/str2/inflections.rs
+-rw-r--r--   0     1001      127      483 2024-04-28 23:44:00.000000 polars_ds-0.4.3/src/str2/is_stopword.rs
+-rw-r--r--   0     1001      127     5723 2024-04-28 23:44:00.000000 polars_ds-0.4.3/src/str2/jaro.rs
+-rw-r--r--   0     1001      127     7937 2024-04-28 23:44:00.000000 polars_ds-0.4.3/src/str2/knn_strs.rs
+-rw-r--r--   0     1001      127    13628 2024-04-28 23:44:00.000000 polars_ds-0.4.3/src/str2/levenshtein.rs
+-rw-r--r--   0     1001      127     1159 2024-04-28 23:44:00.000000 polars_ds-0.4.3/src/str2/mod.rs
+-rw-r--r--   0     1001      127     5731 2024-04-28 23:44:00.000000 polars_ds-0.4.3/src/str2/osa.rs
+-rw-r--r--   0     1001      127     3051 2024-04-28 23:44:00.000000 polars_ds-0.4.3/src/str2/overlap.rs
+-rw-r--r--   0     1001      127    24197 2024-04-28 23:44:00.000000 polars_ds-0.4.3/src/str2/snowball/algorithms/english_stemmer.rs
+-rw-r--r--   0     1001      127      110 2024-04-28 23:44:00.000000 polars_ds-0.4.3/src/str2/snowball/algorithms/mod.rs
+-rw-r--r--   0     1001      127      198 2024-04-28 23:44:00.000000 polars_ds-0.4.3/src/str2/snowball/among.rs
+-rw-r--r--   0     1001      127     1371 2024-04-28 23:44:00.000000 polars_ds-0.4.3/src/str2/snowball/mod.rs
+-rw-r--r--   0     1001      127    12885 2024-04-28 23:44:00.000000 polars_ds-0.4.3/src/str2/snowball/snowball_env.rs
+-rw-r--r--   0     1001      127      870 2024-04-28 23:44:00.000000 polars_ds-0.4.3/src/str2/snowball_stem.rs
+-rw-r--r--   0     1001      127     3059 2024-04-28 23:44:00.000000 polars_ds-0.4.3/src/str2/sorensen_dice.rs
+-rw-r--r--   0     1001      127     3050 2024-04-28 23:44:00.000000 polars_ds-0.4.3/src/str2/str_jaccard.rs
+-rw-r--r--   0     1001      127     3461 2024-04-28 23:44:00.000000 polars_ds-0.4.3/src/str2/tversky.rs
+-rw-r--r--   0     1001      127     2447 2024-04-28 23:44:00.000000 polars_ds-0.4.3/src/utils/mod.rs
+-rw-r--r--   0     1001      127      121 2024-04-28 23:44:00.000000 polars_ds-0.4.3/tests/requirements-test.txt
+-rw-r--r--   0     1001      127     4463 2024-04-28 23:44:00.000000 polars_ds-0.4.3/tests/test.ipynb
+-rw-r--r--   0     1001      127    40942 2024-04-28 23:44:00.000000 polars_ds-0.4.3/tests/test_correctness.py
+-rw-r--r--   0     1001      127    73361 2024-04-28 23:44:00.000000 polars_ds-0.4.3/Cargo.lock
+-rw-r--r--   0     1001      127     1125 2024-04-28 23:44:00.000000 polars_ds-0.4.3/pyproject.toml
+-rw-r--r--   0        0        0    10560 1970-01-01 00:00:00.000000 polars_ds-0.4.3/PKG-INFO
```

### Comparing `polars_ds-0.4.2/Cargo.toml` & `polars_ds-0.4.3/Cargo.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [package]
 name = "polars_ds"
-version = "0.4.2"
+version = "0.4.3"
 edition = "2021"
 
 [lib]
 name = "_polars_ds"
 crate-type = ["cdylib"]
 
 # See more keys and their definitions at https://doc.rust-lang.org/cargo/reference/manifest.html
```

### Comparing `polars_ds-0.4.2/.github/workflows/CI.yml` & `polars_ds-0.4.3/.github/workflows/CI.yml`

 * *Files 15% similar despite different names*

```diff
@@ -14,14 +14,15 @@
         description: Commit SHA
         type: string
 
 defaults:
   run:
     shell: bash
 
+# Drop 3.8 once it reaches end of life
 env:
   PYTHON_VERSION: '3.8'
 
 jobs:
   create-sdist:
     runs-on: ubuntu-latest
     strategy:
@@ -70,15 +71,15 @@
   build-wheels:
     runs-on: ${{ matrix.os }}
     needs: [create-sdist]
     strategy:
       fail-fast: false
       matrix:
         package: [polars_ds]
-        os: [ubuntu-latest, macos-latest, windows-latest]
+        os: [ubuntu-latest, macos-13, windows-latest]
         architecture: [x86-64, aarch64]
         exclude:
           - os: windows-latest
             architecture: aarch64
 
     steps:
       - uses: actions/checkout@v4
@@ -90,15 +91,15 @@
         with:
           python-version: ${{ env.PYTHON_VERSION }}
 
       - name: Determine CPU features for x86-64
         id: features
         if: matrix.architecture == 'x86-64'
         env:
-          IS_MACOS: ${{ matrix.os == 'macos-latest' }}
+          IS_MACOS: ${{ matrix.os == 'macos-13' }}
         run: |
           if [[ "$IS_MACOS" = true ]]; then
             FEATURES=+sse3,+ssse3,+sse4.1,+sse4.2,+popcnt,+avx,+fma,+pclmulqdq
           else
             FEATURES=+sse3,+ssse3,+sse4.1,+sse4.2,+popcnt,+avx,+avx2,+fma,+bmi1,+bmi2,+lzcnt,+pclmulqdq
           fi
           echo "features=$FEATURES" >> $GITHUB_OUTPUT
@@ -109,15 +110,15 @@
           FEATURES: ${{ steps.features.outputs.features }}
         run: echo "RUSTFLAGS=-C target-feature=${{ steps.features.outputs.features }}" >> $GITHUB_ENV
 
       - name: Set Rust target for aarch64
         if: matrix.architecture == 'aarch64'
         id: target
         run: |
-          TARGET=${{ matrix.os == 'macos-latest' && 'aarch64-apple-darwin' || 'aarch64-unknown-linux-gnu'}}
+          TARGET=${{ matrix.os == 'macos-13' && 'aarch64-apple-darwin' || 'aarch64-unknown-linux-gnu'}}
           echo "target=$TARGET" >> $GITHUB_OUTPUT
 
       - name: Set jemalloc for aarch64 Linux
         if: matrix.architecture == 'aarch64' && matrix.os == 'ubuntu-latest'
         run: |
           echo "JEMALLOC_SYS_WITH_LG_PAGE=16" >> $GITHUB_ENV
 
@@ -143,15 +144,15 @@
       - name: Upload wheel
         uses: actions/upload-artifact@v4
         with:
           name: wheel-${{ matrix.package }}-${{ matrix.os }}-${{ matrix.architecture }}
           path: dist/*.whl
 
   release:
-    name: Test Release
+    name: Release
     runs-on: ubuntu-latest
     if: "startsWith(github.ref, 'refs/tags/')"
     needs: [build-wheels, create-sdist]
     permissions:
         id-token: write
     steps:
       - uses: actions/download-artifact@v4
```

### Comparing `polars_ds-0.4.2/.gitignore` & `polars_ds-0.4.3/.gitignore`

 * *Files identical despite different names*

### Comparing `polars_ds-0.4.2/CONTRIBUTING.md` & `polars_ds-0.4.3/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `polars_ds-0.4.2/LICENSE.txt` & `polars_ds-0.4.3/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `polars_ds-0.4.2/Makefile` & `polars_ds-0.4.3/Makefile`

 * *Files identical despite different names*

### Comparing `polars_ds-0.4.2/README.md` & `polars_ds-0.4.3/README.md`

 * *Files 14% similar despite different names*

```diff
@@ -11,27 +11,37 @@
   <a href="https://github.com/abstractqqq/polars_ds_extension/blob/main/CONTRIBUTING.md">Want to Contribute?</a>
 <br>
 <b>pip install polars-ds</b>
 </p>
 
 # The Project
 
-The goal of the project is to **reduce dependencies**, **improve code organization**, **simplify data pipelines** and overall **faciliate analysis of various kinds of tabular data** that a data scientist may encounter. It is a package built around your favorite **Polars dataframe**. Here are the current namespaces (Polars Extensions) provided by the package:
+The goal of the project is to **reduce dependencies**, **improve code organization**, **simplify data pipelines** and overall **faciliate analysis of various kinds of tabular data** that a data scientist may encounter. It is a package built around your favorite **Polars dataframe**. Here are some of the main areas of data science that is covered by the package:
 
-1. A numerical extension (num), which focuses on numerical quantities common in many fields of data analysis (credit modelling, time series, other well-known quantities, etc.), such as rfft, entropies, k-nearest-neighbors queries, Population Stability Index, Information Value, etc.
+1. Well-known numerical transform/quantities. E.g. fft, conditional entropy, singular values, basic linear regression related quantities, population stability index, weight of evidence, column-wise/row-wise jaccard similarity etc.
 
-2. A metrics extension (metric), which contains a lot of common error/loss functions, model evaluation metrics. This module is mostly designed to generate model performance monitoring data.
+2. Statistics. Basic tests such as the t-test, f-test, KS statistics. Miscallaneous functions like weighted correlation, Xi-correlation. In-dataframe random column generations, etc. 
 
-3. A str extension (str2), which focuses on str distances/similarities, and other commonly used string manipulation procedures.
+3. Metrics. ML metrics for common model performance reporting. E.g ROC AUC for binary/multiclass classification, logloss, r2, MAPE, etc.
 
-4. A stats extension (stats), which has common statistical tests such as t-test, chi2, and f-test, etc., and random sampling from a distribution, etc.
+4. KNN-related queries. E.g. filter to k-nearest neighbors to point, find indices of all neighbors within a certain distance, etc.
 
-5. A complex extension (c), which treats complex numbers as a column of array of size 2. Sometimes complex numbers are needed for processing FFT outputs.
+5. String metrics such as Levenshtein distance, Damure Levenshtein distance, other string distances, snowball stemming (English only), string Jaccard similarity, etc.
 
-6. A graph extension (graph) for very simple graph queries, such as shortest path queries, eigenvector centrality computations. More will be added. (Usable but limited. Will to be refactored/redesigned.)
+6. Diagnosis. This modules contains the DIA (Data Inspection Assitant) class, which can help you profile your data, visualize data in lower dimensions, detect functional dependencies, detect other common data quality issues like null rate or high correlation.
+
+7. Sample. Traditional dataset sampling. No time series sampling yet. This module provides functionalities such as stratified downsample, volume neutral random sampling, etc.
+
+8. Polars Native ML Pipeline. Planned but not started yet. The goal is to have a Polars native pipeline that can replace Scikit-learn's pipeline and provides all the benefits of Polars. All the basic transforms in Scikit-leran, categorical-encoders are planned. This can be super powerful together with Polars's expressions. (Basically, once you have expressions, you don't need to write custom transforms like col(A)/col(B), log transform, sqrt transform, linear/polynomial transforms, etc.)
+
+Some other areas that currently exist, but is de-prioritized:
+
+1. Complex number related queries.
+
+2. Graph related queries. (The various representations of "Graphs" in tabular dataframe makes it hard to have consistent backend handling of such data.)
 
 # But why? Why not use Sklearn? SciPy? NumPy?
 
 The goal of the package is to **facilitate** data processes and analysis that go beyond standard SQL queries, and to **reduce** the number of dependencies in your project. It incorproates parts of SciPy, NumPy, Scikit-learn, and NLP (NLTK), etc., and treats them as Polars queries so that they can be run in parallel, in group_by contexts, all for almost no extra engineering effort. 
 
 Let's see an example. Say we want to generate a model performance report. In our data, we have segments. We are not only interested in the ROC AUC of our model on the entire dataset, but we are also interested in the model's performance on different segments.
 
@@ -120,20 +130,20 @@
 **Performance and elegance - something that is quite rare in the Python world.**
 
 ## Getting Started
 
 ```python
 import polars_ds as pds
 ```
-when you want to access the namespaces provided by the package.
+
+To make full use of the Diagnosis module, do
 
 ```python
 pip install "polars_ds[plot]"
 ```
-for dataframe diagnosis related features.
 
 ## Examples
 
 See this for Polars Extensions: [notebook](./examples/basics.ipynb)
 
 See this for Native Polars DataFrame Explorative tools: [notebook](./examples/diagnosis.ipynb)
```

#### html2text {}

```diff
@@ -2,30 +2,42 @@
                                      ************
                _D_o_c_u_m_e_n_t_a_t_i_o_n | _U_s_e_r_ _G_u_i_d_e | _W_a_n_t_ _t_o_ _C_o_n_t_r_i_b_u_t_e_?
                              ppiipp iinnssttaallll ppoollaarrss--ddss
 # The Project The goal of the project is to **reduce dependencies**, **improve
 code organization**, **simplify data pipelines** and overall **faciliate
 analysis of various kinds of tabular data** that a data scientist may
 encounter. It is a package built around your favorite **Polars dataframe**.
-Here are the current namespaces (Polars Extensions) provided by the package: 1.
-A numerical extension (num), which focuses on numerical quantities common in
-many fields of data analysis (credit modelling, time series, other well-known
-quantities, etc.), such as rfft, entropies, k-nearest-neighbors queries,
-Population Stability Index, Information Value, etc. 2. A metrics extension
-(metric), which contains a lot of common error/loss functions, model evaluation
-metrics. This module is mostly designed to generate model performance
-monitoring data. 3. A str extension (str2), which focuses on str distances/
-similarities, and other commonly used string manipulation procedures. 4. A
-stats extension (stats), which has common statistical tests such as t-test,
-chi2, and f-test, etc., and random sampling from a distribution, etc. 5. A
-complex extension (c), which treats complex numbers as a column of array of
-size 2. Sometimes complex numbers are needed for processing FFT outputs. 6. A
-graph extension (graph) for very simple graph queries, such as shortest path
-queries, eigenvector centrality computations. More will be added. (Usable but
-limited. Will to be refactored/redesigned.) # But why? Why not use Sklearn?
+Here are some of the main areas of data science that is covered by the package:
+1. Well-known numerical transform/quantities. E.g. fft, conditional entropy,
+singular values, basic linear regression related quantities, population
+stability index, weight of evidence, column-wise/row-wise jaccard similarity
+etc. 2. Statistics. Basic tests such as the t-test, f-test, KS statistics.
+Miscallaneous functions like weighted correlation, Xi-correlation. In-dataframe
+random column generations, etc. 3. Metrics. ML metrics for common model
+performance reporting. E.g ROC AUC for binary/multiclass classification,
+logloss, r2, MAPE, etc. 4. KNN-related queries. E.g. filter to k-nearest
+neighbors to point, find indices of all neighbors within a certain distance,
+etc. 5. String metrics such as Levenshtein distance, Damure Levenshtein
+distance, other string distances, snowball stemming (English only), string
+Jaccard similarity, etc. 6. Diagnosis. This modules contains the DIA (Data
+Inspection Assitant) class, which can help you profile your data, visualize
+data in lower dimensions, detect functional dependencies, detect other common
+data quality issues like null rate or high correlation. 7. Sample. Traditional
+dataset sampling. No time series sampling yet. This module provides
+functionalities such as stratified downsample, volume neutral random sampling,
+etc. 8. Polars Native ML Pipeline. Planned but not started yet. The goal is to
+have a Polars native pipeline that can replace Scikit-learn's pipeline and
+provides all the benefits of Polars. All the basic transforms in Scikit-leran,
+categorical-encoders are planned. This can be super powerful together with
+Polars's expressions. (Basically, once you have expressions, you don't need to
+write custom transforms like col(A)/col(B), log transform, sqrt transform,
+linear/polynomial transforms, etc.) Some other areas that currently exist, but
+is de-prioritized: 1. Complex number related queries. 2. Graph related queries.
+(The various representations of "Graphs" in tabular dataframe makes it hard to
+have consistent backend handling of such data.) # But why? Why not use Sklearn?
 SciPy? NumPy? The goal of the package is to **facilitate** data processes and
 analysis that go beyond standard SQL queries, and to **reduce** the number of
 dependencies in your project. It incorproates parts of SciPy, NumPy, Scikit-
 learn, and NLP (NLTK), etc., and treats them as Polars queries so that they can
 be run in parallel, in group_by contexts, all for almost no extra engineering
 effort. Let's see an example. Say we want to generate a model performance
 report. In our data, we have segments. We are not only interested in the ROC
@@ -75,32 +87,31 @@
 hidden away from the end user. (3) Because Polars provides parallel execution
 for free, we can compute ROC AUC and log loss simultaneously on each segment!
 (In Pandas, one can do something like this in aggregations but is soooo much
 harder to write and way more confusing to reason about.) The end result is
 simpler, more intuitive code that is also easier to reason about, and faster
 execution time. Because of Polars's extension (plugin) system, we are now
 blessed with both: **Performance and elegance - something that is quite rare in
-the Python world.** ## Getting Started ```python import polars_ds as pds ```
-when you want to access the namespaces provided by the package. ```python pip
-install "polars_ds[plot]" ``` for dataframe diagnosis related features. ##
-Examples See this for Polars Extensions: [notebook](./examples/basics.ipynb)
-See this for Native Polars DataFrame Explorative tools: [notebook](./examples/
-diagnosis.ipynb) # Disclaimer **Currently in Beta. Feel free to submit feature
-requests in the issues section of the repo. This library will only depend on
-python Polars and will try to be as stable as possible for polars>=0.20.6.
-Exceptions will be made when Polars's update forces changes in the plugins.**
-This package is not tested with Polars streaming mode and is not designed to
-work with data so big that has to be streamed. The recommended usage will be
-for datasets of size 1k to 2-3mm rows, but actual performance will vary
-depending on dataset and hardware. Performance will only be a priority for
-datasets that fit in memory. It is a known fact that knn performance suffers
-greatly with a large k. Str-knn and Graph queries are only suitable for smaller
-data, of size ~1-5k for common computers. # Credits 1. Rust Snowball Stemmer is
-taken from Tsoding's Seroost project (MIT). See [here](https://github.com/
-tsoding/seroost) 2. Some statistics functions are taken from Statrs (MIT) and
-internalized. See [here](https://github.com/statrs-dev/statrs/tree/master) 3.
-Graph functionalities are powered by the petgragh crate. See [here](https://
-crates.io/crates/petgraph) 4. Linear algebra routines are powered partly by
-[faer](https://crates.io/crates/faer) # Other related Projects 1. Take a look
-at our friendly neighbor [functime](https://github.com/TracecatHQ/functime) 2.
-String similarity metrics is soooo fast and easy to use because of [RapidFuzz]
-(https://github.com/maxbachmann/rapidfuzz-rs)
+the Python world.** ## Getting Started ```python import polars_ds as pds ``` To
+make full use of the Diagnosis module, do ```python pip install "polars_ds
+[plot]" ``` ## Examples See this for Polars Extensions: [notebook](./examples/
+basics.ipynb) See this for Native Polars DataFrame Explorative tools:
+[notebook](./examples/diagnosis.ipynb) # Disclaimer **Currently in Beta. Feel
+free to submit feature requests in the issues section of the repo. This library
+will only depend on python Polars and will try to be as stable as possible for
+polars>=0.20.6. Exceptions will be made when Polars's update forces changes in
+the plugins.** This package is not tested with Polars streaming mode and is not
+designed to work with data so big that has to be streamed. The recommended
+usage will be for datasets of size 1k to 2-3mm rows, but actual performance
+will vary depending on dataset and hardware. Performance will only be a
+priority for datasets that fit in memory. It is a known fact that knn
+performance suffers greatly with a large k. Str-knn and Graph queries are only
+suitable for smaller data, of size ~1-5k for common computers. # Credits 1.
+Rust Snowball Stemmer is taken from Tsoding's Seroost project (MIT). See [here]
+(https://github.com/tsoding/seroost) 2. Some statistics functions are taken
+from Statrs (MIT) and internalized. See [here](https://github.com/statrs-dev/
+statrs/tree/master) 3. Graph functionalities are powered by the petgragh crate.
+See [here](https://crates.io/crates/petgraph) 4. Linear algebra routines are
+powered partly by [faer](https://crates.io/crates/faer) # Other related
+Projects 1. Take a look at our friendly neighbor [functime](https://github.com/
+TracecatHQ/functime) 2. String similarity metrics is soooo fast and easy to use
+because of [RapidFuzz](https://github.com/maxbachmann/rapidfuzz-rs)
```

### Comparing `polars_ds-0.4.2/docs/index.md` & `polars_ds-0.4.3/docs/index.md`

 * *Files 17% similar despite different names*

```diff
@@ -2,27 +2,37 @@
 
 A comprehensive [walkthrough](https://github.com/abstractqqq/polars_ds_extension/blob/knn_entropy/examples/basics.ipynb).
 
 Read the [Docs](https://polars-ds-extension.readthedocs.io/en/latest/).
 
 # The Project
 
-The goal of the project is to **reduce dependencies**, **improve code organization**, **simplify data pipelines** and overall **faciliate analysis of various kinds of tabular data** that a data scientist may encounter. It is a package built around your favorite **Polars dataframe**. Here are the current namespaces (Polars Extensions) provided by the package:
+The goal of the project is to **reduce dependencies**, **improve code organization**, **simplify data pipelines** and overall **faciliate analysis of various kinds of tabular data** that a data scientist may encounter. It is a package built around your favorite **Polars dataframe**. Here are some of the main areas of data science that is covered by the package:
 
-1. A numerical extension (num), which focuses on numerical quantities common in many fields of data analysis (credit modelling, time series, other well-known quantities, etc.), such as rfft, entropies, k-nearest-neighbors queries, Population Stability Index, Information Value, etc.
+1. Well-known numerical transform/quantities. E.g. fft, conditional entropy, singular values, basic linear regression related quantities, population stability index, weight of evidence, column-wise/row-wise jaccard similarity etc.
 
-2. A metrics extension (metric), which contains a lot of common error/loss functions, model evaluation metrics. This module is mostly designed to generate model performance monitoring
+2. Statistics. Basic tests such as the t-test, f-test, KS statistics. Miscallaneous functions like weighted correlation, Xi-correlation. In-dataframe random column generations, etc. 
 
-3. A str extension (str2), which focuses on str distances/similarities, and other commonly used string manipulation procedures.
+3. Metrics. ML metrics for common model performance reporting. E.g ROC AUC for binary/multiclass classification, logloss, r2, MAPE, etc.
 
-4. A stats extension (stats), which has common statistical tests such as t-test, chi2, and f-test, etc., and random sampling from a distribution without leaving dataframes.
+4. KNN-related queries. E.g. filter to k-nearest neighbors to point, find indices of all neighbors within a certain distance, etc.
 
-5. A complex extension (c), which treats complex numbers as a column of array of size 2. Sometimes complex numbers are needed for processing FFT outputs.
+5. String metrics such as Levenshtein distance, Damure Levenshtein distance, other string distances, snowball stemming (English only), string Jaccard similarity, etc.
 
-6. A graph extension (graph) for very simple graph queries, such as shortest path queries, eigenvector centrality computations. More will be added.
+6. Diagnosis. This modules contains the DIA (Data Inspection Assitant) class, which can help you profile your data, visualize data in lower dimensions, detect functional dependencies, detect other common data quality issues like null rate or high correlation.
+
+7. Sample. Traditional dataset sampling. No time series sampling yet. This module provides functionalities such as stratified downsample, volume neutral random sampling, etc.
+
+8. Polars Native ML Pipeline. Planned but not started yet. The goal is to have a Polars native pipeline that can replace Scikit-learn's pipeline and provides all the benefits of Polars. All the basic transforms in Scikit-leran, categorical-encoders are planned. This can be super powerful together with Polars's expressions. (Basically, once you have expressions, you don't need to write custom transforms like col(A)/col(B), log transform, sqrt transform, linear/polynomial transforms, etc.)
+
+Some other areas that currently exist, but is de-prioritized:
+
+1. Complex number related queries.
+
+2. Graph related queries. (The various representations of "Graphs" in tabular dataframe makes it hard to have consistent backend handling of such data.)
 
 # But why? Why not use Sklearn? SciPy? NumPy?
 
 The goal of the package is to **facilitate** data processes and analysis that go beyond standard SQL queries, and to **reduce** the number of dependencies in your project. It incorproates parts of SciPy, NumPy, Scikit-learn, and NLP (NLTK), etc., and treats them as Polars queries so that they can be run in parallel, in group_by contexts, all for almost no extra engineering effort. 
 
 Let's see an example. Say we want to generate a model performance report. In our data, we have segments. We are not only interested in the ROC AUC of our model on the entire dataset, but we are also interested in the model's performance on different segments.
 
@@ -111,24 +121,26 @@
 **Performance and elegance - something that is quite rare in the Python world.**
 
 ## Getting Started
 
 ```python
 import polars_ds as pds
 ```
-when you want to access the namespaces provided by the package. Do
+
+To make full use of the Diagnosis module, do
 
 ```python
 pip install "polars_ds[plot]"
 ```
-for dataframe diagnosis related features.
 
 ## Examples
 
+See this for Polars Extensions: [notebook](./examples/basics.ipynb)
 
+See this for Native Polars DataFrame Explorative tools: [notebook](./examples/diagnosis.ipynb)
 
 # Disclaimer
 
 **Currently in Beta. Feel free to submit feature requests in the issues section of the repo. This library will only depend on python Polars and will try to be as stable as possible for polars>=0.20.6. Exceptions will be made when Polars's update forces changes in the plugins.**
 
 This package is not tested with Polars streaming mode and is not designed to work with data so big that has to be streamed.
```

### Comparing `polars_ds-0.4.2/examples/basics.ipynb` & `polars_ds-0.4.3/examples/basics.ipynb`

 * *Files 2% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9998531438717855%*

 * *Differences: {"'cells'": "{3: {'outputs': {0: {'data': {'text/html': {insert: [(7, '<small>shape: (5, "*

 * *            '11)</small><table border="1" '*

 * *            'class="dataframe"><thead><tr><th>f</th><th>time_idx</th><th>dummy</th><th>a</th><th>b</th><th>x1</th><th>x2</th><th>y</th><th>actual</th><th>predicted</th><th>dummy_groups</th></tr><tr><td>f64</td><td>i64</td><td>str</td><td>f64</td><td>f64</td><td>i64</td><td>i64</td><td>i64</td><td>i32</td><td>f64</td><td>str</td></tr></thead><tbody><tr><td>0.0</td><td>0</td>< […]*

```diff
@@ -42,28 +42,28 @@
                             "<div><style>\n",
                             ".dataframe > thead > tr,\n",
                             ".dataframe > tbody > tr {\n",
                             "  text-align: right;\n",
                             "  white-space: pre-wrap;\n",
                             "}\n",
                             "</style>\n",
-                            "<small>shape: (5, 11)</small><table border=\"1\" class=\"dataframe\"><thead><tr><th>f</th><th>time_idx</th><th>dummy</th><th>a</th><th>b</th><th>x1</th><th>x2</th><th>y</th><th>actual</th><th>predicted</th><th>dummy_groups</th></tr><tr><td>f64</td><td>i64</td><td>str</td><td>f64</td><td>f64</td><td>i64</td><td>i64</td><td>i64</td><td>i32</td><td>f64</td><td>str</td></tr></thead><tbody><tr><td>0.0</td><td>0</td><td>&quot;a&quot;</td><td>0.682803</td><td>0.415153</td><td>0</td><td>10000</td><td>-10000</td><td>1</td><td>0.873578</td><td>&quot;a&quot;</td></tr><tr><td>0.841471</td><td>1</td><td>&quot;a&quot;</td><td>0.687497</td><td>0.591041</td><td>1</td><td>10001</td><td>-9999</td><td>0</td><td>0.816631</td><td>&quot;a&quot;</td></tr><tr><td>0.909297</td><td>2</td><td>&quot;a&quot;</td><td>0.671245</td><td>0.565974</td><td>2</td><td>10002</td><td>-9998</td><td>1</td><td>0.806592</td><td>&quot;a&quot;</td></tr><tr><td>0.14112</td><td>3</td><td>&quot;a&quot;</td><td>0.446571</td><td>0.501598</td><td>3</td><td>10003</td><td>-9997</td><td>1</td><td>0.848589</td><td>&quot;a&quot;</td></tr><tr><td>-0.756802</td><td>4</td><td>&quot;a&quot;</td><td>0.836808</td><td>0.782067</td><td>4</td><td>10004</td><td>-9996</td><td>0</td><td>0.746404</td><td>&quot;a&quot;</td></tr></tbody></table></div>"
+                            "<small>shape: (5, 11)</small><table border=\"1\" class=\"dataframe\"><thead><tr><th>f</th><th>time_idx</th><th>dummy</th><th>a</th><th>b</th><th>x1</th><th>x2</th><th>y</th><th>actual</th><th>predicted</th><th>dummy_groups</th></tr><tr><td>f64</td><td>i64</td><td>str</td><td>f64</td><td>f64</td><td>i64</td><td>i64</td><td>i64</td><td>i32</td><td>f64</td><td>str</td></tr></thead><tbody><tr><td>0.0</td><td>0</td><td>&quot;a&quot;</td><td>0.481374</td><td>0.692214</td><td>0</td><td>10000</td><td>-10000</td><td>0</td><td>0.937129</td><td>&quot;a&quot;</td></tr><tr><td>0.841471</td><td>1</td><td>&quot;a&quot;</td><td>0.745246</td><td>0.313353</td><td>1</td><td>10001</td><td>-9999</td><td>0</td><td>0.076196</td><td>&quot;a&quot;</td></tr><tr><td>0.909297</td><td>2</td><td>&quot;a&quot;</td><td>0.732082</td><td>0.399353</td><td>2</td><td>10002</td><td>-9998</td><td>1</td><td>0.157438</td><td>&quot;a&quot;</td></tr><tr><td>0.14112</td><td>3</td><td>&quot;a&quot;</td><td>0.094566</td><td>0.510672</td><td>3</td><td>10003</td><td>-9997</td><td>0</td><td>0.281071</td><td>&quot;a&quot;</td></tr><tr><td>-0.756802</td><td>4</td><td>&quot;a&quot;</td><td>0.32162</td><td>0.180718</td><td>4</td><td>10004</td><td>-9996</td><td>1</td><td>0.106533</td><td>&quot;a&quot;</td></tr></tbody></table></div>"
                         ],
                         "text/plain": [
                             "shape: (5, 11)\n",
                             "\u250c\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u252c\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u252c\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u252c\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u252c\u2500\u2500\u2500\u252c\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u252c\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u252c\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u252c\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2510\n",
                             "\u2502 f         \u2506 time_idx \u2506 dummy \u2506 a        \u2506 \u2026 \u2506 y      \u2506 actual \u2506 predicted \u2506 dummy_groups \u2502\n",
                             "\u2502 ---       \u2506 ---      \u2506 ---   \u2506 ---      \u2506   \u2506 ---    \u2506 ---    \u2506 ---       \u2506 ---          \u2502\n",
                             "\u2502 f64       \u2506 i64      \u2506 str   \u2506 f64      \u2506   \u2506 i64    \u2506 i32    \u2506 f64       \u2506 str          \u2502\n",
                             "\u255e\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u256a\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u256a\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u256a\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u256a\u2550\u2550\u2550\u256a\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u256a\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u256a\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u256a\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2561\n",
-                            "\u2502 0.0       \u2506 0        \u2506 a     \u2506 0.682803 \u2506 \u2026 \u2506 -10000 \u2506 1      \u2506 0.873578  \u2506 a            \u2502\n",
-                            "\u2502 0.841471  \u2506 1        \u2506 a     \u2506 0.687497 \u2506 \u2026 \u2506 -9999  \u2506 0      \u2506 0.816631  \u2506 a            \u2502\n",
-                            "\u2502 0.909297  \u2506 2        \u2506 a     \u2506 0.671245 \u2506 \u2026 \u2506 -9998  \u2506 1      \u2506 0.806592  \u2506 a            \u2502\n",
-                            "\u2502 0.14112   \u2506 3        \u2506 a     \u2506 0.446571 \u2506 \u2026 \u2506 -9997  \u2506 1      \u2506 0.848589  \u2506 a            \u2502\n",
-                            "\u2502 -0.756802 \u2506 4        \u2506 a     \u2506 0.836808 \u2506 \u2026 \u2506 -9996  \u2506 0      \u2506 0.746404  \u2506 a            \u2502\n",
+                            "\u2502 0.0       \u2506 0        \u2506 a     \u2506 0.481374 \u2506 \u2026 \u2506 -10000 \u2506 0      \u2506 0.937129  \u2506 a            \u2502\n",
+                            "\u2502 0.841471  \u2506 1        \u2506 a     \u2506 0.745246 \u2506 \u2026 \u2506 -9999  \u2506 0      \u2506 0.076196  \u2506 a            \u2502\n",
+                            "\u2502 0.909297  \u2506 2        \u2506 a     \u2506 0.732082 \u2506 \u2026 \u2506 -9998  \u2506 1      \u2506 0.157438  \u2506 a            \u2502\n",
+                            "\u2502 0.14112   \u2506 3        \u2506 a     \u2506 0.094566 \u2506 \u2026 \u2506 -9997  \u2506 0      \u2506 0.281071  \u2506 a            \u2502\n",
+                            "\u2502 -0.756802 \u2506 4        \u2506 a     \u2506 0.32162  \u2506 \u2026 \u2506 -9996  \u2506 1      \u2506 0.106533  \u2506 a            \u2502\n",
                             "\u2514\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2534\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2534\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2534\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2534\u2500\u2500\u2500\u2534\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2534\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2534\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2534\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2518"
                         ]
                     },
                     "execution_count": 2,
                     "metadata": {},
                     "output_type": "execute_result"
                 }
@@ -210,28 +210,28 @@
                             "<div><style>\n",
                             ".dataframe > thead > tr,\n",
                             ".dataframe > tbody > tr {\n",
                             "  text-align: right;\n",
                             "  white-space: pre-wrap;\n",
                             "}\n",
                             "</style>\n",
-                            "<small>shape: (5, 3)</small><table border=\"1\" class=\"dataframe\"><thead><tr><th>f</th><th>a</th><th>b</th></tr><tr><td>f64</td><td>f64</td><td>f64</td></tr></thead><tbody><tr><td>1.3944e-15</td><td>-0.682803</td><td>-0.415153</td></tr><tr><td>-0.841471</td><td>-0.687497</td><td>-0.591041</td></tr><tr><td>-0.909297</td><td>-0.671245</td><td>-0.565974</td></tr><tr><td>-0.14112</td><td>-0.446571</td><td>-0.501598</td></tr><tr><td>0.756802</td><td>-0.154005</td><td>-0.366915</td></tr></tbody></table></div>"
+                            "<small>shape: (5, 3)</small><table border=\"1\" class=\"dataframe\"><thead><tr><th>f</th><th>a</th><th>b</th></tr><tr><td>f64</td><td>f64</td><td>f64</td></tr></thead><tbody><tr><td>1.3944e-15</td><td>-0.481374</td><td>-0.692214</td></tr><tr><td>-0.841471</td><td>-0.745246</td><td>-0.313353</td></tr><tr><td>-0.909297</td><td>-0.732082</td><td>-0.399353</td></tr><tr><td>-0.14112</td><td>-0.094566</td><td>-0.510672</td></tr><tr><td>0.756802</td><td>0.159754</td><td>0.511495</td></tr></tbody></table></div>"
                         ],
                         "text/plain": [
                             "shape: (5, 3)\n",
                             "\u250c\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u252c\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u252c\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2510\n",
                             "\u2502 f          \u2506 a         \u2506 b         \u2502\n",
                             "\u2502 ---        \u2506 ---       \u2506 ---       \u2502\n",
                             "\u2502 f64        \u2506 f64       \u2506 f64       \u2502\n",
                             "\u255e\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u256a\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u256a\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2561\n",
-                            "\u2502 1.3944e-15 \u2506 -0.682803 \u2506 -0.415153 \u2502\n",
-                            "\u2502 -0.841471  \u2506 -0.687497 \u2506 -0.591041 \u2502\n",
-                            "\u2502 -0.909297  \u2506 -0.671245 \u2506 -0.565974 \u2502\n",
-                            "\u2502 -0.14112   \u2506 -0.446571 \u2506 -0.501598 \u2502\n",
-                            "\u2502 0.756802   \u2506 -0.154005 \u2506 -0.366915 \u2502\n",
+                            "\u2502 1.3944e-15 \u2506 -0.481374 \u2506 -0.692214 \u2502\n",
+                            "\u2502 -0.841471  \u2506 -0.745246 \u2506 -0.313353 \u2502\n",
+                            "\u2502 -0.909297  \u2506 -0.732082 \u2506 -0.399353 \u2502\n",
+                            "\u2502 -0.14112   \u2506 -0.094566 \u2506 -0.510672 \u2502\n",
+                            "\u2502 0.756802   \u2506 0.159754  \u2506 0.511495  \u2502\n",
                             "\u2514\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2534\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2534\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2518"
                         ]
                     },
                     "execution_count": 6,
                     "metadata": {},
                     "output_type": "execute_result"
                 }
@@ -638,24 +638,24 @@
                             "<div><style>\n",
                             ".dataframe > thead > tr,\n",
                             ".dataframe > tbody > tr {\n",
                             "  text-align: right;\n",
                             "  white-space: pre-wrap;\n",
                             "}\n",
                             "</style>\n",
-                            "<small>shape: (1, 1)</small><table border=\"1\" class=\"dataframe\"><thead><tr><th>a</th></tr><tr><td>list[f64]</td></tr></thead><tbody><tr><td>[288675.133152, 28.94286, 28.709543]</td></tr></tbody></table></div>"
+                            "<small>shape: (1, 1)</small><table border=\"1\" class=\"dataframe\"><thead><tr><th>a</th></tr><tr><td>list[f64]</td></tr></thead><tbody><tr><td>[288675.133152, 28.9779, 28.751495]</td></tr></tbody></table></div>"
                         ],
                         "text/plain": [
                             "shape: (1, 1)\n",
                             "\u250c\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2510\n",
                             "\u2502 a                                 \u2502\n",
                             "\u2502 ---                               \u2502\n",
                             "\u2502 list[f64]                         \u2502\n",
                             "\u255e\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2561\n",
-                            "\u2502 [288675.133152, 28.94286, 28.709\u2026 \u2502\n",
+                            "\u2502 [288675.133152, 28.9779, 28.7514\u2026 \u2502\n",
                             "\u2514\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2518"
                         ]
                     },
                     "execution_count": 15,
                     "metadata": {},
                     "output_type": "execute_result"
                 }
@@ -679,25 +679,25 @@
                             "<div><style>\n",
                             ".dataframe > thead > tr,\n",
                             ".dataframe > tbody > tr {\n",
                             "  text-align: right;\n",
                             "  white-space: pre-wrap;\n",
                             "}\n",
                             "</style>\n",
-                            "<small>shape: (2, 2)</small><table border=\"1\" class=\"dataframe\"><thead><tr><th>singular_value</th><th>principal_vectors</th></tr><tr><td>f64</td><td>list[f64]</td></tr></thead><tbody><tr><td>28.945769</td><td>[0.698117, 0.715984]</td></tr><tr><td>28.710273</td><td>[0.715984, -0.698117]</td></tr></tbody></table></div>"
+                            "<small>shape: (2, 2)</small><table border=\"1\" class=\"dataframe\"><thead><tr><th>singular_value</th><th>weight_vector</th></tr><tr><td>f64</td><td>list[f64]</td></tr></thead><tbody><tr><td>28.978009</td><td>[0.024624, 0.999697]</td></tr><tr><td>28.753293</td><td>[0.999697, -0.024624]</td></tr></tbody></table></div>"
                         ],
                         "text/plain": [
                             "shape: (2, 2)\n",
                             "\u250c\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u252c\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2510\n",
-                            "\u2502 singular_value \u2506 principal_vectors     \u2502\n",
+                            "\u2502 singular_value \u2506 weight_vector         \u2502\n",
                             "\u2502 ---            \u2506 ---                   \u2502\n",
                             "\u2502 f64            \u2506 list[f64]             \u2502\n",
                             "\u255e\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u256a\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2561\n",
-                            "\u2502 28.945769      \u2506 [0.698117, 0.715984]  \u2502\n",
-                            "\u2502 28.710273      \u2506 [0.715984, -0.698117] \u2502\n",
+                            "\u2502 28.978009      \u2506 [0.024624, 0.999697]  \u2502\n",
+                            "\u2502 28.753293      \u2506 [0.999697, -0.024624] \u2502\n",
                             "\u2514\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2534\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2518"
                         ]
                     },
                     "execution_count": 16,
                     "metadata": {},
                     "output_type": "execute_result"
                 }
@@ -729,26 +729,26 @@
                             "<div><style>\n",
                             ".dataframe > thead > tr,\n",
                             ".dataframe > tbody > tr {\n",
                             "  text-align: right;\n",
                             "  white-space: pre-wrap;\n",
                             "}\n",
                             "</style>\n",
-                            "<small>shape: (2, 8)</small><table border=\"1\" class=\"dataframe\"><thead><tr><th>dummy_groups</th><th>l2</th><th>log loss</th><th>precision</th><th>recall</th><th>f</th><th>average_precision</th><th>roc_auc</th></tr><tr><td>str</td><td>f64</td><td>f64</td><td>f64</td><td>f64</td><td>f64</td><td>f64</td><td>f64</td></tr></thead><tbody><tr><td>&quot;b&quot;</td><td>0.329581</td><td>0.985112</td><td>0.499601</td><td>0.5012</td><td>0.2502</td><td>0.502613</td><td>0.502348</td></tr><tr><td>&quot;a&quot;</td><td>0.33594</td><td>1.003373</td><td>0.48839</td><td>0.503244</td><td>0.247853</td><td>0.490244</td><td>0.494221</td></tr></tbody></table></div>"
+                            "<small>shape: (2, 8)</small><table border=\"1\" class=\"dataframe\"><thead><tr><th>dummy_groups</th><th>l2</th><th>log loss</th><th>precision</th><th>recall</th><th>f</th><th>average_precision</th><th>roc_auc</th></tr><tr><td>str</td><td>f64</td><td>f64</td><td>f64</td><td>f64</td><td>f64</td><td>f64</td><td>f64</td></tr></thead><tbody><tr><td>&quot;a&quot;</td><td>0.332346</td><td>0.997371</td><td>0.500984</td><td>0.511656</td><td>0.253132</td><td>0.502761</td><td>0.503789</td></tr><tr><td>&quot;b&quot;</td><td>0.341309</td><td>1.03576</td><td>0.48747</td><td>0.484922</td><td>0.243096</td><td>0.489989</td><td>0.484345</td></tr></tbody></table></div>"
                         ],
                         "text/plain": [
                             "shape: (2, 8)\n",
                             "\u250c\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u252c\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u252c\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u252c\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u252c\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u252c\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u252c\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u252c\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2510\n",
                             "\u2502 dummy_groups \u2506 l2       \u2506 log loss \u2506 precision \u2506 recall   \u2506 f        \u2506 average_precis \u2506 roc_auc  \u2502\n",
                             "\u2502 ---          \u2506 ---      \u2506 ---      \u2506 ---       \u2506 ---      \u2506 ---      \u2506 ion            \u2506 ---      \u2502\n",
                             "\u2502 str          \u2506 f64      \u2506 f64      \u2506 f64       \u2506 f64      \u2506 f64      \u2506 ---            \u2506 f64      \u2502\n",
                             "\u2502              \u2506          \u2506          \u2506           \u2506          \u2506          \u2506 f64            \u2506          \u2502\n",
                             "\u255e\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u256a\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u256a\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u256a\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u256a\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u256a\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u256a\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u256a\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2561\n",
-                            "\u2502 b            \u2506 0.329581 \u2506 0.985112 \u2506 0.499601  \u2506 0.5012   \u2506 0.2502   \u2506 0.502613       \u2506 0.502348 \u2502\n",
-                            "\u2502 a            \u2506 0.33594  \u2506 1.003373 \u2506 0.48839   \u2506 0.503244 \u2506 0.247853 \u2506 0.490244       \u2506 0.494221 \u2502\n",
+                            "\u2502 a            \u2506 0.332346 \u2506 0.997371 \u2506 0.500984  \u2506 0.511656 \u2506 0.253132 \u2506 0.502761       \u2506 0.503789 \u2502\n",
+                            "\u2502 b            \u2506 0.341309 \u2506 1.03576  \u2506 0.48747   \u2506 0.484922 \u2506 0.243096 \u2506 0.489989       \u2506 0.484345 \u2502\n",
                             "\u2514\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2534\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2534\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2534\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2534\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2534\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2534\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2534\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2518"
                         ]
                     },
                     "execution_count": 17,
                     "metadata": {},
                     "output_type": "execute_result"
                 }
@@ -828,28 +828,28 @@
                             "<div><style>\n",
                             ".dataframe > thead > tr,\n",
                             ".dataframe > tbody > tr {\n",
                             "  text-align: right;\n",
                             "  white-space: pre-wrap;\n",
                             "}\n",
                             "</style>\n",
-                            "<small>shape: (5, 1)</small><table border=\"1\" class=\"dataframe\"><thead><tr><th>sen</th></tr><tr><td>str</td></tr></thead><tbody><tr><td>&quot;world&quot;</td></tr><tr><td>&quot;to&quot;</td></tr><tr><td>&quot;church&quot;</td></tr><tr><td>&quot;hello&quot;</td></tr><tr><td>&quot;going&quot;</td></tr></tbody></table></div>"
+                            "<small>shape: (5, 1)</small><table border=\"1\" class=\"dataframe\"><thead><tr><th>sen</th></tr><tr><td>str</td></tr></thead><tbody><tr><td>&quot;hello&quot;</td></tr><tr><td>&quot;church&quot;</td></tr><tr><td>&quot;to&quot;</td></tr><tr><td>&quot;going&quot;</td></tr><tr><td>&quot;world&quot;</td></tr></tbody></table></div>"
                         ],
                         "text/plain": [
                             "shape: (5, 1)\n",
                             "\u250c\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2510\n",
                             "\u2502 sen    \u2502\n",
                             "\u2502 ---    \u2502\n",
                             "\u2502 str    \u2502\n",
                             "\u255e\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2561\n",
-                            "\u2502 world  \u2502\n",
-                            "\u2502 to     \u2502\n",
-                            "\u2502 church \u2502\n",
                             "\u2502 hello  \u2502\n",
+                            "\u2502 church \u2502\n",
+                            "\u2502 to     \u2502\n",
                             "\u2502 going  \u2502\n",
+                            "\u2502 world  \u2502\n",
                             "\u2514\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2518"
                         ]
                     },
                     "execution_count": 19,
                     "metadata": {},
                     "output_type": "execute_result"
                 }
@@ -873,28 +873,28 @@
                             "<div><style>\n",
                             ".dataframe > thead > tr,\n",
                             ".dataframe > tbody > tr {\n",
                             "  text-align: right;\n",
                             "  white-space: pre-wrap;\n",
                             "}\n",
                             "</style>\n",
-                            "<small>shape: (5, 1)</small><table border=\"1\" class=\"dataframe\"><thead><tr><th>sen</th></tr><tr><td>str</td></tr></thead><tbody><tr><td>&quot;&quot;</td></tr><tr><td>&quot;hello&quot;</td></tr><tr><td>&quot;church&quot;</td></tr><tr><td>&quot;go&quot;</td></tr><tr><td>&quot;world&quot;</td></tr></tbody></table></div>"
+                            "<small>shape: (5, 1)</small><table border=\"1\" class=\"dataframe\"><thead><tr><th>sen</th></tr><tr><td>str</td></tr></thead><tbody><tr><td>&quot;&quot;</td></tr><tr><td>&quot;go&quot;</td></tr><tr><td>&quot;world&quot;</td></tr><tr><td>&quot;church&quot;</td></tr><tr><td>&quot;hello&quot;</td></tr></tbody></table></div>"
                         ],
                         "text/plain": [
                             "shape: (5, 1)\n",
                             "\u250c\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2510\n",
                             "\u2502 sen    \u2502\n",
                             "\u2502 ---    \u2502\n",
                             "\u2502 str    \u2502\n",
                             "\u255e\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2561\n",
                             "\u2502        \u2502\n",
-                            "\u2502 hello  \u2502\n",
-                            "\u2502 church \u2502\n",
                             "\u2502 go     \u2502\n",
                             "\u2502 world  \u2502\n",
+                            "\u2502 church \u2502\n",
+                            "\u2502 hello  \u2502\n",
                             "\u2514\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2518"
                         ]
                     },
                     "execution_count": 20,
                     "metadata": {},
                     "output_type": "execute_result"
                 }
@@ -1214,29 +1214,29 @@
                             "<div><style>\n",
                             ".dataframe > thead > tr,\n",
                             ".dataframe > tbody > tr {\n",
                             "  text-align: right;\n",
                             "  white-space: pre-wrap;\n",
                             "}\n",
                             "</style>\n",
-                            "<small>shape: (5, 1)</small><table border=\"1\" class=\"dataframe\"><thead><tr><th>a</th></tr><tr><td>f64</td></tr></thead><tbody><tr><td>null</td></tr><tr><td>null</td></tr><tr><td>0.066091</td></tr><tr><td>-0.35634</td></tr><tr><td>1.17341</td></tr></tbody></table></div>"
+                            "<small>shape: (5, 1)</small><table border=\"1\" class=\"dataframe\"><thead><tr><th>a</th></tr><tr><td>f64</td></tr></thead><tbody><tr><td>null</td></tr><tr><td>null</td></tr><tr><td>-0.233906</td></tr><tr><td>2.031312</td></tr><tr><td>1.410816</td></tr></tbody></table></div>"
                         ],
                         "text/plain": [
                             "shape: (5, 1)\n",
-                            "\u250c\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2510\n",
-                            "\u2502 a        \u2502\n",
-                            "\u2502 ---      \u2502\n",
-                            "\u2502 f64      \u2502\n",
-                            "\u255e\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2561\n",
-                            "\u2502 null     \u2502\n",
-                            "\u2502 null     \u2502\n",
-                            "\u2502 0.066091 \u2502\n",
-                            "\u2502 -0.35634 \u2502\n",
-                            "\u2502 1.17341  \u2502\n",
-                            "\u2514\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2518"
+                            "\u250c\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2510\n",
+                            "\u2502 a         \u2502\n",
+                            "\u2502 ---       \u2502\n",
+                            "\u2502 f64       \u2502\n",
+                            "\u255e\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2561\n",
+                            "\u2502 null      \u2502\n",
+                            "\u2502 null      \u2502\n",
+                            "\u2502 -0.233906 \u2502\n",
+                            "\u2502 2.031312  \u2502\n",
+                            "\u2502 1.410816  \u2502\n",
+                            "\u2514\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2518"
                         ]
                     },
                     "execution_count": 28,
                     "metadata": {},
                     "output_type": "execute_result"
                 }
             ],
@@ -1261,29 +1261,29 @@
                             "<div><style>\n",
                             ".dataframe > thead > tr,\n",
                             ".dataframe > tbody > tr {\n",
                             "  text-align: right;\n",
                             "  white-space: pre-wrap;\n",
                             "}\n",
                             "</style>\n",
-                            "<small>shape: (5, 2)</small><table border=\"1\" class=\"dataframe\"><thead><tr><th>a</th><th>random</th></tr><tr><td>f64</td><td>f64</td></tr></thead><tbody><tr><td>null</td><td>null</td></tr><tr><td>null</td><td>null</td></tr><tr><td>0.066091</td><td>1.838582</td></tr><tr><td>-0.35634</td><td>1.149611</td></tr><tr><td>1.17341</td><td>0.960881</td></tr></tbody></table></div>"
+                            "<small>shape: (5, 2)</small><table border=\"1\" class=\"dataframe\"><thead><tr><th>a</th><th>random</th></tr><tr><td>f64</td><td>f64</td></tr></thead><tbody><tr><td>null</td><td>null</td></tr><tr><td>null</td><td>null</td></tr><tr><td>-0.233906</td><td>1.894852</td></tr><tr><td>2.031312</td><td>1.17594</td></tr><tr><td>1.410816</td><td>-0.382411</td></tr></tbody></table></div>"
                         ],
                         "text/plain": [
                             "shape: (5, 2)\n",
-                            "\u250c\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u252c\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2510\n",
-                            "\u2502 a        \u2506 random   \u2502\n",
-                            "\u2502 ---      \u2506 ---      \u2502\n",
-                            "\u2502 f64      \u2506 f64      \u2502\n",
-                            "\u255e\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u256a\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2561\n",
-                            "\u2502 null     \u2506 null     \u2502\n",
-                            "\u2502 null     \u2506 null     \u2502\n",
-                            "\u2502 0.066091 \u2506 1.838582 \u2502\n",
-                            "\u2502 -0.35634 \u2506 1.149611 \u2502\n",
-                            "\u2502 1.17341  \u2506 0.960881 \u2502\n",
-                            "\u2514\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2534\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2518"
+                            "\u250c\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u252c\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2510\n",
+                            "\u2502 a         \u2506 random    \u2502\n",
+                            "\u2502 ---       \u2506 ---       \u2502\n",
+                            "\u2502 f64       \u2506 f64       \u2502\n",
+                            "\u255e\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u256a\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2561\n",
+                            "\u2502 null      \u2506 null      \u2502\n",
+                            "\u2502 null      \u2506 null      \u2502\n",
+                            "\u2502 -0.233906 \u2506 1.894852  \u2502\n",
+                            "\u2502 2.031312  \u2506 1.17594   \u2502\n",
+                            "\u2502 1.410816  \u2506 -0.382411 \u2502\n",
+                            "\u2514\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2534\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2518"
                         ]
                     },
                     "execution_count": 29,
                     "metadata": {},
                     "output_type": "execute_result"
                 }
             ],
@@ -1306,29 +1306,29 @@
                             "<div><style>\n",
                             ".dataframe > thead > tr,\n",
                             ".dataframe > tbody > tr {\n",
                             "  text-align: right;\n",
                             "  white-space: pre-wrap;\n",
                             "}\n",
                             "</style>\n",
-                            "<small>shape: (5, 2)</small><table border=\"1\" class=\"dataframe\"><thead><tr><th>a</th><th>random_str</th></tr><tr><td>f64</td><td>str</td></tr></thead><tbody><tr><td>null</td><td>null</td></tr><tr><td>null</td><td>null</td></tr><tr><td>0.066091</td><td>&quot;DIu2G&quot;</td></tr><tr><td>-0.35634</td><td>&quot;9eNwx&quot;</td></tr><tr><td>1.17341</td><td>&quot;W&quot;</td></tr></tbody></table></div>"
+                            "<small>shape: (5, 2)</small><table border=\"1\" class=\"dataframe\"><thead><tr><th>a</th><th>random_str</th></tr><tr><td>f64</td><td>str</td></tr></thead><tbody><tr><td>null</td><td>null</td></tr><tr><td>null</td><td>null</td></tr><tr><td>-0.233906</td><td>&quot;y&quot;</td></tr><tr><td>2.031312</td><td>&quot;lBEiU&quot;</td></tr><tr><td>1.410816</td><td>&quot;FWz5&quot;</td></tr></tbody></table></div>"
                         ],
                         "text/plain": [
                             "shape: (5, 2)\n",
-                            "\u250c\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u252c\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2510\n",
-                            "\u2502 a        \u2506 random_str \u2502\n",
-                            "\u2502 ---      \u2506 ---        \u2502\n",
-                            "\u2502 f64      \u2506 str        \u2502\n",
-                            "\u255e\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u256a\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2561\n",
-                            "\u2502 null     \u2506 null       \u2502\n",
-                            "\u2502 null     \u2506 null       \u2502\n",
-                            "\u2502 0.066091 \u2506 DIu2G      \u2502\n",
-                            "\u2502 -0.35634 \u2506 9eNwx      \u2502\n",
-                            "\u2502 1.17341  \u2506 W          \u2502\n",
-                            "\u2514\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2534\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2518"
+                            "\u250c\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u252c\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2510\n",
+                            "\u2502 a         \u2506 random_str \u2502\n",
+                            "\u2502 ---       \u2506 ---        \u2502\n",
+                            "\u2502 f64       \u2506 str        \u2502\n",
+                            "\u255e\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u256a\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2561\n",
+                            "\u2502 null      \u2506 null       \u2502\n",
+                            "\u2502 null      \u2506 null       \u2502\n",
+                            "\u2502 -0.233906 \u2506 y          \u2502\n",
+                            "\u2502 2.031312  \u2506 lBEiU      \u2502\n",
+                            "\u2502 1.410816  \u2506 FWz5       \u2502\n",
+                            "\u2514\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2534\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2518"
                         ]
                     },
                     "execution_count": 30,
                     "metadata": {},
                     "output_type": "execute_result"
                 }
             ],
@@ -1351,29 +1351,29 @@
                             "<div><style>\n",
                             ".dataframe > thead > tr,\n",
                             ".dataframe > tbody > tr {\n",
                             "  text-align: right;\n",
                             "  white-space: pre-wrap;\n",
                             "}\n",
                             "</style>\n",
-                            "<small>shape: (5, 2)</small><table border=\"1\" class=\"dataframe\"><thead><tr><th>a</th><th>random_str</th></tr><tr><td>f64</td><td>str</td></tr></thead><tbody><tr><td>null</td><td>null</td></tr><tr><td>null</td><td>null</td></tr><tr><td>0.066091</td><td>&quot;kLzzH&quot;</td></tr><tr><td>-0.35634</td><td>&quot;Kjqg2&quot;</td></tr><tr><td>1.17341</td><td>&quot;dtleS&quot;</td></tr></tbody></table></div>"
+                            "<small>shape: (5, 2)</small><table border=\"1\" class=\"dataframe\"><thead><tr><th>a</th><th>random_str</th></tr><tr><td>f64</td><td>str</td></tr></thead><tbody><tr><td>null</td><td>null</td></tr><tr><td>null</td><td>null</td></tr><tr><td>-0.233906</td><td>&quot;yie8o&quot;</td></tr><tr><td>2.031312</td><td>&quot;0gRK7&quot;</td></tr><tr><td>1.410816</td><td>&quot;ATWwe&quot;</td></tr></tbody></table></div>"
                         ],
                         "text/plain": [
                             "shape: (5, 2)\n",
-                            "\u250c\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u252c\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2510\n",
-                            "\u2502 a        \u2506 random_str \u2502\n",
-                            "\u2502 ---      \u2506 ---        \u2502\n",
-                            "\u2502 f64      \u2506 str        \u2502\n",
-                            "\u255e\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u256a\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2561\n",
-                            "\u2502 null     \u2506 null       \u2502\n",
-                            "\u2502 null     \u2506 null       \u2502\n",
-                            "\u2502 0.066091 \u2506 kLzzH      \u2502\n",
-                            "\u2502 -0.35634 \u2506 Kjqg2      \u2502\n",
-                            "\u2502 1.17341  \u2506 dtleS      \u2502\n",
-                            "\u2514\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2534\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2518"
+                            "\u250c\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u252c\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2510\n",
+                            "\u2502 a         \u2506 random_str \u2502\n",
+                            "\u2502 ---       \u2506 ---        \u2502\n",
+                            "\u2502 f64       \u2506 str        \u2502\n",
+                            "\u255e\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u256a\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2561\n",
+                            "\u2502 null      \u2506 null       \u2502\n",
+                            "\u2502 null      \u2506 null       \u2502\n",
+                            "\u2502 -0.233906 \u2506 yie8o      \u2502\n",
+                            "\u2502 2.031312  \u2506 0gRK7      \u2502\n",
+                            "\u2502 1.410816  \u2506 ATWwe      \u2502\n",
+                            "\u2514\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2534\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2518"
                         ]
                     },
                     "execution_count": 31,
                     "metadata": {},
                     "output_type": "execute_result"
                 }
             ],
@@ -1396,29 +1396,29 @@
                             "<div><style>\n",
                             ".dataframe > thead > tr,\n",
                             ".dataframe > tbody > tr {\n",
                             "  text-align: right;\n",
                             "  white-space: pre-wrap;\n",
                             "}\n",
                             "</style>\n",
-                            "<small>shape: (5, 4)</small><table border=\"1\" class=\"dataframe\"><thead><tr><th>a</th><th>test1</th><th>test2</th><th>test1_perturbed</th></tr><tr><td>f64</td><td>f64</td><td>f64</td><td>f64</td></tr></thead><tbody><tr><td>null</td><td>-0.352337</td><td>null</td><td>-0.352074</td></tr><tr><td>null</td><td>-0.987273</td><td>null</td><td>-0.986941</td></tr><tr><td>0.066091</td><td>-1.252643</td><td>1.691665</td><td>-1.25276</td></tr><tr><td>-0.35634</td><td>-0.180388</td><td>1.093283</td><td>-0.180884</td></tr><tr><td>1.17341</td><td>-0.649039</td><td>0.139838</td><td>-0.648904</td></tr></tbody></table></div>"
+                            "<small>shape: (5, 4)</small><table border=\"1\" class=\"dataframe\"><thead><tr><th>a</th><th>test1</th><th>test2</th><th>test1_perturbed</th></tr><tr><td>f64</td><td>f64</td><td>f64</td><td>f64</td></tr></thead><tbody><tr><td>null</td><td>3.109216</td><td>null</td><td>3.109434</td></tr><tr><td>null</td><td>-1.463081</td><td>null</td><td>-1.462674</td></tr><tr><td>-0.233906</td><td>-0.883572</td><td>0.940633</td><td>-0.883105</td></tr><tr><td>2.031312</td><td>0.222987</td><td>1.927644</td><td>0.223086</td></tr><tr><td>1.410816</td><td>1.796171</td><td>0.821915</td><td>1.796525</td></tr></tbody></table></div>"
                         ],
                         "text/plain": [
                             "shape: (5, 4)\n",
-                            "\u250c\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u252c\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u252c\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u252c\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2510\n",
-                            "\u2502 a        \u2506 test1     \u2506 test2    \u2506 test1_perturbed \u2502\n",
-                            "\u2502 ---      \u2506 ---       \u2506 ---      \u2506 ---             \u2502\n",
-                            "\u2502 f64      \u2506 f64       \u2506 f64      \u2506 f64             \u2502\n",
-                            "\u255e\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u256a\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u256a\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u256a\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2561\n",
-                            "\u2502 null     \u2506 -0.352337 \u2506 null     \u2506 -0.352074       \u2502\n",
-                            "\u2502 null     \u2506 -0.987273 \u2506 null     \u2506 -0.986941       \u2502\n",
-                            "\u2502 0.066091 \u2506 -1.252643 \u2506 1.691665 \u2506 -1.25276        \u2502\n",
-                            "\u2502 -0.35634 \u2506 -0.180388 \u2506 1.093283 \u2506 -0.180884       \u2502\n",
-                            "\u2502 1.17341  \u2506 -0.649039 \u2506 0.139838 \u2506 -0.648904       \u2502\n",
-                            "\u2514\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2534\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2534\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2534\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2518"
+                            "\u250c\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u252c\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u252c\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u252c\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2510\n",
+                            "\u2502 a         \u2506 test1     \u2506 test2    \u2506 test1_perturbed \u2502\n",
+                            "\u2502 ---       \u2506 ---       \u2506 ---      \u2506 ---             \u2502\n",
+                            "\u2502 f64       \u2506 f64       \u2506 f64      \u2506 f64             \u2502\n",
+                            "\u255e\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u256a\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u256a\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u256a\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2561\n",
+                            "\u2502 null      \u2506 3.109216  \u2506 null     \u2506 3.109434        \u2502\n",
+                            "\u2502 null      \u2506 -1.463081 \u2506 null     \u2506 -1.462674       \u2502\n",
+                            "\u2502 -0.233906 \u2506 -0.883572 \u2506 0.940633 \u2506 -0.883105       \u2502\n",
+                            "\u2502 2.031312  \u2506 0.222987  \u2506 1.927644 \u2506 0.223086        \u2502\n",
+                            "\u2502 1.410816  \u2506 1.796171  \u2506 0.821915 \u2506 1.796525        \u2502\n",
+                            "\u2514\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2534\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2534\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2534\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2518"
                         ]
                     },
                     "execution_count": 32,
                     "metadata": {},
                     "output_type": "execute_result"
                 }
             ],
@@ -1446,29 +1446,29 @@
                             "<div><style>\n",
                             ".dataframe > thead > tr,\n",
                             ".dataframe > tbody > tr {\n",
                             "  text-align: right;\n",
                             "  white-space: pre-wrap;\n",
                             "}\n",
                             "</style>\n",
-                            "<small>shape: (5, 4)</small><table border=\"1\" class=\"dataframe\"><thead><tr><th>a</th><th>[0, 1)</th><th>Normal</th><th>Int from [0, 10)</th></tr><tr><td>f64</td><td>f64</td><td>f64</td><td>i32</td></tr></thead><tbody><tr><td>null</td><td>0.205474</td><td>-1.056756</td><td>5</td></tr><tr><td>null</td><td>0.015194</td><td>0.056542</td><td>4</td></tr><tr><td>0.066091</td><td>0.659457</td><td>-0.101667</td><td>8</td></tr><tr><td>-0.35634</td><td>0.639568</td><td>-2.193398</td><td>7</td></tr><tr><td>1.17341</td><td>0.315957</td><td>-0.790355</td><td>5</td></tr></tbody></table></div>"
+                            "<small>shape: (5, 4)</small><table border=\"1\" class=\"dataframe\"><thead><tr><th>a</th><th>[0, 1)</th><th>Normal</th><th>Int from [0, 10)</th></tr><tr><td>f64</td><td>f64</td><td>f64</td><td>i32</td></tr></thead><tbody><tr><td>null</td><td>0.811185</td><td>1.371197</td><td>9</td></tr><tr><td>null</td><td>0.225194</td><td>0.436565</td><td>2</td></tr><tr><td>-0.233906</td><td>0.286964</td><td>-0.973012</td><td>7</td></tr><tr><td>2.031312</td><td>0.344108</td><td>1.569547</td><td>7</td></tr><tr><td>1.410816</td><td>0.986432</td><td>-0.065434</td><td>8</td></tr></tbody></table></div>"
                         ],
                         "text/plain": [
                             "shape: (5, 4)\n",
-                            "\u250c\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u252c\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u252c\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u252c\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2510\n",
-                            "\u2502 a        \u2506 [0, 1)   \u2506 Normal    \u2506 Int from [0, 10) \u2502\n",
-                            "\u2502 ---      \u2506 ---      \u2506 ---       \u2506 ---              \u2502\n",
-                            "\u2502 f64      \u2506 f64      \u2506 f64       \u2506 i32              \u2502\n",
-                            "\u255e\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u256a\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u256a\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u256a\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2561\n",
-                            "\u2502 null     \u2506 0.205474 \u2506 -1.056756 \u2506 5                \u2502\n",
-                            "\u2502 null     \u2506 0.015194 \u2506 0.056542  \u2506 4                \u2502\n",
-                            "\u2502 0.066091 \u2506 0.659457 \u2506 -0.101667 \u2506 8                \u2502\n",
-                            "\u2502 -0.35634 \u2506 0.639568 \u2506 -2.193398 \u2506 7                \u2502\n",
-                            "\u2502 1.17341  \u2506 0.315957 \u2506 -0.790355 \u2506 5                \u2502\n",
-                            "\u2514\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2534\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2534\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2534\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2518"
+                            "\u250c\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u252c\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u252c\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u252c\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2510\n",
+                            "\u2502 a         \u2506 [0, 1)   \u2506 Normal    \u2506 Int from [0, 10) \u2502\n",
+                            "\u2502 ---       \u2506 ---      \u2506 ---       \u2506 ---              \u2502\n",
+                            "\u2502 f64       \u2506 f64      \u2506 f64       \u2506 i32              \u2502\n",
+                            "\u255e\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u256a\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u256a\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u256a\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2561\n",
+                            "\u2502 null      \u2506 0.811185 \u2506 1.371197  \u2506 9                \u2502\n",
+                            "\u2502 null      \u2506 0.225194 \u2506 0.436565  \u2506 2                \u2502\n",
+                            "\u2502 -0.233906 \u2506 0.286964 \u2506 -0.973012 \u2506 7                \u2502\n",
+                            "\u2502 2.031312  \u2506 0.344108 \u2506 1.569547  \u2506 7                \u2502\n",
+                            "\u2502 1.410816  \u2506 0.986432 \u2506 -0.065434 \u2506 8                \u2502\n",
+                            "\u2514\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2534\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2534\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2534\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2518"
                         ]
                     },
                     "execution_count": 33,
                     "metadata": {},
                     "output_type": "execute_result"
                 }
             ],
@@ -1494,24 +1494,24 @@
                             "<div><style>\n",
                             ".dataframe > thead > tr,\n",
                             ".dataframe > tbody > tr {\n",
                             "  text-align: right;\n",
                             "  white-space: pre-wrap;\n",
                             "}\n",
                             "</style>\n",
-                            "<small>shape: (1, 4)</small><table border=\"1\" class=\"dataframe\"><thead><tr><th>t-tests: statistics</th><th>t-tests: pvalue</th><th>normality_test: statistics</th><th>normality_test: pvalue</th></tr><tr><td>f64</td><td>f64</td><td>f64</td><td>f64</td></tr></thead><tbody><tr><td>-0.261893</td><td>0.793441</td><td>1.747484</td><td>0.417387</td></tr></tbody></table></div>"
+                            "<small>shape: (1, 4)</small><table border=\"1\" class=\"dataframe\"><thead><tr><th>t-tests: statistics</th><th>t-tests: pvalue</th><th>normality_test: statistics</th><th>normality_test: pvalue</th></tr><tr><td>f64</td><td>f64</td><td>f64</td><td>f64</td></tr></thead><tbody><tr><td>1.302671</td><td>0.192892</td><td>0.345933</td><td>0.841166</td></tr></tbody></table></div>"
                         ],
                         "text/plain": [
                             "shape: (1, 4)\n",
                             "\u250c\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u252c\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u252c\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u252c\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2510\n",
                             "\u2502 t-tests: statistics \u2506 t-tests: pvalue \u2506 normality_test: statistics \u2506 normality_test: pvalue \u2502\n",
                             "\u2502 ---                 \u2506 ---             \u2506 ---                        \u2506 ---                    \u2502\n",
                             "\u2502 f64                 \u2506 f64             \u2506 f64                        \u2506 f64                    \u2502\n",
                             "\u255e\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u256a\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u256a\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u256a\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2561\n",
-                            "\u2502 -0.261893           \u2506 0.793441        \u2506 1.747484                   \u2506 0.417387               \u2502\n",
+                            "\u2502 1.302671            \u2506 0.192892        \u2506 0.345933                   \u2506 0.841166               \u2502\n",
                             "\u2514\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2534\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2534\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2534\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2518"
                         ]
                     },
                     "execution_count": 34,
                     "metadata": {},
                     "output_type": "execute_result"
                 }
@@ -1547,28 +1547,28 @@
                             "<div><style>\n",
                             ".dataframe > thead > tr,\n",
                             ".dataframe > tbody > tr {\n",
                             "  text-align: right;\n",
                             "  white-space: pre-wrap;\n",
                             "}\n",
                             "</style>\n",
-                            "<small>shape: (5, 5)</small><table border=\"1\" class=\"dataframe\"><thead><tr><th>market_id</th><th>var1</th><th>var2</th><th>category_1</th><th>category_2</th></tr><tr><td>i64</td><td>f64</td><td>f64</td><td>i32</td><td>i32</td></tr></thead><tbody><tr><td>0</td><td>0.498654</td><td>0.281769</td><td>3</td><td>5</td></tr><tr><td>1</td><td>0.242465</td><td>0.652056</td><td>3</td><td>4</td></tr><tr><td>2</td><td>0.538076</td><td>0.841711</td><td>1</td><td>9</td></tr><tr><td>0</td><td>0.79132</td><td>0.491</td><td>0</td><td>3</td></tr><tr><td>1</td><td>0.827066</td><td>0.551273</td><td>4</td><td>8</td></tr></tbody></table></div>"
+                            "<small>shape: (5, 5)</small><table border=\"1\" class=\"dataframe\"><thead><tr><th>market_id</th><th>var1</th><th>var2</th><th>category_1</th><th>category_2</th></tr><tr><td>i64</td><td>f64</td><td>f64</td><td>i32</td><td>i32</td></tr></thead><tbody><tr><td>0</td><td>0.248869</td><td>0.132532</td><td>0</td><td>9</td></tr><tr><td>1</td><td>0.131251</td><td>0.518646</td><td>3</td><td>9</td></tr><tr><td>2</td><td>0.857064</td><td>0.826533</td><td>3</td><td>7</td></tr><tr><td>0</td><td>0.69999</td><td>0.002881</td><td>2</td><td>3</td></tr><tr><td>1</td><td>0.698539</td><td>0.072711</td><td>0</td><td>7</td></tr></tbody></table></div>"
                         ],
                         "text/plain": [
                             "shape: (5, 5)\n",
                             "\u250c\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u252c\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u252c\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u252c\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u252c\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2510\n",
                             "\u2502 market_id \u2506 var1     \u2506 var2     \u2506 category_1 \u2506 category_2 \u2502\n",
                             "\u2502 ---       \u2506 ---      \u2506 ---      \u2506 ---        \u2506 ---        \u2502\n",
                             "\u2502 i64       \u2506 f64      \u2506 f64      \u2506 i32        \u2506 i32        \u2502\n",
                             "\u255e\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u256a\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u256a\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u256a\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u256a\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2561\n",
-                            "\u2502 0         \u2506 0.498654 \u2506 0.281769 \u2506 3          \u2506 5          \u2502\n",
-                            "\u2502 1         \u2506 0.242465 \u2506 0.652056 \u2506 3          \u2506 4          \u2502\n",
-                            "\u2502 2         \u2506 0.538076 \u2506 0.841711 \u2506 1          \u2506 9          \u2502\n",
-                            "\u2502 0         \u2506 0.79132  \u2506 0.491    \u2506 0          \u2506 3          \u2502\n",
-                            "\u2502 1         \u2506 0.827066 \u2506 0.551273 \u2506 4          \u2506 8          \u2502\n",
+                            "\u2502 0         \u2506 0.248869 \u2506 0.132532 \u2506 0          \u2506 9          \u2502\n",
+                            "\u2502 1         \u2506 0.131251 \u2506 0.518646 \u2506 3          \u2506 9          \u2502\n",
+                            "\u2502 2         \u2506 0.857064 \u2506 0.826533 \u2506 3          \u2506 7          \u2502\n",
+                            "\u2502 0         \u2506 0.69999  \u2506 0.002881 \u2506 2          \u2506 3          \u2502\n",
+                            "\u2502 1         \u2506 0.698539 \u2506 0.072711 \u2506 0          \u2506 7          \u2502\n",
                             "\u2514\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2534\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2534\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2534\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2534\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2518"
                         ]
                     },
                     "execution_count": 35,
                     "metadata": {},
                     "output_type": "execute_result"
                 }
@@ -1600,25 +1600,25 @@
                             "<div><style>\n",
                             ".dataframe > thead > tr,\n",
                             ".dataframe > tbody > tr {\n",
                             "  text-align: right;\n",
                             "  white-space: pre-wrap;\n",
                             "}\n",
                             "</style>\n",
-                            "<small>shape: (1, 3)</small><table border=\"1\" class=\"dataframe\"><thead><tr><th>t-test</th><th>chi2-test</th><th>f-test</th></tr><tr><td>struct[2]</td><td>struct[2]</td><td>struct[2]</td></tr></thead><tbody><tr><td>{-2.204845,0.027488}</td><td>{28.786602,0.798015}</td><td>{1.520127,0.193397}</td></tr></tbody></table></div>"
+                            "<small>shape: (1, 3)</small><table border=\"1\" class=\"dataframe\"><thead><tr><th>t-test</th><th>chi2-test</th><th>f-test</th></tr><tr><td>struct[2]</td><td>struct[2]</td><td>struct[2]</td></tr></thead><tbody><tr><td>{2.150104,0.031571}</td><td>{28.805566,0.797284}</td><td>{1.22338,0.298549}</td></tr></tbody></table></div>"
                         ],
                         "text/plain": [
                             "shape: (1, 3)\n",
-                            "\u250c\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u252c\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u252c\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2510\n",
-                            "\u2502 t-test               \u2506 chi2-test            \u2506 f-test              \u2502\n",
-                            "\u2502 ---                  \u2506 ---                  \u2506 ---                 \u2502\n",
-                            "\u2502 struct[2]            \u2506 struct[2]            \u2506 struct[2]           \u2502\n",
-                            "\u255e\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u256a\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u256a\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2561\n",
-                            "\u2502 {-2.204845,0.027488} \u2506 {28.786602,0.798015} \u2506 {1.520127,0.193397} \u2502\n",
-                            "\u2514\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2534\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2534\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2518"
+                            "\u250c\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u252c\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u252c\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2510\n",
+                            "\u2502 t-test              \u2506 chi2-test            \u2506 f-test             \u2502\n",
+                            "\u2502 ---                 \u2506 ---                  \u2506 ---                \u2502\n",
+                            "\u2502 struct[2]           \u2506 struct[2]            \u2506 struct[2]          \u2502\n",
+                            "\u255e\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u256a\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u256a\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2561\n",
+                            "\u2502 {2.150104,0.031571} \u2506 {28.805566,0.797284} \u2506 {1.22338,0.298549} \u2502\n",
+                            "\u2514\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2534\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2534\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2518"
                         ]
                     },
                     "execution_count": 36,
                     "metadata": {},
                     "output_type": "execute_result"
                 }
             ],
@@ -1643,26 +1643,26 @@
                             "<div><style>\n",
                             ".dataframe > thead > tr,\n",
                             ".dataframe > tbody > tr {\n",
                             "  text-align: right;\n",
                             "  white-space: pre-wrap;\n",
                             "}\n",
                             "</style>\n",
-                            "<small>shape: (3, 4)</small><table border=\"1\" class=\"dataframe\"><thead><tr><th>market_id</th><th>t-test</th><th>chi2-test</th><th>f-test</th></tr><tr><td>i64</td><td>struct[2]</td><td>struct[2]</td><td>struct[2]</td></tr></thead><tbody><tr><td>0</td><td>{-1.118248,0.263541}</td><td>{38.128166,0.372848}</td><td>{0.758698,0.552177}</td></tr><tr><td>1</td><td>{-1.29356,0.195907}</td><td>{31.584237,0.678621}</td><td>{0.67456,0.609622}</td></tr><tr><td>2</td><td>{-1.405805,0.159875}</td><td>{36.244973,0.457224}</td><td>{2.309402,0.055886}</td></tr></tbody></table></div>"
+                            "<small>shape: (3, 4)</small><table border=\"1\" class=\"dataframe\"><thead><tr><th>market_id</th><th>t-test</th><th>chi2-test</th><th>f-test</th></tr><tr><td>i64</td><td>struct[2]</td><td>struct[2]</td><td>struct[2]</td></tr></thead><tbody><tr><td>0</td><td>{2.054032,0.04005}</td><td>{33.167495,0.604033}</td><td>{1.670606,0.154209}</td></tr><tr><td>1</td><td>{-0.340076,0.733821}</td><td>{36.485591,0.446087}</td><td>{0.702859,0.589979}</td></tr><tr><td>2</td><td>{1.995052,0.046119}</td><td>{34.837296,0.523782}</td><td>{1.159508,0.326912}</td></tr></tbody></table></div>"
                         ],
                         "text/plain": [
                             "shape: (3, 4)\n",
                             "\u250c\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u252c\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u252c\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u252c\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2510\n",
                             "\u2502 market_id \u2506 t-test               \u2506 chi2-test            \u2506 f-test              \u2502\n",
                             "\u2502 ---       \u2506 ---                  \u2506 ---                  \u2506 ---                 \u2502\n",
                             "\u2502 i64       \u2506 struct[2]            \u2506 struct[2]            \u2506 struct[2]           \u2502\n",
                             "\u255e\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u256a\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u256a\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u256a\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2561\n",
-                            "\u2502 0         \u2506 {-1.118248,0.263541} \u2506 {38.128166,0.372848} \u2506 {0.758698,0.552177} \u2502\n",
-                            "\u2502 1         \u2506 {-1.29356,0.195907}  \u2506 {31.584237,0.678621} \u2506 {0.67456,0.609622}  \u2502\n",
-                            "\u2502 2         \u2506 {-1.405805,0.159875} \u2506 {36.244973,0.457224} \u2506 {2.309402,0.055886} \u2502\n",
+                            "\u2502 0         \u2506 {2.054032,0.04005}   \u2506 {33.167495,0.604033} \u2506 {1.670606,0.154209} \u2502\n",
+                            "\u2502 1         \u2506 {-0.340076,0.733821} \u2506 {36.485591,0.446087} \u2506 {0.702859,0.589979} \u2502\n",
+                            "\u2502 2         \u2506 {1.995052,0.046119}  \u2506 {34.837296,0.523782} \u2506 {1.159508,0.326912} \u2502\n",
                             "\u2514\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2534\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2534\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2534\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2518"
                         ]
                     },
                     "execution_count": 37,
                     "metadata": {},
                     "output_type": "execute_result"
                 }
@@ -1719,28 +1719,28 @@
                             "<div><style>\n",
                             ".dataframe > thead > tr,\n",
                             ".dataframe > tbody > tr {\n",
                             "  text-align: right;\n",
                             "  white-space: pre-wrap;\n",
                             "}\n",
                             "</style>\n",
-                            "<small>shape: (5, 7)</small><table border=\"1\" class=\"dataframe\"><thead><tr><th>id</th><th>var1</th><th>var2</th><th>var3</th><th>r</th><th>rh</th><th>nb_l_inf_cnt</th></tr><tr><td>u32</td><td>f64</td><td>f64</td><td>f64</td><td>f64</td><td>f64</td><td>u32</td></tr></thead><tbody><tr><td>0</td><td>0.850509</td><td>0.03804</td><td>0.700016</td><td>0.682363</td><td>0.504606</td><td>9</td></tr><tr><td>1</td><td>0.646007</td><td>0.384087</td><td>0.533855</td><td>0.30102</td><td>1.695952</td><td>11</td></tr><tr><td>2</td><td>0.952063</td><td>0.354422</td><td>0.640121</td><td>0.37486</td><td>9.210626</td><td>13</td></tr><tr><td>3</td><td>0.765802</td><td>0.0884</td><td>0.266615</td><td>0.497384</td><td>8.343505</td><td>27</td></tr><tr><td>4</td><td>0.17171</td><td>0.500247</td><td>0.12381</td><td>0.733858</td><td>1.715458</td><td>14</td></tr></tbody></table></div>"
+                            "<small>shape: (5, 7)</small><table border=\"1\" class=\"dataframe\"><thead><tr><th>id</th><th>var1</th><th>var2</th><th>var3</th><th>r</th><th>rh</th><th>nb_l_inf_cnt</th></tr><tr><td>u32</td><td>f64</td><td>f64</td><td>f64</td><td>f64</td><td>f64</td><td>u32</td></tr></thead><tbody><tr><td>0</td><td>0.911672</td><td>0.819826</td><td>0.986483</td><td>0.437032</td><td>7.519072</td><td>10</td></tr><tr><td>1</td><td>0.59381</td><td>0.496358</td><td>0.765642</td><td>0.08905</td><td>0.527819</td><td>12</td></tr><tr><td>2</td><td>0.651759</td><td>0.473416</td><td>0.654051</td><td>0.772629</td><td>3.989873</td><td>10</td></tr><tr><td>3</td><td>0.588802</td><td>0.095334</td><td>0.51503</td><td>0.893853</td><td>7.933253</td><td>24</td></tr><tr><td>4</td><td>0.862729</td><td>0.695517</td><td>0.712502</td><td>0.821449</td><td>7.214843</td><td>11</td></tr></tbody></table></div>"
                         ],
                         "text/plain": [
                             "shape: (5, 7)\n",
                             "\u250c\u2500\u2500\u2500\u2500\u2500\u252c\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u252c\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u252c\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u252c\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u252c\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u252c\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2510\n",
                             "\u2502 id  \u2506 var1     \u2506 var2     \u2506 var3     \u2506 r        \u2506 rh       \u2506 nb_l_inf_cnt \u2502\n",
                             "\u2502 --- \u2506 ---      \u2506 ---      \u2506 ---      \u2506 ---      \u2506 ---      \u2506 ---          \u2502\n",
                             "\u2502 u32 \u2506 f64      \u2506 f64      \u2506 f64      \u2506 f64      \u2506 f64      \u2506 u32          \u2502\n",
                             "\u255e\u2550\u2550\u2550\u2550\u2550\u256a\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u256a\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u256a\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u256a\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u256a\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u256a\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2561\n",
-                            "\u2502 0   \u2506 0.850509 \u2506 0.03804  \u2506 0.700016 \u2506 0.682363 \u2506 0.504606 \u2506 9            \u2502\n",
-                            "\u2502 1   \u2506 0.646007 \u2506 0.384087 \u2506 0.533855 \u2506 0.30102  \u2506 1.695952 \u2506 11           \u2502\n",
-                            "\u2502 2   \u2506 0.952063 \u2506 0.354422 \u2506 0.640121 \u2506 0.37486  \u2506 9.210626 \u2506 13           \u2502\n",
-                            "\u2502 3   \u2506 0.765802 \u2506 0.0884   \u2506 0.266615 \u2506 0.497384 \u2506 8.343505 \u2506 27           \u2502\n",
-                            "\u2502 4   \u2506 0.17171  \u2506 0.500247 \u2506 0.12381  \u2506 0.733858 \u2506 1.715458 \u2506 14           \u2502\n",
+                            "\u2502 0   \u2506 0.911672 \u2506 0.819826 \u2506 0.986483 \u2506 0.437032 \u2506 7.519072 \u2506 10           \u2502\n",
+                            "\u2502 1   \u2506 0.59381  \u2506 0.496358 \u2506 0.765642 \u2506 0.08905  \u2506 0.527819 \u2506 12           \u2502\n",
+                            "\u2502 2   \u2506 0.651759 \u2506 0.473416 \u2506 0.654051 \u2506 0.772629 \u2506 3.989873 \u2506 10           \u2502\n",
+                            "\u2502 3   \u2506 0.588802 \u2506 0.095334 \u2506 0.51503  \u2506 0.893853 \u2506 7.933253 \u2506 24           \u2502\n",
+                            "\u2502 4   \u2506 0.862729 \u2506 0.695517 \u2506 0.712502 \u2506 0.821449 \u2506 7.214843 \u2506 11           \u2502\n",
                             "\u2514\u2500\u2500\u2500\u2500\u2500\u2534\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2534\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2534\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2534\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2534\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2534\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2518"
                         ]
                     },
                     "execution_count": 39,
                     "metadata": {},
                     "output_type": "execute_result"
                 }
@@ -1769,28 +1769,28 @@
                             "<div><style>\n",
                             ".dataframe > thead > tr,\n",
                             ".dataframe > tbody > tr {\n",
                             "  text-align: right;\n",
                             "  white-space: pre-wrap;\n",
                             "}\n",
                             "</style>\n",
-                            "<small>shape: (5, 7)</small><table border=\"1\" class=\"dataframe\"><thead><tr><th>id</th><th>var1</th><th>var2</th><th>var3</th><th>r</th><th>rh</th><th>nb_l1_r_cnt</th></tr><tr><td>u32</td><td>f64</td><td>f64</td><td>f64</td><td>f64</td><td>f64</td><td>u32</td></tr></thead><tbody><tr><td>0</td><td>0.850509</td><td>0.03804</td><td>0.700016</td><td>0.682363</td><td>0.504606</td><td>352</td></tr><tr><td>1</td><td>0.646007</td><td>0.384087</td><td>0.533855</td><td>0.30102</td><td>1.695952</td><td>71</td></tr><tr><td>2</td><td>0.952063</td><td>0.354422</td><td>0.640121</td><td>0.37486</td><td>9.210626</td><td>99</td></tr><tr><td>3</td><td>0.765802</td><td>0.0884</td><td>0.266615</td><td>0.497384</td><td>8.343505</td><td>199</td></tr><tr><td>4</td><td>0.17171</td><td>0.500247</td><td>0.12381</td><td>0.733858</td><td>1.715458</td><td>523</td></tr></tbody></table></div>"
+                            "<small>shape: (5, 7)</small><table border=\"1\" class=\"dataframe\"><thead><tr><th>id</th><th>var1</th><th>var2</th><th>var3</th><th>r</th><th>rh</th><th>nb_l1_r_cnt</th></tr><tr><td>u32</td><td>f64</td><td>f64</td><td>f64</td><td>f64</td><td>f64</td><td>u32</td></tr></thead><tbody><tr><td>0</td><td>0.911672</td><td>0.819826</td><td>0.986483</td><td>0.437032</td><td>7.519072</td><td>74</td></tr><tr><td>1</td><td>0.59381</td><td>0.496358</td><td>0.765642</td><td>0.08905</td><td>0.527819</td><td>1</td></tr><tr><td>2</td><td>0.651759</td><td>0.473416</td><td>0.654051</td><td>0.772629</td><td>3.989873</td><td>968</td></tr><tr><td>3</td><td>0.588802</td><td>0.095334</td><td>0.51503</td><td>0.893853</td><td>7.933253</td><td>927</td></tr><tr><td>4</td><td>0.862729</td><td>0.695517</td><td>0.712502</td><td>0.821449</td><td>7.214843</td><td>727</td></tr></tbody></table></div>"
                         ],
                         "text/plain": [
                             "shape: (5, 7)\n",
                             "\u250c\u2500\u2500\u2500\u2500\u2500\u252c\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u252c\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u252c\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u252c\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u252c\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u252c\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2510\n",
                             "\u2502 id  \u2506 var1     \u2506 var2     \u2506 var3     \u2506 r        \u2506 rh       \u2506 nb_l1_r_cnt \u2502\n",
                             "\u2502 --- \u2506 ---      \u2506 ---      \u2506 ---      \u2506 ---      \u2506 ---      \u2506 ---         \u2502\n",
                             "\u2502 u32 \u2506 f64      \u2506 f64      \u2506 f64      \u2506 f64      \u2506 f64      \u2506 u32         \u2502\n",
                             "\u255e\u2550\u2550\u2550\u2550\u2550\u256a\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u256a\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u256a\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u256a\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u256a\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u256a\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2561\n",
-                            "\u2502 0   \u2506 0.850509 \u2506 0.03804  \u2506 0.700016 \u2506 0.682363 \u2506 0.504606 \u2506 352         \u2502\n",
-                            "\u2502 1   \u2506 0.646007 \u2506 0.384087 \u2506 0.533855 \u2506 0.30102  \u2506 1.695952 \u2506 71          \u2502\n",
-                            "\u2502 2   \u2506 0.952063 \u2506 0.354422 \u2506 0.640121 \u2506 0.37486  \u2506 9.210626 \u2506 99          \u2502\n",
-                            "\u2502 3   \u2506 0.765802 \u2506 0.0884   \u2506 0.266615 \u2506 0.497384 \u2506 8.343505 \u2506 199         \u2502\n",
-                            "\u2502 4   \u2506 0.17171  \u2506 0.500247 \u2506 0.12381  \u2506 0.733858 \u2506 1.715458 \u2506 523         \u2502\n",
+                            "\u2502 0   \u2506 0.911672 \u2506 0.819826 \u2506 0.986483 \u2506 0.437032 \u2506 7.519072 \u2506 74          \u2502\n",
+                            "\u2502 1   \u2506 0.59381  \u2506 0.496358 \u2506 0.765642 \u2506 0.08905  \u2506 0.527819 \u2506 1           \u2502\n",
+                            "\u2502 2   \u2506 0.651759 \u2506 0.473416 \u2506 0.654051 \u2506 0.772629 \u2506 3.989873 \u2506 968         \u2502\n",
+                            "\u2502 3   \u2506 0.588802 \u2506 0.095334 \u2506 0.51503  \u2506 0.893853 \u2506 7.933253 \u2506 927         \u2502\n",
+                            "\u2502 4   \u2506 0.862729 \u2506 0.695517 \u2506 0.712502 \u2506 0.821449 \u2506 7.214843 \u2506 727         \u2502\n",
                             "\u2514\u2500\u2500\u2500\u2500\u2500\u2534\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2534\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2534\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2534\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2534\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2534\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2518"
                         ]
                     },
                     "execution_count": 40,
                     "metadata": {},
                     "output_type": "execute_result"
                 }
@@ -1818,28 +1818,28 @@
                             "<div><style>\n",
                             ".dataframe > thead > tr,\n",
                             ".dataframe > tbody > tr {\n",
                             "  text-align: right;\n",
                             "  white-space: pre-wrap;\n",
                             "}\n",
                             "</style>\n",
-                            "<small>shape: (5, 7)</small><table border=\"1\" class=\"dataframe\"><thead><tr><th>id</th><th>var1</th><th>var2</th><th>var3</th><th>r</th><th>rh</th><th>best friends</th></tr><tr><td>u32</td><td>f64</td><td>f64</td><td>f64</td><td>f64</td><td>f64</td><td>list[u32]</td></tr></thead><tbody><tr><td>0</td><td>0.850509</td><td>0.03804</td><td>0.700016</td><td>0.682363</td><td>0.504606</td><td>[0, 1537, \u2026 1065]</td></tr><tr><td>1</td><td>0.646007</td><td>0.384087</td><td>0.533855</td><td>0.30102</td><td>1.695952</td><td>[1, 729, \u2026 377]</td></tr><tr><td>2</td><td>0.952063</td><td>0.354422</td><td>0.640121</td><td>0.37486</td><td>9.210626</td><td>[2, 1246, \u2026 1666]</td></tr><tr><td>3</td><td>0.765802</td><td>0.0884</td><td>0.266615</td><td>0.497384</td><td>8.343505</td><td>[3, 898, \u2026 631]</td></tr><tr><td>4</td><td>0.17171</td><td>0.500247</td><td>0.12381</td><td>0.733858</td><td>1.715458</td><td>[4, 1096, \u2026 165]</td></tr></tbody></table></div>"
+                            "<small>shape: (5, 7)</small><table border=\"1\" class=\"dataframe\"><thead><tr><th>id</th><th>var1</th><th>var2</th><th>var3</th><th>r</th><th>rh</th><th>best friends</th></tr><tr><td>u32</td><td>f64</td><td>f64</td><td>f64</td><td>f64</td><td>f64</td><td>list[u32]</td></tr></thead><tbody><tr><td>0</td><td>0.911672</td><td>0.819826</td><td>0.986483</td><td>0.437032</td><td>7.519072</td><td>[0, 373, \u2026 1018]</td></tr><tr><td>1</td><td>0.59381</td><td>0.496358</td><td>0.765642</td><td>0.08905</td><td>0.527819</td><td>[1, 657, \u2026 1806]</td></tr><tr><td>2</td><td>0.651759</td><td>0.473416</td><td>0.654051</td><td>0.772629</td><td>3.989873</td><td>[2, 1547, \u2026 1624]</td></tr><tr><td>3</td><td>0.588802</td><td>0.095334</td><td>0.51503</td><td>0.893853</td><td>7.933253</td><td>[3, 1431, \u2026 890]</td></tr><tr><td>4</td><td>0.862729</td><td>0.695517</td><td>0.712502</td><td>0.821449</td><td>7.214843</td><td>[4, 1456, \u2026 1332]</td></tr></tbody></table></div>"
                         ],
                         "text/plain": [
                             "shape: (5, 7)\n",
                             "\u250c\u2500\u2500\u2500\u2500\u2500\u252c\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u252c\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u252c\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u252c\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u252c\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u252c\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2510\n",
                             "\u2502 id  \u2506 var1     \u2506 var2     \u2506 var3     \u2506 r        \u2506 rh       \u2506 best friends      \u2502\n",
                             "\u2502 --- \u2506 ---      \u2506 ---      \u2506 ---      \u2506 ---      \u2506 ---      \u2506 ---               \u2502\n",
                             "\u2502 u32 \u2506 f64      \u2506 f64      \u2506 f64      \u2506 f64      \u2506 f64      \u2506 list[u32]         \u2502\n",
                             "\u255e\u2550\u2550\u2550\u2550\u2550\u256a\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u256a\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u256a\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u256a\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u256a\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u256a\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2561\n",
-                            "\u2502 0   \u2506 0.850509 \u2506 0.03804  \u2506 0.700016 \u2506 0.682363 \u2506 0.504606 \u2506 [0, 1537, \u2026 1065] \u2502\n",
-                            "\u2502 1   \u2506 0.646007 \u2506 0.384087 \u2506 0.533855 \u2506 0.30102  \u2506 1.695952 \u2506 [1, 729, \u2026 377]   \u2502\n",
-                            "\u2502 2   \u2506 0.952063 \u2506 0.354422 \u2506 0.640121 \u2506 0.37486  \u2506 9.210626 \u2506 [2, 1246, \u2026 1666] \u2502\n",
-                            "\u2502 3   \u2506 0.765802 \u2506 0.0884   \u2506 0.266615 \u2506 0.497384 \u2506 8.343505 \u2506 [3, 898, \u2026 631]   \u2502\n",
-                            "\u2502 4   \u2506 0.17171  \u2506 0.500247 \u2506 0.12381  \u2506 0.733858 \u2506 1.715458 \u2506 [4, 1096, \u2026 165]  \u2502\n",
+                            "\u2502 0   \u2506 0.911672 \u2506 0.819826 \u2506 0.986483 \u2506 0.437032 \u2506 7.519072 \u2506 [0, 373, \u2026 1018]  \u2502\n",
+                            "\u2502 1   \u2506 0.59381  \u2506 0.496358 \u2506 0.765642 \u2506 0.08905  \u2506 0.527819 \u2506 [1, 657, \u2026 1806]  \u2502\n",
+                            "\u2502 2   \u2506 0.651759 \u2506 0.473416 \u2506 0.654051 \u2506 0.772629 \u2506 3.989873 \u2506 [2, 1547, \u2026 1624] \u2502\n",
+                            "\u2502 3   \u2506 0.588802 \u2506 0.095334 \u2506 0.51503  \u2506 0.893853 \u2506 7.933253 \u2506 [3, 1431, \u2026 890]  \u2502\n",
+                            "\u2502 4   \u2506 0.862729 \u2506 0.695517 \u2506 0.712502 \u2506 0.821449 \u2506 7.214843 \u2506 [4, 1456, \u2026 1332] \u2502\n",
                             "\u2514\u2500\u2500\u2500\u2500\u2500\u2534\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2534\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2534\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2534\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2534\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2534\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2518"
                         ]
                     },
                     "execution_count": 41,
                     "metadata": {},
                     "output_type": "execute_result"
                 }
@@ -1865,25 +1865,25 @@
             "metadata": {},
             "outputs": [
                 {
                     "name": "stdout",
                     "output_type": "stream",
                     "text": [
                         "shape: (5, 3)\n",
-                        "\u250c\u2500\u2500\u2500\u2500\u2500\u252c\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u252c\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2510\n",
-                        "\u2502 id  \u2506 best friends      \u2506 best friends count \u2502\n",
-                        "\u2502 --- \u2506 ---               \u2506 ---                \u2502\n",
-                        "\u2502 u32 \u2506 list[u32]         \u2506 u32                \u2502\n",
-                        "\u255e\u2550\u2550\u2550\u2550\u2550\u256a\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u256a\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2561\n",
-                        "\u2502 0   \u2506 [0, 1537, \u2026 298]  \u2506 140                \u2502\n",
-                        "\u2502 1   \u2506 [1, 729, \u2026 1477]  \u2506 266                \u2502\n",
-                        "\u2502 2   \u2506 [2, 1246, \u2026 1619] \u2506 172                \u2502\n",
-                        "\u2502 3   \u2506 [3, 898, \u2026 811]   \u2506 172                \u2502\n",
-                        "\u2502 4   \u2506 [4, 1096, \u2026 461]  \u2506 160                \u2502\n",
-                        "\u2514\u2500\u2500\u2500\u2500\u2500\u2534\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2534\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2518\n"
+                        "\u250c\u2500\u2500\u2500\u2500\u2500\u252c\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u252c\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2510\n",
+                        "\u2502 id  \u2506 best friends     \u2506 best friends count \u2502\n",
+                        "\u2502 --- \u2506 ---              \u2506 ---                \u2502\n",
+                        "\u2502 u32 \u2506 list[u32]        \u2506 u32                \u2502\n",
+                        "\u255e\u2550\u2550\u2550\u2550\u2550\u256a\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u256a\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2561\n",
+                        "\u2502 0   \u2506 [0, 373, \u2026 1538] \u2506 71                 \u2502\n",
+                        "\u2502 1   \u2506 [1, 657, \u2026 1292] \u2506 253                \u2502\n",
+                        "\u2502 2   \u2506 [2, 1547, \u2026 21]  \u2506 249                \u2502\n",
+                        "\u2502 3   \u2506 [3, 1431, \u2026 724] \u2506 213                \u2502\n",
+                        "\u2502 4   \u2506 [4, 1456, \u2026 152] \u2506 202                \u2502\n",
+                        "\u2514\u2500\u2500\u2500\u2500\u2500\u2534\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2534\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2518\n"
                     ]
                 }
             ],
             "source": [
                 "# Get all neighbors within radius r\n",
                 "# The point itself is always considered a neighbor to itself.\n",
                 "print(df.select(\n",
@@ -1912,33 +1912,33 @@
                             "<div><style>\n",
                             ".dataframe > thead > tr,\n",
                             ".dataframe > tbody > tr {\n",
                             "  text-align: right;\n",
                             "  white-space: pre-wrap;\n",
                             "}\n",
                             "</style>\n",
-                            "<small>shape: (5, 8)</small><table border=\"1\" class=\"dataframe\"><thead><tr><th>id</th><th>var1</th><th>var2</th><th>var3</th><th>r</th><th>rh</th><th>idx</th><th>dist</th></tr><tr><td>u32</td><td>f64</td><td>f64</td><td>f64</td><td>f64</td><td>f64</td><td>list[u32]</td><td>list[f64]</td></tr></thead><tbody><tr><td>0</td><td>0.850509</td><td>0.03804</td><td>0.700016</td><td>0.682363</td><td>0.504606</td><td>[0, 1537, \u2026 1065]</td><td>[0.0, 0.0013, \u2026 0.006013]</td></tr><tr><td>1</td><td>0.646007</td><td>0.384087</td><td>0.533855</td><td>0.30102</td><td>1.695952</td><td>[1, 729, \u2026 377]</td><td>[0.0, 0.003972, \u2026 0.006201]</td></tr><tr><td>2</td><td>0.952063</td><td>0.354422</td><td>0.640121</td><td>0.37486</td><td>9.210626</td><td>[2, 1246, \u2026 1666]</td><td>[0.0, 0.001598, \u2026 0.003286]</td></tr><tr><td>3</td><td>0.765802</td><td>0.0884</td><td>0.266615</td><td>0.497384</td><td>8.343505</td><td>[3, 898, \u2026 631]</td><td>[0.0, 0.001056, \u2026 0.003583]</td></tr><tr><td>4</td><td>0.17171</td><td>0.500247</td><td>0.12381</td><td>0.733858</td><td>1.715458</td><td>[4, 1096, \u2026 165]</td><td>[0.0, 0.001941, \u2026 0.007024]</td></tr></tbody></table></div>"
+                            "<small>shape: (5, 8)</small><table border=\"1\" class=\"dataframe\"><thead><tr><th>id</th><th>var1</th><th>var2</th><th>var3</th><th>r</th><th>rh</th><th>idx</th><th>dist</th></tr><tr><td>u32</td><td>f64</td><td>f64</td><td>f64</td><td>f64</td><td>f64</td><td>list[u32]</td><td>list[f64]</td></tr></thead><tbody><tr><td>0</td><td>0.911672</td><td>0.819826</td><td>0.986483</td><td>0.437032</td><td>7.519072</td><td>[0, 373, \u2026 1018]</td><td>[0.0, 0.000565, \u2026 0.007648]</td></tr><tr><td>1</td><td>0.59381</td><td>0.496358</td><td>0.765642</td><td>0.08905</td><td>0.527819</td><td>[1, 657, \u2026 1806]</td><td>[0.0, 0.004691, \u2026 0.006369]</td></tr><tr><td>2</td><td>0.651759</td><td>0.473416</td><td>0.654051</td><td>0.772629</td><td>3.989873</td><td>[2, 1547, \u2026 1624]</td><td>[0.0, 0.004597, \u2026 0.005537]</td></tr><tr><td>3</td><td>0.588802</td><td>0.095334</td><td>0.51503</td><td>0.893853</td><td>7.933253</td><td>[3, 1431, \u2026 890]</td><td>[0.0, 0.002061, \u2026 0.002906]</td></tr><tr><td>4</td><td>0.862729</td><td>0.695517</td><td>0.712502</td><td>0.821449</td><td>7.214843</td><td>[4, 1456, \u2026 1332]</td><td>[0.0, 0.004749, \u2026 0.006297]</td></tr></tbody></table></div>"
                         ],
                         "text/plain": [
                             "shape: (5, 8)\n",
                             "\u250c\u2500\u2500\u2500\u2500\u2500\u252c\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u252c\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u252c\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u252c\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u252c\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u252c\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u252c\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2510\n",
                             "\u2502 id  \u2506 var1     \u2506 var2     \u2506 var3     \u2506 r        \u2506 rh       \u2506 idx              \u2506 dist             \u2502\n",
                             "\u2502 --- \u2506 ---      \u2506 ---      \u2506 ---      \u2506 ---      \u2506 ---      \u2506 ---              \u2506 ---              \u2502\n",
                             "\u2502 u32 \u2506 f64      \u2506 f64      \u2506 f64      \u2506 f64      \u2506 f64      \u2506 list[u32]        \u2506 list[f64]        \u2502\n",
                             "\u255e\u2550\u2550\u2550\u2550\u2550\u256a\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u256a\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u256a\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u256a\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u256a\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u256a\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u256a\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2561\n",
-                            "\u2502 0   \u2506 0.850509 \u2506 0.03804  \u2506 0.700016 \u2506 0.682363 \u2506 0.504606 \u2506 [0, 1537, \u2026      \u2506 [0.0, 0.0013, \u2026  \u2502\n",
-                            "\u2502     \u2506          \u2506          \u2506          \u2506          \u2506          \u2506 1065]            \u2506 0.006013]        \u2502\n",
-                            "\u2502 1   \u2506 0.646007 \u2506 0.384087 \u2506 0.533855 \u2506 0.30102  \u2506 1.695952 \u2506 [1, 729, \u2026 377]  \u2506 [0.0, 0.003972,  \u2502\n",
-                            "\u2502     \u2506          \u2506          \u2506          \u2506          \u2506          \u2506                  \u2506 \u2026 0.006201]      \u2502\n",
-                            "\u2502 2   \u2506 0.952063 \u2506 0.354422 \u2506 0.640121 \u2506 0.37486  \u2506 9.210626 \u2506 [2, 1246, \u2026      \u2506 [0.0, 0.001598,  \u2502\n",
-                            "\u2502     \u2506          \u2506          \u2506          \u2506          \u2506          \u2506 1666]            \u2506 \u2026 0.003286]      \u2502\n",
-                            "\u2502 3   \u2506 0.765802 \u2506 0.0884   \u2506 0.266615 \u2506 0.497384 \u2506 8.343505 \u2506 [3, 898, \u2026 631]  \u2506 [0.0, 0.001056,  \u2502\n",
-                            "\u2502     \u2506          \u2506          \u2506          \u2506          \u2506          \u2506                  \u2506 \u2026 0.003583]      \u2502\n",
-                            "\u2502 4   \u2506 0.17171  \u2506 0.500247 \u2506 0.12381  \u2506 0.733858 \u2506 1.715458 \u2506 [4, 1096, \u2026 165] \u2506 [0.0, 0.001941,  \u2502\n",
-                            "\u2502     \u2506          \u2506          \u2506          \u2506          \u2506          \u2506                  \u2506 \u2026 0.007024]      \u2502\n",
+                            "\u2502 0   \u2506 0.911672 \u2506 0.819826 \u2506 0.986483 \u2506 0.437032 \u2506 7.519072 \u2506 [0, 373, \u2026 1018] \u2506 [0.0, 0.000565,  \u2502\n",
+                            "\u2502     \u2506          \u2506          \u2506          \u2506          \u2506          \u2506                  \u2506 \u2026 0.007648]      \u2502\n",
+                            "\u2502 1   \u2506 0.59381  \u2506 0.496358 \u2506 0.765642 \u2506 0.08905  \u2506 0.527819 \u2506 [1, 657, \u2026 1806] \u2506 [0.0, 0.004691,  \u2502\n",
+                            "\u2502     \u2506          \u2506          \u2506          \u2506          \u2506          \u2506                  \u2506 \u2026 0.006369]      \u2502\n",
+                            "\u2502 2   \u2506 0.651759 \u2506 0.473416 \u2506 0.654051 \u2506 0.772629 \u2506 3.989873 \u2506 [2, 1547, \u2026      \u2506 [0.0, 0.004597,  \u2502\n",
+                            "\u2502     \u2506          \u2506          \u2506          \u2506          \u2506          \u2506 1624]            \u2506 \u2026 0.005537]      \u2502\n",
+                            "\u2502 3   \u2506 0.588802 \u2506 0.095334 \u2506 0.51503  \u2506 0.893853 \u2506 7.933253 \u2506 [3, 1431, \u2026 890] \u2506 [0.0, 0.002061,  \u2502\n",
+                            "\u2502     \u2506          \u2506          \u2506          \u2506          \u2506          \u2506                  \u2506 \u2026 0.002906]      \u2502\n",
+                            "\u2502 4   \u2506 0.862729 \u2506 0.695517 \u2506 0.712502 \u2506 0.821449 \u2506 7.214843 \u2506 [4, 1456, \u2026      \u2506 [0.0, 0.004749,  \u2502\n",
+                            "\u2502     \u2506          \u2506          \u2506          \u2506          \u2506          \u2506 1332]            \u2506 \u2026 0.006297]      \u2502\n",
                             "\u2514\u2500\u2500\u2500\u2500\u2500\u2534\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2534\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2534\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2534\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2534\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2534\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2534\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2518"
                         ]
                     },
                     "execution_count": 43,
                     "metadata": {},
                     "output_type": "execute_result"
                 }
@@ -1970,28 +1970,28 @@
                             "<div><style>\n",
                             ".dataframe > thead > tr,\n",
                             ".dataframe > tbody > tr {\n",
                             "  text-align: right;\n",
                             "  white-space: pre-wrap;\n",
                             "}\n",
                             "</style>\n",
-                            "<small>shape: (5, 6)</small><table border=\"1\" class=\"dataframe\"><thead><tr><th>id</th><th>var1</th><th>var2</th><th>var3</th><th>r</th><th>rh</th></tr><tr><td>u32</td><td>f64</td><td>f64</td><td>f64</td><td>f64</td><td>f64</td></tr></thead><tbody><tr><td>1</td><td>0.646007</td><td>0.384087</td><td>0.533855</td><td>0.30102</td><td>1.695952</td></tr><tr><td>6</td><td>0.356637</td><td>0.916926</td><td>0.509538</td><td>0.344282</td><td>5.110688</td></tr><tr><td>7</td><td>0.489873</td><td>0.351803</td><td>0.861379</td><td>0.985876</td><td>3.487034</td></tr><tr><td>8</td><td>0.485547</td><td>0.796377</td><td>0.776287</td><td>0.102771</td><td>9.366586</td></tr><tr><td>11</td><td>0.548642</td><td>0.621415</td><td>0.179476</td><td>0.942682</td><td>9.447275</td></tr></tbody></table></div>"
+                            "<small>shape: (5, 6)</small><table border=\"1\" class=\"dataframe\"><thead><tr><th>id</th><th>var1</th><th>var2</th><th>var3</th><th>r</th><th>rh</th></tr><tr><td>u32</td><td>f64</td><td>f64</td><td>f64</td><td>f64</td><td>f64</td></tr></thead><tbody><tr><td>1</td><td>0.59381</td><td>0.496358</td><td>0.765642</td><td>0.08905</td><td>0.527819</td></tr><tr><td>2</td><td>0.651759</td><td>0.473416</td><td>0.654051</td><td>0.772629</td><td>3.989873</td></tr><tr><td>3</td><td>0.588802</td><td>0.095334</td><td>0.51503</td><td>0.893853</td><td>7.933253</td></tr><tr><td>7</td><td>0.825937</td><td>0.670161</td><td>0.397054</td><td>0.902048</td><td>0.030179</td></tr><tr><td>8</td><td>0.835848</td><td>0.712411</td><td>0.478414</td><td>0.024903</td><td>6.137378</td></tr></tbody></table></div>"
                         ],
                         "text/plain": [
                             "shape: (5, 6)\n",
                             "\u250c\u2500\u2500\u2500\u2500\u2500\u252c\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u252c\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u252c\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u252c\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u252c\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2510\n",
                             "\u2502 id  \u2506 var1     \u2506 var2     \u2506 var3     \u2506 r        \u2506 rh       \u2502\n",
                             "\u2502 --- \u2506 ---      \u2506 ---      \u2506 ---      \u2506 ---      \u2506 ---      \u2502\n",
                             "\u2502 u32 \u2506 f64      \u2506 f64      \u2506 f64      \u2506 f64      \u2506 f64      \u2502\n",
                             "\u255e\u2550\u2550\u2550\u2550\u2550\u256a\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u256a\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u256a\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u256a\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u256a\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2561\n",
-                            "\u2502 1   \u2506 0.646007 \u2506 0.384087 \u2506 0.533855 \u2506 0.30102  \u2506 1.695952 \u2502\n",
-                            "\u2502 6   \u2506 0.356637 \u2506 0.916926 \u2506 0.509538 \u2506 0.344282 \u2506 5.110688 \u2502\n",
-                            "\u2502 7   \u2506 0.489873 \u2506 0.351803 \u2506 0.861379 \u2506 0.985876 \u2506 3.487034 \u2502\n",
-                            "\u2502 8   \u2506 0.485547 \u2506 0.796377 \u2506 0.776287 \u2506 0.102771 \u2506 9.366586 \u2502\n",
-                            "\u2502 11  \u2506 0.548642 \u2506 0.621415 \u2506 0.179476 \u2506 0.942682 \u2506 9.447275 \u2502\n",
+                            "\u2502 1   \u2506 0.59381  \u2506 0.496358 \u2506 0.765642 \u2506 0.08905  \u2506 0.527819 \u2502\n",
+                            "\u2502 2   \u2506 0.651759 \u2506 0.473416 \u2506 0.654051 \u2506 0.772629 \u2506 3.989873 \u2502\n",
+                            "\u2502 3   \u2506 0.588802 \u2506 0.095334 \u2506 0.51503  \u2506 0.893853 \u2506 7.933253 \u2502\n",
+                            "\u2502 7   \u2506 0.825937 \u2506 0.670161 \u2506 0.397054 \u2506 0.902048 \u2506 0.030179 \u2502\n",
+                            "\u2502 8   \u2506 0.835848 \u2506 0.712411 \u2506 0.478414 \u2506 0.024903 \u2506 6.137378 \u2502\n",
                             "\u2514\u2500\u2500\u2500\u2500\u2500\u2534\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2534\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2534\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2534\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2534\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2518"
                         ]
                     },
                     "execution_count": 44,
                     "metadata": {},
                     "output_type": "execute_result"
                 }
@@ -2020,28 +2020,28 @@
                             "<div><style>\n",
                             ".dataframe > thead > tr,\n",
                             ".dataframe > tbody > tr {\n",
                             "  text-align: right;\n",
                             "  white-space: pre-wrap;\n",
                             "}\n",
                             "</style>\n",
-                            "<small>shape: (5, 6)</small><table border=\"1\" class=\"dataframe\"><thead><tr><th>id</th><th>var1</th><th>var2</th><th>var3</th><th>r</th><th>rh</th></tr><tr><td>u32</td><td>f64</td><td>f64</td><td>f64</td><td>f64</td><td>f64</td></tr></thead><tbody><tr><td>50</td><td>0.521872</td><td>0.520009</td><td>0.089207</td><td>0.446793</td><td>2.756932</td></tr><tr><td>138</td><td>0.476258</td><td>0.457252</td><td>0.578248</td><td>0.696907</td><td>4.576948</td></tr><tr><td>174</td><td>0.466104</td><td>0.489402</td><td>0.703968</td><td>0.308085</td><td>7.681611</td></tr><tr><td>178</td><td>0.478427</td><td>0.490086</td><td>0.903002</td><td>0.287589</td><td>5.352698</td></tr><tr><td>319</td><td>0.413976</td><td>0.488702</td><td>0.666915</td><td>0.328137</td><td>5.147284</td></tr></tbody></table></div>"
+                            "<small>shape: (5, 6)</small><table border=\"1\" class=\"dataframe\"><thead><tr><th>id</th><th>var1</th><th>var2</th><th>var3</th><th>r</th><th>rh</th></tr><tr><td>u32</td><td>f64</td><td>f64</td><td>f64</td><td>f64</td><td>f64</td></tr></thead><tbody><tr><td>65</td><td>0.52442</td><td>0.583255</td><td>0.384267</td><td>0.665396</td><td>8.013905</td></tr><tr><td>97</td><td>0.454917</td><td>0.525371</td><td>0.32274</td><td>0.691031</td><td>0.289121</td></tr><tr><td>169</td><td>0.439562</td><td>0.520168</td><td>0.677887</td><td>0.577202</td><td>5.904235</td></tr><tr><td>194</td><td>0.521875</td><td>0.555248</td><td>0.445828</td><td>0.014645</td><td>6.531176</td></tr><tr><td>196</td><td>0.503961</td><td>0.540833</td><td>0.962907</td><td>0.006286</td><td>4.006109</td></tr></tbody></table></div>"
                         ],
                         "text/plain": [
                             "shape: (5, 6)\n",
                             "\u250c\u2500\u2500\u2500\u2500\u2500\u252c\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u252c\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u252c\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u252c\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u252c\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2510\n",
                             "\u2502 id  \u2506 var1     \u2506 var2     \u2506 var3     \u2506 r        \u2506 rh       \u2502\n",
                             "\u2502 --- \u2506 ---      \u2506 ---      \u2506 ---      \u2506 ---      \u2506 ---      \u2502\n",
                             "\u2502 u32 \u2506 f64      \u2506 f64      \u2506 f64      \u2506 f64      \u2506 f64      \u2502\n",
                             "\u255e\u2550\u2550\u2550\u2550\u2550\u256a\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u256a\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u256a\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u256a\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u256a\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2561\n",
-                            "\u2502 50  \u2506 0.521872 \u2506 0.520009 \u2506 0.089207 \u2506 0.446793 \u2506 2.756932 \u2502\n",
-                            "\u2502 138 \u2506 0.476258 \u2506 0.457252 \u2506 0.578248 \u2506 0.696907 \u2506 4.576948 \u2502\n",
-                            "\u2502 174 \u2506 0.466104 \u2506 0.489402 \u2506 0.703968 \u2506 0.308085 \u2506 7.681611 \u2502\n",
-                            "\u2502 178 \u2506 0.478427 \u2506 0.490086 \u2506 0.903002 \u2506 0.287589 \u2506 5.352698 \u2502\n",
-                            "\u2502 319 \u2506 0.413976 \u2506 0.488702 \u2506 0.666915 \u2506 0.328137 \u2506 5.147284 \u2502\n",
+                            "\u2502 65  \u2506 0.52442  \u2506 0.583255 \u2506 0.384267 \u2506 0.665396 \u2506 8.013905 \u2502\n",
+                            "\u2502 97  \u2506 0.454917 \u2506 0.525371 \u2506 0.32274  \u2506 0.691031 \u2506 0.289121 \u2502\n",
+                            "\u2502 169 \u2506 0.439562 \u2506 0.520168 \u2506 0.677887 \u2506 0.577202 \u2506 5.904235 \u2502\n",
+                            "\u2502 194 \u2506 0.521875 \u2506 0.555248 \u2506 0.445828 \u2506 0.014645 \u2506 6.531176 \u2502\n",
+                            "\u2502 196 \u2506 0.503961 \u2506 0.540833 \u2506 0.962907 \u2506 0.006286 \u2506 4.006109 \u2502\n",
                             "\u2514\u2500\u2500\u2500\u2500\u2500\u2534\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2534\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2534\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2534\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2534\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2518"
                         ]
                     },
                     "execution_count": 45,
                     "metadata": {},
                     "output_type": "execute_result"
                 }
@@ -2070,29 +2070,29 @@
                             "<div><style>\n",
                             ".dataframe > thead > tr,\n",
                             ".dataframe > tbody > tr {\n",
                             "  text-align: right;\n",
                             "  white-space: pre-wrap;\n",
                             "}\n",
                             "</style>\n",
-                            "<small>shape: (5, 6)</small><table border=\"1\" class=\"dataframe\"><thead><tr><th>id</th><th>var1</th><th>var2</th><th>var3</th><th>r</th><th>rh</th></tr><tr><td>u32</td><td>f64</td><td>f64</td><td>f64</td><td>f64</td><td>f64</td></tr></thead><tbody><tr><td>174</td><td>0.466104</td><td>0.489402</td><td>0.703968</td><td>0.308085</td><td>7.681611</td></tr><tr><td>178</td><td>0.478427</td><td>0.490086</td><td>0.903002</td><td>0.287589</td><td>5.352698</td></tr><tr><td>331</td><td>0.46378</td><td>0.470691</td><td>0.504769</td><td>0.565669</td><td>8.41936</td></tr><tr><td>388</td><td>0.469873</td><td>0.490685</td><td>0.51908</td><td>0.135412</td><td>9.419304</td></tr><tr><td>482</td><td>0.499758</td><td>0.505641</td><td>0.436567</td><td>0.83411</td><td>0.849715</td></tr></tbody></table></div>"
+                            "<small>shape: (5, 6)</small><table border=\"1\" class=\"dataframe\"><thead><tr><th>id</th><th>var1</th><th>var2</th><th>var3</th><th>r</th><th>rh</th></tr><tr><td>u32</td><td>f64</td><td>f64</td><td>f64</td><td>f64</td><td>f64</td></tr></thead><tbody><tr><td>447</td><td>0.550618</td><td>0.547562</td><td>0.273377</td><td>0.410981</td><td>9.727249</td></tr><tr><td>573</td><td>0.484537</td><td>0.524645</td><td>0.943169</td><td>0.641065</td><td>8.905943</td></tr><tr><td>657</td><td>0.536476</td><td>0.480191</td><td>0.79945</td><td>0.779526</td><td>8.022189</td></tr><tr><td>1090</td><td>0.45779</td><td>0.52121</td><td>0.145912</td><td>0.870635</td><td>8.265113</td></tr><tr><td>1198</td><td>0.470434</td><td>0.460267</td><td>0.67229</td><td>0.695826</td><td>8.519747</td></tr></tbody></table></div>"
                         ],
                         "text/plain": [
                             "shape: (5, 6)\n",
-                            "\u250c\u2500\u2500\u2500\u2500\u2500\u252c\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u252c\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u252c\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u252c\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u252c\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2510\n",
-                            "\u2502 id  \u2506 var1     \u2506 var2     \u2506 var3     \u2506 r        \u2506 rh       \u2502\n",
-                            "\u2502 --- \u2506 ---      \u2506 ---      \u2506 ---      \u2506 ---      \u2506 ---      \u2502\n",
-                            "\u2502 u32 \u2506 f64      \u2506 f64      \u2506 f64      \u2506 f64      \u2506 f64      \u2502\n",
-                            "\u255e\u2550\u2550\u2550\u2550\u2550\u256a\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u256a\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u256a\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u256a\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u256a\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2561\n",
-                            "\u2502 174 \u2506 0.466104 \u2506 0.489402 \u2506 0.703968 \u2506 0.308085 \u2506 7.681611 \u2502\n",
-                            "\u2502 178 \u2506 0.478427 \u2506 0.490086 \u2506 0.903002 \u2506 0.287589 \u2506 5.352698 \u2502\n",
-                            "\u2502 331 \u2506 0.46378  \u2506 0.470691 \u2506 0.504769 \u2506 0.565669 \u2506 8.41936  \u2502\n",
-                            "\u2502 388 \u2506 0.469873 \u2506 0.490685 \u2506 0.51908  \u2506 0.135412 \u2506 9.419304 \u2502\n",
-                            "\u2502 482 \u2506 0.499758 \u2506 0.505641 \u2506 0.436567 \u2506 0.83411  \u2506 0.849715 \u2502\n",
-                            "\u2514\u2500\u2500\u2500\u2500\u2500\u2534\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2534\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2534\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2534\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2534\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2518"
+                            "\u250c\u2500\u2500\u2500\u2500\u2500\u2500\u252c\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u252c\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u252c\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u252c\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u252c\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2510\n",
+                            "\u2502 id   \u2506 var1     \u2506 var2     \u2506 var3     \u2506 r        \u2506 rh       \u2502\n",
+                            "\u2502 ---  \u2506 ---      \u2506 ---      \u2506 ---      \u2506 ---      \u2506 ---      \u2502\n",
+                            "\u2502 u32  \u2506 f64      \u2506 f64      \u2506 f64      \u2506 f64      \u2506 f64      \u2502\n",
+                            "\u255e\u2550\u2550\u2550\u2550\u2550\u2550\u256a\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u256a\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u256a\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u256a\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u256a\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2561\n",
+                            "\u2502 447  \u2506 0.550618 \u2506 0.547562 \u2506 0.273377 \u2506 0.410981 \u2506 9.727249 \u2502\n",
+                            "\u2502 573  \u2506 0.484537 \u2506 0.524645 \u2506 0.943169 \u2506 0.641065 \u2506 8.905943 \u2502\n",
+                            "\u2502 657  \u2506 0.536476 \u2506 0.480191 \u2506 0.79945  \u2506 0.779526 \u2506 8.022189 \u2502\n",
+                            "\u2502 1090 \u2506 0.45779  \u2506 0.52121  \u2506 0.145912 \u2506 0.870635 \u2506 8.265113 \u2502\n",
+                            "\u2502 1198 \u2506 0.470434 \u2506 0.460267 \u2506 0.67229  \u2506 0.695826 \u2506 8.519747 \u2502\n",
+                            "\u2514\u2500\u2500\u2500\u2500\u2500\u2500\u2534\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2534\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2534\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2534\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2534\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2518"
                         ]
                     },
                     "execution_count": 46,
                     "metadata": {},
                     "output_type": "execute_result"
                 }
             ],
@@ -2120,29 +2120,29 @@
                             "<div><style>\n",
                             ".dataframe > thead > tr,\n",
                             ".dataframe > tbody > tr {\n",
                             "  text-align: right;\n",
                             "  white-space: pre-wrap;\n",
                             "}\n",
                             "</style>\n",
-                            "<small>shape: (5, 3)</small><table border=\"1\" class=\"dataframe\"><thead><tr><th>id</th><th>friends</th><th>count</th></tr><tr><td>u64</td><td>list[u32]</td><td>u32</td></tr></thead><tbody><tr><td>0</td><td>[0, 1675, \u2026 1305]</td><td>79</td></tr><tr><td>1</td><td>[1, 128, \u2026 322]</td><td>112</td></tr><tr><td>2</td><td>[2, 54, \u2026 1633]</td><td>94</td></tr><tr><td>3</td><td>[3, 963, \u2026 978]</td><td>122</td></tr><tr><td>4</td><td>[4, 61, \u2026 1899]</td><td>120</td></tr></tbody></table></div>"
+                            "<small>shape: (5, 3)</small><table border=\"1\" class=\"dataframe\"><thead><tr><th>id</th><th>friends</th><th>count</th></tr><tr><td>u64</td><td>list[u32]</td><td>u32</td></tr></thead><tbody><tr><td>0</td><td>[0, 466, \u2026 1269]</td><td>109</td></tr><tr><td>1</td><td>[1, 203, \u2026 197]</td><td>124</td></tr><tr><td>2</td><td>[2, 350, \u2026 1806]</td><td>116</td></tr><tr><td>3</td><td>[3, 367, \u2026 1076]</td><td>143</td></tr><tr><td>4</td><td>[4, 1625, \u2026 363]</td><td>126</td></tr></tbody></table></div>"
                         ],
                         "text/plain": [
                             "shape: (5, 3)\n",
-                            "\u250c\u2500\u2500\u2500\u2500\u2500\u252c\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u252c\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2510\n",
-                            "\u2502 id  \u2506 friends           \u2506 count \u2502\n",
-                            "\u2502 --- \u2506 ---               \u2506 ---   \u2502\n",
-                            "\u2502 u64 \u2506 list[u32]         \u2506 u32   \u2502\n",
-                            "\u255e\u2550\u2550\u2550\u2550\u2550\u256a\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u256a\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2561\n",
-                            "\u2502 0   \u2506 [0, 1675, \u2026 1305] \u2506 79    \u2502\n",
-                            "\u2502 1   \u2506 [1, 128, \u2026 322]   \u2506 112   \u2502\n",
-                            "\u2502 2   \u2506 [2, 54, \u2026 1633]   \u2506 94    \u2502\n",
-                            "\u2502 3   \u2506 [3, 963, \u2026 978]   \u2506 122   \u2502\n",
-                            "\u2502 4   \u2506 [4, 61, \u2026 1899]   \u2506 120   \u2502\n",
-                            "\u2514\u2500\u2500\u2500\u2500\u2500\u2534\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2534\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2518"
+                            "\u250c\u2500\u2500\u2500\u2500\u2500\u252c\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u252c\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2510\n",
+                            "\u2502 id  \u2506 friends          \u2506 count \u2502\n",
+                            "\u2502 --- \u2506 ---              \u2506 ---   \u2502\n",
+                            "\u2502 u64 \u2506 list[u32]        \u2506 u32   \u2502\n",
+                            "\u255e\u2550\u2550\u2550\u2550\u2550\u256a\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u256a\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2561\n",
+                            "\u2502 0   \u2506 [0, 466, \u2026 1269] \u2506 109   \u2502\n",
+                            "\u2502 1   \u2506 [1, 203, \u2026 197]  \u2506 124   \u2502\n",
+                            "\u2502 2   \u2506 [2, 350, \u2026 1806] \u2506 116   \u2502\n",
+                            "\u2502 3   \u2506 [3, 367, \u2026 1076] \u2506 143   \u2502\n",
+                            "\u2502 4   \u2506 [4, 1625, \u2026 363] \u2506 126   \u2502\n",
+                            "\u2514\u2500\u2500\u2500\u2500\u2500\u2534\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2534\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2518"
                         ]
                     },
                     "execution_count": 47,
                     "metadata": {},
                     "output_type": "execute_result"
                 }
             ],
@@ -2198,28 +2198,28 @@
                             "<div><style>\n",
                             ".dataframe > thead > tr,\n",
                             ".dataframe > tbody > tr {\n",
                             "  text-align: right;\n",
                             "  white-space: pre-wrap;\n",
                             "}\n",
                             "</style>\n",
-                            "<small>shape: (5, 2)</small><table border=\"1\" class=\"dataframe\"><thead><tr><th>id</th><th>friends</th></tr><tr><td>u32</td><td>u32</td></tr></thead><tbody><tr><td>0</td><td>0</td></tr><tr><td>0</td><td>1675</td></tr><tr><td>0</td><td>33</td></tr><tr><td>0</td><td>905</td></tr><tr><td>0</td><td>806</td></tr></tbody></table></div>"
+                            "<small>shape: (5, 2)</small><table border=\"1\" class=\"dataframe\"><thead><tr><th>id</th><th>friends</th></tr><tr><td>u32</td><td>u32</td></tr></thead><tbody><tr><td>0</td><td>0</td></tr><tr><td>0</td><td>466</td></tr><tr><td>0</td><td>174</td></tr><tr><td>0</td><td>373</td></tr><tr><td>0</td><td>374</td></tr></tbody></table></div>"
                         ],
                         "text/plain": [
                             "shape: (5, 2)\n",
                             "\u250c\u2500\u2500\u2500\u2500\u2500\u252c\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2510\n",
                             "\u2502 id  \u2506 friends \u2502\n",
                             "\u2502 --- \u2506 ---     \u2502\n",
                             "\u2502 u32 \u2506 u32     \u2502\n",
                             "\u255e\u2550\u2550\u2550\u2550\u2550\u256a\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2561\n",
                             "\u2502 0   \u2506 0       \u2502\n",
-                            "\u2502 0   \u2506 1675    \u2502\n",
-                            "\u2502 0   \u2506 33      \u2502\n",
-                            "\u2502 0   \u2506 905     \u2502\n",
-                            "\u2502 0   \u2506 806     \u2502\n",
+                            "\u2502 0   \u2506 466     \u2502\n",
+                            "\u2502 0   \u2506 174     \u2502\n",
+                            "\u2502 0   \u2506 373     \u2502\n",
+                            "\u2502 0   \u2506 374     \u2502\n",
                             "\u2514\u2500\u2500\u2500\u2500\u2500\u2534\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2518"
                         ]
                     },
                     "execution_count": 49,
                     "metadata": {},
                     "output_type": "execute_result"
                 }
@@ -2248,34 +2248,34 @@
                             "<div><style>\n",
                             ".dataframe > thead > tr,\n",
                             ".dataframe > tbody > tr {\n",
                             "  text-align: right;\n",
                             "  white-space: pre-wrap;\n",
                             "}\n",
                             "</style>\n",
-                            "<small>shape: (2_000, 2)</small><table border=\"1\" class=\"dataframe\"><thead><tr><th>id</th><th>path</th></tr><tr><td>u32</td><td>list[u32]</td></tr></thead><tbody><tr><td>0</td><td>[3]</td></tr><tr><td>1</td><td>[1594, 1975, 3]</td></tr><tr><td>2</td><td>[1673, 1707, 3]</td></tr><tr><td>3</td><td>[]</td></tr><tr><td>4</td><td>[1070, 1200, \u2026 3]</td></tr><tr><td>&hellip;</td><td>&hellip;</td></tr><tr><td>1995</td><td>[94, 1397, \u2026 3]</td></tr><tr><td>1996</td><td>[469, 1739, \u2026 3]</td></tr><tr><td>1997</td><td>[797, 1853, \u2026 3]</td></tr><tr><td>1998</td><td>[1994, 197, \u2026 3]</td></tr><tr><td>1999</td><td>[409, 1278, 3]</td></tr></tbody></table></div>"
+                            "<small>shape: (2_000, 2)</small><table border=\"1\" class=\"dataframe\"><thead><tr><th>id</th><th>path</th></tr><tr><td>u32</td><td>list[u32]</td></tr></thead><tbody><tr><td>0</td><td>[1057, 405, \u2026 3]</td></tr><tr><td>1</td><td>[795, 627, 3]</td></tr><tr><td>2</td><td>[795, 627, 3]</td></tr><tr><td>3</td><td>[]</td></tr><tr><td>4</td><td>[1634, 1252, \u2026 3]</td></tr><tr><td>&hellip;</td><td>&hellip;</td></tr><tr><td>1995</td><td>[1417, 203, \u2026 3]</td></tr><tr><td>1996</td><td>[920, 224, \u2026 3]</td></tr><tr><td>1997</td><td>[827, 1047, \u2026 3]</td></tr><tr><td>1998</td><td>[719, 1162, \u2026 3]</td></tr><tr><td>1999</td><td>[324, 1665, \u2026 3]</td></tr></tbody></table></div>"
                         ],
                         "text/plain": [
                             "shape: (2_000, 2)\n",
                             "\u250c\u2500\u2500\u2500\u2500\u2500\u2500\u252c\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2510\n",
                             "\u2502 id   \u2506 path              \u2502\n",
                             "\u2502 ---  \u2506 ---               \u2502\n",
                             "\u2502 u32  \u2506 list[u32]         \u2502\n",
                             "\u255e\u2550\u2550\u2550\u2550\u2550\u2550\u256a\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2561\n",
-                            "\u2502 0    \u2506 [3]               \u2502\n",
-                            "\u2502 1    \u2506 [1594, 1975, 3]   \u2502\n",
-                            "\u2502 2    \u2506 [1673, 1707, 3]   \u2502\n",
+                            "\u2502 0    \u2506 [1057, 405, \u2026 3]  \u2502\n",
+                            "\u2502 1    \u2506 [795, 627, 3]     \u2502\n",
+                            "\u2502 2    \u2506 [795, 627, 3]     \u2502\n",
                             "\u2502 3    \u2506 []                \u2502\n",
-                            "\u2502 4    \u2506 [1070, 1200, \u2026 3] \u2502\n",
+                            "\u2502 4    \u2506 [1634, 1252, \u2026 3] \u2502\n",
                             "\u2502 \u2026    \u2506 \u2026                 \u2502\n",
-                            "\u2502 1995 \u2506 [94, 1397, \u2026 3]   \u2502\n",
-                            "\u2502 1996 \u2506 [469, 1739, \u2026 3]  \u2502\n",
-                            "\u2502 1997 \u2506 [797, 1853, \u2026 3]  \u2502\n",
-                            "\u2502 1998 \u2506 [1994, 197, \u2026 3]  \u2502\n",
-                            "\u2502 1999 \u2506 [409, 1278, 3]    \u2502\n",
+                            "\u2502 1995 \u2506 [1417, 203, \u2026 3]  \u2502\n",
+                            "\u2502 1996 \u2506 [920, 224, \u2026 3]   \u2502\n",
+                            "\u2502 1997 \u2506 [827, 1047, \u2026 3]  \u2502\n",
+                            "\u2502 1998 \u2506 [719, 1162, \u2026 3]  \u2502\n",
+                            "\u2502 1999 \u2506 [324, 1665, \u2026 3]  \u2502\n",
                             "\u2514\u2500\u2500\u2500\u2500\u2500\u2500\u2534\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2518"
                         ]
                     },
                     "execution_count": 50,
                     "metadata": {},
                     "output_type": "execute_result"
                 }
@@ -2300,34 +2300,34 @@
                             "<div><style>\n",
                             ".dataframe > thead > tr,\n",
                             ".dataframe > tbody > tr {\n",
                             "  text-align: right;\n",
                             "  white-space: pre-wrap;\n",
                             "}\n",
                             "</style>\n",
-                            "<small>shape: (2_000, 3)</small><table border=\"1\" class=\"dataframe\"><thead><tr><th>id</th><th>reachable</th><th>steps</th></tr><tr><td>u32</td><td>bool</td><td>u32</td></tr></thead><tbody><tr><td>958</td><td>true</td><td>4</td></tr><tr><td>1420</td><td>true</td><td>3</td></tr><tr><td>1505</td><td>true</td><td>1</td></tr><tr><td>1027</td><td>true</td><td>7</td></tr><tr><td>1577</td><td>true</td><td>3</td></tr><tr><td>&hellip;</td><td>&hellip;</td><td>&hellip;</td></tr><tr><td>1791</td><td>true</td><td>7</td></tr><tr><td>1777</td><td>true</td><td>8</td></tr><tr><td>1113</td><td>true</td><td>3</td></tr><tr><td>550</td><td>true</td><td>6</td></tr><tr><td>1653</td><td>true</td><td>1</td></tr></tbody></table></div>"
+                            "<small>shape: (2_000, 3)</small><table border=\"1\" class=\"dataframe\"><thead><tr><th>id</th><th>reachable</th><th>steps</th></tr><tr><td>u32</td><td>bool</td><td>u32</td></tr></thead><tbody><tr><td>391</td><td>true</td><td>2</td></tr><tr><td>1927</td><td>true</td><td>7</td></tr><tr><td>617</td><td>true</td><td>3</td></tr><tr><td>821</td><td>true</td><td>1</td></tr><tr><td>1298</td><td>true</td><td>7</td></tr><tr><td>&hellip;</td><td>&hellip;</td><td>&hellip;</td></tr><tr><td>184</td><td>true</td><td>5</td></tr><tr><td>791</td><td>true</td><td>3</td></tr><tr><td>966</td><td>true</td><td>3</td></tr><tr><td>310</td><td>true</td><td>1</td></tr><tr><td>951</td><td>true</td><td>5</td></tr></tbody></table></div>"
                         ],
                         "text/plain": [
                             "shape: (2_000, 3)\n",
                             "\u250c\u2500\u2500\u2500\u2500\u2500\u2500\u252c\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u252c\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2510\n",
                             "\u2502 id   \u2506 reachable \u2506 steps \u2502\n",
                             "\u2502 ---  \u2506 ---       \u2506 ---   \u2502\n",
                             "\u2502 u32  \u2506 bool      \u2506 u32   \u2502\n",
                             "\u255e\u2550\u2550\u2550\u2550\u2550\u2550\u256a\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u256a\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2561\n",
-                            "\u2502 958  \u2506 true      \u2506 4     \u2502\n",
-                            "\u2502 1420 \u2506 true      \u2506 3     \u2502\n",
-                            "\u2502 1505 \u2506 true      \u2506 1     \u2502\n",
-                            "\u2502 1027 \u2506 true      \u2506 7     \u2502\n",
-                            "\u2502 1577 \u2506 true      \u2506 3     \u2502\n",
+                            "\u2502 391  \u2506 true      \u2506 2     \u2502\n",
+                            "\u2502 1927 \u2506 true      \u2506 7     \u2502\n",
+                            "\u2502 617  \u2506 true      \u2506 3     \u2502\n",
+                            "\u2502 821  \u2506 true      \u2506 1     \u2502\n",
+                            "\u2502 1298 \u2506 true      \u2506 7     \u2502\n",
                             "\u2502 \u2026    \u2506 \u2026         \u2506 \u2026     \u2502\n",
-                            "\u2502 1791 \u2506 true      \u2506 7     \u2502\n",
-                            "\u2502 1777 \u2506 true      \u2506 8     \u2502\n",
-                            "\u2502 1113 \u2506 true      \u2506 3     \u2502\n",
-                            "\u2502 550  \u2506 true      \u2506 6     \u2502\n",
-                            "\u2502 1653 \u2506 true      \u2506 1     \u2502\n",
+                            "\u2502 184  \u2506 true      \u2506 5     \u2502\n",
+                            "\u2502 791  \u2506 true      \u2506 3     \u2502\n",
+                            "\u2502 966  \u2506 true      \u2506 3     \u2502\n",
+                            "\u2502 310  \u2506 true      \u2506 1     \u2502\n",
+                            "\u2502 951  \u2506 true      \u2506 5     \u2502\n",
                             "\u2514\u2500\u2500\u2500\u2500\u2500\u2500\u2534\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2534\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2518"
                         ]
                     },
                     "execution_count": 51,
                     "metadata": {},
                     "output_type": "execute_result"
                 }
@@ -2412,28 +2412,28 @@
                             "<div><style>\n",
                             ".dataframe > thead > tr,\n",
                             ".dataframe > tbody > tr {\n",
                             "  text-align: right;\n",
                             "  white-space: pre-wrap;\n",
                             "}\n",
                             "</style>\n",
-                            "<small>shape: (5, 3)</small><table border=\"1\" class=\"dataframe\"><thead><tr><th>id</th><th>path</th><th>cost</th></tr><tr><td>u32</td><td>list[u32]</td><td>f64</td></tr></thead><tbody><tr><td>3</td><td>[1]</td><td>0.1</td></tr><tr><td>2</td><td>[4, 1]</td><td>0.6</td></tr><tr><td>0</td><td>[4, 1]</td><td>0.2</td></tr><tr><td>1</td><td>[]</td><td>0.0</td></tr><tr><td>4</td><td>[1]</td><td>0.1</td></tr></tbody></table></div>"
+                            "<small>shape: (5, 3)</small><table border=\"1\" class=\"dataframe\"><thead><tr><th>id</th><th>path</th><th>cost</th></tr><tr><td>u32</td><td>list[u32]</td><td>f64</td></tr></thead><tbody><tr><td>3</td><td>[1]</td><td>0.1</td></tr><tr><td>1</td><td>[]</td><td>0.0</td></tr><tr><td>4</td><td>[1]</td><td>0.1</td></tr><tr><td>0</td><td>[4, 1]</td><td>0.2</td></tr><tr><td>2</td><td>[4, 1]</td><td>0.6</td></tr></tbody></table></div>"
                         ],
                         "text/plain": [
                             "shape: (5, 3)\n",
                             "\u250c\u2500\u2500\u2500\u2500\u2500\u252c\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u252c\u2500\u2500\u2500\u2500\u2500\u2500\u2510\n",
                             "\u2502 id  \u2506 path      \u2506 cost \u2502\n",
                             "\u2502 --- \u2506 ---       \u2506 ---  \u2502\n",
                             "\u2502 u32 \u2506 list[u32] \u2506 f64  \u2502\n",
                             "\u255e\u2550\u2550\u2550\u2550\u2550\u256a\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u256a\u2550\u2550\u2550\u2550\u2550\u2550\u2561\n",
                             "\u2502 3   \u2506 [1]       \u2506 0.1  \u2502\n",
-                            "\u2502 2   \u2506 [4, 1]    \u2506 0.6  \u2502\n",
-                            "\u2502 0   \u2506 [4, 1]    \u2506 0.2  \u2502\n",
                             "\u2502 1   \u2506 []        \u2506 0.0  \u2502\n",
                             "\u2502 4   \u2506 [1]       \u2506 0.1  \u2502\n",
+                            "\u2502 0   \u2506 [4, 1]    \u2506 0.2  \u2502\n",
+                            "\u2502 2   \u2506 [4, 1]    \u2506 0.6  \u2502\n",
                             "\u2514\u2500\u2500\u2500\u2500\u2500\u2534\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2534\u2500\u2500\u2500\u2500\u2500\u2500\u2518"
                         ]
                     },
                     "execution_count": 53,
                     "metadata": {},
                     "output_type": "execute_result"
                 }
@@ -2457,28 +2457,28 @@
                             "<div><style>\n",
                             ".dataframe > thead > tr,\n",
                             ".dataframe > tbody > tr {\n",
                             "  text-align: right;\n",
                             "  white-space: pre-wrap;\n",
                             "}\n",
                             "</style>\n",
-                            "<small>shape: (5, 2)</small><table border=\"1\" class=\"dataframe\"><thead><tr><th>node</th><th>deg</th></tr><tr><td>u32</td><td>u32</td></tr></thead><tbody><tr><td>3</td><td>3</td></tr><tr><td>2</td><td>1</td></tr><tr><td>0</td><td>4</td></tr><tr><td>1</td><td>2</td></tr><tr><td>4</td><td>1</td></tr></tbody></table></div>"
+                            "<small>shape: (5, 2)</small><table border=\"1\" class=\"dataframe\"><thead><tr><th>node</th><th>deg</th></tr><tr><td>u32</td><td>u32</td></tr></thead><tbody><tr><td>3</td><td>3</td></tr><tr><td>1</td><td>2</td></tr><tr><td>4</td><td>1</td></tr><tr><td>0</td><td>4</td></tr><tr><td>2</td><td>1</td></tr></tbody></table></div>"
                         ],
                         "text/plain": [
                             "shape: (5, 2)\n",
                             "\u250c\u2500\u2500\u2500\u2500\u2500\u2500\u252c\u2500\u2500\u2500\u2500\u2500\u2510\n",
                             "\u2502 node \u2506 deg \u2502\n",
                             "\u2502 ---  \u2506 --- \u2502\n",
                             "\u2502 u32  \u2506 u32 \u2502\n",
                             "\u255e\u2550\u2550\u2550\u2550\u2550\u2550\u256a\u2550\u2550\u2550\u2550\u2550\u2561\n",
                             "\u2502 3    \u2506 3   \u2502\n",
-                            "\u2502 2    \u2506 1   \u2502\n",
-                            "\u2502 0    \u2506 4   \u2502\n",
                             "\u2502 1    \u2506 2   \u2502\n",
                             "\u2502 4    \u2506 1   \u2502\n",
+                            "\u2502 0    \u2506 4   \u2502\n",
+                            "\u2502 2    \u2506 1   \u2502\n",
                             "\u2514\u2500\u2500\u2500\u2500\u2500\u2500\u2534\u2500\u2500\u2500\u2500\u2500\u2518"
                         ]
                     },
                     "execution_count": 54,
                     "metadata": {},
                     "output_type": "execute_result"
                 }
```

### Comparing `polars_ds-0.4.2/examples/dependency.parquet` & `polars_ds-0.4.3/examples/dependency.parquet`

 * *Files identical despite different names*

### Comparing `polars_ds-0.4.2/examples/sample_and_split.ipynb` & `polars_ds-0.4.3/examples/sample_and_split.ipynb`

 * *Files identical despite different names*

### Comparing `polars_ds-0.4.2/mkdocs.yml` & `polars_ds-0.4.3/mkdocs.yml`

 * *Files identical despite different names*

### Comparing `polars_ds-0.4.2/python/polars_ds/__init__.py` & `polars_ds-0.4.3/python/polars_ds/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 from polars_ds.metrics import *  # noqa: F403
 from polars_ds.stats import *  # noqa: F403
 from polars_ds.complex import ComplexExt  # noqa: E402, F401
 from polars_ds.str2 import *  # noqa: F403
 
 logging.basicConfig(level=logging.INFO)
 
-__version__ = "0.4.2"
+__version__ = "0.4.3"
 
 
 def l_inf_horizontal(*v: Union[str, pl.Expr], normalize: bool = False) -> pl.Expr:
     """
     Horizontally L inf norm. Shorthand for pl.max_horizontal(pl.col(x).abs() for x in exprs).
 
     Parameters
```

### Comparing `polars_ds-0.4.2/python/polars_ds/_utils.py` & `polars_ds-0.4.3/python/polars_ds/_utils.py`

 * *Files identical despite different names*

### Comparing `polars_ds-0.4.2/python/polars_ds/complex.py` & `polars_ds-0.4.3/python/polars_ds/complex.py`

 * *Files identical despite different names*

### Comparing `polars_ds-0.4.2/python/polars_ds/diagnosis.py` & `polars_ds-0.4.3/python/polars_ds/diagnosis.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,26 +1,32 @@
 import polars.selectors as cs
 import polars as pl
 import logging
-from typing import Union, List, Optional, Iterable
+import plotly.express as px
+import plotly.graph_objects as go
+from typing import Union, List, Optional, Iterable, Tuple
 from functools import lru_cache
-from .num import query_cond_entropy, query_principal_components
+from .num import query_cond_entropy, query_principal_components, query_lstsq_report
 from itertools import combinations
+from .type_alias import CorrMethod
+from .stats import corr
+from .sample import sample
 import graphviz
-from great_tables import GT
+from great_tables import GT, nanoplot_options
 from polars.type_aliases import IntoExpr
 
 logger = logging.getLogger(__name__)
 
 
 # DIA = Data Inspection Assistant / DIAgonsis
 class DIA:
 
     """
-    Data Inspection Assistant.
+    Data Inspection Assistant. Most plots are powered by plotly/great_tables. Plotly may require
+    additional package downloads.
 
     If you cannot import this module, please try: pip install "polars_ds[plot]"
     """
 
     def __init__(self, df: Union[pl.DataFrame, pl.LazyFrame]):
         self._frame: pl.LazyFrame = df.lazy()
         self.numerics: List[str] = df.select(cs.numeric()).columns
@@ -124,14 +130,69 @@
             .fmt_percent(columns="null%")
             .fmt_number(
                 columns=["mean", "std", "min", "q1", "median", "q3", "max", "IQR"], decimals=3
             )
             .fmt_nanoplot(columns="histogram", plot_type="bar")
         )
 
+    def plot_null_distribution(
+        self, subset: Union[IntoExpr, Iterable[IntoExpr]] = pl.all(), n_bins: int = 50
+    ):
+        """
+        Checks the null percentages per row group. Row groups are consecutive rows grouped by row number,
+        with each group having len//n_bins number of elements. The height of each bin is the percentage
+        of nulls in the row group.
+
+        This plot shows whether nulls in one feature is correlated with nulls in other features.
+
+        Parameters
+        ----------
+        subset
+            Anything that can be put into a Polars .select statement. Defaults to pl.all()
+        n_bins
+            The number
+        """
+        cols = self._frame.select(subset).columns
+        temp = (
+            self._frame.with_row_index(name="row_group")
+            .group_by((pl.col("row_group") // (pl.len() // n_bins)).alias("row_group"))
+            .agg(pl.col(cols).null_count() / pl.len())
+            .sort("row_group")
+            .select(
+                pl.col(cols).exclude(["row_group"]).implode(),
+            )
+            .collect()
+        )
+        # Values for plot. The first n are list[f64] used in nanoplot. The rest are overall null rates
+        percentages = temp.row(0)
+
+        temp2 = self._frame.select(pl.col(cols).null_count() / pl.len()).collect()
+        null_rates = temp2.row(0)
+
+        null_table = pl.DataFrame(
+            {
+                "column": cols,
+                "percentages in row groups": [{"val": values} for values in percentages],
+                "null%": null_rates,
+            }
+        )
+
+        return (
+            GT(null_table, rowname_col="column")
+            .tab_header(title="Null Distribution")
+            .tab_stubhead("column")
+            .fmt_number(columns=["null%"], decimals=5)
+            .fmt_percent(columns="null%")
+            .fmt_nanoplot(
+                columns="percentages in row groups",
+                plot_type="bar",
+                options=nanoplot_options(data_bar_fill_color="red"),
+            )
+        )
+
     def meta(self):
         """
         Returns internal data in this class as a dictionary.
         """
         out = self.__dict__.copy()
         out.pop("_frame")
         return out
@@ -161,53 +222,61 @@
                 pl.col(c).str.len_bytes().quantile(0.05).alias("5p_byte_len"),
                 pl.col(c).str.len_bytes().quantile(0.95).alias("95p_byte_len"),
             )
             for c in to_check
         ]
         return pl.concat(pl.collect_all(frames))
 
-    def corr(self, subset: Union[IntoExpr, Iterable[IntoExpr]]) -> pl.DataFrame:
+    def corr(
+        self, subset: Union[IntoExpr, Iterable[IntoExpr]], method: CorrMethod = "pearson"
+    ) -> pl.DataFrame:
         """
         Returns a dataframe containing correlation information between the subset and all numeric columns.
 
         Parameters
         ----------
         subset
             Anything that can be put into a Polars .select statement.
+        method
+            One of ["pearson", "spearman", "xi", "kendall"]
         """
         temp = self._frame.select(subset).columns
         to_check = [c for c in temp if c in self.numerics]
         if len(to_check) != len(temp):
             removed = list(set(temp).difference(to_check))
             logger.info(
                 f"The following columns are not numeric/not in the dataframe, skipped: \n{removed}"
             )
 
         corrs = [
             self._frame.select(
-                pl.lit(x).alias("column"), *(pl.corr(x, y).alias(y) for y in self.numerics)
+                pl.lit(x).alias("column"), *(corr(x, y).alias(y) for y in self.numerics)
             )
             for x in to_check
         ]
 
         return pl.concat(pl.collect_all(corrs))
 
-    def plot_corr(self, subset: Union[IntoExpr, Iterable[IntoExpr]]):
+    def plot_corr(
+        self, subset: Union[IntoExpr, Iterable[IntoExpr]], method: CorrMethod = "pearson"
+    ):
         """
         Plots the correlations using classic heat maps.
 
         Parameters
         ----------
         subset
             Anything that can be put into a Polars .select statement.
+        method
+            One of ["pearson", "spearman", "xi", "kendall"]
         """
-        corr = self.corr(subset)
-        cols = [c for c in corr.columns if c != "column"]
+        corr_values = self.corr(subset, method)
+        cols = [c for c in corr_values.columns if c != "column"]
         return (
-            GT(corr)
+            GT(corr_values)
             .fmt_number(columns=cols, decimals=3)
             .data_color(
                 columns=cols,
                 palette=["#0202bd", "#bd0237"],
                 domain=[-1, 1],
                 alpha=0.5,
                 na_color="#000000",
@@ -394,53 +463,65 @@
                 .collect()
                 .row(0)
             )
 
         return [c for c, ok in zip(self._frame.columns, is_ok) if ok is True]
 
     @lru_cache
-    def infer_corr(self) -> pl.DataFrame:
+    def infer_corr(self, method: CorrMethod = "pearson") -> pl.DataFrame:
         """
         Trying to infer highly correlated columns by computing correlation between
         all numerical (including boolean) columns.
+
+        Parameters
+        ----------
+        method
+            One of ["pearson", "spearman", "xi", "kendall"]
         """
         to_check = self.numerics + self.bools
         correlation = (
             self._frame.with_columns(pl.col(c).cast(pl.UInt8) for c in self.bools)
-            .select(
-                pl.corr(x, y).alias(f"{i}") for i, (x, y) in enumerate(combinations(to_check, 2))
-            )
+            .select(corr(x, y).alias(f"{i}") for i, (x, y) in enumerate(combinations(to_check, 2)))
             .collect()
             .row(0)
         )
 
         xx = []
         yy = []
         for x, y in combinations(to_check, 2):
             xx.append(x)
             yy.append(y)
 
         return pl.DataFrame({"x": xx, "y": yy, "corr": correlation}).sort(
             pl.col("corr").abs(), descending=True
         )
 
-    @lru_cache
-    def infer_dependency(self) -> pl.DataFrame:
+    def infer_dependency(
+        self, subset: Union[IntoExpr, Iterable[IntoExpr]] = pl.all()
+    ) -> pl.DataFrame:
         """
         Infers (functional) dependency using the method of conditional entropy. This only evaluates
         potential qualifying columns. Potential qualifying columns are columns of type:
         int, str, categorical, or booleans.
 
         If returned conditional entropy is very low, that means knowning the column in
         `by` is enough to to infer the column in `column`, or the column in `column` can
         be determined by the column in `by`.
+
+        Parameters
+        ----------
+        subset
+            A subset of columns to try running the dependency check. The subset input can be
+            anything that can be turned into a Polars selector. Only valid columns will be checked,
+            however.
         """
 
         # Infer valid columns to run this detection
-        to_check = self.ints + self.strs + self.cats + self.bools
+        valid = self.ints + self.strs + self.cats + self.bools
+        to_check = [x for x in self._frame.select(subset).columns if x in valid]
 
         n_uniques = self._frame.select(pl.col(c).n_unique() for c in to_check).collect().row(0)
 
         frame = (
             pl.DataFrame({"column": to_check, "n_unique": n_uniques})
             .filter(pl.col("n_unique") > 1)
             .sort("n_unique")
@@ -476,38 +557,32 @@
             by.append(y)
 
         out = pl.DataFrame({"column": column, "by": by, "cond_entropy": ce}).sort("cond_entropy")
 
         return out
 
     def plot_dependency(
-        self, threshold: float = 0.01, exclude: Optional[list[str]] = None
+        self, threshold: float = 0.01, subset: Union[IntoExpr, Iterable[IntoExpr]] = pl.all()
     ) -> graphviz.Digraph:
         """
         Plot dependency using the result of self.infer_dependency and positively dtermines
         dependency by the threshold.
 
         Parameters
         ----------
         threshold
             If conditional entropy is < threshold, we draw a line indicating dependency.
-        exclude
-            None or a list of column names to exclude from plotting. E.g. ID column will always
-            uniquely determine values in other columns. So plotting ID will make the plot crowded
-            and provides no additional information.
+        subset
+            A subset of columns to try running the dependency check. The subset input can be
+            anything that can be turned into a Polars selector
         """
 
-        dep_frame = self.infer_dependency()
-        to_exclude = (
-            pl.lit(True, dtype=pl.Boolean)
-            if exclude is None
-            else pl.col("by").is_in(exclude).not_()
-        )
+        dep_frame = self.infer_dependency(subset=subset)
 
-        df_local = dep_frame.filter((pl.col("cond_entropy") < threshold) & to_exclude).select(
+        df_local = dep_frame.filter((pl.col("cond_entropy") < threshold)).select(
             pl.col("column").alias("child"),  # c for child
             pl.col("by").alias("parent"),  # p for parent
         )
         cp = df_local.group_by("child").agg(pl.col("parent"))
         pc = df_local.group_by("parent").agg(pl.col("child"))
         child_parent: dict[str, pl.Series] = dict(
             zip(cp.drop_in_place("child"), cp.drop_in_place("parent"))
@@ -531,36 +606,135 @@
             dot.node(c)
             for p in parents_of_c:
                 dot.node(p)
                 dot.edge(p, c)
 
         return dot
 
-    def plot_pc2(
-        self, *features: Union[IntoExpr, Iterable[IntoExpr]], by: str, center: bool = True, **kwargs
-    ):
+    def plot_lstsq(
+        self,
+        x: Union[IntoExpr, Iterable[IntoExpr]],
+        target: Union[IntoExpr, Iterable[IntoExpr]],
+        add_bias: bool = False,
+        condition: Optional[pl.Expr] = None,
+        max_points: int = 20_000,
+        **kwargs,
+    ) -> Tuple[pl.DataFrame, go.Figure]:
+        """
+        Plots the least squares between x and target.
+
+        Paramters
+        ---------
+        x
+            The preditive variable
+        target
+            The target variable
+        add_bias
+            Whether to add bias in the linear regression
+        condition
+            An additional filter condition you want to apply before runing lstsq on the data. This must
+            be a boolean expression. If none, run this on the entire dataset. (The frame used to initialize DIA.)
+        max_points
+            The max number of points to be displayed. If data > this limit, the data will be sampled
+        kwargs
+            Kwargs to be passed to Plotly's Figure object
+        """
+        if condition is None:
+            temp = self._frame.select(x, target)
+            condition_str = ""
+        else:
+            temp = self._frame.filter(condition).select(x, target)
+            condition_str = "\nCondition: " + str(condition)
+
+        x_name, y_name = temp.columns
+        coeffs = (
+            temp.select(
+                query_lstsq_report(x_name, target=y_name, add_bias=add_bias).alias("report")
+            )
+            .unnest("report")
+            .select(
+                pl.all().exclude("idx")  # All but the idx column in lstsq_report
+            )
+            .collect()
+        )
+        if add_bias:
+            b1, alpha = coeffs["coeff"]
+        else:
+            b1, alpha = coeffs["coeff"][0], 0
+        # Get the data necessary for plotting
+        temp = self._frame.select(
+            pl.col(x_name).alias("x"),
+            pl.col(y_name).alias("y"),
+            (pl.col(x_name) * b1 + alpha).alias("y_pred"),
+        )  # Sample down. If len(temp) < max_points, all temp will be selected. This sample supports lazy.
+        df = sample(temp, value=max_points)
+
+        fig = go.Figure(**kwargs)
+        fig.update_layout(
+            title=f"y={y_name}, x={x_name}, y_pred = ({x_name}) * {b1:.5f} + {alpha:.5f}<br><sup>{condition_str}</sup>",
+            xaxis_title=x_name,
+            yaxis_title=y_name,
+        )
+
+        fig.add_trace(go.Scatter(x=df["x"], y=df["y"], mode="markers", name="data scatter"))
+        fig.add_trace(go.Scatter(x=df["x"], y=df["y_pred"], mode="lines", name="Least Squares"))
+        print(coeffs)
+        return fig
+
+    def plot_pca(
+        self,
+        *features: Union[IntoExpr, Iterable[IntoExpr]],
+        by: Union[IntoExpr, Iterable[IntoExpr]],
+        center: bool = True,
+        dim: int = 2,
+        max_points: int = 20_000,
+        **kwargs,
+    ) -> go.Figure:
         """
-        Creates a 2D scatter plot based on the reduced dimensions via PCA, and color it by `by`.
+        Creates a scatter plot based on the reduced dimensions via PCA, and color it by `by`.
 
         Paramters
         ---------
         features
             Any selection expression for Polars
         by
             Color the 2-D PCA plot by the values in the column
         center
             Whether to automatically center the features
+        dim
+            Either 2 or 3. Plot either a 2d principal component plot or a 3d one.
+        max_points
+            The max number of points to be displayed. If data > this limit, the data will be sampled.
         kwargs
-            Anything else that will be passed to hvplot's scatter function
+            Anything else that will be passed to plotly's scatter function
         """
         feats = self._frame.select(features).columns
         if len(feats) < 2:
             raise ValueError("You must pass >= 2 features.")
+        if dim < 2 or dim > 3:
+            raise ValueError("Input `dim` must either be 2 or 3.")
 
-        temp = (
-            self._frame.select(
-                query_principal_components(*feats, center=center, k=2).alias("pc"), by
-            )
-            .collect()
-            .unnest("pc")
+        temp = self._frame.select(
+            query_principal_components(*feats, center=center, k=dim).alias("pc"), by
         )
-        return temp.plot.scatter("pc1", "pc2", by=by, **kwargs)
+        df = sample(temp, value=max_points).unnest("pc")
+
+        if dim == 2:
+            fig = px.scatter(
+                x=df["pc1"],
+                y=df["pc2"],
+                color=df[by],
+                labels={"x": "pc1", "y": "pc2"},
+                title="2 Principal Components",
+                **kwargs,
+            )
+        else:
+            fig = px.scatter_3d(
+                x=df["pc1"],
+                y=df["pc2"],
+                z=df["pc3"],
+                color=df[by],
+                labels={"x": "pc1", "y": "pc2", "z": "pc3"},
+                title="3 Principal Components",
+                **kwargs,
+            )
+        return fig
```

### Comparing `polars_ds-0.4.2/python/polars_ds/graph.py` & `polars_ds-0.4.3/python/polars_ds/graph.py`

 * *Files identical despite different names*

### Comparing `polars_ds-0.4.2/python/polars_ds/metrics.py` & `polars_ds-0.4.3/python/polars_ds/metrics.py`

 * *Files identical despite different names*

### Comparing `polars_ds-0.4.2/python/polars_ds/num.py` & `polars_ds-0.4.3/python/polars_ds/num.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from __future__ import annotations
 import math
 import polars as pl
 from typing import Union, Optional, List, Iterable
-from .type_alias import DetrendMethod, Distance, ConvMode, str_to_expr, StrOrExpr
+from .type_alias import DetrendMethod, Distance, ConvMode, ConvMethod, str_to_expr, StrOrExpr
 from polars.utils.udfs import _get_shared_lib_location
 from ._utils import pl_plugin
 
 _lib = _get_shared_lib_location(__file__)
 
 
 @pl.api.register_expr_namespace("num")
@@ -974,15 +974,14 @@
     cols.extend(str_to_expr(z) for z in x)
     if return_pred:
         return pl_plugin(
             lib=_lib,
             symbol="pl_lstsq_pred",
             args=cols,
             kwargs={"bias": add_bias, "skip_null": skip_null},
-            is_elementwise=True,
         )
     else:
         return pl_plugin(
             lib=_lib,
             symbol="pl_lstsq",
             args=cols,
             kwargs={"bias": add_bias, "skip_null": skip_null},
@@ -1151,15 +1150,15 @@
     )
     brk = vc.struct.field("brk")  # .cast(pl.Float64)
     cnt_ref = vc.struct.field("count")  # .cast(pl.UInt32)
 
     return pl_plugin(
         lib=_lib,
         symbol="pl_psi",
-        args=[valid_x, brk, cnt_ref],
+        args=[valid_x.rechunk(), brk, cnt_ref],
         returns_scalar=True,
     )
 
 
 def query_psi_discrete(
     x: StrOrExpr,
     ref: Union[pl.Expr, List[float], "np.ndarray", pl.Series],  # noqa: F821
@@ -1347,41 +1346,61 @@
         args=[yy, xx],
         returns_scalar=True,
     )
 
 
 def convolve(
     x: StrOrExpr,
-    filter_: Union[List[float], "np.ndarray", pl.Series],  # noqa: F821
+    kernel: Union[List[float], "np.ndarray", pl.Series, pl.Expr],  # noqa: F821
+    fill_value: Union[float, pl.Expr] = 0.0,
+    method: ConvMethod = "direct",
     mode: ConvMode = "full",
 ) -> pl.Expr:
     """
     Performs a convolution with the filter via FFT. The current implementation's performance is worse
-    than SciPy but offers parallelization within Polars Context.
+    than SciPy but offers parallelization within Polars.
+
+    For large kernels (usually kernel length > 120), convolving with FFT is faster, but for smaller kernels,
+    convolving with direct method is faster.
 
     parameters
     ----------
     x
         A column of numbers
-    filter_
-        The filter for the convolution. Anything that can be turned into a Polars Series will work.
+    kernel
+        The filter for the convolution. Anything that can be turned into a Polars Series will work. All non-finite
+        values will be filtered out before the convolution.
+    fill_value
+        Fill null values in `x` with this value. Either a float or a polars's expression representing 1 element
+    method
+        Either `fft` or `direct`.
     mode
         Please check the reference. One of `same`, `left` (left-aligned same), `right` (right-aligned same),
         `valid` or `full`.
 
     Reference
     ---------
     https://brianmcfee.net/dstbook-site/content/ch03-convolution/Modes.html
+    https://en.wikipedia.org/wiki/Convolution
     """
-    xx = str_to_expr(x).cast(pl.Float64)
-    f = pl.Series(values=filter_, dtype=pl.Float64)
+    xx = str_to_expr(x).fill_null(fill_value).cast(pl.Float64).rechunk()  # One cont slice
+    if isinstance(kernel, pl.Expr):
+        f = kernel.filter(kernel.is_finite()).rechunk()  # One cont slice
+    else:
+        f = pl.Series(values=kernel, dtype=pl.Float64)
+        f = f.filter(f.is_finite()).rechunk()  # One cont slice
+
+    if method == "direct":
+        f = f.reverse()
+
     return pl_plugin(
         lib=_lib,
-        symbol="pl_fft_convolve",
-        args=[xx, f, pl.lit(mode, dtype=pl.String)],
+        symbol="pl_convolve",
+        args=[xx, f],
+        kwargs={"mode": mode, "method": method},
         changes_length=True,
     )
 
 
 def list_amax(list_col: StrOrExpr) -> pl.Expr:
     """
     Finds the argmax of the list in this column. This is useful for
@@ -1463,25 +1482,25 @@
         args=[str_to_expr(x)],
         lib=_lib,
         symbol="pl_trunc",
         is_elementwise=True,
     )
 
 
-def signum(x: StrOrExpr) -> pl.Expr:
-    """
-    Returns sign of the input values. Note: NaN is returned for NaN. This is faster
-    and more accurate than doing pl.when(..).then().otherwise().
-    """
-    return pl_plugin(
-        args=[str_to_expr(x)],
-        lib=_lib,
-        symbol="pl_signum",
-        is_elementwise=True,
-    )
+# def signum(x: StrOrExpr) -> pl.Expr:
+#     """
+#     Returns sign of the input values. Note: NaN is returned for NaN. This is faster
+#     and more accurate than doing pl.when(..).then().otherwise().
+#     """
+#     return pl_plugin(
+#         args=[str_to_expr(x)],
+#         lib=_lib,
+#         symbol="pl_signum",
+#         is_elementwise=True,
+#     )
 
 
 def sinc(x: StrOrExpr) -> pl.Expr:
     """
     Computes the sinc function normalized by pi.
     """
     xx = str_to_expr(x)
```

### Comparing `polars_ds-0.4.2/python/polars_ds/sample.py` & `polars_ds-0.4.3/python/polars_ds/sample.py`

 * *Files identical despite different names*

### Comparing `polars_ds-0.4.2/python/polars_ds/stats.py` & `polars_ds-0.4.3/python/polars_ds/stats.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from __future__ import annotations
 import polars as pl
 import math
-from .type_alias import Alternative, str_to_expr, StrOrExpr
+from .type_alias import Alternative, str_to_expr, StrOrExpr, CorrMethod
 from typing import Optional, Union
 from polars.utils.udfs import _get_shared_lib_location
 from ._utils import pl_plugin
 
 _lib = _get_shared_lib_location(__file__)
 
 
@@ -964,21 +964,45 @@
     xx, yy = str_to_expr(x), str_to_expr(y)
     w = str_to_expr(weights)
     wx2 = xx.pow(2).dot(w)
     wy2 = yy.pow(2).dot(w)
     return (w * xx).dot(yy) / (wx2 * wy2).sqrt()
 
 
+def kendall_tau(x: StrOrExpr, y: StrOrExpr) -> pl.Expr:
+    """
+    Computes Kendall's Tau (b) correlation between x and y. This automatically drops rows with null.
+
+    Note: this will map NaN to null and drop all rows with null. Inf will be kept and cosidered as
+    the largest value and multiple Infs will be equal. -Inf will be the smallest if it exists in the
+    data. A value of NaN will be returned if the data has < 2 rows after nulls are dropped.
+
+    Parameters
+    ----------
+    x
+        The first variable
+    y
+        The second variable
+    """
+    xx, yy = str_to_expr(x).fill_nan(None), str_to_expr(y).fill_nan(None)
+    return pl_plugin(
+        lib=_lib,
+        symbol="pl_kendall_tau",
+        args=[xx.rank(method="min"), yy.rank(method="min")],
+        returns_scalar=True,
+    )
+
+
 def xi_corr(
     x: StrOrExpr, y: StrOrExpr, seed: Optional[int] = None, return_p: bool = False
 ) -> pl.Expr:
     """
     Computes the ξ(xi) correlation developed by SOURAV CHATTERJEE in the paper in the reference.
     This will return both the correlation (the statistic) and the p-value. Note that if sample size
-    is smaller than 30, p-value will always be NaN. The ξ correlation is not symmetric, and this only
+    is smaller than 30, p-value will always be NaN. The ξ correlation is not symmetric, as it only
     tries to explain whether y is a function of x.
 
     Parameters
     ----------
     x
         The first variable
     y
@@ -1008,7 +1032,31 @@
     else:
         return pl_plugin(
             lib=_lib,
             symbol="pl_xi_corr",
             args=args,
             returns_scalar=True,
         )
+
+
+def corr(x: StrOrExpr, y: StrOrExpr, method: CorrMethod = "pearson") -> pl.Expr:
+    """
+    A convenience function for calling different types of correlations. Pearson and Spearman correlation
+    runs on Polar's native expression, while Kendall and Xi correlation runs on code in this package.
+
+    Paramters
+    ---------
+    x
+        The first variable
+    y
+        The second variable
+    method
+        One of ["pearson", "spearman", "xi", "kendall"]
+    """
+    if method in ["pearson", "spearman"]:
+        return pl.corr(x, y, method=method)
+    elif method == "xi":
+        return xi_corr(x, y)
+    elif method == "kendall":
+        return kendall_tau(x, y)
+    else:
+        raise ValueError(f"Unknown correlation method: {method}.")
```

### Comparing `polars_ds-0.4.2/python/polars_ds/str2.py` & `polars_ds-0.4.3/python/polars_ds/str2.py`

 * *Files identical despite different names*

### Comparing `polars_ds-0.4.2/python/polars_ds/type_alias.py` & `polars_ds-0.4.3/python/polars_ds/type_alias.py`

 * *Files 8% similar despite different names*

```diff
@@ -4,20 +4,22 @@
 import polars as pl
 
 if sys.version_info >= (3, 10):
     from typing import TypeAlias
 else:  # 3.9, 3.8
     from typing_extensions import TypeAlias
 
-# Custom Enum Types
+# Custom "Enum" Types
 DetrendMethod: TypeAlias = Literal["linear", "mean"]
 Alternative: TypeAlias = Literal["two-sided", "less", "greater"]
 ROCAUCStrategy: TypeAlias = Literal["macro", "weighted"]
 Distance: TypeAlias = Literal["l1", "l2", "inf", "h", "cosine", "haversine"]
 ConvMode: TypeAlias = Literal["same", "left", "right", "full", "valid"]
+ConvMethod: TypeAlias = Literal["fft", "direct"]
+CorrMethod: TypeAlias = Literal["pearson", "spearman", "xi", "kendall"]
 
 # Other Custom Types
 PolarsFrame: TypeAlias = Union[pl.DataFrame, pl.LazyFrame]
 StrOrExpr: TypeAlias = Union[str, pl.Expr]
 
 
 # Auxiliary functions for type conversions
```

### Comparing `polars_ds-0.4.2/src/graph/degree.rs` & `polars_ds-0.4.3/src/graph/degree.rs`

 * *Files identical despite different names*

### Comparing `polars_ds-0.4.2/src/graph/eigen_centrality.rs` & `polars_ds-0.4.3/src/graph/eigen_centrality.rs`

 * *Files identical despite different names*

### Comparing `polars_ds-0.4.2/src/graph/mod.rs` & `polars_ds-0.4.3/src/graph/mod.rs`

 * *Files identical despite different names*

### Comparing `polars_ds-0.4.2/src/graph/shortest_path.rs` & `polars_ds-0.4.3/src/graph/shortest_path.rs`

 * *Files identical despite different names*

### Comparing `polars_ds-0.4.2/src/num/cond_entropy.rs` & `polars_ds-0.4.3/src/num/cond_entropy.rs`

 * *Files identical despite different names*

### Comparing `polars_ds-0.4.2/src/num/convolve.rs` & `polars_ds-0.4.3/src/num/convolve.rs`

 * *Files 25% similar despite different names*

```diff
@@ -1,75 +1,99 @@
 use polars::prelude::*;
 use pyo3_polars::derive::polars_expr;
 use realfft::RealFftPlanner;
+use ndarray::{ArrayView1, Array1};
+use serde::Deserialize;
 
-// Optimization ideas: small size, e.g. <= 2048, always allocate a fixed sized slice?
-// 2^n padding in the general case
+// Pending: small vec optimizations? Fixed sized allocation for <= 4096?
+#[derive(Deserialize, Debug)]
+pub(crate) struct ConvolveKwargs {
+    pub(crate) mode: String,
+    pub(crate) method: String,
+}
 
 enum ConvMode {
     FULL,
     SAME,
     LEFT,
     RIGHT,
     VALID,
 }
 
-impl From<&str> for ConvMode {
-    fn from(value: &str) -> Self {
+impl TryFrom<String> for ConvMode {
+    type Error = PolarsError;
+    fn try_from(value: String) -> PolarsResult<Self> {
+        match value.to_lowercase().as_ref() {
+            "full" => Ok(Self::FULL),
+            "same" => Ok(Self::SAME),
+            "left" => Ok(Self::LEFT),
+            "right" => Ok(Self::RIGHT),
+            "valid" => Ok(Self::VALID),
+            _ => Err(PolarsError::ComputeError(
+                "Unknown convolution mode.".into(),
+            )),
+        }
+    }
+}
+
+enum ConvMethod {
+    FFT,
+    DIRECT,
+}
+
+impl TryFrom<String> for ConvMethod {
+    type Error = PolarsError;
+    fn try_from(value: String) -> PolarsResult<Self> {
         match value.to_lowercase().as_ref() {
-            "full" => Self::FULL,
-            "same" => Self::SAME,
-            "left" => Self::LEFT,
-            "right" => Self::RIGHT,
-            "valid" => Self::VALID,
-            _ => Self::FULL,
+            "fft" => Ok(Self::FFT),
+            "direct" => Ok(Self::DIRECT),
+            _ => Err(PolarsError::ComputeError(
+                "Unknown convolution method.".into(),
+            )),
         }
     }
 }
 
 // fn next_pow_2(n:usize) -> usize {
 //     let mut m:usize = 2;
 //     while m < n {
 //         m <<= 1;
 //     }
 //     m
 // }
 
-// Pad to 2^n size and make this faster?
 fn valid_fft_convolve(input: &[f64], filter: &[f64]) -> PolarsResult<Vec<f64>> {
     let in_shape = input.len();
-    // let good_size = next_pow_2(in_shape);
+
     // Prepare
     let mut output_vec = vec![0.; in_shape];
     output_vec[..in_shape].copy_from_slice(input);
 
     let mut oth = vec![0.; in_shape];
     oth[..filter.len()].copy_from_slice(filter);
 
-    // let n = output_vec.len() as f64;
     let mut planner: RealFftPlanner<f64> = RealFftPlanner::new();
     let r2c = planner.plan_fft_forward(in_shape);
     let c2r = planner.plan_fft_inverse(in_shape);
-    let mut spec_p = r2c.make_output_vec();
-    let mut spec_q = r2c.make_output_vec();
+    // let mut spec_p = r2c.make_output_vec();
+    let mut spec_p = Array1::from_vec(r2c.make_output_vec());
+    // let mut spec_q = r2c.make_output_vec();
+    let mut spec_q = Array1::from_vec(r2c.make_output_vec());
     // Forward FFT on the inputs
-    let _ = r2c.process(&mut output_vec, &mut spec_p);
+    let _ = r2c.process(&mut output_vec, spec_p.as_slice_mut().unwrap());
     // .map_err(|e| PolarsError::ComputeError(e.to_string().into()))?;
-    let _ = r2c.process(&mut oth, &mut spec_q);
+    let _ = r2c.process(&mut oth, spec_q.as_slice_mut().unwrap());
     // .map_err(|e| PolarsError::ComputeError(e.to_string().into()))?;
 
-    // After forward FFT, multiply in place in spec_p.
-    for (z1, z2) in spec_p.iter_mut().zip(spec_q.into_iter()) {
-        *z1 = *z1 * z2;
-    }
+    // After forward FFT, multiply elementwise
+    spec_p = spec_p * spec_q;
     // Inverse FFT
-    let _ = c2r.process(&mut spec_p, &mut output_vec);
+    let _ = c2r.process(spec_p.as_slice_mut().unwrap(), &mut output_vec);
     // .map_err(|e| PolarsError::ComputeError(e.to_string().into()))?;
 
-    // output_vec.truncate(in_shape);
     Ok(output_vec)
 }
 
 fn fft_convolve(input: &[f64], filter: &[f64], mode: ConvMode) -> PolarsResult<Vec<f64>> {
     match mode {
         ConvMode::FULL => {
             let t = filter.len() - 1;
@@ -101,32 +125,72 @@
                 .skip(filter.len() - 1)
                 .map(|x| x / n)
                 .collect())
         }
     }
 }
 
+fn convolve(input: &[f64], filter: &[f64], mode: ConvMode) -> PolarsResult<Vec<f64>> {
+    match mode {
+        ConvMode::FULL => {
+            let t = filter.len() - 1;
+            let mut padded_input = vec![0.; input.len() + 2 * t];
+            let from_to = t..(t + input.len());
+            padded_input[from_to].copy_from_slice(input);
+            convolve(&padded_input, filter, ConvMode::VALID)
+        }
+        ConvMode::SAME => {
+            let skip = (filter.len() - 1) / 2;
+            let out = convolve(input, filter, ConvMode::FULL)?;
+            Ok(out.into_iter().skip(skip).take(input.len()).collect())
+        }
+        ConvMode::LEFT => {
+            let n = input.len();
+            let mut out = convolve(input, filter, ConvMode::FULL)?;
+            out.truncate(n);
+            Ok(out)
+        }
+        ConvMode::RIGHT => {
+            let out = convolve(input, filter, ConvMode::FULL)?;
+            Ok(out.into_iter().skip(filter.len() - 1).collect())
+        }
+        ConvMode::VALID => {
+            let kernel = ArrayView1::from(filter);
+            Ok(
+                input
+                .windows(filter.len())
+                .map(|sl| {
+                    let slice = ArrayView1::from(sl);
+                    kernel.dot(&slice)
+                })
+                .collect()
+            )
+        }
+        
+        
+    }
+}
+
 #[polars_expr(output_type=Float64)]
-fn pl_fft_convolve(inputs: &[Series]) -> PolarsResult<Series> {
+fn pl_convolve(inputs: &[Series], kwargs: ConvolveKwargs) -> PolarsResult<Series> {
     let s1 = inputs[0].f64()?;
     let s2 = inputs[1].f64()?;
-    let mode = inputs[2].str()?;
-    let mode = mode.get(0).unwrap_or("full");
-    let mode: ConvMode = mode.into();
+
+    let mode: ConvMode = kwargs.mode.try_into()?;
+    let method: ConvMethod = kwargs.method.try_into()?;
 
     if s1.len() < s2.len() || s2.len() < 2 {
         return Err(PolarsError::ComputeError(
             "Convolution: The filter should have smaller length than the input column, and filter should have length >= 2.".into(),
         ));
     }
 
-    let input = s1.rechunk();
-    let input = input.cont_slice().unwrap();
-
-    let other = s2.rechunk();
-    let other = other.cont_slice().unwrap();
-
-    let out = fft_convolve(input, other, mode)?;
+    let input = s1.cont_slice().unwrap();
+    let filter = s2.cont_slice().unwrap();
 
-    let ca = Float64Chunked::from_slice(s1.name(), &out);
+    let out = match method {
+        ConvMethod::FFT => fft_convolve(input, filter, mode),
+        ConvMethod::DIRECT => convolve(input, filter, mode),
+    }?;
+    let ca = Float64Chunked::from_vec(s1.name(), out);
     Ok(ca.into_series())
 }
```

### Comparing `polars_ds-0.4.2/src/num/entrophies.rs` & `polars_ds-0.4.3/src/num/entrophies.rs`

 * *Files identical despite different names*

### Comparing `polars_ds-0.4.2/src/num/fft.rs` & `polars_ds-0.4.3/src/num/fft.rs`

 * *Files identical despite different names*

### Comparing `polars_ds-0.4.2/src/num/float_extras.rs` & `polars_ds-0.4.3/src/num/float_extras.rs`

 * *Files 11% similar despite different names*

```diff
@@ -36,17 +36,17 @@
     ca.cast_and_apply_in_place(f64::gamma)
 }
 
 fn cast_and_apply_exp2<T: PolarsNumericType>(ca: &ChunkedArray<T>) -> Float64Chunked {
     ca.cast_and_apply_in_place(f64::exp2)
 }
 
-fn cast_and_apply_sign<T: PolarsNumericType>(ca: &ChunkedArray<T>) -> Float64Chunked {
-    ca.cast_and_apply_in_place(f64::signum)
-}
+// fn cast_and_apply_sign<T: PolarsNumericType>(ca: &ChunkedArray<T>) -> Float64Chunked {
+//     ca.cast_and_apply_in_place(f64::signum)
+// }
 
 #[polars_expr(output_type_func=float_output)]
 fn pl_logit(inputs: &[Series]) -> PolarsResult<Series> {
     let s = &inputs[0];
     match s.dtype() {
         DataType::UInt8 => Ok(cast_and_apply_logit(s.u8().unwrap()).into_series()),
         DataType::UInt16 => Ok(cast_and_apply_logit(s.u16().unwrap()).into_series()),
@@ -196,32 +196,32 @@
         }
         _ => Err(PolarsError::ComputeError(
             "Input column must be numerical.".into(),
         )),
     }
 }
 
-#[polars_expr(output_type_func=float_output)]
-fn pl_signum(inputs: &[Series]) -> PolarsResult<Series> {
-    let s = &inputs[0];
-    match s.dtype() {
-        DataType::UInt8 => Ok(Series::from_vec(s.name(), vec![1_f64; s.len()])),
-        DataType::UInt16 => Ok(Series::from_vec(s.name(), vec![1_f64; s.len()])),
-        DataType::UInt32 => Ok(Series::from_vec(s.name(), vec![1_f64; s.len()])),
-        DataType::UInt64 => Ok(Series::from_vec(s.name(), vec![1_f64; s.len()])),
-        DataType::Int8 => Ok(cast_and_apply_sign(s.i8().unwrap()).into_series()),
-        DataType::Int16 => Ok(cast_and_apply_sign(s.i16().unwrap()).into_series()),
-        DataType::Int32 => Ok(cast_and_apply_sign(s.i32().unwrap()).into_series()),
-        DataType::Int64 => Ok(cast_and_apply_sign(s.i64().unwrap()).into_series()),
-        DataType::Float64 => {
-            let ca = s.f64().unwrap();
-            Ok(ca.apply_values(f64::signum).into_series())
-        }
-        DataType::Float32 => {
-            let ca = s.f32().unwrap();
-            Ok(ca.apply_values(f32::signum).into_series())
-        }
-        _ => Err(PolarsError::ComputeError(
-            "Input column must be numerical.".into(),
-        )),
-    }
-}
+// #[polars_expr(output_type_func=float_output)]
+// fn pl_signum(inputs: &[Series]) -> PolarsResult<Series> {
+//     let s = &inputs[0];
+//     match s.dtype() {
+//         DataType::UInt8 => Ok(Series::from_vec(s.name(), vec![1_f64; s.len()])),
+//         DataType::UInt16 => Ok(Series::from_vec(s.name(), vec![1_f64; s.len()])),
+//         DataType::UInt32 => Ok(Series::from_vec(s.name(), vec![1_f64; s.len()])),
+//         DataType::UInt64 => Ok(Series::from_vec(s.name(), vec![1_f64; s.len()])),
+//         DataType::Int8 => Ok(cast_and_apply_sign(s.i8().unwrap()).into_series()),
+//         DataType::Int16 => Ok(cast_and_apply_sign(s.i16().unwrap()).into_series()),
+//         DataType::Int32 => Ok(cast_and_apply_sign(s.i32().unwrap()).into_series()),
+//         DataType::Int64 => Ok(cast_and_apply_sign(s.i64().unwrap()).into_series()),
+//         DataType::Float64 => {
+//             let ca = s.f64().unwrap();
+//             Ok(ca.apply_values(f64::signum).into_series())
+//         }
+//         DataType::Float32 => {
+//             let ca = s.f32().unwrap();
+//             Ok(ca.apply_values(f32::signum).into_series())
+//         }
+//         _ => Err(PolarsError::ComputeError(
+//             "Input column must be numerical.".into(),
+//         )),
+//     }
+// }
```

### Comparing `polars_ds-0.4.2/src/num/gcd_lcm.rs` & `polars_ds-0.4.3/src/num/gcd_lcm.rs`

 * *Files identical despite different names*

### Comparing `polars_ds-0.4.2/src/num/haversine.rs` & `polars_ds-0.4.3/src/num/haversine.rs`

 * *Files identical despite different names*

### Comparing `polars_ds-0.4.2/src/num/jaccard.rs` & `polars_ds-0.4.3/src/num/jaccard.rs`

 * *Files identical despite different names*

### Comparing `polars_ds-0.4.2/src/num/knn.rs` & `polars_ds-0.4.3/src/num/knn.rs`

 * *Files 0% similar despite different names*

```diff
@@ -44,15 +44,15 @@
     dim: usize,
     leaf_size: usize,
     data: &'a ArrayView2<f64>,
 ) -> KdTree<f64, usize, &'a [f64]> {
     // Building the tree
     let mut tree = KdTree::with_capacity(dim, leaf_size);
     for (i, p) in data.axis_iter(Axis(0)).enumerate() {
-        // C order makes sure rows are contiguous
+        // C order makes sure rows are contiguous. If error, then ignore the addition of that row
         match tree.add(p.to_slice().unwrap(), i) {
             Ok(_) => {}
             Err(_) => {}
         }
     }
     tree
 }
```

### Comparing `polars_ds-0.4.2/src/num/lempel_ziv.rs` & `polars_ds-0.4.3/src/num/lempel_ziv.rs`

 * *Files identical despite different names*

### Comparing `polars_ds-0.4.2/src/num/mod.rs` & `polars_ds-0.4.3/src/num/mod.rs`

 * *Files identical despite different names*

### Comparing `polars_ds-0.4.2/src/num/ols.rs` & `polars_ds-0.4.3/src/num/ols.rs`

 * *Files 4% similar despite different names*

```diff
@@ -50,62 +50,64 @@
         // Fall back to LU decomp
         Err(_) => xtx.partial_piv_lu().inverse(),
     };
     let coeffs = inv * xt * y;
     coeffs
 }
 
-/// Returns a Array2 ready for linear regression, and a mask, indicates valid rows
+/// Returns a Array2 ready for linear regression, and a mask, indicating valid rows
 #[inline(always)]
 fn series_to_mat_for_lstsq(
     inputs: &[Series],
     add_bias: bool,
     skip_null: bool,
 ) -> PolarsResult<(Array2<f64>, BooleanChunked)> {
     let nrows = inputs[0].len();
-    let mut ncols = inputs.len();
-    // Should we actually skip nulls? Create null mask
+    // minus 1 because target is also in inputs
+    let n_features = inputs.len().abs_diff(1);
+    // Create null mask
     let mut has_null = inputs[0].has_validity();
-    let mut mask = inputs[0].is_not_null();
+    let mut mask = inputs[0].is_null();
     for s in inputs[1..].iter() {
         has_null |= s.has_validity();
-        mask = mask & s.is_not_null();
-    }
-    if has_null && !skip_null {
-        return Err(PolarsError::ComputeError(
-            "Lstsq: Data must not contain nulls.".into(),
-        ));
+        mask = mask | s.is_null();
     }
+    mask = !mask; // Return a mask where true is kept (true means not null).
 
-    let mut df_x = if add_bias {
-        ncols += 1;
-        let mut series_vec = inputs.to_vec(); // cheap copy
-        series_vec.push(Series::from_vec("const", vec![1_f64; nrows]));
-        rechunk_to_frame(&series_vec)
+    if has_null && !skip_null {
+        Err(PolarsError::ComputeError(
+            "Lstsq: Data must not contain nulls when skip_null is False.".into(),
+        ))
     } else {
-        rechunk_to_frame(&inputs)
-    }?;
+        let mut df_x = if add_bias {
+            let mut series_vec = inputs.to_vec(); // cheap copy
+            series_vec.push(Series::from_iter(std::iter::repeat(1f64).take(nrows)));
+            rechunk_to_frame(&series_vec)
+        } else {
+            rechunk_to_frame(&inputs)
+        }?;
 
-    if skip_null && has_null {
-        df_x = df_x.filter(&mask)?;
-    }
-    if df_x.height() <= ncols {
-        return Err(PolarsError::ComputeError(
-            "Lstsq: #Data < #features. No conclusive result.".into(),
-        ));
+        if has_null && skip_null {
+            df_x = df_x.filter(&mask)?;
+        }
+        if df_x.height() < n_features {
+            Err(PolarsError::ComputeError(
+                "Lstsq: #Data < #features. No conclusive result.".into(),
+            ))
+        } else {
+            let mat = df_x.to_ndarray::<Float64Type>(IndexOrder::Fortran)?;
+            Ok((mat, mask))
+        }
     }
-    let mat = df_x.to_ndarray::<Float64Type>(IndexOrder::Fortran)?;
-    Ok((mat, mask))
 }
 
 #[polars_expr(output_type_func=coeff_output)]
 fn pl_lstsq(inputs: &[Series], kwargs: LstsqKwargs) -> PolarsResult<Series> {
     let add_bias = kwargs.bias;
     let skip_null = kwargs.skip_null;
-    // Copy data
     // Target y is at index 0
     match series_to_mat_for_lstsq(inputs, add_bias, skip_null) {
         Ok((mat, _)) => {
             let nrows = mat.nrows();
             let y = mat.slice(s![0..nrows, 0..1]);
             let y = y.view().into_faer();
             let x = mat.slice(s![0..nrows, 1..]);
```

### Comparing `polars_ds-0.4.2/src/num/pca.rs` & `polars_ds-0.4.3/src/num/pca.rs`

 * *Files identical despite different names*

### Comparing `polars_ds-0.4.2/src/num/psi.rs` & `polars_ds-0.4.3/src/num/psi.rs`

 * *Files 5% similar despite different names*

```diff
@@ -1,54 +1,56 @@
 use polars::prelude::*;
 use pyo3_polars::derive::polars_expr;
 
 #[polars_expr(output_type=Float64)]
 fn pl_psi(inputs: &[Series]) -> PolarsResult<Series> {
     // The actual data
     let data = inputs[0].f64()?;
+    let name = data.name();
+    let data = data.cont_slice().unwrap();
     // breaks according to reference, already sorted, should be contiguous
     let brk = inputs[1].f64()?;
     if brk.len() < 2 {
         return Err(PolarsError::ComputeError(
             "PSI: Not enough bins can be created.".into(),
         ));
     }
     // cnts for each brk in ref
     let cnt_ref = inputs[2].u32()?;
+    let cnt_ref = cnt_ref.cont_slice().unwrap();
     // slice to do binary search with.
     let brk_sl = brk.cont_slice().unwrap();
     // Compute the correct cnt (of values that are inside the bins defined by ref)
     let mut cnt_data = vec![0_u32; brk_sl.len()];
-    for d in data.into_no_null_iter() {
+
+    for d in data {
         // values in brk_sl is guaranteed to be sorted, unique, and finite
         let idx = match brk_sl.binary_search_by(|x| x.partial_cmp(&d).unwrap()) {
             Ok(i) => i,
             Err(j) => j,
         };
         cnt_data[idx] += 1;
     }
     // Total cnt in ref
-    let ref_total = cnt_ref.sum().unwrap_or(0) as f64;
+    let ref_total = cnt_ref.into_iter().sum::<u32>() as f64;
     // Total cnt in actual
     let act_total = data.len() as f64; // cnt_data.iter().sum::<u32>() as f64;
-                                       // PSI
-    let psi = cnt_ref
-        .into_no_null_iter()
-        .zip(cnt_data.into_iter())
-        .fold(0., |acc, (a, b)| {
-            let aa = ((a as f64) / ref_total).max(0.0001_f64);
-            let bb = ((b as f64) / act_total).max(0.0001_f64);
-            acc + (aa - bb) * (aa / bb).ln()
-        });
-    let out = Float64Chunked::from_iter([Some(psi)]);
+
+    let psi = cnt_ref.iter().zip(cnt_data.iter()).fold(0., |acc, (a, b)| {
+        let aa = ((*a as f64) / ref_total).max(0.0001_f64);
+        let bb = ((*b as f64) / act_total).max(0.0001_f64);
+        acc + (aa - bb) * (aa / bb).ln()
+    });
+    let out = Float64Chunked::from_vec(name, vec![psi]);
     Ok(out.into_series())
 }
 
 #[polars_expr(output_type=Float64)]
 fn pl_psi_discrete(inputs: &[Series]) -> PolarsResult<Series> {
+    let name = inputs[0].name();
     if inputs[0].len() == 1 && inputs[2].len() == 1 {
         let v1 = inputs[0].get(0).unwrap();
         let v2 = inputs[1].get(0).unwrap();
         let psi: f64 = if v1.eq(&v2) {
             0_f64
         } else {
             2.0_f64 * (1.0_f64 - 0.0001_f64) * (1.0_f64 / 0.0001_f64).ln()
@@ -94,10 +96,10 @@
         .into_no_null_iter()
         .zip(cnt_data.into_no_null_iter())
         .fold(0., |acc, (a, b)| {
             let aa = ((a as f64) / ref_total).max(0.0001_f64);
             let bb = ((b as f64) / data_total).max(0.0001_f64);
             acc + (aa - bb) * (aa / bb).ln()
         });
-    let out = Float64Chunked::from_iter([Some(psi)]);
+    let out = Float64Chunked::from_vec(name, vec![psi]);
     Ok(out.into_series())
 }
```

### Comparing `polars_ds-0.4.2/src/num/target_encode.rs` & `polars_ds-0.4.3/src/num/target_encode.rs`

 * *Files identical despite different names*

### Comparing `polars_ds-0.4.2/src/num/tp_fp.rs` & `polars_ds-0.4.3/src/num/tp_fp.rs`

 * *Files identical despite different names*

### Comparing `polars_ds-0.4.2/src/num/trapz.rs` & `polars_ds-0.4.3/src/num/trapz.rs`

 * *Files identical despite different names*

### Comparing `polars_ds-0.4.2/src/num/woe_iv.rs` & `polars_ds-0.4.3/src/num/woe_iv.rs`

 * *Files identical despite different names*

### Comparing `polars_ds-0.4.2/src/stats/chi2.rs` & `polars_ds-0.4.3/src/stats/chi2.rs`

 * *Files identical despite different names*

### Comparing `polars_ds-0.4.2/src/stats/fstats.rs` & `polars_ds-0.4.3/src/stats/fstats.rs`

 * *Files identical despite different names*

### Comparing `polars_ds-0.4.2/src/stats/ks.rs` & `polars_ds-0.4.3/src/stats/ks.rs`

 * *Files identical despite different names*

### Comparing `polars_ds-0.4.2/src/stats/mod.rs` & `polars_ds-0.4.3/src/stats/mod.rs`

 * *Files 20% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 mod chi2;
 mod fstats;
+mod kendall_tau;
 mod ks;
 mod normal_test;
 mod sample;
 mod t_test;
 mod xi_corr;
 
 use polars::prelude::*;
```

### Comparing `polars_ds-0.4.2/src/stats/normal_test.rs` & `polars_ds-0.4.3/src/stats/normal_test.rs`

 * *Files identical despite different names*

### Comparing `polars_ds-0.4.2/src/stats/sample.rs` & `polars_ds-0.4.3/src/stats/sample.rs`

 * *Files identical despite different names*

### Comparing `polars_ds-0.4.2/src/stats/t_test.rs` & `polars_ds-0.4.3/src/stats/t_test.rs`

 * *Files identical despite different names*

### Comparing `polars_ds-0.4.2/src/stats/xi_corr.rs` & `polars_ds-0.4.3/src/stats/xi_corr.rs`

 * *Files identical despite different names*

### Comparing `polars_ds-0.4.2/src/stats_utils/beta.rs` & `polars_ds-0.4.3/src/stats_utils/beta.rs`

 * *Files identical despite different names*

### Comparing `polars_ds-0.4.2/src/stats_utils/gamma.rs` & `polars_ds-0.4.3/src/stats_utils/gamma.rs`

 * *Files identical despite different names*

### Comparing `polars_ds-0.4.2/src/stats_utils/mod.rs` & `polars_ds-0.4.3/src/stats_utils/mod.rs`

 * *Files identical despite different names*

### Comparing `polars_ds-0.4.2/src/stats_utils/normal.rs` & `polars_ds-0.4.3/src/stats_utils/normal.rs`

 * *Files identical despite different names*

### Comparing `polars_ds-0.4.2/src/str2/consts.rs` & `polars_ds-0.4.3/src/str2/consts.rs`

 * *Files identical despite different names*

### Comparing `polars_ds-0.4.2/src/str2/fuzz.rs` & `polars_ds-0.4.3/src/str2/fuzz.rs`

 * *Files identical despite different names*

### Comparing `polars_ds-0.4.2/src/str2/hamming.rs` & `polars_ds-0.4.3/src/str2/hamming.rs`

 * *Files identical despite different names*

### Comparing `polars_ds-0.4.2/src/str2/inflections.rs` & `polars_ds-0.4.3/src/str2/inflections.rs`

 * *Files identical despite different names*

### Comparing `polars_ds-0.4.2/src/str2/jaro.rs` & `polars_ds-0.4.3/src/str2/jaro.rs`

 * *Files identical despite different names*

### Comparing `polars_ds-0.4.2/src/str2/knn_strs.rs` & `polars_ds-0.4.3/src/str2/knn_strs.rs`

 * *Files identical despite different names*

### Comparing `polars_ds-0.4.2/src/str2/levenshtein.rs` & `polars_ds-0.4.3/src/str2/levenshtein.rs`

 * *Files identical despite different names*

### Comparing `polars_ds-0.4.2/src/str2/mod.rs` & `polars_ds-0.4.3/src/str2/mod.rs`

 * *Files identical despite different names*

### Comparing `polars_ds-0.4.2/src/str2/osa.rs` & `polars_ds-0.4.3/src/str2/osa.rs`

 * *Files identical despite different names*

### Comparing `polars_ds-0.4.2/src/str2/overlap.rs` & `polars_ds-0.4.3/src/str2/overlap.rs`

 * *Files identical despite different names*

### Comparing `polars_ds-0.4.2/src/str2/snowball/algorithms/english_stemmer.rs` & `polars_ds-0.4.3/src/str2/snowball/algorithms/english_stemmer.rs`

 * *Files identical despite different names*

### Comparing `polars_ds-0.4.2/src/str2/snowball/mod.rs` & `polars_ds-0.4.3/src/str2/snowball/mod.rs`

 * *Files identical despite different names*

### Comparing `polars_ds-0.4.2/src/str2/snowball/snowball_env.rs` & `polars_ds-0.4.3/src/str2/snowball/snowball_env.rs`

 * *Files identical despite different names*

### Comparing `polars_ds-0.4.2/src/str2/snowball_stem.rs` & `polars_ds-0.4.3/src/str2/snowball_stem.rs`

 * *Files identical despite different names*

### Comparing `polars_ds-0.4.2/src/str2/sorensen_dice.rs` & `polars_ds-0.4.3/src/str2/sorensen_dice.rs`

 * *Files identical despite different names*

### Comparing `polars_ds-0.4.2/src/str2/str_jaccard.rs` & `polars_ds-0.4.3/src/str2/str_jaccard.rs`

 * *Files identical despite different names*

### Comparing `polars_ds-0.4.2/src/str2/tversky.rs` & `polars_ds-0.4.3/src/str2/tversky.rs`

 * *Files identical despite different names*

### Comparing `polars_ds-0.4.2/src/utils/mod.rs` & `polars_ds-0.4.3/src/utils/mod.rs`

 * *Files identical despite different names*

### Comparing `polars_ds-0.4.2/tests/test.ipynb` & `polars_ds-0.4.3/tests/test.ipynb`

 * *Files 22% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9346913197097021%*

 * *Differences: {"'cells'": "{1: {'source': {insert: [(0, 'import numpy as np\\n'), (1, '\\n'), (2, 'df = "*

 * *            'pl.DataFrame(\\n\'), (3, \'    {"x": '*

 * *            'np.random.normal(size=100_000)}).with_row_index().with_columns(pl.lit(1).alias("const")\\n\'), '*

 * *            "(5, '\\n'), (6, 'kernel = np.array([1] * 50)')], delete: [4, 2, 1, 0]}}, 4: "*

 * *            '{\'source\': [\'arr1 = df["x"].to_numpy()\\n\', \'arr2 = kernel\']}, 5: {\'source\': '*

 * *            '[\'convolve(arr1, arr2)\']}, 6: {\'source\': [\'%timei […]*

```diff
@@ -12,60 +12,69 @@
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {},
             "outputs": [],
             "source": [
-                "df = pds.random_data(size=5_000, n_cols = 0).select(\n",
-                "    pds.random(0.0, 12.0).alias(\"x\"),\n",
-                "    pds.random(0.0, 1.0).alias(\"y\"),\n",
+                "import numpy as np\n",
+                "\n",
+                "df = pl.DataFrame(\n",
+                "    {\"x\": np.random.normal(size=100_000)}).with_row_index().with_columns(pl.lit(1).alias(\"const\")\n",
                 ")\n",
-                "df.head()"
+                "\n",
+                "kernel = np.array([1] * 50)"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {},
             "outputs": [],
             "source": [
-                "df.sort(pl.col(\"x\").rank(method=\"random\")).select(\n",
-                "    \"x\",\n",
-                "    \"y\",\n",
-                "    pl.col(\"y\").rank(method=\"max\").cast(pl.Float64).alias(\"r\"),\n",
-                "    (-pl.col(\"y\")).rank(method=\"max\").cast(pl.Float64).alias(\"l\"),\n",
-                ").with_columns(\n",
-                "    pl.col(\"r\").diff().abs().alias(\"r_abs_diff\"),\n",
-                "    (pl.col(\"l\") * (pl.len() - pl.col(\"l\"))).alias(\"l(n-l)\"),\n",
-                ").select(\n",
-                "    1 - (pl.len() / 2) * (pl.col(\"r_abs_diff\").sum() / pl.col(\"l(n-l)\").sum())\n",
-                ")"
+                "df.select(pds.convolve(\"x\", kernel, method=\"fft\"))\n"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {},
             "outputs": [],
             "source": [
-                "from xicor.xicor import Xi\n",
-                "x = df[\"x\"].to_numpy()\n",
-                "y = df[\"y\"].to_numpy()\n",
-                "xi_obj = Xi(x, y)\n",
-                "xi_obj.correlation"
+                "from scipy.signal import convolve"
+            ]
+        },
+        {
+            "cell_type": "code",
+            "execution_count": null,
+            "metadata": {},
+            "outputs": [],
+            "source": [
+                "arr1 = df[\"x\"].to_numpy()\n",
+                "arr2 = kernel"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {},
             "outputs": [],
             "source": [
-                "xi_obj.correlation"
+                "convolve(arr1, arr2)"
+            ]
+        },
+        {
+            "cell_type": "code",
+            "execution_count": null,
+            "metadata": {},
+            "outputs": [],
+            "source": [
+                "%timeit df.select(pds.convolve(\"x\", kernel))\n",
+                "%timeit df.select(pds.convolve(\"x\", kernel, method=\"fft\"))\n",
+                "%timeit convolve(arr1, arr2)"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {},
             "outputs": [],
@@ -73,36 +82,113 @@
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {},
             "outputs": [],
             "source": [
+                "df = pds.random_data(size=100_000, n_cols = 0).select(\n",
+                "    pds.random_int(0, 200).alias(\"x\"),\n",
+                "    pds.random_int(0, 200).alias(\"y\"),\n",
+                "    pl.Series([1] * 50_000 + list(range(50_000, 100_000))).alias(\"test\")\n",
+                ")\n",
+                "df.head()"
+            ]
+        },
+        {
+            "cell_type": "code",
+            "execution_count": null,
+            "metadata": {},
+            "outputs": [],
+            "source": [
                 "df.select(\n",
-                "    pds.query_f_test(\"uniform_1\", \"uniform_2\", group = \"y\")\n",
+                "    pl.col(\"x\").qcut(10, left_closed=False, allow_duplicates=True, include_breaks=True)\n",
+                "        .struct.field(\"brk\")\n",
+                "        .value_counts()\n",
+                "        .sort()\n",
+                ").unnest(\"brk\")"
+            ]
+        },
+        {
+            "cell_type": "code",
+            "execution_count": null,
+            "metadata": {},
+            "outputs": [],
+            "source": []
+        },
+        {
+            "cell_type": "code",
+            "execution_count": null,
+            "metadata": {},
+            "outputs": [],
+            "source": []
+        },
+        {
+            "cell_type": "code",
+            "execution_count": null,
+            "metadata": {},
+            "outputs": [],
+            "source": [
+                "df.select(\n",
+                "    pl.corr(\"x\", \"y\")\n",
                 ")"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {},
             "outputs": [],
             "source": [
+                "\n",
                 "df.select(\n",
-                "    pl.col(\"y\").stats.f_test(pl.col(\"uniform_1\"), pl.col(\"uniform_2\"))\n",
+                "    pds.kendall_tau(\"x\", \"y\")\n",
                 ")"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {},
             "outputs": [],
-            "source": []
+            "source": [
+                "from scipy.stats import kendalltau\n",
+                "\n",
+                "x = df[\"x\"].to_numpy()\n",
+                "y = df[\"y\"].to_numpy()"
+            ]
+        },
+        {
+            "cell_type": "code",
+            "execution_count": null,
+            "metadata": {},
+            "outputs": [],
+            "source": [
+                "%%timeit\n",
+                "kendalltau(x,y, nan_policy=\"omit\")"
+            ]
+        },
+        {
+            "cell_type": "code",
+            "execution_count": null,
+            "metadata": {},
+            "outputs": [],
+            "source": [
+                "df.sort(pl.col(\"x\").rank(method=\"random\")).select(\n",
+                "    \"x\",\n",
+                "    \"y\",\n",
+                "    pl.col(\"y\").rank(method=\"max\").cast(pl.Float64).alias(\"r\"),\n",
+                "    (-pl.col(\"y\")).rank(method=\"max\").cast(pl.Float64).alias(\"l\"),\n",
+                ").with_columns(\n",
+                "    pl.col(\"r\").diff().abs().alias(\"r_abs_diff\"),\n",
+                "    (pl.col(\"l\") * (pl.len() - pl.col(\"l\"))).alias(\"l(n-l)\"),\n",
+                ").select(\n",
+                "    1 - (pl.len() / 2) * (pl.col(\"r_abs_diff\").sum() / pl.col(\"l(n-l)\").sum())\n",
+                ")"
+            ]
         }
     ],
     "metadata": {
         "kernelspec": {
             "display_name": ".venv",
             "language": "python",
             "name": "python3"
@@ -113,13 +199,13 @@
                 "version": 3
             },
             "file_extension": ".py",
             "mimetype": "text/x-python",
             "name": "python",
             "nbconvert_exporter": "python",
             "pygments_lexer": "ipython3",
-            "version": "3.11.8"
+            "version": "3.12.3"
         }
     },
     "nbformat": 4,
     "nbformat_minor": 2
 }
```

### Comparing `polars_ds-0.4.2/tests/test_correctness.py` & `polars_ds-0.4.3/tests/test_correctness.py`

 * *Files 4% similar despite different names*

```diff
@@ -57,14 +57,29 @@
     xi_obj = Xi(x, y)
     ans_statistic = xi_obj.correlation
     test_statistic = df.select(pds.xi_corr("x", "y")).item(0, 0)
 
     assert np.isclose(ans_statistic, test_statistic, rtol=1e-4)
 
 
+def test_kendall_tau():
+    from scipy.stats import kendalltau
+
+    df = pds.random_data(size=2000, n_cols=0).select(
+        pds.random_int(0, 200).alias("x"),
+        pds.random_int(0, 200).alias("y"),
+    )
+
+    test = df.select(pds.kendall_tau("x", "y")).item(0, 0)
+
+    res = kendalltau(df["x"].to_numpy(), df["y"].to_numpy())
+
+    assert np.isclose(test, res.statistic)
+
+
 @pytest.mark.parametrize(
     "df, ft, res_full, res_valid, res_same",
     [
         (
             pl.DataFrame({"a": [5, 6, 7, 8, 9]}),
             [1, 0, -1],
             pl.DataFrame({"a": pl.Series([5, 6, 2, 2, 2, -8, -9], dtype=pl.Float64)}),
@@ -82,14 +97,26 @@
 
     assert_frame_equal(res, res_valid)
 
     res = df.select(pds.convolve("a", ft, mode="same"))
 
     assert_frame_equal(res, res_same)
 
+    res = df.select(pds.convolve("a", ft, mode="full", method="fft"))
+
+    assert_frame_equal(res, res_full)
+
+    res = df.select(pds.convolve("a", ft, mode="valid", method="fft"))
+
+    assert_frame_equal(res, res_valid)
+
+    res = df.select(pds.convolve("a", ft, mode="same", method="fft"))
+
+    assert_frame_equal(res, res_same)
+
 
 @pytest.mark.parametrize(
     "arr, n",
     [
         # n is Optional[int]
         (np.random.normal(size=200), None),
         (np.random.normal(size=200), 100),
@@ -149,26 +176,26 @@
     scikit_s = scikit_res[0][0]
     scikit_p = scikit_res[1][0]
 
     assert np.isclose(statistic, scikit_s)
     assert np.isclose(pvalue, scikit_p)
 
 
-@pytest.mark.parametrize(
-    "df, res",
-    [
-        (
-            pl.DataFrame({"a": [2.0, None, -2.0, float("nan")]}),
-            pl.DataFrame({"a": [1.0, None, -1.0, float("nan")]}),
-        ),
-    ],
-)
-def test_signum(df, res):
-    assert_frame_equal(df.select(pds.signum("a")), res)
-    assert_frame_equal(df.lazy().select(pds.signum("a")).collect(), res)
+# @pytest.mark.parametrize(
+#     "df, res",
+#     [
+#         (
+#             pl.DataFrame({"a": [2.0, None, -2.0, float("nan")]}),
+#             pl.DataFrame({"a": [1.0, None, -1.0, float("nan")]}),
+#         ),
+#     ],
+# )
+# def test_signum(df, res):
+#     assert_frame_equal(df.select(pds.signum("a")), res)
+#     assert_frame_equal(df.lazy().select(pds.signum("a")).collect(), res)
 
 
 @pytest.mark.parametrize(
     "df, res",
     [
         (
             pl.DataFrame({"a": [2.123, None, -2.111, float("nan")]}),
@@ -357,14 +384,56 @@
                 pl.col("a"), pl.col("b"), target="y", skip_null=True, return_pred=True
             ).alias("result")
         ).unnest("result"),
         res,
     )
 
 
+def test_lstsq_in_group_by():
+    df = pl.DataFrame(
+        {
+            "A": [1] * 4 + [2] * 4,
+            "Y": [1] * 8,
+            "X1": [1, 2, 3, 4, 5, 6, 7, 8],
+            "X2": [2, 3, 4, 1, 6, 7, 8, 5],
+        }
+    )
+
+    first = df.filter(pl.col("A").eq(1)).with_columns(
+        pds.query_lstsq(
+            pl.col("X1"), pl.col("X2"), target=pl.col("Y"), add_bias=False, return_pred=True
+        ).alias("pred")
+    )
+
+    second = df.filter(pl.col("A").eq(2)).with_columns(
+        pds.query_lstsq(
+            pl.col("X1"), pl.col("X2"), target=pl.col("Y"), add_bias=False, return_pred=True
+        ).alias("pred")
+    )
+
+    test = (
+        df.group_by("A", maintain_order=True)
+        .agg(
+            "Y",
+            "X1",
+            "X2",
+            pds.query_lstsq(
+                pl.col("X1"), pl.col("X2"), target=pl.col("Y"), add_bias=False, return_pred=True
+            ).alias("pred"),
+        )
+        .explode("Y", "X1", "X2", "pred")
+    )
+
+    test_first = test.filter(pl.col("A") == 1)
+    test_second = test.filter(pl.col("A") == 2)
+
+    assert_frame_equal(first, test_first)
+    assert_frame_equal(second, test_second)
+
+
 @pytest.mark.parametrize(
     "df, res",
     [
         (
             pl.DataFrame({"a": [1, 2, 3, 4, 5], "b": [2, 3, 4, 5, 6]}),
             pl.DataFrame({"j": [2 / 3]}),
         ),
@@ -1143,21 +1212,14 @@
     res = res.select(pl.col("nn").list.eval(pl.element().sort().cast(pl.UInt32)))
     assert_frame_equal(df2, res)
 
 
 @pytest.mark.parametrize(
     "df, x, dist, k, res",
     [
-        (
-            pl.DataFrame({"id": range(5), "val1": range(5), "val2": range(5), "val3": range(5)}),
-            [0.5, 0.5, 0.5],
-            "l2",
-            3,
-            pl.DataFrame({"id": [0, 1, 2]}),
-        ),
         (  # Only the first row is the nearest neighbor to [0.5, 0.5, 0.5]
             pl.DataFrame(
                 {"id": [1, 2], "val1": [0.1, 0.2], "val2": [0.1, 0.3], "val3": [0.1, 0.4]}
             ),
             [0.5, 0.5, 0.5],
             "cosine",
             1,
```

### Comparing `polars_ds-0.4.2/Cargo.lock` & `polars_ds-0.4.3/Cargo.lock`

 * *Files 0% similar despite different names*

```diff
@@ -1878,15 +1878,15 @@
  "stacker",
  "sysinfo",
  "version_check",
 ]
 
 [[package]]
 name = "polars_ds"
-version = "0.4.2"
+version = "0.4.3"
 dependencies = [
  "ahash",
  "approx",
  "faer",
  "faer-ext",
  "hashbrown",
  "inflections",
```

### Comparing `polars_ds-0.4.2/pyproject.toml` & `polars_ds-0.4.3/pyproject.toml`

 * *Files 7% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [build-system]
 requires = ["maturin>=1.3.2"]
 build-backend = "maturin"
 
 [project]
 name = "polars_ds"
 requires-python = ">=3.8"
-version = "0.4.2"
+version = "0.4.3"
 
 license = {file = "LICENSE.txt"}
 classifiers = [
     "Development Status :: 4 - Beta",
     "Programming Language :: Rust",
     "Programming Language :: Python :: Implementation :: CPython",
     "Programming Language :: Python :: Implementation :: PyPy",
@@ -22,17 +22,19 @@
     "polars >= 0.20.6, !=0.20.12",
 ] 
 
 keywords = ["polars-extension", "scientific-computing", "data-science"]
 
 [project.optional-dependencies]
 plot = [
-    "great-tables >= 0.5",
-    "graphviz >= 0.20",
-    "hvplot >= 0.9.1" # Polars's plot backend for now, which in term is backed by Bokeh
+    "great-tables>=0.5",
+    "graphviz>=0.20",
+    # Polars's plot backend for now, which in turn is backed by Bokeh
+    # Not the best in terms of dependency management. But keep it for now.
+    "plotly>=5.0,<6" 
 ]
 
 [tool.maturin]
 strip = true
 python-source = "python"
 features = ["pyo3/extension-module"]
 module-name = "polars_ds._polars_ds"
```

### Comparing `polars_ds-0.4.2/PKG-INFO` & `polars_ds-0.4.3/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 Metadata-Version: 2.3
 Name: polars_ds
-Version: 0.4.2
+Version: 0.4.3
 Classifier: Development Status :: 4 - Beta
 Classifier: Programming Language :: Rust
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Classifier: License :: OSI Approved :: MIT License
 Requires-Dist: polars >=0.20.6, !=0.20.12
 Requires-Dist: great-tables >=0.5 ; extra == 'plot'
 Requires-Dist: graphviz >=0.20 ; extra == 'plot'
-Requires-Dist: hvplot >=0.9.1 ; extra == 'plot'
+Requires-Dist: plotly >=5.0, <6 ; extra == 'plot'
 Provides-Extra: plot
 License-File: LICENSE.txt
 Keywords: polars-extension,scientific-computing,data-science
 Author-email: Tianren Qin <tq9695@gmail.com>
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown; charset=UTF-8; variant=GFM
 
@@ -30,27 +30,37 @@
   <a href="https://github.com/abstractqqq/polars_ds_extension/blob/main/CONTRIBUTING.md">Want to Contribute?</a>
 <br>
 <b>pip install polars-ds</b>
 </p>
 
 # The Project
 
-The goal of the project is to **reduce dependencies**, **improve code organization**, **simplify data pipelines** and overall **faciliate analysis of various kinds of tabular data** that a data scientist may encounter. It is a package built around your favorite **Polars dataframe**. Here are the current namespaces (Polars Extensions) provided by the package:
+The goal of the project is to **reduce dependencies**, **improve code organization**, **simplify data pipelines** and overall **faciliate analysis of various kinds of tabular data** that a data scientist may encounter. It is a package built around your favorite **Polars dataframe**. Here are some of the main areas of data science that is covered by the package:
 
-1. A numerical extension (num), which focuses on numerical quantities common in many fields of data analysis (credit modelling, time series, other well-known quantities, etc.), such as rfft, entropies, k-nearest-neighbors queries, Population Stability Index, Information Value, etc.
+1. Well-known numerical transform/quantities. E.g. fft, conditional entropy, singular values, basic linear regression related quantities, population stability index, weight of evidence, column-wise/row-wise jaccard similarity etc.
 
-2. A metrics extension (metric), which contains a lot of common error/loss functions, model evaluation metrics. This module is mostly designed to generate model performance monitoring data.
+2. Statistics. Basic tests such as the t-test, f-test, KS statistics. Miscallaneous functions like weighted correlation, Xi-correlation. In-dataframe random column generations, etc. 
 
-3. A str extension (str2), which focuses on str distances/similarities, and other commonly used string manipulation procedures.
+3. Metrics. ML metrics for common model performance reporting. E.g ROC AUC for binary/multiclass classification, logloss, r2, MAPE, etc.
 
-4. A stats extension (stats), which has common statistical tests such as t-test, chi2, and f-test, etc., and random sampling from a distribution, etc.
+4. KNN-related queries. E.g. filter to k-nearest neighbors to point, find indices of all neighbors within a certain distance, etc.
 
-5. A complex extension (c), which treats complex numbers as a column of array of size 2. Sometimes complex numbers are needed for processing FFT outputs.
+5. String metrics such as Levenshtein distance, Damure Levenshtein distance, other string distances, snowball stemming (English only), string Jaccard similarity, etc.
 
-6. A graph extension (graph) for very simple graph queries, such as shortest path queries, eigenvector centrality computations. More will be added. (Usable but limited. Will to be refactored/redesigned.)
+6. Diagnosis. This modules contains the DIA (Data Inspection Assitant) class, which can help you profile your data, visualize data in lower dimensions, detect functional dependencies, detect other common data quality issues like null rate or high correlation.
+
+7. Sample. Traditional dataset sampling. No time series sampling yet. This module provides functionalities such as stratified downsample, volume neutral random sampling, etc.
+
+8. Polars Native ML Pipeline. Planned but not started yet. The goal is to have a Polars native pipeline that can replace Scikit-learn's pipeline and provides all the benefits of Polars. All the basic transforms in Scikit-leran, categorical-encoders are planned. This can be super powerful together with Polars's expressions. (Basically, once you have expressions, you don't need to write custom transforms like col(A)/col(B), log transform, sqrt transform, linear/polynomial transforms, etc.)
+
+Some other areas that currently exist, but is de-prioritized:
+
+1. Complex number related queries.
+
+2. Graph related queries. (The various representations of "Graphs" in tabular dataframe makes it hard to have consistent backend handling of such data.)
 
 # But why? Why not use Sklearn? SciPy? NumPy?
 
 The goal of the package is to **facilitate** data processes and analysis that go beyond standard SQL queries, and to **reduce** the number of dependencies in your project. It incorproates parts of SciPy, NumPy, Scikit-learn, and NLP (NLTK), etc., and treats them as Polars queries so that they can be run in parallel, in group_by contexts, all for almost no extra engineering effort. 
 
 Let's see an example. Say we want to generate a model performance report. In our data, we have segments. We are not only interested in the ROC AUC of our model on the entire dataset, but we are also interested in the model's performance on different segments.
 
@@ -139,20 +149,20 @@
 **Performance and elegance - something that is quite rare in the Python world.**
 
 ## Getting Started
 
 ```python
 import polars_ds as pds
 ```
-when you want to access the namespaces provided by the package.
+
+To make full use of the Diagnosis module, do
 
 ```python
 pip install "polars_ds[plot]"
 ```
-for dataframe diagnosis related features.
 
 ## Examples
 
 See this for Polars Extensions: [notebook](./examples/basics.ipynb)
 
 See this for Native Polars DataFrame Explorative tools: [notebook](./examples/diagnosis.ipynb)
```

#### html2text {}

```diff
@@ -1,42 +1,54 @@
-Metadata-Version: 2.3 Name: polars_ds Version: 0.4.2 Classifier: Development
+Metadata-Version: 2.3 Name: polars_ds Version: 0.4.3 Classifier: Development
 Status :: 4 - Beta Classifier: Programming Language :: Rust Classifier:
 Programming Language :: Python :: Implementation :: CPython Classifier:
 Programming Language :: Python :: Implementation :: PyPy Classifier: License ::
 OSI Approved :: MIT License Requires-Dist: polars >=0.20.6, !=0.20.12 Requires-
 Dist: great-tables >=0.5 ; extra == 'plot' Requires-Dist: graphviz >=0.20 ;
-extra == 'plot' Requires-Dist: hvplot >=0.9.1 ; extra == 'plot' Provides-Extra:
-plot License-File: LICENSE.txt Keywords: polars-extension,scientific-
+extra == 'plot' Requires-Dist: plotly >=5.0, <6 ; extra == 'plot' Provides-
+Extra: plot License-File: LICENSE.txt Keywords: polars-extension,scientific-
 computing,data-science Author-email: Tianren Qin
 gmail.com> Requires-Python: >=3.8 Description-Content-Type: text/markdown;
 charset=UTF-8; variant=GFM
                         ************ PPoollaarrss ffoorr DDaattaa SScciieennccee
                                      ************
                _D_o_c_u_m_e_n_t_a_t_i_o_n | _U_s_e_r_ _G_u_i_d_e | _W_a_n_t_ _t_o_ _C_o_n_t_r_i_b_u_t_e_?
                              ppiipp iinnssttaallll ppoollaarrss--ddss
 # The Project The goal of the project is to **reduce dependencies**, **improve
 code organization**, **simplify data pipelines** and overall **faciliate
 analysis of various kinds of tabular data** that a data scientist may
 encounter. It is a package built around your favorite **Polars dataframe**.
-Here are the current namespaces (Polars Extensions) provided by the package: 1.
-A numerical extension (num), which focuses on numerical quantities common in
-many fields of data analysis (credit modelling, time series, other well-known
-quantities, etc.), such as rfft, entropies, k-nearest-neighbors queries,
-Population Stability Index, Information Value, etc. 2. A metrics extension
-(metric), which contains a lot of common error/loss functions, model evaluation
-metrics. This module is mostly designed to generate model performance
-monitoring data. 3. A str extension (str2), which focuses on str distances/
-similarities, and other commonly used string manipulation procedures. 4. A
-stats extension (stats), which has common statistical tests such as t-test,
-chi2, and f-test, etc., and random sampling from a distribution, etc. 5. A
-complex extension (c), which treats complex numbers as a column of array of
-size 2. Sometimes complex numbers are needed for processing FFT outputs. 6. A
-graph extension (graph) for very simple graph queries, such as shortest path
-queries, eigenvector centrality computations. More will be added. (Usable but
-limited. Will to be refactored/redesigned.) # But why? Why not use Sklearn?
+Here are some of the main areas of data science that is covered by the package:
+1. Well-known numerical transform/quantities. E.g. fft, conditional entropy,
+singular values, basic linear regression related quantities, population
+stability index, weight of evidence, column-wise/row-wise jaccard similarity
+etc. 2. Statistics. Basic tests such as the t-test, f-test, KS statistics.
+Miscallaneous functions like weighted correlation, Xi-correlation. In-dataframe
+random column generations, etc. 3. Metrics. ML metrics for common model
+performance reporting. E.g ROC AUC for binary/multiclass classification,
+logloss, r2, MAPE, etc. 4. KNN-related queries. E.g. filter to k-nearest
+neighbors to point, find indices of all neighbors within a certain distance,
+etc. 5. String metrics such as Levenshtein distance, Damure Levenshtein
+distance, other string distances, snowball stemming (English only), string
+Jaccard similarity, etc. 6. Diagnosis. This modules contains the DIA (Data
+Inspection Assitant) class, which can help you profile your data, visualize
+data in lower dimensions, detect functional dependencies, detect other common
+data quality issues like null rate or high correlation. 7. Sample. Traditional
+dataset sampling. No time series sampling yet. This module provides
+functionalities such as stratified downsample, volume neutral random sampling,
+etc. 8. Polars Native ML Pipeline. Planned but not started yet. The goal is to
+have a Polars native pipeline that can replace Scikit-learn's pipeline and
+provides all the benefits of Polars. All the basic transforms in Scikit-leran,
+categorical-encoders are planned. This can be super powerful together with
+Polars's expressions. (Basically, once you have expressions, you don't need to
+write custom transforms like col(A)/col(B), log transform, sqrt transform,
+linear/polynomial transforms, etc.) Some other areas that currently exist, but
+is de-prioritized: 1. Complex number related queries. 2. Graph related queries.
+(The various representations of "Graphs" in tabular dataframe makes it hard to
+have consistent backend handling of such data.) # But why? Why not use Sklearn?
 SciPy? NumPy? The goal of the package is to **facilitate** data processes and
 analysis that go beyond standard SQL queries, and to **reduce** the number of
 dependencies in your project. It incorproates parts of SciPy, NumPy, Scikit-
 learn, and NLP (NLTK), etc., and treats them as Polars queries so that they can
 be run in parallel, in group_by contexts, all for almost no extra engineering
 effort. Let's see an example. Say we want to generate a model performance
 report. In our data, we have segments. We are not only interested in the ROC
@@ -86,32 +98,31 @@
 hidden away from the end user. (3) Because Polars provides parallel execution
 for free, we can compute ROC AUC and log loss simultaneously on each segment!
 (In Pandas, one can do something like this in aggregations but is soooo much
 harder to write and way more confusing to reason about.) The end result is
 simpler, more intuitive code that is also easier to reason about, and faster
 execution time. Because of Polars's extension (plugin) system, we are now
 blessed with both: **Performance and elegance - something that is quite rare in
-the Python world.** ## Getting Started ```python import polars_ds as pds ```
-when you want to access the namespaces provided by the package. ```python pip
-install "polars_ds[plot]" ``` for dataframe diagnosis related features. ##
-Examples See this for Polars Extensions: [notebook](./examples/basics.ipynb)
-See this for Native Polars DataFrame Explorative tools: [notebook](./examples/
-diagnosis.ipynb) # Disclaimer **Currently in Beta. Feel free to submit feature
-requests in the issues section of the repo. This library will only depend on
-python Polars and will try to be as stable as possible for polars>=0.20.6.
-Exceptions will be made when Polars's update forces changes in the plugins.**
-This package is not tested with Polars streaming mode and is not designed to
-work with data so big that has to be streamed. The recommended usage will be
-for datasets of size 1k to 2-3mm rows, but actual performance will vary
-depending on dataset and hardware. Performance will only be a priority for
-datasets that fit in memory. It is a known fact that knn performance suffers
-greatly with a large k. Str-knn and Graph queries are only suitable for smaller
-data, of size ~1-5k for common computers. # Credits 1. Rust Snowball Stemmer is
-taken from Tsoding's Seroost project (MIT). See [here](https://github.com/
-tsoding/seroost) 2. Some statistics functions are taken from Statrs (MIT) and
-internalized. See [here](https://github.com/statrs-dev/statrs/tree/master) 3.
-Graph functionalities are powered by the petgragh crate. See [here](https://
-crates.io/crates/petgraph) 4. Linear algebra routines are powered partly by
-[faer](https://crates.io/crates/faer) # Other related Projects 1. Take a look
-at our friendly neighbor [functime](https://github.com/TracecatHQ/functime) 2.
-String similarity metrics is soooo fast and easy to use because of [RapidFuzz]
-(https://github.com/maxbachmann/rapidfuzz-rs)
+the Python world.** ## Getting Started ```python import polars_ds as pds ``` To
+make full use of the Diagnosis module, do ```python pip install "polars_ds
+[plot]" ``` ## Examples See this for Polars Extensions: [notebook](./examples/
+basics.ipynb) See this for Native Polars DataFrame Explorative tools:
+[notebook](./examples/diagnosis.ipynb) # Disclaimer **Currently in Beta. Feel
+free to submit feature requests in the issues section of the repo. This library
+will only depend on python Polars and will try to be as stable as possible for
+polars>=0.20.6. Exceptions will be made when Polars's update forces changes in
+the plugins.** This package is not tested with Polars streaming mode and is not
+designed to work with data so big that has to be streamed. The recommended
+usage will be for datasets of size 1k to 2-3mm rows, but actual performance
+will vary depending on dataset and hardware. Performance will only be a
+priority for datasets that fit in memory. It is a known fact that knn
+performance suffers greatly with a large k. Str-knn and Graph queries are only
+suitable for smaller data, of size ~1-5k for common computers. # Credits 1.
+Rust Snowball Stemmer is taken from Tsoding's Seroost project (MIT). See [here]
+(https://github.com/tsoding/seroost) 2. Some statistics functions are taken
+from Statrs (MIT) and internalized. See [here](https://github.com/statrs-dev/
+statrs/tree/master) 3. Graph functionalities are powered by the petgragh crate.
+See [here](https://crates.io/crates/petgraph) 4. Linear algebra routines are
+powered partly by [faer](https://crates.io/crates/faer) # Other related
+Projects 1. Take a look at our friendly neighbor [functime](https://github.com/
+TracecatHQ/functime) 2. String similarity metrics is soooo fast and easy to use
+because of [RapidFuzz](https://github.com/maxbachmann/rapidfuzz-rs)
```

