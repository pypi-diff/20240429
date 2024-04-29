# Comparing `tmp/mitos-2.1.8.tar.gz` & `tmp/mitos-2.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/mitos-2.1.8.tar", last modified: Thu Mar 21 08:49:00 2024, max compression
+gzip compressed data, was "dist/mitos-2.1.9.tar", last modified: Mon Apr 29 16:59:51 2024, max compression
```

## Comparing `mitos-2.1.8.tar` & `mitos-2.1.9.tar`

### file list

```diff
@@ -1,112 +1,112 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-21 08:49:00.000000 mitos-2.1.8/
--rw-rw-rw-   0 root         (0) root         (0)     1071 2024-03-21 08:48:53.000000 mitos-2.1.8/LICENSE
--rw-rw-rw-   0 root         (0) root         (0)      102 2024-03-21 08:48:53.000000 mitos-2.1.8/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)      801 2024-03-21 08:49:00.000000 mitos-2.1.8/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)     1316 2024-03-21 08:48:53.000000 mitos-2.1.8/README.md
--rw-rw-rw-   0 root         (0) root         (0)    12817 2024-03-21 08:48:53.000000 mitos-2.1.8/analyse.py
--rwxrwxrwx   0 root         (0) root         (0)     1016 2024-03-21 08:48:53.000000 mitos-2.1.8/drawmitos.py
--rw-rw-rw-   0 root         (0) root         (0)     8395 2024-03-21 08:48:53.000000 mitos-2.1.8/gcpp.py
--rwxrwxrwx   0 root         (0) root         (0)    15758 2024-03-21 08:48:53.000000 mitos-2.1.8/geneorder.py
--rwxrwxrwx   0 root         (0) root         (0)     7477 2024-03-21 08:48:53.000000 mitos-2.1.8/getfeatures.py
--rwxrwxrwx   0 root         (0) root         (0)     2926 2024-03-21 08:48:53.000000 mitos-2.1.8/getinfo.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-21 08:49:00.000000 mitos-2.1.8/mitos/
--rw-rw-rw-   0 root         (0) root         (0)     4383 2024-03-21 08:48:53.000000 mitos-2.1.8/mitos/CONFIG.py
--rw-rw-rw-   0 root         (0) root         (0)      244 2024-03-21 08:48:53.000000 mitos-2.1.8/mitos/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-21 08:49:00.000000 mitos-2.1.8/mitos/bedfile/
--rwxrwxrwx   0 root         (0) root         (0)     4222 2024-03-21 08:48:53.000000 mitos-2.1.8/mitos/bedfile/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-21 08:49:00.000000 mitos-2.1.8/mitos/blast/
--rw-rw-rw-   0 root         (0) root         (0)    85100 2024-03-21 08:48:53.000000 mitos-2.1.8/mitos/blast/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     6996 2024-03-21 08:48:53.000000 mitos-2.1.8/mitos/booreparser.py
--rw-rw-rw-   0 root         (0) root         (0)     2699 2024-03-21 08:48:53.000000 mitos-2.1.8/mitos/cmsearch_parse_separate.py
--rw-rw-rw-   0 root         (0) root         (0)     2286 2024-03-21 08:48:53.000000 mitos-2.1.8/mitos/codoncount.py
--rw-rw-rw-   0 root         (0) root         (0)    28739 2024-03-21 08:48:53.000000 mitos-2.1.8/mitos/convert_tree.py
--rw-rw-rw-   0 root         (0) root         (0)    11347 2024-03-21 08:48:53.000000 mitos-2.1.8/mitos/create_prot_fasta.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-21 08:49:00.000000 mitos-2.1.8/mitos/draw/
--rw-rw-rw-   0 root         (0) root         (0)     5348 2024-03-21 08:48:53.000000 mitos-2.1.8/mitos/draw/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-21 08:49:00.000000 mitos-2.1.8/mitos/extprog/
--rw-rw-rw-   0 root         (0) root         (0)     6149 2024-03-21 08:48:53.000000 mitos-2.1.8/mitos/extprog/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-21 08:49:00.000000 mitos-2.1.8/mitos/feature/
--rwxrwxrwx   0 root         (0) root         (0)    44233 2024-03-21 08:48:53.000000 mitos-2.1.8/mitos/feature/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-21 08:49:00.000000 mitos-2.1.8/mitos/gb/
--rw-rw-rw-   0 root         (0) root         (0)    45550 2024-03-21 08:48:53.000000 mitos-2.1.8/mitos/gb/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    11845 2024-03-21 08:48:53.000000 mitos-2.1.8/mitos/gb/unify.py
--rw-rw-rw-   0 root         (0) root         (0)     4366 2024-03-21 08:48:53.000000 mitos-2.1.8/mitos/get-wancy.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-21 08:49:00.000000 mitos-2.1.8/mitos/gfffile/
--rwxrwxrwx   0 root         (0) root         (0)     1045 2024-03-21 08:48:53.000000 mitos-2.1.8/mitos/gfffile/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    10004 2024-03-21 08:48:53.000000 mitos-2.1.8/mitos/inihit.py
--rw-rw-rw-   0 root         (0) root         (0)     6318 2024-03-21 08:48:53.000000 mitos-2.1.8/mitos/merge_results.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-21 08:49:00.000000 mitos-2.1.8/mitos/mergefeature/
--rw-rw-rw-   0 root         (0) root         (0)    26160 2024-03-21 08:48:53.000000 mitos-2.1.8/mitos/mergefeature/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-21 08:49:00.000000 mitos-2.1.8/mitos/mitfi/
--rwxrwxrwx   0 root         (0) root         (0)    19962 2024-03-21 08:48:53.000000 mitos-2.1.8/mitos/mitfi/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-21 08:49:00.000000 mitos-2.1.8/mitos/mitfi/parser/
--rw-rw-rw-   0 root         (0) root         (0)     4745 2024-03-21 08:48:53.000000 mitos-2.1.8/mitos/mitfi/parser/improve_infernal_structure.jar
--rw-rw-rw-   0 root         (0) root         (0)    11747 2024-03-21 08:48:53.000000 mitos-2.1.8/mitos/mitfi/parser/mitfiGeneticCodes
--rw-rw-rw-   0 root         (0) root         (0)    29220 2024-03-21 08:48:53.000000 mitos-2.1.8/mitos/mitfi/parser/mitfi_import-1.1.jar
--rw-rw-rw-   0 root         (0) root         (0)    29864 2024-03-21 08:48:53.000000 mitos-2.1.8/mitos/mitfi/parser/mitfi_import-1.1.jar.old
--rw-rw-rw-   0 root         (0) root         (0)    28131 2024-03-21 08:48:53.000000 mitos-2.1.8/mitos/mitfi/parser/mitfi_import-1.1.jar.org
--rw-rw-rw-   0 root         (0) root         (0)    28944 2024-03-21 08:48:53.000000 mitos-2.1.8/mitos/mitfi/parser/mitfi_import-1.1.jar.org.pre-circ
--rw-rw-rw-   0 root         (0) root         (0)    29197 2024-03-21 08:48:53.000000 mitos-2.1.8/mitos/mitfi/parser/mitfi_import.jar
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-21 08:49:00.000000 mitos-2.1.8/mitos/mito/
--rw-rw-rw-   0 root         (0) root         (0)     5074 2024-03-21 08:48:53.000000 mitos-2.1.8/mitos/mito/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    60417 2024-03-21 08:48:53.000000 mitos-2.1.8/mitos/mitoch_revisions.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-21 08:49:00.000000 mitos-2.1.8/mitos/mitofile/
--rw-rw-rw-   0 root         (0) root         (0)     5272 2024-03-21 08:48:53.000000 mitos-2.1.8/mitos/mitofile/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     4327 2024-03-21 08:48:53.000000 mitos-2.1.8/mitos/mitoloc.py
--rw-rw-rw-   0 root         (0) root         (0)    16081 2024-03-21 08:48:53.000000 mitos-2.1.8/mitos/mitos-extension.py
--rw-rw-rw-   0 root         (0) root         (0)    13698 2024-03-21 08:48:53.000000 mitos-2.1.8/mitos/mitos-extension2.py
--rw-rw-rw-   0 root         (0) root         (0)     2100 2024-03-21 08:48:53.000000 mitos-2.1.8/mitos/mumcmp.py
--rw-rw-rw-   0 root         (0) root         (0)      829 2024-03-21 08:48:53.000000 mitos-2.1.8/mitos/names.py
--rw-rw-rw-   0 root         (0) root         (0)     3009 2024-03-21 08:48:53.000000 mitos-2.1.8/mitos/ogre-geneorder.py
--rwxrwxrwx   0 root         (0) root         (0)     3043 2024-03-21 08:48:53.000000 mitos-2.1.8/mitos/plotprot.R
--rwxrwxrwx   0 root         (0) root         (0)     2538 2024-03-21 08:48:53.000000 mitos-2.1.8/mitos/plotrna.R
--rwxrwxrwx   0 root         (0) root         (0)     4391 2024-03-21 08:48:53.000000 mitos-2.1.8/mitos/plotstst.R
--rw-rw-rw-   0 root         (0) root         (0)     3186 2024-03-21 08:48:53.000000 mitos-2.1.8/mitos/prepareFiles.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-21 08:49:00.000000 mitos-2.1.8/mitos/protfeat/
--rw-rw-rw-   0 root         (0) root         (0)    27133 2024-03-21 08:48:53.000000 mitos-2.1.8/mitos/protfeat/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1426 2024-03-21 08:48:53.000000 mitos-2.1.8/mitos/removegene.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-21 08:49:00.000000 mitos-2.1.8/mitos/rna/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-03-21 08:48:53.000000 mitos-2.1.8/mitos/rna/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     4119 2024-03-21 08:48:53.000000 mitos-2.1.8/mitos/rna/forester.py
--rw-rw-rw-   0 root         (0) root         (0)     1446 2024-03-21 08:48:53.000000 mitos-2.1.8/mitos/rna/vienna.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-21 08:49:00.000000 mitos-2.1.8/mitos/sequence/
--rw-rw-rw-   0 root         (0) root         (0)    16807 2024-03-21 08:48:53.000000 mitos-2.1.8/mitos/sequence/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1487 2024-03-21 08:48:53.000000 mitos-2.1.8/mitos/sequence/degenerate.py
--rw-rw-rw-   0 root         (0) root         (0)    14519 2024-03-21 08:48:53.000000 mitos-2.1.8/mitos/skew.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-21 08:49:00.000000 mitos-2.1.8/mitos/tax/
--rw-rw-rw-   0 root         (0) root         (0)     3602 2024-03-21 08:48:53.000000 mitos-2.1.8/mitos/tax/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-21 08:49:00.000000 mitos-2.1.8/mitos/tbl/
--rw-rw-rw-   0 root         (0) root         (0)     5004 2024-03-21 08:48:53.000000 mitos-2.1.8/mitos/tbl/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-21 08:49:00.000000 mitos-2.1.8/mitos/trna/
--rw-rw-rw-   0 root         (0) root         (0)     4278 2024-03-21 08:48:53.000000 mitos-2.1.8/mitos/trna/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     8984 2024-03-21 08:48:53.000000 mitos-2.1.8/mitos/trna/arwenscan.py
--rw-rw-rw-   0 root         (0) root         (0)    11962 2024-03-21 08:48:53.000000 mitos-2.1.8/mitos/trna/trnascan.py
--rw-rw-rw-   0 root         (0) root         (0)   157352 2024-03-21 08:48:53.000000 mitos-2.1.8/mitos/trna-cm.py
--rw-rw-rw-   0 root         (0) root         (0)    23410 2024-03-21 08:48:53.000000 mitos-2.1.8/mitos/trnadist.py
--rw-rw-rw-   0 root         (0) root         (0)     4917 2024-03-21 08:48:53.000000 mitos-2.1.8/mitos/trnascan_parse_separate.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-21 08:49:00.000000 mitos-2.1.8/mitos/update/
--rw-rw-rw-   0 root         (0) root         (0)    25529 2024-03-21 08:48:53.000000 mitos-2.1.8/mitos/update/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     4823 2024-03-21 08:48:53.000000 mitos-2.1.8/mitos/update-mitolog.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-21 08:49:00.000000 mitos-2.1.8/mitos/util/
--rw-rw-rw-   0 root         (0) root         (0)      660 2024-03-21 08:48:53.000000 mitos-2.1.8/mitos/util/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-21 08:49:00.000000 mitos-2.1.8/mitos/webserver/
--rw-rw-rw-   0 root         (0) root         (0)    10152 2024-03-21 08:48:53.000000 mitos-2.1.8/mitos/webserver/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    26961 2024-03-21 08:48:53.000000 mitos-2.1.8/mitos/webserver/help.txt
--rwxrwxrwx   0 root         (0) root         (0)      785 2024-03-21 08:48:53.000000 mitos-2.1.8/mitos/webserver/history.txt
--rw-rw-rw-   0 root         (0) root         (0)     6691 2024-03-21 08:48:53.000000 mitos-2.1.8/mitos/webserver/index.txt
--rw-rw-rw-   0 root         (0) root         (0)      541 2024-03-21 08:48:53.000000 mitos-2.1.8/mitos/webserver/news.txt
--rw-rw-rw-   0 root         (0) root         (0)     3686 2024-03-21 08:48:53.000000 mitos-2.1.8/mitos/webserver/upload.txt
--rw-rw-rw-   0 root         (0) root         (0)      439 2024-03-21 08:48:53.000000 mitos-2.1.8/mitos/webserver/wait.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-21 08:49:00.000000 mitos-2.1.8/mitos.egg-info/
--rw-r--r--   0 root         (0) root         (0)      801 2024-03-21 08:49:00.000000 mitos-2.1.8/mitos.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1983 2024-03-21 08:49:00.000000 mitos-2.1.8/mitos.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-03-21 08:49:00.000000 mitos-2.1.8/mitos.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       16 2024-03-21 08:49:00.000000 mitos-2.1.8/mitos.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        6 2024-03-21 08:49:00.000000 mitos-2.1.8/mitos.egg-info/top_level.txt
--rwxrwxrwx   0 root         (0) root         (0)     1654 2024-03-21 08:48:53.000000 mitos-2.1.8/refseqsplit.py
--rwxrwxrwx   0 root         (0) root         (0)    46181 2024-03-21 08:48:53.000000 mitos-2.1.8/runmitos.py
--rw-rw-rw-   0 root         (0) root         (0)      280 2024-03-21 08:49:00.000000 mitos-2.1.8/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)     1391 2024-03-21 08:48:53.000000 mitos-2.1.8/setup.py
--rwxrwxrwx   0 root         (0) root         (0)     9153 2024-03-21 08:48:53.000000 mitos-2.1.8/subseq.py
--rwxrwxrwx   0 root         (0) root         (0)     4277 2024-03-21 08:48:53.000000 mitos-2.1.8/taxtree.py
--rw-rw-rw-   0 root         (0) root         (0)     2485 2024-03-21 08:48:53.000000 mitos-2.1.8/update-blastdb.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-29 16:59:51.000000 mitos-2.1.9/
+-rw-rw-rw-   0 root         (0) root         (0)     1071 2024-04-29 16:59:43.000000 mitos-2.1.9/LICENSE
+-rw-rw-rw-   0 root         (0) root         (0)      102 2024-04-29 16:59:43.000000 mitos-2.1.9/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)      801 2024-04-29 16:59:51.000000 mitos-2.1.9/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)     1316 2024-04-29 16:59:43.000000 mitos-2.1.9/README.md
+-rw-rw-rw-   0 root         (0) root         (0)    12817 2024-04-29 16:59:43.000000 mitos-2.1.9/analyse.py
+-rwxrwxrwx   0 root         (0) root         (0)     1016 2024-04-29 16:59:43.000000 mitos-2.1.9/drawmitos.py
+-rw-rw-rw-   0 root         (0) root         (0)     8395 2024-04-29 16:59:43.000000 mitos-2.1.9/gcpp.py
+-rwxrwxrwx   0 root         (0) root         (0)    15758 2024-04-29 16:59:43.000000 mitos-2.1.9/geneorder.py
+-rwxrwxrwx   0 root         (0) root         (0)     7477 2024-04-29 16:59:43.000000 mitos-2.1.9/getfeatures.py
+-rwxrwxrwx   0 root         (0) root         (0)     2926 2024-04-29 16:59:43.000000 mitos-2.1.9/getinfo.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-29 16:59:51.000000 mitos-2.1.9/mitos/
+-rw-rw-rw-   0 root         (0) root         (0)     4383 2024-04-29 16:59:43.000000 mitos-2.1.9/mitos/CONFIG.py
+-rw-rw-rw-   0 root         (0) root         (0)      244 2024-04-29 16:59:43.000000 mitos-2.1.9/mitos/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-29 16:59:51.000000 mitos-2.1.9/mitos/bedfile/
+-rwxrwxrwx   0 root         (0) root         (0)     4222 2024-04-29 16:59:43.000000 mitos-2.1.9/mitos/bedfile/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-29 16:59:51.000000 mitos-2.1.9/mitos/blast/
+-rw-rw-rw-   0 root         (0) root         (0)    85100 2024-04-29 16:59:43.000000 mitos-2.1.9/mitos/blast/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     6996 2024-04-29 16:59:43.000000 mitos-2.1.9/mitos/booreparser.py
+-rw-rw-rw-   0 root         (0) root         (0)     2699 2024-04-29 16:59:43.000000 mitos-2.1.9/mitos/cmsearch_parse_separate.py
+-rw-rw-rw-   0 root         (0) root         (0)     2286 2024-04-29 16:59:43.000000 mitos-2.1.9/mitos/codoncount.py
+-rw-rw-rw-   0 root         (0) root         (0)    28739 2024-04-29 16:59:43.000000 mitos-2.1.9/mitos/convert_tree.py
+-rw-rw-rw-   0 root         (0) root         (0)    11347 2024-04-29 16:59:43.000000 mitos-2.1.9/mitos/create_prot_fasta.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-29 16:59:51.000000 mitos-2.1.9/mitos/draw/
+-rw-rw-rw-   0 root         (0) root         (0)     5348 2024-04-29 16:59:43.000000 mitos-2.1.9/mitos/draw/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-29 16:59:51.000000 mitos-2.1.9/mitos/extprog/
+-rw-rw-rw-   0 root         (0) root         (0)     6149 2024-04-29 16:59:43.000000 mitos-2.1.9/mitos/extprog/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-29 16:59:51.000000 mitos-2.1.9/mitos/feature/
+-rwxrwxrwx   0 root         (0) root         (0)    44285 2024-04-29 16:59:43.000000 mitos-2.1.9/mitos/feature/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-29 16:59:51.000000 mitos-2.1.9/mitos/gb/
+-rw-rw-rw-   0 root         (0) root         (0)    45550 2024-04-29 16:59:43.000000 mitos-2.1.9/mitos/gb/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    11845 2024-04-29 16:59:43.000000 mitos-2.1.9/mitos/gb/unify.py
+-rw-rw-rw-   0 root         (0) root         (0)     4366 2024-04-29 16:59:43.000000 mitos-2.1.9/mitos/get-wancy.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-29 16:59:51.000000 mitos-2.1.9/mitos/gfffile/
+-rwxrwxrwx   0 root         (0) root         (0)     1045 2024-04-29 16:59:43.000000 mitos-2.1.9/mitos/gfffile/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    10004 2024-04-29 16:59:43.000000 mitos-2.1.9/mitos/inihit.py
+-rw-rw-rw-   0 root         (0) root         (0)     6318 2024-04-29 16:59:43.000000 mitos-2.1.9/mitos/merge_results.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-29 16:59:51.000000 mitos-2.1.9/mitos/mergefeature/
+-rw-rw-rw-   0 root         (0) root         (0)    26160 2024-04-29 16:59:43.000000 mitos-2.1.9/mitos/mergefeature/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-29 16:59:51.000000 mitos-2.1.9/mitos/mitfi/
+-rwxrwxrwx   0 root         (0) root         (0)    19962 2024-04-29 16:59:43.000000 mitos-2.1.9/mitos/mitfi/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-29 16:59:51.000000 mitos-2.1.9/mitos/mitfi/parser/
+-rw-rw-rw-   0 root         (0) root         (0)     4745 2024-04-29 16:59:43.000000 mitos-2.1.9/mitos/mitfi/parser/improve_infernal_structure.jar
+-rw-rw-rw-   0 root         (0) root         (0)    11747 2024-04-29 16:59:43.000000 mitos-2.1.9/mitos/mitfi/parser/mitfiGeneticCodes
+-rw-rw-rw-   0 root         (0) root         (0)    29220 2024-04-29 16:59:43.000000 mitos-2.1.9/mitos/mitfi/parser/mitfi_import-1.1.jar
+-rw-rw-rw-   0 root         (0) root         (0)    29864 2024-04-29 16:59:43.000000 mitos-2.1.9/mitos/mitfi/parser/mitfi_import-1.1.jar.old
+-rw-rw-rw-   0 root         (0) root         (0)    28131 2024-04-29 16:59:43.000000 mitos-2.1.9/mitos/mitfi/parser/mitfi_import-1.1.jar.org
+-rw-rw-rw-   0 root         (0) root         (0)    28944 2024-04-29 16:59:43.000000 mitos-2.1.9/mitos/mitfi/parser/mitfi_import-1.1.jar.org.pre-circ
+-rw-rw-rw-   0 root         (0) root         (0)    29197 2024-04-29 16:59:43.000000 mitos-2.1.9/mitos/mitfi/parser/mitfi_import.jar
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-29 16:59:51.000000 mitos-2.1.9/mitos/mito/
+-rw-rw-rw-   0 root         (0) root         (0)     5074 2024-04-29 16:59:43.000000 mitos-2.1.9/mitos/mito/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    60417 2024-04-29 16:59:43.000000 mitos-2.1.9/mitos/mitoch_revisions.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-29 16:59:51.000000 mitos-2.1.9/mitos/mitofile/
+-rw-rw-rw-   0 root         (0) root         (0)     5272 2024-04-29 16:59:43.000000 mitos-2.1.9/mitos/mitofile/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     4327 2024-04-29 16:59:43.000000 mitos-2.1.9/mitos/mitoloc.py
+-rw-rw-rw-   0 root         (0) root         (0)    16081 2024-04-29 16:59:43.000000 mitos-2.1.9/mitos/mitos-extension.py
+-rw-rw-rw-   0 root         (0) root         (0)    13698 2024-04-29 16:59:43.000000 mitos-2.1.9/mitos/mitos-extension2.py
+-rw-rw-rw-   0 root         (0) root         (0)     2100 2024-04-29 16:59:43.000000 mitos-2.1.9/mitos/mumcmp.py
+-rw-rw-rw-   0 root         (0) root         (0)      829 2024-04-29 16:59:43.000000 mitos-2.1.9/mitos/names.py
+-rw-rw-rw-   0 root         (0) root         (0)     3009 2024-04-29 16:59:43.000000 mitos-2.1.9/mitos/ogre-geneorder.py
+-rwxrwxrwx   0 root         (0) root         (0)     3043 2024-04-29 16:59:43.000000 mitos-2.1.9/mitos/plotprot.R
+-rwxrwxrwx   0 root         (0) root         (0)     2538 2024-04-29 16:59:43.000000 mitos-2.1.9/mitos/plotrna.R
+-rwxrwxrwx   0 root         (0) root         (0)     4391 2024-04-29 16:59:43.000000 mitos-2.1.9/mitos/plotstst.R
+-rw-rw-rw-   0 root         (0) root         (0)     3186 2024-04-29 16:59:43.000000 mitos-2.1.9/mitos/prepareFiles.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-29 16:59:51.000000 mitos-2.1.9/mitos/protfeat/
+-rw-rw-rw-   0 root         (0) root         (0)    27133 2024-04-29 16:59:43.000000 mitos-2.1.9/mitos/protfeat/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1426 2024-04-29 16:59:43.000000 mitos-2.1.9/mitos/removegene.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-29 16:59:51.000000 mitos-2.1.9/mitos/rna/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-29 16:59:43.000000 mitos-2.1.9/mitos/rna/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     4119 2024-04-29 16:59:43.000000 mitos-2.1.9/mitos/rna/forester.py
+-rw-rw-rw-   0 root         (0) root         (0)     1446 2024-04-29 16:59:43.000000 mitos-2.1.9/mitos/rna/vienna.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-29 16:59:51.000000 mitos-2.1.9/mitos/sequence/
+-rw-rw-rw-   0 root         (0) root         (0)    16807 2024-04-29 16:59:43.000000 mitos-2.1.9/mitos/sequence/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1487 2024-04-29 16:59:43.000000 mitos-2.1.9/mitos/sequence/degenerate.py
+-rw-rw-rw-   0 root         (0) root         (0)    14519 2024-04-29 16:59:43.000000 mitos-2.1.9/mitos/skew.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-29 16:59:51.000000 mitos-2.1.9/mitos/tax/
+-rw-rw-rw-   0 root         (0) root         (0)     3602 2024-04-29 16:59:43.000000 mitos-2.1.9/mitos/tax/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-29 16:59:51.000000 mitos-2.1.9/mitos/tbl/
+-rw-rw-rw-   0 root         (0) root         (0)     5004 2024-04-29 16:59:43.000000 mitos-2.1.9/mitos/tbl/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-29 16:59:51.000000 mitos-2.1.9/mitos/trna/
+-rw-rw-rw-   0 root         (0) root         (0)     4278 2024-04-29 16:59:43.000000 mitos-2.1.9/mitos/trna/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     8984 2024-04-29 16:59:43.000000 mitos-2.1.9/mitos/trna/arwenscan.py
+-rw-rw-rw-   0 root         (0) root         (0)    11962 2024-04-29 16:59:43.000000 mitos-2.1.9/mitos/trna/trnascan.py
+-rw-rw-rw-   0 root         (0) root         (0)   157352 2024-04-29 16:59:43.000000 mitos-2.1.9/mitos/trna-cm.py
+-rw-rw-rw-   0 root         (0) root         (0)    23410 2024-04-29 16:59:43.000000 mitos-2.1.9/mitos/trnadist.py
+-rw-rw-rw-   0 root         (0) root         (0)     4917 2024-04-29 16:59:43.000000 mitos-2.1.9/mitos/trnascan_parse_separate.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-29 16:59:51.000000 mitos-2.1.9/mitos/update/
+-rw-rw-rw-   0 root         (0) root         (0)    25529 2024-04-29 16:59:43.000000 mitos-2.1.9/mitos/update/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     4823 2024-04-29 16:59:43.000000 mitos-2.1.9/mitos/update-mitolog.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-29 16:59:51.000000 mitos-2.1.9/mitos/util/
+-rw-rw-rw-   0 root         (0) root         (0)      660 2024-04-29 16:59:43.000000 mitos-2.1.9/mitos/util/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-29 16:59:51.000000 mitos-2.1.9/mitos/webserver/
+-rw-rw-rw-   0 root         (0) root         (0)    10152 2024-04-29 16:59:43.000000 mitos-2.1.9/mitos/webserver/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    26961 2024-04-29 16:59:43.000000 mitos-2.1.9/mitos/webserver/help.txt
+-rwxrwxrwx   0 root         (0) root         (0)      785 2024-04-29 16:59:43.000000 mitos-2.1.9/mitos/webserver/history.txt
+-rw-rw-rw-   0 root         (0) root         (0)     6691 2024-04-29 16:59:43.000000 mitos-2.1.9/mitos/webserver/index.txt
+-rw-rw-rw-   0 root         (0) root         (0)      541 2024-04-29 16:59:43.000000 mitos-2.1.9/mitos/webserver/news.txt
+-rw-rw-rw-   0 root         (0) root         (0)     3686 2024-04-29 16:59:43.000000 mitos-2.1.9/mitos/webserver/upload.txt
+-rw-rw-rw-   0 root         (0) root         (0)      439 2024-04-29 16:59:43.000000 mitos-2.1.9/mitos/webserver/wait.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-29 16:59:51.000000 mitos-2.1.9/mitos.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      801 2024-04-29 16:59:51.000000 mitos-2.1.9/mitos.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1983 2024-04-29 16:59:51.000000 mitos-2.1.9/mitos.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-04-29 16:59:51.000000 mitos-2.1.9/mitos.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       16 2024-04-29 16:59:51.000000 mitos-2.1.9/mitos.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        6 2024-04-29 16:59:51.000000 mitos-2.1.9/mitos.egg-info/top_level.txt
+-rwxrwxrwx   0 root         (0) root         (0)     1654 2024-04-29 16:59:43.000000 mitos-2.1.9/refseqsplit.py
+-rwxrwxrwx   0 root         (0) root         (0)    46181 2024-04-29 16:59:43.000000 mitos-2.1.9/runmitos.py
+-rw-rw-rw-   0 root         (0) root         (0)      280 2024-04-29 16:59:51.000000 mitos-2.1.9/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)     1391 2024-04-29 16:59:43.000000 mitos-2.1.9/setup.py
+-rwxrwxrwx   0 root         (0) root         (0)     9153 2024-04-29 16:59:43.000000 mitos-2.1.9/subseq.py
+-rwxrwxrwx   0 root         (0) root         (0)     4277 2024-04-29 16:59:43.000000 mitos-2.1.9/taxtree.py
+-rw-rw-rw-   0 root         (0) root         (0)     2485 2024-04-29 16:59:43.000000 mitos-2.1.9/update-blastdb.py
```

### Comparing `mitos-2.1.8/LICENSE` & `mitos-2.1.9/LICENSE`

 * *Files identical despite different names*

### Comparing `mitos-2.1.8/PKG-INFO` & `mitos-2.1.9/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mitos
-Version: 2.1.8
+Version: 2.1.9
 Summary: MITOS: de novo annotation of metazoan mitochondrial genomes
 Home-page: http://mitos.bioinf.uni-leipzig.de
 Author: Matthias Bernt
 Author-email: bernt@informatik.uni-leipzig.de
 License: UNKNOWN
 Download-URL: https://gitlab.com/Bernt/MITOS
 Platform: UNKNOWN
