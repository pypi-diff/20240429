# Comparing `tmp/vclean-0.0.0.tar.gz` & `tmp/vclean-0.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "vclean-0.0.0.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "vclean-0.0.1.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `vclean-0.0.0.tar` & `vclean-0.0.1.tar`

### file list

```diff
@@ -1,35 +1,33 @@
--rw-r--r--   0        0        0     3078 2024-04-29 06:45:12.904469 vclean-0.0.0/.gitignore
--rw-r--r--   0        0        0    35149 2024-04-29 05:52:14.809658 vclean-0.0.0/LICENSE
--rw-r--r--   0        0        0       54 2024-04-29 05:34:42.060128 vclean-0.0.0/README.md
--rwxr-xr-x   0        0        0    16587 2024-04-29 05:17:58.232413 vclean-0.0.0/bin/vclean_tmp.py
--rw-r--r--   0        0        0      424 2024-04-29 05:17:58.267934 vclean-0.0.0/db/single_pfam.txt
--rw-r--r--   0        0        0     1001 2024-04-29 05:17:58.268074 vclean-0.0.0/db/single_pfam_099.txt
--rw-r--r--   0        0        0      320 2024-04-29 05:17:58.268212 vclean-0.0.0/db/unique_single_pfam.txt
--rw-r--r--   0        0        0      239 2024-04-29 05:17:58.241660 vclean-0.0.0/environment.yml
--rwxr-xr-x   0        0        0   177885 2024-04-29 05:17:58.242173 vclean-0.0.0/models/best_lgb_model_fold0.txt
--rwxr-xr-x   0        0        0   178054 2024-04-29 05:17:58.242644 vclean-0.0.0/models/best_lgb_model_fold1.txt
--rwxr-xr-x   0        0        0   177968 2024-04-29 05:17:58.242412 vclean-0.0.0/models/best_lgb_model_fold2.txt
--rwxr-xr-x   0        0        0   177533 2024-04-29 05:17:58.243940 vclean-0.0.0/models/best_lgb_model_fold3.txt
--rwxr-xr-x   0        0        0   177279 2024-04-29 05:17:58.244187 vclean-0.0.0/models/best_lgb_model_fold4.txt
--rwxr-xr-x   0        0        0   890533 2024-04-29 05:17:58.243474 vclean-0.0.0/models/best_lgb_model_v1.3.2.pickle
--rw-r--r--   0        0        0      665 2024-04-29 06:29:36.659047 vclean-0.0.0/pyproject.toml
--rw-r--r--   0        0        0      237 2024-04-29 05:17:58.232035 vclean-0.0.0/setup.py
--rw-r--r--   0        0        0       84 2024-04-29 06:31:49.251875 vclean-0.0.0/vclean/__init__.py
--rw-r--r--   0        0        0     1949 2024-04-29 05:17:58.232734 vclean-0.0.0/vclean/cli.py
--rwxr-xr-x   0        0        0      344 2024-04-29 05:17:58.234664 vclean-0.0.0/vclean/modules/checkv.py
--rwxr-xr-x   0        0        0     1762 2024-04-29 05:17:58.233156 vclean-0.0.0/vclean/modules/cli.py
--rwxr-xr-x   0        0        0     1616 2024-04-29 05:17:58.233450 vclean-0.0.0/vclean/modules/codon.py
--rwxr-xr-x   0        0        0     1304 2024-04-29 05:17:58.234811 vclean-0.0.0/vclean/modules/count_redundant_protein.py
--rwxr-xr-x   0        0        0      643 2024-04-29 05:17:58.234377 vclean-0.0.0/vclean/modules/download_database.py
--rwxr-xr-x   0        0        0     1088 2024-04-29 05:17:58.234088 vclean-0.0.0/vclean/modules/download_database_for_cli.py
--rwxr-xr-x   0        0        0      697 2024-04-29 05:17:58.233598 vclean-0.0.0/vclean/modules/estimate_simu_contami.py
--rwxr-xr-x   0        0        0     1750 2024-04-29 05:17:58.234233 vclean-0.0.0/vclean/modules/gc.py
--rwxr-xr-x   0        0        0      981 2024-04-29 05:17:58.235276 vclean-0.0.0/vclean/modules/lgb_model.py
--rwxr-xr-x   0        0        0     1897 2024-04-29 05:17:58.233946 vclean-0.0.0/vclean/modules/penta_jelly.py
--rwxr-xr-x   0        0        0     7094 2024-04-29 05:17:58.238137 vclean-0.0.0/vclean/modules/read_table.py
--rwxr-xr-x   0        0        0    16457 2024-04-29 05:17:58.233772 vclean-0.0.0/vclean/modules/run.py
--rwxr-xr-x   0        0        0    18559 2024-04-29 05:17:58.235115 vclean-0.0.0/vclean/modules/run_for_cli.py
--rwxr-xr-x   0        0        0      404 2024-04-29 05:17:58.234953 vclean-0.0.0/vclean/modules/seqkit.py
--rwxr-xr-x   0        0        0     3615 2024-04-29 05:17:58.234520 vclean-0.0.0/vclean/modules/singlecopy_counts.py
--rwxr-xr-x   0        0        0     1893 2024-04-29 05:17:58.233305 vclean-0.0.0/vclean/modules/tetra_jelly.py
--rw-r--r--   0        0        0      681 1970-01-01 00:00:00.000000 vclean-0.0.0/PKG-INFO
+-rw-r--r--   0        0        0     3078 2024-04-29 06:45:12.904469 vclean-0.0.1/.gitignore
+-rw-r--r--   0        0        0    35149 2024-04-29 05:52:14.809658 vclean-0.0.1/LICENSE
+-rw-r--r--   0        0        0     1414 2024-04-29 07:48:13.129720 vclean-0.0.1/README.md
+-rw-r--r--   0        0        0      424 2024-04-29 05:17:58.267934 vclean-0.0.1/db/single_pfam.txt
+-rw-r--r--   0        0        0     1001 2024-04-29 05:17:58.268074 vclean-0.0.1/db/single_pfam_099.txt
+-rw-r--r--   0        0        0      320 2024-04-29 05:17:58.268212 vclean-0.0.1/db/unique_single_pfam.txt
+-rw-r--r--   0        0        0      239 2024-04-29 05:17:58.241660 vclean-0.0.1/environment.yml
+-rwxr-xr-x   0        0        0   177885 2024-04-29 05:17:58.242173 vclean-0.0.1/models/best_lgb_model_fold0.txt
+-rwxr-xr-x   0        0        0   178054 2024-04-29 05:17:58.242644 vclean-0.0.1/models/best_lgb_model_fold1.txt
+-rwxr-xr-x   0        0        0   177968 2024-04-29 05:17:58.242412 vclean-0.0.1/models/best_lgb_model_fold2.txt
+-rwxr-xr-x   0        0        0   177533 2024-04-29 05:17:58.243940 vclean-0.0.1/models/best_lgb_model_fold3.txt
+-rwxr-xr-x   0        0        0   177279 2024-04-29 05:17:58.244187 vclean-0.0.1/models/best_lgb_model_fold4.txt
+-rwxr-xr-x   0        0        0   890533 2024-04-29 05:17:58.243474 vclean-0.0.1/models/best_lgb_model_v1.3.2.pickle
+-rw-r--r--   0        0        0      585 2024-04-29 07:48:32.134138 vclean-0.0.1/pyproject.toml
+-rw-r--r--   0        0        0       84 2024-04-29 07:53:30.159701 vclean-0.0.1/vclean/__init__.py
+-rw-r--r--   0        0        0     1949 2024-04-29 05:17:58.232734 vclean-0.0.1/vclean/cli.py
+-rwxr-xr-x   0        0        0      344 2024-04-29 05:17:58.234664 vclean-0.0.1/vclean/modules/checkv.py
+-rwxr-xr-x   0        0        0     1762 2024-04-29 05:17:58.233156 vclean-0.0.1/vclean/modules/cli.py
+-rwxr-xr-x   0        0        0     1616 2024-04-29 05:17:58.233450 vclean-0.0.1/vclean/modules/codon.py
+-rwxr-xr-x   0        0        0     1304 2024-04-29 05:17:58.234811 vclean-0.0.1/vclean/modules/count_redundant_protein.py
+-rwxr-xr-x   0        0        0      643 2024-04-29 05:17:58.234377 vclean-0.0.1/vclean/modules/download_database.py
+-rwxr-xr-x   0        0        0     1088 2024-04-29 05:17:58.234088 vclean-0.0.1/vclean/modules/download_database_for_cli.py
+-rwxr-xr-x   0        0        0      697 2024-04-29 05:17:58.233598 vclean-0.0.1/vclean/modules/estimate_simu_contami.py
+-rwxr-xr-x   0        0        0     1750 2024-04-29 05:17:58.234233 vclean-0.0.1/vclean/modules/gc.py
+-rwxr-xr-x   0        0        0      981 2024-04-29 05:17:58.235276 vclean-0.0.1/vclean/modules/lgb_model.py
+-rwxr-xr-x   0        0        0     1897 2024-04-29 05:17:58.233946 vclean-0.0.1/vclean/modules/penta_jelly.py
+-rwxr-xr-x   0        0        0     7094 2024-04-29 05:17:58.238137 vclean-0.0.1/vclean/modules/read_table.py
+-rwxr-xr-x   0        0        0    16457 2024-04-29 05:17:58.233772 vclean-0.0.1/vclean/modules/run.py
+-rwxr-xr-x   0        0        0    18559 2024-04-29 05:17:58.235115 vclean-0.0.1/vclean/modules/run_for_cli.py
+-rwxr-xr-x   0        0        0      404 2024-04-29 05:17:58.234953 vclean-0.0.1/vclean/modules/seqkit.py
+-rwxr-xr-x   0        0        0     3615 2024-04-29 05:17:58.234520 vclean-0.0.1/vclean/modules/singlecopy_counts.py
+-rwxr-xr-x   0        0        0     1893 2024-04-29 05:17:58.233305 vclean-0.0.1/vclean/modules/tetra_jelly.py
+-rw-r--r--   0        0        0     1921 1970-01-01 00:00:00.000000 vclean-0.0.1/PKG-INFO
```

