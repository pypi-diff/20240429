# Comparing `tmp/pseudonymizer-0.1.6.tar.gz` & `tmp/pseudonymizer-0.1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pseudonymizer-0.1.6.tar", last modified: Mon Apr 29 14:54:50 2024, max compression
+gzip compressed data, was "pseudonymizer-0.1.7.tar", last modified: Mon Apr 29 15:04:25 2024, max compression
```

## Comparing `pseudonymizer-0.1.6.tar` & `pseudonymizer-0.1.7.tar`

### file list

```diff
@@ -1,66 +1,66 @@
-drwxr-xr-x   0 minjoo     (501) staff       (20)        0 2024-04-29 14:54:50.864333 pseudonymizer-0.1.6/
--rw-r--r--   0 minjoo     (501) staff       (20)     1082 2024-04-29 14:46:11.000000 pseudonymizer-0.1.6/LICENSE.txt
--rw-r--r--   0 minjoo     (501) staff       (20)    57516 2024-04-29 14:54:50.863396 pseudonymizer-0.1.6/PKG-INFO
--rw-r--r--   0 minjoo     (501) staff       (20)    57212 2024-04-29 13:13:22.000000 pseudonymizer-0.1.6/README.md
-drwxr-xr-x   0 minjoo     (501) staff       (20)        0 2024-04-29 14:54:50.776489 pseudonymizer-0.1.6/pseudonymizer/
--rw-r--r--   0 minjoo     (501) staff       (20)        1 2024-01-14 10:42:09.000000 pseudonymizer-0.1.6/pseudonymizer/__init__.py
--rw-r--r--   0 minjoo     (501) staff       (20)     3616 2024-04-21 07:22:03.000000 pseudonymizer-0.1.6/pseudonymizer/anonymizationSecurityMeasure.py
--rw-r--r--   0 minjoo     (501) staff       (20)     5589 2024-04-21 11:47:54.000000 pseudonymizer-0.1.6/pseudonymizer/createMappingTable.py
-drwxr-xr-x   0 minjoo     (501) staff       (20)        0 2024-04-29 14:54:50.784717 pseudonymizer-0.1.6/pseudonymizer/cryptocontainers/
--rw-r--r--   0 minjoo     (501) staff       (20)      603 2024-04-14 05:50:36.000000 pseudonymizer-0.1.6/pseudonymizer/cryptocontainers/DBContainer.py
--rw-r--r--   0 minjoo     (501) staff       (20)        0 2024-04-13 04:53:17.000000 pseudonymizer-0.1.6/pseudonymizer/cryptocontainers/__init__.py
--rw-r--r--   0 minjoo     (501) staff       (20)     1378 2024-04-14 05:50:36.000000 pseudonymizer-0.1.6/pseudonymizer/cryptocontainers/bundleKeyTable.py
--rw-r--r--   0 minjoo     (501) staff       (20)      855 2024-04-14 05:50:36.000000 pseudonymizer-0.1.6/pseudonymizer/cryptocontainers/bundleMainTable.py
--rw-r--r--   0 minjoo     (501) staff       (20)      755 2024-04-14 05:50:36.000000 pseudonymizer-0.1.6/pseudonymizer/cryptocontainers/bundleTables.py
--rw-r--r--   0 minjoo     (501) staff       (20)     1223 2024-04-14 05:50:36.000000 pseudonymizer-0.1.6/pseudonymizer/cryptocontainers/bundleTargetTable.py
-drwxr-xr-x   0 minjoo     (501) staff       (20)        0 2024-04-29 14:54:50.801957 pseudonymizer-0.1.6/pseudonymizer/deidentificationTechnique/
--rw-r--r--   0 minjoo     (501) staff       (20)        1 2024-01-14 10:42:09.000000 pseudonymizer-0.1.6/pseudonymizer/deidentificationTechnique/__init__.py
--rw-r--r--   0 minjoo     (501) staff       (20)     7458 2024-04-18 12:29:55.000000 pseudonymizer-0.1.6/pseudonymizer/deidentificationTechnique/differentialPrivacy.py
--rw-r--r--   0 minjoo     (501) staff       (20)     2211 2024-04-21 13:50:24.000000 pseudonymizer-0.1.6/pseudonymizer/deidentificationTechnique/equivalentClass.py
--rw-r--r--   0 minjoo     (501) staff       (20)     7270 2024-04-21 13:50:39.000000 pseudonymizer-0.1.6/pseudonymizer/deidentificationTechnique/gaussiandifferentialPrivacy.py
--rw-r--r--   0 minjoo     (501) staff       (20)     1530 2024-04-21 08:14:38.000000 pseudonymizer-0.1.6/pseudonymizer/deidentificationTechnique/kAnonymity.py
--rw-r--r--   0 minjoo     (501) staff       (20)     3582 2024-04-21 08:21:45.000000 pseudonymizer-0.1.6/pseudonymizer/deidentificationTechnique/lDiversity.py
--rw-r--r--   0 minjoo     (501) staff       (20)     4309 2024-04-21 08:34:19.000000 pseudonymizer-0.1.6/pseudonymizer/deidentificationTechnique/tClosenessFactor.py
--rw-r--r--   0 minjoo     (501) staff       (20)     5871 2024-04-21 08:32:00.000000 pseudonymizer-0.1.6/pseudonymizer/deidentificationTechnique/tClosenessNumeric.py
-drwxr-xr-x   0 minjoo     (501) staff       (20)        0 2024-04-29 14:54:50.809119 pseudonymizer-0.1.6/pseudonymizer/encryptionPseudonyms/
--rw-r--r--   0 minjoo     (501) staff       (20)        1 2024-02-25 06:39:57.000000 pseudonymizer-0.1.6/pseudonymizer/encryptionPseudonyms/__init__.py
--rw-r--r--   0 minjoo     (501) staff       (20)      573 2024-02-25 06:45:57.000000 pseudonymizer-0.1.6/pseudonymizer/encryptionPseudonyms/abstractPreprocessQuery.py
--rw-r--r--   0 minjoo     (501) staff       (20)     1244 2024-04-14 05:50:36.000000 pseudonymizer-0.1.6/pseudonymizer/encryptionPseudonyms/encrypttoKeyColumn.py
--rw-r--r--   0 minjoo     (501) staff       (20)     4229 2024-04-14 07:25:15.000000 pseudonymizer-0.1.6/pseudonymizer/encryptionPseudonyms/insertKeyintoMainTable.py
--rw-r--r--   0 minjoo     (501) staff       (20)     2932 2024-04-14 05:50:36.000000 pseudonymizer-0.1.6/pseudonymizer/encryptionPseudonyms/insertTargetintoMainTable.py
--rw-r--r--   0 minjoo     (501) staff       (20)     4361 2024-04-13 04:53:17.000000 pseudonymizer-0.1.6/pseudonymizer/encryptionPseudonyms/pyMySQLQuery.py
--rw-r--r--   0 minjoo     (501) staff       (20)     1885 2024-04-14 05:50:36.000000 pseudonymizer-0.1.6/pseudonymizer/encryptionPseudonyms/updateSerialNumColumn.py
-drwxr-xr-x   0 minjoo     (501) staff       (20)        0 2024-04-29 14:54:50.810006 pseudonymizer-0.1.6/pseudonymizer/examples/
--rw-r--r--   0 minjoo     (501) staff       (20)        1 2024-01-14 10:42:09.000000 pseudonymizer-0.1.6/pseudonymizer/examples/__init__.py
--rw-r--r--   0 minjoo     (501) staff       (20)     6332 2024-04-21 11:34:05.000000 pseudonymizer-0.1.6/pseudonymizer/extractJoinDatafromDB.py
--rw-r--r--   0 minjoo     (501) staff       (20)     5131 2024-04-21 11:52:41.000000 pseudonymizer-0.1.6/pseudonymizer/joinTargetTables.py
--rw-r--r--   0 minjoo     (501) staff       (20)     9509 2024-04-21 12:11:36.000000 pseudonymizer-0.1.6/pseudonymizer/privacyPreservingModels.py
--rw-r--r--   0 minjoo     (501) staff       (20)     5267 2024-04-21 13:36:57.000000 pseudonymizer-0.1.6/pseudonymizer/pseudonym.py
--rw-r--r--   0 minjoo     (501) staff       (20)     6157 2024-04-21 07:47:59.000000 pseudonymizer-0.1.6/pseudonymizer/pseudonymUtilityMeasure.py
--rw-r--r--   0 minjoo     (501) staff       (20)      434 2024-04-13 04:53:17.000000 pseudonymizer-0.1.6/pseudonymizer/pseudonymizer.py
-drwxr-xr-x   0 minjoo     (501) staff       (20)        0 2024-04-29 14:54:50.859079 pseudonymizer-0.1.6/pseudonymizer/pseudonymizers/
--rw-r--r--   0 minjoo     (501) staff       (20)        1 2024-01-14 10:42:09.000000 pseudonymizer-0.1.6/pseudonymizer/pseudonymizers/__init__.py
--rw-r--r--   0 minjoo     (501) staff       (20)     2292 2024-04-20 01:35:47.000000 pseudonymizer-0.1.6/pseudonymizer/pseudonymizers/addressMaskingModule.py
--rw-r--r--   0 minjoo     (501) staff       (20)     1609 2024-04-21 13:46:13.000000 pseudonymizer-0.1.6/pseudonymizer/pseudonymizers/businessNumMasking.py
--rw-r--r--   0 minjoo     (501) staff       (20)     4086 2024-04-21 12:55:26.000000 pseudonymizer-0.1.6/pseudonymizer/pseudonymizers/charcategorization.py
--rw-r--r--   0 minjoo     (501) staff       (20)     6215 2024-04-21 13:00:42.000000 pseudonymizer-0.1.6/pseudonymizer/pseudonymizers/columncategorization.py
--rw-r--r--   0 minjoo     (501) staff       (20)     2011 2024-04-19 12:17:36.000000 pseudonymizer-0.1.6/pseudonymizer/pseudonymizers/emailMasking.py
--rw-r--r--   0 minjoo     (501) staff       (20)     3319 2024-04-21 13:49:16.000000 pseudonymizer-0.1.6/pseudonymizer/pseudonymizers/maskingPseudonymizer.py
--rw-r--r--   0 minjoo     (501) staff       (20)     2894 2024-04-21 13:05:59.000000 pseudonymizer-0.1.6/pseudonymizer/pseudonymizers/microAggregation.py
--rw-r--r--   0 minjoo     (501) staff       (20)      612 2024-04-13 04:53:17.000000 pseudonymizer-0.1.6/pseudonymizer/pseudonymizers/nameMasking.py
--rw-r--r--   0 minjoo     (501) staff       (20)     5485 2024-04-21 13:14:51.000000 pseudonymizer-0.1.6/pseudonymizer/pseudonymizers/numcategorization.py
--rw-r--r--   0 minjoo     (501) staff       (20)     1627 2024-04-18 11:00:15.000000 pseudonymizer-0.1.6/pseudonymizer/pseudonymizers/phoneNumMasking.py
--rw-r--r--   0 minjoo     (501) staff       (20)     1707 2024-04-21 13:38:26.000000 pseudonymizer-0.1.6/pseudonymizer/pseudonymizers/randomRoundingPseudonymizer.py
--rw-r--r--   0 minjoo     (501) staff       (20)     1058 2024-04-21 13:49:47.000000 pseudonymizer-0.1.6/pseudonymizer/pseudonymizers/residentNumMasking.py
--rw-r--r--   0 minjoo     (501) staff       (20)     5739 2024-04-21 13:35:28.000000 pseudonymizer-0.1.6/pseudonymizer/pseudonymizers/topandBottomCoding.py
--rw-r--r--   0 minjoo     (501) staff       (20)     7340 2024-04-21 06:40:27.000000 pseudonymizer-0.1.6/pseudonymizer/updateEncryptedKeyIntoDB.py
-drwxr-xr-x   0 minjoo     (501) staff       (20)        0 2024-04-29 14:54:50.778702 pseudonymizer-0.1.6/pseudonymizer.egg-info/
--rw-r--r--   0 minjoo     (501) staff       (20)    57516 2024-04-29 14:54:50.000000 pseudonymizer-0.1.6/pseudonymizer.egg-info/PKG-INFO
--rw-r--r--   0 minjoo     (501) staff       (20)     2493 2024-04-29 14:54:50.000000 pseudonymizer-0.1.6/pseudonymizer.egg-info/SOURCES.txt
--rw-r--r--   0 minjoo     (501) staff       (20)        1 2024-04-29 14:54:50.000000 pseudonymizer-0.1.6/pseudonymizer.egg-info/dependency_links.txt
--rw-r--r--   0 minjoo     (501) staff       (20)       95 2024-04-29 14:54:50.000000 pseudonymizer-0.1.6/pseudonymizer.egg-info/requires.txt
--rw-r--r--   0 minjoo     (501) staff       (20)       20 2024-04-29 14:54:50.000000 pseudonymizer-0.1.6/pseudonymizer.egg-info/top_level.txt
--rw-r--r--   0 minjoo     (501) staff       (20)       38 2024-04-29 14:54:50.864447 pseudonymizer-0.1.6/setup.cfg
--rw-r--r--   0 minjoo     (501) staff       (20)     1122 2024-04-29 14:53:30.000000 pseudonymizer-0.1.6/setup.py
-drwxr-xr-x   0 minjoo     (501) staff       (20)        0 2024-04-29 14:54:50.860929 pseudonymizer-0.1.6/tests/
--rw-r--r--   0 minjoo     (501) staff       (20)        1 2024-01-14 10:42:09.000000 pseudonymizer-0.1.6/tests/__init__.py
+drwxr-xr-x   0 minjoo     (501) staff       (20)        0 2024-04-29 15:04:25.896632 pseudonymizer-0.1.7/
+-rw-r--r--   0 minjoo     (501) staff       (20)     1082 2024-04-29 14:46:11.000000 pseudonymizer-0.1.7/LICENSE.txt
+-rw-r--r--   0 minjoo     (501) staff       (20)    57516 2024-04-29 15:04:25.896058 pseudonymizer-0.1.7/PKG-INFO
+-rw-r--r--   0 minjoo     (501) staff       (20)    57212 2024-04-29 13:13:22.000000 pseudonymizer-0.1.7/README.md
+drwxr-xr-x   0 minjoo     (501) staff       (20)        0 2024-04-29 15:04:25.870708 pseudonymizer-0.1.7/pseudonymizer/
+-rw-r--r--   0 minjoo     (501) staff       (20)        1 2024-01-14 10:42:09.000000 pseudonymizer-0.1.7/pseudonymizer/__init__.py
+-rw-r--r--   0 minjoo     (501) staff       (20)     3616 2024-04-21 07:22:03.000000 pseudonymizer-0.1.7/pseudonymizer/anonymizationSecurityMeasure.py
+-rw-r--r--   0 minjoo     (501) staff       (20)     5589 2024-04-21 11:47:54.000000 pseudonymizer-0.1.7/pseudonymizer/createMappingTable.py
+drwxr-xr-x   0 minjoo     (501) staff       (20)        0 2024-04-29 15:04:25.876636 pseudonymizer-0.1.7/pseudonymizer/cryptocontainers/
+-rw-r--r--   0 minjoo     (501) staff       (20)      603 2024-04-14 05:50:36.000000 pseudonymizer-0.1.7/pseudonymizer/cryptocontainers/DBContainer.py
+-rw-r--r--   0 minjoo     (501) staff       (20)        0 2024-04-13 04:53:17.000000 pseudonymizer-0.1.7/pseudonymizer/cryptocontainers/__init__.py
+-rw-r--r--   0 minjoo     (501) staff       (20)     1378 2024-04-14 05:50:36.000000 pseudonymizer-0.1.7/pseudonymizer/cryptocontainers/bundleKeyTable.py
+-rw-r--r--   0 minjoo     (501) staff       (20)      855 2024-04-14 05:50:36.000000 pseudonymizer-0.1.7/pseudonymizer/cryptocontainers/bundleMainTable.py
+-rw-r--r--   0 minjoo     (501) staff       (20)      755 2024-04-14 05:50:36.000000 pseudonymizer-0.1.7/pseudonymizer/cryptocontainers/bundleTables.py
+-rw-r--r--   0 minjoo     (501) staff       (20)     1223 2024-04-14 05:50:36.000000 pseudonymizer-0.1.7/pseudonymizer/cryptocontainers/bundleTargetTable.py
+drwxr-xr-x   0 minjoo     (501) staff       (20)        0 2024-04-29 15:04:25.881951 pseudonymizer-0.1.7/pseudonymizer/deidentificationTechnique/
+-rw-r--r--   0 minjoo     (501) staff       (20)        1 2024-01-14 10:42:09.000000 pseudonymizer-0.1.7/pseudonymizer/deidentificationTechnique/__init__.py
+-rw-r--r--   0 minjoo     (501) staff       (20)     7458 2024-04-18 12:29:55.000000 pseudonymizer-0.1.7/pseudonymizer/deidentificationTechnique/differentialPrivacy.py
+-rw-r--r--   0 minjoo     (501) staff       (20)     2211 2024-04-21 13:50:24.000000 pseudonymizer-0.1.7/pseudonymizer/deidentificationTechnique/equivalentClass.py
+-rw-r--r--   0 minjoo     (501) staff       (20)     7270 2024-04-21 13:50:39.000000 pseudonymizer-0.1.7/pseudonymizer/deidentificationTechnique/gaussiandifferentialPrivacy.py
+-rw-r--r--   0 minjoo     (501) staff       (20)     1530 2024-04-21 08:14:38.000000 pseudonymizer-0.1.7/pseudonymizer/deidentificationTechnique/kAnonymity.py
+-rw-r--r--   0 minjoo     (501) staff       (20)     3582 2024-04-21 08:21:45.000000 pseudonymizer-0.1.7/pseudonymizer/deidentificationTechnique/lDiversity.py
+-rw-r--r--   0 minjoo     (501) staff       (20)     4309 2024-04-21 08:34:19.000000 pseudonymizer-0.1.7/pseudonymizer/deidentificationTechnique/tClosenessFactor.py
+-rw-r--r--   0 minjoo     (501) staff       (20)     5871 2024-04-21 08:32:00.000000 pseudonymizer-0.1.7/pseudonymizer/deidentificationTechnique/tClosenessNumeric.py
+drwxr-xr-x   0 minjoo     (501) staff       (20)        0 2024-04-29 15:04:25.885847 pseudonymizer-0.1.7/pseudonymizer/encryptionPseudonyms/
+-rw-r--r--   0 minjoo     (501) staff       (20)        1 2024-02-25 06:39:57.000000 pseudonymizer-0.1.7/pseudonymizer/encryptionPseudonyms/__init__.py
+-rw-r--r--   0 minjoo     (501) staff       (20)      573 2024-02-25 06:45:57.000000 pseudonymizer-0.1.7/pseudonymizer/encryptionPseudonyms/abstractPreprocessQuery.py
+-rw-r--r--   0 minjoo     (501) staff       (20)     1244 2024-04-14 05:50:36.000000 pseudonymizer-0.1.7/pseudonymizer/encryptionPseudonyms/encrypttoKeyColumn.py
+-rw-r--r--   0 minjoo     (501) staff       (20)     4229 2024-04-14 07:25:15.000000 pseudonymizer-0.1.7/pseudonymizer/encryptionPseudonyms/insertKeyintoMainTable.py
+-rw-r--r--   0 minjoo     (501) staff       (20)     2932 2024-04-14 05:50:36.000000 pseudonymizer-0.1.7/pseudonymizer/encryptionPseudonyms/insertTargetintoMainTable.py
+-rw-r--r--   0 minjoo     (501) staff       (20)     4361 2024-04-13 04:53:17.000000 pseudonymizer-0.1.7/pseudonymizer/encryptionPseudonyms/pyMySQLQuery.py
+-rw-r--r--   0 minjoo     (501) staff       (20)     1885 2024-04-14 05:50:36.000000 pseudonymizer-0.1.7/pseudonymizer/encryptionPseudonyms/updateSerialNumColumn.py
+drwxr-xr-x   0 minjoo     (501) staff       (20)        0 2024-04-29 15:04:25.886484 pseudonymizer-0.1.7/pseudonymizer/examples/
+-rw-r--r--   0 minjoo     (501) staff       (20)        1 2024-01-14 10:42:09.000000 pseudonymizer-0.1.7/pseudonymizer/examples/__init__.py
+-rw-r--r--   0 minjoo     (501) staff       (20)     6332 2024-04-21 11:34:05.000000 pseudonymizer-0.1.7/pseudonymizer/extractJoinDatafromDB.py
+-rw-r--r--   0 minjoo     (501) staff       (20)     5131 2024-04-21 11:52:41.000000 pseudonymizer-0.1.7/pseudonymizer/joinTargetTables.py
+-rw-r--r--   0 minjoo     (501) staff       (20)     9509 2024-04-21 12:11:36.000000 pseudonymizer-0.1.7/pseudonymizer/privacyPreservingModels.py
+-rw-r--r--   0 minjoo     (501) staff       (20)     5267 2024-04-21 13:36:57.000000 pseudonymizer-0.1.7/pseudonymizer/pseudonym.py
+-rw-r--r--   0 minjoo     (501) staff       (20)     6157 2024-04-21 07:47:59.000000 pseudonymizer-0.1.7/pseudonymizer/pseudonymUtilityMeasure.py
+-rw-r--r--   0 minjoo     (501) staff       (20)      434 2024-04-13 04:53:17.000000 pseudonymizer-0.1.7/pseudonymizer/pseudonymizer.py
+drwxr-xr-x   0 minjoo     (501) staff       (20)        0 2024-04-29 15:04:25.894866 pseudonymizer-0.1.7/pseudonymizer/pseudonymizers/
+-rw-r--r--   0 minjoo     (501) staff       (20)        1 2024-01-14 10:42:09.000000 pseudonymizer-0.1.7/pseudonymizer/pseudonymizers/__init__.py
+-rw-r--r--   0 minjoo     (501) staff       (20)     2292 2024-04-20 01:35:47.000000 pseudonymizer-0.1.7/pseudonymizer/pseudonymizers/addressMaskingModule.py
+-rw-r--r--   0 minjoo     (501) staff       (20)     1609 2024-04-21 13:46:13.000000 pseudonymizer-0.1.7/pseudonymizer/pseudonymizers/businessNumMasking.py
+-rw-r--r--   0 minjoo     (501) staff       (20)     4086 2024-04-21 12:55:26.000000 pseudonymizer-0.1.7/pseudonymizer/pseudonymizers/charcategorization.py
+-rw-r--r--   0 minjoo     (501) staff       (20)     6215 2024-04-21 13:00:42.000000 pseudonymizer-0.1.7/pseudonymizer/pseudonymizers/columncategorization.py
+-rw-r--r--   0 minjoo     (501) staff       (20)     2011 2024-04-19 12:17:36.000000 pseudonymizer-0.1.7/pseudonymizer/pseudonymizers/emailMasking.py
+-rw-r--r--   0 minjoo     (501) staff       (20)     3319 2024-04-21 13:49:16.000000 pseudonymizer-0.1.7/pseudonymizer/pseudonymizers/maskingPseudonymizer.py
+-rw-r--r--   0 minjoo     (501) staff       (20)     2894 2024-04-21 13:05:59.000000 pseudonymizer-0.1.7/pseudonymizer/pseudonymizers/microAggregation.py
+-rw-r--r--   0 minjoo     (501) staff       (20)      612 2024-04-13 04:53:17.000000 pseudonymizer-0.1.7/pseudonymizer/pseudonymizers/nameMasking.py
+-rw-r--r--   0 minjoo     (501) staff       (20)     5485 2024-04-21 13:14:51.000000 pseudonymizer-0.1.7/pseudonymizer/pseudonymizers/numcategorization.py
+-rw-r--r--   0 minjoo     (501) staff       (20)     1627 2024-04-18 11:00:15.000000 pseudonymizer-0.1.7/pseudonymizer/pseudonymizers/phoneNumMasking.py
+-rw-r--r--   0 minjoo     (501) staff       (20)     1707 2024-04-21 13:38:26.000000 pseudonymizer-0.1.7/pseudonymizer/pseudonymizers/randomRoundingPseudonymizer.py
+-rw-r--r--   0 minjoo     (501) staff       (20)     1058 2024-04-21 13:49:47.000000 pseudonymizer-0.1.7/pseudonymizer/pseudonymizers/residentNumMasking.py
+-rw-r--r--   0 minjoo     (501) staff       (20)     5739 2024-04-21 13:35:28.000000 pseudonymizer-0.1.7/pseudonymizer/pseudonymizers/topandBottomCoding.py
+-rw-r--r--   0 minjoo     (501) staff       (20)     7340 2024-04-21 06:40:27.000000 pseudonymizer-0.1.7/pseudonymizer/updateEncryptedKeyIntoDB.py
+drwxr-xr-x   0 minjoo     (501) staff       (20)        0 2024-04-29 15:04:25.873954 pseudonymizer-0.1.7/pseudonymizer.egg-info/
+-rw-r--r--   0 minjoo     (501) staff       (20)    57516 2024-04-29 15:04:25.000000 pseudonymizer-0.1.7/pseudonymizer.egg-info/PKG-INFO
+-rw-r--r--   0 minjoo     (501) staff       (20)     2493 2024-04-29 15:04:25.000000 pseudonymizer-0.1.7/pseudonymizer.egg-info/SOURCES.txt
+-rw-r--r--   0 minjoo     (501) staff       (20)        1 2024-04-29 15:04:25.000000 pseudonymizer-0.1.7/pseudonymizer.egg-info/dependency_links.txt
+-rw-r--r--   0 minjoo     (501) staff       (20)       95 2024-04-29 15:04:25.000000 pseudonymizer-0.1.7/pseudonymizer.egg-info/requires.txt
+-rw-r--r--   0 minjoo     (501) staff       (20)       20 2024-04-29 15:04:25.000000 pseudonymizer-0.1.7/pseudonymizer.egg-info/top_level.txt
+-rw-r--r--   0 minjoo     (501) staff       (20)       38 2024-04-29 15:04:25.896722 pseudonymizer-0.1.7/setup.cfg
+-rw-r--r--   0 minjoo     (501) staff       (20)     1129 2024-04-29 15:03:50.000000 pseudonymizer-0.1.7/setup.py
+drwxr-xr-x   0 minjoo     (501) staff       (20)        0 2024-04-29 15:04:25.895288 pseudonymizer-0.1.7/tests/
+-rw-r--r--   0 minjoo     (501) staff       (20)        1 2024-01-14 10:42:09.000000 pseudonymizer-0.1.7/tests/__init__.py
```

### Comparing `pseudonymizer-0.1.6/LICENSE.txt` & `pseudonymizer-0.1.7/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `pseudonymizer-0.1.6/PKG-INFO` & `pseudonymizer-0.1.7/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pseudonymizer
-Version: 0.1.6
+Version: 0.1.7
 Summary: pseudonymizer-to-protect-private-personal-data
 Home-page: https://github.com/ksydata/pseudonymizer
 Author: ksydata
 Author-email: ksydata01@gmail.com
 Requires-Python: >3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
```

