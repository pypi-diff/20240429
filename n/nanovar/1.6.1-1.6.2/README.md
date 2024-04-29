# Comparing `tmp/nanovar-1.6.1.tar.gz` & `tmp/nanovar-1.6.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nanovar-1.6.1.tar", last modified: Sun Mar 31 07:52:00 2024, max compression
+gzip compressed data, was "nanovar-1.6.2.tar", last modified: Mon Apr 29 15:45:01 2024, max compression
```

## Comparing `nanovar-1.6.1.tar` & `nanovar-1.6.2.tar`

### file list

```diff
@@ -1,65 +1,65 @@
-drwxr-xr-x   0 cy        (1000) cy        (1000)        0 2024-03-31 07:52:00.093847 nanovar-1.6.1/
--rw-r--r--   0 cy        (1000) cy        (1000)    11269 2024-03-30 14:49:59.000000 nanovar-1.6.1/CHANGELOG.txt
--rw-r--r--   0 cy        (1000) cy        (1000)    35149 2024-01-16 13:46:16.000000 nanovar-1.6.1/LICENSE.txt
--rw-r--r--   0 cy        (1000) cy        (1000)      213 2024-01-16 13:46:16.000000 nanovar-1.6.1/MANIFEST.in
--rw-r--r--   0 cy        (1000) cy        (1000)    12900 2024-03-31 07:52:00.093847 nanovar-1.6.1/PKG-INFO
--rw-r--r--   0 cy        (1000) cy        (1000)    11837 2024-03-30 14:49:59.000000 nanovar-1.6.1/README.md
-drwxr-xr-x   0 cy        (1000) cy        (1000)        0 2024-03-31 07:52:00.083847 nanovar-1.6.1/nanovar/
--rw-r--r--   0 cy        (1000) cy        (1000)      167 2024-01-16 13:46:16.000000 nanovar-1.6.1/nanovar/__init__.py
-drwxr-xr-x   0 cy        (1000) cy        (1000)        0 2024-03-31 07:52:00.083847 nanovar-1.6.1/nanovar/css/
--rw-r--r--   0 cy        (1000) cy        (1000)        0 2024-01-16 13:46:16.000000 nanovar-1.6.1/nanovar/css/__init__.py
--rw-r--r--   0 cy        (1000) cy        (1000)   137276 2024-01-16 13:46:16.000000 nanovar-1.6.1/nanovar/css/bootstrap.min.css
--rw-r--r--   0 cy        (1000) cy        (1000)     9250 2024-01-16 13:46:16.000000 nanovar-1.6.1/nanovar/css/buttons.dataTables.min.css
--rw-r--r--   0 cy        (1000) cy        (1000)    31001 2024-01-16 13:46:16.000000 nanovar-1.6.1/nanovar/css/font-awesome.min.css
--rw-r--r--   0 cy        (1000) cy        (1000)    13900 2024-01-16 13:46:16.000000 nanovar-1.6.1/nanovar/css/jquery.dataTables.min.css
--rw-r--r--   0 cy        (1000) cy        (1000)   214364 2024-01-16 13:46:16.000000 nanovar-1.6.1/nanovar/css/mdb.min.css
-drwxr-xr-x   0 cy        (1000) cy        (1000)        0 2024-03-31 07:52:00.083847 nanovar-1.6.1/nanovar/gaps/
--rw-r--r--   0 cy        (1000) cy        (1000)        0 2024-01-16 13:46:16.000000 nanovar-1.6.1/nanovar/gaps/__init__.py
--rw-r--r--   0 cy        (1000) cy        (1000)     2597 2024-01-16 13:46:16.000000 nanovar-1.6.1/nanovar/gaps/hg19_filter-B400.bed
--rw-r--r--   0 cy        (1000) cy        (1000)     9159 2024-01-16 13:46:16.000000 nanovar-1.6.1/nanovar/gaps/hg38_curated_filter_main.bed
--rw-r--r--   0 cy        (1000) cy        (1000)     2291 2024-01-16 13:46:16.000000 nanovar-1.6.1/nanovar/gaps/mm10_filter-B400.bed
-drwxr-xr-x   0 cy        (1000) cy        (1000)        0 2024-03-31 07:52:00.093847 nanovar-1.6.1/nanovar/js/
--rw-r--r--   0 cy        (1000) cy        (1000)        0 2024-01-16 13:46:16.000000 nanovar-1.6.1/nanovar/js/__init__.py
--rw-r--r--   0 cy        (1000) cy        (1000)    51039 2024-01-16 13:46:16.000000 nanovar-1.6.1/nanovar/js/bootstrap.min.js
--rw-r--r--   0 cy        (1000) cy        (1000)    26039 2024-01-16 13:46:16.000000 nanovar-1.6.1/nanovar/js/buttons.flash.min.js
--rw-r--r--   0 cy        (1000) cy        (1000)    24010 2024-01-16 13:46:16.000000 nanovar-1.6.1/nanovar/js/buttons.html5.min.js
--rw-r--r--   0 cy        (1000) cy        (1000)    18260 2024-01-16 13:46:16.000000 nanovar-1.6.1/nanovar/js/dataTables.buttons.min.js
--rw-r--r--   0 cy        (1000) cy        (1000)    86927 2024-01-16 13:46:16.000000 nanovar-1.6.1/nanovar/js/jquery-3.3.1.min.js
--rw-r--r--   0 cy        (1000) cy        (1000)    82411 2024-01-16 13:46:16.000000 nanovar-1.6.1/nanovar/js/jquery.dataTables.min.js
--rw-r--r--   0 cy        (1000) cy        (1000)   101940 2024-01-16 13:46:16.000000 nanovar-1.6.1/nanovar/js/jszip.min.js
--rw-r--r--   0 cy        (1000) cy        (1000)   210115 2024-01-16 13:46:16.000000 nanovar-1.6.1/nanovar/js/mdb.min.js
--rw-r--r--   0 cy        (1000) cy        (1000)    19197 2024-01-16 13:46:16.000000 nanovar-1.6.1/nanovar/js/popper.min.js
-drwxr-xr-x   0 cy        (1000) cy        (1000)        0 2024-03-31 07:52:00.093847 nanovar-1.6.1/nanovar/model/
--rw-r--r--   0 cy        (1000) cy        (1000)    22592 2024-01-16 13:46:16.000000 nanovar-1.6.1/nanovar/model/ANN.E100B400L3N12-5D0.4-0.2SGDsee11_het_ccs_v1.h5
--rw-r--r--   0 cy        (1000) cy        (1000)    22592 2024-01-16 13:46:16.000000 nanovar-1.6.1/nanovar/model/ANN.E100B400L3N12-5D0.4-0.2SGDsee11_het_clr_v1.h5
--rw-r--r--   0 cy        (1000) cy        (1000)    22592 2024-01-16 13:46:16.000000 nanovar-1.6.1/nanovar/model/ANN.E100B400L3N12-5D0.4-0.2SGDsee11_het_gup_v1.h5
--rw-r--r--   0 cy        (1000) cy        (1000)        0 2024-01-16 13:46:16.000000 nanovar-1.6.1/nanovar/model/__init__.py
--rw-r--r--   0 cy        (1000) cy        (1000)    24911 2024-01-16 13:46:16.000000 nanovar-1.6.1/nanovar/nanovar
--rw-r--r--   0 cy        (1000) cy        (1000)     8262 2024-01-16 13:46:16.000000 nanovar-1.6.1/nanovar/nv_align.py
--rw-r--r--   0 cy        (1000) cy        (1000)   668769 2024-01-16 13:46:16.000000 nanovar-1.6.1/nanovar/nv_bam_parser.c
--rw-r--r--   0 cy        (1000) cy        (1000)    14463 2024-01-16 13:46:16.000000 nanovar-1.6.1/nanovar/nv_bam_parser.pyx
--rw-r--r--   0 cy        (1000) cy        (1000)    11514 2024-01-16 13:46:16.000000 nanovar-1.6.1/nanovar/nv_characterize.py
--rw-r--r--   0 cy        (1000) cy        (1000)    36161 2024-01-16 13:46:16.000000 nanovar-1.6.1/nanovar/nv_cluster.py
--rw-r--r--   0 cy        (1000) cy        (1000)     5118 2024-01-16 13:46:16.000000 nanovar-1.6.1/nanovar/nv_cov_upper.py
--rw-r--r--   0 cy        (1000) cy        (1000)    41821 2024-01-16 13:46:16.000000 nanovar-1.6.1/nanovar/nv_detect_algo.py
--rw-r--r--   0 cy        (1000) cy        (1000)     9074 2024-01-16 13:46:16.000000 nanovar-1.6.1/nanovar/nv_dup_te_detect.py
--rw-r--r--   0 cy        (1000) cy        (1000)     7524 2024-01-16 13:46:16.000000 nanovar-1.6.1/nanovar/nv_input.py
--rw-r--r--   0 cy        (1000) cy        (1000)     8907 2024-01-16 13:46:16.000000 nanovar-1.6.1/nanovar/nv_nn.py
--rw-r--r--   0 cy        (1000) cy        (1000)    28845 2024-01-16 13:46:16.000000 nanovar-1.6.1/nanovar/nv_parser.py
--rw-r--r--   0 cy        (1000) cy        (1000)    25255 2024-01-16 13:46:16.000000 nanovar-1.6.1/nanovar/nv_report.py
--rw-r--r--   0 cy        (1000) cy        (1000)     6431 2024-01-16 13:46:16.000000 nanovar-1.6.1/nanovar/nv_te_analyzer.py
--rw-r--r--   0 cy        (1000) cy        (1000)     8826 2024-01-16 13:46:16.000000 nanovar-1.6.1/nanovar/nv_valid.py
--rw-r--r--   0 cy        (1000) cy        (1000)    18511 2024-01-16 13:46:16.000000 nanovar-1.6.1/nanovar/nv_vcf.py
-drwxr-xr-x   0 cy        (1000) cy        (1000)        0 2024-03-31 07:52:00.093847 nanovar-1.6.1/nanovar/ref/
--rw-r--r--   0 cy        (1000) cy        (1000)     8991 2024-01-16 13:46:16.000000 nanovar-1.6.1/nanovar/ref/hg38_L1_Alu.counts.obinary
--rw-r--r--   0 cy        (1000) cy        (1000)     7707 2024-01-16 13:46:16.000000 nanovar-1.6.1/nanovar/ref/hg38_L1_Alu.fa
--rw-r--r--   0 cy        (1000) cy        (1000)       22 2024-03-30 14:49:59.000000 nanovar-1.6.1/nanovar/version.py
-drwxr-xr-x   0 cy        (1000) cy        (1000)        0 2024-03-31 07:52:00.083847 nanovar-1.6.1/nanovar.egg-info/
--rw-r--r--   0 cy        (1000) cy        (1000)    12900 2024-03-31 07:51:59.000000 nanovar-1.6.1/nanovar.egg-info/PKG-INFO
--rw-r--r--   0 cy        (1000) cy        (1000)     1529 2024-03-31 07:52:00.000000 nanovar-1.6.1/nanovar.egg-info/SOURCES.txt
--rw-r--r--   0 cy        (1000) cy        (1000)        1 2024-03-31 07:51:59.000000 nanovar-1.6.1/nanovar.egg-info/dependency_links.txt
--rw-r--r--   0 cy        (1000) cy        (1000)      187 2024-03-31 07:51:59.000000 nanovar-1.6.1/nanovar.egg-info/requires.txt
--rw-r--r--   0 cy        (1000) cy        (1000)        8 2024-03-31 07:51:59.000000 nanovar-1.6.1/nanovar.egg-info/top_level.txt
--rw-r--r--   0 cy        (1000) cy        (1000)     1401 2024-01-16 13:46:16.000000 nanovar-1.6.1/requirements.txt
--rw-r--r--   0 cy        (1000) cy        (1000)       79 2024-03-31 07:52:00.093847 nanovar-1.6.1/setup.cfg
--rw-r--r--   0 cy        (1000) cy        (1000)     1758 2024-03-30 14:49:59.000000 nanovar-1.6.1/setup.py
+drwxr-xr-x   0 cy        (1000) cy        (1000)        0 2024-04-29 15:45:01.922109 nanovar-1.6.2/
+-rw-r--r--   0 cy        (1000) cy        (1000)    11421 2024-04-29 15:44:35.000000 nanovar-1.6.2/CHANGELOG.txt
+-rw-r--r--   0 cy        (1000) cy        (1000)    35149 2024-01-16 13:46:16.000000 nanovar-1.6.2/LICENSE.txt
+-rw-r--r--   0 cy        (1000) cy        (1000)      213 2024-01-16 13:46:16.000000 nanovar-1.6.2/MANIFEST.in
+-rw-r--r--   0 cy        (1000) cy        (1000)    12900 2024-04-29 15:45:01.922109 nanovar-1.6.2/PKG-INFO
+-rw-r--r--   0 cy        (1000) cy        (1000)    11837 2024-04-29 15:44:35.000000 nanovar-1.6.2/README.md
+drwxr-xr-x   0 cy        (1000) cy        (1000)        0 2024-04-29 15:45:01.912109 nanovar-1.6.2/nanovar/
+-rw-r--r--   0 cy        (1000) cy        (1000)      167 2024-01-16 13:46:16.000000 nanovar-1.6.2/nanovar/__init__.py
+drwxr-xr-x   0 cy        (1000) cy        (1000)        0 2024-04-29 15:45:01.922109 nanovar-1.6.2/nanovar/css/
+-rw-r--r--   0 cy        (1000) cy        (1000)        0 2024-01-16 13:46:16.000000 nanovar-1.6.2/nanovar/css/__init__.py
+-rw-r--r--   0 cy        (1000) cy        (1000)   137276 2024-01-16 13:46:16.000000 nanovar-1.6.2/nanovar/css/bootstrap.min.css
+-rw-r--r--   0 cy        (1000) cy        (1000)     9250 2024-01-16 13:46:16.000000 nanovar-1.6.2/nanovar/css/buttons.dataTables.min.css
+-rw-r--r--   0 cy        (1000) cy        (1000)    31001 2024-01-16 13:46:16.000000 nanovar-1.6.2/nanovar/css/font-awesome.min.css
+-rw-r--r--   0 cy        (1000) cy        (1000)    13900 2024-01-16 13:46:16.000000 nanovar-1.6.2/nanovar/css/jquery.dataTables.min.css
+-rw-r--r--   0 cy        (1000) cy        (1000)   214364 2024-01-16 13:46:16.000000 nanovar-1.6.2/nanovar/css/mdb.min.css
+drwxr-xr-x   0 cy        (1000) cy        (1000)        0 2024-04-29 15:45:01.922109 nanovar-1.6.2/nanovar/gaps/
+-rw-r--r--   0 cy        (1000) cy        (1000)        0 2024-01-16 13:46:16.000000 nanovar-1.6.2/nanovar/gaps/__init__.py
+-rw-r--r--   0 cy        (1000) cy        (1000)     2597 2024-01-16 13:46:16.000000 nanovar-1.6.2/nanovar/gaps/hg19_filter-B400.bed
+-rw-r--r--   0 cy        (1000) cy        (1000)     9159 2024-01-16 13:46:16.000000 nanovar-1.6.2/nanovar/gaps/hg38_curated_filter_main.bed
+-rw-r--r--   0 cy        (1000) cy        (1000)     2291 2024-01-16 13:46:16.000000 nanovar-1.6.2/nanovar/gaps/mm10_filter-B400.bed
+drwxr-xr-x   0 cy        (1000) cy        (1000)        0 2024-04-29 15:45:01.922109 nanovar-1.6.2/nanovar/js/
+-rw-r--r--   0 cy        (1000) cy        (1000)        0 2024-01-16 13:46:16.000000 nanovar-1.6.2/nanovar/js/__init__.py
+-rw-r--r--   0 cy        (1000) cy        (1000)    51039 2024-01-16 13:46:16.000000 nanovar-1.6.2/nanovar/js/bootstrap.min.js
+-rw-r--r--   0 cy        (1000) cy        (1000)    26039 2024-01-16 13:46:16.000000 nanovar-1.6.2/nanovar/js/buttons.flash.min.js
+-rw-r--r--   0 cy        (1000) cy        (1000)    24010 2024-01-16 13:46:16.000000 nanovar-1.6.2/nanovar/js/buttons.html5.min.js
+-rw-r--r--   0 cy        (1000) cy        (1000)    18260 2024-01-16 13:46:16.000000 nanovar-1.6.2/nanovar/js/dataTables.buttons.min.js
+-rw-r--r--   0 cy        (1000) cy        (1000)    86927 2024-01-16 13:46:16.000000 nanovar-1.6.2/nanovar/js/jquery-3.3.1.min.js
+-rw-r--r--   0 cy        (1000) cy        (1000)    82411 2024-01-16 13:46:16.000000 nanovar-1.6.2/nanovar/js/jquery.dataTables.min.js
+-rw-r--r--   0 cy        (1000) cy        (1000)   101940 2024-01-16 13:46:16.000000 nanovar-1.6.2/nanovar/js/jszip.min.js
+-rw-r--r--   0 cy        (1000) cy        (1000)   210115 2024-01-16 13:46:16.000000 nanovar-1.6.2/nanovar/js/mdb.min.js
+-rw-r--r--   0 cy        (1000) cy        (1000)    19197 2024-01-16 13:46:16.000000 nanovar-1.6.2/nanovar/js/popper.min.js
+drwxr-xr-x   0 cy        (1000) cy        (1000)        0 2024-04-29 15:45:01.922109 nanovar-1.6.2/nanovar/model/
+-rw-r--r--   0 cy        (1000) cy        (1000)    22592 2024-01-16 13:46:16.000000 nanovar-1.6.2/nanovar/model/ANN.E100B400L3N12-5D0.4-0.2SGDsee11_het_ccs_v1.h5
+-rw-r--r--   0 cy        (1000) cy        (1000)    22592 2024-01-16 13:46:16.000000 nanovar-1.6.2/nanovar/model/ANN.E100B400L3N12-5D0.4-0.2SGDsee11_het_clr_v1.h5
+-rw-r--r--   0 cy        (1000) cy        (1000)    22592 2024-01-16 13:46:16.000000 nanovar-1.6.2/nanovar/model/ANN.E100B400L3N12-5D0.4-0.2SGDsee11_het_gup_v1.h5
+-rw-r--r--   0 cy        (1000) cy        (1000)        0 2024-01-16 13:46:16.000000 nanovar-1.6.2/nanovar/model/__init__.py
+-rw-r--r--   0 cy        (1000) cy        (1000)    24911 2024-01-16 13:46:16.000000 nanovar-1.6.2/nanovar/nanovar
+-rw-r--r--   0 cy        (1000) cy        (1000)     8262 2024-01-16 13:46:16.000000 nanovar-1.6.2/nanovar/nv_align.py
+-rw-r--r--   0 cy        (1000) cy        (1000)   833047 2024-04-29 15:44:35.000000 nanovar-1.6.2/nanovar/nv_bam_parser.c
+-rw-r--r--   0 cy        (1000) cy        (1000)    14668 2024-04-29 15:44:35.000000 nanovar-1.6.2/nanovar/nv_bam_parser.pyx
+-rw-r--r--   0 cy        (1000) cy        (1000)    11514 2024-01-16 13:46:16.000000 nanovar-1.6.2/nanovar/nv_characterize.py
+-rw-r--r--   0 cy        (1000) cy        (1000)    36161 2024-01-16 13:46:16.000000 nanovar-1.6.2/nanovar/nv_cluster.py
+-rw-r--r--   0 cy        (1000) cy        (1000)     5118 2024-01-16 13:46:16.000000 nanovar-1.6.2/nanovar/nv_cov_upper.py
+-rw-r--r--   0 cy        (1000) cy        (1000)    41821 2024-01-16 13:46:16.000000 nanovar-1.6.2/nanovar/nv_detect_algo.py
+-rw-r--r--   0 cy        (1000) cy        (1000)     9074 2024-01-16 13:46:16.000000 nanovar-1.6.2/nanovar/nv_dup_te_detect.py
+-rw-r--r--   0 cy        (1000) cy        (1000)     7524 2024-01-16 13:46:16.000000 nanovar-1.6.2/nanovar/nv_input.py
+-rw-r--r--   0 cy        (1000) cy        (1000)     8907 2024-01-16 13:46:16.000000 nanovar-1.6.2/nanovar/nv_nn.py
+-rw-r--r--   0 cy        (1000) cy        (1000)    28845 2024-01-16 13:46:16.000000 nanovar-1.6.2/nanovar/nv_parser.py
+-rw-r--r--   0 cy        (1000) cy        (1000)    25255 2024-01-16 13:46:16.000000 nanovar-1.6.2/nanovar/nv_report.py
+-rw-r--r--   0 cy        (1000) cy        (1000)     6431 2024-01-16 13:46:16.000000 nanovar-1.6.2/nanovar/nv_te_analyzer.py
+-rw-r--r--   0 cy        (1000) cy        (1000)     8826 2024-01-16 13:46:16.000000 nanovar-1.6.2/nanovar/nv_valid.py
+-rw-r--r--   0 cy        (1000) cy        (1000)    18511 2024-01-16 13:46:16.000000 nanovar-1.6.2/nanovar/nv_vcf.py
+drwxr-xr-x   0 cy        (1000) cy        (1000)        0 2024-04-29 15:45:01.922109 nanovar-1.6.2/nanovar/ref/
+-rw-r--r--   0 cy        (1000) cy        (1000)     8991 2024-01-16 13:46:16.000000 nanovar-1.6.2/nanovar/ref/hg38_L1_Alu.counts.obinary
+-rw-r--r--   0 cy        (1000) cy        (1000)     7707 2024-01-16 13:46:16.000000 nanovar-1.6.2/nanovar/ref/hg38_L1_Alu.fa
+-rw-r--r--   0 cy        (1000) cy        (1000)       22 2024-04-29 15:44:35.000000 nanovar-1.6.2/nanovar/version.py
+drwxr-xr-x   0 cy        (1000) cy        (1000)        0 2024-04-29 15:45:01.912109 nanovar-1.6.2/nanovar.egg-info/
+-rw-r--r--   0 cy        (1000) cy        (1000)    12900 2024-04-29 15:45:01.000000 nanovar-1.6.2/nanovar.egg-info/PKG-INFO
+-rw-r--r--   0 cy        (1000) cy        (1000)     1529 2024-04-29 15:45:01.000000 nanovar-1.6.2/nanovar.egg-info/SOURCES.txt
+-rw-r--r--   0 cy        (1000) cy        (1000)        1 2024-04-29 15:45:01.000000 nanovar-1.6.2/nanovar.egg-info/dependency_links.txt
+-rw-r--r--   0 cy        (1000) cy        (1000)      187 2024-04-29 15:45:01.000000 nanovar-1.6.2/nanovar.egg-info/requires.txt
+-rw-r--r--   0 cy        (1000) cy        (1000)        8 2024-04-29 15:45:01.000000 nanovar-1.6.2/nanovar.egg-info/top_level.txt
+-rw-r--r--   0 cy        (1000) cy        (1000)     1401 2024-01-16 13:46:16.000000 nanovar-1.6.2/requirements.txt
+-rw-r--r--   0 cy        (1000) cy        (1000)       79 2024-04-29 15:45:01.922109 nanovar-1.6.2/setup.cfg
+-rw-r--r--   0 cy        (1000) cy        (1000)     1758 2024-03-30 14:49:59.000000 nanovar-1.6.2/setup.py
```

### Comparing `nanovar-1.6.1/CHANGELOG.txt` & `nanovar-1.6.2/CHANGELOG.txt`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,17 @@
 NanoVar Changelog
 
 
 Release Summary:
 
 
+Version 1.6.2 - Apr 29, 2024
+    * Fixed bug where some supplementary alignments do not have primary alignments, in the case of a subsample BAM input
+
+
 Version 1.6.1 - Mar 30, 2024
     * Fix Tensorflow 2.16 compatibility issue, restrict tensorflow-cpu<=2.15.1 in setup.py
 
 
 Version 1.6.0 - Jan 15, 2024
     * Added NanoINSight INS annotation function (--annotate_ins [species])
     * Fixed NanoVar report scatter plot xaxis range
```