### Comparing `vclean-0.0.0/.gitignore` & `vclean-0.0.1/.gitignore`

 * *Files identical despite different names*

### Comparing `vclean-0.0.0/LICENSE` & `vclean-0.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `vclean-0.0.0/bin/vclean_tmp.py` & `vclean-0.0.1/vclean/modules/run.py`

 * *Files 6% similar despite different names*

```diff
@@ -11,24 +11,24 @@
 import glob
 import concurrent.futures
 import lightgbm as lgb
 from Bio import SeqIO
 import shutil
 
 # original scripts
-from scripts import seqkit as seqkit
-from scripts import checkv as checkv
-from scripts import gc as gc
-from scripts import tetra_jelly as tetra
-from scripts import penta_jelly as penta
-from scripts import codon as codon
-from scripts import estimate_simu_contami as contami
-from scripts import singlecopy_counts as scopy
-from scripts import count_redundant_protein as red_pr
-from scripts import lgb_model as lgb_model
+import seqkit as seqkit
+import checkv as checkv
+import gc as gc
+import tetra_jelly as tetra
+import penta_jelly as penta
+import codon as codon
+import estimate_simu_contami as contami
+import singlecopy_counts as scopy
+import count_redundant_protein as red_pr
+import lgb_model as lgb_model
 
 
 #################################################################################
 ############### Process for each file ###########################################
 #################################################################################
 def process_file(input_fasta, outdir, run_mode, tmpout, cpu, checkv_ref_dir,
                 input_protein, input_gene, trans_table):
@@ -160,15 +160,15 @@
 ############### Main  ###########################################################
 #################################################################################
 def main(argv=None):
     ap = argparse.ArgumentParser()
     ap.add_argument('-i', '--input', action='store', dest='input', help='Put the input fasta directory')
     ap.add_argument('-d', '--checv_ref', action='store', dest='checkv_dir', default='/home/wagatsuma/db/checkv_v1.0.1/checkv-db-v1.5')
     ap.add_argument('-tmp', action='store', dest='tmp', default='./tmp', help='Set the path of temporary file directory')
-    ap.add_argument('-t', '--threads', action='store', dest='threads', default='4', help='Put the number of CPU to use. default=4')
+    ap.add_argument('-t', '--threads', action='store', dest='threads', default='1', help='Put the number of CPU to use. default=1')
     ap.add_argument('-p', '--protein', action='store', dest='protein', default=None,
                     help='Not nessesary. you can input protein fasta file if you have. In default, vDeteCon predict CDS using prodigal from nucleotide fasta file.')
     ap.add_argument('-n', '--nucleotide', action='store', dest='gene', default=None)
     ap.add_argument('-o', '--output', action='store', dest='output', default='./output',
                     help='refer output directory')
     ap.add_argument('--translate_table', action='store', dest='t_table', default=11, help='put the translate table, default=11')
     ap.add_argument('-m', '--mode', action='store', dest='mode', default='F', help='True or False. If you want to calculate contamination value of simulation data, set this value True')
```

