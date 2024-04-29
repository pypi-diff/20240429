# Comparing `tmp/ir_datasets-0.5.6.tar.gz` & `tmp/ir_datasets-0.5.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/ir_datasets-0.5.6.tar", last modified: Sun Feb  4 16:14:22 2024, max compression
+gzip compressed data, was "ir_datasets-0.5.7.tar", last modified: Mon Apr 29 13:11:14 2024, max compression
```

## Comparing `ir_datasets-0.5.6.tar` & `ir_datasets-0.5.7.tar`

### file list

```diff
@@ -1,185 +1,187 @@
-drwxr-xr-x   0 sean       (501) staff       (20)        0 2024-02-04 16:14:22.000000 ir_datasets-0.5.6/
--rw-r--r--   0 sean       (501) staff       (20)    11358 2020-11-29 17:54:50.000000 ir_datasets-0.5.6/LICENSE
--rw-r--r--   0 sean       (501) staff       (20)      135 2021-08-03 22:51:30.000000 ir_datasets-0.5.6/MANIFEST.in
--rw-r--r--   0 sean       (501) staff       (20)    13942 2024-02-04 16:14:22.000000 ir_datasets-0.5.6/PKG-INFO
--rw-r--r--   0 sean       (501) staff       (20)    11600 2022-10-19 19:08:01.000000 ir_datasets-0.5.6/README.md
-drwxr-xr-x   0 sean       (501) staff       (20)        0 2024-02-04 16:14:22.000000 ir_datasets-0.5.6/ir_datasets/
--rw-r--r--   0 sean       (501) staff       (20)     3326 2024-02-04 15:57:03.000000 ir_datasets-0.5.6/ir_datasets/__init__.py
--rw-r--r--   0 sean       (501) staff       (20)       74 2020-11-29 17:54:50.000000 ir_datasets-0.5.6/ir_datasets/__main__.py
-drwxr-xr-x   0 sean       (501) staff       (20)        0 2024-02-04 16:14:22.000000 ir_datasets-0.5.6/ir_datasets/commands/
--rw-r--r--   0 sean       (501) staff       (20)      638 2022-02-27 13:29:46.000000 ir_datasets-0.5.6/ir_datasets/commands/__init__.py
--rw-r--r--   0 sean       (501) staff       (20)     3161 2022-01-16 17:10:49.000000 ir_datasets-0.5.6/ir_datasets/commands/build_c4_checkpoints.py
--rw-r--r--   0 sean       (501) staff       (20)     1728 2021-08-03 22:51:30.000000 ir_datasets-0.5.6/ir_datasets/commands/build_clueweb_warc_indexes.py
--rw-r--r--   0 sean       (501) staff       (20)     2441 2022-01-16 17:10:49.000000 ir_datasets-0.5.6/ir_datasets/commands/build_download_cache.py
--rw-r--r--   0 sean       (501) staff       (20)     4090 2021-08-03 22:51:30.000000 ir_datasets-0.5.6/ir_datasets/commands/clean.py
--rw-r--r--   0 sean       (501) staff       (20)     2983 2022-01-16 17:10:49.000000 ir_datasets-0.5.6/ir_datasets/commands/doc_fifos.py
--rw-r--r--   0 sean       (501) staff       (20)    10515 2021-06-05 13:26:51.000000 ir_datasets-0.5.6/ir_datasets/commands/export.py
--rw-r--r--   0 sean       (501) staff       (20)     3293 2022-02-27 13:29:46.000000 ir_datasets-0.5.6/ir_datasets/commands/generate_metadata.py
--rw-r--r--   0 sean       (501) staff       (20)      476 2021-01-23 11:42:50.000000 ir_datasets-0.5.6/ir_datasets/commands/list.py
--rw-r--r--   0 sean       (501) staff       (20)     1910 2021-01-23 11:42:50.000000 ir_datasets-0.5.6/ir_datasets/commands/lookup.py
-drwxr-xr-x   0 sean       (501) staff       (20)        0 2024-02-04 16:14:22.000000 ir_datasets-0.5.6/ir_datasets/datasets/
--rw-r--r--   0 sean       (501) staff       (20)     1407 2023-08-06 12:06:12.000000 ir_datasets-0.5.6/ir_datasets/datasets/__init__.py
--rw-r--r--   0 sean       (501) staff       (20)     5400 2022-02-27 13:29:46.000000 ir_datasets-0.5.6/ir_datasets/datasets/antique.py
--rw-r--r--   0 sean       (501) staff       (20)     8293 2023-08-06 11:36:52.000000 ir_datasets-0.5.6/ir_datasets/datasets/aol_ia.py
--rw-r--r--   0 sean       (501) staff       (20)     1413 2022-02-27 18:37:01.000000 ir_datasets-0.5.6/ir_datasets/datasets/aquaint.py
--rw-r--r--   0 sean       (501) staff       (20)     3747 2022-10-18 13:10:16.000000 ir_datasets-0.5.6/ir_datasets/datasets/argsme.py
--rw-r--r--   0 sean       (501) staff       (20)    13855 2023-06-15 08:12:25.000000 ir_datasets-0.5.6/ir_datasets/datasets/base.py
--rw-r--r--   0 sean       (501) staff       (20)     9543 2023-08-06 11:36:52.000000 ir_datasets-0.5.6/ir_datasets/datasets/beir.py
--rw-r--r--   0 sean       (501) staff       (20)     9235 2023-08-06 11:36:52.000000 ir_datasets-0.5.6/ir_datasets/datasets/c4.py
--rw-r--r--   0 sean       (501) staff       (20)     6123 2023-08-06 11:36:52.000000 ir_datasets-0.5.6/ir_datasets/datasets/car.py
--rw-r--r--   0 sean       (501) staff       (20)     6281 2022-10-06 08:46:46.000000 ir_datasets-0.5.6/ir_datasets/datasets/clinicaltrials.py
--rw-r--r--   0 sean       (501) staff       (20)     4642 2022-02-27 13:29:46.000000 ir_datasets-0.5.6/ir_datasets/datasets/clirmatrix.py
--rw-r--r--   0 sean       (501) staff       (20)    13622 2023-08-06 11:36:52.000000 ir_datasets-0.5.6/ir_datasets/datasets/clueweb09.py
--rw-r--r--   0 sean       (501) staff       (20)    17599 2023-08-06 11:36:52.000000 ir_datasets-0.5.6/ir_datasets/datasets/clueweb12.py
--rw-r--r--   0 sean       (501) staff       (20)     2906 2023-08-06 11:36:52.000000 ir_datasets-0.5.6/ir_datasets/datasets/codec.py
--rw-r--r--   0 sean       (501) staff       (20)     7164 2022-11-17 09:45:36.000000 ir_datasets-0.5.6/ir_datasets/datasets/codesearchnet.py
--rw-r--r--   0 sean       (501) staff       (20)    10239 2023-08-06 11:36:52.000000 ir_datasets-0.5.6/ir_datasets/datasets/cord19.py
--rw-r--r--   0 sean       (501) staff       (20)     5734 2023-08-06 11:36:52.000000 ir_datasets-0.5.6/ir_datasets/datasets/cranfield.py
--rw-r--r--   0 sean       (501) staff       (20)     5049 2022-05-24 16:02:41.000000 ir_datasets-0.5.6/ir_datasets/datasets/disks45.py
--rw-r--r--   0 sean       (501) staff       (20)     5964 2023-08-06 11:36:52.000000 ir_datasets-0.5.6/ir_datasets/datasets/dpr_w100.py
--rw-r--r--   0 sean       (501) staff       (20)     7230 2023-08-06 11:36:52.000000 ir_datasets-0.5.6/ir_datasets/datasets/gov.py
--rw-r--r--   0 sean       (501) staff       (20)    17389 2023-08-06 11:36:52.000000 ir_datasets-0.5.6/ir_datasets/datasets/gov2.py
--rw-r--r--   0 sean       (501) staff       (20)     1760 2023-06-14 14:47:39.000000 ir_datasets-0.5.6/ir_datasets/datasets/hc4.py
--rw-r--r--   0 sean       (501) staff       (20)     7758 2023-08-06 11:36:52.000000 ir_datasets-0.5.6/ir_datasets/datasets/highwire.py
--rw-r--r--   0 sean       (501) staff       (20)     2687 2023-08-06 11:36:52.000000 ir_datasets-0.5.6/ir_datasets/datasets/istella22.py
--rw-r--r--   0 sean       (501) staff       (20)     4505 2023-08-06 11:36:52.000000 ir_datasets-0.5.6/ir_datasets/datasets/kilt.py
--rw-r--r--   0 sean       (501) staff       (20)     2474 2022-03-04 12:17:39.000000 ir_datasets-0.5.6/ir_datasets/datasets/lotte.py
--rw-r--r--   0 sean       (501) staff       (20)     9892 2023-08-06 11:36:52.000000 ir_datasets-0.5.6/ir_datasets/datasets/medline.py
--rw-r--r--   0 sean       (501) staff       (20)     3618 2023-08-06 13:40:07.000000 ir_datasets-0.5.6/ir_datasets/datasets/miracl.py
--rw-r--r--   0 sean       (501) staff       (20)     4466 2022-02-27 13:29:46.000000 ir_datasets-0.5.6/ir_datasets/datasets/mmarco.py
--rw-r--r--   0 sean       (501) staff       (20)     4074 2022-02-27 13:29:46.000000 ir_datasets-0.5.6/ir_datasets/datasets/mr_tydi.py
--rw-r--r--   0 sean       (501) staff       (20)     8943 2023-08-06 11:36:52.000000 ir_datasets-0.5.6/ir_datasets/datasets/msmarco_document.py
--rw-r--r--   0 sean       (501) staff       (20)     9570 2023-08-06 11:36:52.000000 ir_datasets-0.5.6/ir_datasets/datasets/msmarco_document_v2.py
--rw-r--r--   0 sean       (501) staff       (20)    19477 2023-08-06 11:36:52.000000 ir_datasets-0.5.6/ir_datasets/datasets/msmarco_passage.py
--rw-r--r--   0 sean       (501) staff       (20)    13471 2023-08-06 11:36:52.000000 ir_datasets-0.5.6/ir_datasets/datasets/msmarco_passage_v2.py
--rw-r--r--   0 sean       (501) staff       (20)    16761 2023-08-06 11:36:52.000000 ir_datasets-0.5.6/ir_datasets/datasets/msmarco_qna.py
--rw-r--r--   0 sean       (501) staff       (20)     9749 2023-08-06 11:36:52.000000 ir_datasets-0.5.6/ir_datasets/datasets/natural_questions.py
--rw-r--r--   0 sean       (501) staff       (20)     3830 2023-06-14 14:47:39.000000 ir_datasets-0.5.6/ir_datasets/datasets/neuclir.py
--rw-r--r--   0 sean       (501) staff       (20)     2522 2022-10-06 08:46:46.000000 ir_datasets-0.5.6/ir_datasets/datasets/neumarco.py
--rw-r--r--   0 sean       (501) staff       (20)     7548 2023-08-06 11:36:52.000000 ir_datasets-0.5.6/ir_datasets/datasets/nfcorpus.py
--rw-r--r--   0 sean       (501) staff       (20)    15719 2023-08-06 11:36:52.000000 ir_datasets-0.5.6/ir_datasets/datasets/nyt.py
--rw-r--r--   0 sean       (501) staff       (20)     6362 2023-08-06 11:36:52.000000 ir_datasets-0.5.6/ir_datasets/datasets/pmc.py
--rw-r--r--   0 sean       (501) staff       (20)     3651 2023-08-06 11:36:52.000000 ir_datasets-0.5.6/ir_datasets/datasets/sara.py
--rw-r--r--   0 sean       (501) staff       (20)     8556 2022-10-18 13:10:16.000000 ir_datasets-0.5.6/ir_datasets/datasets/touche.py
--rw-r--r--   0 sean       (501) staff       (20)     1395 2022-10-18 13:10:16.000000 ir_datasets-0.5.6/ir_datasets/datasets/touche_image.py
--rw-r--r--   0 sean       (501) staff       (20)     1614 2022-02-27 13:29:46.000000 ir_datasets-0.5.6/ir_datasets/datasets/trec_arabic.py
--rw-r--r--   0 sean       (501) staff       (20)     9500 2023-08-06 11:36:52.000000 ir_datasets-0.5.6/ir_datasets/datasets/trec_cast.py
--rw-r--r--   0 sean       (501) staff       (20)    11692 2023-08-06 11:36:52.000000 ir_datasets-0.5.6/ir_datasets/datasets/trec_fair.py
--rw-r--r--   0 sean       (501) staff       (20)     2244 2023-08-06 11:36:52.000000 ir_datasets-0.5.6/ir_datasets/datasets/trec_mandarin.py
--rw-r--r--   0 sean       (501) staff       (20)     3916 2022-05-24 16:02:41.000000 ir_datasets-0.5.6/ir_datasets/datasets/trec_robust04.py
--rw-r--r--   0 sean       (501) staff       (20)     3993 2023-08-06 11:36:52.000000 ir_datasets-0.5.6/ir_datasets/datasets/trec_spanish.py
--rw-r--r--   0 sean       (501) staff       (20)     2457 2023-08-06 11:36:52.000000 ir_datasets-0.5.6/ir_datasets/datasets/trec_tot.py
--rw-r--r--   0 sean       (501) staff       (20)    16373 2023-08-06 11:36:52.000000 ir_datasets-0.5.6/ir_datasets/datasets/tripclick.py
--rw-r--r--   0 sean       (501) staff       (20)    19126 2023-08-06 11:36:52.000000 ir_datasets-0.5.6/ir_datasets/datasets/tweets2013_ia.py
--rw-r--r--   0 sean       (501) staff       (20)     3881 2022-02-27 13:29:46.000000 ir_datasets-0.5.6/ir_datasets/datasets/vaswani.py
--rw-r--r--   0 sean       (501) staff       (20)     7151 2023-08-06 11:36:52.000000 ir_datasets-0.5.6/ir_datasets/datasets/wapo.py
--rw-r--r--   0 sean       (501) staff       (20)     3077 2023-08-06 11:36:52.000000 ir_datasets-0.5.6/ir_datasets/datasets/wikiclir.py
--rw-r--r--   0 sean       (501) staff       (20)     2129 2022-02-27 13:29:46.000000 ir_datasets-0.5.6/ir_datasets/datasets/wikir.py
-drwxr-xr-x   0 sean       (501) staff       (20)        0 2024-02-04 16:14:22.000000 ir_datasets-0.5.6/ir_datasets/docs/
--rw-r--r--   0 sean       (501) staff       (20)     1265 2021-06-10 21:29:31.000000 ir_datasets-0.5.6/ir_datasets/docs/antique.yaml
--rw-r--r--   0 sean       (501) staff       (20)     1291 2022-02-27 13:29:46.000000 ir_datasets-0.5.6/ir_datasets/docs/aol-ia.yaml
--rw-r--r--   0 sean       (501) staff       (20)     1689 2021-08-03 22:56:25.000000 ir_datasets-0.5.6/ir_datasets/docs/aquaint.yaml
--rw-r--r--   0 sean       (501) staff       (20)     4214 2022-10-18 13:10:16.000000 ir_datasets-0.5.6/ir_datasets/docs/argsme.yaml
--rw-r--r--   0 sean       (501) staff       (20)    16889 2021-10-26 12:13:10.000000 ir_datasets-0.5.6/ir_datasets/docs/beir.yaml
--rw-r--r--   0 sean       (501) staff       (20)    36796 2023-08-06 13:31:47.000000 ir_datasets-0.5.6/ir_datasets/docs/bibliography.bib
--rw-r--r--   0 sean       (501) staff       (20)      643 2021-08-03 22:51:30.000000 ir_datasets-0.5.6/ir_datasets/docs/c4.yaml
--rw-r--r--   0 sean       (501) staff       (20)     2537 2022-02-27 13:29:46.000000 ir_datasets-0.5.6/ir_datasets/docs/car.yaml
--rw-r--r--   0 sean       (501) staff       (20)     2705 2022-10-06 08:46:46.000000 ir_datasets-0.5.6/ir_datasets/docs/clinicaltrials.yaml
--rw-r--r--   0 sean       (501) staff       (20)     2195 2021-06-10 21:29:31.000000 ir_datasets-0.5.6/ir_datasets/docs/clirmatrix.yaml
--rw-r--r--   0 sean       (501) staff       (20)     4530 2021-06-10 21:29:31.000000 ir_datasets-0.5.6/ir_datasets/docs/clueweb09.yaml
--rw-r--r--   0 sean       (501) staff       (20)     7470 2022-10-06 08:46:46.000000 ir_datasets-0.5.6/ir_datasets/docs/clueweb12.yaml
--rw-r--r--   0 sean       (501) staff       (20)     1349 2022-10-06 08:46:46.000000 ir_datasets-0.5.6/ir_datasets/docs/codec.yaml
--rw-r--r--   0 sean       (501) staff       (20)     1022 2021-06-10 21:29:31.000000 ir_datasets-0.5.6/ir_datasets/docs/codesearchnet.yaml
--rw-r--r--   0 sean       (501) staff       (20)     5002 2021-06-10 21:29:31.000000 ir_datasets-0.5.6/ir_datasets/docs/cord19.yaml
--rw-r--r--   0 sean       (501) staff       (20)      300 2021-05-01 10:12:08.000000 ir_datasets-0.5.6/ir_datasets/docs/cranfield.yaml
--rw-r--r--   0 sean       (501) staff       (20)     4479 2022-05-24 16:02:42.000000 ir_datasets-0.5.6/ir_datasets/docs/disks45.yaml
--rw-r--r--   0 sean       (501) staff       (20)     2184 2021-06-10 21:29:31.000000 ir_datasets-0.5.6/ir_datasets/docs/dpr-w100.yaml
--rw-r--r--   0 sean       (501) staff       (20)     3154 2021-06-10 21:29:31.000000 ir_datasets-0.5.6/ir_datasets/docs/gov.yaml
--rw-r--r--   0 sean       (501) staff       (20)     6202 2021-06-10 21:29:31.000000 ir_datasets-0.5.6/ir_datasets/docs/gov2.yaml
--rw-r--r--   0 sean       (501) staff       (20)     5257 2023-06-14 14:47:39.000000 ir_datasets-0.5.6/ir_datasets/docs/hc4.yaml
--rw-r--r--   0 sean       (501) staff       (20)     1574 2021-06-10 21:29:31.000000 ir_datasets-0.5.6/ir_datasets/docs/highwire.yaml
--rw-r--r--   0 sean       (501) staff       (20)     1169 2022-10-06 08:46:46.000000 ir_datasets-0.5.6/ir_datasets/docs/istella22.yaml
--rw-r--r--   0 sean       (501) staff       (20)     1144 2022-10-06 08:46:46.000000 ir_datasets-0.5.6/ir_datasets/docs/kilt.yaml
--rw-r--r--   0 sean       (501) staff       (20)     7868 2022-03-04 12:17:39.000000 ir_datasets-0.5.6/ir_datasets/docs/lotte.yaml
--rw-r--r--   0 sean       (501) staff       (20)     3031 2022-10-06 08:46:46.000000 ir_datasets-0.5.6/ir_datasets/docs/medline.yaml
--rw-r--r--   0 sean       (501) staff       (20)     8198 2023-08-06 13:45:16.000000 ir_datasets-0.5.6/ir_datasets/docs/miracl.yaml
--rw-r--r--   0 sean       (501) staff       (20)    17454 2022-02-27 13:29:46.000000 ir_datasets-0.5.6/ir_datasets/docs/mmarco.yaml
--rw-r--r--   0 sean       (501) staff       (20)     5608 2021-10-25 13:42:17.000000 ir_datasets-0.5.6/ir_datasets/docs/mr-tydi.yaml
--rw-r--r--   0 sean       (501) staff       (20)     3994 2023-08-06 11:36:52.000000 ir_datasets-0.5.6/ir_datasets/docs/msmarco-document-v2.yaml
--rw-r--r--   0 sean       (501) staff       (20)     5810 2022-02-27 13:29:46.000000 ir_datasets-0.5.6/ir_datasets/docs/msmarco-document.yaml
--rw-r--r--   0 sean       (501) staff       (20)     3190 2023-08-06 11:36:52.000000 ir_datasets-0.5.6/ir_datasets/docs/msmarco-passage-v2.yaml
--rw-r--r--   0 sean       (501) staff       (20)     8747 2023-08-06 11:36:52.000000 ir_datasets-0.5.6/ir_datasets/docs/msmarco-passage.yaml
--rw-r--r--   0 sean       (501) staff       (20)     2590 2021-06-10 21:29:31.000000 ir_datasets-0.5.6/ir_datasets/docs/msmarco-qna.yaml
--rw-r--r--   0 sean       (501) staff       (20)     1381 2021-06-10 21:29:31.000000 ir_datasets-0.5.6/ir_datasets/docs/natural-questions.yaml
--rw-r--r--   0 sean       (501) staff       (20)     4829 2023-06-14 14:47:39.000000 ir_datasets-0.5.6/ir_datasets/docs/neuclir.yaml
--rw-r--r--   0 sean       (501) staff       (20)     2860 2022-10-06 08:46:46.000000 ir_datasets-0.5.6/ir_datasets/docs/neumarco.yaml
--rw-r--r--   0 sean       (501) staff       (20)     2124 2021-06-10 21:29:31.000000 ir_datasets-0.5.6/ir_datasets/docs/nfcorpus.yaml
--rw-r--r--   0 sean       (501) staff       (20)     2818 2021-06-10 21:29:31.000000 ir_datasets-0.5.6/ir_datasets/docs/nyt.yaml
--rw-r--r--   0 sean       (501) staff       (20)     1787 2021-06-10 21:29:31.000000 ir_datasets-0.5.6/ir_datasets/docs/pmc.yaml
--rw-r--r--   0 sean       (501) staff       (20)      372 2023-08-06 11:36:52.000000 ir_datasets-0.5.6/ir_datasets/docs/sara.yaml
--rw-r--r--   0 sean       (501) staff       (20)     1852 2022-10-18 13:10:16.000000 ir_datasets-0.5.6/ir_datasets/docs/touche-image.yaml
--rw-r--r--   0 sean       (501) staff       (20)    13234 2022-10-18 14:42:22.000000 ir_datasets-0.5.6/ir_datasets/docs/touche.yaml
--rw-r--r--   0 sean       (501) staff       (20)     1489 2021-06-10 21:29:31.000000 ir_datasets-0.5.6/ir_datasets/docs/trec-arabic.yaml
--rw-r--r--   0 sean       (501) staff       (20)     3807 2022-02-27 13:29:46.000000 ir_datasets-0.5.6/ir_datasets/docs/trec-cast.yaml
--rw-r--r--   0 sean       (501) staff       (20)     1000 2022-10-06 08:46:46.000000 ir_datasets-0.5.6/ir_datasets/docs/trec-fair.yaml
--rw-r--r--   0 sean       (501) staff       (20)     1536 2021-06-10 21:29:31.000000 ir_datasets-0.5.6/ir_datasets/docs/trec-mandarin.yaml
--rw-r--r--   0 sean       (501) staff       (20)     2876 2022-02-28 10:52:37.000000 ir_datasets-0.5.6/ir_datasets/docs/trec-robust04.yaml
--rw-r--r--   0 sean       (501) staff       (20)     1458 2021-06-10 21:29:31.000000 ir_datasets-0.5.6/ir_datasets/docs/trec-spanish.yaml
--rw-r--r--   0 sean       (501) staff       (20)      634 2023-08-06 11:36:52.000000 ir_datasets-0.5.6/ir_datasets/docs/trec-tot.yaml
--rw-r--r--   0 sean       (501) staff       (20)     9088 2022-02-27 13:29:46.000000 ir_datasets-0.5.6/ir_datasets/docs/tripclick.yaml
--rw-r--r--   0 sean       (501) staff       (20)     1721 2021-06-10 21:29:31.000000 ir_datasets-0.5.6/ir_datasets/docs/tweets2013-ia.yaml
--rw-r--r--   0 sean       (501) staff       (20)      305 2021-01-23 11:42:50.000000 ir_datasets-0.5.6/ir_datasets/docs/vaswani.yaml
--rw-r--r--   0 sean       (501) staff       (20)     3079 2021-10-26 12:13:01.000000 ir_datasets-0.5.6/ir_datasets/docs/wapo.yaml
--rw-r--r--   0 sean       (501) staff       (20)     3047 2022-10-06 08:46:46.000000 ir_datasets-0.5.6/ir_datasets/docs/wikiclir.yaml
--rw-r--r--   0 sean       (501) staff       (20)     5125 2021-08-03 22:51:30.000000 ir_datasets-0.5.6/ir_datasets/docs/wikir.yaml
-drwxr-xr-x   0 sean       (501) staff       (20)        0 2024-02-04 16:14:22.000000 ir_datasets-0.5.6/ir_datasets/etc/
--rw-r--r--   0 sean       (501) staff       (20)   266308 2024-02-04 15:56:36.000000 ir_datasets-0.5.6/ir_datasets/etc/downloads.json
--rw-r--r--   0 sean       (501) staff       (20)   125224 2023-08-06 13:45:51.000000 ir_datasets-0.5.6/ir_datasets/etc/metadata.json
-drwxr-xr-x   0 sean       (501) staff       (20)        0 2024-02-04 16:14:22.000000 ir_datasets-0.5.6/ir_datasets/formats/
--rw-r--r--   0 sean       (501) staff       (20)     1634 2022-12-29 17:46:19.000000 ir_datasets-0.5.6/ir_datasets/formats/__init__.py
--rw-r--r--   0 sean       (501) staff       (20)    16566 2023-08-06 11:36:52.000000 ir_datasets-0.5.6/ir_datasets/formats/argsme.py
--rw-r--r--   0 sean       (501) staff       (20)    11804 2023-08-06 11:36:52.000000 ir_datasets-0.5.6/ir_datasets/formats/base.py
--rw-r--r--   0 sean       (501) staff       (20)     1299 2021-06-04 14:39:58.000000 ir_datasets-0.5.6/ir_datasets/formats/clirmatrix.py
--rw-r--r--   0 sean       (501) staff       (20)     3163 2022-02-27 13:29:46.000000 ir_datasets-0.5.6/ir_datasets/formats/csv_fmt.py
--rw-r--r--   0 sean       (501) staff       (20)     4357 2023-08-06 11:36:52.000000 ir_datasets-0.5.6/ir_datasets/formats/extracted_cc.py
--rw-r--r--   0 sean       (501) staff       (20)     2979 2023-08-06 11:58:38.000000 ir_datasets-0.5.6/ir_datasets/formats/jsonl.py
--rw-r--r--   0 sean       (501) staff       (20)      593 2021-01-23 11:42:50.000000 ir_datasets-0.5.6/ir_datasets/formats/ntcir.py
--rw-r--r--   0 sean       (501) staff       (20)    23348 2023-08-06 11:36:52.000000 ir_datasets-0.5.6/ir_datasets/formats/touche.py
--rw-r--r--   0 sean       (501) staff       (20)     8694 2022-10-18 13:10:16.000000 ir_datasets-0.5.6/ir_datasets/formats/touche_image.py
--rw-r--r--   0 sean       (501) staff       (20)    20220 2024-02-04 15:53:25.000000 ir_datasets-0.5.6/ir_datasets/formats/trec.py
--rw-r--r--   0 sean       (501) staff       (20)     7038 2022-04-22 12:40:55.000000 ir_datasets-0.5.6/ir_datasets/formats/tsv.py
--rw-r--r--   0 sean       (501) staff       (20)     3133 2023-08-06 11:36:52.000000 ir_datasets-0.5.6/ir_datasets/formats/webarc.py
-drwxr-xr-x   0 sean       (501) staff       (20)        0 2024-02-04 16:14:22.000000 ir_datasets-0.5.6/ir_datasets/indices/
--rw-r--r--   0 sean       (501) staff       (20)      366 2022-01-16 17:10:49.000000 ir_datasets-0.5.6/ir_datasets/indices/__init__.py
--rw-r--r--   0 sean       (501) staff       (20)      910 2024-02-04 15:53:25.000000 ir_datasets-0.5.6/ir_datasets/indices/base.py
--rw-r--r--   0 sean       (501) staff       (20)     1006 2021-01-23 11:42:50.000000 ir_datasets-0.5.6/ir_datasets/indices/cache_docstore.py
--rw-r--r--   0 sean       (501) staff       (20)    11317 2022-05-24 16:02:42.000000 ir_datasets-0.5.6/ir_datasets/indices/clueweb_warc.py
--rw-r--r--   0 sean       (501) staff       (20)    11612 2022-02-27 13:29:46.000000 ir_datasets-0.5.6/ir_datasets/indices/indexed_tsv_docstore.py
--rw-r--r--   0 sean       (501) staff       (20)     9776 2022-10-06 08:46:46.000000 ir_datasets-0.5.6/ir_datasets/indices/lz4_pickle.py
--rw-r--r--   0 sean       (501) staff       (20)     6147 2022-01-16 17:10:49.000000 ir_datasets-0.5.6/ir_datasets/indices/numpy_sorted_index.py
--rw-r--r--   0 sean       (501) staff       (20)     4824 2022-02-27 13:29:46.000000 ir_datasets-0.5.6/ir_datasets/indices/zpickle_docstore.py
--rw-r--r--   0 sean       (501) staff       (20)     2682 2022-12-29 17:46:19.000000 ir_datasets-0.5.6/ir_datasets/lazy_libs.py
--rw-r--r--   0 sean       (501) staff       (20)     5726 2021-10-25 13:44:15.000000 ir_datasets-0.5.6/ir_datasets/log.py
-drwxr-xr-x   0 sean       (501) staff       (20)        0 2024-02-04 16:14:22.000000 ir_datasets-0.5.6/ir_datasets/util/
--rw-r--r--   0 sean       (501) staff       (20)     9550 2022-05-24 16:02:42.000000 ir_datasets-0.5.6/ir_datasets/util/__init__.py
--rw-r--r--   0 sean       (501) staff       (20)    16067 2023-08-09 20:55:02.000000 ir_datasets-0.5.6/ir_datasets/util/download.py
--rw-r--r--   0 sean       (501) staff       (20)     9099 2022-02-27 13:29:47.000000 ir_datasets-0.5.6/ir_datasets/util/fileio.py
--rw-r--r--   0 sean       (501) staff       (20)     1433 2021-05-30 16:56:45.000000 ir_datasets-0.5.6/ir_datasets/util/hash.py
--rw-r--r--   0 sean       (501) staff       (20)     3341 2023-02-01 13:52:42.000000 ir_datasets-0.5.6/ir_datasets/util/html_parsing.py
--rw-r--r--   0 sean       (501) staff       (20)     3304 2022-02-27 13:29:47.000000 ir_datasets-0.5.6/ir_datasets/util/metadata.py
--rw-r--r--   0 sean       (501) staff       (20)     1591 2022-10-06 08:46:46.000000 ir_datasets-0.5.6/ir_datasets/util/registry.py
-drwxr-xr-x   0 sean       (501) staff       (20)        0 2024-02-04 16:14:22.000000 ir_datasets-0.5.6/ir_datasets/wrappers/
--rw-r--r--   0 sean       (501) staff       (20)       45 2021-01-23 11:42:50.000000 ir_datasets-0.5.6/ir_datasets/wrappers/__init__.py
--rw-r--r--   0 sean       (501) staff       (20)     4795 2022-10-19 19:08:01.000000 ir_datasets-0.5.6/ir_datasets/wrappers/html_extractor.py
-drwxr-xr-x   0 sean       (501) staff       (20)        0 2024-02-04 16:14:22.000000 ir_datasets-0.5.6/ir_datasets.egg-info/
--rw-r--r--   0 sean       (501) staff       (20)    13942 2024-02-04 16:14:21.000000 ir_datasets-0.5.6/ir_datasets.egg-info/PKG-INFO
--rw-r--r--   0 sean       (501) staff       (20)     5429 2024-02-04 16:14:21.000000 ir_datasets-0.5.6/ir_datasets.egg-info/SOURCES.txt
--rw-r--r--   0 sean       (501) staff       (20)        1 2024-02-04 16:14:21.000000 ir_datasets-0.5.6/ir_datasets.egg-info/dependency_links.txt
--rw-r--r--   0 sean       (501) staff       (20)       54 2024-02-04 16:14:21.000000 ir_datasets-0.5.6/ir_datasets.egg-info/entry_points.txt
--rw-r--r--   0 sean       (501) staff       (20)      253 2024-02-04 16:14:21.000000 ir_datasets-0.5.6/ir_datasets.egg-info/requires.txt
--rw-r--r--   0 sean       (501) staff       (20)       12 2024-02-04 16:14:21.000000 ir_datasets-0.5.6/ir_datasets.egg-info/top_level.txt
--rw-r--r--   0 sean       (501) staff       (20)      253 2022-12-29 17:46:19.000000 ir_datasets-0.5.6/requirements.txt
--rw-r--r--   0 sean       (501) staff       (20)       38 2024-02-04 16:14:22.000000 ir_datasets-0.5.6/setup.cfg
--rw-r--r--   0 sean       (501) staff       (20)     1000 2024-02-04 15:56:48.000000 ir_datasets-0.5.6/setup.py
-drwxr-xr-x   0 sean       (501) staff       (20)        0 2024-02-04 16:14:22.000000 ir_datasets-0.5.6/test/
--rw-r--r--   0 sean       (501) staff       (20)     1695 2023-08-06 11:36:52.000000 ir_datasets-0.5.6/test/test_defaulttext.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 13:11:14.307146 ir_datasets-0.5.7/
+-rw-r--r--   0 runner    (1001) docker     (127)    11358 2024-04-29 13:11:03.000000 ir_datasets-0.5.7/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      135 2024-04-29 13:11:03.000000 ir_datasets-0.5.7/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)    12399 2024-04-29 13:11:14.307146 ir_datasets-0.5.7/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    11600 2024-04-29 13:11:03.000000 ir_datasets-0.5.7/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 13:11:14.279146 ir_datasets-0.5.7/ir_datasets/
+-rw-r--r--   0 runner    (1001) docker     (127)     3326 2024-04-29 13:11:03.000000 ir_datasets-0.5.7/ir_datasets/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       74 2024-04-29 13:11:03.000000 ir_datasets-0.5.7/ir_datasets/__main__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 13:11:14.279146 ir_datasets-0.5.7/ir_datasets/commands/
+-rw-r--r--   0 runner    (1001) docker     (127)      638 2024-04-29 13:11:03.000000 ir_datasets-0.5.7/ir_datasets/commands/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3161 2024-04-29 13:11:03.000000 ir_datasets-0.5.7/ir_datasets/commands/build_c4_checkpoints.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1728 2024-04-29 13:11:03.000000 ir_datasets-0.5.7/ir_datasets/commands/build_clueweb_warc_indexes.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2441 2024-04-29 13:11:03.000000 ir_datasets-0.5.7/ir_datasets/commands/build_download_cache.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4090 2024-04-29 13:11:03.000000 ir_datasets-0.5.7/ir_datasets/commands/clean.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2983 2024-04-29 13:11:03.000000 ir_datasets-0.5.7/ir_datasets/commands/doc_fifos.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10515 2024-04-29 13:11:03.000000 ir_datasets-0.5.7/ir_datasets/commands/export.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3293 2024-04-29 13:11:03.000000 ir_datasets-0.5.7/ir_datasets/commands/generate_metadata.py
+-rw-r--r--   0 runner    (1001) docker     (127)      476 2024-04-29 13:11:03.000000 ir_datasets-0.5.7/ir_datasets/commands/list.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1910 2024-04-29 13:11:03.000000 ir_datasets-0.5.7/ir_datasets/commands/lookup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 13:11:14.291146 ir_datasets-0.5.7/ir_datasets/datasets/
+-rw-r--r--   0 runner    (1001) docker     (127)     1425 2024-04-29 13:11:03.000000 ir_datasets-0.5.7/ir_datasets/datasets/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5400 2024-04-29 13:11:03.000000 ir_datasets-0.5.7/ir_datasets/datasets/antique.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8293 2024-04-29 13:11:03.000000 ir_datasets-0.5.7/ir_datasets/datasets/aol_ia.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1413 2024-04-29 13:11:03.000000 ir_datasets-0.5.7/ir_datasets/datasets/aquaint.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3747 2024-04-29 13:11:03.000000 ir_datasets-0.5.7/ir_datasets/datasets/argsme.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13855 2024-04-29 13:11:03.000000 ir_datasets-0.5.7/ir_datasets/datasets/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9543 2024-04-29 13:11:03.000000 ir_datasets-0.5.7/ir_datasets/datasets/beir.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9235 2024-04-29 13:11:03.000000 ir_datasets-0.5.7/ir_datasets/datasets/c4.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6123 2024-04-29 13:11:03.000000 ir_datasets-0.5.7/ir_datasets/datasets/car.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6281 2024-04-29 13:11:03.000000 ir_datasets-0.5.7/ir_datasets/datasets/clinicaltrials.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4642 2024-04-29 13:11:03.000000 ir_datasets-0.5.7/ir_datasets/datasets/clirmatrix.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13622 2024-04-29 13:11:03.000000 ir_datasets-0.5.7/ir_datasets/datasets/clueweb09.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17599 2024-04-29 13:11:03.000000 ir_datasets-0.5.7/ir_datasets/datasets/clueweb12.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2906 2024-04-29 13:11:03.000000 ir_datasets-0.5.7/ir_datasets/datasets/codec.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7164 2024-04-29 13:11:03.000000 ir_datasets-0.5.7/ir_datasets/datasets/codesearchnet.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10239 2024-04-29 13:11:03.000000 ir_datasets-0.5.7/ir_datasets/datasets/cord19.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5734 2024-04-29 13:11:03.000000 ir_datasets-0.5.7/ir_datasets/datasets/cranfield.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1936 2024-04-29 13:11:03.000000 ir_datasets-0.5.7/ir_datasets/datasets/csl.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5049 2024-04-29 13:11:03.000000 ir_datasets-0.5.7/ir_datasets/datasets/disks45.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5964 2024-04-29 13:11:03.000000 ir_datasets-0.5.7/ir_datasets/datasets/dpr_w100.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7230 2024-04-29 13:11:03.000000 ir_datasets-0.5.7/ir_datasets/datasets/gov.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17389 2024-04-29 13:11:03.000000 ir_datasets-0.5.7/ir_datasets/datasets/gov2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1760 2024-04-29 13:11:03.000000 ir_datasets-0.5.7/ir_datasets/datasets/hc4.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7758 2024-04-29 13:11:03.000000 ir_datasets-0.5.7/ir_datasets/datasets/highwire.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2687 2024-04-29 13:11:03.000000 ir_datasets-0.5.7/ir_datasets/datasets/istella22.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4505 2024-04-29 13:11:03.000000 ir_datasets-0.5.7/ir_datasets/datasets/kilt.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2474 2024-04-29 13:11:03.000000 ir_datasets-0.5.7/ir_datasets/datasets/lotte.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9892 2024-04-29 13:11:03.000000 ir_datasets-0.5.7/ir_datasets/datasets/medline.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3618 2024-04-29 13:11:03.000000 ir_datasets-0.5.7/ir_datasets/datasets/miracl.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4466 2024-04-29 13:11:03.000000 ir_datasets-0.5.7/ir_datasets/datasets/mmarco.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4074 2024-04-29 13:11:03.000000 ir_datasets-0.5.7/ir_datasets/datasets/mr_tydi.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8943 2024-04-29 13:11:03.000000 ir_datasets-0.5.7/ir_datasets/datasets/msmarco_document.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9570 2024-04-29 13:11:03.000000 ir_datasets-0.5.7/ir_datasets/datasets/msmarco_document_v2.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19477 2024-04-29 13:11:03.000000 ir_datasets-0.5.7/ir_datasets/datasets/msmarco_passage.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13471 2024-04-29 13:11:03.000000 ir_datasets-0.5.7/ir_datasets/datasets/msmarco_passage_v2.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16761 2024-04-29 13:11:03.000000 ir_datasets-0.5.7/ir_datasets/datasets/msmarco_qna.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9749 2024-04-29 13:11:03.000000 ir_datasets-0.5.7/ir_datasets/datasets/natural_questions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5985 2024-04-29 13:11:03.000000 ir_datasets-0.5.7/ir_datasets/datasets/neuclir.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2522 2024-04-29 13:11:03.000000 ir_datasets-0.5.7/ir_datasets/datasets/neumarco.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7548 2024-04-29 13:11:03.000000 ir_datasets-0.5.7/ir_datasets/datasets/nfcorpus.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15719 2024-04-29 13:11:03.000000 ir_datasets-0.5.7/ir_datasets/datasets/nyt.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6362 2024-04-29 13:11:03.000000 ir_datasets-0.5.7/ir_datasets/datasets/pmc.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3651 2024-04-29 13:11:03.000000 ir_datasets-0.5.7/ir_datasets/datasets/sara.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8556 2024-04-29 13:11:03.000000 ir_datasets-0.5.7/ir_datasets/datasets/touche.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1395 2024-04-29 13:11:03.000000 ir_datasets-0.5.7/ir_datasets/datasets/touche_image.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1614 2024-04-29 13:11:03.000000 ir_datasets-0.5.7/ir_datasets/datasets/trec_arabic.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9500 2024-04-29 13:11:03.000000 ir_datasets-0.5.7/ir_datasets/datasets/trec_cast.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11692 2024-04-29 13:11:03.000000 ir_datasets-0.5.7/ir_datasets/datasets/trec_fair.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2244 2024-04-29 13:11:03.000000 ir_datasets-0.5.7/ir_datasets/datasets/trec_mandarin.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3916 2024-04-29 13:11:03.000000 ir_datasets-0.5.7/ir_datasets/datasets/trec_robust04.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3993 2024-04-29 13:11:03.000000 ir_datasets-0.5.7/ir_datasets/datasets/trec_spanish.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2457 2024-04-29 13:11:03.000000 ir_datasets-0.5.7/ir_datasets/datasets/trec_tot.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16373 2024-04-29 13:11:03.000000 ir_datasets-0.5.7/ir_datasets/datasets/tripclick.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19126 2024-04-29 13:11:03.000000 ir_datasets-0.5.7/ir_datasets/datasets/tweets2013_ia.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3881 2024-04-29 13:11:03.000000 ir_datasets-0.5.7/ir_datasets/datasets/vaswani.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7151 2024-04-29 13:11:03.000000 ir_datasets-0.5.7/ir_datasets/datasets/wapo.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3077 2024-04-29 13:11:03.000000 ir_datasets-0.5.7/ir_datasets/datasets/wikiclir.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2129 2024-04-29 13:11:03.000000 ir_datasets-0.5.7/ir_datasets/datasets/wikir.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 13:11:14.303146 ir_datasets-0.5.7/ir_datasets/docs/
+-rw-r--r--   0 runner    (1001) docker     (127)     1265 2024-04-29 13:11:03.000000 ir_datasets-0.5.7/ir_datasets/docs/antique.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1291 2024-04-29 13:11:03.000000 ir_datasets-0.5.7/ir_datasets/docs/aol-ia.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1689 2024-04-29 13:11:03.000000 ir_datasets-0.5.7/ir_datasets/docs/aquaint.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     4214 2024-04-29 13:11:03.000000 ir_datasets-0.5.7/ir_datasets/docs/argsme.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)    16889 2024-04-29 13:11:03.000000 ir_datasets-0.5.7/ir_datasets/docs/beir.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)    36796 2024-04-29 13:11:03.000000 ir_datasets-0.5.7/ir_datasets/docs/bibliography.bib
+-rw-r--r--   0 runner    (1001) docker     (127)      643 2024-04-29 13:11:03.000000 ir_datasets-0.5.7/ir_datasets/docs/c4.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     2537 2024-04-29 13:11:03.000000 ir_datasets-0.5.7/ir_datasets/docs/car.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     2705 2024-04-29 13:11:03.000000 ir_datasets-0.5.7/ir_datasets/docs/clinicaltrials.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     2195 2024-04-29 13:11:03.000000 ir_datasets-0.5.7/ir_datasets/docs/clirmatrix.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     4530 2024-04-29 13:11:03.000000 ir_datasets-0.5.7/ir_datasets/docs/clueweb09.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     7470 2024-04-29 13:11:03.000000 ir_datasets-0.5.7/ir_datasets/docs/clueweb12.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1349 2024-04-29 13:11:03.000000 ir_datasets-0.5.7/ir_datasets/docs/codec.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1022 2024-04-29 13:11:03.000000 ir_datasets-0.5.7/ir_datasets/docs/codesearchnet.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     5002 2024-04-29 13:11:03.000000 ir_datasets-0.5.7/ir_datasets/docs/cord19.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      300 2024-04-29 13:11:03.000000 ir_datasets-0.5.7/ir_datasets/docs/cranfield.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      192 2024-04-29 13:11:03.000000 ir_datasets-0.5.7/ir_datasets/docs/csl.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     4479 2024-04-29 13:11:03.000000 ir_datasets-0.5.7/ir_datasets/docs/disks45.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     2184 2024-04-29 13:11:03.000000 ir_datasets-0.5.7/ir_datasets/docs/dpr-w100.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     3154 2024-04-29 13:11:03.000000 ir_datasets-0.5.7/ir_datasets/docs/gov.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     6202 2024-04-29 13:11:03.000000 ir_datasets-0.5.7/ir_datasets/docs/gov2.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     5257 2024-04-29 13:11:03.000000 ir_datasets-0.5.7/ir_datasets/docs/hc4.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1574 2024-04-29 13:11:03.000000 ir_datasets-0.5.7/ir_datasets/docs/highwire.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1169 2024-04-29 13:11:03.000000 ir_datasets-0.5.7/ir_datasets/docs/istella22.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1144 2024-04-29 13:11:03.000000 ir_datasets-0.5.7/ir_datasets/docs/kilt.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     7868 2024-04-29 13:11:03.000000 ir_datasets-0.5.7/ir_datasets/docs/lotte.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     3031 2024-04-29 13:11:03.000000 ir_datasets-0.5.7/ir_datasets/docs/medline.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     8198 2024-04-29 13:11:03.000000 ir_datasets-0.5.7/ir_datasets/docs/miracl.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)    17454 2024-04-29 13:11:03.000000 ir_datasets-0.5.7/ir_datasets/docs/mmarco.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     5608 2024-04-29 13:11:03.000000 ir_datasets-0.5.7/ir_datasets/docs/mr-tydi.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     3994 2024-04-29 13:11:03.000000 ir_datasets-0.5.7/ir_datasets/docs/msmarco-document-v2.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     5810 2024-04-29 13:11:03.000000 ir_datasets-0.5.7/ir_datasets/docs/msmarco-document.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     3190 2024-04-29 13:11:03.000000 ir_datasets-0.5.7/ir_datasets/docs/msmarco-passage-v2.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     8747 2024-04-29 13:11:03.000000 ir_datasets-0.5.7/ir_datasets/docs/msmarco-passage.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     2590 2024-04-29 13:11:03.000000 ir_datasets-0.5.7/ir_datasets/docs/msmarco-qna.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1381 2024-04-29 13:11:03.000000 ir_datasets-0.5.7/ir_datasets/docs/natural-questions.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     3992 2024-04-29 13:11:03.000000 ir_datasets-0.5.7/ir_datasets/docs/neuclir.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     2860 2024-04-29 13:11:03.000000 ir_datasets-0.5.7/ir_datasets/docs/neumarco.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     2124 2024-04-29 13:11:03.000000 ir_datasets-0.5.7/ir_datasets/docs/nfcorpus.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     2818 2024-04-29 13:11:03.000000 ir_datasets-0.5.7/ir_datasets/docs/nyt.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1787 2024-04-29 13:11:03.000000 ir_datasets-0.5.7/ir_datasets/docs/pmc.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      372 2024-04-29 13:11:03.000000 ir_datasets-0.5.7/ir_datasets/docs/sara.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1852 2024-04-29 13:11:03.000000 ir_datasets-0.5.7/ir_datasets/docs/touche-image.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)    13234 2024-04-29 13:11:03.000000 ir_datasets-0.5.7/ir_datasets/docs/touche.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1489 2024-04-29 13:11:03.000000 ir_datasets-0.5.7/ir_datasets/docs/trec-arabic.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     3807 2024-04-29 13:11:03.000000 ir_datasets-0.5.7/ir_datasets/docs/trec-cast.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1000 2024-04-29 13:11:03.000000 ir_datasets-0.5.7/ir_datasets/docs/trec-fair.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1536 2024-04-29 13:11:03.000000 ir_datasets-0.5.7/ir_datasets/docs/trec-mandarin.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     2876 2024-04-29 13:11:03.000000 ir_datasets-0.5.7/ir_datasets/docs/trec-robust04.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1458 2024-04-29 13:11:03.000000 ir_datasets-0.5.7/ir_datasets/docs/trec-spanish.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      634 2024-04-29 13:11:03.000000 ir_datasets-0.5.7/ir_datasets/docs/trec-tot.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     9088 2024-04-29 13:11:03.000000 ir_datasets-0.5.7/ir_datasets/docs/tripclick.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1721 2024-04-29 13:11:03.000000 ir_datasets-0.5.7/ir_datasets/docs/tweets2013-ia.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      305 2024-04-29 13:11:03.000000 ir_datasets-0.5.7/ir_datasets/docs/vaswani.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     3079 2024-04-29 13:11:03.000000 ir_datasets-0.5.7/ir_datasets/docs/wapo.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     3047 2024-04-29 13:11:03.000000 ir_datasets-0.5.7/ir_datasets/docs/wikiclir.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     5125 2024-04-29 13:11:03.000000 ir_datasets-0.5.7/ir_datasets/docs/wikir.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 13:11:14.303146 ir_datasets-0.5.7/ir_datasets/etc/
+-rw-r--r--   0 runner    (1001) docker     (127)   268112 2024-04-29 13:11:03.000000 ir_datasets-0.5.7/ir_datasets/etc/downloads.json
+-rw-r--r--   0 runner    (1001) docker     (127)   127051 2024-04-29 13:11:03.000000 ir_datasets-0.5.7/ir_datasets/etc/metadata.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 13:11:14.303146 ir_datasets-0.5.7/ir_datasets/formats/
+-rw-r--r--   0 runner    (1001) docker     (127)     1721 2024-04-29 13:11:03.000000 ir_datasets-0.5.7/ir_datasets/formats/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16566 2024-04-29 13:11:03.000000 ir_datasets-0.5.7/ir_datasets/formats/argsme.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11804 2024-04-29 13:11:03.000000 ir_datasets-0.5.7/ir_datasets/formats/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1299 2024-04-29 13:11:03.000000 ir_datasets-0.5.7/ir_datasets/formats/clirmatrix.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3163 2024-04-29 13:11:03.000000 ir_datasets-0.5.7/ir_datasets/formats/csv_fmt.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8735 2024-04-29 13:11:03.000000 ir_datasets-0.5.7/ir_datasets/formats/extracted_cc.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2979 2024-04-29 13:11:03.000000 ir_datasets-0.5.7/ir_datasets/formats/jsonl.py
+-rw-r--r--   0 runner    (1001) docker     (127)      593 2024-04-29 13:11:03.000000 ir_datasets-0.5.7/ir_datasets/formats/ntcir.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23348 2024-04-29 13:11:03.000000 ir_datasets-0.5.7/ir_datasets/formats/touche.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8694 2024-04-29 13:11:03.000000 ir_datasets-0.5.7/ir_datasets/formats/touche_image.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20220 2024-04-29 13:11:03.000000 ir_datasets-0.5.7/ir_datasets/formats/trec.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7056 2024-04-29 13:11:03.000000 ir_datasets-0.5.7/ir_datasets/formats/tsv.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3133 2024-04-29 13:11:03.000000 ir_datasets-0.5.7/ir_datasets/formats/webarc.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 13:11:14.307146 ir_datasets-0.5.7/ir_datasets/indices/
+-rw-r--r--   0 runner    (1001) docker     (127)      366 2024-04-29 13:11:03.000000 ir_datasets-0.5.7/ir_datasets/indices/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      910 2024-04-29 13:11:03.000000 ir_datasets-0.5.7/ir_datasets/indices/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1006 2024-04-29 13:11:03.000000 ir_datasets-0.5.7/ir_datasets/indices/cache_docstore.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11317 2024-04-29 13:11:03.000000 ir_datasets-0.5.7/ir_datasets/indices/clueweb_warc.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11612 2024-04-29 13:11:03.000000 ir_datasets-0.5.7/ir_datasets/indices/indexed_tsv_docstore.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9776 2024-04-29 13:11:03.000000 ir_datasets-0.5.7/ir_datasets/indices/lz4_pickle.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6147 2024-04-29 13:11:03.000000 ir_datasets-0.5.7/ir_datasets/indices/numpy_sorted_index.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4824 2024-04-29 13:11:03.000000 ir_datasets-0.5.7/ir_datasets/indices/zpickle_docstore.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2841 2024-04-29 13:11:03.000000 ir_datasets-0.5.7/ir_datasets/lazy_libs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5726 2024-04-29 13:11:03.000000 ir_datasets-0.5.7/ir_datasets/log.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 13:11:14.307146 ir_datasets-0.5.7/ir_datasets/util/
+-rw-r--r--   0 runner    (1001) docker     (127)     9550 2024-04-29 13:11:03.000000 ir_datasets-0.5.7/ir_datasets/util/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16850 2024-04-29 13:11:03.000000 ir_datasets-0.5.7/ir_datasets/util/download.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9099 2024-04-29 13:11:03.000000 ir_datasets-0.5.7/ir_datasets/util/fileio.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1433 2024-04-29 13:11:03.000000 ir_datasets-0.5.7/ir_datasets/util/hash.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3341 2024-04-29 13:11:03.000000 ir_datasets-0.5.7/ir_datasets/util/html_parsing.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3304 2024-04-29 13:11:03.000000 ir_datasets-0.5.7/ir_datasets/util/metadata.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1591 2024-04-29 13:11:03.000000 ir_datasets-0.5.7/ir_datasets/util/registry.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 13:11:14.307146 ir_datasets-0.5.7/ir_datasets/wrappers/
+-rw-r--r--   0 runner    (1001) docker     (127)       45 2024-04-29 13:11:03.000000 ir_datasets-0.5.7/ir_datasets/wrappers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4795 2024-04-29 13:11:03.000000 ir_datasets-0.5.7/ir_datasets/wrappers/html_extractor.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 13:11:14.307146 ir_datasets-0.5.7/ir_datasets.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    12399 2024-04-29 13:11:14.000000 ir_datasets-0.5.7/ir_datasets.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     5483 2024-04-29 13:11:14.000000 ir_datasets-0.5.7/ir_datasets.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-29 13:11:14.000000 ir_datasets-0.5.7/ir_datasets.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       53 2024-04-29 13:11:14.000000 ir_datasets-0.5.7/ir_datasets.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      233 2024-04-29 13:11:14.000000 ir_datasets-0.5.7/ir_datasets.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       12 2024-04-29 13:11:14.000000 ir_datasets-0.5.7/ir_datasets.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      233 2024-04-29 13:11:03.000000 ir_datasets-0.5.7/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-29 13:11:14.307146 ir_datasets-0.5.7/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1000 2024-04-29 13:11:03.000000 ir_datasets-0.5.7/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 13:11:14.307146 ir_datasets-0.5.7/test/
+-rw-r--r--   0 runner    (1001) docker     (127)     1695 2024-04-29 13:11:03.000000 ir_datasets-0.5.7/test/test_defaulttext.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `ir_datasets-0.5.6/LICENSE` & `ir_datasets-0.5.7/LICENSE`

 * *Files identical despite different names*

