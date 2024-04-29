# Comparing `tmp/eis1600-1.6.2.tar.gz` & `tmp/eis1600-1.6.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "eis1600-1.6.2.tar", last modified: Thu Apr  4 14:25:54 2024, max compression
+gzip compressed data, was "eis1600-1.6.3.tar", last modified: Mon Apr 29 10:16:13 2024, max compression
```

## Comparing `eis1600-1.6.2.tar` & `eis1600-1.6.3.tar`

### file list

```diff
@@ -1,155 +1,161 @@
-drwxrwxr-x   0 alicia    (1000) alicia    (1000)        0 2024-04-04 14:25:54.176272 eis1600-1.6.2/
--rw-rw-r--   0 alicia    (1000) alicia    (1000)     1046 2023-08-12 14:27:20.000000 eis1600-1.6.2/LICENSE
--rw-r--r--   0 alicia    (1000) alicia    (1000)    14837 2024-04-04 14:25:54.176272 eis1600-1.6.2/PKG-INFO
--rw-rw-r--   0 alicia    (1000) alicia    (1000)    13595 2024-03-16 19:46:15.000000 eis1600-1.6.2/README.md
-drwxrwxr-x   0 alicia    (1000) alicia    (1000)        0 2024-04-04 14:25:54.160272 eis1600-1.6.2/eis1600/
--rw-rw-r--   0 alicia    (1000) alicia    (1000)        0 2023-08-12 14:27:20.000000 eis1600-1.6.2/eis1600/__init__.py
-drwxrwxr-x   0 alicia    (1000) alicia    (1000)        0 2024-04-04 14:25:54.164271 eis1600-1.6.2/eis1600/bio/
--rw-rw-r--   0 alicia    (1000) alicia    (1000)        0 2024-01-18 10:18:32.000000 eis1600-1.6.2/eis1600/bio/__init__.py
--rw-rw-r--   0 alicia    (1000) alicia    (1000)     7450 2024-01-18 10:18:32.000000 eis1600-1.6.2/eis1600/bio/md_to_bio.py
--rw-rw-r--   0 alicia    (1000) alicia    (1000)     3998 2024-01-18 10:18:32.000000 eis1600-1.6.2/eis1600/bio/q_tags_to_bio.py
--rw-rw-r--   0 alicia    (1000) alicia    (1000)     3108 2024-01-18 10:18:32.000000 eis1600-1.6.2/eis1600/bio/topo_tags_to_bio.py
-drwxrwxr-x   0 alicia    (1000) alicia    (1000)        0 2024-04-04 14:25:54.164271 eis1600-1.6.2/eis1600/corpus_analysis/
--rw-rw-r--   0 alicia    (1000) alicia    (1000)        0 2023-11-06 14:14:46.000000 eis1600-1.6.2/eis1600/corpus_analysis/__init__.py
--rw-rw-r--   0 alicia    (1000) alicia    (1000)     5545 2024-03-27 16:37:17.000000 eis1600-1.6.2/eis1600/corpus_analysis/analyse_all_on_cluster.py
--rw-rw-r--   0 alicia    (1000) alicia    (1000)     1732 2024-03-22 08:47:34.000000 eis1600-1.6.2/eis1600/corpus_analysis/analyse_text.py
--rw-rw-r--   0 alicia    (1000) alicia    (1000)     5156 2024-04-04 09:50:23.000000 eis1600-1.6.2/eis1600/corpus_analysis/miu_methods.py
--rw-rw-r--   0 alicia    (1000) alicia    (1000)     3335 2024-03-27 16:36:35.000000 eis1600-1.6.2/eis1600/corpus_analysis/text_methods.py
-drwxrwxr-x   0 alicia    (1000) alicia    (1000)        0 2024-04-04 14:25:54.164271 eis1600-1.6.2/eis1600/dates/
--rw-rw-r--   0 alicia    (1000) alicia    (1000)      911 2023-11-02 15:25:23.000000 eis1600-1.6.2/eis1600/dates/Date.py
--rw-rw-r--   0 alicia    (1000) alicia    (1000)      755 2024-02-12 17:00:08.000000 eis1600-1.6.2/eis1600/dates/Month.py
--rw-rw-r--   0 alicia    (1000) alicia    (1000)        0 2023-08-12 14:27:20.000000 eis1600-1.6.2/eis1600/dates/__init__.py
--rw-rw-r--   0 alicia    (1000) alicia    (1000)     6571 2024-03-21 18:00:42.000000 eis1600-1.6.2/eis1600/dates/date_methods.py
--rw-rw-r--   0 alicia    (1000) alicia    (1000)     7397 2024-03-21 17:57:44.000000 eis1600-1.6.2/eis1600/dates/date_patterns.py
--rw-rw-r--   0 alicia    (1000) alicia    (1000)     2237 2024-03-01 13:31:17.000000 eis1600-1.6.2/eis1600/dates/month_methods.py
-drwxrwxr-x   0 alicia    (1000) alicia    (1000)        0 2024-04-04 14:25:54.164271 eis1600-1.6.2/eis1600/gazetteers/
--rw-rw-r--   0 alicia    (1000) alicia    (1000)     4411 2024-03-01 13:31:17.000000 eis1600-1.6.2/eis1600/gazetteers/Onomastics.py
--rw-rw-r--   0 alicia    (1000) alicia    (1000)     1267 2024-03-01 13:31:17.000000 eis1600-1.6.2/eis1600/gazetteers/Spellings.py
--rw-rw-r--   0 alicia    (1000) alicia    (1000)     3553 2024-03-01 13:31:17.000000 eis1600-1.6.2/eis1600/gazetteers/Toponyms.py
--rw-rw-r--   0 alicia    (1000) alicia    (1000)        0 2023-08-12 14:27:20.000000 eis1600-1.6.2/eis1600/gazetteers/__init__.py
-drwxrwxr-x   0 alicia    (1000) alicia    (1000)        0 2024-04-04 14:25:54.164271 eis1600-1.6.2/eis1600/gazetteers/data/
--rw-rw-r--   0 alicia    (1000) alicia    (1000)        0 2022-11-14 11:12:12.000000 eis1600-1.6.2/eis1600/gazetteers/data/__init__.py
--rw-rw-r--   0 alicia    (1000) alicia    (1000)      536 2023-07-19 09:36:14.000000 eis1600-1.6.2/eis1600/gazetteers/data/days_gazetteer.csv
--rw-rw-r--   0 alicia    (1000) alicia    (1000)      587 2023-07-19 09:36:14.000000 eis1600-1.6.2/eis1600/gazetteers/data/months_gazetteer.csv
--rw-rw-r--   0 alicia    (1000) alicia    (1000)    96536 2023-04-17 09:44:13.000000 eis1600-1.6.2/eis1600/gazetteers/data/onomastic_gazetteer.csv
--rw-rw-r--   0 alicia    (1000) alicia    (1000)     1448 2023-10-25 09:16:34.000000 eis1600-1.6.2/eis1600/gazetteers/data/spelling_gazetteer.csv
--rw-rw-r--   0 alicia    (1000) alicia    (1000)   339886 2023-11-06 12:34:27.000000 eis1600-1.6.2/eis1600/gazetteers/data/toponyms_gazetteer.csv
--rw-rw-r--   0 alicia    (1000) alicia    (1000)     2604 2023-07-19 09:36:14.000000 eis1600-1.6.2/eis1600/gazetteers/data/years_gazetteer.csv
-drwxrwxr-x   0 alicia    (1000) alicia    (1000)        0 2024-04-04 14:25:54.168271 eis1600-1.6.2/eis1600/helper/
--rw-rw-r--   0 alicia    (1000) alicia    (1000)     3429 2024-03-22 08:56:31.000000 eis1600-1.6.2/eis1600/helper/CheckFileEndingActions.py
--rw-rw-r--   0 alicia    (1000) alicia    (1000)      186 2023-11-10 14:22:15.000000 eis1600-1.6.2/eis1600/helper/Singleton.py
--rw-rw-r--   0 alicia    (1000) alicia    (1000)        0 2023-08-12 14:27:20.000000 eis1600-1.6.2/eis1600/helper/__init__.py
--rw-rw-r--   0 alicia    (1000) alicia    (1000)     1212 2024-02-19 13:06:34.000000 eis1600-1.6.2/eis1600/helper/ar_normalization.py
--rw-rw-r--   0 alicia    (1000) alicia    (1000)     3934 2024-03-27 11:22:04.000000 eis1600-1.6.2/eis1600/helper/chunking.py
-drwxrwxr-x   0 alicia    (1000) alicia    (1000)        0 2024-04-04 14:25:54.168271 eis1600-1.6.2/eis1600/helper/data/
--rw-rw-r--   0 alicia    (1000) alicia    (1000)        0 2023-04-03 10:40:59.000000 eis1600-1.6.2/eis1600/helper/data/__init__.py
--rw-rw-r--   0 alicia    (1000) alicia    (1000)     1356 2024-03-18 17:41:21.000000 eis1600-1.6.2/eis1600/helper/files_sizes.py
--rw-rw-r--   0 alicia    (1000) alicia    (1000)     2027 2024-04-04 11:02:16.000000 eis1600-1.6.2/eis1600/helper/fix_dataframe.py
--rw-rw-r--   0 alicia    (1000) alicia    (1000)      994 2024-03-16 19:46:15.000000 eis1600-1.6.2/eis1600/helper/logging.py
--rw-rw-r--   0 alicia    (1000) alicia    (1000)     6461 2023-08-12 14:27:20.000000 eis1600-1.6.2/eis1600/helper/miu_random_revisions.py
--rw-rw-r--   0 alicia    (1000) alicia    (1000)      370 2024-03-01 13:31:17.000000 eis1600-1.6.2/eis1600/helper/parse_range.py
--rw-rw-r--   0 alicia    (1000) alicia    (1000)      306 2024-03-21 11:13:13.000000 eis1600-1.6.2/eis1600/helper/part_file_names.py
-drwxrwxr-x   0 alicia    (1000) alicia    (1000)        0 2024-04-04 14:25:54.168271 eis1600-1.6.2/eis1600/json_to_text/
--rw-rw-r--   0 alicia    (1000) alicia    (1000)        0 2024-03-22 08:40:12.000000 eis1600-1.6.2/eis1600/json_to_text/__init__.py
--rw-rw-r--   0 alicia    (1000) alicia    (1000)     4106 2024-04-04 10:56:08.000000 eis1600-1.6.2/eis1600/json_to_text/reconstruct.py
-drwxrwxr-x   0 alicia    (1000) alicia    (1000)        0 2024-04-04 14:25:54.168271 eis1600-1.6.2/eis1600/json_to_tsv/
--rw-rw-r--   0 alicia    (1000) alicia    (1000)        0 2024-03-22 08:34:00.000000 eis1600-1.6.2/eis1600/json_to_tsv/__init__.py
--rw-rw-r--   0 alicia    (1000) alicia    (1000)     4912 2024-04-04 08:53:33.000000 eis1600-1.6.2/eis1600/json_to_tsv/corpus_dump.py
-drwxrwxr-x   0 alicia    (1000) alicia    (1000)        0 2024-04-04 14:25:54.168271 eis1600-1.6.2/eis1600/markdown/
--rw-rw-r--   0 alicia    (1000) alicia    (1000)      988 2024-01-18 10:18:32.000000 eis1600-1.6.2/eis1600/markdown/EntityTags.py
--rw-rw-r--   0 alicia    (1000) alicia    (1000)        0 2023-08-12 14:27:20.000000 eis1600-1.6.2/eis1600/markdown/__init__.py
--rw-rw-r--   0 alicia    (1000) alicia    (1000)     1606 2024-04-03 11:51:57.000000 eis1600-1.6.2/eis1600/markdown/category.py
-drwxrwxr-x   0 alicia    (1000) alicia    (1000)        0 2024-04-04 14:25:54.168271 eis1600-1.6.2/eis1600/markdown/data/
--rw-rw-r--   0 alicia    (1000) alicia    (1000)        0 2023-04-03 10:40:59.000000 eis1600-1.6.2/eis1600/markdown/data/__init__.py
--rw-rw-r--   0 alicia    (1000) alicia    (1000)      383 2024-02-07 09:59:48.000000 eis1600-1.6.2/eis1600/markdown/data/entity_tags.csv
--rw-rw-r--   0 alicia    (1000) alicia    (1000)      851 2024-03-01 13:31:17.000000 eis1600-1.6.2/eis1600/markdown/markdown_methods.py
--rw-rw-r--   0 alicia    (1000) alicia    (1000)     6628 2024-04-03 09:08:42.000000 eis1600-1.6.2/eis1600/markdown/markdown_patterns.py
-drwxrwxr-x   0 alicia    (1000) alicia    (1000)        0 2024-04-04 14:25:54.168271 eis1600-1.6.2/eis1600/miu/
--rw-rw-r--   0 alicia    (1000) alicia    (1000)     3513 2024-02-13 09:24:54.000000 eis1600-1.6.2/eis1600/miu/HeadingTracker.py
--rw-rw-r--   0 alicia    (1000) alicia    (1000)        0 2023-08-12 14:27:20.000000 eis1600-1.6.2/eis1600/miu/__init__.py
-drwxrwxr-x   0 alicia    (1000) alicia    (1000)        0 2024-04-04 14:25:54.168271 eis1600-1.6.2/eis1600/model_evaluations/
--rw-rw-r--   0 alicia    (1000) alicia    (1000)      393 2024-01-18 10:18:32.000000 eis1600-1.6.2/eis1600/model_evaluations/EvalResultsEncoder.py
--rw-rw-r--   0 alicia    (1000) alicia    (1000)        0 2024-01-18 10:18:32.000000 eis1600-1.6.2/eis1600/model_evaluations/__init__.py
--rw-rw-r--   0 alicia    (1000) alicia    (1000)     7701 2024-02-12 17:00:08.000000 eis1600-1.6.2/eis1600/model_evaluations/eval_date_model.py
--rw-rw-r--   0 alicia    (1000) alicia    (1000)     4800 2024-01-18 10:18:32.000000 eis1600-1.6.2/eis1600/model_evaluations/eval_topo_cat_model.py
-drwxrwxr-x   0 alicia    (1000) alicia    (1000)        0 2024-04-04 14:25:54.172271 eis1600-1.6.2/eis1600/models/
--rw-rw-r--   0 alicia    (1000) alicia    (1000)      671 2024-02-05 08:54:18.000000 eis1600-1.6.2/eis1600/models/BiosPunctuationModel.py
--rw-rw-r--   0 alicia    (1000) alicia    (1000)      566 2024-02-13 10:55:51.000000 eis1600-1.6.2/eis1600/models/Disambiguator.py
--rw-rw-r--   0 alicia    (1000) alicia    (1000)      660 2024-02-12 17:00:08.000000 eis1600-1.6.2/eis1600/models/EventsPunctuationModel.py
--rw-rw-r--   0 alicia    (1000) alicia    (1000)      259 2024-01-30 08:39:34.000000 eis1600-1.6.2/eis1600/models/FamilyContactOpinionModel.py
--rw-rw-r--   0 alicia    (1000) alicia    (1000)      592 2024-02-13 10:55:51.000000 eis1600-1.6.2/eis1600/models/Lemmatizer.py
--rw-rw-r--   0 alicia    (1000) alicia    (1000)     1762 2024-02-05 08:54:18.000000 eis1600-1.6.2/eis1600/models/Model.py
--rw-rw-r--   0 alicia    (1000) alicia    (1000)      237 2024-01-30 08:39:34.000000 eis1600-1.6.2/eis1600/models/NERModel.py
--rw-rw-r--   0 alicia    (1000) alicia    (1000)      250 2024-02-01 10:44:02.000000 eis1600-1.6.2/eis1600/models/NasabDetectionModel.py
--rw-rw-r--   0 alicia    (1000) alicia    (1000)      257 2024-01-30 08:39:34.000000 eis1600-1.6.2/eis1600/models/OnomsticElementsModel.py
--rw-rw-r--   0 alicia    (1000) alicia    (1000)      582 2024-02-13 10:55:51.000000 eis1600-1.6.2/eis1600/models/POSTagger.py
--rw-rw-r--   0 alicia    (1000) alicia    (1000)     1154 2024-02-16 15:42:32.000000 eis1600-1.6.2/eis1600/models/PoetryDetectionModel.py
--rw-rw-r--   0 alicia    (1000) alicia    (1000)      258 2024-01-30 08:39:34.000000 eis1600-1.6.2/eis1600/models/StudentTeacherModel.py
--rw-rw-r--   0 alicia    (1000) alicia    (1000)      261 2023-11-20 09:22:09.000000 eis1600-1.6.2/eis1600/models/ToponymDescriptionModel.py
--rw-rw-r--   0 alicia    (1000) alicia    (1000)      246 2024-01-30 08:39:34.000000 eis1600-1.6.2/eis1600/models/ToponymModel.py
--rw-rw-r--   0 alicia    (1000) alicia    (1000)        0 2023-11-20 09:22:09.000000 eis1600-1.6.2/eis1600/models/__init__.py
-drwxrwxr-x   0 alicia    (1000) alicia    (1000)        0 2024-04-04 14:25:54.172271 eis1600-1.6.2/eis1600/nlp/
--rw-rw-r--   0 alicia    (1000) alicia    (1000)        0 2023-08-12 14:27:20.000000 eis1600-1.6.2/eis1600/nlp/__init__.py
--rw-rw-r--   0 alicia    (1000) alicia    (1000)     4464 2024-04-03 13:59:59.000000 eis1600-1.6.2/eis1600/nlp/annotation_utils.py
--rw-rw-r--   0 alicia    (1000) alicia    (1000)     1604 2024-01-30 08:39:34.000000 eis1600-1.6.2/eis1600/nlp/utils.py
-drwxrwxr-x   0 alicia    (1000) alicia    (1000)        0 2024-04-04 14:25:54.172271 eis1600-1.6.2/eis1600/onomastics/
--rw-rw-r--   0 alicia    (1000) alicia    (1000)        0 2023-08-12 14:27:20.000000 eis1600-1.6.2/eis1600/onomastics/__init__.py
--rw-rw-r--   0 alicia    (1000) alicia    (1000)     1364 2024-01-30 08:39:34.000000 eis1600-1.6.2/eis1600/onomastics/initial_annotation.py
--rw-rw-r--   0 alicia    (1000) alicia    (1000)    10640 2024-04-03 11:14:52.000000 eis1600-1.6.2/eis1600/onomastics/methods.py
--rw-rw-r--   0 alicia    (1000) alicia    (1000)     1968 2024-01-18 10:18:32.000000 eis1600-1.6.2/eis1600/onomastics/re_pattern.py
-drwxrwxr-x   0 alicia    (1000) alicia    (1000)        0 2024-04-04 14:25:54.172271 eis1600-1.6.2/eis1600/paragraphs/
--rw-rw-r--   0 alicia    (1000) alicia    (1000)        0 2024-01-18 10:18:32.000000 eis1600-1.6.2/eis1600/paragraphs/__init__.py
--rw-rw-r--   0 alicia    (1000) alicia    (1000)     9974 2024-03-01 13:31:17.000000 eis1600-1.6.2/eis1600/paragraphs/paragraph_methods.py
--rw-rw-r--   0 alicia    (1000) alicia    (1000)     2163 2024-02-16 15:42:32.000000 eis1600-1.6.2/eis1600/paragraphs/split_mius_into_paragraphs.py
-drwxrwxr-x   0 alicia    (1000) alicia    (1000)        0 2024-04-04 14:25:54.172271 eis1600-1.6.2/eis1600/processing/
--rw-rw-r--   0 alicia    (1000) alicia    (1000)        0 2023-08-12 14:27:20.000000 eis1600-1.6.2/eis1600/processing/__init__.py
--rw-rw-r--   0 alicia    (1000) alicia    (1000)     5802 2024-04-04 10:38:59.000000 eis1600-1.6.2/eis1600/processing/postprocessing.py
--rw-rw-r--   0 alicia    (1000) alicia    (1000)     6230 2024-04-03 13:24:21.000000 eis1600-1.6.2/eis1600/processing/preprocessing.py
-drwxrwxr-x   0 alicia    (1000) alicia    (1000)        0 2024-04-04 14:25:54.172271 eis1600-1.6.2/eis1600/repositories/
--rw-rw-r--   0 alicia    (1000) alicia    (1000)        0 2024-01-18 10:18:32.000000 eis1600-1.6.2/eis1600/repositories/__init__.py
--rw-rw-r--   0 alicia    (1000) alicia    (1000)    16545 2024-04-04 08:50:01.000000 eis1600-1.6.2/eis1600/repositories/repo.py
-drwxrwxr-x   0 alicia    (1000) alicia    (1000)        0 2024-04-04 14:25:54.172271 eis1600-1.6.2/eis1600/texts_to_mius/
--rw-rw-r--   0 alicia    (1000) alicia    (1000)      431 2024-01-30 08:39:34.000000 eis1600-1.6.2/eis1600/texts_to_mius/SubIDs.py
--rw-rw-r--   0 alicia    (1000) alicia    (1000)     1820 2024-01-18 10:18:32.000000 eis1600-1.6.2/eis1600/texts_to_mius/UIDs.py
--rw-rw-r--   0 alicia    (1000) alicia    (1000)        0 2024-01-18 10:18:32.000000 eis1600-1.6.2/eis1600/texts_to_mius/__init__.py
--rw-rw-r--   0 alicia    (1000) alicia    (1000)     1939 2024-03-16 19:46:15.000000 eis1600-1.6.2/eis1600/texts_to_mius/check_formatting.py
--rw-rw-r--   0 alicia    (1000) alicia    (1000)     7572 2024-04-03 09:09:16.000000 eis1600-1.6.2/eis1600/texts_to_mius/check_formatting_methods.py
--rw-rw-r--   0 alicia    (1000) alicia    (1000)     3696 2024-03-16 19:46:15.000000 eis1600-1.6.2/eis1600/texts_to_mius/check_mius.py
--rw-rw-r--   0 alicia    (1000) alicia    (1000)     3742 2024-01-18 10:18:32.000000 eis1600-1.6.2/eis1600/texts_to_mius/convert_mARkdown_methods.py
--rw-rw-r--   0 alicia    (1000) alicia    (1000)     4179 2024-02-05 08:54:18.000000 eis1600-1.6.2/eis1600/texts_to_mius/convert_mARkdown_to_EIS1600TMP.py
--rw-rw-r--   0 alicia    (1000) alicia    (1000)     1562 2024-03-01 13:31:17.000000 eis1600-1.6.2/eis1600/texts_to_mius/download_text_selection_sheet.py
--rw-rw-r--   0 alicia    (1000) alicia    (1000)     3312 2024-03-16 19:46:15.000000 eis1600-1.6.2/eis1600/texts_to_mius/ids_insert_or_update.py
--rw-rw-r--   0 alicia    (1000) alicia    (1000)     1463 2024-03-01 13:50:55.000000 eis1600-1.6.2/eis1600/texts_to_mius/incorporate_newly_prepared_files_in_corpus.py
--rw-rw-r--   0 alicia    (1000) alicia    (1000)    14062 2024-04-03 11:49:39.000000 eis1600-1.6.2/eis1600/texts_to_mius/subid_methods.py
-drwxrwxr-x   0 alicia    (1000) alicia    (1000)        0 2024-04-04 14:25:54.176272 eis1600-1.6.2/eis1600/toponym_descriptions/
--rw-rw-r--   0 alicia    (1000) alicia    (1000)        0 2024-01-18 10:18:32.000000 eis1600-1.6.2/eis1600/toponym_descriptions/__init__.py
--rw-rw-r--   0 alicia    (1000) alicia    (1000)     4456 2024-03-01 13:31:17.000000 eis1600-1.6.2/eis1600/toponym_descriptions/annotate_topd.py
--rw-rw-r--   0 alicia    (1000) alicia    (1000)     2783 2024-01-18 10:18:32.000000 eis1600-1.6.2/eis1600/toponym_descriptions/btopd_to_bio.py
--rw-rw-r--   0 alicia    (1000) alicia    (1000)     4944 2024-01-18 10:18:32.000000 eis1600-1.6.2/eis1600/toponym_descriptions/topod_extract_incomplete.py
--rw-rw-r--   0 alicia    (1000) alicia    (1000)     4151 2024-01-18 10:18:32.000000 eis1600-1.6.2/eis1600/toponym_descriptions/topod_extract_places_regex.py
--rw-rw-r--   0 alicia    (1000) alicia    (1000)     3709 2024-02-16 15:42:32.000000 eis1600-1.6.2/eis1600/toponym_descriptions/topod_insert_into_miu.py
--rw-rw-r--   0 alicia    (1000) alicia    (1000)     1710 2024-01-18 10:18:32.000000 eis1600-1.6.2/eis1600/toponym_descriptions/topod_sheets_stats.py
-drwxrwxr-x   0 alicia    (1000) alicia    (1000)        0 2024-04-04 14:25:54.176272 eis1600-1.6.2/eis1600/toponyms/
--rw-rw-r--   0 alicia    (1000) alicia    (1000)        0 2023-08-12 14:27:20.000000 eis1600-1.6.2/eis1600/toponyms/__init__.py
--rw-rw-r--   0 alicia    (1000) alicia    (1000)     1975 2024-01-30 08:39:34.000000 eis1600-1.6.2/eis1600/toponyms/initial_category_annotation.py
--rw-rw-r--   0 alicia    (1000) alicia    (1000)     3199 2023-11-02 14:43:12.000000 eis1600-1.6.2/eis1600/toponyms/methods.py
--rw-rw-r--   0 alicia    (1000) alicia    (1000)     1659 2023-11-02 14:43:12.000000 eis1600-1.6.2/eis1600/toponyms/toponym_categories.py
-drwxrwxr-x   0 alicia    (1000) alicia    (1000)        0 2024-04-04 14:25:54.176272 eis1600-1.6.2/eis1600/training_data/
--rw-rw-r--   0 alicia    (1000) alicia    (1000)        0 2024-01-30 08:39:34.000000 eis1600-1.6.2/eis1600/training_data/__init__.py
--rw-rw-r--   0 alicia    (1000) alicia    (1000)     1535 2024-01-30 08:39:34.000000 eis1600-1.6.2/eis1600/training_data/annotate_onomastics.py
--rw-rw-r--   0 alicia    (1000) alicia    (1000)     1098 2024-01-30 08:39:34.000000 eis1600-1.6.2/eis1600/training_data/online_editor_files.py
--rw-rw-r--   0 alicia    (1000) alicia    (1000)     4121 2024-01-30 08:39:34.000000 eis1600-1.6.2/eis1600/training_data/reannotation.py
-drwxrwxr-x   0 alicia    (1000) alicia    (1000)        0 2024-04-04 14:25:54.176272 eis1600-1.6.2/eis1600/yml/
--rw-rw-r--   0 alicia    (1000) alicia    (1000)     9610 2024-04-03 15:04:40.000000 eis1600-1.6.2/eis1600/yml/YAMLHandler.py
--rw-rw-r--   0 alicia    (1000) alicia    (1000)        0 2024-01-18 10:18:32.000000 eis1600-1.6.2/eis1600/yml/__init__.py
--rw-rw-r--   0 alicia    (1000) alicia    (1000)    12671 2024-04-04 08:44:59.000000 eis1600-1.6.2/eis1600/yml/yml_handling.py
--rw-rw-r--   0 alicia    (1000) alicia    (1000)      383 2024-01-18 10:18:32.000000 eis1600-1.6.2/eis1600/yml/yml_methods.py
-drwxrwxr-x   0 alicia    (1000) alicia    (1000)        0 2024-04-04 14:25:54.176272 eis1600-1.6.2/eis1600.egg-info/
--rw-r--r--   0 alicia    (1000) alicia    (1000)    14837 2024-04-04 14:25:54.000000 eis1600-1.6.2/eis1600.egg-info/PKG-INFO
--rw-rw-r--   0 alicia    (1000) alicia    (1000)     4456 2024-04-04 14:25:54.000000 eis1600-1.6.2/eis1600.egg-info/SOURCES.txt
--rw-rw-r--   0 alicia    (1000) alicia    (1000)        1 2024-04-04 14:25:54.000000 eis1600-1.6.2/eis1600.egg-info/dependency_links.txt
--rw-rw-r--   0 alicia    (1000) alicia    (1000)     1770 2024-04-04 14:25:54.000000 eis1600-1.6.2/eis1600.egg-info/entry_points.txt
--rw-rw-r--   0 alicia    (1000) alicia    (1000)      201 2024-04-04 14:25:54.000000 eis1600-1.6.2/eis1600.egg-info/requires.txt
--rw-rw-r--   0 alicia    (1000) alicia    (1000)        8 2024-04-04 14:25:54.000000 eis1600-1.6.2/eis1600.egg-info/top_level.txt
--rw-rw-r--   0 alicia    (1000) alicia    (1000)       38 2024-04-04 14:25:54.176272 eis1600-1.6.2/setup.cfg
--rw-rw-r--   0 alicia    (1000) alicia    (1000)     3930 2024-04-04 14:25:31.000000 eis1600-1.6.2/setup.py
+drwxrwxr-x   0 alicia    (1000) alicia    (1000)        0 2024-04-29 10:16:13.471563 eis1600-1.6.3/
+-rw-rw-r--   0 alicia    (1000) alicia    (1000)     1046 2023-08-12 14:27:20.000000 eis1600-1.6.3/LICENSE
+-rw-r--r--   0 alicia    (1000) alicia    (1000)    14837 2024-04-29 10:16:13.471563 eis1600-1.6.3/PKG-INFO
+-rw-rw-r--   0 alicia    (1000) alicia    (1000)    13595 2024-03-16 19:46:15.000000 eis1600-1.6.3/README.md
+drwxrwxr-x   0 alicia    (1000) alicia    (1000)        0 2024-04-29 10:16:13.455563 eis1600-1.6.3/eis1600/
+-rw-rw-r--   0 alicia    (1000) alicia    (1000)        0 2023-08-12 14:27:20.000000 eis1600-1.6.3/eis1600/__init__.py
+drwxrwxr-x   0 alicia    (1000) alicia    (1000)        0 2024-04-29 10:16:13.455563 eis1600-1.6.3/eis1600/bio/
+-rw-rw-r--   0 alicia    (1000) alicia    (1000)        0 2024-01-18 10:18:32.000000 eis1600-1.6.3/eis1600/bio/__init__.py
+-rw-rw-r--   0 alicia    (1000) alicia    (1000)     7450 2024-01-18 10:18:32.000000 eis1600-1.6.3/eis1600/bio/md_to_bio.py
+-rw-rw-r--   0 alicia    (1000) alicia    (1000)     3998 2024-01-18 10:18:32.000000 eis1600-1.6.3/eis1600/bio/q_tags_to_bio.py
+-rw-rw-r--   0 alicia    (1000) alicia    (1000)     3108 2024-01-18 10:18:32.000000 eis1600-1.6.3/eis1600/bio/topo_tags_to_bio.py
+drwxrwxr-x   0 alicia    (1000) alicia    (1000)        0 2024-04-29 10:16:13.459563 eis1600-1.6.3/eis1600/corpus_analysis/
+-rw-rw-r--   0 alicia    (1000) alicia    (1000)        0 2023-11-06 14:14:46.000000 eis1600-1.6.3/eis1600/corpus_analysis/__init__.py
+-rw-rw-r--   0 alicia    (1000) alicia    (1000)     6032 2024-04-25 15:37:43.000000 eis1600-1.6.3/eis1600/corpus_analysis/analyse_all_on_cluster.py
+-rw-rw-r--   0 alicia    (1000) alicia    (1000)     1732 2024-03-22 08:47:34.000000 eis1600-1.6.3/eis1600/corpus_analysis/analyse_text.py
+-rw-rw-r--   0 alicia    (1000) alicia    (1000)     5156 2024-04-04 09:50:23.000000 eis1600-1.6.3/eis1600/corpus_analysis/miu_methods.py
+-rw-rw-r--   0 alicia    (1000) alicia    (1000)     3335 2024-03-27 16:36:35.000000 eis1600-1.6.3/eis1600/corpus_analysis/text_methods.py
+drwxrwxr-x   0 alicia    (1000) alicia    (1000)        0 2024-04-29 10:16:13.459563 eis1600-1.6.3/eis1600/dates/
+-rw-rw-r--   0 alicia    (1000) alicia    (1000)      911 2023-11-02 15:25:23.000000 eis1600-1.6.3/eis1600/dates/Date.py
+-rw-rw-r--   0 alicia    (1000) alicia    (1000)      755 2024-02-12 17:00:08.000000 eis1600-1.6.3/eis1600/dates/Month.py
+-rw-rw-r--   0 alicia    (1000) alicia    (1000)        0 2023-08-12 14:27:20.000000 eis1600-1.6.3/eis1600/dates/__init__.py
+-rw-rw-r--   0 alicia    (1000) alicia    (1000)     6571 2024-02-12 17:08:43.000000 eis1600-1.6.3/eis1600/dates/date_methods.py
+-rw-rw-r--   0 alicia    (1000) alicia    (1000)     7397 2024-03-21 17:57:44.000000 eis1600-1.6.3/eis1600/dates/date_patterns.py
+-rw-rw-r--   0 alicia    (1000) alicia    (1000)     2237 2024-03-01 13:31:17.000000 eis1600-1.6.3/eis1600/dates/month_methods.py
+drwxrwxr-x   0 alicia    (1000) alicia    (1000)        0 2024-04-29 10:16:13.459563 eis1600-1.6.3/eis1600/gazetteers/
+-rw-rw-r--   0 alicia    (1000) alicia    (1000)     4411 2024-03-01 13:31:17.000000 eis1600-1.6.3/eis1600/gazetteers/Onomastics.py
+-rw-rw-r--   0 alicia    (1000) alicia    (1000)     1267 2024-03-01 13:31:17.000000 eis1600-1.6.3/eis1600/gazetteers/Spellings.py
+-rw-rw-r--   0 alicia    (1000) alicia    (1000)     3553 2024-03-01 13:31:17.000000 eis1600-1.6.3/eis1600/gazetteers/Toponyms.py
+-rw-rw-r--   0 alicia    (1000) alicia    (1000)        0 2023-08-12 14:27:20.000000 eis1600-1.6.3/eis1600/gazetteers/__init__.py
+drwxrwxr-x   0 alicia    (1000) alicia    (1000)        0 2024-04-29 10:16:13.459563 eis1600-1.6.3/eis1600/gazetteers/data/
+-rw-rw-r--   0 alicia    (1000) alicia    (1000)        0 2022-11-14 11:12:12.000000 eis1600-1.6.3/eis1600/gazetteers/data/__init__.py
+-rw-rw-r--   0 alicia    (1000) alicia    (1000)      536 2023-07-19 09:36:14.000000 eis1600-1.6.3/eis1600/gazetteers/data/days_gazetteer.csv
+-rw-rw-r--   0 alicia    (1000) alicia    (1000)      587 2023-07-19 09:36:14.000000 eis1600-1.6.3/eis1600/gazetteers/data/months_gazetteer.csv
+-rw-rw-r--   0 alicia    (1000) alicia    (1000)    96536 2023-04-17 09:44:13.000000 eis1600-1.6.3/eis1600/gazetteers/data/onomastic_gazetteer.csv
+-rw-rw-r--   0 alicia    (1000) alicia    (1000)     1448 2023-10-25 09:16:34.000000 eis1600-1.6.3/eis1600/gazetteers/data/spelling_gazetteer.csv
+-rw-rw-r--   0 alicia    (1000) alicia    (1000)   339886 2023-11-06 12:34:27.000000 eis1600-1.6.3/eis1600/gazetteers/data/toponyms_gazetteer.csv
+-rw-rw-r--   0 alicia    (1000) alicia    (1000)     2604 2023-07-19 09:36:14.000000 eis1600-1.6.3/eis1600/gazetteers/data/years_gazetteer.csv
+drwxrwxr-x   0 alicia    (1000) alicia    (1000)        0 2024-04-29 10:16:13.463563 eis1600-1.6.3/eis1600/helper/
+-rw-rw-r--   0 alicia    (1000) alicia    (1000)     3429 2024-03-22 08:56:31.000000 eis1600-1.6.3/eis1600/helper/CheckFileEndingActions.py
+-rw-rw-r--   0 alicia    (1000) alicia    (1000)      186 2023-11-10 14:22:15.000000 eis1600-1.6.3/eis1600/helper/Singleton.py
+-rw-rw-r--   0 alicia    (1000) alicia    (1000)        0 2023-08-12 14:27:20.000000 eis1600-1.6.3/eis1600/helper/__init__.py
+-rw-rw-r--   0 alicia    (1000) alicia    (1000)     1212 2024-02-19 13:06:34.000000 eis1600-1.6.3/eis1600/helper/ar_normalization.py
+-rw-rw-r--   0 alicia    (1000) alicia    (1000)     3934 2024-03-27 11:22:04.000000 eis1600-1.6.3/eis1600/helper/chunking.py
+drwxrwxr-x   0 alicia    (1000) alicia    (1000)        0 2024-04-29 10:16:13.463563 eis1600-1.6.3/eis1600/helper/data/
+-rw-rw-r--   0 alicia    (1000) alicia    (1000)        0 2023-04-03 10:40:59.000000 eis1600-1.6.3/eis1600/helper/data/__init__.py
+-rw-rw-r--   0 alicia    (1000) alicia    (1000)     1356 2024-03-18 17:41:21.000000 eis1600-1.6.3/eis1600/helper/files_sizes.py
+-rw-rw-r--   0 alicia    (1000) alicia    (1000)     2027 2024-04-04 11:02:16.000000 eis1600-1.6.3/eis1600/helper/fix_dataframe.py
+-rw-rw-r--   0 alicia    (1000) alicia    (1000)      994 2024-03-16 19:46:15.000000 eis1600-1.6.3/eis1600/helper/logging.py
+-rw-rw-r--   0 alicia    (1000) alicia    (1000)     6461 2023-08-12 14:27:20.000000 eis1600-1.6.3/eis1600/helper/miu_random_revisions.py
+-rw-rw-r--   0 alicia    (1000) alicia    (1000)      370 2024-03-01 13:31:17.000000 eis1600-1.6.3/eis1600/helper/parse_range.py
+-rw-rw-r--   0 alicia    (1000) alicia    (1000)      306 2024-03-21 11:13:13.000000 eis1600-1.6.3/eis1600/helper/part_file_names.py
+drwxrwxr-x   0 alicia    (1000) alicia    (1000)        0 2024-04-29 10:16:13.463563 eis1600-1.6.3/eis1600/json_to_text/
+-rw-rw-r--   0 alicia    (1000) alicia    (1000)        0 2024-03-22 08:40:12.000000 eis1600-1.6.3/eis1600/json_to_text/__init__.py
+-rw-rw-r--   0 alicia    (1000) alicia    (1000)     4106 2024-04-24 08:16:19.000000 eis1600-1.6.3/eis1600/json_to_text/reconstruct.py
+drwxrwxr-x   0 alicia    (1000) alicia    (1000)        0 2024-04-29 10:16:13.463563 eis1600-1.6.3/eis1600/json_to_tsv/
+-rw-rw-r--   0 alicia    (1000) alicia    (1000)        0 2024-03-22 08:34:00.000000 eis1600-1.6.3/eis1600/json_to_tsv/__init__.py
+-rw-rw-r--   0 alicia    (1000) alicia    (1000)     5013 2024-04-04 15:35:16.000000 eis1600-1.6.3/eis1600/json_to_tsv/corpus_dump.py
+drwxrwxr-x   0 alicia    (1000) alicia    (1000)        0 2024-04-29 10:16:13.463563 eis1600-1.6.3/eis1600/markdown/
+-rw-rw-r--   0 alicia    (1000) alicia    (1000)      988 2024-01-18 10:18:32.000000 eis1600-1.6.3/eis1600/markdown/EntityTags.py
+-rw-rw-r--   0 alicia    (1000) alicia    (1000)        0 2023-08-12 14:27:20.000000 eis1600-1.6.3/eis1600/markdown/__init__.py
+-rw-rw-r--   0 alicia    (1000) alicia    (1000)     1606 2024-04-03 11:51:57.000000 eis1600-1.6.3/eis1600/markdown/category.py
+drwxrwxr-x   0 alicia    (1000) alicia    (1000)        0 2024-04-29 10:16:13.463563 eis1600-1.6.3/eis1600/markdown/data/
+-rw-rw-r--   0 alicia    (1000) alicia    (1000)        0 2024-01-18 10:18:32.000000 eis1600-1.6.3/eis1600/markdown/data/__init__.py
+-rw-rw-r--   0 alicia    (1000) alicia    (1000)      383 2024-02-12 17:00:08.000000 eis1600-1.6.3/eis1600/markdown/data/entity_tags.csv
+-rw-rw-r--   0 alicia    (1000) alicia    (1000)      851 2024-03-01 13:31:17.000000 eis1600-1.6.3/eis1600/markdown/markdown_methods.py
+-rw-rw-r--   0 alicia    (1000) alicia    (1000)     6628 2024-04-03 09:08:42.000000 eis1600-1.6.3/eis1600/markdown/markdown_patterns.py
+drwxrwxr-x   0 alicia    (1000) alicia    (1000)        0 2024-04-29 10:16:13.463563 eis1600-1.6.3/eis1600/miu/
+-rw-rw-r--   0 alicia    (1000) alicia    (1000)     3513 2024-02-13 09:24:54.000000 eis1600-1.6.3/eis1600/miu/HeadingTracker.py
+-rw-rw-r--   0 alicia    (1000) alicia    (1000)        0 2023-08-12 14:27:20.000000 eis1600-1.6.3/eis1600/miu/__init__.py
+drwxrwxr-x   0 alicia    (1000) alicia    (1000)        0 2024-04-29 10:16:13.463563 eis1600-1.6.3/eis1600/model_evaluations/
+-rw-rw-r--   0 alicia    (1000) alicia    (1000)      393 2024-01-18 10:18:32.000000 eis1600-1.6.3/eis1600/model_evaluations/EvalResultsEncoder.py
+-rw-rw-r--   0 alicia    (1000) alicia    (1000)        0 2024-01-18 10:18:32.000000 eis1600-1.6.3/eis1600/model_evaluations/__init__.py
+-rw-rw-r--   0 alicia    (1000) alicia    (1000)     7701 2024-02-12 17:00:08.000000 eis1600-1.6.3/eis1600/model_evaluations/eval_date_model.py
+-rw-rw-r--   0 alicia    (1000) alicia    (1000)     4800 2024-01-18 10:18:32.000000 eis1600-1.6.3/eis1600/model_evaluations/eval_topo_cat_model.py
+drwxrwxr-x   0 alicia    (1000) alicia    (1000)        0 2024-04-29 10:16:13.463563 eis1600-1.6.3/eis1600/models/
+-rw-rw-r--   0 alicia    (1000) alicia    (1000)      671 2024-02-05 08:54:18.000000 eis1600-1.6.3/eis1600/models/BiosPunctuationModel.py
+-rw-rw-r--   0 alicia    (1000) alicia    (1000)      566 2024-02-13 10:55:51.000000 eis1600-1.6.3/eis1600/models/Disambiguator.py
+-rw-rw-r--   0 alicia    (1000) alicia    (1000)      660 2024-02-12 17:00:08.000000 eis1600-1.6.3/eis1600/models/EventsPunctuationModel.py
+-rw-rw-r--   0 alicia    (1000) alicia    (1000)      259 2024-01-30 08:39:34.000000 eis1600-1.6.3/eis1600/models/FamilyContactOpinionModel.py
+-rw-rw-r--   0 alicia    (1000) alicia    (1000)      592 2024-02-13 10:55:51.000000 eis1600-1.6.3/eis1600/models/Lemmatizer.py
+-rw-rw-r--   0 alicia    (1000) alicia    (1000)     1762 2024-02-05 08:54:18.000000 eis1600-1.6.3/eis1600/models/Model.py
+-rw-rw-r--   0 alicia    (1000) alicia    (1000)      237 2024-01-30 08:39:34.000000 eis1600-1.6.3/eis1600/models/NERModel.py
+-rw-rw-r--   0 alicia    (1000) alicia    (1000)      250 2024-02-01 10:44:02.000000 eis1600-1.6.3/eis1600/models/NasabDetectionModel.py
+-rw-rw-r--   0 alicia    (1000) alicia    (1000)      257 2024-01-30 08:39:34.000000 eis1600-1.6.3/eis1600/models/OnomsticElementsModel.py
+-rw-rw-r--   0 alicia    (1000) alicia    (1000)      582 2024-02-13 10:55:51.000000 eis1600-1.6.3/eis1600/models/POSTagger.py
+-rw-rw-r--   0 alicia    (1000) alicia    (1000)     1154 2024-02-16 15:42:32.000000 eis1600-1.6.3/eis1600/models/PoetryDetectionModel.py
+-rw-rw-r--   0 alicia    (1000) alicia    (1000)      258 2024-01-30 08:39:34.000000 eis1600-1.6.3/eis1600/models/StudentTeacherModel.py
+-rw-rw-r--   0 alicia    (1000) alicia    (1000)      261 2023-11-20 09:22:09.000000 eis1600-1.6.3/eis1600/models/ToponymDescriptionModel.py
+-rw-rw-r--   0 alicia    (1000) alicia    (1000)      246 2024-01-30 08:39:34.000000 eis1600-1.6.3/eis1600/models/ToponymModel.py
+-rw-rw-r--   0 alicia    (1000) alicia    (1000)        0 2023-11-20 09:22:09.000000 eis1600-1.6.3/eis1600/models/__init__.py
+drwxrwxr-x   0 alicia    (1000) alicia    (1000)        0 2024-04-29 10:16:13.463563 eis1600-1.6.3/eis1600/nlp/
+-rw-rw-r--   0 alicia    (1000) alicia    (1000)        0 2023-08-12 14:27:20.000000 eis1600-1.6.3/eis1600/nlp/__init__.py
+-rw-rw-r--   0 alicia    (1000) alicia    (1000)     4464 2024-04-11 12:45:39.000000 eis1600-1.6.3/eis1600/nlp/annotation_utils.py
+-rw-rw-r--   0 alicia    (1000) alicia    (1000)     1604 2024-01-30 08:39:34.000000 eis1600-1.6.3/eis1600/nlp/utils.py
+drwxrwxr-x   0 alicia    (1000) alicia    (1000)        0 2024-04-29 10:16:13.467563 eis1600-1.6.3/eis1600/onomastics/
+-rw-rw-r--   0 alicia    (1000) alicia    (1000)        0 2023-08-12 14:27:20.000000 eis1600-1.6.3/eis1600/onomastics/__init__.py
+-rw-rw-r--   0 alicia    (1000) alicia    (1000)     1364 2024-01-30 08:39:34.000000 eis1600-1.6.3/eis1600/onomastics/initial_annotation.py
+-rw-rw-r--   0 alicia    (1000) alicia    (1000)    10640 2024-04-03 11:14:52.000000 eis1600-1.6.3/eis1600/onomastics/methods.py
+-rw-rw-r--   0 alicia    (1000) alicia    (1000)     1968 2024-01-18 10:18:32.000000 eis1600-1.6.3/eis1600/onomastics/re_pattern.py
+drwxrwxr-x   0 alicia    (1000) alicia    (1000)        0 2024-04-29 10:16:13.467563 eis1600-1.6.3/eis1600/paragraphs/
+-rw-rw-r--   0 alicia    (1000) alicia    (1000)        0 2024-01-18 10:18:32.000000 eis1600-1.6.3/eis1600/paragraphs/__init__.py
+-rw-rw-r--   0 alicia    (1000) alicia    (1000)     9974 2024-03-01 13:31:17.000000 eis1600-1.6.3/eis1600/paragraphs/paragraph_methods.py
+-rw-rw-r--   0 alicia    (1000) alicia    (1000)     2163 2024-02-16 15:42:32.000000 eis1600-1.6.3/eis1600/paragraphs/split_mius_into_paragraphs.py
+drwxrwxr-x   0 alicia    (1000) alicia    (1000)        0 2024-04-29 10:16:13.467563 eis1600-1.6.3/eis1600/processing/
+-rw-rw-r--   0 alicia    (1000) alicia    (1000)        0 2023-08-12 14:27:20.000000 eis1600-1.6.3/eis1600/processing/__init__.py
+-rw-rw-r--   0 alicia    (1000) alicia    (1000)     5802 2024-04-25 14:11:19.000000 eis1600-1.6.3/eis1600/processing/postprocessing.py
+-rw-rw-r--   0 alicia    (1000) alicia    (1000)     6230 2024-02-12 17:00:08.000000 eis1600-1.6.3/eis1600/processing/preprocessing.py
+-rw-rw-r--   0 alicia    (1000) alicia    (1000)     3008 2024-04-29 10:00:52.000000 eis1600-1.6.3/eis1600/processing/short_miu_generation.py
+drwxrwxr-x   0 alicia    (1000) alicia    (1000)        0 2024-04-29 10:16:13.467563 eis1600-1.6.3/eis1600/repositories/
+-rw-rw-r--   0 alicia    (1000) alicia    (1000)        0 2024-01-18 10:18:32.000000 eis1600-1.6.3/eis1600/repositories/__init__.py
+-rw-rw-r--   0 alicia    (1000) alicia    (1000)    16545 2024-04-04 08:50:01.000000 eis1600-1.6.3/eis1600/repositories/repo.py
+drwxrwxr-x   0 alicia    (1000) alicia    (1000)        0 2024-04-29 10:16:13.467563 eis1600-1.6.3/eis1600/statistics/
+-rw-r--r--   0 alicia    (1000) alicia    (1000)        0 2023-08-12 14:27:20.000000 eis1600-1.6.3/eis1600/statistics/__init__.py
+-rw-r--r--   0 alicia    (1000) alicia    (1000)     2786 2024-01-18 10:18:32.000000 eis1600-1.6.3/eis1600/statistics/count_categories.py
+-rw-r--r--   0 alicia    (1000) alicia    (1000)     3548 2024-01-18 10:18:32.000000 eis1600-1.6.3/eis1600/statistics/count_tokens_per_miu.py
+-rw-r--r--   0 alicia    (1000) alicia    (1000)      958 2023-08-12 14:27:20.000000 eis1600-1.6.3/eis1600/statistics/methods.py
+drwxrwxr-x   0 alicia    (1000) alicia    (1000)        0 2024-04-29 10:16:13.467563 eis1600-1.6.3/eis1600/texts_to_mius/
+-rw-rw-r--   0 alicia    (1000) alicia    (1000)      431 2024-01-30 08:39:34.000000 eis1600-1.6.3/eis1600/texts_to_mius/SubIDs.py
+-rw-rw-r--   0 alicia    (1000) alicia    (1000)     1820 2024-01-18 10:18:32.000000 eis1600-1.6.3/eis1600/texts_to_mius/UIDs.py
+-rw-rw-r--   0 alicia    (1000) alicia    (1000)        0 2024-01-18 10:18:32.000000 eis1600-1.6.3/eis1600/texts_to_mius/__init__.py
+-rw-rw-r--   0 alicia    (1000) alicia    (1000)     1939 2024-03-16 19:46:15.000000 eis1600-1.6.3/eis1600/texts_to_mius/check_formatting.py
+-rw-rw-r--   0 alicia    (1000) alicia    (1000)     7572 2024-04-03 09:09:16.000000 eis1600-1.6.3/eis1600/texts_to_mius/check_formatting_methods.py
+-rw-rw-r--   0 alicia    (1000) alicia    (1000)     3696 2024-03-16 19:46:15.000000 eis1600-1.6.3/eis1600/texts_to_mius/check_mius.py
+-rw-rw-r--   0 alicia    (1000) alicia    (1000)     3742 2024-01-18 10:18:32.000000 eis1600-1.6.3/eis1600/texts_to_mius/convert_mARkdown_methods.py
+-rw-rw-r--   0 alicia    (1000) alicia    (1000)     4179 2024-02-05 08:54:18.000000 eis1600-1.6.3/eis1600/texts_to_mius/convert_mARkdown_to_EIS1600TMP.py
+-rw-rw-r--   0 alicia    (1000) alicia    (1000)     1562 2024-03-01 13:31:17.000000 eis1600-1.6.3/eis1600/texts_to_mius/download_text_selection_sheet.py
+-rw-rw-r--   0 alicia    (1000) alicia    (1000)     3312 2024-03-16 19:46:15.000000 eis1600-1.6.3/eis1600/texts_to_mius/ids_insert_or_update.py
+-rw-rw-r--   0 alicia    (1000) alicia    (1000)     1463 2024-03-01 13:50:55.000000 eis1600-1.6.3/eis1600/texts_to_mius/incorporate_newly_prepared_files_in_corpus.py
+-rw-rw-r--   0 alicia    (1000) alicia    (1000)    14062 2024-04-03 11:49:39.000000 eis1600-1.6.3/eis1600/texts_to_mius/subid_methods.py
+drwxrwxr-x   0 alicia    (1000) alicia    (1000)        0 2024-04-29 10:16:13.467563 eis1600-1.6.3/eis1600/toponym_descriptions/
+-rw-rw-r--   0 alicia    (1000) alicia    (1000)        0 2024-01-18 10:18:32.000000 eis1600-1.6.3/eis1600/toponym_descriptions/__init__.py
+-rw-rw-r--   0 alicia    (1000) alicia    (1000)     4456 2024-03-01 13:31:17.000000 eis1600-1.6.3/eis1600/toponym_descriptions/annotate_topd.py
+-rw-rw-r--   0 alicia    (1000) alicia    (1000)     2783 2024-01-18 10:18:32.000000 eis1600-1.6.3/eis1600/toponym_descriptions/btopd_to_bio.py
+-rw-rw-r--   0 alicia    (1000) alicia    (1000)     4944 2024-01-18 10:18:32.000000 eis1600-1.6.3/eis1600/toponym_descriptions/topod_extract_incomplete.py
+-rw-rw-r--   0 alicia    (1000) alicia    (1000)     4151 2024-01-18 10:18:32.000000 eis1600-1.6.3/eis1600/toponym_descriptions/topod_extract_places_regex.py
+-rw-rw-r--   0 alicia    (1000) alicia    (1000)     3709 2024-02-16 15:42:32.000000 eis1600-1.6.3/eis1600/toponym_descriptions/topod_insert_into_miu.py
+-rw-rw-r--   0 alicia    (1000) alicia    (1000)     1710 2024-01-18 10:18:32.000000 eis1600-1.6.3/eis1600/toponym_descriptions/topod_sheets_stats.py
+drwxrwxr-x   0 alicia    (1000) alicia    (1000)        0 2024-04-29 10:16:13.467563 eis1600-1.6.3/eis1600/toponyms/
+-rw-rw-r--   0 alicia    (1000) alicia    (1000)        0 2023-08-12 14:27:20.000000 eis1600-1.6.3/eis1600/toponyms/__init__.py
+-rw-rw-r--   0 alicia    (1000) alicia    (1000)     1975 2024-01-30 08:39:34.000000 eis1600-1.6.3/eis1600/toponyms/initial_category_annotation.py
+-rw-rw-r--   0 alicia    (1000) alicia    (1000)     3199 2023-11-02 14:43:12.000000 eis1600-1.6.3/eis1600/toponyms/methods.py
+-rw-rw-r--   0 alicia    (1000) alicia    (1000)     1659 2023-11-02 14:43:12.000000 eis1600-1.6.3/eis1600/toponyms/toponym_categories.py
+drwxrwxr-x   0 alicia    (1000) alicia    (1000)        0 2024-04-29 10:16:13.467563 eis1600-1.6.3/eis1600/training_data/
+-rw-rw-r--   0 alicia    (1000) alicia    (1000)        0 2024-01-30 08:39:34.000000 eis1600-1.6.3/eis1600/training_data/__init__.py
+-rw-rw-r--   0 alicia    (1000) alicia    (1000)     1535 2024-01-30 08:39:34.000000 eis1600-1.6.3/eis1600/training_data/annotate_onomastics.py
+-rw-rw-r--   0 alicia    (1000) alicia    (1000)     1098 2024-01-30 08:39:34.000000 eis1600-1.6.3/eis1600/training_data/online_editor_files.py
+-rw-rw-r--   0 alicia    (1000) alicia    (1000)     4121 2024-01-30 08:39:34.000000 eis1600-1.6.3/eis1600/training_data/reannotation.py
+drwxrwxr-x   0 alicia    (1000) alicia    (1000)        0 2024-04-29 10:16:13.471563 eis1600-1.6.3/eis1600/yml/
+-rw-rw-r--   0 alicia    (1000) alicia    (1000)     9610 2024-04-03 15:04:40.000000 eis1600-1.6.3/eis1600/yml/YAMLHandler.py
+-rw-rw-r--   0 alicia    (1000) alicia    (1000)        0 2024-01-18 10:18:32.000000 eis1600-1.6.3/eis1600/yml/__init__.py
+-rw-rw-r--   0 alicia    (1000) alicia    (1000)    12820 2024-04-09 11:27:31.000000 eis1600-1.6.3/eis1600/yml/yml_handling.py
+-rw-rw-r--   0 alicia    (1000) alicia    (1000)      383 2024-01-18 10:18:32.000000 eis1600-1.6.3/eis1600/yml/yml_methods.py
+drwxrwxr-x   0 alicia    (1000) alicia    (1000)        0 2024-04-29 10:16:13.471563 eis1600-1.6.3/eis1600.egg-info/
+-rw-r--r--   0 alicia    (1000) alicia    (1000)    14837 2024-04-29 10:16:13.000000 eis1600-1.6.3/eis1600.egg-info/PKG-INFO
+-rw-rw-r--   0 alicia    (1000) alicia    (1000)     4642 2024-04-29 10:16:13.000000 eis1600-1.6.3/eis1600.egg-info/SOURCES.txt
+-rw-rw-r--   0 alicia    (1000) alicia    (1000)        1 2024-04-29 10:16:13.000000 eis1600-1.6.3/eis1600.egg-info/dependency_links.txt
+-rw-rw-r--   0 alicia    (1000) alicia    (1000)     1851 2024-04-29 10:16:13.000000 eis1600-1.6.3/eis1600.egg-info/entry_points.txt
+-rw-rw-r--   0 alicia    (1000) alicia    (1000)      201 2024-04-29 10:16:13.000000 eis1600-1.6.3/eis1600.egg-info/requires.txt
+-rw-rw-r--   0 alicia    (1000) alicia    (1000)        8 2024-04-29 10:16:13.000000 eis1600-1.6.3/eis1600.egg-info/top_level.txt
+-rw-rw-r--   0 alicia    (1000) alicia    (1000)       38 2024-04-29 10:16:13.471563 eis1600-1.6.3/setup.cfg
+-rw-rw-r--   0 alicia    (1000) alicia    (1000)     4214 2024-04-29 10:15:51.000000 eis1600-1.6.3/setup.py
```

### Comparing `eis1600-1.6.2/LICENSE` & `eis1600-1.6.3/LICENSE`

 * *Files identical despite different names*

### Comparing `eis1600-1.6.2/PKG-INFO` & `eis1600-1.6.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: eis1600
-Version: 1.6.2
+Version: 1.6.3
 Summary: EIS1600 project tools and utilities
 Home-page: https://github.com/EIS1600/eis1600-pkg
 Author: Lisa Mischer
 Author-email: mischer.lisa@gmail.com
 License: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `eis1600-1.6.2/README.md` & `eis1600-1.6.3/README.md`

 * *Files identical despite different names*