### Comparing `vclean-0.0.0/db/single_pfam_099.txt` & `vclean-0.0.1/db/single_pfam_099.txt`

 * *Files identical despite different names*

### Comparing `vclean-0.0.0/models/best_lgb_model_fold0.txt` & `vclean-0.0.1/models/best_lgb_model_fold0.txt`

 * *Files identical despite different names*

### Comparing `vclean-0.0.0/models/best_lgb_model_fold1.txt` & `vclean-0.0.1/models/best_lgb_model_fold1.txt`

 * *Files identical despite different names*

### Comparing `vclean-0.0.0/models/best_lgb_model_fold2.txt` & `vclean-0.0.1/models/best_lgb_model_fold2.txt`

 * *Files identical despite different names*

### Comparing `vclean-0.0.0/models/best_lgb_model_fold3.txt` & `vclean-0.0.1/models/best_lgb_model_fold3.txt`

 * *Files identical despite different names*

### Comparing `vclean-0.0.0/models/best_lgb_model_fold4.txt` & `vclean-0.0.1/models/best_lgb_model_fold4.txt`

 * *Files identical despite different names*

### Comparing `vclean-0.0.0/models/best_lgb_model_v1.3.2.pickle` & `vclean-0.0.1/models/best_lgb_model_v1.3.2.pickle`

 * *Files identical despite different names*