### Comparing `pseudonymizer-0.1.6/README.md` & `pseudonymizer-0.1.7/README.md`

 * *Files identical despite different names*

### Comparing `pseudonymizer-0.1.6/pseudonymizer/anonymizationSecurityMeasure.py` & `pseudonymizer-0.1.7/pseudonymizer/anonymizationSecurityMeasure.py`

 * *Files identical despite different names*

### Comparing `pseudonymizer-0.1.6/pseudonymizer/createMappingTable.py` & `pseudonymizer-0.1.7/pseudonymizer/createMappingTable.py`

 * *Files identical despite different names*

### Comparing `pseudonymizer-0.1.6/pseudonymizer/cryptocontainers/DBContainer.py` & `pseudonymizer-0.1.7/pseudonymizer/cryptocontainers/DBContainer.py`

 * *Files identical despite different names*

### Comparing `pseudonymizer-0.1.6/pseudonymizer/cryptocontainers/bundleKeyTable.py` & `pseudonymizer-0.1.7/pseudonymizer/cryptocontainers/bundleKeyTable.py`

 * *Files identical despite different names*

### Comparing `pseudonymizer-0.1.6/pseudonymizer/cryptocontainers/bundleMainTable.py` & `pseudonymizer-0.1.7/pseudonymizer/cryptocontainers/bundleMainTable.py`

 * *Files identical despite different names*