### Comparing `eis1600-1.6.2/eis1600/bio/md_to_bio.py` & `eis1600-1.6.3/eis1600/bio/md_to_bio.py`

 * *Files identical despite different names*

### Comparing `eis1600-1.6.2/eis1600/bio/q_tags_to_bio.py` & `eis1600-1.6.3/eis1600/bio/q_tags_to_bio.py`

 * *Files identical despite different names*

### Comparing `eis1600-1.6.2/eis1600/bio/topo_tags_to_bio.py` & `eis1600-1.6.3/eis1600/bio/topo_tags_to_bio.py`

 * *Files identical despite different names*

### Comparing `eis1600-1.6.2/eis1600/corpus_analysis/analyse_all_on_cluster.py` & `eis1600-1.6.3/eis1600/corpus_analysis/analyse_all_on_cluster.py`

 * *Files 6% similar despite different names*

```diff
@@ -19,14 +19,16 @@
 from eis1600.corpus_analysis.text_methods import get_text_as_list_of_mius
 from eis1600.json_to_tsv.corpus_dump import dump_file
 from eis1600.helper.logging import setup_persistent_logger
 from eis1600.helper.parse_range import parse_range
 from eis1600.repositories.repo import JSON_REPO, TEXT_REPO, PART_NAME_INFIX, PART_NUM_REGEX, \
                                        get_ready_and_double_checked_files
 
+from eis1600.processing.short_miu_generation import get_short_miu, save_ids
+
 
 def routine_per_text(
         infile: str,
         parallel: Optional[bool] = False,
         force: Optional[bool] = False,
         clean_out_dir: Optional[bool] = False,
         debug: Optional[bool] = False,
@@ -64,25 +66,32 @@
                 error += f'{uid}\n{e}\n\n\n'
             except Exception:
                 raise
 
     dir_path, _ = os.path.split(out_path)
     Path(dir_path).mkdir(parents=True, exist_ok=True)
 
-    # if file is original or part 1, remove previous json files to avoid problem with previous chunkings
+    # if file is original or part 1, it might be good to remove previous json files
+    # to avoid problems with previous chunking
     if clean_out_dir and (PART_NAME_INFIX not in out_path or int(PART_NUM_REGEX.search(out_path).group(1)) == 1):
         if os.path.exists(dir_path):
             for json_file in glob.iglob(os.path.join(dir_path, "*.json")):
                 os.remove(json_file)
 
+    # add short id to each miu object
+    for miu_obj in res:
+        miu_obj["yml"]["id"] = get_short_miu(miu_obj["yml"]["UID"])
+
     with open(out_path, 'w', encoding='utf-8') as fh:
         jsonpickle.set_encoder_options('json', indent=4, ensure_ascii=False)
         json_str = jsonpickle.encode(res, unpicklable=False)
         fh.write(json_str)
 
+    save_ids()
+
     if error:
         raise ValueError(error)
 
 
 def main():
     arg_parser = ArgumentParser(
             prog=sys.argv[0], formatter_class=RawDescriptionHelpFormatter,
@@ -103,23 +112,29 @@
     )
     arg_parser.add_argument(
             "--random", "-r",
             action="store_true",
             help="randomise list of files"
     )
     arg_parser.add_argument(
+            "--clean_out_dir",
+            action="store_true",
+            help="clean previous processing, in case there has been a different chunking"
+    )
+    arg_parser.add_argument(
             "--force", "-f",
             action="store_true",
             help="process file regardless if it exist and overwrite it"
     )
 
     args = arg_parser.parse_args()
     debug = args.debug
     parallel = args.parallel
     force = args.force
+    clean_out_dir = args.clean_out_dir
 
     print(f'GPU available: {cuda.is_available()}')
 
     st = time()
     stp = process_time()
 
     # Retrieve all double-checked texts
@@ -141,15 +156,15 @@
         shuffle(infiles_indexes)
 
     for i in tqdm(infiles_indexes):
         infile = infiles[i]
         print(f"[{i+1}] {infile}")
 
         try:
-            routine_per_text(infile, parallel=parallel, force=force, clean_out_dir=True, debug=debug)
+            routine_per_text(infile, parallel=parallel, force=force, clean_out_dir=clean_out_dir, debug=debug)
             if not args.no_tsv:
                 dump_file(infile)
         except ValueError as e:
             logger.error(f'{infile}\n{e}')
         except Exception as e:
             print(e)
             logger.exception(f'{infile}\n{e}')
```