```

### Comparing `mitos-2.1.8/README.md` & `mitos-2.1.9/README.md`

 * *Files identical despite different names*

### Comparing `mitos-2.1.8/analyse.py` & `mitos-2.1.9/analyse.py`

 * *Files identical despite different names*

### Comparing `mitos-2.1.8/drawmitos.py` & `mitos-2.1.9/drawmitos.py`

 * *Files identical despite different names*

### Comparing `mitos-2.1.8/gcpp.py` & `mitos-2.1.9/gcpp.py`

 * *Files identical despite different names*

### Comparing `mitos-2.1.8/geneorder.py` & `mitos-2.1.9/geneorder.py`

 * *Files identical despite different names*

### Comparing `mitos-2.1.8/getfeatures.py` & `mitos-2.1.9/getfeatures.py`

 * *Files identical despite different names*

### Comparing `mitos-2.1.8/getinfo.py` & `mitos-2.1.9/getinfo.py`

 * *Files identical despite different names*

### Comparing `mitos-2.1.8/mitos/CONFIG.py` & `mitos-2.1.9/mitos/CONFIG.py`

 * *Files identical despite different names*

### Comparing `mitos-2.1.8/mitos/bedfile/__init__.py` & `mitos-2.1.9/mitos/bedfile/__init__.py`

 * *Files identical despite different names*

### Comparing `mitos-2.1.8/mitos/blast/__init__.py` & `mitos-2.1.9/mitos/blast/__init__.py`

 * *Files identical despite different names*

### Comparing `mitos-2.1.8/mitos/booreparser.py` & `mitos-2.1.9/mitos/booreparser.py`

 * *Files identical despite different names*

### Comparing `mitos-2.1.8/mitos/cmsearch_parse_separate.py` & `mitos-2.1.9/mitos/cmsearch_parse_separate.py`

 * *Files identical despite different names*

### Comparing `mitos-2.1.8/mitos/codoncount.py` & `mitos-2.1.9/mitos/codoncount.py`

 * *Files identical despite different names*

### Comparing `mitos-2.1.8/mitos/convert_tree.py` & `mitos-2.1.9/mitos/convert_tree.py`

 * *Files identical despite different names*

### Comparing `mitos-2.1.8/mitos/create_prot_fasta.py` & `mitos-2.1.9/mitos/create_prot_fasta.py`

 * *Files identical despite different names*

### Comparing `mitos-2.1.8/mitos/draw/__init__.py` & `mitos-2.1.9/mitos/draw/__init__.py`

 * *Files identical despite different names*

### Comparing `mitos-2.1.8/mitos/extprog/__init__.py` & `mitos-2.1.9/mitos/extprog/__init__.py`

 * *Files identical despite different names*

### Comparing `mitos-2.1.8/mitos/feature/__init__.py` & `mitos-2.1.9/mitos/feature/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -828,28 +828,30 @@
             if self.type not in ["tRNA", "rRNA", "gene"]:
                 return "\n".join(gff)
 
         if self.score is not None:
             s = str(self.score)
         else:
             s = "."