### Comparing `vclean-0.0.0/vclean/cli.py` & `vclean-0.0.1/vclean/cli.py`

 * *Files identical despite different names*

### Comparing `vclean-0.0.0/vclean/modules/cli.py` & `vclean-0.0.1/vclean/modules/cli.py`

 * *Files identical despite different names*

### Comparing `vclean-0.0.0/vclean/modules/codon.py` & `vclean-0.0.1/vclean/modules/codon.py`

 * *Files identical despite different names*

### Comparing `vclean-0.0.0/vclean/modules/count_redundant_protein.py` & `vclean-0.0.1/vclean/modules/count_redundant_protein.py`

 * *Files identical despite different names*

### Comparing `vclean-0.0.0/vclean/modules/download_database.py` & `vclean-0.0.1/vclean/modules/download_database.py`

 * *Files identical despite different names*

### Comparing `vclean-0.0.0/vclean/modules/download_database_for_cli.py` & `vclean-0.0.1/vclean/modules/download_database_for_cli.py`

 * *Files identical despite different names*

### Comparing `vclean-0.0.0/vclean/modules/estimate_simu_contami.py` & `vclean-0.0.1/vclean/modules/estimate_simu_contami.py`

 * *Files identical despite different names*

### Comparing `vclean-0.0.0/vclean/modules/gc.py` & `vclean-0.0.1/vclean/modules/gc.py`

 * *Files identical despite different names*

### Comparing `vclean-0.0.0/vclean/modules/lgb_model.py` & `vclean-0.0.1/vclean/modules/lgb_model.py`

 * *Files identical despite different names*

### Comparing `vclean-0.0.0/vclean/modules/penta_jelly.py` & `vclean-0.0.1/vclean/modules/penta_jelly.py`

 * *Files identical despite different names*

### Comparing `vclean-0.0.0/vclean/modules/read_table.py` & `vclean-0.0.1/vclean/modules/read_table.py`

 * *Files identical despite different names*

### Comparing `vclean-0.0.0/vclean/modules/run.py` & `vclean-0.0.1/vclean/modules/run_for_cli.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,43 +1,44 @@
 #!/usr/bin/env python
 
 import argparse
 import subprocess as sp
 import sys
 import random, string
 import os
+import time
 import pandas as pd
 import numpy as np
 import pickle
 import glob
 import concurrent.futures
 import lightgbm as lgb
 from Bio import SeqIO
 import shutil
 
 # original scripts
-import seqkit as seqkit
-import checkv as checkv
-import gc as gc
-import tetra_jelly as tetra
-import penta_jelly as penta
-import codon as codon
-import estimate_simu_contami as contami
-import singlecopy_counts as scopy
-import count_redundant_protein as red_pr
-import lgb_model as lgb_model
-
+# import seqkit as seqkit
+from modules import seqkit as seqkit
+from modules import checkv as checkv
+from modules import gc as gc
+from modules import tetra_jelly as tetra
+from modules import penta_jelly as penta
+from modules import codon as codon
+from modules import estimate_simu_contami as contami
+from modules import singlecopy_counts as scopy
+from modules import count_redundant_protein as red_pr
+from modules import lgb_model as lgb_model
 
 #################################################################################
 ############### Process for each file ###########################################
 #################################################################################
-def process_file(input_fasta, outdir, run_mode, tmpout, cpu, checkv_ref_dir,
-                input_protein, input_gene, trans_table):
-    pfamdb = "/home/wagatsuma/db/Pfam/Pfam-A_v35.0.hmm"
-    single_like_pfam = "/home/wagatsuma/analysis/virus/Tool/tmp/vDeteCon/db/single_pfam_099.txt"
+def process_file(input_fasta, outdir, run_mode, tmpout, cpu, checkv_db_dir, pfam_db,
+                input_protein, input_gene, trans_table, single_like_pfam):
+    gene_set_dir = os.path.dirname(os.path.dirname(os.path.dirname(os.path.abspath(__file__))))
+    single_like_pfam = os.path.join(gene_set_dir, 'db', 'single_pfam_099.txt')
 
     fasta_file_name = os.path.basename(input_fasta)
     basename = os.path.splitext(fasta_file_name)[0]
 
     sp.run(['mkdir', '-p', tmpout])
     random_val = ''.join(random.choices(string.ascii_letters + string.digits, k=15))
     tmp_dir = tmpout + "/" + random_val