### Comparing `eis1600-1.6.2/eis1600/corpus_analysis/analyse_text.py` & `eis1600-1.6.3/eis1600/corpus_analysis/analyse_text.py`

 * *Files identical despite different names*

### Comparing `eis1600-1.6.2/eis1600/corpus_analysis/miu_methods.py` & `eis1600-1.6.3/eis1600/corpus_analysis/miu_methods.py`

 * *Files identical despite different names*

### Comparing `eis1600-1.6.2/eis1600/corpus_analysis/text_methods.py` & `eis1600-1.6.3/eis1600/corpus_analysis/text_methods.py`

 * *Files identical despite different names*

### Comparing `eis1600-1.6.2/eis1600/dates/Date.py` & `eis1600-1.6.3/eis1600/dates/Date.py`

 * *Files identical despite different names*

### Comparing `eis1600-1.6.2/eis1600/dates/Month.py` & `eis1600-1.6.3/eis1600/dates/Month.py`

 * *Files identical despite different names*

### Comparing `eis1600-1.6.2/eis1600/dates/date_methods.py` & `eis1600-1.6.3/eis1600/dates/date_methods.py`

 * *Files identical despite different names*

### Comparing `eis1600-1.6.2/eis1600/dates/date_patterns.py` & `eis1600-1.6.3/eis1600/dates/date_patterns.py`

 * *Files identical despite different names*