+
+        # using rf as indicator for PCGs, phase is 0
         if self.rf is None:
-            rf = "."
+            phase = "."
         else:
-            rf = str(self.rf)
+            phase = 0
 
         # exon
         start, stop = self.start, self.stop
         if start > stop:
             stop += size
 
         gff.append("{seqid}\t{source}\t{type}\t{start}\t{end}\t{score}\t{strand}\t{phase}\tParent=transcript_{namep};Name={name}".format(
             seqid=acc, source=self.method, type="exon",
             start=start + 1, end=stop + 1, score=s, strand=self.plusminus(),
-            phase=rf, namep=self.outputname(anticodon=False, part=False), name=self.outputname(anticodon=False)))
+            phase=phase, namep=self.outputname(anticodon=False, part=False), name=self.outputname(anticodon=False)))
         return "\n".join(gff)
 
     def tblstr(self):
         """
         this function returns the string to be written in a mito file
         """
```

### Comparing `mitos-2.1.8/mitos/gb/__init__.py` & `mitos-2.1.9/mitos/gb/__init__.py`

 * *Files identical despite different names*

### Comparing `mitos-2.1.8/mitos/gb/unify.py` & `mitos-2.1.9/mitos/gb/unify.py`

 * *Files identical despite different names*

### Comparing `mitos-2.1.8/mitos/get-wancy.py` & `mitos-2.1.9/mitos/get-wancy.py`

 * *Files identical despite different names*

### Comparing `mitos-2.1.8/mitos/gfffile/__init__.py` & `mitos-2.1.9/mitos/gfffile/__init__.py`

 * *Files identical despite different names*

### Comparing `mitos-2.1.8/mitos/inihit.py` & `mitos-2.1.9/mitos/inihit.py`

 * *Files identical despite different names*

### Comparing `mitos-2.1.8/mitos/merge_results.py` & `mitos-2.1.9/mitos/merge_results.py`

 * *Files identical despite different names*

### Comparing `mitos-2.1.8/mitos/mergefeature/__init__.py` & `mitos-2.1.9/mitos/mergefeature/__init__.py`

 * *Files identical despite different names*

### Comparing `mitos-2.1.8/mitos/mitfi/__init__.py` & `mitos-2.1.9/mitos/mitfi/__init__.py`

 * *Files identical despite different names*

### Comparing `mitos-2.1.8/mitos/mitfi/parser/improve_infernal_structure.jar` & `mitos-2.1.9/mitos/mitfi/parser/improve_infernal_structure.jar`

 * *Files identical despite different names*

### Comparing `mitos-2.1.8/mitos/mitfi/parser/mitfiGeneticCodes` & `mitos-2.1.9/mitos/mitfi/parser/mitfiGeneticCodes`

 * *Files identical despite different names*

### Comparing `mitos-2.1.8/mitos/mitfi/parser/mitfi_import-1.1.jar` & `mitos-2.1.9/mitos/mitfi/parser/mitfi_import-1.1.jar`

 * *Files identical despite different names*

### Comparing `mitos-2.1.8/mitos/mitfi/parser/mitfi_import-1.1.jar.old` & `mitos-2.1.9/mitos/mitfi/parser/mitfi_import-1.1.jar.old`

 * *Files identical despite different names*

### Comparing `mitos-2.1.8/mitos/mitfi/parser/mitfi_import-1.1.jar.org` & `mitos-2.1.9/mitos/mitfi/parser/mitfi_import-1.1.jar.org`

 * *Files identical despite different names*

### Comparing `mitos-2.1.8/mitos/mitfi/parser/mitfi_import-1.1.jar.org.pre-circ` & `mitos-2.1.9/mitos/mitfi/parser/mitfi_import-1.1.jar.org.pre-circ`

 * *Files identical despite different names*

### Comparing `mitos-2.1.8/mitos/mitfi/parser/mitfi_import.jar` & `mitos-2.1.9/mitos/mitfi/parser/mitfi_import.jar`

 * *Files identical despite different names*

### Comparing `mitos-2.1.8/mitos/mito/__init__.py` & `mitos-2.1.9/mitos/mito/__init__.py`

 * *Files identical despite different names*

### Comparing `mitos-2.1.8/mitos/mitoch_revisions.py` & `mitos-2.1.9/mitos/mitoch_revisions.py`

 * *Files identical despite different names*

### Comparing `mitos-2.1.8/mitos/mitofile/__init__.py` & `mitos-2.1.9/mitos/mitofile/__init__.py`

 * *Files identical despite different names*

### Comparing `mitos-2.1.8/mitos/mitoloc.py` & `mitos-2.1.9/mitos/mitoloc.py`

 * *Files identical despite different names*

### Comparing `mitos-2.1.8/mitos/mitos-extension.py` & `mitos-2.1.9/mitos/mitos-extension.py`

 * *Files identical despite different names*

### Comparing `mitos-2.1.8/mitos/mitos-extension2.py` & `mitos-2.1.9/mitos/mitos-extension2.py`

 * *Files identical despite different names*

### Comparing `mitos-2.1.8/mitos/mumcmp.py` & `mitos-2.1.9/mitos/mumcmp.py`

 * *Files identical despite different names*

### Comparing `mitos-2.1.8/mitos/names.py` & `mitos-2.1.9/mitos/names.py`

 * *Files identical despite different names*

### Comparing `mitos-2.1.8/mitos/ogre-geneorder.py` & `mitos-2.1.9/mitos/ogre-geneorder.py`

 * *Files identical despite different names*

### Comparing `mitos-2.1.8/mitos/plotprot.R` & `mitos-2.1.9/mitos/plotprot.R`

 * *Files identical despite different names*

### Comparing `mitos-2.1.8/mitos/plotrna.R` & `mitos-2.1.9/mitos/plotrna.R`

 * *Files identical despite different names*

### Comparing `mitos-2.1.8/mitos/plotstst.R` & `mitos-2.1.9/mitos/plotstst.R`

 * *Files identical despite different names*

### Comparing `mitos-2.1.8/mitos/prepareFiles.py` & `mitos-2.1.9/mitos/prepareFiles.py`

 * *Files identical despite different names*

### Comparing `mitos-2.1.8/mitos/protfeat/__init__.py` & `mitos-2.1.9/mitos/protfeat/__init__.py`

 * *Files identical despite different names*

### Comparing `mitos-2.1.8/mitos/removegene.py` & `mitos-2.1.9/mitos/removegene.py`

 * *Files identical despite different names*

### Comparing `mitos-2.1.8/mitos/rna/forester.py` & `mitos-2.1.9/mitos/rna/forester.py`

 * *Files identical despite different names*

### Comparing `mitos-2.1.8/mitos/rna/vienna.py` & `mitos-2.1.9/mitos/rna/vienna.py`

 * *Files identical despite different names*

### Comparing `mitos-2.1.8/mitos/sequence/__init__.py` & `mitos-2.1.9/mitos/sequence/__init__.py`

 * *Files identical despite different names*

### Comparing `mitos-2.1.8/mitos/sequence/degenerate.py` & `mitos-2.1.9/mitos/sequence/degenerate.py`

 * *Files identical despite different names*

### Comparing `mitos-2.1.8/mitos/skew.py` & `mitos-2.1.9/mitos/skew.py`

 * *Files identical despite different names*

### Comparing `mitos-2.1.8/mitos/tax/__init__.py` & `mitos-2.1.9/mitos/tax/__init__.py`

 * *Files identical despite different names*

### Comparing `mitos-2.1.8/mitos/tbl/__init__.py` & `mitos-2.1.9/mitos/tbl/__init__.py`

 * *Files identical despite different names*

### Comparing `mitos-2.1.8/mitos/trna/__init__.py` & `mitos-2.1.9/mitos/trna/__init__.py`

 * *Files identical despite different names*

### Comparing `mitos-2.1.8/mitos/trna/arwenscan.py` & `mitos-2.1.9/mitos/trna/arwenscan.py`

 * *Files identical despite different names*

### Comparing `mitos-2.1.8/mitos/trna/trnascan.py` & `mitos-2.1.9/mitos/trna/trnascan.py`

 * *Files identical despite different names*

### Comparing `mitos-2.1.8/mitos/trna-cm.py` & `mitos-2.1.9/mitos/trna-cm.py`

 * *Files identical despite different names*

### Comparing `mitos-2.1.8/mitos/trnadist.py` & `mitos-2.1.9/mitos/trnadist.py`

 * *Files identical despite different names*

### Comparing `mitos-2.1.8/mitos/trnascan_parse_separate.py` & `mitos-2.1.9/mitos/trnascan_parse_separate.py`

 * *Files identical despite different names*

### Comparing `mitos-2.1.8/mitos/update/__init__.py` & `mitos-2.1.9/mitos/update/__init__.py`

 * *Files identical despite different names*

### Comparing `mitos-2.1.8/mitos/update-mitolog.py` & `mitos-2.1.9/mitos/update-mitolog.py`

 * *Files identical despite different names*

### Comparing `mitos-2.1.8/mitos/util/__init__.py` & `mitos-2.1.9/mitos/util/__init__.py`

 * *Files identical despite different names*

### Comparing `mitos-2.1.8/mitos/webserver/__init__.py` & `mitos-2.1.9/mitos/webserver/__init__.py`

 * *Files identical despite different names*

### Comparing `mitos-2.1.8/mitos/webserver/help.txt` & `mitos-2.1.9/mitos/webserver/help.txt`

 * *Files identical despite different names*

### Comparing `mitos-2.1.8/mitos/webserver/history.txt` & `mitos-2.1.9/mitos/webserver/history.txt`

 * *Files identical despite different names*

### Comparing `mitos-2.1.8/mitos/webserver/index.txt` & `mitos-2.1.9/mitos/webserver/index.txt`

 * *Files identical despite different names*

### Comparing `mitos-2.1.8/mitos/webserver/news.txt` & `mitos-2.1.9/mitos/webserver/news.txt`

 * *Files identical despite different names*

### Comparing `mitos-2.1.8/mitos/webserver/upload.txt` & `mitos-2.1.9/mitos/webserver/upload.txt`

 * *Files identical despite different names*

### Comparing `mitos-2.1.8/mitos.egg-info/PKG-INFO` & `mitos-2.1.9/mitos.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mitos
-Version: 2.1.8
+Version: 2.1.9
 Summary: MITOS: de novo annotation of metazoan mitochondrial genomes
 Home-page: http://mitos.bioinf.uni-leipzig.de
 Author: Matthias Bernt
 Author-email: bernt@informatik.uni-leipzig.de
 License: UNKNOWN
 Download-URL: https://gitlab.com/Bernt/MITOS
 Platform: UNKNOWN
```

### Comparing `mitos-2.1.8/mitos.egg-info/SOURCES.txt` & `mitos-2.1.9/mitos.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mitos-2.1.8/refseqsplit.py` & `mitos-2.1.9/refseqsplit.py`

 * *Files identical despite different names*

### Comparing `mitos-2.1.8/runmitos.py` & `mitos-2.1.9/runmitos.py`

 * *Files identical despite different names*

### Comparing `mitos-2.1.8/setup.py` & `mitos-2.1.9/setup.py`

 * *Files identical despite different names*

### Comparing `mitos-2.1.8/subseq.py` & `mitos-2.1.9/subseq.py`

 * *Files identical despite different names*

### Comparing `mitos-2.1.8/taxtree.py` & `mitos-2.1.9/taxtree.py`

 * *Files identical despite different names*

### Comparing `mitos-2.1.8/update-blastdb.py` & `mitos-2.1.9/update-blastdb.py`

 * *Files identical despite different names*