### Comparing `pseudonymizer-0.1.6/pseudonymizer/cryptocontainers/bundleTables.py` & `pseudonymizer-0.1.7/pseudonymizer/cryptocontainers/bundleTables.py`

 * *Files identical despite different names*

### Comparing `pseudonymizer-0.1.6/pseudonymizer/cryptocontainers/bundleTargetTable.py` & `pseudonymizer-0.1.7/pseudonymizer/cryptocontainers/bundleTargetTable.py`

 * *Files identical despite different names*

### Comparing `pseudonymizer-0.1.6/pseudonymizer/deidentificationTechnique/differentialPrivacy.py` & `pseudonymizer-0.1.7/pseudonymizer/deidentificationTechnique/differentialPrivacy.py`

 * *Files identical despite different names*

### Comparing `pseudonymizer-0.1.6/pseudonymizer/deidentificationTechnique/equivalentClass.py` & `pseudonymizer-0.1.7/pseudonymizer/deidentificationTechnique/equivalentClass.py`

 * *Files identical despite different names*

### Comparing `pseudonymizer-0.1.6/pseudonymizer/deidentificationTechnique/gaussiandifferentialPrivacy.py` & `pseudonymizer-0.1.7/pseudonymizer/deidentificationTechnique/gaussiandifferentialPrivacy.py`

 * *Files identical despite different names*