### Comparing `eis1600-1.6.2/eis1600/dates/month_methods.py` & `eis1600-1.6.3/eis1600/dates/month_methods.py`

 * *Files identical despite different names*

### Comparing `eis1600-1.6.2/eis1600/gazetteers/Onomastics.py` & `eis1600-1.6.3/eis1600/gazetteers/Onomastics.py`

 * *Files identical despite different names*

### Comparing `eis1600-1.6.2/eis1600/gazetteers/Spellings.py` & `eis1600-1.6.3/eis1600/gazetteers/Spellings.py`

 * *Files identical despite different names*

### Comparing `eis1600-1.6.2/eis1600/gazetteers/Toponyms.py` & `eis1600-1.6.3/eis1600/gazetteers/Toponyms.py`

 * *Files identical despite different names*

### Comparing `eis1600-1.6.2/eis1600/gazetteers/data/days_gazetteer.csv` & `eis1600-1.6.3/eis1600/gazetteers/data/days_gazetteer.csv`

 * *Files identical despite different names*

### Comparing `eis1600-1.6.2/eis1600/gazetteers/data/months_gazetteer.csv` & `eis1600-1.6.3/eis1600/gazetteers/data/months_gazetteer.csv`

 * *Files identical despite different names*

### Comparing `eis1600-1.6.2/eis1600/gazetteers/data/onomastic_gazetteer.csv` & `eis1600-1.6.3/eis1600/gazetteers/data/onomastic_gazetteer.csv`

 * *Files identical despite different names*