### Comparing `ir_datasets-0.5.6/PKG-INFO` & `ir_datasets-0.5.7/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,257 +1,270 @@
 Metadata-Version: 2.1
 Name: ir_datasets
-Version: 0.5.6
+Version: 0.5.7
 Summary: provides a common interface to many IR ad-hoc ranking benchmarks, training datasets, etc.
 Home-page: https://github.com/allenai/ir_datasets
 Author: Sean MacAvaney
 Author-email: sean.macavaney@glasgow.ac.uk
-License: UNKNOWN
-Description: # ir_datasets
-        
-        `ir_datasets` is a python package that provides a common interface to many IR ad-hoc ranking
-        benchmarks, training datasets, etc.
-        
-        The package takes care of downloading datasets (including documents, queries, relevance judgments,
-        etc.) when available from public sources. Instructions on how to obtain datasets are provided when
-        they are not publicly available.
-        
-        `ir_datasets` provides a common iterator format to allow them to be easily used in python. It
-        attempts to provide the data in an unaltered form (i.e., keeping all fields and markup), while
-        handling differences in file formats, encoding, etc. Adapters provide extra functionality, e.g., to
-        allow quick lookups of documents by ID.
-        
-        A command line interface is also available.
-        
-        You can find a list of datasets and their features [here](https://ir-datasets.com/).
-        Want a new dataset, added functionality, or a bug fixed? Feel free to post an issue or make a pull request! 
-        
-        ## Getting Started
-        
-        For a quick start with the Python API, check out our Colab tutorials:
-        [Python](https://colab.research.google.com/github/allenai/ir_datasets/blob/master/examples/ir_datasets.ipynb)
-        [Command Line](https://colab.research.google.com/github/allenai/ir_datasets/blob/master/examples/ir_datasets_cli.ipynb)
-        
-        Install via pip:
-        
-        ```
-        pip install ir_datasets
-        ```
-        
-        If you want the main branch, you install as such:
-        
-        ```
-        pip install git+https://github.com/allenai/ir_datasets.git
-        ```
-        
-        If you want to build from source, use:
-        
-        ```
-        $ git clone https://github.com/allenai/ir_datasets
-        $ cd ir_datasets
-        $ python setup.py bdist_wheel
-        $ pip install dist/ir_datasets-*.whl
-        ```
-        
-        Tested with python versions 3.7, 3.8, 3.9, and 3.10. (Mininum python version is 3.7.)
-        
-        ## Features
-        
-        **Python and Command Line Interfaces**. Access datasts both through a simple Python API and
-        via the command line.
-        
-        ```python
-        import ir_datasets
-        dataset = ir_datasets.load('msmarco-passage/train')
-        # Documents
-        for doc in dataset.docs_iter():
-            print(doc)
-        # GenericDoc(doc_id='0', text='The presence of communication amid scientific minds was equa...
-        # GenericDoc(doc_id='1', text='The Manhattan Project and its atomic bomb helped bring an en...
-        # ...
-        ```
-        
-        ```bash
-        ir_datasets export msmarco-passage/train docs | head -n2
-        0 The presence of communication amid scientific minds was equally important to the success of the Manh...
-        1 The Manhattan Project and its atomic bomb helped bring an end to World War II. Its legacy of peacefu...
-        ```
-        
-        **Automatically downloads source files** (when available). Will download and verify the source
-        files for queries, documents, qrels, etc. when they are publicly available, as they are needed.
-        A CI build checks weekly to ensure that all the downloadable content is available and correct:
-        [![Downloadable Content](https://github.com/seanmacavaney/ir-datasets.com/actions/workflows/verify_downloads.yml/badge.svg)](https://github.com/seanmacavaney/ir-datasets.com/actions/workflows/verify_downloads.yml).
-        We mirror some troublesome files on [mirror.ir-datasets.com](https://mirror.ir-datasets.com/), and
-        automatically switch to the mirror when the original source is not available.
-        
-        ```python
-        import ir_datasets
-        dataset = ir_datasets.load('msmarco-passage/train')
-        for doc in dataset.docs_iter(): # Will download and extract MS-MARCO's collection.tar.gz the first time
-            ...
-        for query in dataset.queries_iter(): # Will download and extract MS-MARCO's queries.tar.gz the first time
-            ...
-        ```
-        
-        **Instructions for dataset access** (when not publicly available). Provides instructions on how
-        to get a copy of the data when it is not publicly available online (e.g., when it requires a
-        data usage agreement).
-        
-        ```python
-        import ir_datasets
-        dataset = ir_datasets.load('trec-arabic')
-        for doc in dataset.docs_iter():
-            ...
-        # Provides the following instructions:
-        # The dataset is based on the Arabic Newswire corpus. It is available from the LDC via: <https://catalog.ldc.upenn.edu/LDC2001T55>
-        # To proceed, symlink the source file here: [gives path]
-        ```
-        
-        **Support for datasets big and small**. By using iterators, supports large datasets that may
-        not fit into system memory, such as ClueWeb.
-        
-        ```python
-        import ir_datasets
-        dataset = ir_datasets.load('clueweb09')
-        for doc in dataset.docs_iter():
-            ... # will iterate through all ~1B documents
-        ```
-        
-        **Fixes known dataset issues**. For instance, automatically corrects the document UTF-8 encoding
-        problem in the MS-MARCO passage collection.
-        
-        ```python
-        import ir_datasets
-        dataset = ir_datasets.load('msmarco-passage')
-        docstore = dataset.docs_store()
-        docstore.get('243').text
-        # "John Maynard Keynes, 1st Baron Keynes, CB, FBA (/ˈkeɪnz/ KAYNZ; 5 June 1883 – 21 April [SNIP]"
-        # Naïve UTF-8 decoding yields double-encoding artifacts like:
-        # "John Maynard Keynes, 1st Baron Keynes, CB, FBA (/Ë\x88keÉªnz/ KAYNZ; 5 June 1883 â\x80\x93 21 April [SNIP]"
-        #                                                  ~~~~~~  ~~                       ~~~~~~~~~
-        ```
-        
-        **Fast Random Document Access.** Builds data structures that allow fast and efficient lookup of
-        document content. For large datasets, such as ClueWeb, uses
-        [checkpoint files](https://ir-datasets.com/clueweb_warc_checkpoints.md) to load documents from
-        source 40x faster than normal. Results are cached for even faster subsequent accesses.
-        
-        ```python
-        import ir_datasets
-        dataset = ir_datasets.load('clueweb12')
-        docstore = dataset.docs_store()
-        docstore.get_many(['clueweb12-0000tw-05-00014', 'clueweb12-0000tw-05-12119', 'clueweb12-0106wb-18-19516'])
-        # {'clueweb12-0000tw-05-00014': ..., 'clueweb12-0000tw-05-12119': ..., 'clueweb12-0106wb-18-19516': ...}
-        ```
-        
-        **Fancy Iter Slicing.** Sometimes it's helpful to be able to select ranges of data (e.g., for processing
-        document collections in parallel on multiple devices). Efficient implementations of slicing operations
-        allow for much faster dataset partitioning than using `itertools.slice`.
-        
-        ```python
-        import ir_datasets
-        dataset = ir_datasets.load('clueweb12')
-        dataset.docs_iter()[500:1000] # normal slicing behavior
-        # WarcDoc(doc_id='clueweb12-0000tw-00-00502', ...), WarcDoc(doc_id='clueweb12-0000tw-00-00503', ...), ...
-        dataset.docs_iter()[-10:-8] # includes negative indexing
-        # WarcDoc(doc_id='clueweb12-1914wb-28-24245', ...), WarcDoc(doc_id='clueweb12-1914wb-28-24246', ...)
-        dataset.docs_iter()[::100] # includes support for skip (only positive values)
-        # WarcDoc(doc_id='clueweb12-0000tw-00-00000', ...), WarcDoc(doc_id='clueweb12-0000tw-00-00100', ...), ...
-        dataset.docs_iter()[1/3:2/3] # supports proportional slicing (this takes the middle third of the collection)
-        # WarcDoc(doc_id='clueweb12-0605wb-28-12714', ...), WarcDoc(doc_id='clueweb12-0605wb-28-12715', ...), ...
-        ```
-        
-        ## Datasets
-        
-        Available datasets include:
-         - [ANTIQUE](https://ir-datasets.com/antique.html)
-         - [AQUAINT](https://ir-datasets.com/aquaint.html)
-         - [BEIR (benchmark suite)](https://ir-datasets.com/beir.html)
-         - [TREC CAR](https://ir-datasets.com/car.html)
-         - [C4](https://ir-datasets.com/c4.html)
-         - [ClueWeb09](https://ir-datasets.com/clueweb09.html)
-         - [ClueWeb12](https://ir-datasets.com/clueweb12.html)
-         - [CLIRMatrix](https://ir-datasets.com/clirmatrix.html)
-         - [CodeSearchNet](https://ir-datasets.com/codesearchnet.html)
-         - [CORD-19](https://ir-datasets.com/cord19.html)
-         - [DPR Wiki100](https://ir-datasets.com/dpr-w100.html)
-         - [GOV](https://ir-datasets.com/gov.html)
-         - [GOV2](https://ir-datasets.com/gov2.html)
-         - [HC4](https://ir-datasets.com/hc4.html)
-         - [Highwire (TREC Genomics 2006-07)](https://ir-datasets.com/highwire.html)
-         - [Medline](https://ir-datasets.com/medline.html)
-         - [MSMARCO (document)](https://ir-datasets.com/msmarco-document.html)
-         - [MSMARCO (passage)](https://ir-datasets.com/msmarco-passage.html)
-         - [MSMARCO (QnA)](https://ir-datasets.com/msmarco-qna.html)
-         - [Natural Questions](https://ir-datasets.com/natural-questions.html)
-         - [NFCorpus (NutritionFacts)](https://ir-datasets.com/nfcorpus.html)
-         - [NYT](https://ir-datasets.com/nyt.html)
-         - [PubMed Central (TREC CDS)](https://ir-datasets.com/pmc.html)
-         - [TREC Arabic](https://ir-datasets.com/trec-arabic.html)
-         - [TREC Fair Ranking 2021](https://ir-datasets.com/trec-fair-2021.html)
-         - [TREC Mandarin](https://ir-datasets.com/trec-mandarin.html)
-         - [TREC Robust 2004](https://ir-datasets.com/trec-robust04.html)
-         - [TREC Spanish](https://ir-datasets.com/trec-spanish.html)
-         - [TripClick](https://ir-datasets.com/tripclick.html)
-         - [Tweets 2013 (Internet Archive)](https://ir-datasets.com/tweets2013-ia.html)
-         - [Vaswani](https://ir-datasets.com/vaswani.html)
-         - [Washington Post](https://ir-datasets.com/wapo.html)
-         - [WikIR](https://ir-datasets.com/wikir.html)
-        
-        There are "subsets" under each dataset. For instance, `clueweb12/b13/trec-misinfo-2019` provides the
-        queries and judgments from the [2019 TREC misinformation track](https://trec.nist.gov/data/misinfo2019.html),
-        and `msmarco-document/orcas` provides the [ORCAS dataset](https://microsoft.github.io/msmarco/ORCAS). They
-        tend to be organized with the document collection at the top level.
-        
-        See the ir_dataets docs ([ir_datasets.com](https://ir-datasets.com/)) for details about each
-        dataset, its available subsets, and what data they provide.
-        
-        ## Environment variables
-        
-         - `IR_DATASETS_HOME`: Home directory for ir_datasets data (default `~/.ir_datasets/`). Contains directories
-           for each top-level dataset.
-         - `IR_DATASETS_TMP`: Temporary working directory (default `/tmp/ir_datasets/`).
-         - `IR_DATASETS_DL_TIMEOUT`: Download stream read timeout, in seconds (default `15`). If no data is received
-           within this duration, the connection will be assumed to be dead, and another download may be attempted.
-         - `IR_DATASETS_DL_TRIES`: Default number of download attempts before exception is thrown (default `3`).
-           When the server accepts Range requests, uses them. Otherwise, will download the entire file again
-         - `IR_DATASETS_DL_DISABLE_PBAR`: Set to `true` to disable the progress bar for downloads. Useful in settings
-           where an interactive console is not available.
-         - `IR_DATASETS_DL_SKIP_SSL`: Set to `true` to disable checking SSL certificates when downloading files.
-           Useful as a short-term solution when SSL certificates expire or are otherwise invalid. Note that this
-           does not disable hash verification of the downloaded content.
-         - `IR_DATASETS_SKIP_DISK_FREE`: Set to `true` to disable checks for enough free space on disk before
-           downloading content or otherwise creating large files.
-         - `IR_DATASETS_SMALL_FILE_SIZE`: The size of files that are considered "small", in bytes. Instructions for
-           linking small files rather then downloading them are not shown. Defaults to 5000000 (5MB).
-        
-        ## Citing
-        
-        When using datasets provided by this package, be sure to properly cite them. Bibtex for each dataset
-        can be found on the [datasets documentation page](https://ir-datasets.com/).
-        
-        If you use this tool, please cite [our SIGIR resource paper](https://arxiv.org/pdf/2103.02280.pdf):
-        
-        ```
-        @inproceedings{macavaney:sigir2021-irds,
-          author = {MacAvaney, Sean and Yates, Andrew and Feldman, Sergey and Downey, Doug and Cohan, Arman and Goharian, Nazli},
-          title = {Simplified Data Wrangling with ir_datasets},
-          year = {2021},
-          booktitle = {SIGIR}
-        }
-        ```
-        
-        ## Credits
-        
-        Contributors to this repository:
-        
-         - Sean MacAvaney (University of Glasgow)
-         - Shuo Sun (Johns Hopkins University)
-         - Thomas Jänich (University of Glasgow)
-         - Jan Heinrich Reimer (Martin Luther University Halle-Wittenberg)
-         - Maik Fröbe (Martin Luther University Halle-Wittenberg)
-         - Eugene Yang (Johns Hopkins University)
-         - Augustin Godinot (NAVERLABS Europe, ENS Paris-Saclay)
-        
-Platform: UNKNOWN
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
+License-File: LICENSE
+Requires-Dist: beautifulsoup4>=4.4.1
+Requires-Dist: inscriptis>=2.2.0
+Requires-Dist: lxml>=4.5.2
+Requires-Dist: numpy>=1.18.1
+Requires-Dist: pyyaml>=5.3.1
+Requires-Dist: requests>=2.22.0
+Requires-Dist: tqdm>=4.38.0
+Requires-Dist: trec-car-tools>=2.5.4
+Requires-Dist: lz4>=3.1.10
+Requires-Dist: warc3-wet>=0.2.3
+Requires-Dist: warc3-wet-clueweb09>=0.2.5
+Requires-Dist: zlib-state>=0.1.3
+Requires-Dist: ijson>=3.1.3
+Requires-Dist: unlzw3>=0.2.1
+
+# ir_datasets
+
+`ir_datasets` is a python package that provides a common interface to many IR ad-hoc ranking
+benchmarks, training datasets, etc.
+
+The package takes care of downloading datasets (including documents, queries, relevance judgments,
+etc.) when available from public sources. Instructions on how to obtain datasets are provided when
+they are not publicly available.
+
+`ir_datasets` provides a common iterator format to allow them to be easily used in python. It
+attempts to provide the data in an unaltered form (i.e., keeping all fields and markup), while
+handling differences in file formats, encoding, etc. Adapters provide extra functionality, e.g., to
+allow quick lookups of documents by ID.
+
+A command line interface is also available.
+
+You can find a list of datasets and their features [here](https://ir-datasets.com/).
+Want a new dataset, added functionality, or a bug fixed? Feel free to post an issue or make a pull request! 
+
+## Getting Started
+
+For a quick start with the Python API, check out our Colab tutorials:
+[Python](https://colab.research.google.com/github/allenai/ir_datasets/blob/master/examples/ir_datasets.ipynb)
+[Command Line](https://colab.research.google.com/github/allenai/ir_datasets/blob/master/examples/ir_datasets_cli.ipynb)
+
+Install via pip:
+
+```
+pip install ir_datasets
+```
+
+If you want the main branch, you install as such:
+
+```
+pip install git+https://github.com/allenai/ir_datasets.git
+```
+
+If you want to build from source, use:
+
+```
+$ git clone https://github.com/allenai/ir_datasets
+$ cd ir_datasets
+$ python setup.py bdist_wheel
+$ pip install dist/ir_datasets-*.whl
+```
+
+Tested with python versions 3.7, 3.8, 3.9, and 3.10. (Mininum python version is 3.7.)
+
+## Features
+
+**Python and Command Line Interfaces**. Access datasts both through a simple Python API and
+via the command line.
+
+```python
+import ir_datasets
+dataset = ir_datasets.load('msmarco-passage/train')
+# Documents
+for doc in dataset.docs_iter():
+    print(doc)
+# GenericDoc(doc_id='0', text='The presence of communication amid scientific minds was equa...
+# GenericDoc(doc_id='1', text='The Manhattan Project and its atomic bomb helped bring an en...
+# ...
+```
+
+```bash
+ir_datasets export msmarco-passage/train docs | head -n2
+0 The presence of communication amid scientific minds was equally important to the success of the Manh...
+1 The Manhattan Project and its atomic bomb helped bring an end to World War II. Its legacy of peacefu...
+```
+
+**Automatically downloads source files** (when available). Will download and verify the source
+files for queries, documents, qrels, etc. when they are publicly available, as they are needed.
+A CI build checks weekly to ensure that all the downloadable content is available and correct:
+[![Downloadable Content](https://github.com/seanmacavaney/ir-datasets.com/actions/workflows/verify_downloads.yml/badge.svg)](https://github.com/seanmacavaney/ir-datasets.com/actions/workflows/verify_downloads.yml).
+We mirror some troublesome files on [mirror.ir-datasets.com](https://mirror.ir-datasets.com/), and
+automatically switch to the mirror when the original source is not available.
+
+```python
+import ir_datasets
+dataset = ir_datasets.load('msmarco-passage/train')
+for doc in dataset.docs_iter(): # Will download and extract MS-MARCO's collection.tar.gz the first time
+    ...
+for query in dataset.queries_iter(): # Will download and extract MS-MARCO's queries.tar.gz the first time
+    ...
+```
+
+**Instructions for dataset access** (when not publicly available). Provides instructions on how
+to get a copy of the data when it is not publicly available online (e.g., when it requires a
+data usage agreement).
+
+```python
+import ir_datasets
+dataset = ir_datasets.load('trec-arabic')
+for doc in dataset.docs_iter():
+    ...
+# Provides the following instructions:
+# The dataset is based on the Arabic Newswire corpus. It is available from the LDC via: <https://catalog.ldc.upenn.edu/LDC2001T55>
+# To proceed, symlink the source file here: [gives path]
+```
+
+**Support for datasets big and small**. By using iterators, supports large datasets that may
+not fit into system memory, such as ClueWeb.
+
+```python
+import ir_datasets
+dataset = ir_datasets.load('clueweb09')
+for doc in dataset.docs_iter():
+    ... # will iterate through all ~1B documents
+```
+
+**Fixes known dataset issues**. For instance, automatically corrects the document UTF-8 encoding
+problem in the MS-MARCO passage collection.
+
+```python
+import ir_datasets
+dataset = ir_datasets.load('msmarco-passage')
+docstore = dataset.docs_store()
+docstore.get('243').text
+# "John Maynard Keynes, 1st Baron Keynes, CB, FBA (/ˈkeɪnz/ KAYNZ; 5 June 1883 – 21 April [SNIP]"
+# Naïve UTF-8 decoding yields double-encoding artifacts like:
+# "John Maynard Keynes, 1st Baron Keynes, CB, FBA (/Ë\x88keÉªnz/ KAYNZ; 5 June 1883 â\x80\x93 21 April [SNIP]"
+#                                                  ~~~~~~  ~~                       ~~~~~~~~~
+```
+
+**Fast Random Document Access.** Builds data structures that allow fast and efficient lookup of
+document content. For large datasets, such as ClueWeb, uses
+[checkpoint files](https://ir-datasets.com/clueweb_warc_checkpoints.md) to load documents from
+source 40x faster than normal. Results are cached for even faster subsequent accesses.
+
+```python
+import ir_datasets
+dataset = ir_datasets.load('clueweb12')
+docstore = dataset.docs_store()
+docstore.get_many(['clueweb12-0000tw-05-00014', 'clueweb12-0000tw-05-12119', 'clueweb12-0106wb-18-19516'])
+# {'clueweb12-0000tw-05-00014': ..., 'clueweb12-0000tw-05-12119': ..., 'clueweb12-0106wb-18-19516': ...}
+```
+
+**Fancy Iter Slicing.** Sometimes it's helpful to be able to select ranges of data (e.g., for processing
+document collections in parallel on multiple devices). Efficient implementations of slicing operations
+allow for much faster dataset partitioning than using `itertools.slice`.
+
+```python
+import ir_datasets
+dataset = ir_datasets.load('clueweb12')
+dataset.docs_iter()[500:1000] # normal slicing behavior
+# WarcDoc(doc_id='clueweb12-0000tw-00-00502', ...), WarcDoc(doc_id='clueweb12-0000tw-00-00503', ...), ...
+dataset.docs_iter()[-10:-8] # includes negative indexing
+# WarcDoc(doc_id='clueweb12-1914wb-28-24245', ...), WarcDoc(doc_id='clueweb12-1914wb-28-24246', ...)
+dataset.docs_iter()[::100] # includes support for skip (only positive values)
+# WarcDoc(doc_id='clueweb12-0000tw-00-00000', ...), WarcDoc(doc_id='clueweb12-0000tw-00-00100', ...), ...
+dataset.docs_iter()[1/3:2/3] # supports proportional slicing (this takes the middle third of the collection)
+# WarcDoc(doc_id='clueweb12-0605wb-28-12714', ...), WarcDoc(doc_id='clueweb12-0605wb-28-12715', ...), ...
+```
+
+## Datasets
+
+Available datasets include:
+ - [ANTIQUE](https://ir-datasets.com/antique.html)
+ - [AQUAINT](https://ir-datasets.com/aquaint.html)
+ - [BEIR (benchmark suite)](https://ir-datasets.com/beir.html)
+ - [TREC CAR](https://ir-datasets.com/car.html)
+ - [C4](https://ir-datasets.com/c4.html)
+ - [ClueWeb09](https://ir-datasets.com/clueweb09.html)
+ - [ClueWeb12](https://ir-datasets.com/clueweb12.html)
+ - [CLIRMatrix](https://ir-datasets.com/clirmatrix.html)
+ - [CodeSearchNet](https://ir-datasets.com/codesearchnet.html)
+ - [CORD-19](https://ir-datasets.com/cord19.html)
+ - [DPR Wiki100](https://ir-datasets.com/dpr-w100.html)
+ - [GOV](https://ir-datasets.com/gov.html)
+ - [GOV2](https://ir-datasets.com/gov2.html)
+ - [HC4](https://ir-datasets.com/hc4.html)
+ - [Highwire (TREC Genomics 2006-07)](https://ir-datasets.com/highwire.html)
+ - [Medline](https://ir-datasets.com/medline.html)
+ - [MSMARCO (document)](https://ir-datasets.com/msmarco-document.html)
+ - [MSMARCO (passage)](https://ir-datasets.com/msmarco-passage.html)
+ - [MSMARCO (QnA)](https://ir-datasets.com/msmarco-qna.html)
+ - [Natural Questions](https://ir-datasets.com/natural-questions.html)
+ - [NFCorpus (NutritionFacts)](https://ir-datasets.com/nfcorpus.html)
+ - [NYT](https://ir-datasets.com/nyt.html)
+ - [PubMed Central (TREC CDS)](https://ir-datasets.com/pmc.html)
+ - [TREC Arabic](https://ir-datasets.com/trec-arabic.html)
+ - [TREC Fair Ranking 2021](https://ir-datasets.com/trec-fair-2021.html)
+ - [TREC Mandarin](https://ir-datasets.com/trec-mandarin.html)
+ - [TREC Robust 2004](https://ir-datasets.com/trec-robust04.html)
+ - [TREC Spanish](https://ir-datasets.com/trec-spanish.html)
+ - [TripClick](https://ir-datasets.com/tripclick.html)
+ - [Tweets 2013 (Internet Archive)](https://ir-datasets.com/tweets2013-ia.html)
+ - [Vaswani](https://ir-datasets.com/vaswani.html)
+ - [Washington Post](https://ir-datasets.com/wapo.html)
+ - [WikIR](https://ir-datasets.com/wikir.html)
+
+There are "subsets" under each dataset. For instance, `clueweb12/b13/trec-misinfo-2019` provides the
+queries and judgments from the [2019 TREC misinformation track](https://trec.nist.gov/data/misinfo2019.html),
+and `msmarco-document/orcas` provides the [ORCAS dataset](https://microsoft.github.io/msmarco/ORCAS). They
+tend to be organized with the document collection at the top level.
+
+See the ir_dataets docs ([ir_datasets.com](https://ir-datasets.com/)) for details about each
+dataset, its available subsets, and what data they provide.
+
+## Environment variables
+
+ - `IR_DATASETS_HOME`: Home directory for ir_datasets data (default `~/.ir_datasets/`). Contains directories
+   for each top-level dataset.
+ - `IR_DATASETS_TMP`: Temporary working directory (default `/tmp/ir_datasets/`).
+ - `IR_DATASETS_DL_TIMEOUT`: Download stream read timeout, in seconds (default `15`). If no data is received
+   within this duration, the connection will be assumed to be dead, and another download may be attempted.
+ - `IR_DATASETS_DL_TRIES`: Default number of download attempts before exception is thrown (default `3`).
+   When the server accepts Range requests, uses them. Otherwise, will download the entire file again
+ - `IR_DATASETS_DL_DISABLE_PBAR`: Set to `true` to disable the progress bar for downloads. Useful in settings
+   where an interactive console is not available.
+ - `IR_DATASETS_DL_SKIP_SSL`: Set to `true` to disable checking SSL certificates when downloading files.
+   Useful as a short-term solution when SSL certificates expire or are otherwise invalid. Note that this
+   does not disable hash verification of the downloaded content.
+ - `IR_DATASETS_SKIP_DISK_FREE`: Set to `true` to disable checks for enough free space on disk before
+   downloading content or otherwise creating large files.
+ - `IR_DATASETS_SMALL_FILE_SIZE`: The size of files that are considered "small", in bytes. Instructions for
+   linking small files rather then downloading them are not shown. Defaults to 5000000 (5MB).
+
+## Citing
+
+When using datasets provided by this package, be sure to properly cite them. Bibtex for each dataset
+can be found on the [datasets documentation page](https://ir-datasets.com/).
+
+If you use this tool, please cite [our SIGIR resource paper](https://arxiv.org/pdf/2103.02280.pdf):
+
+```
+@inproceedings{macavaney:sigir2021-irds,
+  author = {MacAvaney, Sean and Yates, Andrew and Feldman, Sergey and Downey, Doug and Cohan, Arman and Goharian, Nazli},
+  title = {Simplified Data Wrangling with ir_datasets},
+  year = {2021},
+  booktitle = {SIGIR}
+}
+```
+
+## Credits
+
+Contributors to this repository:
+
+ - Sean MacAvaney (University of Glasgow)
+ - Shuo Sun (Johns Hopkins University)
+ - Thomas Jänich (University of Glasgow)
+ - Jan Heinrich Reimer (Martin Luther University Halle-Wittenberg)
+ - Maik Fröbe (Martin Luther University Halle-Wittenberg)
+ - Eugene Yang (Johns Hopkins University)
+ - Augustin Godinot (NAVERLABS Europe, ENS Paris-Saclay)
```

### Comparing `ir_datasets-0.5.6/README.md` & `ir_datasets-0.5.7/README.md`

 * *Files identical despite different names*

### Comparing `ir_datasets-0.5.6/ir_datasets/__init__.py` & `ir_datasets-0.5.7/ir_datasets/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -97,8 +97,8 @@
     commands.COMMANDS[args[0]](args[1:])
 
 
 def main_cli():
     import sys
     main(sys.argv[1:])
 
-__version__ = "0.5.6" # NOTE: keep this in sync with setup.py
+__version__ = "0.5.7" # NOTE: keep this in sync with setup.py
```

### Comparing `ir_datasets-0.5.6/ir_datasets/commands/__init__.py` & `ir_datasets-0.5.7/ir_datasets/commands/__init__.py`

 * *Files identical despite different names*

### Comparing `ir_datasets-0.5.6/ir_datasets/commands/build_c4_checkpoints.py` & `ir_datasets-0.5.7/ir_datasets/commands/build_c4_checkpoints.py`

 * *Files identical despite different names*

### Comparing `ir_datasets-0.5.6/ir_datasets/commands/build_clueweb_warc_indexes.py` & `ir_datasets-0.5.7/ir_datasets/commands/build_clueweb_warc_indexes.py`

 * *Files identical despite different names*

### Comparing `ir_datasets-0.5.6/ir_datasets/commands/build_download_cache.py` & `ir_datasets-0.5.7/ir_datasets/commands/build_download_cache.py`

 * *Files identical despite different names*

### Comparing `ir_datasets-0.5.6/ir_datasets/commands/clean.py` & `ir_datasets-0.5.7/ir_datasets/commands/clean.py`

 * *Files identical despite different names*

### Comparing `ir_datasets-0.5.6/ir_datasets/commands/doc_fifos.py` & `ir_datasets-0.5.7/ir_datasets/commands/doc_fifos.py`

 * *Files identical despite different names*

### Comparing `ir_datasets-0.5.6/ir_datasets/commands/export.py` & `ir_datasets-0.5.7/ir_datasets/commands/export.py`

 * *Files identical despite different names*

### Comparing `ir_datasets-0.5.6/ir_datasets/commands/generate_metadata.py` & `ir_datasets-0.5.7/ir_datasets/commands/generate_metadata.py`

 * *Files identical despite different names*

### Comparing `ir_datasets-0.5.6/ir_datasets/commands/lookup.py` & `ir_datasets-0.5.7/ir_datasets/commands/lookup.py`

 * *Files identical despite different names*

### Comparing `ir_datasets-0.5.6/ir_datasets/datasets/__init__.py` & `ir_datasets-0.5.7/ir_datasets/datasets/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -9,14 +9,15 @@
 from . import clinicaltrials
 from . import clirmatrix
 from . import clueweb09
 from . import clueweb12
 from . import codec
 from . import cord19
 from . import cranfield
+from . import csl
 from . import disks45
 from . import dpr_w100
 from . import codesearchnet
 from . import gov
 from . import gov2
 from . import highwire
 from . import istella22
```

### Comparing `ir_datasets-0.5.6/ir_datasets/datasets/antique.py` & `ir_datasets-0.5.7/ir_datasets/datasets/antique.py`

 * *Files identical despite different names*

### Comparing `ir_datasets-0.5.6/ir_datasets/datasets/aol_ia.py` & `ir_datasets-0.5.7/ir_datasets/datasets/aol_ia.py`

 * *Files identical despite different names*

### Comparing `ir_datasets-0.5.6/ir_datasets/datasets/aquaint.py` & `ir_datasets-0.5.7/ir_datasets/datasets/aquaint.py`

 * *Files identical despite different names*

### Comparing `ir_datasets-0.5.6/ir_datasets/datasets/argsme.py` & `ir_datasets-0.5.7/ir_datasets/datasets/argsme.py`

 * *Files identical despite different names*

### Comparing `ir_datasets-0.5.6/ir_datasets/datasets/base.py` & `ir_datasets-0.5.7/ir_datasets/datasets/base.py`

 * *Files identical despite different names*

### Comparing `ir_datasets-0.5.6/ir_datasets/datasets/beir.py` & `ir_datasets-0.5.7/ir_datasets/datasets/beir.py`

 * *Files identical despite different names*

### Comparing `ir_datasets-0.5.6/ir_datasets/datasets/c4.py` & `ir_datasets-0.5.7/ir_datasets/datasets/c4.py`

 * *Files identical despite different names*

### Comparing `ir_datasets-0.5.6/ir_datasets/datasets/car.py` & `ir_datasets-0.5.7/ir_datasets/datasets/car.py`

 * *Files identical despite different names*

### Comparing `ir_datasets-0.5.6/ir_datasets/datasets/clinicaltrials.py` & `ir_datasets-0.5.7/ir_datasets/datasets/clinicaltrials.py`

 * *Files identical despite different names*

### Comparing `ir_datasets-0.5.6/ir_datasets/datasets/clirmatrix.py` & `ir_datasets-0.5.7/ir_datasets/datasets/clirmatrix.py`

 * *Files identical despite different names*

### Comparing `ir_datasets-0.5.6/ir_datasets/datasets/clueweb09.py` & `ir_datasets-0.5.7/ir_datasets/datasets/clueweb09.py`

 * *Files identical despite different names*

### Comparing `ir_datasets-0.5.6/ir_datasets/datasets/clueweb12.py` & `ir_datasets-0.5.7/ir_datasets/datasets/clueweb12.py`

 * *Files identical despite different names*

### Comparing `ir_datasets-0.5.6/ir_datasets/datasets/codec.py` & `ir_datasets-0.5.7/ir_datasets/datasets/codec.py`

 * *Files identical despite different names*

### Comparing `ir_datasets-0.5.6/ir_datasets/datasets/codesearchnet.py` & `ir_datasets-0.5.7/ir_datasets/datasets/codesearchnet.py`

 * *Files identical despite different names*

### Comparing `ir_datasets-0.5.6/ir_datasets/datasets/cord19.py` & `ir_datasets-0.5.7/ir_datasets/datasets/cord19.py`

 * *Files identical despite different names*

### Comparing `ir_datasets-0.5.6/ir_datasets/datasets/cranfield.py` & `ir_datasets-0.5.7/ir_datasets/datasets/cranfield.py`

 * *Files identical despite different names*

### Comparing `ir_datasets-0.5.6/ir_datasets/datasets/disks45.py` & `ir_datasets-0.5.7/ir_datasets/datasets/disks45.py`

 * *Files identical despite different names*

### Comparing `ir_datasets-0.5.6/ir_datasets/datasets/dpr_w100.py` & `ir_datasets-0.5.7/ir_datasets/datasets/dpr_w100.py`

 * *Files identical despite different names*

### Comparing `ir_datasets-0.5.6/ir_datasets/datasets/gov.py` & `ir_datasets-0.5.7/ir_datasets/datasets/gov.py`

 * *Files identical despite different names*

### Comparing `ir_datasets-0.5.6/ir_datasets/datasets/gov2.py` & `ir_datasets-0.5.7/ir_datasets/datasets/gov2.py`

 * *Files identical despite different names*

### Comparing `ir_datasets-0.5.6/ir_datasets/datasets/hc4.py` & `ir_datasets-0.5.7/ir_datasets/datasets/hc4.py`

 * *Files identical despite different names*

### Comparing `ir_datasets-0.5.6/ir_datasets/datasets/highwire.py` & `ir_datasets-0.5.7/ir_datasets/datasets/highwire.py`

 * *Files identical despite different names*

### Comparing `ir_datasets-0.5.6/ir_datasets/datasets/istella22.py` & `ir_datasets-0.5.7/ir_datasets/datasets/istella22.py`

 * *Files identical despite different names*

### Comparing `ir_datasets-0.5.6/ir_datasets/datasets/kilt.py` & `ir_datasets-0.5.7/ir_datasets/datasets/kilt.py`

 * *Files identical despite different names*

### Comparing `ir_datasets-0.5.6/ir_datasets/datasets/lotte.py` & `ir_datasets-0.5.7/ir_datasets/datasets/lotte.py`

 * *Files identical despite different names*

### Comparing `ir_datasets-0.5.6/ir_datasets/datasets/medline.py` & `ir_datasets-0.5.7/ir_datasets/datasets/medline.py`

 * *Files identical despite different names*

### Comparing `ir_datasets-0.5.6/ir_datasets/datasets/miracl.py` & `ir_datasets-0.5.7/ir_datasets/datasets/miracl.py`

 * *Files identical despite different names*

### Comparing `ir_datasets-0.5.6/ir_datasets/datasets/mmarco.py` & `ir_datasets-0.5.7/ir_datasets/datasets/mmarco.py`

 * *Files identical despite different names*

### Comparing `ir_datasets-0.5.6/ir_datasets/datasets/mr_tydi.py` & `ir_datasets-0.5.7/ir_datasets/datasets/mr_tydi.py`

 * *Files identical despite different names*

### Comparing `ir_datasets-0.5.6/ir_datasets/datasets/msmarco_document.py` & `ir_datasets-0.5.7/ir_datasets/datasets/msmarco_document.py`

 * *Files identical despite different names*

### Comparing `ir_datasets-0.5.6/ir_datasets/datasets/msmarco_document_v2.py` & `ir_datasets-0.5.7/ir_datasets/datasets/msmarco_document_v2.py`

 * *Files identical despite different names*

### Comparing `ir_datasets-0.5.6/ir_datasets/datasets/msmarco_passage.py` & `ir_datasets-0.5.7/ir_datasets/datasets/msmarco_passage.py`

 * *Files identical despite different names*

### Comparing `ir_datasets-0.5.6/ir_datasets/datasets/msmarco_passage_v2.py` & `ir_datasets-0.5.7/ir_datasets/datasets/msmarco_passage_v2.py`

 * *Files identical despite different names*

### Comparing `ir_datasets-0.5.6/ir_datasets/datasets/msmarco_qna.py` & `ir_datasets-0.5.7/ir_datasets/datasets/msmarco_qna.py`

 * *Files identical despite different names*

### Comparing `ir_datasets-0.5.6/ir_datasets/datasets/natural_questions.py` & `ir_datasets-0.5.7/ir_datasets/datasets/natural_questions.py`

 * *Files identical despite different names*

### Comparing `ir_datasets-0.5.6/ir_datasets/datasets/neuclir.py` & `ir_datasets-0.5.7/ir_datasets/datasets/neuclir.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 import gzip
 import json
 from functools import lru_cache
 
 import ir_datasets
-from ir_datasets.util import DownloadConfig
-from ir_datasets.datasets.base import Dataset, YamlDocumentation
+from ir_datasets.util import DownloadConfig, Lazy
+from ir_datasets.datasets.base import Dataset, YamlDocumentation, FilteredQueries
 from ir_datasets.formats.trec import TrecQrels
 
-from ir_datasets.formats import ExctractedCCDocs, ExctractedCCQueries
+from ir_datasets.formats import ExctractedCCDocs, ExctractedCCQueries, ExctractedCCNoReportQuery, ExctractedCCNoReportNoHtNarQuery, ExctractedCCMultiMtQuery
 
 from ir_datasets.datasets.hc4 import NAME as HC4_NAME
-from ir_datasets.util.fileio import GzipExtract
+from ir_datasets.util.fileio import GzipExtract, TarExtract
 
 NAME = 'neuclir'
 
 DOC_COUNTS = {
     'zh': 3179209,
     'fa': 2232016,
     'ru': 4627543
@@ -53,14 +53,25 @@
     def qrels_iter(self):
         include_doc_id = get_ids(self._include_doc_id_dlc)
         for qrel in super().qrels_iter():
             if qrel.doc_id in include_doc_id:
                 yield qrel
 
 
+class LangFilteredTrecQrels(TrecQrels):
+    def __init__(self, qrels_dlc, qrels_defs, lang, format_3col=False):
+        super().__init__(qrels_dlc, qrels_defs, format_3col)
+        self._lang = lang
+    
+    def qrels_iter(self):
+        for qrel in super().qrels_iter():
+            if qrel.iteration == self._lang:
+                yield qrel
+
+
 QREL_DEFS = {
     3: 'Very-valuable. Information in the document would be found in the lead paragraph of a report that is later written on the topic.',
     1: 'Somewhat-valuable. The most valuable information in the document would be found in the remainder of such a report.',
     0: 'Not-valuable. Information in the document might be included in a report footnote, or omitted entirely.',
 }
 
 def _init():
@@ -69,29 +80,65 @@
     dlc = DownloadConfig.context(NAME, base_path)
     hc4_dlc = DownloadConfig.context(HC4_NAME, ir_datasets.util.home_path()/HC4_NAME)
     documentation = YamlDocumentation(f'docs/{NAME}.yaml')
 
     base = Dataset(documentation('_')) # dummy top level ds
     subsets["1"] = Dataset(documentation('1')) # dummy year level ds
 
+    qrels2022 = dlc['trec-2022/qrels']
+    qrels2023 = TarExtract(dlc['trec-2023/qrels'], 'qrels.final')
+
     # For NeuCLIR Collection 1
     for lang in ['zh', 'fa', 'ru']:
-        lang_docs = ExctractedCCDocs(dlc[f'1/{lang}/docs'], subset_lang=lang, namespace=NAME, count=DOC_COUNTS[lang])
+        lang3 = {'fa': 'fas', 'zh': 'zho', 'ru': 'rus'}[lang]
+        lang_docs = ExctractedCCDocs(GzipExtract(dlc[f'1/{lang}/docs']), subset_lang=lang, namespace=NAME, count=DOC_COUNTS[lang])
         subsets[f"1/{lang}"] = Dataset(
             lang_docs,
             documentation(f"1/{lang}")
         )
+        qrels = LangFilteredTrecQrels(qrels2022, QREL_DEFS, lang3)
+        subsets[f"1/{lang}/trec-2022"] = Dataset(
+            lang_docs,
+            FilteredQueries(ExctractedCCQueries(dlc['trec-2022/queries'], subset_lang=lang, filter_lwq=False, cls=ExctractedCCNoReportQuery, namespace=NAME), _lazy_qids_set(qrels), mode='include'),
+            qrels,
+            documentation(f"1/{lang}/trec-2022"),
+        )
+        qrels = LangFilteredTrecQrels(qrels2023, QREL_DEFS, lang3)
+        subsets[f"1/{lang}/trec-2023"] = Dataset(
+            lang_docs,
+            FilteredQueries(ExctractedCCQueries(dlc['trec-2023/queries'], subset_lang=lang, filter_lwq=False, cls=ExctractedCCNoReportNoHtNarQuery, namespace=NAME), _lazy_qids_set(qrels), mode='include'),
+            qrels,
+            documentation(f"1/{lang}/trec-2023"),
+        )
         include_doc_id_dlc = hc4_dlc[f'{lang}/docs/ids'] if lang != 'ru' else tuple([ hc4_dlc[f'{lang}/docs/ids/{i}'] for i in range(8) ])
         subsets[f"1/{lang}/hc4-filtered"] = Dataset(
-            FilteredExctractedCCDocs(dlc[f'1/{lang}/docs'], subset_lang=lang, namespace=NAME, include_doc_id_dlc=include_doc_id_dlc),
-            ExctractedCCQueries([hc4_dlc[f'dev/topics'], hc4_dlc[f'test/topics']], subset_lang=lang, namespace=NAME),
+            FilteredExctractedCCDocs(GzipExtract(dlc[f'1/{lang}/docs']), subset_lang=lang, namespace=NAME, include_doc_id_dlc=include_doc_id_dlc),
+            ExctractedCCQueries([hc4_dlc['dev/topics'], hc4_dlc['test/topics']], subset_lang=lang, namespace=NAME),
             FilteredTrecQrels([ hc4_dlc[f'{lang}/dev/qrels'], hc4_dlc[f'{lang}/test/qrels'] ], QREL_DEFS, include_doc_id_dlc=include_doc_id_dlc),
             documentation(f"1/{lang}/hc4-filtered")
         )
-    
+
+    multi_docs = ExctractedCCDocs([GzipExtract(dlc[f'1/{lang}/docs']) for lang in ['zh', 'fa', 'ru']], namespace=NAME, count=sum(DOC_COUNTS.values()), docstore_path=base_path/'1'/'multi')
+    subsets['1/multi'] = Dataset(
+        multi_docs,
+        documentation("1/multi")
+    )
+
+    subsets['1/multi/trec-2023'] = Dataset(
+        multi_docs,
+        ExctractedCCQueries(dlc['trec-2023/queries'], filter_lwq=False, cls=ExctractedCCMultiMtQuery, namespace=NAME),
+        TrecQrels(qrels2023, QREL_DEFS),
+        documentation("1/multi/trec-2023")
+    )
+
     ir_datasets.registry.register(NAME, base)
     for s in sorted(subsets):
         ir_datasets.registry.register(f'{NAME}/{s}', subsets[s])
 
     return base, subsets
 
+
+def _lazy_qids_set(qrels):
+    return Lazy(lambda: {qrel.query_id for qrel in qrels.qrels_iter()})
+
+
 base, subsets = _init()
```

### Comparing `ir_datasets-0.5.6/ir_datasets/datasets/neumarco.py` & `ir_datasets-0.5.7/ir_datasets/datasets/neumarco.py`

 * *Files identical despite different names*

### Comparing `ir_datasets-0.5.6/ir_datasets/datasets/nfcorpus.py` & `ir_datasets-0.5.7/ir_datasets/datasets/nfcorpus.py`

 * *Files identical despite different names*

### Comparing `ir_datasets-0.5.6/ir_datasets/datasets/nyt.py` & `ir_datasets-0.5.7/ir_datasets/datasets/nyt.py`

 * *Files identical despite different names*

### Comparing `ir_datasets-0.5.6/ir_datasets/datasets/pmc.py` & `ir_datasets-0.5.7/ir_datasets/datasets/pmc.py`

 * *Files identical despite different names*

### Comparing `ir_datasets-0.5.6/ir_datasets/datasets/sara.py` & `ir_datasets-0.5.7/ir_datasets/datasets/sara.py`

 * *Files identical despite different names*

### Comparing `ir_datasets-0.5.6/ir_datasets/datasets/touche.py` & `ir_datasets-0.5.7/ir_datasets/datasets/touche.py`

 * *Files identical despite different names*

### Comparing `ir_datasets-0.5.6/ir_datasets/datasets/touche_image.py` & `ir_datasets-0.5.7/ir_datasets/datasets/touche_image.py`

 * *Files identical despite different names*

### Comparing `ir_datasets-0.5.6/ir_datasets/datasets/trec_arabic.py` & `ir_datasets-0.5.7/ir_datasets/datasets/trec_arabic.py`

 * *Files identical despite different names*

### Comparing `ir_datasets-0.5.6/ir_datasets/datasets/trec_cast.py` & `ir_datasets-0.5.7/ir_datasets/datasets/trec_cast.py`

 * *Files identical despite different names*

### Comparing `ir_datasets-0.5.6/ir_datasets/datasets/trec_fair.py` & `ir_datasets-0.5.7/ir_datasets/datasets/trec_fair.py`

 * *Files identical despite different names*

### Comparing `ir_datasets-0.5.6/ir_datasets/datasets/trec_mandarin.py` & `ir_datasets-0.5.7/ir_datasets/datasets/trec_mandarin.py`

 * *Files identical despite different names*

### Comparing `ir_datasets-0.5.6/ir_datasets/datasets/trec_robust04.py` & `ir_datasets-0.5.7/ir_datasets/datasets/trec_robust04.py`

 * *Files identical despite different names*

### Comparing `ir_datasets-0.5.6/ir_datasets/datasets/trec_spanish.py` & `ir_datasets-0.5.7/ir_datasets/datasets/trec_spanish.py`

 * *Files identical despite different names*

### Comparing `ir_datasets-0.5.6/ir_datasets/datasets/trec_tot.py` & `ir_datasets-0.5.7/ir_datasets/datasets/trec_tot.py`

 * *Files identical despite different names*

### Comparing `ir_datasets-0.5.6/ir_datasets/datasets/tripclick.py` & `ir_datasets-0.5.7/ir_datasets/datasets/tripclick.py`

 * *Files identical despite different names*

### Comparing `ir_datasets-0.5.6/ir_datasets/datasets/tweets2013_ia.py` & `ir_datasets-0.5.7/ir_datasets/datasets/tweets2013_ia.py`

 * *Files identical despite different names*

### Comparing `ir_datasets-0.5.6/ir_datasets/datasets/vaswani.py` & `ir_datasets-0.5.7/ir_datasets/datasets/vaswani.py`

 * *Files identical despite different names*

### Comparing `ir_datasets-0.5.6/ir_datasets/datasets/wapo.py` & `ir_datasets-0.5.7/ir_datasets/datasets/wapo.py`

 * *Files identical despite different names*

### Comparing `ir_datasets-0.5.6/ir_datasets/datasets/wikiclir.py` & `ir_datasets-0.5.7/ir_datasets/datasets/wikiclir.py`

 * *Files identical despite different names*

### Comparing `ir_datasets-0.5.6/ir_datasets/datasets/wikir.py` & `ir_datasets-0.5.7/ir_datasets/datasets/wikir.py`

 * *Files identical despite different names*

### Comparing `ir_datasets-0.5.6/ir_datasets/docs/antique.yaml` & `ir_datasets-0.5.7/ir_datasets/docs/antique.yaml`

 * *Files identical despite different names*

### Comparing `ir_datasets-0.5.6/ir_datasets/docs/aol-ia.yaml` & `ir_datasets-0.5.7/ir_datasets/docs/aol-ia.yaml`

 * *Files identical despite different names*

### Comparing `ir_datasets-0.5.6/ir_datasets/docs/aquaint.yaml` & `ir_datasets-0.5.7/ir_datasets/docs/aquaint.yaml`

 * *Files identical despite different names*

### Comparing `ir_datasets-0.5.6/ir_datasets/docs/argsme.yaml` & `ir_datasets-0.5.7/ir_datasets/docs/argsme.yaml`

 * *Files identical despite different names*

### Comparing `ir_datasets-0.5.6/ir_datasets/docs/beir.yaml` & `ir_datasets-0.5.7/ir_datasets/docs/beir.yaml`

 * *Files identical despite different names*

### Comparing `ir_datasets-0.5.6/ir_datasets/docs/bibliography.bib` & `ir_datasets-0.5.7/ir_datasets/docs/bibliography.bib`

 * *Files identical despite different names*

### Comparing `ir_datasets-0.5.6/ir_datasets/docs/c4.yaml` & `ir_datasets-0.5.7/ir_datasets/docs/c4.yaml`

 * *Files identical despite different names*

### Comparing `ir_datasets-0.5.6/ir_datasets/docs/car.yaml` & `ir_datasets-0.5.7/ir_datasets/docs/car.yaml`

 * *Files identical despite different names*

### Comparing `ir_datasets-0.5.6/ir_datasets/docs/clinicaltrials.yaml` & `ir_datasets-0.5.7/ir_datasets/docs/clinicaltrials.yaml`

 * *Files identical despite different names*

### Comparing `ir_datasets-0.5.6/ir_datasets/docs/clirmatrix.yaml` & `ir_datasets-0.5.7/ir_datasets/docs/clirmatrix.yaml`

 * *Files identical despite different names*

### Comparing `ir_datasets-0.5.6/ir_datasets/docs/clueweb09.yaml` & `ir_datasets-0.5.7/ir_datasets/docs/clueweb09.yaml`

 * *Files identical despite different names*

### Comparing `ir_datasets-0.5.6/ir_datasets/docs/clueweb12.yaml` & `ir_datasets-0.5.7/ir_datasets/docs/clueweb12.yaml`

 * *Files identical despite different names*

### Comparing `ir_datasets-0.5.6/ir_datasets/docs/codec.yaml` & `ir_datasets-0.5.7/ir_datasets/docs/codec.yaml`

 * *Files identical despite different names*

### Comparing `ir_datasets-0.5.6/ir_datasets/docs/codesearchnet.yaml` & `ir_datasets-0.5.7/ir_datasets/docs/codesearchnet.yaml`

 * *Files identical despite different names*

### Comparing `ir_datasets-0.5.6/ir_datasets/docs/cord19.yaml` & `ir_datasets-0.5.7/ir_datasets/docs/cord19.yaml`

 * *Files identical despite different names*

### Comparing `ir_datasets-0.5.6/ir_datasets/docs/disks45.yaml` & `ir_datasets-0.5.7/ir_datasets/docs/disks45.yaml`

 * *Files identical despite different names*

### Comparing `ir_datasets-0.5.6/ir_datasets/docs/dpr-w100.yaml` & `ir_datasets-0.5.7/ir_datasets/docs/dpr-w100.yaml`

 * *Files identical despite different names*

### Comparing `ir_datasets-0.5.6/ir_datasets/docs/gov.yaml` & `ir_datasets-0.5.7/ir_datasets/docs/gov.yaml`

 * *Files identical despite different names*

### Comparing `ir_datasets-0.5.6/ir_datasets/docs/gov2.yaml` & `ir_datasets-0.5.7/ir_datasets/docs/gov2.yaml`

 * *Files identical despite different names*

### Comparing `ir_datasets-0.5.6/ir_datasets/docs/hc4.yaml` & `ir_datasets-0.5.7/ir_datasets/docs/hc4.yaml`

 * *Files identical despite different names*

### Comparing `ir_datasets-0.5.6/ir_datasets/docs/highwire.yaml` & `ir_datasets-0.5.7/ir_datasets/docs/highwire.yaml`

 * *Files identical despite different names*

### Comparing `ir_datasets-0.5.6/ir_datasets/docs/istella22.yaml` & `ir_datasets-0.5.7/ir_datasets/docs/istella22.yaml`

 * *Files identical despite different names*

### Comparing `ir_datasets-0.5.6/ir_datasets/docs/kilt.yaml` & `ir_datasets-0.5.7/ir_datasets/docs/kilt.yaml`

 * *Files identical despite different names*

### Comparing `ir_datasets-0.5.6/ir_datasets/docs/lotte.yaml` & `ir_datasets-0.5.7/ir_datasets/docs/lotte.yaml`

 * *Files identical despite different names*

### Comparing `ir_datasets-0.5.6/ir_datasets/docs/medline.yaml` & `ir_datasets-0.5.7/ir_datasets/docs/medline.yaml`

 * *Files identical despite different names*

### Comparing `ir_datasets-0.5.6/ir_datasets/docs/miracl.yaml` & `ir_datasets-0.5.7/ir_datasets/docs/miracl.yaml`

 * *Files identical despite different names*

### Comparing `ir_datasets-0.5.6/ir_datasets/docs/mmarco.yaml` & `ir_datasets-0.5.7/ir_datasets/docs/mmarco.yaml`

 * *Files identical despite different names*

### Comparing `ir_datasets-0.5.6/ir_datasets/docs/mr-tydi.yaml` & `ir_datasets-0.5.7/ir_datasets/docs/mr-tydi.yaml`

 * *Files identical despite different names*

### Comparing `ir_datasets-0.5.6/ir_datasets/docs/msmarco-document-v2.yaml` & `ir_datasets-0.5.7/ir_datasets/docs/msmarco-document-v2.yaml`

 * *Files identical despite different names*

### Comparing `ir_datasets-0.5.6/ir_datasets/docs/msmarco-document.yaml` & `ir_datasets-0.5.7/ir_datasets/docs/msmarco-document.yaml`

 * *Files identical despite different names*

### Comparing `ir_datasets-0.5.6/ir_datasets/docs/msmarco-passage-v2.yaml` & `ir_datasets-0.5.7/ir_datasets/docs/msmarco-passage-v2.yaml`

 * *Files identical despite different names*

### Comparing `ir_datasets-0.5.6/ir_datasets/docs/msmarco-passage.yaml` & `ir_datasets-0.5.7/ir_datasets/docs/msmarco-passage.yaml`

 * *Files identical despite different names*

### Comparing `ir_datasets-0.5.6/ir_datasets/docs/msmarco-qna.yaml` & `ir_datasets-0.5.7/ir_datasets/docs/msmarco-qna.yaml`

 * *Files identical despite different names*

### Comparing `ir_datasets-0.5.6/ir_datasets/docs/natural-questions.yaml` & `ir_datasets-0.5.7/ir_datasets/docs/natural-questions.yaml`

 * *Files identical despite different names*

### Comparing `ir_datasets-0.5.6/ir_datasets/docs/neumarco.yaml` & `ir_datasets-0.5.7/ir_datasets/docs/neumarco.yaml`

 * *Files identical despite different names*

### Comparing `ir_datasets-0.5.6/ir_datasets/docs/nfcorpus.yaml` & `ir_datasets-0.5.7/ir_datasets/docs/nfcorpus.yaml`

 * *Files identical despite different names*

### Comparing `ir_datasets-0.5.6/ir_datasets/docs/nyt.yaml` & `ir_datasets-0.5.7/ir_datasets/docs/nyt.yaml`

 * *Files identical despite different names*

### Comparing `ir_datasets-0.5.6/ir_datasets/docs/pmc.yaml` & `ir_datasets-0.5.7/ir_datasets/docs/pmc.yaml`

 * *Files identical despite different names*

### Comparing `ir_datasets-0.5.6/ir_datasets/docs/touche-image.yaml` & `ir_datasets-0.5.7/ir_datasets/docs/touche-image.yaml`

 * *Files identical despite different names*

### Comparing `ir_datasets-0.5.6/ir_datasets/docs/touche.yaml` & `ir_datasets-0.5.7/ir_datasets/docs/touche.yaml`

 * *Files identical despite different names*

### Comparing `ir_datasets-0.5.6/ir_datasets/docs/trec-arabic.yaml` & `ir_datasets-0.5.7/ir_datasets/docs/trec-arabic.yaml`

 * *Files identical despite different names*

### Comparing `ir_datasets-0.5.6/ir_datasets/docs/trec-cast.yaml` & `ir_datasets-0.5.7/ir_datasets/docs/trec-cast.yaml`

 * *Files identical despite different names*

### Comparing `ir_datasets-0.5.6/ir_datasets/docs/trec-fair.yaml` & `ir_datasets-0.5.7/ir_datasets/docs/trec-fair.yaml`

 * *Files identical despite different names*

### Comparing `ir_datasets-0.5.6/ir_datasets/docs/trec-mandarin.yaml` & `ir_datasets-0.5.7/ir_datasets/docs/trec-mandarin.yaml`

 * *Files identical despite different names*

### Comparing `ir_datasets-0.5.6/ir_datasets/docs/trec-robust04.yaml` & `ir_datasets-0.5.7/ir_datasets/docs/trec-robust04.yaml`

 * *Files identical despite different names*

### Comparing `ir_datasets-0.5.6/ir_datasets/docs/trec-spanish.yaml` & `ir_datasets-0.5.7/ir_datasets/docs/trec-spanish.yaml`

 * *Files identical despite different names*

### Comparing `ir_datasets-0.5.6/ir_datasets/docs/trec-tot.yaml` & `ir_datasets-0.5.7/ir_datasets/docs/trec-tot.yaml`

 * *Files identical despite different names*

### Comparing `ir_datasets-0.5.6/ir_datasets/docs/tripclick.yaml` & `ir_datasets-0.5.7/ir_datasets/docs/tripclick.yaml`

 * *Files identical despite different names*

### Comparing `ir_datasets-0.5.6/ir_datasets/docs/tweets2013-ia.yaml` & `ir_datasets-0.5.7/ir_datasets/docs/tweets2013-ia.yaml`

 * *Files identical despite different names*

### Comparing `ir_datasets-0.5.6/ir_datasets/docs/wapo.yaml` & `ir_datasets-0.5.7/ir_datasets/docs/wapo.yaml`

 * *Files identical despite different names*

### Comparing `ir_datasets-0.5.6/ir_datasets/docs/wikiclir.yaml` & `ir_datasets-0.5.7/ir_datasets/docs/wikiclir.yaml`

 * *Files identical despite different names*

### Comparing `ir_datasets-0.5.6/ir_datasets/docs/wikir.yaml` & `ir_datasets-0.5.7/ir_datasets/docs/wikir.yaml`

 * *Files identical despite different names*

### Comparing `ir_datasets-0.5.6/ir_datasets/etc/downloads.json` & `ir_datasets-0.5.7/ir_datasets/etc/downloads.json`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9753188775510203%*

 * *Differences: {"'csl'": "OrderedDict([('docs', OrderedDict([('url', "*

 * *          "'https://huggingface.co/datasets/neuclir/csl/resolve/main/data/csl.jsonl.gz?download=true'), "*

 * *          "('size_hint', 115749077), ('expected_md5', '4198f7b442187320e2351b3b473c1883'), "*

 * *          "('cache_path', 'docs.jsonl.gz')])), ('trec-2023/queries', OrderedDict([('url', "*

 * *          "'https://trec.nist.gov/data/neuclir/2023/neuclir-2023-technical_topics.0719.jsonl'), "*

 * *          "('size_hint', 86519), ('expected_md5', '0dd5ba173c695362 […]*

```diff
@@ -860,14 +860,36 @@
         "main": {
             "cache_path": "cran.tar.gz",
             "expected_md5": "1730f7be572d95a5a4b56c59a7b900a5",
             "size_hint": 506960,
             "url": "http://ir.dcs.gla.ac.uk/resources/test_collections/cran/cran.tar.gz"
         }
     },
+    "csl": {
+        "docs": {
+            "cache_path": "docs.jsonl.gz",
+            "expected_md5": "4198f7b442187320e2351b3b473c1883",
+            "size_hint": 115749077,
+            "url": "https://huggingface.co/datasets/neuclir/csl/resolve/main/data/csl.jsonl.gz?download=true"
+        },
+        "trec-2023/qrels": {
+            "cache_path": "trec-2023/qrels.tar.gz",
+            "expected_md5": "cea4ff3d9eba612c7119e6490217d4e1",
+            "irds_mirror": true,
+            "size_hint": 6023886,
+            "url": "https://trec.nist.gov/data/neuclir/2023/neuclir-2023-qrels.final.tar.gz"
+        },
+        "trec-2023/queries": {
+            "cache_path": "trec-2023/topics.jsonl",
+            "expected_md5": "0dd5ba173c695362a8705056edca481b",
+            "irds_mirror": true,
+            "size_hint": 86519,
+            "url": "https://trec.nist.gov/data/neuclir/2023/neuclir-2023-technical_topics.0719.jsonl"
+        }
+    },
     "disks45": {
         "docs": {
             "cache_path": "corpus",
             "instructions": "The TREC Robust document collection is from TREC disks 4 and 5. Due to the copyrighted nature of the  documents, this collection is for research use only, which requires agreements to be filed with NIST. See details here: <https://trec.nist.gov/data/cd45/index.html>.\nMore details about the procedure can be found here: <https://ir-datasets.com/trec-robust04.html#DataAccess>.\nOnce completed, place the uncompressed source here: {path}\nThis should contain directories like NEWS_data/FBIS, NEWS_data/FR94, etc."
         },
         "robust04-qrels": {
             "cache_path": "qrels.robust2004.txt",
@@ -5284,24 +5306,58 @@
             "skip_local": true,
             "stream": true,
             "url": "https://storage.googleapis.com/natural_questions/v1.0/train/nq-train-49.jsonl.gz"
         }
     },
     "neuclir": {
         "1/fa/docs": {
-            "cache_path": "1/fas/docs.jsonl",
-            "instructions": "To use this dataset, you need to download the document files using the HC4 document download the post-processing script here: <https://github.com/NeuCLIR/download-collection>.\nTo proceed, symlink the source file here: {path}"
+            "cache_path": "1/fas/docs.jsonl.gz",
+            "expected_md5": "c88f79f6b6da974db22cef3dd73fcee1",
+            "size_hint": 2359094118,
+            "url": "https://huggingface.co/datasets/neuclir/neuclir1/resolve/main/data/fas-00000-of-00001.jsonl.gz?download=true"
         },
         "1/ru/docs": {
-            "cache_path": "1/rus/docs.jsonl",
-            "instructions": "To use this dataset, you need to download the document files using the HC4 document download the post-processing script here: <https://github.com/NeuCLIR/download-collection>.\nTo proceed, symlink the source file here: {path}"
+            "cache_path": "1/rus/docs.jsonl.gz",
+            "expected_md5": "3aabc798a3b5dd92d7c47db9521870b1",
+            "size_hint": 4504119267,
+            "url": "https://huggingface.co/datasets/neuclir/neuclir1/resolve/main/data/rus-00000-of-00001.jsonl.gz?download=true"
         },
         "1/zh/docs": {
-            "cache_path": "1/zho/docs.jsonl",
-            "instructions": "To use this dataset, you need to download the document files using the HC4 document download the post-processing script here: <https://github.com/NeuCLIR/download-collection>.\nTo proceed, symlink the source file here: {path}"
+            "cache_path": "1/zho/docs.jsonl.gz",
+            "expected_md5": "99eb400f3a474603d1db5d41f606889b",
+            "size_hint": 3188072408,
+            "url": "https://huggingface.co/datasets/neuclir/neuclir1/resolve/main/data/zho-00000-of-00001.jsonl.gz?download=true"
+        },
+        "trec-2022/qrels": {
+            "cache_path": "trec-2022/qrels",
+            "expected_md5": "8dc1aecf13fbe358eea74ade7496b085",
+            "irds_mirror": true,
+            "size_hint": 4785668,
+            "url": "https://trec.nist.gov/data/neuclir/2022/2022-qrels.all"
+        },
+        "trec-2022/queries": {
+            "cache_path": "trec-2022/topics.jsonl",
+            "expected_md5": "264bf244f798670f063f32ff57ba6135",
+            "irds_mirror": true,
+            "size_hint": 662272,
+            "url": "https://trec.nist.gov/data/neuclir/2022/topics.0720.utf8.jsonl"
+        },
+        "trec-2023/qrels": {
+            "cache_path": "trec-2023/qrels.tar.gz",
+            "expected_md5": "cea4ff3d9eba612c7119e6490217d4e1",
+            "irds_mirror": true,
+            "size_hint": 6023886,
+            "url": "https://trec.nist.gov/data/neuclir/2023/neuclir-2023-qrels.final.tar.gz"
+        },
+        "trec-2023/queries": {
+            "cache_path": "trec-2023/topics.jsonl",
+            "expected_md5": "3dbb41b02bfbd719d8b55632d9b15b83",
+            "irds_mirror": true,
+            "size_hint": 683779,
+            "url": "https://trec.nist.gov/data/neuclir/2023/neuclir-2023-topics.0605.jsonl"
         }
     },
     "neumarco": {
         "main": {
             "cache_path": "neuMSMARCO.tar.gz",
             "expected_md5": "733181c211959a7c09c695bfcddaea54",
             "size_hint": 3723728998,
```

### Comparing `ir_datasets-0.5.6/ir_datasets/etc/metadata.json` & `ir_datasets-0.5.7/ir_datasets/etc/metadata.json`

 * *Files 1% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9865591397849462%*

 * *Differences: {"'csl'": "OrderedDict([('docs', OrderedDict([('count', 395927), ('fields', "*

 * *          "OrderedDict([('doc_id', OrderedDict([('max_len', 10), ('common_prefix', "*

 * *          "'csl-')]))]))]))])",*

 * * "'csl/trec-2023'": "OrderedDict([('docs', OrderedDict([('_ref', 'csl')])), ('queries', "*

 * *                    "OrderedDict([('count', 41)])), ('qrels', OrderedDict([('count', 11291), "*

 * *                    "('fields', OrderedDict([('relevance', OrderedDict([('counts_by_value', "*

 * *                    "OrderedDict([('0' […]*

```diff
@@ -2959,14 +2959,45 @@
                 }
             }
         },
         "queries": {
             "count": 225
         }
     },
+    "csl": {
+        "docs": {
+            "count": 395927,
+            "fields": {
+                "doc_id": {
+                    "common_prefix": "csl-",
+                    "max_len": 10
+                }
+            }
+        }
+    },
+    "csl/trec-2023": {
+        "docs": {
+            "_ref": "csl"
+        },
+        "qrels": {
+            "count": 11291,
+            "fields": {
+                "relevance": {
+                    "counts_by_value": {
+                        "0": 10644,
+                        "1": 419,
+                        "3": 228
+                    }
+                }
+            }
+        },
+        "queries": {
+            "count": 41
+        }
+    },
     "disks45": {},
     "disks45/nocr": {
         "docs": {
             "count": 528155,
             "fields": {
                 "doc_id": {
                     "common_prefix": "",
@@ -9523,14 +9554,87 @@
                 }
             }
         },
         "queries": {
             "count": 60
         }
     },
+    "neuclir/1/fa/trec-2022": {
+        "docs": {
+            "_ref": "neuclir/1/fa"
+        },
+        "qrels": {
+            "count": 34174,
+            "fields": {
+                "relevance": {
+                    "counts_by_value": {
+                        "0": 32702,
+                        "1": 602,
+                        "3": 870
+                    }
+                }
+            }
+        },
+        "queries": {
+            "count": 46
+        }
+    },
+    "neuclir/1/fa/trec-2023": {
+        "docs": {
+            "_ref": "neuclir/1/fa"
+        },
+        "qrels": {
+            "count": 26662,
+            "fields": {
+                "relevance": {
+                    "counts_by_value": {
+                        "0": 21624,
+                        "1": 2491,
+                        "2": 2068,
+                        "3": 479
+                    }
+                }
+            }
+        },
+        "queries": {
+            "count": 76
+        }
+    },
+    "neuclir/1/multi": {
+        "docs": {
+            "count": 10038768,
+            "fields": {
+                "doc_id": {
+                    "common_prefix": "",
+                    "max_len": 36
+                }
+            }
+        }
+    },
+    "neuclir/1/multi/trec-2023": {
+        "docs": {
+            "_ref": "neuclir/1/multi"
+        },
+        "qrels": {
+            "count": 79934,
+            "fields": {
+                "relevance": {
+                    "counts_by_value": {
+                        "0": 66087,
+                        "1": 6041,
+                        "2": 7171,
+                        "3": 635
+                    }
+                }
+            }
+        },
+        "queries": {
+            "count": 76
+        }
+    },
     "neuclir/1/ru": {
         "docs": {
             "count": 4627543,
             "fields": {
                 "doc_id": {
                     "common_prefix": "",
                     "max_len": 36
@@ -9560,14 +9664,55 @@
                 }
             }
         },
         "queries": {
             "count": 54
         }
     },
+    "neuclir/1/ru/trec-2022": {
+        "docs": {
+            "_ref": "neuclir/1/ru"
+        },
+        "qrels": {
+            "count": 33006,
+            "fields": {
+                "relevance": {
+                    "counts_by_value": {
+                        "0": 31117,
+                        "1": 1079,
+                        "3": 810
+                    }
+                }
+            }
+        },
+        "queries": {
+            "count": 45
+        }
+    },
+    "neuclir/1/ru/trec-2023": {
+        "docs": {
+            "_ref": "neuclir/1/ru"
+        },
+        "qrels": {
+            "count": 25634,
+            "fields": {
+                "relevance": {
+                    "counts_by_value": {
+                        "0": 20905,
+                        "1": 1422,
+                        "2": 3190,
+                        "3": 117
+                    }
+                }
+            }
+        },
+        "queries": {
+            "count": 76
+        }
+    },
     "neuclir/1/zh": {
         "docs": {
             "count": 3179209,
             "fields": {
                 "doc_id": {
                     "common_prefix": "",
                     "max_len": 36
@@ -9597,14 +9742,55 @@
                 }
             }
         },
         "queries": {
             "count": 60
         }
     },
+    "neuclir/1/zh/trec-2022": {
+        "docs": {
+            "_ref": "neuclir/1/zh"
+        },
+        "qrels": {
+            "count": 36575,
+            "fields": {
+                "relevance": {
+                    "counts_by_value": {
+                        "0": 34442,
+                        "1": 1413,
+                        "3": 720
+                    }
+                }
+            }
+        },
+        "queries": {
+            "count": 49
+        }
+    },
+    "neuclir/1/zh/trec-2023": {
+        "docs": {
+            "_ref": "neuclir/1/zh"
+        },
+        "qrels": {
+            "count": 27638,
+            "fields": {
+                "relevance": {
+                    "counts_by_value": {
+                        "0": 23558,
+                        "1": 2128,
+                        "2": 1913,
+                        "3": 39
+                    }
+                }
+            }
+        },
+        "queries": {
+            "count": 76
+        }
+    },
     "neumarco": {},
     "neumarco/fa": {
         "docs": {
             "count": 8841823,
             "fields": {
                 "doc_id": {
                     "common_prefix": "",
```

### Comparing `ir_datasets-0.5.6/ir_datasets/formats/__init__.py` & `ir_datasets-0.5.7/ir_datasets/formats/__init__.py`

 * *Files 5% similar despite different names*

```diff
@@ -5,9 +5,9 @@
 from .trec import TrecDocs, TrecQueries, TrecXmlQueries, TrecColonQueries, TrecQrels, TrecSubQrels, TrecPrels, TrecScoredDocs, TrecDoc, TitleUrlTextDoc, TrecQuery, TrecSubtopic, TrecQrel, TrecSubQrel, TrecPrel, TrecParsedDoc
 from .touche import ToucheQuery, ToucheTitleQuery, ToucheComparativeQuery, ToucheQualityQrel, ToucheQualityCoherenceQrel, ToucheComparativeStance, ToucheQualityComparativeStanceQrel, ToucheControversialStance, ToucheControversialStanceQrel, TouchePassageDoc, ToucheQueries, ToucheTitleQueries, ToucheComparativeQueries, ToucheQrels, ToucheQualityQrels, ToucheQualityCoherenceQrels, ToucheQualityComparativeStanceQrels, ToucheControversialStanceQrels, TouchePassageDocs
 from .touche_image import ToucheImageRanking, ToucheImageNode, ToucheImagePage, ToucheImageDoc, ToucheImageDocs
 from .webarc import WarcDocs, WarcDoc
 from .ntcir import NtcirQrels
 from .clirmatrix import CLIRMatrixQueries, CLIRMatrixQrels
 from .argsme import ArgsMeStance, ArgsMeMode, ArgsMeSourceDomain, ArgsMePremiseAnnotation, ArgsMePremise, ArgsMeAspect, ArgsMeDoc, ArgsMeProcessedDoc, ArgsMeDocs, ArgsMeProcessedDocs, ArgsMeCombinedDocs
-from .extracted_cc import ExctractedCCDoc, ExctractedCCDocs, ExctractedCCQuery, ExctractedCCQueries
+from .extracted_cc import ExctractedCCDoc, ExctractedCCDocs, ExctractedCCQuery, ExctractedCCQueries, ExctractedCCNoReportQuery, ExctractedCCNoReportNoHtNarQuery, ExctractedCCMultiMtQuery
 from .jsonl import JsonlDocs, JsonlQueries
```

### Comparing `ir_datasets-0.5.6/ir_datasets/formats/argsme.py` & `ir_datasets-0.5.7/ir_datasets/formats/argsme.py`

 * *Files identical despite different names*

### Comparing `ir_datasets-0.5.6/ir_datasets/formats/base.py` & `ir_datasets-0.5.7/ir_datasets/formats/base.py`

 * *Files identical despite different names*

### Comparing `ir_datasets-0.5.6/ir_datasets/formats/clirmatrix.py` & `ir_datasets-0.5.7/ir_datasets/formats/clirmatrix.py`

 * *Files identical despite different names*

### Comparing `ir_datasets-0.5.6/ir_datasets/formats/csv_fmt.py` & `ir_datasets-0.5.7/ir_datasets/formats/csv_fmt.py`

 * *Files identical despite different names*

### Comparing `ir_datasets-0.5.6/ir_datasets/formats/jsonl.py` & `ir_datasets-0.5.7/ir_datasets/formats/jsonl.py`

 * *Files identical despite different names*

### Comparing `ir_datasets-0.5.6/ir_datasets/formats/ntcir.py` & `ir_datasets-0.5.7/ir_datasets/formats/ntcir.py`

 * *Files identical despite different names*

### Comparing `ir_datasets-0.5.6/ir_datasets/formats/touche.py` & `ir_datasets-0.5.7/ir_datasets/formats/touche.py`

 * *Files identical despite different names*

### Comparing `ir_datasets-0.5.6/ir_datasets/formats/touche_image.py` & `ir_datasets-0.5.7/ir_datasets/formats/touche_image.py`

 * *Files identical despite different names*

### Comparing `ir_datasets-0.5.6/ir_datasets/formats/trec.py` & `ir_datasets-0.5.7/ir_datasets/formats/trec.py`

 * *Files identical despite different names*

### Comparing `ir_datasets-0.5.6/ir_datasets/formats/tsv.py` & `ir_datasets-0.5.7/ir_datasets/formats/tsv.py`

 * *Files 0% similar despite different names*

```diff
@@ -22,14 +22,15 @@
             self.ctxt.close()
             raise StopIteration
         if self.stream is None:
             if isinstance(self.dlc, list):
                 self.stream = io.TextIOWrapper(self.ctxt.enter_context(self.dlc[self.stream_idx].stream()))
             else:
                 self.stream = io.TextIOWrapper(self.ctxt.enter_context(self.dlc.stream()))
+        line = ''
         while self.pos < self.start:
             line = self.stream.readline()
             if line != '\n':
                 self.pos += 1
         if line == '':
             if isinstance(self.dlc, list):
                 self.stream_idx += 1
```

### Comparing `ir_datasets-0.5.6/ir_datasets/formats/webarc.py` & `ir_datasets-0.5.7/ir_datasets/formats/webarc.py`

 * *Files identical despite different names*

### Comparing `ir_datasets-0.5.6/ir_datasets/indices/base.py` & `ir_datasets-0.5.7/ir_datasets/indices/base.py`

 * *Files identical despite different names*

### Comparing `ir_datasets-0.5.6/ir_datasets/indices/cache_docstore.py` & `ir_datasets-0.5.7/ir_datasets/indices/cache_docstore.py`

 * *Files identical despite different names*

### Comparing `ir_datasets-0.5.6/ir_datasets/indices/clueweb_warc.py` & `ir_datasets-0.5.7/ir_datasets/indices/clueweb_warc.py`

 * *Files identical despite different names*

### Comparing `ir_datasets-0.5.6/ir_datasets/indices/indexed_tsv_docstore.py` & `ir_datasets-0.5.7/ir_datasets/indices/indexed_tsv_docstore.py`

 * *Files identical despite different names*

### Comparing `ir_datasets-0.5.6/ir_datasets/indices/lz4_pickle.py` & `ir_datasets-0.5.7/ir_datasets/indices/lz4_pickle.py`

 * *Files identical despite different names*

### Comparing `ir_datasets-0.5.6/ir_datasets/indices/numpy_sorted_index.py` & `ir_datasets-0.5.7/ir_datasets/indices/numpy_sorted_index.py`

 * *Files identical despite different names*

### Comparing `ir_datasets-0.5.6/ir_datasets/indices/zpickle_docstore.py` & `ir_datasets-0.5.7/ir_datasets/indices/zpickle_docstore.py`

 * *Files identical despite different names*

### Comparing `ir_datasets-0.5.6/ir_datasets/lazy_libs.py` & `ir_datasets-0.5.7/ir_datasets/lazy_libs.py`

 * *Files 9% similar despite different names*

```diff
@@ -103,15 +103,18 @@
     if 'ijson' not in _cache:
         import ijson
         _cache['ijson'] = ijson
     return _cache['ijson']
 
 def pyautocorpus():
     if 'pyautocorpus' not in _cache:
-        import pyautocorpus
+        try:
+            import pyautocorpus
+        except ImportError as ie:
+            raise ImportError("This dataset requires pyautocorpus. Run 'pip install pyautocorpus'") from ie
         _cache['pyautocorpus'] = pyautocorpus
     return _cache['pyautocorpus']
 
 def unlzw3():
     if 'unlzw3' not in _cache:
         import unlzw3
         _cache['unlzw3'] = unlzw3
```

### Comparing `ir_datasets-0.5.6/ir_datasets/log.py` & `ir_datasets-0.5.7/ir_datasets/log.py`

 * *Files identical despite different names*

### Comparing `ir_datasets-0.5.6/ir_datasets/util/__init__.py` & `ir_datasets-0.5.7/ir_datasets/util/__init__.py`

 * *Files identical despite different names*

### Comparing `ir_datasets-0.5.6/ir_datasets/util/download.py` & `ir_datasets-0.5.7/ir_datasets/util/download.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 import json
 import pkgutil
 import os
+import sys
 from pathlib import Path
 import atexit
 from collections import deque
 import io
 import shutil
 import tempfile
 import contextlib
@@ -16,14 +17,28 @@
 _logger = ir_datasets.log.easy()
 
 
 class BaseDownload:
     def stream(self):
         raise NotImplementedError()
 
+class GoogleCloudBucketStream(BaseDownload):
+    def __init__(self, url, tries=None):
+        self.uri = url.replace("https://storage.googleapis.com/", "gs://")
+        self.tries = tries
+
+    def __repr__(self):
+        return f'GoogleCloudBucketStream({repr(self.uri)}, tries={self.tries})'
+    
+    @contextlib.contextmanager
+    def stream(self):
+        import subprocess
+        proc = subprocess.Popen(['gsutil', 'cat', self.uri], stdout=subprocess.PIPE)
+        with io.BufferedReader(proc.stdout, buffer_size=io.DEFAULT_BUFFER_SIZE) as stream:
+            yield stream
 
 class GoogleDriveDownload(BaseDownload):
     def __init__(self, url, tries=None):
         self.url = url
         self.tries = tries
 
     def stream(self):
@@ -329,15 +344,17 @@
         if 'url' in dlc:
             small_file_size = int(os.environ.get('IR_DATASETS_SMALL_FILE_SIZE', '5000000'))
             if not dlc.get('skip_local') and dlc.get('expected_md5') and not dlc.get('size_hint', small_file_size) < small_file_size:
                 local_path = Path(self.get_download_path()) / dlc['expected_md5']
                 local_msg = (f'If you have a local copy of {dlc["url"]}, you can symlink it here '
                              f'to avoid downloading it again: {local_path}')
                 sources.append(LocalDownload(local_path, local_msg, mkdir=False))
-            if dlc['url'].startswith('https://drive.google.com/'):
+            if dlc['url'].startswith("https://storage.googleapis.com/") and 'google.colab' in sys.modules:
+                sources.append(GoogleCloudBucketStream(dlc['url'], **download_args))
+            elif dlc['url'].startswith('https://drive.google.com/'):
                 sources.append(GoogleDriveDownload(dlc['url'], **download_args))
             else:
                 sources.append(RequestsDownload(dlc['url'], **download_args))
             if dlc.get('irds_mirror') and dlc.get('expected_md5'):
                 # this file has the irds mirror to fall back on
                 sources.append(RequestsDownload(f'https://mirror.ir-datasets.com/{dlc["expected_md5"]}'))
         elif 'instructions' in dlc:
```

### Comparing `ir_datasets-0.5.6/ir_datasets/util/fileio.py` & `ir_datasets-0.5.7/ir_datasets/util/fileio.py`

 * *Files identical despite different names*

### Comparing `ir_datasets-0.5.6/ir_datasets/util/hash.py` & `ir_datasets-0.5.7/ir_datasets/util/hash.py`

 * *Files identical despite different names*

### Comparing `ir_datasets-0.5.6/ir_datasets/util/html_parsing.py` & `ir_datasets-0.5.7/ir_datasets/util/html_parsing.py`

 * *Files identical despite different names*

### Comparing `ir_datasets-0.5.6/ir_datasets/util/metadata.py` & `ir_datasets-0.5.7/ir_datasets/util/metadata.py`

 * *Files identical despite different names*

### Comparing `ir_datasets-0.5.6/ir_datasets/util/registry.py` & `ir_datasets-0.5.7/ir_datasets/util/registry.py`

 * *Files identical despite different names*

### Comparing `ir_datasets-0.5.6/ir_datasets/wrappers/html_extractor.py` & `ir_datasets-0.5.7/ir_datasets/wrappers/html_extractor.py`

 * *Files identical despite different names*

### Comparing `ir_datasets-0.5.6/ir_datasets.egg-info/PKG-INFO` & `ir_datasets-0.5.7/ir_datasets.egg-info/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,257 +1,270 @@
 Metadata-Version: 2.1
-Name: ir-datasets
-Version: 0.5.6
+Name: ir_datasets
+Version: 0.5.7
 Summary: provides a common interface to many IR ad-hoc ranking benchmarks, training datasets, etc.
 Home-page: https://github.com/allenai/ir_datasets
 Author: Sean MacAvaney
 Author-email: sean.macavaney@glasgow.ac.uk
-License: UNKNOWN
-Description: # ir_datasets
-        
-        `ir_datasets` is a python package that provides a common interface to many IR ad-hoc ranking
-        benchmarks, training datasets, etc.
-        
-        The package takes care of downloading datasets (including documents, queries, relevance judgments,
-        etc.) when available from public sources. Instructions on how to obtain datasets are provided when
-        they are not publicly available.
-        
-        `ir_datasets` provides a common iterator format to allow them to be easily used in python. It
-        attempts to provide the data in an unaltered form (i.e., keeping all fields and markup), while
-        handling differences in file formats, encoding, etc. Adapters provide extra functionality, e.g., to
-        allow quick lookups of documents by ID.
-        
-        A command line interface is also available.
-        
-        You can find a list of datasets and their features [here](https://ir-datasets.com/).
-        Want a new dataset, added functionality, or a bug fixed? Feel free to post an issue or make a pull request! 
-        
-        ## Getting Started
-        
-        For a quick start with the Python API, check out our Colab tutorials:
-        [Python](https://colab.research.google.com/github/allenai/ir_datasets/blob/master/examples/ir_datasets.ipynb)
-        [Command Line](https://colab.research.google.com/github/allenai/ir_datasets/blob/master/examples/ir_datasets_cli.ipynb)
-        
-        Install via pip:
-        
-        ```
-        pip install ir_datasets
-        ```
-        
-        If you want the main branch, you install as such:
-        
-        ```
-        pip install git+https://github.com/allenai/ir_datasets.git
-        ```
-        
-        If you want to build from source, use:
-        
-        ```
-        $ git clone https://github.com/allenai/ir_datasets
-        $ cd ir_datasets
-        $ python setup.py bdist_wheel
-        $ pip install dist/ir_datasets-*.whl
-        ```
-        
-        Tested with python versions 3.7, 3.8, 3.9, and 3.10. (Mininum python version is 3.7.)
-        
-        ## Features
-        
-        **Python and Command Line Interfaces**. Access datasts both through a simple Python API and
-        via the command line.
-        
-        ```python
-        import ir_datasets
-        dataset = ir_datasets.load('msmarco-passage/train')
-        # Documents
-        for doc in dataset.docs_iter():
-            print(doc)
-        # GenericDoc(doc_id='0', text='The presence of communication amid scientific minds was equa...
-        # GenericDoc(doc_id='1', text='The Manhattan Project and its atomic bomb helped bring an en...
-        # ...
-        ```
-        
-        ```bash
-        ir_datasets export msmarco-passage/train docs | head -n2
-        0 The presence of communication amid scientific minds was equally important to the success of the Manh...
-        1 The Manhattan Project and its atomic bomb helped bring an end to World War II. Its legacy of peacefu...
-        ```
-        
-        **Automatically downloads source files** (when available). Will download and verify the source
-        files for queries, documents, qrels, etc. when they are publicly available, as they are needed.
-        A CI build checks weekly to ensure that all the downloadable content is available and correct:
-        [![Downloadable Content](https://github.com/seanmacavaney/ir-datasets.com/actions/workflows/verify_downloads.yml/badge.svg)](https://github.com/seanmacavaney/ir-datasets.com/actions/workflows/verify_downloads.yml).
-        We mirror some troublesome files on [mirror.ir-datasets.com](https://mirror.ir-datasets.com/), and
-        automatically switch to the mirror when the original source is not available.
-        
-        ```python
-        import ir_datasets
-        dataset = ir_datasets.load('msmarco-passage/train')
-        for doc in dataset.docs_iter(): # Will download and extract MS-MARCO's collection.tar.gz the first time
-            ...
-        for query in dataset.queries_iter(): # Will download and extract MS-MARCO's queries.tar.gz the first time
-            ...
-        ```
-        
-        **Instructions for dataset access** (when not publicly available). Provides instructions on how
-        to get a copy of the data when it is not publicly available online (e.g., when it requires a
-        data usage agreement).
-        
-        ```python
-        import ir_datasets
-        dataset = ir_datasets.load('trec-arabic')
-        for doc in dataset.docs_iter():
-            ...
-        # Provides the following instructions:
-        # The dataset is based on the Arabic Newswire corpus. It is available from the LDC via: <https://catalog.ldc.upenn.edu/LDC2001T55>
-        # To proceed, symlink the source file here: [gives path]
-        ```
-        
-        **Support for datasets big and small**. By using iterators, supports large datasets that may
-        not fit into system memory, such as ClueWeb.
-        
-        ```python
-        import ir_datasets
-        dataset = ir_datasets.load('clueweb09')
-        for doc in dataset.docs_iter():
-            ... # will iterate through all ~1B documents
-        ```
-        
-        **Fixes known dataset issues**. For instance, automatically corrects the document UTF-8 encoding
-        problem in the MS-MARCO passage collection.
-        
-        ```python
-        import ir_datasets
-        dataset = ir_datasets.load('msmarco-passage')
-        docstore = dataset.docs_store()
-        docstore.get('243').text
-        # "John Maynard Keynes, 1st Baron Keynes, CB, FBA (/ˈkeɪnz/ KAYNZ; 5 June 1883 – 21 April [SNIP]"
-        # Naïve UTF-8 decoding yields double-encoding artifacts like:
-        # "John Maynard Keynes, 1st Baron Keynes, CB, FBA (/Ë\x88keÉªnz/ KAYNZ; 5 June 1883 â\x80\x93 21 April [SNIP]"
-        #                                                  ~~~~~~  ~~                       ~~~~~~~~~
-        ```
-        
-        **Fast Random Document Access.** Builds data structures that allow fast and efficient lookup of
-        document content. For large datasets, such as ClueWeb, uses
-        [checkpoint files](https://ir-datasets.com/clueweb_warc_checkpoints.md) to load documents from
-        source 40x faster than normal. Results are cached for even faster subsequent accesses.
-        
-        ```python
-        import ir_datasets
-        dataset = ir_datasets.load('clueweb12')
-        docstore = dataset.docs_store()
-        docstore.get_many(['clueweb12-0000tw-05-00014', 'clueweb12-0000tw-05-12119', 'clueweb12-0106wb-18-19516'])
-        # {'clueweb12-0000tw-05-00014': ..., 'clueweb12-0000tw-05-12119': ..., 'clueweb12-0106wb-18-19516': ...}
-        ```
-        
-        **Fancy Iter Slicing.** Sometimes it's helpful to be able to select ranges of data (e.g., for processing
-        document collections in parallel on multiple devices). Efficient implementations of slicing operations
-        allow for much faster dataset partitioning than using `itertools.slice`.
-        
-        ```python
-        import ir_datasets
-        dataset = ir_datasets.load('clueweb12')
-        dataset.docs_iter()[500:1000] # normal slicing behavior
-        # WarcDoc(doc_id='clueweb12-0000tw-00-00502', ...), WarcDoc(doc_id='clueweb12-0000tw-00-00503', ...), ...
-        dataset.docs_iter()[-10:-8] # includes negative indexing
-        # WarcDoc(doc_id='clueweb12-1914wb-28-24245', ...), WarcDoc(doc_id='clueweb12-1914wb-28-24246', ...)
-        dataset.docs_iter()[::100] # includes support for skip (only positive values)
-        # WarcDoc(doc_id='clueweb12-0000tw-00-00000', ...), WarcDoc(doc_id='clueweb12-0000tw-00-00100', ...), ...
-        dataset.docs_iter()[1/3:2/3] # supports proportional slicing (this takes the middle third of the collection)
-        # WarcDoc(doc_id='clueweb12-0605wb-28-12714', ...), WarcDoc(doc_id='clueweb12-0605wb-28-12715', ...), ...
-        ```
-        
-        ## Datasets
-        
-        Available datasets include:
-         - [ANTIQUE](https://ir-datasets.com/antique.html)
-         - [AQUAINT](https://ir-datasets.com/aquaint.html)
-         - [BEIR (benchmark suite)](https://ir-datasets.com/beir.html)
-         - [TREC CAR](https://ir-datasets.com/car.html)
-         - [C4](https://ir-datasets.com/c4.html)
-         - [ClueWeb09](https://ir-datasets.com/clueweb09.html)
-         - [ClueWeb12](https://ir-datasets.com/clueweb12.html)
-         - [CLIRMatrix](https://ir-datasets.com/clirmatrix.html)
-         - [CodeSearchNet](https://ir-datasets.com/codesearchnet.html)
-         - [CORD-19](https://ir-datasets.com/cord19.html)
-         - [DPR Wiki100](https://ir-datasets.com/dpr-w100.html)
-         - [GOV](https://ir-datasets.com/gov.html)
-         - [GOV2](https://ir-datasets.com/gov2.html)
-         - [HC4](https://ir-datasets.com/hc4.html)
-         - [Highwire (TREC Genomics 2006-07)](https://ir-datasets.com/highwire.html)
-         - [Medline](https://ir-datasets.com/medline.html)
-         - [MSMARCO (document)](https://ir-datasets.com/msmarco-document.html)
-         - [MSMARCO (passage)](https://ir-datasets.com/msmarco-passage.html)
-         - [MSMARCO (QnA)](https://ir-datasets.com/msmarco-qna.html)
-         - [Natural Questions](https://ir-datasets.com/natural-questions.html)
-         - [NFCorpus (NutritionFacts)](https://ir-datasets.com/nfcorpus.html)
-         - [NYT](https://ir-datasets.com/nyt.html)
-         - [PubMed Central (TREC CDS)](https://ir-datasets.com/pmc.html)
-         - [TREC Arabic](https://ir-datasets.com/trec-arabic.html)
-         - [TREC Fair Ranking 2021](https://ir-datasets.com/trec-fair-2021.html)
-         - [TREC Mandarin](https://ir-datasets.com/trec-mandarin.html)
-         - [TREC Robust 2004](https://ir-datasets.com/trec-robust04.html)
-         - [TREC Spanish](https://ir-datasets.com/trec-spanish.html)
-         - [TripClick](https://ir-datasets.com/tripclick.html)
-         - [Tweets 2013 (Internet Archive)](https://ir-datasets.com/tweets2013-ia.html)
-         - [Vaswani](https://ir-datasets.com/vaswani.html)
-         - [Washington Post](https://ir-datasets.com/wapo.html)
-         - [WikIR](https://ir-datasets.com/wikir.html)
-        
-        There are "subsets" under each dataset. For instance, `clueweb12/b13/trec-misinfo-2019` provides the
-        queries and judgments from the [2019 TREC misinformation track](https://trec.nist.gov/data/misinfo2019.html),
-        and `msmarco-document/orcas` provides the [ORCAS dataset](https://microsoft.github.io/msmarco/ORCAS). They
-        tend to be organized with the document collection at the top level.
-        
-        See the ir_dataets docs ([ir_datasets.com](https://ir-datasets.com/)) for details about each
-        dataset, its available subsets, and what data they provide.
-        
-        ## Environment variables
-        
-         - `IR_DATASETS_HOME`: Home directory for ir_datasets data (default `~/.ir_datasets/`). Contains directories
-           for each top-level dataset.
-         - `IR_DATASETS_TMP`: Temporary working directory (default `/tmp/ir_datasets/`).
-         - `IR_DATASETS_DL_TIMEOUT`: Download stream read timeout, in seconds (default `15`). If no data is received
-           within this duration, the connection will be assumed to be dead, and another download may be attempted.
-         - `IR_DATASETS_DL_TRIES`: Default number of download attempts before exception is thrown (default `3`).
-           When the server accepts Range requests, uses them. Otherwise, will download the entire file again
-         - `IR_DATASETS_DL_DISABLE_PBAR`: Set to `true` to disable the progress bar for downloads. Useful in settings
-           where an interactive console is not available.
-         - `IR_DATASETS_DL_SKIP_SSL`: Set to `true` to disable checking SSL certificates when downloading files.
-           Useful as a short-term solution when SSL certificates expire or are otherwise invalid. Note that this
-           does not disable hash verification of the downloaded content.
-         - `IR_DATASETS_SKIP_DISK_FREE`: Set to `true` to disable checks for enough free space on disk before
-           downloading content or otherwise creating large files.
-         - `IR_DATASETS_SMALL_FILE_SIZE`: The size of files that are considered "small", in bytes. Instructions for
-           linking small files rather then downloading them are not shown. Defaults to 5000000 (5MB).
-        
-        ## Citing
-        
-        When using datasets provided by this package, be sure to properly cite them. Bibtex for each dataset
-        can be found on the [datasets documentation page](https://ir-datasets.com/).
-        
-        If you use this tool, please cite [our SIGIR resource paper](https://arxiv.org/pdf/2103.02280.pdf):
-        
-        ```
-        @inproceedings{macavaney:sigir2021-irds,
-          author = {MacAvaney, Sean and Yates, Andrew and Feldman, Sergey and Downey, Doug and Cohan, Arman and Goharian, Nazli},
-          title = {Simplified Data Wrangling with ir_datasets},
-          year = {2021},
-          booktitle = {SIGIR}
-        }
-        ```
-        
-        ## Credits
-        
-        Contributors to this repository:
-        
-         - Sean MacAvaney (University of Glasgow)
-         - Shuo Sun (Johns Hopkins University)
-         - Thomas Jänich (University of Glasgow)
-         - Jan Heinrich Reimer (Martin Luther University Halle-Wittenberg)
-         - Maik Fröbe (Martin Luther University Halle-Wittenberg)
-         - Eugene Yang (Johns Hopkins University)
-         - Augustin Godinot (NAVERLABS Europe, ENS Paris-Saclay)
-        
-Platform: UNKNOWN
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
+License-File: LICENSE
+Requires-Dist: beautifulsoup4>=4.4.1
+Requires-Dist: inscriptis>=2.2.0
+Requires-Dist: lxml>=4.5.2
+Requires-Dist: numpy>=1.18.1
+Requires-Dist: pyyaml>=5.3.1
+Requires-Dist: requests>=2.22.0
+Requires-Dist: tqdm>=4.38.0
+Requires-Dist: trec-car-tools>=2.5.4
+Requires-Dist: lz4>=3.1.10
+Requires-Dist: warc3-wet>=0.2.3
+Requires-Dist: warc3-wet-clueweb09>=0.2.5
+Requires-Dist: zlib-state>=0.1.3
+Requires-Dist: ijson>=3.1.3
+Requires-Dist: unlzw3>=0.2.1
+
+# ir_datasets
+
+`ir_datasets` is a python package that provides a common interface to many IR ad-hoc ranking
+benchmarks, training datasets, etc.
+
+The package takes care of downloading datasets (including documents, queries, relevance judgments,
+etc.) when available from public sources. Instructions on how to obtain datasets are provided when
+they are not publicly available.
+
+`ir_datasets` provides a common iterator format to allow them to be easily used in python. It
+attempts to provide the data in an unaltered form (i.e., keeping all fields and markup), while
+handling differences in file formats, encoding, etc. Adapters provide extra functionality, e.g., to
+allow quick lookups of documents by ID.
+
+A command line interface is also available.
+
+You can find a list of datasets and their features [here](https://ir-datasets.com/).
+Want a new dataset, added functionality, or a bug fixed? Feel free to post an issue or make a pull request! 
+
+## Getting Started
+
+For a quick start with the Python API, check out our Colab tutorials:
+[Python](https://colab.research.google.com/github/allenai/ir_datasets/blob/master/examples/ir_datasets.ipynb)
+[Command Line](https://colab.research.google.com/github/allenai/ir_datasets/blob/master/examples/ir_datasets_cli.ipynb)
+
+Install via pip:
+
+```
+pip install ir_datasets
+```
+
+If you want the main branch, you install as such:
+
+```
+pip install git+https://github.com/allenai/ir_datasets.git
+```
+
+If you want to build from source, use:
+
+```
+$ git clone https://github.com/allenai/ir_datasets
+$ cd ir_datasets
+$ python setup.py bdist_wheel
+$ pip install dist/ir_datasets-*.whl
+```
+
+Tested with python versions 3.7, 3.8, 3.9, and 3.10. (Mininum python version is 3.7.)
+
+## Features
+
+**Python and Command Line Interfaces**. Access datasts both through a simple Python API and
+via the command line.
+
+```python
+import ir_datasets
+dataset = ir_datasets.load('msmarco-passage/train')
+# Documents
+for doc in dataset.docs_iter():
+    print(doc)
+# GenericDoc(doc_id='0', text='The presence of communication amid scientific minds was equa...
+# GenericDoc(doc_id='1', text='The Manhattan Project and its atomic bomb helped bring an en...
+# ...
+```
+
+```bash
+ir_datasets export msmarco-passage/train docs | head -n2
+0 The presence of communication amid scientific minds was equally important to the success of the Manh...
+1 The Manhattan Project and its atomic bomb helped bring an end to World War II. Its legacy of peacefu...
+```
+
+**Automatically downloads source files** (when available). Will download and verify the source
+files for queries, documents, qrels, etc. when they are publicly available, as they are needed.
+A CI build checks weekly to ensure that all the downloadable content is available and correct:
+[![Downloadable Content](https://github.com/seanmacavaney/ir-datasets.com/actions/workflows/verify_downloads.yml/badge.svg)](https://github.com/seanmacavaney/ir-datasets.com/actions/workflows/verify_downloads.yml).
+We mirror some troublesome files on [mirror.ir-datasets.com](https://mirror.ir-datasets.com/), and
+automatically switch to the mirror when the original source is not available.
+
+```python
+import ir_datasets
+dataset = ir_datasets.load('msmarco-passage/train')
+for doc in dataset.docs_iter(): # Will download and extract MS-MARCO's collection.tar.gz the first time
+    ...
+for query in dataset.queries_iter(): # Will download and extract MS-MARCO's queries.tar.gz the first time
+    ...
+```
+
+**Instructions for dataset access** (when not publicly available). Provides instructions on how
+to get a copy of the data when it is not publicly available online (e.g., when it requires a
+data usage agreement).
+
+```python
+import ir_datasets
+dataset = ir_datasets.load('trec-arabic')
+for doc in dataset.docs_iter():
+    ...
+# Provides the following instructions:
+# The dataset is based on the Arabic Newswire corpus. It is available from the LDC via: <https://catalog.ldc.upenn.edu/LDC2001T55>
+# To proceed, symlink the source file here: [gives path]
+```
+
+**Support for datasets big and small**. By using iterators, supports large datasets that may
+not fit into system memory, such as ClueWeb.
+
+```python
+import ir_datasets
+dataset = ir_datasets.load('clueweb09')
+for doc in dataset.docs_iter():
+    ... # will iterate through all ~1B documents
+```
+
+**Fixes known dataset issues**. For instance, automatically corrects the document UTF-8 encoding
+problem in the MS-MARCO passage collection.
+
+```python
+import ir_datasets
+dataset = ir_datasets.load('msmarco-passage')
+docstore = dataset.docs_store()
+docstore.get('243').text
+# "John Maynard Keynes, 1st Baron Keynes, CB, FBA (/ˈkeɪnz/ KAYNZ; 5 June 1883 – 21 April [SNIP]"
+# Naïve UTF-8 decoding yields double-encoding artifacts like:
+# "John Maynard Keynes, 1st Baron Keynes, CB, FBA (/Ë\x88keÉªnz/ KAYNZ; 5 June 1883 â\x80\x93 21 April [SNIP]"
+#                                                  ~~~~~~  ~~                       ~~~~~~~~~
+```
+
+**Fast Random Document Access.** Builds data structures that allow fast and efficient lookup of
+document content. For large datasets, such as ClueWeb, uses
+[checkpoint files](https://ir-datasets.com/clueweb_warc_checkpoints.md) to load documents from
+source 40x faster than normal. Results are cached for even faster subsequent accesses.
+
+```python
+import ir_datasets
+dataset = ir_datasets.load('clueweb12')
+docstore = dataset.docs_store()
+docstore.get_many(['clueweb12-0000tw-05-00014', 'clueweb12-0000tw-05-12119', 'clueweb12-0106wb-18-19516'])
+# {'clueweb12-0000tw-05-00014': ..., 'clueweb12-0000tw-05-12119': ..., 'clueweb12-0106wb-18-19516': ...}
+```
+
+**Fancy Iter Slicing.** Sometimes it's helpful to be able to select ranges of data (e.g., for processing
+document collections in parallel on multiple devices). Efficient implementations of slicing operations
+allow for much faster dataset partitioning than using `itertools.slice`.
+
+```python
+import ir_datasets
+dataset = ir_datasets.load('clueweb12')
+dataset.docs_iter()[500:1000] # normal slicing behavior
+# WarcDoc(doc_id='clueweb12-0000tw-00-00502', ...), WarcDoc(doc_id='clueweb12-0000tw-00-00503', ...), ...
+dataset.docs_iter()[-10:-8] # includes negative indexing
+# WarcDoc(doc_id='clueweb12-1914wb-28-24245', ...), WarcDoc(doc_id='clueweb12-1914wb-28-24246', ...)
+dataset.docs_iter()[::100] # includes support for skip (only positive values)
+# WarcDoc(doc_id='clueweb12-0000tw-00-00000', ...), WarcDoc(doc_id='clueweb12-0000tw-00-00100', ...), ...
+dataset.docs_iter()[1/3:2/3] # supports proportional slicing (this takes the middle third of the collection)
+# WarcDoc(doc_id='clueweb12-0605wb-28-12714', ...), WarcDoc(doc_id='clueweb12-0605wb-28-12715', ...), ...
+```
+
+## Datasets
+
+Available datasets include:
+ - [ANTIQUE](https://ir-datasets.com/antique.html)
+ - [AQUAINT](https://ir-datasets.com/aquaint.html)
+ - [BEIR (benchmark suite)](https://ir-datasets.com/beir.html)
+ - [TREC CAR](https://ir-datasets.com/car.html)
+ - [C4](https://ir-datasets.com/c4.html)
+ - [ClueWeb09](https://ir-datasets.com/clueweb09.html)
+ - [ClueWeb12](https://ir-datasets.com/clueweb12.html)
+ - [CLIRMatrix](https://ir-datasets.com/clirmatrix.html)
+ - [CodeSearchNet](https://ir-datasets.com/codesearchnet.html)
+ - [CORD-19](https://ir-datasets.com/cord19.html)
+ - [DPR Wiki100](https://ir-datasets.com/dpr-w100.html)
+ - [GOV](https://ir-datasets.com/gov.html)
+ - [GOV2](https://ir-datasets.com/gov2.html)
+ - [HC4](https://ir-datasets.com/hc4.html)
+ - [Highwire (TREC Genomics 2006-07)](https://ir-datasets.com/highwire.html)
+ - [Medline](https://ir-datasets.com/medline.html)
+ - [MSMARCO (document)](https://ir-datasets.com/msmarco-document.html)
+ - [MSMARCO (passage)](https://ir-datasets.com/msmarco-passage.html)
+ - [MSMARCO (QnA)](https://ir-datasets.com/msmarco-qna.html)
+ - [Natural Questions](https://ir-datasets.com/natural-questions.html)
+ - [NFCorpus (NutritionFacts)](https://ir-datasets.com/nfcorpus.html)
+ - [NYT](https://ir-datasets.com/nyt.html)
+ - [PubMed Central (TREC CDS)](https://ir-datasets.com/pmc.html)
+ - [TREC Arabic](https://ir-datasets.com/trec-arabic.html)
+ - [TREC Fair Ranking 2021](https://ir-datasets.com/trec-fair-2021.html)
+ - [TREC Mandarin](https://ir-datasets.com/trec-mandarin.html)
+ - [TREC Robust 2004](https://ir-datasets.com/trec-robust04.html)
+ - [TREC Spanish](https://ir-datasets.com/trec-spanish.html)
+ - [TripClick](https://ir-datasets.com/tripclick.html)
+ - [Tweets 2013 (Internet Archive)](https://ir-datasets.com/tweets2013-ia.html)
+ - [Vaswani](https://ir-datasets.com/vaswani.html)
+ - [Washington Post](https://ir-datasets.com/wapo.html)
+ - [WikIR](https://ir-datasets.com/wikir.html)
+
+There are "subsets" under each dataset. For instance, `clueweb12/b13/trec-misinfo-2019` provides the
+queries and judgments from the [2019 TREC misinformation track](https://trec.nist.gov/data/misinfo2019.html),
+and `msmarco-document/orcas` provides the [ORCAS dataset](https://microsoft.github.io/msmarco/ORCAS). They
+tend to be organized with the document collection at the top level.
+
+See the ir_dataets docs ([ir_datasets.com](https://ir-datasets.com/)) for details about each
+dataset, its available subsets, and what data they provide.
+
+## Environment variables
+
+ - `IR_DATASETS_HOME`: Home directory for ir_datasets data (default `~/.ir_datasets/`). Contains directories
+   for each top-level dataset.
+ - `IR_DATASETS_TMP`: Temporary working directory (default `/tmp/ir_datasets/`).
+ - `IR_DATASETS_DL_TIMEOUT`: Download stream read timeout, in seconds (default `15`). If no data is received
+   within this duration, the connection will be assumed to be dead, and another download may be attempted.
+ - `IR_DATASETS_DL_TRIES`: Default number of download attempts before exception is thrown (default `3`).
+   When the server accepts Range requests, uses them. Otherwise, will download the entire file again
+ - `IR_DATASETS_DL_DISABLE_PBAR`: Set to `true` to disable the progress bar for downloads. Useful in settings
+   where an interactive console is not available.
+ - `IR_DATASETS_DL_SKIP_SSL`: Set to `true` to disable checking SSL certificates when downloading files.
+   Useful as a short-term solution when SSL certificates expire or are otherwise invalid. Note that this
+   does not disable hash verification of the downloaded content.
+ - `IR_DATASETS_SKIP_DISK_FREE`: Set to `true` to disable checks for enough free space on disk before
+   downloading content or otherwise creating large files.
+ - `IR_DATASETS_SMALL_FILE_SIZE`: The size of files that are considered "small", in bytes. Instructions for
+   linking small files rather then downloading them are not shown. Defaults to 5000000 (5MB).
+
+## Citing
+
+When using datasets provided by this package, be sure to properly cite them. Bibtex for each dataset
+can be found on the [datasets documentation page](https://ir-datasets.com/).
+
+If you use this tool, please cite [our SIGIR resource paper](https://arxiv.org/pdf/2103.02280.pdf):
+
+```
+@inproceedings{macavaney:sigir2021-irds,
+  author = {MacAvaney, Sean and Yates, Andrew and Feldman, Sergey and Downey, Doug and Cohan, Arman and Goharian, Nazli},
+  title = {Simplified Data Wrangling with ir_datasets},
+  year = {2021},
+  booktitle = {SIGIR}
+}
+```
+
+## Credits
+
+Contributors to this repository:
+
+ - Sean MacAvaney (University of Glasgow)
+ - Shuo Sun (Johns Hopkins University)
+ - Thomas Jänich (University of Glasgow)
+ - Jan Heinrich Reimer (Martin Luther University Halle-Wittenberg)
+ - Maik Fröbe (Martin Luther University Halle-Wittenberg)
+ - Eugene Yang (Johns Hopkins University)
+ - Augustin Godinot (NAVERLABS Europe, ENS Paris-Saclay)
```

### Comparing `ir_datasets-0.5.6/ir_datasets.egg-info/SOURCES.txt` & `ir_datasets-0.5.7/ir_datasets.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -36,14 +36,15 @@
 ir_datasets/datasets/clirmatrix.py
 ir_datasets/datasets/clueweb09.py
 ir_datasets/datasets/clueweb12.py
 ir_datasets/datasets/codec.py
 ir_datasets/datasets/codesearchnet.py
 ir_datasets/datasets/cord19.py
 ir_datasets/datasets/cranfield.py
+ir_datasets/datasets/csl.py
 ir_datasets/datasets/disks45.py
 ir_datasets/datasets/dpr_w100.py
 ir_datasets/datasets/gov.py
 ir_datasets/datasets/gov2.py
 ir_datasets/datasets/hc4.py
 ir_datasets/datasets/highwire.py
 ir_datasets/datasets/istella22.py
@@ -92,14 +93,15 @@
 ir_datasets/docs/clirmatrix.yaml
 ir_datasets/docs/clueweb09.yaml
 ir_datasets/docs/clueweb12.yaml
 ir_datasets/docs/codec.yaml
 ir_datasets/docs/codesearchnet.yaml
 ir_datasets/docs/cord19.yaml
 ir_datasets/docs/cranfield.yaml
+ir_datasets/docs/csl.yaml
 ir_datasets/docs/disks45.yaml
 ir_datasets/docs/dpr-w100.yaml
 ir_datasets/docs/gov.yaml
 ir_datasets/docs/gov2.yaml
 ir_datasets/docs/hc4.yaml
 ir_datasets/docs/highwire.yaml
 ir_datasets/docs/istella22.yaml
```

### Comparing `ir_datasets-0.5.6/setup.py` & `ir_datasets-0.5.7/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="ir_datasets",
-    version="0.5.6", # NOTE: keep this in sync with ir_datasets/__init__.py
+    version="0.5.7", # NOTE: keep this in sync with ir_datasets/__init__.py
     author="Sean MacAvaney",
     author_email="sean.macavaney@glasgow.ac.uk",
     description="provides a common interface to many IR ad-hoc ranking benchmarks, training datasets, etc.",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/allenai/ir_datasets",
     include_package_data = True,
```

### Comparing `ir_datasets-0.5.6/test/test_defaulttext.py` & `ir_datasets-0.5.7/test/test_defaulttext.py`

 * *Files identical despite different names*