### Comparing `pseudonymizer-0.1.6/pseudonymizer/deidentificationTechnique/kAnonymity.py` & `pseudonymizer-0.1.7/pseudonymizer/deidentificationTechnique/kAnonymity.py`

 * *Files identical despite different names*

### Comparing `pseudonymizer-0.1.6/pseudonymizer/deidentificationTechnique/lDiversity.py` & `pseudonymizer-0.1.7/pseudonymizer/deidentificationTechnique/lDiversity.py`

 * *Files identical despite different names*

### Comparing `pseudonymizer-0.1.6/pseudonymizer/deidentificationTechnique/tClosenessFactor.py` & `pseudonymizer-0.1.7/pseudonymizer/deidentificationTechnique/tClosenessFactor.py`

 * *Files identical despite different names*

### Comparing `pseudonymizer-0.1.6/pseudonymizer/deidentificationTechnique/tClosenessNumeric.py` & `pseudonymizer-0.1.7/pseudonymizer/deidentificationTechnique/tClosenessNumeric.py`

 * *Files identical despite different names*

### Comparing `pseudonymizer-0.1.6/pseudonymizer/encryptionPseudonyms/abstractPreprocessQuery.py` & `pseudonymizer-0.1.7/pseudonymizer/encryptionPseudonyms/abstractPreprocessQuery.py`

 * *Files identical despite different names*