### Comparing `eis1600-1.6.2/eis1600/gazetteers/data/spelling_gazetteer.csv` & `eis1600-1.6.3/eis1600/gazetteers/data/spelling_gazetteer.csv`

 * *Files identical despite different names*

### Comparing `eis1600-1.6.2/eis1600/gazetteers/data/toponyms_gazetteer.csv` & `eis1600-1.6.3/eis1600/gazetteers/data/toponyms_gazetteer.csv`

 * *Files identical despite different names*

### Comparing `eis1600-1.6.2/eis1600/gazetteers/data/years_gazetteer.csv` & `eis1600-1.6.3/eis1600/gazetteers/data/years_gazetteer.csv`

 * *Files identical despite different names*

### Comparing `eis1600-1.6.2/eis1600/helper/CheckFileEndingActions.py` & `eis1600-1.6.3/eis1600/helper/CheckFileEndingActions.py`

 * *Files identical despite different names*

### Comparing `eis1600-1.6.2/eis1600/helper/ar_normalization.py` & `eis1600-1.6.3/eis1600/helper/ar_normalization.py`

 * *Files identical despite different names*

### Comparing `eis1600-1.6.2/eis1600/helper/chunking.py` & `eis1600-1.6.3/eis1600/helper/chunking.py`

 * *Files identical despite different names*