### Comparing `nanovar-1.6.1/LICENSE.txt` & `nanovar-1.6.2/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `nanovar-1.6.1/PKG-INFO` & `nanovar-1.6.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nanovar
-Version: 1.6.1
+Version: 1.6.2
 Summary: Structural variant caller using low-depth long reads
 Home-page: https://github.com/cytham/nanovar
 Download-URL: https://github.com/cytham/nanovar/releases
 Author: Tham Cheng Yong
 Author-email: chengyong.tham@u.nus.edu
 License: gpl-3.0
 Keywords: nanovar,structural variant caller,sv,nanopore,long read,low coverage,low depth
@@ -23,15 +23,15 @@
 Requires-Dist: tensorflow-cpu<=2.15.1,>=2.0.0
 Requires-Dist: natsort>=6.2.0
 Requires-Dist: progress>=1.4
 Requires-Dist: pysam>=0.15.3
 Requires-Dist: htmlark>=1.0.0
 Requires-Dist: nanoinsight>=0.0.3
 
-## Please note: Current v1.6.1 not compatible with Tensorflow >= 2.16.0, please downgrade to 2.15.1
+## Please note: Current v1.6.2 not compatible with Tensorflow >= 2.16.0, please downgrade to 2.15.1
 
 `pip install tensorflow-cpu==2.15.1`
 
 Please see issue [here](https://github.com/cytham/nanovar/issues/77)
 
 We are actively working on this, thank you for your understanding.
```

### Comparing `nanovar-1.6.1/README.md` & `nanovar-1.6.2/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-## Please note: Current v1.6.1 not compatible with Tensorflow >= 2.16.0, please downgrade to 2.15.1
+## Please note: Current v1.6.2 not compatible with Tensorflow >= 2.16.0, please downgrade to 2.15.1
 
 `pip install tensorflow-cpu==2.15.1`
 
 Please see issue [here](https://github.com/cytham/nanovar/issues/77)
 
 We are actively working on this, thank you for your understanding.
```

### Comparing `nanovar-1.6.1/nanovar/css/bootstrap.min.css` & `nanovar-1.6.2/nanovar/css/bootstrap.min.css`

 * *Files identical despite different names*

### Comparing `nanovar-1.6.1/nanovar/css/buttons.dataTables.min.css` & `nanovar-1.6.2/nanovar/css/buttons.dataTables.min.css`

 * *Files identical despite different names*

### Comparing `nanovar-1.6.1/nanovar/css/font-awesome.min.css` & `nanovar-1.6.2/nanovar/css/font-awesome.min.css`

 * *Files identical despite different names*

### Comparing `nanovar-1.6.1/nanovar/css/jquery.dataTables.min.css` & `nanovar-1.6.2/nanovar/css/jquery.dataTables.min.css`

 * *Files identical despite different names*

### Comparing `nanovar-1.6.1/nanovar/css/mdb.min.css` & `nanovar-1.6.2/nanovar/css/mdb.min.css`

 * *Files identical despite different names*

### Comparing `nanovar-1.6.1/nanovar/gaps/hg19_filter-B400.bed` & `nanovar-1.6.2/nanovar/gaps/hg19_filter-B400.bed`

 * *Files identical despite different names*

### Comparing `nanovar-1.6.1/nanovar/gaps/hg38_curated_filter_main.bed` & `nanovar-1.6.2/nanovar/gaps/hg38_curated_filter_main.bed`

 * *Files identical despite different names*

### Comparing `nanovar-1.6.1/nanovar/gaps/mm10_filter-B400.bed` & `nanovar-1.6.2/nanovar/gaps/mm10_filter-B400.bed`

 * *Files identical despite different names*

### Comparing `nanovar-1.6.1/nanovar/js/bootstrap.min.js` & `nanovar-1.6.2/nanovar/js/bootstrap.min.js`

 * *Files identical despite different names*

### Comparing `nanovar-1.6.1/nanovar/js/buttons.flash.min.js` & `nanovar-1.6.2/nanovar/js/buttons.flash.min.js`

 * *Files identical despite different names*

### Comparing `nanovar-1.6.1/nanovar/js/buttons.html5.min.js` & `nanovar-1.6.2/nanovar/js/buttons.html5.min.js`

 * *Files identical despite different names*

### Comparing `nanovar-1.6.1/nanovar/js/dataTables.buttons.min.js` & `nanovar-1.6.2/nanovar/js/dataTables.buttons.min.js`

 * *Files identical despite different names*

### Comparing `nanovar-1.6.1/nanovar/js/jquery-3.3.1.min.js` & `nanovar-1.6.2/nanovar/js/jquery-3.3.1.min.js`

 * *Files identical despite different names*

### Comparing `nanovar-1.6.1/nanovar/js/jquery.dataTables.min.js` & `nanovar-1.6.2/nanovar/js/jquery.dataTables.min.js`

 * *Files identical despite different names*

### Comparing `nanovar-1.6.1/nanovar/js/jszip.min.js` & `nanovar-1.6.2/nanovar/js/jszip.min.js`

 * *Files identical despite different names*

### Comparing `nanovar-1.6.1/nanovar/js/mdb.min.js` & `nanovar-1.6.2/nanovar/js/mdb.min.js`

 * *Files identical despite different names*

### Comparing `nanovar-1.6.1/nanovar/js/popper.min.js` & `nanovar-1.6.2/nanovar/js/popper.min.js`

 * *Files identical despite different names*

### Comparing `nanovar-1.6.1/nanovar/model/ANN.E100B400L3N12-5D0.4-0.2SGDsee11_het_ccs_v1.h5` & `nanovar-1.6.2/nanovar/model/ANN.E100B400L3N12-5D0.4-0.2SGDsee11_het_ccs_v1.h5`

 * *Files identical despite different names*

### Comparing `nanovar-1.6.1/nanovar/model/ANN.E100B400L3N12-5D0.4-0.2SGDsee11_het_clr_v1.h5` & `nanovar-1.6.2/nanovar/model/ANN.E100B400L3N12-5D0.4-0.2SGDsee11_het_clr_v1.h5`

 * *Files identical despite different names*

### Comparing `nanovar-1.6.1/nanovar/model/ANN.E100B400L3N12-5D0.4-0.2SGDsee11_het_gup_v1.h5` & `nanovar-1.6.2/nanovar/model/ANN.E100B400L3N12-5D0.4-0.2SGDsee11_het_gup_v1.h5`

 * *Files identical despite different names*

### Comparing `nanovar-1.6.1/nanovar/nanovar` & `nanovar-1.6.2/nanovar/nanovar`

 * *Files identical despite different names*

### Comparing `nanovar-1.6.1/nanovar/nv_align.py` & `nanovar-1.6.2/nanovar/nv_align.py`

 * *Files identical despite different names*

### Comparing `nanovar-1.6.1/nanovar/nv_bam_parser.pyx` & `nanovar-1.6.2/nanovar/nv_bam_parser.pyx`

 * *Files 1% similar despite different names*

```diff
@@ -103,17 +103,19 @@
             main_dict[qname].append((adv, qname, rname, rstart, rend, readlen, qlen, flag, nm, total_score, qseg, sseg, del_list,
             ins_list))
     for sup in add_sup_seq:
         try:
             if repeat_dict[sup]:
                 pass
         except KeyError:
-            repeat_dict[sup] = ''
-            fasta.write('>' + sup + '\n' + fail_qual_seq[sup] + '\n')
-            rlendict[sup] = fail_qual_len[sup] 
+            # Some supplementary alignments do not have primary alignments (in the case of a subset BAM), thus sequence not found and read sequence excluded
+            if sup in fail_qual_seq:
+                repeat_dict[sup] = ''
+                fasta.write('>' + sup + '\n' + fail_qual_seq[sup] + '\n')
+                rlendict[sup] = fail_qual_len[sup]
     fasta.close()
     fasta2.close()
     total_subdata, total_lines, contig_collect, total_out, detect_out = [], [], [], [], []
     # Make gap dictionary
     gapdict = makegapdict(filter_file, contig_omit)
     for qname in main_dict:
         if len(main_dict[qname]) == 1:  # Single alignment read
```

### Comparing `nanovar-1.6.1/nanovar/nv_characterize.py` & `nanovar-1.6.2/nanovar/nv_characterize.py`

 * *Files identical despite different names*

### Comparing `nanovar-1.6.1/nanovar/nv_cluster.py` & `nanovar-1.6.2/nanovar/nv_cluster.py`

 * *Files identical despite different names*

### Comparing `nanovar-1.6.1/nanovar/nv_cov_upper.py` & `nanovar-1.6.2/nanovar/nv_cov_upper.py`

 * *Files identical despite different names*

### Comparing `nanovar-1.6.1/nanovar/nv_detect_algo.py` & `nanovar-1.6.2/nanovar/nv_detect_algo.py`

 * *Files identical despite different names*

### Comparing `nanovar-1.6.1/nanovar/nv_dup_te_detect.py` & `nanovar-1.6.2/nanovar/nv_dup_te_detect.py`

 * *Files identical despite different names*

### Comparing `nanovar-1.6.1/nanovar/nv_input.py` & `nanovar-1.6.2/nanovar/nv_input.py`

 * *Files identical despite different names*

### Comparing `nanovar-1.6.1/nanovar/nv_nn.py` & `nanovar-1.6.2/nanovar/nv_nn.py`

 * *Files identical despite different names*

### Comparing `nanovar-1.6.1/nanovar/nv_parser.py` & `nanovar-1.6.2/nanovar/nv_parser.py`

 * *Files identical despite different names*

### Comparing `nanovar-1.6.1/nanovar/nv_report.py` & `nanovar-1.6.2/nanovar/nv_report.py`

 * *Files identical despite different names*

### Comparing `nanovar-1.6.1/nanovar/nv_te_analyzer.py` & `nanovar-1.6.2/nanovar/nv_te_analyzer.py`

 * *Files identical despite different names*

### Comparing `nanovar-1.6.1/nanovar/nv_valid.py` & `nanovar-1.6.2/nanovar/nv_valid.py`

 * *Files identical despite different names*

### Comparing `nanovar-1.6.1/nanovar/nv_vcf.py` & `nanovar-1.6.2/nanovar/nv_vcf.py`

 * *Files identical despite different names*

### Comparing `nanovar-1.6.1/nanovar/ref/hg38_L1_Alu.counts.obinary` & `nanovar-1.6.2/nanovar/ref/hg38_L1_Alu.counts.obinary`

 * *Files identical despite different names*

### Comparing `nanovar-1.6.1/nanovar/ref/hg38_L1_Alu.fa` & `nanovar-1.6.2/nanovar/ref/hg38_L1_Alu.fa`

 * *Files identical despite different names*

### Comparing `nanovar-1.6.1/nanovar.egg-info/PKG-INFO` & `nanovar-1.6.2/nanovar.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nanovar
-Version: 1.6.1
+Version: 1.6.2
 Summary: Structural variant caller using low-depth long reads
 Home-page: https://github.com/cytham/nanovar
 Download-URL: https://github.com/cytham/nanovar/releases
 Author: Tham Cheng Yong
 Author-email: chengyong.tham@u.nus.edu
 License: gpl-3.0
 Keywords: nanovar,structural variant caller,sv,nanopore,long read,low coverage,low depth
@@ -23,15 +23,15 @@
 Requires-Dist: tensorflow-cpu<=2.15.1,>=2.0.0
 Requires-Dist: natsort>=6.2.0
 Requires-Dist: progress>=1.4
 Requires-Dist: pysam>=0.15.3
 Requires-Dist: htmlark>=1.0.0
 Requires-Dist: nanoinsight>=0.0.3
 
-## Please note: Current v1.6.1 not compatible with Tensorflow >= 2.16.0, please downgrade to 2.15.1
+## Please note: Current v1.6.2 not compatible with Tensorflow >= 2.16.0, please downgrade to 2.15.1
 
 `pip install tensorflow-cpu==2.15.1`
 
 Please see issue [here](https://github.com/cytham/nanovar/issues/77)
 
 We are actively working on this, thank you for your understanding.
```

### Comparing `nanovar-1.6.1/nanovar.egg-info/SOURCES.txt` & `nanovar-1.6.2/nanovar.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `nanovar-1.6.1/requirements.txt` & `nanovar-1.6.2/requirements.txt`

 * *Files identical despite different names*

### Comparing `nanovar-1.6.1/setup.py` & `nanovar-1.6.2/setup.py`

 * *Files identical despite different names*