### Comparing `pseudonymizer-0.1.6/pseudonymizer/encryptionPseudonyms/encrypttoKeyColumn.py` & `pseudonymizer-0.1.7/pseudonymizer/encryptionPseudonyms/encrypttoKeyColumn.py`

 * *Files identical despite different names*

### Comparing `pseudonymizer-0.1.6/pseudonymizer/encryptionPseudonyms/insertKeyintoMainTable.py` & `pseudonymizer-0.1.7/pseudonymizer/encryptionPseudonyms/insertKeyintoMainTable.py`

 * *Files identical despite different names*

### Comparing `pseudonymizer-0.1.6/pseudonymizer/encryptionPseudonyms/insertTargetintoMainTable.py` & `pseudonymizer-0.1.7/pseudonymizer/encryptionPseudonyms/insertTargetintoMainTable.py`

 * *Files identical despite different names*

### Comparing `pseudonymizer-0.1.6/pseudonymizer/encryptionPseudonyms/pyMySQLQuery.py` & `pseudonymizer-0.1.7/pseudonymizer/encryptionPseudonyms/pyMySQLQuery.py`

 * *Files identical despite different names*

### Comparing `pseudonymizer-0.1.6/pseudonymizer/encryptionPseudonyms/updateSerialNumColumn.py` & `pseudonymizer-0.1.7/pseudonymizer/encryptionPseudonyms/updateSerialNumColumn.py`

 * *Files identical despite different names*