### Comparing `eis1600-1.6.2/eis1600/helper/files_sizes.py` & `eis1600-1.6.3/eis1600/helper/files_sizes.py`

 * *Files identical despite different names*

### Comparing `eis1600-1.6.2/eis1600/helper/fix_dataframe.py` & `eis1600-1.6.3/eis1600/helper/fix_dataframe.py`

 * *Files identical despite different names*

### Comparing `eis1600-1.6.2/eis1600/helper/logging.py` & `eis1600-1.6.3/eis1600/helper/logging.py`

 * *Files identical despite different names*

### Comparing `eis1600-1.6.2/eis1600/helper/miu_random_revisions.py` & `eis1600-1.6.3/eis1600/helper/miu_random_revisions.py`

 * *Files identical despite different names*

### Comparing `eis1600-1.6.2/eis1600/json_to_text/reconstruct.py` & `eis1600-1.6.3/eis1600/json_to_text/reconstruct.py`

 * *Files identical despite different names*

### Comparing `eis1600-1.6.2/eis1600/json_to_tsv/corpus_dump.py` & `eis1600-1.6.3/eis1600/json_to_tsv/corpus_dump.py`

 * *Files 2% similar despite different names*

```diff
@@ -19,14 +19,19 @@
 def dump_file(fpath: str, label_list: tuple[str] = ALL_LABELS):
 
     if not fpath.endswith(".json"):
         fpath = fpath.replace(TEXT_REPO, JSON_REPO)
         fpath = fpath.replace('.EIS1600', '.json')
 
     structural_data, content_data = [], []
+
+    if not Path(fpath).is_file():
+        print(f"Warning! file {fpath} not found")
+        return
+
     with open(fpath, "r", encoding="utf-8") as fp:
         data = json.load(fp)
 
     for miu in data:
         header = miu["yml"]
         uid = header["UID"]
```