@@ -60,15 +61,16 @@
     #                                run seqkit
     # --------------------------------------------------------------------------
     seqkit_list = seqkit.run_seqkit(input_fasta)
 
     # --------------------------------------------------------------------------
     #                                run checkV
     # --------------------------------------------------------------------------
-    sum_comp = checkv.run_checkv(input_fasta, tmp_dir, checkv_ref_dir, cpu)
+    sum_comp = checkv.run_checkv(input_fasta, tmp_dir, checkv_db_dir, cpu)
+    print("finish checkv")
 
     # --------------------------------------------------------------------------
     #                    gc-contents, gc-skew, cpg-contents 
     # --------------------------------------------------------------------------
     gc_table = gc.cal_gc_values(input_fasta)
     gc_res_6items = gc.gc_to_features(gc_table)
 
@@ -95,24 +97,24 @@
     if input_protein is None:
         protein_out = outdir + '/' + basename
         sp.run(['mkdir', '-p', protein_out])
         protein_fasta = protein_out + "/" +  basename + ".faa"
         gene_fasta = protein_out + "/" + basename + ".fna"
         gff_out = protein_out + "/" + basename + ".gff"
 
-        sp.run(['prodigal', '-i', input_fasta, '-p', 'meta', '-a', protein_fasta,  '-d', gene_fasta, '-o', gff_out, '-f', 'gff', '-g', trans_table])
+        sp.run(['prodigal', '-i', input_fasta, '-p', 'meta', '-a', protein_fasta,  '-d', gene_fasta, '-o', gff_out, '-f', 'gff', '-g', trans_table, '-q'])
     else:
         protein_fasta = input_protein
         gene_fasta = input_gene
 
     print("finish protein prediction")
     # --------------------------------------------------------------------------
     #                          Single-copy-like genes
     # --------------------------------------------------------------------------
-    hmm_tophit = scopy.run_hmm_pfam(protein_out, protein_fasta, basename, pfamdb, cpu)
+    hmm_tophit = scopy.run_hmm_pfam(protein_out, protein_fasta, basename, pfam_db, cpu)
     # num_single_like_overlaps = scopy.contraposition_single_copy(hmm_tophit, uniq_single_like_pfam)
     num_single_like_overlaps = scopy.contraposition_single_copy(hmm_tophit, single_like_pfam)
 
     # ----------------------protein redundancy -------------------------
     redundant_protein = red_pr.count_redundant_protein(protein_fasta, tmp_dir)
 
     # ------------------------ codon usage -----------------------------
@@ -122,128 +124,177 @@
 
     codon_res = [codon_pca, mm_codon_pca, codon_cos_mm]
 
     # --------------------------------------------------------------------------
     #                            Summary
     # --------------------------------------------------------------------------
     result_list = seqkit_list + sum_comp + gc_res_6items + tetra_res + penta_res + [num_single_like_overlaps] + codon_res + [redundant_protein]
-    print(result_list)
-
-    result_columns = ['num_seqs', 'sum_len', 'min_len', 'avg_len', 'sum_completeness', 'gc_var', 'gc_max_min', 'cpg_var', 'cpg_max_min', 'skew_var', 'skew_max_min', 'tetra_pca', 'mm_tetra_pca', 'tetra_cos_mm', 'penta_pca', 'mm_penta_pca', 'penta_cos_mm', 'overlap_singl_like_gene', 'codon_pca', 'mm_codon_pca', 'codon_cos_mm', 'redundant_protein']
+    result_columns = ['file', 'num_seqs', 'sum_len', 'min_len', 'avg_len', 'sum_completeness', 'gc_var', 'gc_max_min', 'cpg_var', 'cpg_max_min', 'skew_var', 'skew_max_min', 'tetra_pca', 'mm_tetra_pca', 'tetra_cos_mm', 'penta_pca', 'mm_penta_pca', 'penta_cos_mm', 'overlap_singl_like_gene', 'codon_pca', 'mm_codon_pca', 'codon_cos_mm', 'redundant_protein']
     result_df = pd.DataFrame(index=[], columns=result_columns)
+    result_list = [basename] + result_list
     add_series = pd.Series(result_list, index=result_df.columns, name=basename)
-    result_df = result_df.append(add_series)
-    print(result_df)
+    # result_df = result_df.append(add_series)
+    add_series = add_series.to_frame().T
+    result_df = pd.concat([result_df, add_series], ignore_index=True)
     result_path = outdir + '/' + basename + '_result.tsv'