### Comparing `pseudonymizer-0.1.6/pseudonymizer/extractJoinDatafromDB.py` & `pseudonymizer-0.1.7/pseudonymizer/extractJoinDatafromDB.py`

 * *Files identical despite different names*

### Comparing `pseudonymizer-0.1.6/pseudonymizer/joinTargetTables.py` & `pseudonymizer-0.1.7/pseudonymizer/joinTargetTables.py`

 * *Files identical despite different names*

### Comparing `pseudonymizer-0.1.6/pseudonymizer/privacyPreservingModels.py` & `pseudonymizer-0.1.7/pseudonymizer/privacyPreservingModels.py`

 * *Files identical despite different names*

### Comparing `pseudonymizer-0.1.6/pseudonymizer/pseudonym.py` & `pseudonymizer-0.1.7/pseudonymizer/pseudonym.py`

 * *Files identical despite different names*

### Comparing `pseudonymizer-0.1.6/pseudonymizer/pseudonymUtilityMeasure.py` & `pseudonymizer-0.1.7/pseudonymizer/pseudonymUtilityMeasure.py`

 * *Files identical despite different names*

### Comparing `pseudonymizer-0.1.6/pseudonymizer/pseudonymizers/addressMaskingModule.py` & `pseudonymizer-0.1.7/pseudonymizer/pseudonymizers/addressMaskingModule.py`

 * *Files identical despite different names*