### Comparing `eis1600-1.6.2/eis1600/markdown/EntityTags.py` & `eis1600-1.6.3/eis1600/markdown/EntityTags.py`

 * *Files identical despite different names*

### Comparing `eis1600-1.6.2/eis1600/markdown/category.py` & `eis1600-1.6.3/eis1600/markdown/category.py`

 * *Files identical despite different names*

### Comparing `eis1600-1.6.2/eis1600/markdown/markdown_methods.py` & `eis1600-1.6.3/eis1600/markdown/markdown_methods.py`

 * *Files identical despite different names*

### Comparing `eis1600-1.6.2/eis1600/markdown/markdown_patterns.py` & `eis1600-1.6.3/eis1600/markdown/markdown_patterns.py`

 * *Files identical despite different names*

### Comparing `eis1600-1.6.2/eis1600/miu/HeadingTracker.py` & `eis1600-1.6.3/eis1600/miu/HeadingTracker.py`

 * *Files identical despite different names*

### Comparing `eis1600-1.6.2/eis1600/model_evaluations/eval_date_model.py` & `eis1600-1.6.3/eis1600/model_evaluations/eval_date_model.py`

 * *Files identical despite different names*

### Comparing `eis1600-1.6.2/eis1600/model_evaluations/eval_topo_cat_model.py` & `eis1600-1.6.3/eis1600/model_evaluations/eval_topo_cat_model.py`

 * *Files identical despite different names*

### Comparing `eis1600-1.6.2/eis1600/models/BiosPunctuationModel.py` & `eis1600-1.6.3/eis1600/models/BiosPunctuationModel.py`

 * *Files identical despite different names*

### Comparing `eis1600-1.6.2/eis1600/models/Disambiguator.py` & `eis1600-1.6.3/eis1600/models/Disambiguator.py`

 * *Files identical despite different names*

### Comparing `eis1600-1.6.2/eis1600/models/EventsPunctuationModel.py` & `eis1600-1.6.3/eis1600/models/EventsPunctuationModel.py`

 * *Files identical despite different names*

### Comparing `eis1600-1.6.2/eis1600/models/Lemmatizer.py` & `eis1600-1.6.3/eis1600/models/Lemmatizer.py`

 * *Files identical despite different names*

### Comparing `eis1600-1.6.2/eis1600/models/Model.py` & `eis1600-1.6.3/eis1600/models/Model.py`

 * *Files identical despite different names*

### Comparing `eis1600-1.6.2/eis1600/models/POSTagger.py` & `eis1600-1.6.3/eis1600/models/POSTagger.py`

 * *Files identical despite different names*

### Comparing `eis1600-1.6.2/eis1600/models/PoetryDetectionModel.py` & `eis1600-1.6.3/eis1600/models/PoetryDetectionModel.py`

 * *Files identical despite different names*

### Comparing `eis1600-1.6.2/eis1600/nlp/annotation_utils.py` & `eis1600-1.6.3/eis1600/nlp/annotation_utils.py`

 * *Files identical despite different names*

### Comparing `eis1600-1.6.2/eis1600/nlp/utils.py` & `eis1600-1.6.3/eis1600/nlp/utils.py`

 * *Files identical despite different names*

### Comparing `eis1600-1.6.2/eis1600/onomastics/initial_annotation.py` & `eis1600-1.6.3/eis1600/onomastics/initial_annotation.py`

 * *Files identical despite different names*

### Comparing `eis1600-1.6.2/eis1600/onomastics/methods.py` & `eis1600-1.6.3/eis1600/onomastics/methods.py`

 * *Files identical despite different names*

### Comparing `eis1600-1.6.2/eis1600/onomastics/re_pattern.py` & `eis1600-1.6.3/eis1600/onomastics/re_pattern.py`

 * *Files identical despite different names*

### Comparing `eis1600-1.6.2/eis1600/paragraphs/paragraph_methods.py` & `eis1600-1.6.3/eis1600/paragraphs/paragraph_methods.py`

 * *Files identical despite different names*

### Comparing `eis1600-1.6.2/eis1600/paragraphs/split_mius_into_paragraphs.py` & `eis1600-1.6.3/eis1600/paragraphs/split_mius_into_paragraphs.py`

 * *Files identical despite different names*

### Comparing `eis1600-1.6.2/eis1600/processing/postprocessing.py` & `eis1600-1.6.3/eis1600/processing/postprocessing.py`

 * *Files identical despite different names*

### Comparing `eis1600-1.6.2/eis1600/processing/preprocessing.py` & `eis1600-1.6.3/eis1600/processing/preprocessing.py`

 * *Files identical despite different names*

### Comparing `eis1600-1.6.2/eis1600/repositories/repo.py` & `eis1600-1.6.3/eis1600/repositories/repo.py`

 * *Files identical despite different names*

### Comparing `eis1600-1.6.2/eis1600/texts_to_mius/UIDs.py` & `eis1600-1.6.3/eis1600/texts_to_mius/UIDs.py`

 * *Files identical despite different names*

### Comparing `eis1600-1.6.2/eis1600/texts_to_mius/check_formatting.py` & `eis1600-1.6.3/eis1600/texts_to_mius/check_formatting.py`

 * *Files identical despite different names*

### Comparing `eis1600-1.6.2/eis1600/texts_to_mius/check_formatting_methods.py` & `eis1600-1.6.3/eis1600/texts_to_mius/check_formatting_methods.py`

 * *Files identical despite different names*

### Comparing `eis1600-1.6.2/eis1600/texts_to_mius/check_mius.py` & `eis1600-1.6.3/eis1600/texts_to_mius/check_mius.py`

 * *Files identical despite different names*

### Comparing `eis1600-1.6.2/eis1600/texts_to_mius/convert_mARkdown_methods.py` & `eis1600-1.6.3/eis1600/texts_to_mius/convert_mARkdown_methods.py`

 * *Files identical despite different names*

### Comparing `eis1600-1.6.2/eis1600/texts_to_mius/convert_mARkdown_to_EIS1600TMP.py` & `eis1600-1.6.3/eis1600/texts_to_mius/convert_mARkdown_to_EIS1600TMP.py`

 * *Files identical despite different names*

### Comparing `eis1600-1.6.2/eis1600/texts_to_mius/download_text_selection_sheet.py` & `eis1600-1.6.3/eis1600/texts_to_mius/download_text_selection_sheet.py`

 * *Files identical despite different names*