-    result_df.to_csv(result_path, sep='\t')
+    result_df.to_csv(result_path, sep='\t', index=False)
     # --------------------------------------------------------------------------
     #                           Cleaning
     # --------------------------------------------------------------------------
     sp.run(['rm', '-r', tmp_dir])
 
 #################################################################################
 ############### parallel works  #################################################
 #################################################################################
-def process_files_in_folder(input_dir, outdir, run_mode, tmpout, cpu, checkv_ref_dir, input_protein, input_gene, trans_table):
+def process_files_in_folder(input_dir, outdir, run_mode, tmpout, cpu, checkv_db_dir, pfam_db, input_protein, input_gene, trans_table, single_like_pfam):
     # 出力ディレクトリを作成します
     os.makedirs(outdir, exist_ok=True)
 
     with concurrent.futures.ThreadPoolExecutor() as executor:
         # 各ファイルについて並列に処理を行います
-        futures = [executor.submit(process_file, entry.path, outdir, run_mode, tmpout, cpu, checkv_ref_dir, input_protein, input_gene, trans_table) for entry in os.scandir(input_dir) if entry.is_file()]
+        futures = [executor.submit(process_file, entry.path, outdir, run_mode, tmpout, cpu, checkv_db_dir, pfam_db, input_protein, input_gene, trans_table, single_like_pfam) for entry in os.scandir(input_dir) if entry.is_file()]
         for future in concurrent.futures.as_completed(futures):
             try:
                 future.result()
             except Exception as e:
                 print(f"Exception occurred while processing file: {e}")
 
 #################################################################################
 ############### Main  ###########################################################
 #################################################################################