### Comparing `pseudonymizer-0.1.6/pseudonymizer/pseudonymizers/businessNumMasking.py` & `pseudonymizer-0.1.7/pseudonymizer/pseudonymizers/businessNumMasking.py`

 * *Files identical despite different names*

### Comparing `pseudonymizer-0.1.6/pseudonymizer/pseudonymizers/charcategorization.py` & `pseudonymizer-0.1.7/pseudonymizer/pseudonymizers/charcategorization.py`

 * *Files identical despite different names*

### Comparing `pseudonymizer-0.1.6/pseudonymizer/pseudonymizers/columncategorization.py` & `pseudonymizer-0.1.7/pseudonymizer/pseudonymizers/columncategorization.py`

 * *Files identical despite different names*

### Comparing `pseudonymizer-0.1.6/pseudonymizer/pseudonymizers/emailMasking.py` & `pseudonymizer-0.1.7/pseudonymizer/pseudonymizers/emailMasking.py`

 * *Files identical despite different names*

### Comparing `pseudonymizer-0.1.6/pseudonymizer/pseudonymizers/maskingPseudonymizer.py` & `pseudonymizer-0.1.7/pseudonymizer/pseudonymizers/maskingPseudonymizer.py`

 * *Files identical despite different names*

### Comparing `pseudonymizer-0.1.6/pseudonymizer/pseudonymizers/microAggregation.py` & `pseudonymizer-0.1.7/pseudonymizer/pseudonymizers/microAggregation.py`

 * *Files identical despite different names*