### Comparing `eis1600-1.6.2/eis1600/texts_to_mius/ids_insert_or_update.py` & `eis1600-1.6.3/eis1600/texts_to_mius/ids_insert_or_update.py`

 * *Files identical despite different names*

### Comparing `eis1600-1.6.2/eis1600/texts_to_mius/incorporate_newly_prepared_files_in_corpus.py` & `eis1600-1.6.3/eis1600/texts_to_mius/incorporate_newly_prepared_files_in_corpus.py`

 * *Files identical despite different names*

### Comparing `eis1600-1.6.2/eis1600/texts_to_mius/subid_methods.py` & `eis1600-1.6.3/eis1600/texts_to_mius/subid_methods.py`

 * *Files identical despite different names*

### Comparing `eis1600-1.6.2/eis1600/toponym_descriptions/annotate_topd.py` & `eis1600-1.6.3/eis1600/toponym_descriptions/annotate_topd.py`

 * *Files identical despite different names*

### Comparing `eis1600-1.6.2/eis1600/toponym_descriptions/btopd_to_bio.py` & `eis1600-1.6.3/eis1600/toponym_descriptions/btopd_to_bio.py`

 * *Files identical despite different names*

### Comparing `eis1600-1.6.2/eis1600/toponym_descriptions/topod_extract_incomplete.py` & `eis1600-1.6.3/eis1600/toponym_descriptions/topod_extract_incomplete.py`

 * *Files identical despite different names*

### Comparing `eis1600-1.6.2/eis1600/toponym_descriptions/topod_extract_places_regex.py` & `eis1600-1.6.3/eis1600/toponym_descriptions/topod_extract_places_regex.py`

 * *Files identical despite different names*

### Comparing `eis1600-1.6.2/eis1600/toponym_descriptions/topod_insert_into_miu.py` & `eis1600-1.6.3/eis1600/toponym_descriptions/topod_insert_into_miu.py`

 * *Files identical despite different names*

### Comparing `eis1600-1.6.2/eis1600/toponym_descriptions/topod_sheets_stats.py` & `eis1600-1.6.3/eis1600/toponym_descriptions/topod_sheets_stats.py`

 * *Files identical despite different names*

### Comparing `eis1600-1.6.2/eis1600/toponyms/initial_category_annotation.py` & `eis1600-1.6.3/eis1600/toponyms/initial_category_annotation.py`

 * *Files identical despite different names*

### Comparing `eis1600-1.6.2/eis1600/toponyms/methods.py` & `eis1600-1.6.3/eis1600/toponyms/methods.py`

 * *Files identical despite different names*

### Comparing `eis1600-1.6.2/eis1600/toponyms/toponym_categories.py` & `eis1600-1.6.3/eis1600/toponyms/toponym_categories.py`

 * *Files identical despite different names*

### Comparing `eis1600-1.6.2/eis1600/training_data/annotate_onomastics.py` & `eis1600-1.6.3/eis1600/training_data/annotate_onomastics.py`

 * *Files identical despite different names*

### Comparing `eis1600-1.6.2/eis1600/training_data/online_editor_files.py` & `eis1600-1.6.3/eis1600/training_data/online_editor_files.py`

 * *Files identical despite different names*

### Comparing `eis1600-1.6.2/eis1600/training_data/reannotation.py` & `eis1600-1.6.3/eis1600/training_data/reannotation.py`

 * *Files identical despite different names*

### Comparing `eis1600-1.6.2/eis1600/yml/YAMLHandler.py` & `eis1600-1.6.3/eis1600/yml/YAMLHandler.py`

 * *Files identical despite different names*

### Comparing `eis1600-1.6.2/eis1600/yml/yml_handling.py` & `eis1600-1.6.3/eis1600/yml/yml_handling.py`

 * *Files 1% similar despite different names*

```diff
@@ -145,14 +145,17 @@
         try:
             entity = ' '.join(df['TOKENS'].iloc[index:index + length].to_list())
         except TypeError:
             print(f'Entity {" ".join(df["TOKENS"].iloc[index:index + length].replace(np.nan, ""))}'
                   f' with tag {row["full_tag"]} seem to be splitted between two sections.'
                   f' It has been added to the first section.\nCheck: {file_path}')
             entity = ' '.join(df['TOKENS'].iloc[index:index + length].replace(np.nan, '').to_list())
+            if not entity.strip():
+                yml_handler.set_error_while_collecting_annotated_entities(row["full_tag"])
+                return
         cat = entity_tags_df.loc[entity_tags_df['TAG'].str.fullmatch(tag), 'CATEGORY'].iloc[0]
 
         if cat == 'DATE' or cat == 'LUNAR_MONTH' or cat == 'AGE':
             try:
                 val, e_cat = get_yrs_tag_value(row['full_tag'])
                 add_to_entities_dict(entities_dict, cat, {'entity': entity, cat.lower(): val, 'cat': e_cat})
             except ValueError:
```

### Comparing `eis1600-1.6.2/eis1600.egg-info/PKG-INFO` & `eis1600-1.6.3/eis1600.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: eis1600
-Version: 1.6.2
+Version: 1.6.3
 Summary: EIS1600 project tools and utilities
 Home-page: https://github.com/EIS1600/eis1600-pkg
 Author: Lisa Mischer
 Author-email: mischer.lisa@gmail.com
 License: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `eis1600-1.6.2/eis1600.egg-info/SOURCES.txt` & `eis1600-1.6.3/eis1600.egg-info/SOURCES.txt`

 * *Files 6% similar despite different names*

```diff
@@ -87,16 +87,21 @@
 eis1600/onomastics/re_pattern.py
 eis1600/paragraphs/__init__.py
 eis1600/paragraphs/paragraph_methods.py
 eis1600/paragraphs/split_mius_into_paragraphs.py
 eis1600/processing/__init__.py
 eis1600/processing/postprocessing.py
 eis1600/processing/preprocessing.py
+eis1600/processing/short_miu_generation.py
 eis1600/repositories/__init__.py
 eis1600/repositories/repo.py
+eis1600/statistics/__init__.py
+eis1600/statistics/count_categories.py
+eis1600/statistics/count_tokens_per_miu.py
+eis1600/statistics/methods.py
 eis1600/texts_to_mius/SubIDs.py
 eis1600/texts_to_mius/UIDs.py
 eis1600/texts_to_mius/__init__.py
 eis1600/texts_to_mius/check_formatting.py
 eis1600/texts_to_mius/check_formatting_methods.py
 eis1600/texts_to_mius/check_mius.py
 eis1600/texts_to_mius/convert_mARkdown_methods.py
```

### Comparing `eis1600-1.6.2/eis1600.egg-info/entry_points.txt` & `eis1600-1.6.3/eis1600.egg-info/entry_points.txt`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 [console_scripts]
 analyse_all_on_cluster = eis1600.corpus_analysis.analyse_all_on_cluster:main [EIS]
 analyse_text = eis1600.corpus_analysis.analyse_text:main [EIS]
 annotate_topd = eis1600.toponym_descriptions.annotate_topd:main [NER]
 btopd_to_bio = eis1600.toponym_descriptions.btopd_to_bio:main
 check_formatting = eis1600.texts_to_mius.check_formatting:main
 check_mius = eis1600.texts_to_mius.check_mius:main
+clean_ids_mapping = eis1600.processing.short_miu_generation:clean_unused_old_ids
 convert_mARkdown_to_EIS1600TMP = eis1600.texts_to_mius.convert_mARkdown_to_EIS1600TMP:main
 count_tokens_per_miu = eis1600.statistics.count_tokens_per_miu:main
 eval_date_model = eis1600.model_evaluations.eval_date_model:main [EVAL]
 eval_topo_cat_model = eis1600.model_evaluations.eval_topo_cat_model:main [EVAL]
 ids_insert_or_update = eis1600.texts_to_mius.ids_insert_or_update:main
 incorporate_newly_prepared_files_in_corpus = eis1600.texts_to_mius.incorporate_newly_prepared_files_in_corpus:main
 miu_random_revisions = eis1600.helper.miu_random_revisions:main
```

### Comparing `eis1600-1.6.2/setup.py` & `eis1600-1.6.3/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,42 +1,45 @@
 from setuptools import setup, find_packages
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setup(name='eis1600',
-      version='1.6.2',
+      version='1.6.3',
       description='EIS1600 project tools and utilities',
       long_description=long_description,
       long_description_content_type="text/markdown",
       url='https://github.com/EIS1600/eis1600-pkg',
       author='Lisa Mischer',
       author_email='mischer.lisa@gmail.com',
       license='MIT License',
       packages=find_packages(include=['eis1600', 'eis1600.*'], exclude=['excluded']),
       package_data={
               'eis1600.gazetteers.data': ['*.csv'],
               'eis1600.markdown.data': ['*.csv'],
-              'eis1600.models.data': ['*.csv']
+              'eis1600.models.data': ['*.csv'],
+              'eis1600.processing.persistent_ids': ['long_short_ids_mapping.json',
+                                                    'deprecated_long_short_ids_mapping.json']
       },
       entry_points={
           'console_scripts': [
                   'analyse_all_on_cluster = eis1600.corpus_analysis.analyse_all_on_cluster:main [EIS]',
                   'analyse_text = eis1600.corpus_analysis.analyse_text:main [EIS]',
                   'annotate_topd = eis1600.toponym_descriptions.annotate_topd:main [NER]',
                   'btopd_to_bio = eis1600.toponym_descriptions.btopd_to_bio:main',
                   'check_formatting = eis1600.texts_to_mius.check_formatting:main',
                   'check_mius = eis1600.texts_to_mius.check_mius:main',
+                  'clean_ids_mapping = eis1600.processing.short_miu_generation:clean_unused_old_ids',
                   'convert_mARkdown_to_EIS1600TMP = eis1600.texts_to_mius.convert_mARkdown_to_EIS1600TMP:main',
                   'count_tokens_per_miu = eis1600.statistics.count_tokens_per_miu:main',
                   'eval_date_model = eis1600.model_evaluations.eval_date_model:main [EVAL]',
                   'eval_topo_cat_model = eis1600.model_evaluations.eval_topo_cat_model:main [EVAL]',
                   'ids_insert_or_update = eis1600.texts_to_mius.ids_insert_or_update:main',
                   'incorporate_newly_prepared_files_in_corpus = '
-                  'eis1600.texts_to_mius.incorporate_newly_prepared_files_in_corpus:main',
+                      'eis1600.texts_to_mius.incorporate_newly_prepared_files_in_corpus:main',
                   'miu_random_revisions = eis1600.helper.miu_random_revisions:main',
                   'mius_count_categories = eis1600.statistics.count_categories:main',
                   'q_tags_to_bio = eis1600.bio.q_tags_to_bio:main',
                   'reannotation = eis1600.training_data.reannotation:main',
                   'reconstruct_texts = eis1600.json_to_text.reconstruct:main',
                   'sheets_topod_stats = eis1600.toponym_descriptions.topod_sheets_stats:main',
                   'show_input_files_sizes = eis1600.helper.files_sizes:main',
```