-def main(argv=None):
-    ap = argparse.ArgumentParser()
-    ap.add_argument('-i', '--input', action='store', dest='input', help='Put the input fasta directory')
-    ap.add_argument('-d', '--checv_ref', action='store', dest='checkv_dir', default='/home/wagatsuma/db/checkv_v1.0.1/checkv-db-v1.5')
-    ap.add_argument('-tmp', action='store', dest='tmp', default='./tmp', help='Set the path of temporary file directory')
-    ap.add_argument('-t', '--threads', action='store', dest='threads', default='1', help='Put the number of CPU to use. default=1')
-    ap.add_argument('-p', '--protein', action='store', dest='protein', default=None,
+def fetch_arguments(parser):
+    parser.set_defaults(func=main)
+    parser.set_defaults(program="run")
+    
+    parser.add_argument('input', type=str, help='Put the input fasta directory')
+    parser.add_argument('output', type=str, help='Put the output directory')
+    parser.add_argument('-d', '--db', action='store', dest='db', help='Set the database directory path. By default the VCLEANDB environment vairable is used')
+    parser.add_argument('-tmp', action='store', dest='tmp', default='./tmp', help='Set the path of temporary file directory')
+    parser.add_argument('-t', '--threads', action='store', dest='threads', default='1', help='Put the number of CPU to use. default=1')
+    parser.add_argument('-p', '--protein', action='store', dest='protein', default=None,
                     help='Not nessesary. you can input protein fasta file if you have. In default, vDeteCon predict CDS using prodigal from nucleotide fasta file.')
-    ap.add_argument('-n', '--nucleotide', action='store', dest='gene', default=None)
-    ap.add_argument('-o', '--output', action='store', dest='output', default='./output',
-                    help='refer output directory')
-    ap.add_argument('--translate_table', action='store', dest='t_table', default=11, help='put the translate table, default=11')
-    ap.add_argument('-m', '--mode', action='store', dest='mode', default='F', help='True or False. If you want to calculate contamination value of simulation data, set this value True')
-    ap.add_argument('--skip_feature_table', action='store', dest='skip_feature_table', default=False, help='If you set True, skip features prediction step.')
-    ap.add_argument('--skip_lgb_step', action='store', dest='skip_lgb_step', default=False, help='If you set True, skip contamination prediction step.')
-    ap.add_argument('--f_table', action='store', dest='f_table', help="You want to only run lgb model, you have to input the features table path.")
-    ap.add_argument('-pr', '--threshold', action='store', dest='threshold', default=0.6, help='Put the threshold for the Contamination probability rate value. default=0.6. if the contamination probability value is over the set score, the input fasta are assigned as CONTAMINATION.')
-    args = ap.parse_args()
+    parser.add_argument('-n', '--nucleotide', action='store', dest='gene', default=None)
+    parser.add_argument('--translate_table', action='store', dest='t_table', default=11, help='put the translate table, default=11')
+    parser.add_argument('-m', '--mode', action='store', dest='mode', default='F', help='True or False. If you want to calculate contamination value of simulation data, set this value True')
+    parser.add_argument('--skip_feature_table', action='store', dest='skip_feature_table', default=False, help='If you set True, skip features prediction step.')
+    parser.add_argument('--skip_lgb_step', action='store', dest='skip_lgb_step', default=False, help='If you set True, skip contamination prediction step.')
+    parser.add_argument('--f_table', action='store', dest='f_table', help="You want to only run lgb model, you have to input the features table path.")
+    parser.add_argument('-pr', '--threshold', action='store', dest='threshold', default=0.6, help='Put the threshold for the Contamination probability rate value. default=0.6. if the contamination probability value is over the set score, the input fasta are assigned as CONTAMINATION.')
 
     # --------------------------------------------------------------------------
     # interproscan = "/home/mako43/packages/interproscan/interproscan-5.47-82.0/interproscan.sh"
     # single_like_pfam = "/home/wagatsuma/analysis/virus/Tool/tmp/vDeteCon/db/single_pfam.txt"
     # uniq_single_like_pfam = "/home/wagatsuma/analysis/virus/Tool/tmp/vDeteCon/db/unique_single_pfam.txt"
-
     # --------------------------------------------------------------------------
-    input_fasta_dir = args.input
-    checkv_ref_dir = args.checkv_dir
-    tmpout = args.tmp
-    cpu = args.threads
-    input_protein = args.protein
-    input_gene = args.gene
+
+def check_db(dbdir):
+    "check existence of database"
+    if dbdir is None:
+        if "VCLEANDB" not in os.environ:
+            msg="Error: database dir not specified\nUse -d or set VCLEANDB environmental variable"
+            sys.exit(msg)
+        else:
+            print("use VCLEANDB environmental variable")
+            dbdir = os.environ["VCLEANDB"]
+    dbdir = os.path.abspath(dbdir)
+    if not os.path.exists(dbdir):
+        msg = f"Error: database dir not found '{dbdir}'"
+        sys.exit(msg)
+
+    return dbdir
+
+def path_to_db(dbdir):
+    all_dbdir = os.listdir(dbdir)
+    # checkvdb
+    checkv_db_dir = None
+    for d in all_dbdir:
+        if d.startswith('checkv-db') and os.path.isdir(os.path.join(dbdir, d)):
+            checkv_db_dir = os.path.join(dbdir, d)
+            break
+    if checkv_db_dir:
+        print("Found checkv-db directory:", checkv_db_dir)
+    else:
+        msg = f"Error: No checkv-db directory found '{dbdir}'"
+        sys.exit(msg)
+    # pfamdb 
+    pfam_db = None
+    for d in all_dbdir:
+        if d.startswith('Pfam') and os.path.isdir(os.path.join(dbdir, d)):
+            pfam_db = os.path.join(dbdir, d, "Pfam-A.hmm")
+            break
+    if pfam_db:
+        print("Found pfam-db:", pfam_db)
+    else:
+        msg = f"Error: No pfam-db '{dbdir}'"
+        sys.exit(msg)
+
+    return checkv_db_dir, pfam_db
+
+def main(args):
+    program_start = time.time()
+    input_fasta_dir = args["input"]
+    tmpout = args["tmp"]
+    cpu = args["threads"]
+    input_protein = args["protein"]
+    input_gene = args["gene"]
     
-    final_out_dir = args.output
+    final_out_dir = args["output"]
     sp.run(['mkdir', '-p', final_out_dir])
-    outdir = final_out_dir + "/vDeteCon_tmp"
+    outdir = final_out_dir + "/vClean_tmp"
     out_fasta_dir = final_out_dir + "/purified_fasta"
     os.makedirs(outdir, exist_ok=True)
     os.makedirs(out_fasta_dir, exist_ok=True)
     
-    trans_table = str(args.t_table)
-    program_mode = args.mode
-    contami_threshold = args.threshold
-    f_table = args.f_table
+    trans_table = str(args["t_table"])
+    program_mode = args["mode"]
+    contami_threshold = args["threshold"]
+    f_table = args["f_table"]
+    db_dir = check_db(args["db"])
+    checkv_db_dir, pfam_db = path_to_db(db_dir)
+
+    gene_set_dir = os.path.dirname(os.path.dirname(os.path.dirname(os.path.abspath(__file__))))
+    single_like_pfam = os.path.join(gene_set_dir, 'db', 'single_pfam_099.txt')
 
     # --------------------------------------------------------------------------
     # sp.run(['mkdir', '-p', tmpout])
     # random_val = ''.join(random.choices(string.ascii_letters + string.digits, k=15))
     # tmp_dir = tmpout + "/" + random_val
     # sp.run(['mkdir', '-p', tmp_dir])
 
     # ------------------------- produce feature tables -------------------------------------
     
-    if args.skip_feature_table == False:
-        process_files_in_folder(input_fasta_dir, outdir, program_mode, tmpout, cpu, checkv_ref_dir, input_protein, input_gene, trans_table)
+    if args["skip_feature_table"] == False:
+        process_files_in_folder(input_fasta_dir, outdir, program_mode, tmpout, cpu, checkv_db_dir, pfam_db, input_protein, input_gene, trans_table, single_like_pfam)
         tsv_files = glob.glob(os.path.join(outdir, '*.tsv'))
-        print(tsv_files)
         result_dataframes = [pd.read_csv(file, sep='\t') for file in tsv_files]
-        features_table = pd.concat(result_dataframes, ignore_index=True).rename(columns={"Unnamed: 0": "file"})
+        features_table = pd.concat(result_dataframes, ignore_index=True)
         features_table_out_name = final_out_dir + "/features_result.tsv"
         features_table.to_csv(features_table_out_name, sep="\t", index=False)
     else:
         features_table_out_name = final_out_dir + "/features_result.tsv"
         feature_table = pd.read_csv(features_table_out_name, sep="\t")
     
     # --------------------------------------------------------------------------
     #                          Run lightgbm
     # --------------------------------------------------------------------------
     
-    if args.skip_lgb_step == False:
+    if args["skip_lgb_step"] == False:
         result_for_input = lgb_model.table_reformat(features_table)
     
         res_drop_columns =  ["penta_pca", "mm_codon_pca", "gc_max_min", "mm_penta_pca", "mm_tetra_pca", "tetra_cos_mm", "penta_cos_mm", "codon_cos_mm"]
         result_for_input = result_for_input.drop(res_drop_columns, axis=1)
 
         script_dir = os.path.dirname(os.path.abspath(__file__))
-        model_path = os.path.join(script_dir, 'models', 'best_lgb_model_v1.3.2.pickle')
+        model_dir = os.path.dirname(os.path.dirname(script_dir))
+        model_path = os.path.join(model_dir, 'models', 'best_lgb_model_v1.3.2.pickle')
 
         y_pred_proba_list = []
         for i in range(5):
             model_name = f'best_lgb_model_fold{i}.txt'
-            model_path = os.path.join(script_dir, 'models', model_name)
+            model_path = os.path.join(model_dir, 'models', model_name)
             loaded_model = lgb.Booster(model_file=model_path)
             y_pred_proba = loaded_model.predict(result_for_input)
             y_pred_proba_list.append(y_pred_proba)
     
         y_pred_proba_avg = np.array(y_pred_proba_list).mean(axis=0)
         y_pred = np.where(y_pred_proba_avg >= float(contami_threshold), 1, 0)
     
@@ -254,26 +305,26 @@
                                 'y_pred4':y_pred_proba_list[3],
                                 'y_pred5':y_pred_proba_list[4],
                                 'result_prediction': y_pred,
                                 'y_ave':y_pred_proba_avg})
         # contamination_probability_result = pd.merge(contamination_probability_result_over2contigs, features_table['file'], on='file', how='right')
         # column_to_fill = ['y_pred1', 'y_pred2', 'y_pred3', 'y_pred4', 'y_pred5', 'result_prediction', 'y_ave']
         # contamination_probability_result[columns_to_fill] = contamination_probability_result[columns_to_fill].fillna(0)