### Comparing `pseudonymizer-0.1.6/pseudonymizer/pseudonymizers/nameMasking.py` & `pseudonymizer-0.1.7/pseudonymizer/pseudonymizers/nameMasking.py`

 * *Files identical despite different names*

### Comparing `pseudonymizer-0.1.6/pseudonymizer/pseudonymizers/numcategorization.py` & `pseudonymizer-0.1.7/pseudonymizer/pseudonymizers/numcategorization.py`

 * *Files identical despite different names*

### Comparing `pseudonymizer-0.1.6/pseudonymizer/pseudonymizers/phoneNumMasking.py` & `pseudonymizer-0.1.7/pseudonymizer/pseudonymizers/phoneNumMasking.py`

 * *Files identical despite different names*

### Comparing `pseudonymizer-0.1.6/pseudonymizer/pseudonymizers/randomRoundingPseudonymizer.py` & `pseudonymizer-0.1.7/pseudonymizer/pseudonymizers/randomRoundingPseudonymizer.py`

 * *Files identical despite different names*

### Comparing `pseudonymizer-0.1.6/pseudonymizer/pseudonymizers/residentNumMasking.py` & `pseudonymizer-0.1.7/pseudonymizer/pseudonymizers/residentNumMasking.py`

 * *Files identical despite different names*

### Comparing `pseudonymizer-0.1.6/pseudonymizer/pseudonymizers/topandBottomCoding.py` & `pseudonymizer-0.1.7/pseudonymizer/pseudonymizers/topandBottomCoding.py`

 * *Files identical despite different names*

### Comparing `pseudonymizer-0.1.6/pseudonymizer/updateEncryptedKeyIntoDB.py` & `pseudonymizer-0.1.7/pseudonymizer/updateEncryptedKeyIntoDB.py`

 * *Files identical despite different names*

### Comparing `pseudonymizer-0.1.6/pseudonymizer.egg-info/PKG-INFO` & `pseudonymizer-0.1.7/pseudonymizer.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pseudonymizer
-Version: 0.1.6
+Version: 0.1.7
 Summary: pseudonymizer-to-protect-private-personal-data
 Home-page: https://github.com/ksydata/pseudonymizer
 Author: ksydata
 Author-email: ksydata01@gmail.com
 Requires-Python: >3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
```

### Comparing `pseudonymizer-0.1.6/pseudonymizer.egg-info/SOURCES.txt` & `pseudonymizer-0.1.7/pseudonymizer.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pseudonymizer-0.1.6/setup.py` & `pseudonymizer-0.1.7/setup.py`

 * *Files 7% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 
 with open("README.md", "r", encoding = "utf-8") as fh:
           long_description = fh.read()
 # 모듈에서 사용가능한 함수의 목록
         
 setuptools.setup(
     name = "pseudonymizer",
-    version = "0.1.6",
+    version = "0.1.7",
     author = "ksydata",
     author_email = "ksydata01@gmail.com",
     description = "pseudonymizer-to-protect-private-personal-data",
     long_description = open("README.md").read(),
     long_description_content_type = "text/markdown",
     url = "https://github.com/ksydata/pseudonymizer",
     # 모듈 의존성 관리
@@ -23,12 +23,12 @@
         "numpy==1.22.3",
         "scipy==1.10.0", 
         "setuptools==63.4.1",
         "prettytable==3.9.0",
     ],
     # extras_require={"":[]},
     # 필요한 dependencies를 설치하기 위해 requirements.txt를 만드는 것
-    package_data = {"":["LICENSE.txt"]},
+    package_data = {"License":["LICENSE.txt"]},
     include_package_data = True,
     packages = setuptools.find_packages(),
     python_requires = ">3.6"
 )
```