-        contamination_probability_result = contamination_probability_result.assign(file=contamination_probability_result.file.str.replace(r'_edit$', ''))
+        print(contamination_probability_result)
+        # contamination_probability_result = contamination_probability_result.assign(file=contamination_probability_result.file.str)
         contami_prob_res_name = final_out_dir + "/Contamination_probability.tsv"
         contamination_probability_result.to_csv(contami_prob_res_name, sep="\t", index=False)
     else:
         contami_prob_res_name = final_out_dir + "/Contamination_probability.tsv"
         contamination_probability_result = pd.read_csv(contami_prob_res_name, sep="\t")
 
     # --------------------------------------------------------------------------
     #                        Purifying vMAGs and vSAGs
     # --------------------------------------------------------------------------
     purification_target_list = contamination_probability_result[contamination_probability_result['result_prediction']==1]['file'].tolist()
-    print(purification_target_list)
     for fasta_file in os.listdir(input_fasta_dir):
         file_path = os.path.join(input_fasta_dir, fasta_file)
 
         # parse the fasta file
         records = list(SeqIO.parse(file_path, 'fasta'))
         basename = os.path.splitext(fasta_file)[0]
         """
```

### Comparing `vclean-0.0.0/vclean/modules/singlecopy_counts.py` & `vclean-0.0.1/vclean/modules/singlecopy_counts.py`

 * *Files identical despite different names*

### Comparing `vclean-0.0.0/vclean/modules/tetra_jelly.py` & `vclean-0.0.1/vclean/modules/tetra_jelly.py`

 * *Files identical despite different names*

