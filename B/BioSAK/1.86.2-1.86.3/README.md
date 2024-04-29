# Comparing `tmp/BioSAK-1.86.2.tar.gz` & `tmp/BioSAK-1.86.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "BioSAK-1.86.2.tar", last modified: Sun Apr 28 15:18:15 2024, max compression
+gzip compressed data, was "BioSAK-1.86.3.tar", last modified: Mon Apr 29 00:08:39 2024, max compression
```

## Comparing `BioSAK-1.86.2.tar` & `BioSAK-1.86.3.tar`

### file list

```diff
@@ -1,164 +1,164 @@
-drwxr-xr-x   0 songweizhi   (501) staff       (20)        0 2024-04-28 15:18:15.240574 BioSAK-1.86.2/
-drwxr-xr-x   0 songweizhi   (501) staff       (20)        0 2024-04-28 15:18:15.238346 BioSAK-1.86.2/BioSAK/
--rw-r--r--   0 songweizhi   (501) staff       (20)     3653 2024-01-16 05:10:59.000000 BioSAK-1.86.2/BioSAK/BLCA_op_parser.py
--rw-r--r--   0 songweizhi   (501) staff       (20)     2031 2023-05-31 05:26:00.000000 BioSAK-1.86.2/BioSAK/BioSAK_config.py
--rwxr-xr-x   0 songweizhi   (501) staff       (20)    39300 2024-03-22 00:45:31.000000 BioSAK-1.86.2/BioSAK/COG2020.py
--rw-r--r--   0 songweizhi   (501) staff       (20)     3615 2023-05-09 01:09:35.000000 BioSAK-1.86.2/BioSAK/COG_boxplot_last1row.R
--rw-r--r--   0 songweizhi   (501) staff       (20)     6974 2023-05-09 01:09:35.000000 BioSAK-1.86.2/BioSAK/COG_boxplot_last2row.R
--rwxr-xr-x   0 songweizhi   (501) staff       (20)     6067 2024-01-16 05:00:13.000000 BioSAK-1.86.2/BioSAK/CheckM.py
--rw-r--r--   0 songweizhi   (501) staff       (20)     5891 2024-01-16 05:10:59.000000 BioSAK-1.86.2/BioSAK/ConvertMSA.py
--rw-r--r--   0 songweizhi   (501) staff       (20)    16671 2023-05-09 01:09:35.000000 BioSAK-1.86.2/BioSAK/DnaFeaturesViewer.py
--rw-r--r--   0 songweizhi   (501) staff       (20)     2292 2023-05-09 01:09:35.000000 BioSAK-1.86.2/BioSAK/FastaSplitler_by_num.py
--rw-r--r--   0 songweizhi   (501) staff       (20)     2485 2023-05-09 01:09:35.000000 BioSAK-1.86.2/BioSAK/FastaSplitler_by_size.py
--rw-r--r--   0 songweizhi   (501) staff       (20)     2190 2023-05-09 01:09:35.000000 BioSAK-1.86.2/BioSAK/GTDB_for_BLCA.py
--rw-r--r--   0 songweizhi   (501) staff       (20)     1321 2023-05-09 01:09:35.000000 BioSAK-1.86.2/BioSAK/Gene2Ctg.py
--rw-r--r--   0 songweizhi   (501) staff       (20)    45147 2024-03-23 14:54:03.000000 BioSAK-1.86.2/BioSAK/KEGG.py
--rw-r--r--   0 songweizhi   (501) staff       (20)     3484 2023-05-09 01:09:35.000000 BioSAK-1.86.2/BioSAK/KEGG_boxplot_last1row.R
--rw-r--r--   0 songweizhi   (501) staff       (20)      269 2023-05-09 01:09:35.000000 BioSAK-1.86.2/BioSAK/KEGG_get_eukaryotic_kos.py
--rw-r--r--   0 songweizhi   (501) staff       (20)     3077 2023-08-22 09:31:28.000000 BioSAK-1.86.2/BioSAK/KeepRemovingTmp.py
--rw-r--r--   0 songweizhi   (501) staff       (20)     2620 2024-01-16 05:10:59.000000 BioSAK-1.86.2/BioSAK/MeanMappingDepth.py
--rw-r--r--   0 songweizhi   (501) staff       (20)     3682 2024-01-16 12:39:58.000000 BioSAK-1.86.2/BioSAK/MetaBiosample.py
--rw-r--r--   0 songweizhi   (501) staff       (20)  3297822 2023-05-09 01:09:35.000000 BioSAK-1.86.2/BioSAK/MetaCHIP_phylo.hmm
--rw-r--r--   0 songweizhi   (501) staff       (20)  1206805 2023-05-09 01:09:35.000000 BioSAK-1.86.2/BioSAK/MetaCyc_reactions_with_ec.txt
--rw-r--r--   0 songweizhi   (501) staff       (20)    16960 2023-05-09 01:09:35.000000 BioSAK-1.86.2/BioSAK/NetEnzymes.py
--rw-r--r--   0 songweizhi   (501) staff       (20)     3713 2023-05-09 01:09:35.000000 BioSAK-1.86.2/BioSAK/Newick_tree_plotter.py
--rw-r--r--   0 songweizhi   (501) staff       (20)     1659 2024-01-16 05:10:59.000000 BioSAK-1.86.2/BioSAK/OneLineAln.py
--rw-r--r--   0 songweizhi   (501) staff       (20)    10448 2023-05-09 01:09:35.000000 BioSAK-1.86.2/BioSAK/Prodigal.py
--rw-r--r--   0 songweizhi   (501) staff       (20)     6048 2023-05-09 01:09:35.000000 BioSAK-1.86.2/BioSAK/Reads_simulator.py
--rw-r--r--   0 songweizhi   (501) staff       (20)     3573 2024-01-16 05:10:59.000000 BioSAK-1.86.2/BioSAK/RunGraphMB.py
--rw-r--r--   0 songweizhi   (501) staff       (20)     3833 2024-01-16 05:10:59.000000 BioSAK-1.86.2/BioSAK/SILVA_for_BLCA.py
--rwxr-xr-x   0 songweizhi   (501) staff       (20)     6255 2023-05-09 01:09:35.000000 BioSAK-1.86.2/BioSAK/SankeyTaxon.py
--rw-r--r--   0 songweizhi   (501) staff       (20)     5678 2024-01-16 05:10:59.000000 BioSAK-1.86.2/BioSAK/SliceMSA.py
--rw-r--r--   0 songweizhi   (501) staff       (20)     3173 2024-01-16 05:10:59.000000 BioSAK-1.86.2/BioSAK/SubsampleLongReads.py
--rwxr-xr-x   0 songweizhi   (501) staff       (20)     1696 2024-01-16 05:10:59.000000 BioSAK-1.86.2/BioSAK/Tax4Fun2IndOTU.py
--rw-r--r--   0 songweizhi   (501) staff       (20)     3619 2024-04-28 15:18:12.000000 BioSAK-1.86.2/BioSAK/VERSION
--rw-r--r--   0 songweizhi   (501) staff       (20)      467 2023-05-09 01:09:35.000000 BioSAK-1.86.2/BioSAK/VisBlastOp.py
--rw-r--r--   0 songweizhi   (501) staff       (20)     9944 2023-05-09 01:09:35.000000 BioSAK-1.86.2/BioSAK/VisGeneFlk.py
--rwxr-xr-x   0 songweizhi   (501) staff       (20)        0 2023-05-09 01:09:35.000000 BioSAK-1.86.2/BioSAK/__init__.py
--rw-r--r--   0 songweizhi   (501) staff       (20)     2526 2024-03-25 14:00:14.000000 BioSAK-1.86.2/BioSAK/add_desc.py
--rwxr-xr-x   0 songweizhi   (501) staff       (20)    38577 2024-03-22 00:45:31.000000 BioSAK-1.86.2/BioSAK/arCOG.py
--rw-r--r--   0 songweizhi   (501) staff       (20)     6985 2024-01-16 05:00:13.000000 BioSAK-1.86.2/BioSAK/bam2reads.py
--rwxr-xr-x   0 songweizhi   (501) staff       (20)     2630 2024-03-22 13:23:45.000000 BioSAK-1.86.2/BioSAK/boxplot.py
--rw-r--r--   0 songweizhi   (501) staff       (20)     3312 2023-05-09 01:09:35.000000 BioSAK-1.86.2/BioSAK/boxplot_last1row.R
--rw-r--r--   0 songweizhi   (501) staff       (20)     6104 2023-05-09 01:09:35.000000 BioSAK-1.86.2/BioSAK/boxplot_matrix_COG.py
--rw-r--r--   0 songweizhi   (501) staff       (20)     5403 2023-05-09 01:09:35.000000 BioSAK-1.86.2/BioSAK/boxplot_matrix_COG_backup.py
--rw-r--r--   0 songweizhi   (501) staff       (20)     6984 2023-05-09 01:09:35.000000 BioSAK-1.86.2/BioSAK/boxplot_matrix_KEGG.py
--rw-r--r--   0 songweizhi   (501) staff       (20)     5747 2023-05-09 01:09:35.000000 BioSAK-1.86.2/BioSAK/boxplot_matrix_dbCAN.py
--rw-r--r--   0 songweizhi   (501) staff       (20)     1695 2023-05-09 01:09:35.000000 BioSAK-1.86.2/BioSAK/cat_fa.py
--rw-r--r--   0 songweizhi   (501) staff       (20)    13440 2023-05-09 01:09:35.000000 BioSAK-1.86.2/BioSAK/cdd2cog.pl
--rw-r--r--   0 songweizhi   (501) staff       (20)     1186 2023-05-09 01:09:35.000000 BioSAK-1.86.2/BioSAK/checkm_marker.py
--rw-r--r--   0 songweizhi   (501) staff       (20)     1076 2023-05-09 01:09:35.000000 BioSAK-1.86.2/BioSAK/compare_trees.R
--rw-r--r--   0 songweizhi   (501) staff       (20)     9745 2024-01-16 05:10:59.000000 BioSAK-1.86.2/BioSAK/compare_trees.py
--rw-r--r--   0 songweizhi   (501) staff       (20)     6592 2023-05-09 01:09:35.000000 BioSAK-1.86.2/BioSAK/cross_link_seqs.py
--rw-r--r--   0 songweizhi   (501) staff       (20)    24033 2024-03-22 00:45:31.000000 BioSAK-1.86.2/BioSAK/dbCAN.py
--rw-r--r--   0 songweizhi   (501) staff       (20)     1936 2023-05-09 01:09:35.000000 BioSAK-1.86.2/BioSAK/download_GenBank_genome_subset_prokaryotes_csv.py
--rw-r--r--   0 songweizhi   (501) staff       (20)      767 2023-05-09 01:09:35.000000 BioSAK-1.86.2/BioSAK/dwnld_sra_reads.py
--rwxr-xr-x   0 songweizhi   (501) staff       (20)    13250 2024-03-22 08:01:22.000000 BioSAK-1.86.2/BioSAK/enrich.py
--rw-r--r--   0 songweizhi   (501) staff       (20)      929 2023-05-09 01:09:35.000000 BioSAK-1.86.2/BioSAK/exe_cmds.py
--rw-r--r--   0 songweizhi   (501) staff       (20)     1508 2023-12-05 01:06:39.000000 BioSAK-1.86.2/BioSAK/ezaai2mat.py
--rw-r--r--   0 songweizhi   (501) staff       (20)     1396 2023-12-05 01:02:55.000000 BioSAK-1.86.2/BioSAK/fa2id.py
--rw-r--r--   0 songweizhi   (501) staff       (20)     1195 2023-05-17 06:14:50.000000 BioSAK-1.86.2/BioSAK/fa2phy.py
--rw-r--r--   0 songweizhi   (501) staff       (20)     1363 2023-05-09 01:09:35.000000 BioSAK-1.86.2/BioSAK/fa2tree.py
--rw-r--r--   0 songweizhi   (501) staff       (20)     6280 2023-05-09 01:09:35.000000 BioSAK-1.86.2/BioSAK/format_converter.py
--rwxr-xr-x   0 songweizhi   (501) staff       (20)     2861 2023-05-09 01:09:35.000000 BioSAK-1.86.2/BioSAK/format_leaf_name.py
--rw-r--r--   0 songweizhi   (501) staff       (20)      639 2023-05-09 01:09:35.000000 BioSAK-1.86.2/BioSAK/fq2fa.py
--rw-r--r--   0 songweizhi   (501) staff       (20)     3204 2024-04-19 15:04:59.000000 BioSAK-1.86.2/BioSAK/gapseq.py
--rw-r--r--   0 songweizhi   (501) staff       (20)     2846 2023-06-14 10:08:30.000000 BioSAK-1.86.2/BioSAK/gbk2faa.py
--rw-r--r--   0 songweizhi   (501) staff       (20)     3342 2023-06-14 10:14:13.000000 BioSAK-1.86.2/BioSAK/gbk2ffn.py
--rw-r--r--   0 songweizhi   (501) staff       (20)     2528 2023-05-09 01:09:35.000000 BioSAK-1.86.2/BioSAK/gbk2fna.py
--rw-r--r--   0 songweizhi   (501) staff       (20)     3726 2023-05-09 01:09:35.000000 BioSAK-1.86.2/BioSAK/gbk_to_ffn_faa.py
--rw-r--r--   0 songweizhi   (501) staff       (20)     1887 2024-04-15 02:59:40.000000 BioSAK-1.86.2/BioSAK/gc.py
--rw-r--r--   0 songweizhi   (501) staff       (20)      813 2023-05-09 01:09:35.000000 BioSAK-1.86.2/BioSAK/get_EC_from_ko_stats_D.py
--rw-r--r--   0 songweizhi   (501) staff       (20)     7477 2023-05-09 01:09:35.000000 BioSAK-1.86.2/BioSAK/get_GTDB_taxon_gnm.py
--rw-r--r--   0 songweizhi   (501) staff       (20)     5428 2023-06-15 03:03:02.000000 BioSAK-1.86.2/BioSAK/get_MAG_reads_long.py
--rw-r--r--   0 songweizhi   (501) staff       (20)     3991 2023-05-09 01:09:35.000000 BioSAK-1.86.2/BioSAK/get_Pfam_hmms.py
--rw-r--r--   0 songweizhi   (501) staff       (20)    29246 2023-05-09 01:09:35.000000 BioSAK-1.86.2/BioSAK/get_SCG_tree.py
--rw-r--r--   0 songweizhi   (501) staff       (20)     1784 2023-05-09 01:09:35.000000 BioSAK-1.86.2/BioSAK/get_TopHits_taxonomy.py
--rw-r--r--   0 songweizhi   (501) staff       (20)     2247 2023-05-09 01:09:35.000000 BioSAK-1.86.2/BioSAK/get_aa_composition.py
--rw-r--r--   0 songweizhi   (501) staff       (20)    12066 2023-05-09 01:09:35.000000 BioSAK-1.86.2/BioSAK/get_bin_abundance copy.py
--rw-r--r--   0 songweizhi   (501) staff       (20)     2139 2024-01-23 11:57:14.000000 BioSAK-1.86.2/BioSAK/get_data_matrix.py
--rw-r--r--   0 songweizhi   (501) staff       (20)     5523 2023-05-09 01:09:35.000000 BioSAK-1.86.2/BioSAK/get_gene_depth.py
--rw-r--r--   0 songweizhi   (501) staff       (20)     3591 2024-01-16 05:10:59.000000 BioSAK-1.86.2/BioSAK/get_genome_GTDB.py
--rw-r--r--   0 songweizhi   (501) staff       (20)     6070 2024-01-16 04:57:23.000000 BioSAK-1.86.2/BioSAK/get_genome_NCBI.py
--rw-r--r--   0 songweizhi   (501) staff       (20)    11209 2023-05-09 01:09:35.000000 BioSAK-1.86.2/BioSAK/get_genome_NCBI_v1.py
--rw-r--r--   0 songweizhi   (501) staff       (20)    12620 2023-05-09 01:09:35.000000 BioSAK-1.86.2/BioSAK/get_genome_NCBI_v2.py
--rw-r--r--   0 songweizhi   (501) staff       (20)     3048 2023-05-09 01:09:35.000000 BioSAK-1.86.2/BioSAK/get_gnm_size.py
--rw-r--r--   0 songweizhi   (501) staff       (20)     4834 2023-05-09 01:09:35.000000 BioSAK-1.86.2/BioSAK/get_ko_gene_seqs.py
--rw-r--r--   0 songweizhi   (501) staff       (20)     1192 2023-09-21 08:44:42.000000 BioSAK-1.86.2/BioSAK/get_krona_plot.py
--rw-r--r--   0 songweizhi   (501) staff       (20)     1559 2023-05-09 01:09:35.000000 BioSAK-1.86.2/BioSAK/get_reads_from_sam.py
--rw-r--r--   0 songweizhi   (501) staff       (20)      792 2023-05-09 01:09:35.000000 BioSAK-1.86.2/BioSAK/get_reads_id_in_sam.py
--rw-r--r--   0 songweizhi   (501) staff       (20)     2386 2023-05-09 01:09:35.000000 BioSAK-1.86.2/BioSAK/get_sankey_plot.R
--rw-r--r--   0 songweizhi   (501) staff       (20)     4242 2023-05-09 01:09:35.000000 BioSAK-1.86.2/BioSAK/get_top_hit.py
--rw-r--r--   0 songweizhi   (501) staff       (20)      820 2023-05-09 01:09:35.000000 BioSAK-1.86.2/BioSAK/get_total_length.py
--rw-r--r--   0 songweizhi   (501) staff       (20)     4643 2023-05-18 01:37:58.000000 BioSAK-1.86.2/BioSAK/global_functions.py
--rwxr-xr-x   0 songweizhi   (501) staff       (20)     2910 2024-03-11 00:57:02.000000 BioSAK-1.86.2/BioSAK/hpc3.py
--rw-r--r--   0 songweizhi   (501) staff       (20)    26872 2024-04-12 00:51:29.000000 BioSAK-1.86.2/BioSAK/iTOL.py
--rw-r--r--   0 songweizhi   (501) staff       (20)     3337 2024-03-07 03:01:35.000000 BioSAK-1.86.2/BioSAK/js_cmds.py
--rw-r--r--   0 songweizhi   (501) staff       (20)     3281 2024-04-08 09:48:49.000000 BioSAK-1.86.2/BioSAK/js_hpc3.py
--rw-r--r--   0 songweizhi   (501) staff       (20)     1643 2023-05-09 01:09:35.000000 BioSAK-1.86.2/BioSAK/keep_best_hit.py
--rw-r--r--   0 songweizhi   (501) staff       (20)  3361029 2023-05-09 01:09:35.000000 BioSAK-1.86.2/BioSAK/ko00001.keg
--rw-r--r--   0 songweizhi   (501) staff       (20)     1848 2024-03-10 15:18:30.000000 BioSAK-1.86.2/BioSAK/koala.py
--rw-r--r--   0 songweizhi   (501) staff       (20)     2772 2023-05-09 01:09:35.000000 BioSAK-1.86.2/BioSAK/label_tree.R
--rw-r--r--   0 songweizhi   (501) staff       (20)     4788 2024-01-16 05:10:59.000000 BioSAK-1.86.2/BioSAK/label_tree.py
--rw-r--r--   0 songweizhi   (501) staff       (20)    35857 2023-05-09 01:09:35.000000 BioSAK-1.86.2/BioSAK/link_16S_MAG.py
--rw-r--r--   0 songweizhi   (501) staff       (20)    12349 2023-05-09 01:09:35.000000 BioSAK-1.86.2/BioSAK/magabund.py
--rw-r--r--   0 songweizhi   (501) staff       (20)    19855 2023-05-09 01:09:35.000000 BioSAK-1.86.2/BioSAK/magabund2.py
--rw-r--r--   0 songweizhi   (501) staff       (20)     1224 2023-05-09 01:09:35.000000 BioSAK-1.86.2/BioSAK/manipulator_fasta.py
--rw-r--r--   0 songweizhi   (501) staff       (20)        0 2023-05-09 01:09:35.000000 BioSAK-1.86.2/BioSAK/manipulator_msa.py
--rw-r--r--   0 songweizhi   (501) staff       (20)     3659 2023-05-09 01:09:35.000000 BioSAK-1.86.2/BioSAK/manipulator_newick.py
--rw-r--r--   0 songweizhi   (501) staff       (20)        0 2023-05-09 01:09:35.000000 BioSAK-1.86.2/BioSAK/manipulator_sam.py
--rw-r--r--   0 songweizhi   (501) staff       (20)      903 2024-04-17 08:12:49.000000 BioSAK-1.86.2/BioSAK/mannwhitneyu.py
--rw-r--r--   0 songweizhi   (501) staff       (20)     2433 2023-05-30 01:59:44.000000 BioSAK-1.86.2/BioSAK/mean_MAG_cov.py
--rw-r--r--   0 songweizhi   (501) staff       (20)     1880 2024-03-25 06:45:20.000000 BioSAK-1.86.2/BioSAK/merge_df.py
--rw-r--r--   0 songweizhi   (501) staff       (20)     2405 2024-01-16 05:10:59.000000 BioSAK-1.86.2/BioSAK/merge_seq.py
--rw-r--r--   0 songweizhi   (501) staff       (20)     6742 2024-01-23 07:37:01.000000 BioSAK-1.86.2/BioSAK/metaAssembly.py
--rw-r--r--   0 songweizhi   (501) staff       (20)     1327 2023-06-11 13:56:21.000000 BioSAK-1.86.2/BioSAK/metabat2concoct.py
--rw-r--r--   0 songweizhi   (501) staff       (20)     1612 2023-06-11 16:00:51.000000 BioSAK-1.86.2/BioSAK/metabat2maxbin.py
--rw-r--r--   0 songweizhi   (501) staff       (20)        0 2023-05-09 01:09:35.000000 BioSAK-1.86.2/BioSAK/msa_to_distance_matrix.py
--rw-r--r--   0 songweizhi   (501) staff       (20)     1759 2023-05-09 01:09:35.000000 BioSAK-1.86.2/BioSAK/ncbi_dataset.py
--rw-r--r--   0 songweizhi   (501) staff       (20)        0 2024-03-03 11:00:02.000000 BioSAK-1.86.2/BioSAK/odp.py
--rw-r--r--   0 songweizhi   (501) staff       (20)     2820 2023-05-09 01:09:35.000000 BioSAK-1.86.2/BioSAK/parse_MetaCyc_RxnDB.py
--rw-r--r--   0 songweizhi   (501) staff       (20)     1460 2023-09-18 14:42:31.000000 BioSAK-1.86.2/BioSAK/parse_mmseqs_tsv.py
--rw-r--r--   0 songweizhi   (501) staff       (20)     8633 2024-01-16 05:10:59.000000 BioSAK-1.86.2/BioSAK/plot_mag.py
--rw-r--r--   0 songweizhi   (501) staff       (20)     7332 2023-05-09 01:09:35.000000 BioSAK-1.86.2/BioSAK/plot_sam_depth.py
--rw-r--r--   0 songweizhi   (501) staff       (20)     1638 2023-05-09 01:09:35.000000 BioSAK-1.86.2/BioSAK/plot_tree.R
--rw-r--r--   0 songweizhi   (501) staff       (20)     2256 2023-07-22 00:36:16.000000 BioSAK-1.86.2/BioSAK/prefix_file.py
--rw-r--r--   0 songweizhi   (501) staff       (20)     4221 2024-01-16 05:10:59.000000 BioSAK-1.86.2/BioSAK/prokka.py
--rw-r--r--   0 songweizhi   (501) staff       (20)     5057 2023-08-03 02:58:56.000000 BioSAK-1.86.2/BioSAK/reads2bam.py
--rwxr-xr-x   0 songweizhi   (501) staff       (20)     2534 2023-05-09 01:09:35.000000 BioSAK-1.86.2/BioSAK/rename_leaves.py
--rw-r--r--   0 songweizhi   (501) staff       (20)     2005 2023-05-09 01:09:35.000000 BioSAK-1.86.2/BioSAK/rename_reads_for_Reago.py
--rw-r--r--   0 songweizhi   (501) staff       (20)     6801 2023-10-26 11:55:44.000000 BioSAK-1.86.2/BioSAK/rename_seq.py
--rw-r--r--   0 songweizhi   (501) staff       (20)     2210 2024-01-16 05:10:59.000000 BioSAK-1.86.2/BioSAK/rename_seqs.py
--rw-r--r--   0 songweizhi   (501) staff       (20)    13528 2024-04-28 15:16:01.000000 BioSAK-1.86.2/BioSAK/ribbon.py
--rw-r--r--   0 songweizhi   (501) staff       (20)     1996 2023-05-09 01:09:35.000000 BioSAK-1.86.2/BioSAK/sam2bam.py
--rw-r--r--   0 songweizhi   (501) staff       (20)     6877 2023-05-13 11:01:19.000000 BioSAK-1.86.2/BioSAK/sampling_GTDB_gnms.py
--rw-r--r--   0 songweizhi   (501) staff       (20)     3603 2024-01-16 05:10:59.000000 BioSAK-1.86.2/BioSAK/select_seq.py
--rw-r--r--   0 songweizhi   (501) staff       (20)     3167 2023-05-09 01:09:35.000000 BioSAK-1.86.2/BioSAK/sep_reads_by_barcode.py
--rw-r--r--   0 songweizhi   (501) staff       (20)     2671 2024-01-16 05:10:59.000000 BioSAK-1.86.2/BioSAK/slice_seq.py
--rw-r--r--   0 songweizhi   (501) staff       (20)     3788 2023-05-09 01:09:35.000000 BioSAK-1.86.2/BioSAK/split_fasta.py
--rw-r--r--   0 songweizhi   (501) staff       (20)     1998 2024-01-16 05:10:59.000000 BioSAK-1.86.2/BioSAK/split_folder.py
--rw-r--r--   0 songweizhi   (501) staff       (20)     4561 2023-05-09 01:09:35.000000 BioSAK-1.86.2/BioSAK/split_sam.py
--rwxr-xr-x   0 songweizhi   (501) staff       (20)     1204 2024-01-16 05:10:59.000000 BioSAK-1.86.2/BioSAK/submitHPC.py
--rw-r--r--   0 songweizhi   (501) staff       (20)     2011 2024-01-16 05:10:59.000000 BioSAK-1.86.2/BioSAK/subset_GTDB_meta.py
--rw-r--r--   0 songweizhi   (501) staff       (20)     4585 2024-04-09 03:15:33.000000 BioSAK-1.86.2/BioSAK/subset_df.py
--rw-r--r--   0 songweizhi   (501) staff       (20)     7296 2024-01-16 05:10:59.000000 BioSAK-1.86.2/BioSAK/subset_tree.py
--rw-r--r--   0 songweizhi   (501) staff       (20)      108 2024-04-28 15:09:23.000000 BioSAK-1.86.2/BioSAK/tmp_1.py
--rw-r--r--   0 songweizhi   (501) staff       (20)     7844 2024-01-16 05:10:59.000000 BioSAK-1.86.2/BioSAK/top_16S_hits.py
--rw-r--r--   0 songweizhi   (501) staff       (20)     2106 2023-05-09 01:09:35.000000 BioSAK-1.86.2/BioSAK/top_hits_in_a_group.py
--rw-r--r--   0 songweizhi   (501) staff       (20)      831 2024-04-09 06:05:51.000000 BioSAK-1.86.2/BioSAK/transpose.py
--rw-r--r--   0 songweizhi   (501) staff       (20)     2252 2024-01-16 05:10:59.000000 BioSAK-1.86.2/BioSAK/usearch_uc.py
--rw-r--r--   0 songweizhi   (501) staff       (20)      962 2024-04-17 08:12:49.000000 BioSAK-1.86.2/BioSAK/wilcox.py
-drwxr-xr-x   0 songweizhi   (501) staff       (20)        0 2024-04-28 15:18:15.240055 BioSAK-1.86.2/BioSAK.egg-info/
--rw-r--r--   0 songweizhi   (501) staff       (20)      508 2024-04-28 15:18:15.000000 BioSAK-1.86.2/BioSAK.egg-info/PKG-INFO
--rw-r--r--   0 songweizhi   (501) staff       (20)     3682 2024-04-28 15:18:15.000000 BioSAK-1.86.2/BioSAK.egg-info/SOURCES.txt
--rw-r--r--   0 songweizhi   (501) staff       (20)        1 2024-04-28 15:18:15.000000 BioSAK-1.86.2/BioSAK.egg-info/dependency_links.txt
--rw-r--r--   0 songweizhi   (501) staff       (20)       95 2024-04-28 15:18:15.000000 BioSAK-1.86.2/BioSAK.egg-info/requires.txt
--rw-r--r--   0 songweizhi   (501) staff       (20)        7 2024-04-28 15:18:15.000000 BioSAK-1.86.2/BioSAK.egg-info/top_level.txt
--rw-r--r--   0 songweizhi   (501) staff       (20)    35141 2023-05-09 01:09:36.000000 BioSAK-1.86.2/LICENSE
--rwxr-xr-x   0 songweizhi   (501) staff       (20)      300 2023-05-09 01:09:36.000000 BioSAK-1.86.2/MANIFEST.in
--rw-r--r--   0 songweizhi   (501) staff       (20)      508 2024-04-28 15:18:15.240333 BioSAK-1.86.2/PKG-INFO
--rw-r--r--   0 songweizhi   (501) staff       (20)     1533 2024-01-23 07:37:01.000000 BioSAK-1.86.2/README.md
-drwxr-xr-x   0 songweizhi   (501) staff       (20)        0 2024-04-28 15:18:15.239369 BioSAK-1.86.2/bin/
--rwxr-xr-x   0 songweizhi   (501) staff       (20)    77600 2024-04-28 14:57:06.000000 BioSAK-1.86.2/bin/BioSAK
--rw-r--r--   0 songweizhi   (501) staff       (20)       38 2024-04-28 15:18:15.240617 BioSAK-1.86.2/setup.cfg
--rw-r--r--   0 songweizhi   (501) staff       (20)      915 2024-01-15 11:41:11.000000 BioSAK-1.86.2/setup.py
+drwxr-xr-x   0 songweizhi   (501) staff       (20)        0 2024-04-29 00:08:39.627848 BioSAK-1.86.3/
+drwxr-xr-x   0 songweizhi   (501) staff       (20)        0 2024-04-29 00:08:39.624204 BioSAK-1.86.3/BioSAK/
+-rw-r--r--   0 songweizhi   (501) staff       (20)     3653 2024-01-16 05:10:59.000000 BioSAK-1.86.3/BioSAK/BLCA_op_parser.py
+-rw-r--r--   0 songweizhi   (501) staff       (20)     2031 2023-05-31 05:26:00.000000 BioSAK-1.86.3/BioSAK/BioSAK_config.py
+-rwxr-xr-x   0 songweizhi   (501) staff       (20)    39300 2024-03-22 00:45:31.000000 BioSAK-1.86.3/BioSAK/COG2020.py
+-rw-r--r--   0 songweizhi   (501) staff       (20)     3615 2023-05-09 01:09:35.000000 BioSAK-1.86.3/BioSAK/COG_boxplot_last1row.R
+-rw-r--r--   0 songweizhi   (501) staff       (20)     6974 2023-05-09 01:09:35.000000 BioSAK-1.86.3/BioSAK/COG_boxplot_last2row.R
+-rwxr-xr-x   0 songweizhi   (501) staff       (20)     6067 2024-01-16 05:00:13.000000 BioSAK-1.86.3/BioSAK/CheckM.py
+-rw-r--r--   0 songweizhi   (501) staff       (20)     5891 2024-01-16 05:10:59.000000 BioSAK-1.86.3/BioSAK/ConvertMSA.py
+-rw-r--r--   0 songweizhi   (501) staff       (20)    16671 2023-05-09 01:09:35.000000 BioSAK-1.86.3/BioSAK/DnaFeaturesViewer.py
+-rw-r--r--   0 songweizhi   (501) staff       (20)     2292 2023-05-09 01:09:35.000000 BioSAK-1.86.3/BioSAK/FastaSplitler_by_num.py
+-rw-r--r--   0 songweizhi   (501) staff       (20)     2485 2023-05-09 01:09:35.000000 BioSAK-1.86.3/BioSAK/FastaSplitler_by_size.py
+-rw-r--r--   0 songweizhi   (501) staff       (20)     2190 2023-05-09 01:09:35.000000 BioSAK-1.86.3/BioSAK/GTDB_for_BLCA.py
+-rw-r--r--   0 songweizhi   (501) staff       (20)     1321 2023-05-09 01:09:35.000000 BioSAK-1.86.3/BioSAK/Gene2Ctg.py
+-rw-r--r--   0 songweizhi   (501) staff       (20)    45147 2024-03-23 14:54:03.000000 BioSAK-1.86.3/BioSAK/KEGG.py
+-rw-r--r--   0 songweizhi   (501) staff       (20)     3484 2023-05-09 01:09:35.000000 BioSAK-1.86.3/BioSAK/KEGG_boxplot_last1row.R
+-rw-r--r--   0 songweizhi   (501) staff       (20)      269 2023-05-09 01:09:35.000000 BioSAK-1.86.3/BioSAK/KEGG_get_eukaryotic_kos.py
+-rw-r--r--   0 songweizhi   (501) staff       (20)     3077 2023-08-22 09:31:28.000000 BioSAK-1.86.3/BioSAK/KeepRemovingTmp.py
+-rw-r--r--   0 songweizhi   (501) staff       (20)     2620 2024-01-16 05:10:59.000000 BioSAK-1.86.3/BioSAK/MeanMappingDepth.py
+-rw-r--r--   0 songweizhi   (501) staff       (20)     3682 2024-01-16 12:39:58.000000 BioSAK-1.86.3/BioSAK/MetaBiosample.py
+-rw-r--r--   0 songweizhi   (501) staff       (20)  3297822 2023-05-09 01:09:35.000000 BioSAK-1.86.3/BioSAK/MetaCHIP_phylo.hmm
+-rw-r--r--   0 songweizhi   (501) staff       (20)  1206805 2023-05-09 01:09:35.000000 BioSAK-1.86.3/BioSAK/MetaCyc_reactions_with_ec.txt
+-rw-r--r--   0 songweizhi   (501) staff       (20)    16960 2023-05-09 01:09:35.000000 BioSAK-1.86.3/BioSAK/NetEnzymes.py
+-rw-r--r--   0 songweizhi   (501) staff       (20)     3713 2023-05-09 01:09:35.000000 BioSAK-1.86.3/BioSAK/Newick_tree_plotter.py
+-rw-r--r--   0 songweizhi   (501) staff       (20)     1659 2024-01-16 05:10:59.000000 BioSAK-1.86.3/BioSAK/OneLineAln.py
+-rw-r--r--   0 songweizhi   (501) staff       (20)    10448 2023-05-09 01:09:35.000000 BioSAK-1.86.3/BioSAK/Prodigal.py
+-rw-r--r--   0 songweizhi   (501) staff       (20)     6048 2023-05-09 01:09:35.000000 BioSAK-1.86.3/BioSAK/Reads_simulator.py
+-rw-r--r--   0 songweizhi   (501) staff       (20)     3573 2024-01-16 05:10:59.000000 BioSAK-1.86.3/BioSAK/RunGraphMB.py
+-rw-r--r--   0 songweizhi   (501) staff       (20)     3833 2024-01-16 05:10:59.000000 BioSAK-1.86.3/BioSAK/SILVA_for_BLCA.py
+-rwxr-xr-x   0 songweizhi   (501) staff       (20)     6255 2023-05-09 01:09:35.000000 BioSAK-1.86.3/BioSAK/SankeyTaxon.py
+-rw-r--r--   0 songweizhi   (501) staff       (20)     5678 2024-01-16 05:10:59.000000 BioSAK-1.86.3/BioSAK/SliceMSA.py
+-rw-r--r--   0 songweizhi   (501) staff       (20)     3173 2024-01-16 05:10:59.000000 BioSAK-1.86.3/BioSAK/SubsampleLongReads.py
+-rwxr-xr-x   0 songweizhi   (501) staff       (20)     1696 2024-01-16 05:10:59.000000 BioSAK-1.86.3/BioSAK/Tax4Fun2IndOTU.py
+-rw-r--r--   0 songweizhi   (501) staff       (20)     3619 2024-04-29 00:08:38.000000 BioSAK-1.86.3/BioSAK/VERSION
+-rw-r--r--   0 songweizhi   (501) staff       (20)      467 2023-05-09 01:09:35.000000 BioSAK-1.86.3/BioSAK/VisBlastOp.py
+-rw-r--r--   0 songweizhi   (501) staff       (20)     9944 2023-05-09 01:09:35.000000 BioSAK-1.86.3/BioSAK/VisGeneFlk.py
+-rwxr-xr-x   0 songweizhi   (501) staff       (20)        0 2023-05-09 01:09:35.000000 BioSAK-1.86.3/BioSAK/__init__.py
+-rw-r--r--   0 songweizhi   (501) staff       (20)     2526 2024-03-25 14:00:14.000000 BioSAK-1.86.3/BioSAK/add_desc.py
+-rwxr-xr-x   0 songweizhi   (501) staff       (20)    38577 2024-03-22 00:45:31.000000 BioSAK-1.86.3/BioSAK/arCOG.py
+-rw-r--r--   0 songweizhi   (501) staff       (20)     6985 2024-01-16 05:00:13.000000 BioSAK-1.86.3/BioSAK/bam2reads.py
+-rwxr-xr-x   0 songweizhi   (501) staff       (20)     2630 2024-03-22 13:23:45.000000 BioSAK-1.86.3/BioSAK/boxplot.py
+-rw-r--r--   0 songweizhi   (501) staff       (20)     3312 2023-05-09 01:09:35.000000 BioSAK-1.86.3/BioSAK/boxplot_last1row.R
+-rw-r--r--   0 songweizhi   (501) staff       (20)     6104 2023-05-09 01:09:35.000000 BioSAK-1.86.3/BioSAK/boxplot_matrix_COG.py
+-rw-r--r--   0 songweizhi   (501) staff       (20)     5403 2023-05-09 01:09:35.000000 BioSAK-1.86.3/BioSAK/boxplot_matrix_COG_backup.py
+-rw-r--r--   0 songweizhi   (501) staff       (20)     6984 2023-05-09 01:09:35.000000 BioSAK-1.86.3/BioSAK/boxplot_matrix_KEGG.py
+-rw-r--r--   0 songweizhi   (501) staff       (20)     5747 2023-05-09 01:09:35.000000 BioSAK-1.86.3/BioSAK/boxplot_matrix_dbCAN.py
+-rw-r--r--   0 songweizhi   (501) staff       (20)     1695 2023-05-09 01:09:35.000000 BioSAK-1.86.3/BioSAK/cat_fa.py
+-rw-r--r--   0 songweizhi   (501) staff       (20)    13440 2023-05-09 01:09:35.000000 BioSAK-1.86.3/BioSAK/cdd2cog.pl
+-rw-r--r--   0 songweizhi   (501) staff       (20)     1186 2023-05-09 01:09:35.000000 BioSAK-1.86.3/BioSAK/checkm_marker.py
+-rw-r--r--   0 songweizhi   (501) staff       (20)     1076 2023-05-09 01:09:35.000000 BioSAK-1.86.3/BioSAK/compare_trees.R
+-rw-r--r--   0 songweizhi   (501) staff       (20)     9745 2024-01-16 05:10:59.000000 BioSAK-1.86.3/BioSAK/compare_trees.py
+-rw-r--r--   0 songweizhi   (501) staff       (20)     6592 2023-05-09 01:09:35.000000 BioSAK-1.86.3/BioSAK/cross_link_seqs.py
+-rw-r--r--   0 songweizhi   (501) staff       (20)    24033 2024-03-22 00:45:31.000000 BioSAK-1.86.3/BioSAK/dbCAN.py
+-rw-r--r--   0 songweizhi   (501) staff       (20)     1936 2023-05-09 01:09:35.000000 BioSAK-1.86.3/BioSAK/download_GenBank_genome_subset_prokaryotes_csv.py
+-rw-r--r--   0 songweizhi   (501) staff       (20)      767 2023-05-09 01:09:35.000000 BioSAK-1.86.3/BioSAK/dwnld_sra_reads.py
+-rwxr-xr-x   0 songweizhi   (501) staff       (20)    13250 2024-03-22 08:01:22.000000 BioSAK-1.86.3/BioSAK/enrich.py
+-rw-r--r--   0 songweizhi   (501) staff       (20)      929 2023-05-09 01:09:35.000000 BioSAK-1.86.3/BioSAK/exe_cmds.py
+-rw-r--r--   0 songweizhi   (501) staff       (20)     1508 2023-12-05 01:06:39.000000 BioSAK-1.86.3/BioSAK/ezaai2mat.py
+-rw-r--r--   0 songweizhi   (501) staff       (20)     1396 2023-12-05 01:02:55.000000 BioSAK-1.86.3/BioSAK/fa2id.py
+-rw-r--r--   0 songweizhi   (501) staff       (20)     1195 2023-05-17 06:14:50.000000 BioSAK-1.86.3/BioSAK/fa2phy.py
+-rw-r--r--   0 songweizhi   (501) staff       (20)     1363 2023-05-09 01:09:35.000000 BioSAK-1.86.3/BioSAK/fa2tree.py
+-rw-r--r--   0 songweizhi   (501) staff       (20)     6280 2023-05-09 01:09:35.000000 BioSAK-1.86.3/BioSAK/format_converter.py
+-rwxr-xr-x   0 songweizhi   (501) staff       (20)     2861 2023-05-09 01:09:35.000000 BioSAK-1.86.3/BioSAK/format_leaf_name.py
+-rw-r--r--   0 songweizhi   (501) staff       (20)      639 2023-05-09 01:09:35.000000 BioSAK-1.86.3/BioSAK/fq2fa.py
+-rw-r--r--   0 songweizhi   (501) staff       (20)     3204 2024-04-19 15:04:59.000000 BioSAK-1.86.3/BioSAK/gapseq.py
+-rw-r--r--   0 songweizhi   (501) staff       (20)     2846 2023-06-14 10:08:30.000000 BioSAK-1.86.3/BioSAK/gbk2faa.py
+-rw-r--r--   0 songweizhi   (501) staff       (20)     3342 2023-06-14 10:14:13.000000 BioSAK-1.86.3/BioSAK/gbk2ffn.py
+-rw-r--r--   0 songweizhi   (501) staff       (20)     2528 2023-05-09 01:09:35.000000 BioSAK-1.86.3/BioSAK/gbk2fna.py
+-rw-r--r--   0 songweizhi   (501) staff       (20)     3726 2023-05-09 01:09:35.000000 BioSAK-1.86.3/BioSAK/gbk_to_ffn_faa.py
+-rw-r--r--   0 songweizhi   (501) staff       (20)     1887 2024-04-15 02:59:40.000000 BioSAK-1.86.3/BioSAK/gc.py
+-rw-r--r--   0 songweizhi   (501) staff       (20)      813 2023-05-09 01:09:35.000000 BioSAK-1.86.3/BioSAK/get_EC_from_ko_stats_D.py
+-rw-r--r--   0 songweizhi   (501) staff       (20)     7477 2023-05-09 01:09:35.000000 BioSAK-1.86.3/BioSAK/get_GTDB_taxon_gnm.py
+-rw-r--r--   0 songweizhi   (501) staff       (20)     5428 2023-06-15 03:03:02.000000 BioSAK-1.86.3/BioSAK/get_MAG_reads_long.py
+-rw-r--r--   0 songweizhi   (501) staff       (20)     3991 2023-05-09 01:09:35.000000 BioSAK-1.86.3/BioSAK/get_Pfam_hmms.py
+-rw-r--r--   0 songweizhi   (501) staff       (20)    29246 2023-05-09 01:09:35.000000 BioSAK-1.86.3/BioSAK/get_SCG_tree.py
+-rw-r--r--   0 songweizhi   (501) staff       (20)     1784 2023-05-09 01:09:35.000000 BioSAK-1.86.3/BioSAK/get_TopHits_taxonomy.py
+-rw-r--r--   0 songweizhi   (501) staff       (20)     2247 2023-05-09 01:09:35.000000 BioSAK-1.86.3/BioSAK/get_aa_composition.py
+-rw-r--r--   0 songweizhi   (501) staff       (20)    12066 2023-05-09 01:09:35.000000 BioSAK-1.86.3/BioSAK/get_bin_abundance copy.py
+-rw-r--r--   0 songweizhi   (501) staff       (20)     2139 2024-01-23 11:57:14.000000 BioSAK-1.86.3/BioSAK/get_data_matrix.py
+-rw-r--r--   0 songweizhi   (501) staff       (20)     5523 2023-05-09 01:09:35.000000 BioSAK-1.86.3/BioSAK/get_gene_depth.py
+-rw-r--r--   0 songweizhi   (501) staff       (20)     3591 2024-01-16 05:10:59.000000 BioSAK-1.86.3/BioSAK/get_genome_GTDB.py
+-rw-r--r--   0 songweizhi   (501) staff       (20)     6070 2024-01-16 04:57:23.000000 BioSAK-1.86.3/BioSAK/get_genome_NCBI.py
+-rw-r--r--   0 songweizhi   (501) staff       (20)    11209 2023-05-09 01:09:35.000000 BioSAK-1.86.3/BioSAK/get_genome_NCBI_v1.py
+-rw-r--r--   0 songweizhi   (501) staff       (20)    12620 2023-05-09 01:09:35.000000 BioSAK-1.86.3/BioSAK/get_genome_NCBI_v2.py
+-rw-r--r--   0 songweizhi   (501) staff       (20)     3048 2023-05-09 01:09:35.000000 BioSAK-1.86.3/BioSAK/get_gnm_size.py
+-rw-r--r--   0 songweizhi   (501) staff       (20)     4834 2023-05-09 01:09:35.000000 BioSAK-1.86.3/BioSAK/get_ko_gene_seqs.py
+-rw-r--r--   0 songweizhi   (501) staff       (20)     1192 2023-09-21 08:44:42.000000 BioSAK-1.86.3/BioSAK/get_krona_plot.py
+-rw-r--r--   0 songweizhi   (501) staff       (20)     1559 2023-05-09 01:09:35.000000 BioSAK-1.86.3/BioSAK/get_reads_from_sam.py
+-rw-r--r--   0 songweizhi   (501) staff       (20)      792 2023-05-09 01:09:35.000000 BioSAK-1.86.3/BioSAK/get_reads_id_in_sam.py
+-rw-r--r--   0 songweizhi   (501) staff       (20)     2386 2023-05-09 01:09:35.000000 BioSAK-1.86.3/BioSAK/get_sankey_plot.R
+-rw-r--r--   0 songweizhi   (501) staff       (20)     4242 2023-05-09 01:09:35.000000 BioSAK-1.86.3/BioSAK/get_top_hit.py
+-rw-r--r--   0 songweizhi   (501) staff       (20)      820 2023-05-09 01:09:35.000000 BioSAK-1.86.3/BioSAK/get_total_length.py
+-rw-r--r--   0 songweizhi   (501) staff       (20)     4643 2023-05-18 01:37:58.000000 BioSAK-1.86.3/BioSAK/global_functions.py
+-rwxr-xr-x   0 songweizhi   (501) staff       (20)     2910 2024-03-11 00:57:02.000000 BioSAK-1.86.3/BioSAK/hpc3.py
+-rw-r--r--   0 songweizhi   (501) staff       (20)    26872 2024-04-12 00:51:29.000000 BioSAK-1.86.3/BioSAK/iTOL.py
+-rw-r--r--   0 songweizhi   (501) staff       (20)     3337 2024-03-07 03:01:35.000000 BioSAK-1.86.3/BioSAK/js_cmds.py
+-rw-r--r--   0 songweizhi   (501) staff       (20)     3281 2024-04-08 09:48:49.000000 BioSAK-1.86.3/BioSAK/js_hpc3.py
+-rw-r--r--   0 songweizhi   (501) staff       (20)     1643 2023-05-09 01:09:35.000000 BioSAK-1.86.3/BioSAK/keep_best_hit.py
+-rw-r--r--   0 songweizhi   (501) staff       (20)  3361029 2023-05-09 01:09:35.000000 BioSAK-1.86.3/BioSAK/ko00001.keg
+-rw-r--r--   0 songweizhi   (501) staff       (20)     1848 2024-03-10 15:18:30.000000 BioSAK-1.86.3/BioSAK/koala.py
+-rw-r--r--   0 songweizhi   (501) staff       (20)     2772 2023-05-09 01:09:35.000000 BioSAK-1.86.3/BioSAK/label_tree.R
+-rw-r--r--   0 songweizhi   (501) staff       (20)     4788 2024-01-16 05:10:59.000000 BioSAK-1.86.3/BioSAK/label_tree.py
+-rw-r--r--   0 songweizhi   (501) staff       (20)    35857 2023-05-09 01:09:35.000000 BioSAK-1.86.3/BioSAK/link_16S_MAG.py
+-rw-r--r--   0 songweizhi   (501) staff       (20)    12349 2023-05-09 01:09:35.000000 BioSAK-1.86.3/BioSAK/magabund.py
+-rw-r--r--   0 songweizhi   (501) staff       (20)    19855 2023-05-09 01:09:35.000000 BioSAK-1.86.3/BioSAK/magabund2.py
+-rw-r--r--   0 songweizhi   (501) staff       (20)     1224 2023-05-09 01:09:35.000000 BioSAK-1.86.3/BioSAK/manipulator_fasta.py
+-rw-r--r--   0 songweizhi   (501) staff       (20)        0 2023-05-09 01:09:35.000000 BioSAK-1.86.3/BioSAK/manipulator_msa.py
+-rw-r--r--   0 songweizhi   (501) staff       (20)     3659 2023-05-09 01:09:35.000000 BioSAK-1.86.3/BioSAK/manipulator_newick.py
+-rw-r--r--   0 songweizhi   (501) staff       (20)        0 2023-05-09 01:09:35.000000 BioSAK-1.86.3/BioSAK/manipulator_sam.py
+-rw-r--r--   0 songweizhi   (501) staff       (20)      903 2024-04-17 08:12:49.000000 BioSAK-1.86.3/BioSAK/mannwhitneyu.py
+-rw-r--r--   0 songweizhi   (501) staff       (20)     2433 2023-05-30 01:59:44.000000 BioSAK-1.86.3/BioSAK/mean_MAG_cov.py
+-rw-r--r--   0 songweizhi   (501) staff       (20)     1880 2024-03-25 06:45:20.000000 BioSAK-1.86.3/BioSAK/merge_df.py
+-rw-r--r--   0 songweizhi   (501) staff       (20)     2405 2024-01-16 05:10:59.000000 BioSAK-1.86.3/BioSAK/merge_seq.py
+-rw-r--r--   0 songweizhi   (501) staff       (20)     6742 2024-01-23 07:37:01.000000 BioSAK-1.86.3/BioSAK/metaAssembly.py
+-rw-r--r--   0 songweizhi   (501) staff       (20)     1327 2023-06-11 13:56:21.000000 BioSAK-1.86.3/BioSAK/metabat2concoct.py
+-rw-r--r--   0 songweizhi   (501) staff       (20)     1612 2023-06-11 16:00:51.000000 BioSAK-1.86.3/BioSAK/metabat2maxbin.py
+-rw-r--r--   0 songweizhi   (501) staff       (20)        0 2023-05-09 01:09:35.000000 BioSAK-1.86.3/BioSAK/msa_to_distance_matrix.py
+-rw-r--r--   0 songweizhi   (501) staff       (20)     1759 2023-05-09 01:09:35.000000 BioSAK-1.86.3/BioSAK/ncbi_dataset.py
+-rw-r--r--   0 songweizhi   (501) staff       (20)        0 2024-03-03 11:00:02.000000 BioSAK-1.86.3/BioSAK/odp.py
+-rw-r--r--   0 songweizhi   (501) staff       (20)     2820 2023-05-09 01:09:35.000000 BioSAK-1.86.3/BioSAK/parse_MetaCyc_RxnDB.py
+-rw-r--r--   0 songweizhi   (501) staff       (20)     1460 2023-09-18 14:42:31.000000 BioSAK-1.86.3/BioSAK/parse_mmseqs_tsv.py
+-rw-r--r--   0 songweizhi   (501) staff       (20)     8633 2024-01-16 05:10:59.000000 BioSAK-1.86.3/BioSAK/plot_mag.py
+-rw-r--r--   0 songweizhi   (501) staff       (20)     7332 2023-05-09 01:09:35.000000 BioSAK-1.86.3/BioSAK/plot_sam_depth.py
+-rw-r--r--   0 songweizhi   (501) staff       (20)     1638 2023-05-09 01:09:35.000000 BioSAK-1.86.3/BioSAK/plot_tree.R
+-rw-r--r--   0 songweizhi   (501) staff       (20)     2256 2023-07-22 00:36:16.000000 BioSAK-1.86.3/BioSAK/prefix_file.py
+-rw-r--r--   0 songweizhi   (501) staff       (20)     4221 2024-01-16 05:10:59.000000 BioSAK-1.86.3/BioSAK/prokka.py
+-rw-r--r--   0 songweizhi   (501) staff       (20)     5057 2023-08-03 02:58:56.000000 BioSAK-1.86.3/BioSAK/reads2bam.py
+-rwxr-xr-x   0 songweizhi   (501) staff       (20)     2534 2023-05-09 01:09:35.000000 BioSAK-1.86.3/BioSAK/rename_leaves.py
+-rw-r--r--   0 songweizhi   (501) staff       (20)     2005 2023-05-09 01:09:35.000000 BioSAK-1.86.3/BioSAK/rename_reads_for_Reago.py
+-rw-r--r--   0 songweizhi   (501) staff       (20)     6801 2023-10-26 11:55:44.000000 BioSAK-1.86.3/BioSAK/rename_seq.py
+-rw-r--r--   0 songweizhi   (501) staff       (20)     2210 2024-01-16 05:10:59.000000 BioSAK-1.86.3/BioSAK/rename_seqs.py
+-rw-r--r--   0 songweizhi   (501) staff       (20)    14469 2024-04-29 00:07:53.000000 BioSAK-1.86.3/BioSAK/ribbon.py
+-rw-r--r--   0 songweizhi   (501) staff       (20)     1996 2023-05-09 01:09:35.000000 BioSAK-1.86.3/BioSAK/sam2bam.py
+-rw-r--r--   0 songweizhi   (501) staff       (20)     6877 2023-05-13 11:01:19.000000 BioSAK-1.86.3/BioSAK/sampling_GTDB_gnms.py
+-rw-r--r--   0 songweizhi   (501) staff       (20)     3603 2024-01-16 05:10:59.000000 BioSAK-1.86.3/BioSAK/select_seq.py
+-rw-r--r--   0 songweizhi   (501) staff       (20)     3167 2023-05-09 01:09:35.000000 BioSAK-1.86.3/BioSAK/sep_reads_by_barcode.py
+-rw-r--r--   0 songweizhi   (501) staff       (20)     2671 2024-01-16 05:10:59.000000 BioSAK-1.86.3/BioSAK/slice_seq.py
+-rw-r--r--   0 songweizhi   (501) staff       (20)     3788 2023-05-09 01:09:35.000000 BioSAK-1.86.3/BioSAK/split_fasta.py
+-rw-r--r--   0 songweizhi   (501) staff       (20)     1998 2024-01-16 05:10:59.000000 BioSAK-1.86.3/BioSAK/split_folder.py
+-rw-r--r--   0 songweizhi   (501) staff       (20)     4561 2023-05-09 01:09:35.000000 BioSAK-1.86.3/BioSAK/split_sam.py
+-rwxr-xr-x   0 songweizhi   (501) staff       (20)     1204 2024-01-16 05:10:59.000000 BioSAK-1.86.3/BioSAK/submitHPC.py
+-rw-r--r--   0 songweizhi   (501) staff       (20)     2011 2024-01-16 05:10:59.000000 BioSAK-1.86.3/BioSAK/subset_GTDB_meta.py
+-rw-r--r--   0 songweizhi   (501) staff       (20)     4585 2024-04-09 03:15:33.000000 BioSAK-1.86.3/BioSAK/subset_df.py
+-rw-r--r--   0 songweizhi   (501) staff       (20)     7296 2024-01-16 05:10:59.000000 BioSAK-1.86.3/BioSAK/subset_tree.py
+-rw-r--r--   0 songweizhi   (501) staff       (20)      108 2024-04-28 15:09:23.000000 BioSAK-1.86.3/BioSAK/tmp_1.py
+-rw-r--r--   0 songweizhi   (501) staff       (20)     7844 2024-01-16 05:10:59.000000 BioSAK-1.86.3/BioSAK/top_16S_hits.py
+-rw-r--r--   0 songweizhi   (501) staff       (20)     2106 2023-05-09 01:09:35.000000 BioSAK-1.86.3/BioSAK/top_hits_in_a_group.py
+-rw-r--r--   0 songweizhi   (501) staff       (20)      831 2024-04-09 06:05:51.000000 BioSAK-1.86.3/BioSAK/transpose.py
+-rw-r--r--   0 songweizhi   (501) staff       (20)     2252 2024-01-16 05:10:59.000000 BioSAK-1.86.3/BioSAK/usearch_uc.py
+-rw-r--r--   0 songweizhi   (501) staff       (20)      962 2024-04-17 08:12:49.000000 BioSAK-1.86.3/BioSAK/wilcox.py
+drwxr-xr-x   0 songweizhi   (501) staff       (20)        0 2024-04-29 00:08:39.625797 BioSAK-1.86.3/BioSAK.egg-info/
+-rw-r--r--   0 songweizhi   (501) staff       (20)      508 2024-04-29 00:08:39.000000 BioSAK-1.86.3/BioSAK.egg-info/PKG-INFO
+-rw-r--r--   0 songweizhi   (501) staff       (20)     3682 2024-04-29 00:08:39.000000 BioSAK-1.86.3/BioSAK.egg-info/SOURCES.txt
+-rw-r--r--   0 songweizhi   (501) staff       (20)        1 2024-04-29 00:08:39.000000 BioSAK-1.86.3/BioSAK.egg-info/dependency_links.txt
+-rw-r--r--   0 songweizhi   (501) staff       (20)       95 2024-04-29 00:08:39.000000 BioSAK-1.86.3/BioSAK.egg-info/requires.txt
+-rw-r--r--   0 songweizhi   (501) staff       (20)        7 2024-04-29 00:08:39.000000 BioSAK-1.86.3/BioSAK.egg-info/top_level.txt
+-rw-r--r--   0 songweizhi   (501) staff       (20)    35141 2023-05-09 01:09:36.000000 BioSAK-1.86.3/LICENSE
+-rwxr-xr-x   0 songweizhi   (501) staff       (20)      300 2023-05-09 01:09:36.000000 BioSAK-1.86.3/MANIFEST.in
+-rw-r--r--   0 songweizhi   (501) staff       (20)      508 2024-04-29 00:08:39.627581 BioSAK-1.86.3/PKG-INFO
+-rw-r--r--   0 songweizhi   (501) staff       (20)     1533 2024-01-23 07:37:01.000000 BioSAK-1.86.3/README.md
+drwxr-xr-x   0 songweizhi   (501) staff       (20)        0 2024-04-29 00:08:39.625059 BioSAK-1.86.3/bin/
+-rwxr-xr-x   0 songweizhi   (501) staff       (20)    77600 2024-04-28 14:57:06.000000 BioSAK-1.86.3/bin/BioSAK
+-rw-r--r--   0 songweizhi   (501) staff       (20)       38 2024-04-29 00:08:39.627899 BioSAK-1.86.3/setup.cfg
+-rw-r--r--   0 songweizhi   (501) staff       (20)      915 2024-01-15 11:41:11.000000 BioSAK-1.86.3/setup.py
```

### Comparing `BioSAK-1.86.2/BioSAK/BLCA_op_parser.py` & `BioSAK-1.86.3/BioSAK/BLCA_op_parser.py`

 * *Files identical despite different names*

### Comparing `BioSAK-1.86.2/BioSAK/BioSAK_config.py` & `BioSAK-1.86.3/BioSAK/BioSAK_config.py`

 * *Files identical despite different names*

### Comparing `BioSAK-1.86.2/BioSAK/COG2020.py` & `BioSAK-1.86.3/BioSAK/COG2020.py`

 * *Files identical despite different names*

### Comparing `BioSAK-1.86.2/BioSAK/COG_boxplot_last1row.R` & `BioSAK-1.86.3/BioSAK/COG_boxplot_last1row.R`

 * *Files identical despite different names*

### Comparing `BioSAK-1.86.2/BioSAK/COG_boxplot_last2row.R` & `BioSAK-1.86.3/BioSAK/COG_boxplot_last2row.R`

 * *Files identical despite different names*

### Comparing `BioSAK-1.86.2/BioSAK/CheckM.py` & `BioSAK-1.86.3/BioSAK/CheckM.py`

 * *Files identical despite different names*

### Comparing `BioSAK-1.86.2/BioSAK/ConvertMSA.py` & `BioSAK-1.86.3/BioSAK/ConvertMSA.py`

 * *Files identical despite different names*

### Comparing `BioSAK-1.86.2/BioSAK/DnaFeaturesViewer.py` & `BioSAK-1.86.3/BioSAK/DnaFeaturesViewer.py`

 * *Files identical despite different names*

### Comparing `BioSAK-1.86.2/BioSAK/FastaSplitler_by_num.py` & `BioSAK-1.86.3/BioSAK/FastaSplitler_by_num.py`

 * *Files identical despite different names*

### Comparing `BioSAK-1.86.2/BioSAK/FastaSplitler_by_size.py` & `BioSAK-1.86.3/BioSAK/FastaSplitler_by_size.py`

 * *Files identical despite different names*

### Comparing `BioSAK-1.86.2/BioSAK/GTDB_for_BLCA.py` & `BioSAK-1.86.3/BioSAK/GTDB_for_BLCA.py`

 * *Files identical despite different names*

### Comparing `BioSAK-1.86.2/BioSAK/Gene2Ctg.py` & `BioSAK-1.86.3/BioSAK/Gene2Ctg.py`

 * *Files identical despite different names*

### Comparing `BioSAK-1.86.2/BioSAK/KEGG.py` & `BioSAK-1.86.3/BioSAK/KEGG.py`

 * *Files identical despite different names*

### Comparing `BioSAK-1.86.2/BioSAK/KEGG_boxplot_last1row.R` & `BioSAK-1.86.3/BioSAK/KEGG_boxplot_last1row.R`

 * *Files identical despite different names*

### Comparing `BioSAK-1.86.2/BioSAK/KeepRemovingTmp.py` & `BioSAK-1.86.3/BioSAK/KeepRemovingTmp.py`

 * *Files identical despite different names*

### Comparing `BioSAK-1.86.2/BioSAK/MeanMappingDepth.py` & `BioSAK-1.86.3/BioSAK/MeanMappingDepth.py`

 * *Files identical despite different names*

### Comparing `BioSAK-1.86.2/BioSAK/MetaBiosample.py` & `BioSAK-1.86.3/BioSAK/MetaBiosample.py`

 * *Files identical despite different names*

### Comparing `BioSAK-1.86.2/BioSAK/MetaCHIP_phylo.hmm` & `BioSAK-1.86.3/BioSAK/MetaCHIP_phylo.hmm`

 * *Files identical despite different names*

### Comparing `BioSAK-1.86.2/BioSAK/MetaCyc_reactions_with_ec.txt` & `BioSAK-1.86.3/BioSAK/MetaCyc_reactions_with_ec.txt`

 * *Files identical despite different names*

### Comparing `BioSAK-1.86.2/BioSAK/NetEnzymes.py` & `BioSAK-1.86.3/BioSAK/NetEnzymes.py`

 * *Files identical despite different names*

### Comparing `BioSAK-1.86.2/BioSAK/Newick_tree_plotter.py` & `BioSAK-1.86.3/BioSAK/Newick_tree_plotter.py`

 * *Files identical despite different names*

### Comparing `BioSAK-1.86.2/BioSAK/OneLineAln.py` & `BioSAK-1.86.3/BioSAK/OneLineAln.py`

 * *Files identical despite different names*

### Comparing `BioSAK-1.86.2/BioSAK/Prodigal.py` & `BioSAK-1.86.3/BioSAK/Prodigal.py`

 * *Files identical despite different names*

### Comparing `BioSAK-1.86.2/BioSAK/Reads_simulator.py` & `BioSAK-1.86.3/BioSAK/Reads_simulator.py`

 * *Files identical despite different names*

### Comparing `BioSAK-1.86.2/BioSAK/RunGraphMB.py` & `BioSAK-1.86.3/BioSAK/RunGraphMB.py`

 * *Files identical despite different names*

### Comparing `BioSAK-1.86.2/BioSAK/SILVA_for_BLCA.py` & `BioSAK-1.86.3/BioSAK/SILVA_for_BLCA.py`

 * *Files identical despite different names*

### Comparing `BioSAK-1.86.2/BioSAK/SankeyTaxon.py` & `BioSAK-1.86.3/BioSAK/SankeyTaxon.py`

 * *Files identical despite different names*

### Comparing `BioSAK-1.86.2/BioSAK/SliceMSA.py` & `BioSAK-1.86.3/BioSAK/SliceMSA.py`

 * *Files identical despite different names*

### Comparing `BioSAK-1.86.2/BioSAK/SubsampleLongReads.py` & `BioSAK-1.86.3/BioSAK/SubsampleLongReads.py`

 * *Files identical despite different names*

### Comparing `BioSAK-1.86.2/BioSAK/Tax4Fun2IndOTU.py` & `BioSAK-1.86.3/BioSAK/Tax4Fun2IndOTU.py`

 * *Files identical despite different names*

### Comparing `BioSAK-1.86.2/BioSAK/VERSION` & `BioSAK-1.86.3/BioSAK/VERSION`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-1.86.2
+1.86.3
 - fixed bugs
 
 1.86.0
 - new modules added: ribbon
 
 1.85.0
 - new modules added: wilcox and mannwhitneyu
```

### Comparing `BioSAK-1.86.2/BioSAK/VisGeneFlk.py` & `BioSAK-1.86.3/BioSAK/VisGeneFlk.py`

 * *Files identical despite different names*

### Comparing `BioSAK-1.86.2/BioSAK/add_desc.py` & `BioSAK-1.86.3/BioSAK/add_desc.py`

 * *Files identical despite different names*

### Comparing `BioSAK-1.86.2/BioSAK/arCOG.py` & `BioSAK-1.86.3/BioSAK/arCOG.py`

 * *Files identical despite different names*

### Comparing `BioSAK-1.86.2/BioSAK/bam2reads.py` & `BioSAK-1.86.3/BioSAK/bam2reads.py`

 * *Files identical despite different names*

### Comparing `BioSAK-1.86.2/BioSAK/boxplot.py` & `BioSAK-1.86.3/BioSAK/boxplot.py`

 * *Files identical despite different names*

### Comparing `BioSAK-1.86.2/BioSAK/boxplot_last1row.R` & `BioSAK-1.86.3/BioSAK/boxplot_last1row.R`

 * *Files identical despite different names*

### Comparing `BioSAK-1.86.2/BioSAK/boxplot_matrix_COG.py` & `BioSAK-1.86.3/BioSAK/boxplot_matrix_COG.py`

 * *Files identical despite different names*

### Comparing `BioSAK-1.86.2/BioSAK/boxplot_matrix_COG_backup.py` & `BioSAK-1.86.3/BioSAK/boxplot_matrix_COG_backup.py`

 * *Files identical despite different names*

### Comparing `BioSAK-1.86.2/BioSAK/boxplot_matrix_KEGG.py` & `BioSAK-1.86.3/BioSAK/boxplot_matrix_KEGG.py`

 * *Files identical despite different names*

### Comparing `BioSAK-1.86.2/BioSAK/boxplot_matrix_dbCAN.py` & `BioSAK-1.86.3/BioSAK/boxplot_matrix_dbCAN.py`

 * *Files identical despite different names*

### Comparing `BioSAK-1.86.2/BioSAK/cat_fa.py` & `BioSAK-1.86.3/BioSAK/cat_fa.py`

 * *Files identical despite different names*

### Comparing `BioSAK-1.86.2/BioSAK/cdd2cog.pl` & `BioSAK-1.86.3/BioSAK/cdd2cog.pl`

 * *Files identical despite different names*

### Comparing `BioSAK-1.86.2/BioSAK/checkm_marker.py` & `BioSAK-1.86.3/BioSAK/checkm_marker.py`

 * *Files identical despite different names*

### Comparing `BioSAK-1.86.2/BioSAK/compare_trees.R` & `BioSAK-1.86.3/BioSAK/compare_trees.R`

 * *Files identical despite different names*

### Comparing `BioSAK-1.86.2/BioSAK/compare_trees.py` & `BioSAK-1.86.3/BioSAK/compare_trees.py`

 * *Files identical despite different names*

### Comparing `BioSAK-1.86.2/BioSAK/cross_link_seqs.py` & `BioSAK-1.86.3/BioSAK/cross_link_seqs.py`

 * *Files identical despite different names*

### Comparing `BioSAK-1.86.2/BioSAK/dbCAN.py` & `BioSAK-1.86.3/BioSAK/dbCAN.py`

 * *Files identical despite different names*

### Comparing `BioSAK-1.86.2/BioSAK/download_GenBank_genome_subset_prokaryotes_csv.py` & `BioSAK-1.86.3/BioSAK/download_GenBank_genome_subset_prokaryotes_csv.py`

 * *Files identical despite different names*

### Comparing `BioSAK-1.86.2/BioSAK/dwnld_sra_reads.py` & `BioSAK-1.86.3/BioSAK/dwnld_sra_reads.py`

 * *Files identical despite different names*

### Comparing `BioSAK-1.86.2/BioSAK/enrich.py` & `BioSAK-1.86.3/BioSAK/enrich.py`

 * *Files identical despite different names*

### Comparing `BioSAK-1.86.2/BioSAK/exe_cmds.py` & `BioSAK-1.86.3/BioSAK/exe_cmds.py`

 * *Files identical despite different names*

### Comparing `BioSAK-1.86.2/BioSAK/ezaai2mat.py` & `BioSAK-1.86.3/BioSAK/ezaai2mat.py`

 * *Files identical despite different names*

### Comparing `BioSAK-1.86.2/BioSAK/fa2id.py` & `BioSAK-1.86.3/BioSAK/fa2id.py`

 * *Files identical despite different names*

### Comparing `BioSAK-1.86.2/BioSAK/fa2phy.py` & `BioSAK-1.86.3/BioSAK/fa2phy.py`

 * *Files identical despite different names*

### Comparing `BioSAK-1.86.2/BioSAK/fa2tree.py` & `BioSAK-1.86.3/BioSAK/fa2tree.py`

 * *Files identical despite different names*

### Comparing `BioSAK-1.86.2/BioSAK/format_converter.py` & `BioSAK-1.86.3/BioSAK/format_converter.py`

 * *Files identical despite different names*

### Comparing `BioSAK-1.86.2/BioSAK/format_leaf_name.py` & `BioSAK-1.86.3/BioSAK/format_leaf_name.py`

 * *Files identical despite different names*

### Comparing `BioSAK-1.86.2/BioSAK/fq2fa.py` & `BioSAK-1.86.3/BioSAK/fq2fa.py`

 * *Files identical despite different names*

### Comparing `BioSAK-1.86.2/BioSAK/gapseq.py` & `BioSAK-1.86.3/BioSAK/gapseq.py`

 * *Files identical despite different names*

### Comparing `BioSAK-1.86.2/BioSAK/gbk2faa.py` & `BioSAK-1.86.3/BioSAK/gbk2faa.py`

 * *Files identical despite different names*

### Comparing `BioSAK-1.86.2/BioSAK/gbk2ffn.py` & `BioSAK-1.86.3/BioSAK/gbk2ffn.py`

 * *Files identical despite different names*

### Comparing `BioSAK-1.86.2/BioSAK/gbk2fna.py` & `BioSAK-1.86.3/BioSAK/gbk2fna.py`

 * *Files identical despite different names*

### Comparing `BioSAK-1.86.2/BioSAK/gbk_to_ffn_faa.py` & `BioSAK-1.86.3/BioSAK/gbk_to_ffn_faa.py`

 * *Files identical despite different names*

### Comparing `BioSAK-1.86.2/BioSAK/gc.py` & `BioSAK-1.86.3/BioSAK/gc.py`

 * *Files identical despite different names*

### Comparing `BioSAK-1.86.2/BioSAK/get_EC_from_ko_stats_D.py` & `BioSAK-1.86.3/BioSAK/get_EC_from_ko_stats_D.py`

 * *Files identical despite different names*

### Comparing `BioSAK-1.86.2/BioSAK/get_GTDB_taxon_gnm.py` & `BioSAK-1.86.3/BioSAK/get_GTDB_taxon_gnm.py`

 * *Files identical despite different names*

### Comparing `BioSAK-1.86.2/BioSAK/get_MAG_reads_long.py` & `BioSAK-1.86.3/BioSAK/get_MAG_reads_long.py`

 * *Files identical despite different names*

### Comparing `BioSAK-1.86.2/BioSAK/get_Pfam_hmms.py` & `BioSAK-1.86.3/BioSAK/get_Pfam_hmms.py`

 * *Files identical despite different names*

### Comparing `BioSAK-1.86.2/BioSAK/get_SCG_tree.py` & `BioSAK-1.86.3/BioSAK/get_SCG_tree.py`

 * *Files identical despite different names*

### Comparing `BioSAK-1.86.2/BioSAK/get_TopHits_taxonomy.py` & `BioSAK-1.86.3/BioSAK/get_TopHits_taxonomy.py`

 * *Files identical despite different names*

### Comparing `BioSAK-1.86.2/BioSAK/get_aa_composition.py` & `BioSAK-1.86.3/BioSAK/get_aa_composition.py`

 * *Files identical despite different names*

### Comparing `BioSAK-1.86.2/BioSAK/get_bin_abundance copy.py` & `BioSAK-1.86.3/BioSAK/get_bin_abundance copy.py`

 * *Files identical despite different names*

### Comparing `BioSAK-1.86.2/BioSAK/get_data_matrix.py` & `BioSAK-1.86.3/BioSAK/get_data_matrix.py`

 * *Files identical despite different names*

### Comparing `BioSAK-1.86.2/BioSAK/get_gene_depth.py` & `BioSAK-1.86.3/BioSAK/get_gene_depth.py`

 * *Files identical despite different names*

### Comparing `BioSAK-1.86.2/BioSAK/get_genome_GTDB.py` & `BioSAK-1.86.3/BioSAK/get_genome_GTDB.py`

 * *Files identical despite different names*

### Comparing `BioSAK-1.86.2/BioSAK/get_genome_NCBI.py` & `BioSAK-1.86.3/BioSAK/get_genome_NCBI.py`

 * *Files identical despite different names*

### Comparing `BioSAK-1.86.2/BioSAK/get_genome_NCBI_v1.py` & `BioSAK-1.86.3/BioSAK/get_genome_NCBI_v1.py`

 * *Files identical despite different names*

### Comparing `BioSAK-1.86.2/BioSAK/get_genome_NCBI_v2.py` & `BioSAK-1.86.3/BioSAK/get_genome_NCBI_v2.py`

 * *Files identical despite different names*

### Comparing `BioSAK-1.86.2/BioSAK/get_gnm_size.py` & `BioSAK-1.86.3/BioSAK/get_gnm_size.py`

 * *Files identical despite different names*

### Comparing `BioSAK-1.86.2/BioSAK/get_ko_gene_seqs.py` & `BioSAK-1.86.3/BioSAK/get_ko_gene_seqs.py`

 * *Files identical despite different names*

### Comparing `BioSAK-1.86.2/BioSAK/get_krona_plot.py` & `BioSAK-1.86.3/BioSAK/get_krona_plot.py`

 * *Files identical despite different names*

### Comparing `BioSAK-1.86.2/BioSAK/get_reads_from_sam.py` & `BioSAK-1.86.3/BioSAK/get_reads_from_sam.py`

 * *Files identical despite different names*

### Comparing `BioSAK-1.86.2/BioSAK/get_reads_id_in_sam.py` & `BioSAK-1.86.3/BioSAK/get_reads_id_in_sam.py`

 * *Files identical despite different names*

### Comparing `BioSAK-1.86.2/BioSAK/get_sankey_plot.R` & `BioSAK-1.86.3/BioSAK/get_sankey_plot.R`

 * *Files identical despite different names*

### Comparing `BioSAK-1.86.2/BioSAK/get_top_hit.py` & `BioSAK-1.86.3/BioSAK/get_top_hit.py`

 * *Files identical despite different names*

### Comparing `BioSAK-1.86.2/BioSAK/get_total_length.py` & `BioSAK-1.86.3/BioSAK/get_total_length.py`

 * *Files identical despite different names*

### Comparing `BioSAK-1.86.2/BioSAK/global_functions.py` & `BioSAK-1.86.3/BioSAK/global_functions.py`

 * *Files identical despite different names*

### Comparing `BioSAK-1.86.2/BioSAK/hpc3.py` & `BioSAK-1.86.3/BioSAK/hpc3.py`

 * *Files identical despite different names*

### Comparing `BioSAK-1.86.2/BioSAK/iTOL.py` & `BioSAK-1.86.3/BioSAK/iTOL.py`

 * *Files identical despite different names*

### Comparing `BioSAK-1.86.2/BioSAK/js_cmds.py` & `BioSAK-1.86.3/BioSAK/js_cmds.py`

 * *Files identical despite different names*

### Comparing `BioSAK-1.86.2/BioSAK/js_hpc3.py` & `BioSAK-1.86.3/BioSAK/js_hpc3.py`

 * *Files identical despite different names*

### Comparing `BioSAK-1.86.2/BioSAK/keep_best_hit.py` & `BioSAK-1.86.3/BioSAK/keep_best_hit.py`

 * *Files identical despite different names*

### Comparing `BioSAK-1.86.2/BioSAK/ko00001.keg` & `BioSAK-1.86.3/BioSAK/ko00001.keg`

 * *Files identical despite different names*

### Comparing `BioSAK-1.86.2/BioSAK/koala.py` & `BioSAK-1.86.3/BioSAK/koala.py`

 * *Files identical despite different names*

### Comparing `BioSAK-1.86.2/BioSAK/label_tree.R` & `BioSAK-1.86.3/BioSAK/label_tree.R`

 * *Files identical despite different names*

### Comparing `BioSAK-1.86.2/BioSAK/label_tree.py` & `BioSAK-1.86.3/BioSAK/label_tree.py`

 * *Files identical despite different names*

### Comparing `BioSAK-1.86.2/BioSAK/link_16S_MAG.py` & `BioSAK-1.86.3/BioSAK/link_16S_MAG.py`

 * *Files identical despite different names*

### Comparing `BioSAK-1.86.2/BioSAK/magabund.py` & `BioSAK-1.86.3/BioSAK/magabund.py`

 * *Files identical despite different names*

### Comparing `BioSAK-1.86.2/BioSAK/magabund2.py` & `BioSAK-1.86.3/BioSAK/magabund2.py`

 * *Files identical despite different names*

### Comparing `BioSAK-1.86.2/BioSAK/manipulator_fasta.py` & `BioSAK-1.86.3/BioSAK/manipulator_fasta.py`

 * *Files identical despite different names*

### Comparing `BioSAK-1.86.2/BioSAK/manipulator_newick.py` & `BioSAK-1.86.3/BioSAK/manipulator_newick.py`

 * *Files identical despite different names*

### Comparing `BioSAK-1.86.2/BioSAK/mannwhitneyu.py` & `BioSAK-1.86.3/BioSAK/mannwhitneyu.py`

 * *Files identical despite different names*

### Comparing `BioSAK-1.86.2/BioSAK/mean_MAG_cov.py` & `BioSAK-1.86.3/BioSAK/mean_MAG_cov.py`

 * *Files identical despite different names*

### Comparing `BioSAK-1.86.2/BioSAK/merge_df.py` & `BioSAK-1.86.3/BioSAK/merge_df.py`

 * *Files identical despite different names*

### Comparing `BioSAK-1.86.2/BioSAK/merge_seq.py` & `BioSAK-1.86.3/BioSAK/merge_seq.py`

 * *Files identical despite different names*

### Comparing `BioSAK-1.86.2/BioSAK/metaAssembly.py` & `BioSAK-1.86.3/BioSAK/metaAssembly.py`

 * *Files identical despite different names*

### Comparing `BioSAK-1.86.2/BioSAK/metabat2concoct.py` & `BioSAK-1.86.3/BioSAK/metabat2concoct.py`

 * *Files identical despite different names*

### Comparing `BioSAK-1.86.2/BioSAK/metabat2maxbin.py` & `BioSAK-1.86.3/BioSAK/metabat2maxbin.py`

 * *Files identical despite different names*

### Comparing `BioSAK-1.86.2/BioSAK/ncbi_dataset.py` & `BioSAK-1.86.3/BioSAK/ncbi_dataset.py`

 * *Files identical despite different names*

### Comparing `BioSAK-1.86.2/BioSAK/parse_MetaCyc_RxnDB.py` & `BioSAK-1.86.3/BioSAK/parse_MetaCyc_RxnDB.py`

 * *Files identical despite different names*

### Comparing `BioSAK-1.86.2/BioSAK/parse_mmseqs_tsv.py` & `BioSAK-1.86.3/BioSAK/parse_mmseqs_tsv.py`

 * *Files identical despite different names*

### Comparing `BioSAK-1.86.2/BioSAK/plot_mag.py` & `BioSAK-1.86.3/BioSAK/plot_mag.py`

 * *Files identical despite different names*

### Comparing `BioSAK-1.86.2/BioSAK/plot_sam_depth.py` & `BioSAK-1.86.3/BioSAK/plot_sam_depth.py`

 * *Files identical despite different names*

### Comparing `BioSAK-1.86.2/BioSAK/plot_tree.R` & `BioSAK-1.86.3/BioSAK/plot_tree.R`

 * *Files identical despite different names*

### Comparing `BioSAK-1.86.2/BioSAK/prefix_file.py` & `BioSAK-1.86.3/BioSAK/prefix_file.py`

 * *Files identical despite different names*

### Comparing `BioSAK-1.86.2/BioSAK/prokka.py` & `BioSAK-1.86.3/BioSAK/prokka.py`

 * *Files identical despite different names*

### Comparing `BioSAK-1.86.2/BioSAK/reads2bam.py` & `BioSAK-1.86.3/BioSAK/reads2bam.py`

 * *Files identical despite different names*

### Comparing `BioSAK-1.86.2/BioSAK/rename_leaves.py` & `BioSAK-1.86.3/BioSAK/rename_leaves.py`

 * *Files identical despite different names*

### Comparing `BioSAK-1.86.2/BioSAK/rename_reads_for_Reago.py` & `BioSAK-1.86.3/BioSAK/rename_reads_for_Reago.py`

 * *Files identical despite different names*

### Comparing `BioSAK-1.86.2/BioSAK/rename_seq.py` & `BioSAK-1.86.3/BioSAK/rename_seq.py`

 * *Files identical despite different names*

### Comparing `BioSAK-1.86.2/BioSAK/rename_seqs.py` & `BioSAK-1.86.3/BioSAK/rename_seqs.py`

 * *Files identical despite different names*

### Comparing `BioSAK-1.86.2/BioSAK/ribbon.py` & `BioSAK-1.86.3/BioSAK/ribbon.py`

 * *Files 4% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 ==================== ribbon example commands ====================
 
 # Dependencies: opd
 
 # example commands
 odp="/scratch/PI/ocessongwz/Software/odp/scripts/odp"
 odp_rbh_to_ribbon="/scratch/PI/ocessongwz/Software/odp/scripts/odp_rbh_to_ribbon"
-BioSAK ribbon -co chrom_order.txt -o ribbon_op_dir -fa example_files -pep example_files -chrom example_files -f -odp $odp -odp_rbh_to_ribbon $odp_rbh_to_ribbon
+BioSAK ribbon -plot_lgs -co chrom_order.txt -o ribbon_op_dir -fa example_files -pep example_files -chrom example_files -f -odp $odp -odp_rbh_to_ribbon $odp_rbh_to_ribbon
 
 Note:
 1. Species names can't have '_' char
 
 =================================================================
 '''
 
@@ -54,14 +54,16 @@
     odp_exe                 = args['odp']
     odp_rbh_to_ribbon_exe   = args['odp_rbh_to_ribbon']
     plot_all                = args['plot_all']
     plot_lgs                = args['plot_lgs']
 
     ################################################# define file name #################################################
 
+    wd_path = os.path.abspath(os.getcwd())
+
     get_macrosynteny_plot_wd    = '%s/get_macrosynteny_plot'    % op_dir
     get_ribbon_diagram_wd       = '%s/get_ribbon_diagram'       % op_dir
     config_yaml_macrosynteny    = '%s/config.yaml'              % get_macrosynteny_plot_wd
     config_yaml_ribbon          = '%s/config.yaml'              % get_ribbon_diagram_wd
     cmd_txt                     = '%s/commands.txt'             % op_dir
 
     ####################################################################################################################
@@ -109,22 +111,14 @@
                 chrom_order_dict[s_id] = []
             chrom_order_dict[s_id].append(c_id)
 
     fa_in_abspath                       = os.path.abspath(fa_in)
     op_dir_abspath                      = os.path.abspath(op_dir)
     get_macrosynteny_plot_wd_abspath    = os.path.abspath(get_macrosynteny_plot_wd)
     get_ribbon_diagram_wd_abspath       = os.path.abspath(get_ribbon_diagram_wd)
-    rbh_file_dir                        = '%s/odp/step2-figures/synteny_nocolor'        % get_macrosynteny_plot_wd_abspath
-    step2_figures_abspath               = '%s/odp/step2-figures'                        % get_macrosynteny_plot_wd_abspath
-
-    rbh_file_dir_plot_lgs = ''
-    step2_figures_sub_dir_list = next(os.walk(step2_figures_abspath))[1]
-    for each_sub_dir in step2_figures_sub_dir_list:
-        if each_sub_dir.startwith('synteny_coloredby'):
-            rbh_file_dir_plot_lgs = '%s/%s' % (step2_figures_abspath, each_sub_dir)
 
     ################################### get config.yaml for getting macrosynteny plot ##################################
 
     # get config.yaml for getting macrosynteny plot
     config_yaml_macrosynteny_handle = open(config_yaml_macrosynteny, 'w')
     config_yaml_macrosynteny_handle.write('ignore_autobreaks: True\n')
     config_yaml_macrosynteny_handle.write('diamond_or_blastp: "diamond"\n')
@@ -148,94 +142,120 @@
         config_yaml_macrosynteny_handle.write('  %s:\n' % each_species)
         config_yaml_macrosynteny_handle.write('    proteins:    %s\n' % current_pep)
         config_yaml_macrosynteny_handle.write('    chrom:       %s\n' % current_chrom)
         config_yaml_macrosynteny_handle.write('    genome:      %s\n' % current_fa)
         config_yaml_macrosynteny_handle.write('    minscafsize: %s\n' % minscafsize)
     config_yaml_macrosynteny_handle.close()
 
-    #################################### get config.yaml for getting ribbon diagram ####################################
-
-    config_yaml_ribbon_handle = open(config_yaml_ribbon, 'w')
-    config_yaml_ribbon_handle.write('chr_sort_order: optimal-chr-or\n')
-    if plot_all is True:
-        config_yaml_ribbon_handle.write('plot_all: True\n')
-    else:
-        config_yaml_ribbon_handle.write('plot_all: False\n')
-    config_yaml_ribbon_handle.write('\n')
-
-    # write out species_order section
-    config_yaml_ribbon_handle.write('species_order:\n')
-    for species in species_order_list:
-        config_yaml_ribbon_handle.write('  - %s\n' % species)
-    config_yaml_ribbon_handle.write('\n')
-
-    # write out chromorder section
-    config_yaml_ribbon_handle.write('chromorder:\n')
-    if chrom_order_txt is not None:
-        for each_s in chrom_order_dict:
-            config_yaml_ribbon_handle.write('  %s:\n' % each_s)
-            for each_chrom in chrom_order_dict[each_s]:
-                config_yaml_ribbon_handle.write('    - %s\n' % each_chrom)
-        config_yaml_ribbon_handle.write('\n')
-    else:
-        for each_species in species_order_list:
-            current_chrom_list = species_to_chrom_dict.get(each_species, [])
-            if len(current_chrom_list) > 0:
-                config_yaml_ribbon_handle.write('  %s:\n' % each_species)
-                for each_chrom in current_chrom_list:
-                    config_yaml_ribbon_handle.write('    - %s\n' % each_chrom)
-            config_yaml_ribbon_handle.write('\n')
-
-    # write out rbh_directory section
-    if plot_lgs is False:
-        config_yaml_ribbon_handle.write('rbh_directory: %s\n' % rbh_file_dir)
-    else:
-        config_yaml_ribbon_handle.write('rbh_directory: %s\n' % rbh_file_dir_plot_lgs)
-    config_yaml_ribbon_handle.write('\n')
-
-    # write out species section
-    config_yaml_ribbon_handle.write('species:\n')
-    for each_species in species_order_list:
-        current_fa    = '%s/%s.fa'    % (fa_in_abspath, each_species)
-        current_pep   = '%s/%s.pep'   % (fa_in_abspath, each_species)
-        current_chrom = '%s/%s.chrom' % (fa_in_abspath, each_species)
-        config_yaml_ribbon_handle.write('  %s:\n' % each_species)
-        config_yaml_ribbon_handle.write('    proteins:    %s\n' % current_pep)
-        config_yaml_ribbon_handle.write('    chrom:       %s\n' % current_chrom)
-        config_yaml_ribbon_handle.write('    genome:      %s\n' % current_fa)
-        config_yaml_ribbon_handle.write('    minscafsize: %s\n' % minscafsize)
-    config_yaml_ribbon_handle.close()
-
-    ################################################## run snakemake ###################################################
+    ############################################### get macrosynteny plot ##############################################
 
     snakemake_cmd_macrosynteny  = 'snakemake --cores %s --snakefile %s' % (thread_num, odp_exe)
-    snakemake_cmd_ribbon        = 'snakemake --cores %s --snakefile %s' % (thread_num, odp_rbh_to_ribbon_exe)
 
     # write out commands
     cmd_txt_handle = open(cmd_txt, 'w')
     cmd_txt_handle.write('cd %s\n' % get_macrosynteny_plot_wd_abspath)
     cmd_txt_handle.write(snakemake_cmd_macrosynteny + '\n')
     cmd_txt_handle.write('\n')
-    cmd_txt_handle.write('cd %s\n' % get_ribbon_diagram_wd_abspath)
-    cmd_txt_handle.write(snakemake_cmd_ribbon + '\n')
     cmd_txt_handle.close()
 
     # get macrosynteny plot
     print(snakemake_cmd_macrosynteny)
     os.chdir(get_macrosynteny_plot_wd_abspath)
     os.system(snakemake_cmd_macrosynteny)
 
+    #################################### get config.yaml for getting ribbon diagram ####################################
+
+    os.chdir(wd_path)
+    step2_figures_abspath = '%s/odp/step2-figures'                  % get_macrosynteny_plot_wd_abspath
+    snakemake_cmd_ribbon  = 'snakemake --cores %s --snakefile %s'   % (thread_num, odp_rbh_to_ribbon_exe)
+
+    step2_figures_sub_dir_list = next(os.walk(step2_figures_abspath))[1]
+    synteny_plot_list = ['synteny_nocolor']
+    for each_sub_dir in step2_figures_sub_dir_list:
+        if each_sub_dir.startswith('synteny_coloredby'):
+            synteny_plot_list.append(each_sub_dir)
+
+    for color_setting in synteny_plot_list:
+        current_synteny_dir         = '%s/%s'           % (step2_figures_abspath, color_setting)
+        current_wd                  = '%s/%s'           % (get_ribbon_diagram_wd_abspath, color_setting)
+        current_config_yaml_ribbon  = '%s/config.yaml'  % current_wd
+        os.mkdir(current_wd)
+
+        with open(cmd_txt, 'a') as cmd_txt_handle:
+            cmd_txt_handle.write('cd %s\n' % current_wd)
+            cmd_txt_handle.write(snakemake_cmd_ribbon + '\n')
+            cmd_txt_handle.write('\n')
+
+        config_yaml_ribbon_handle = open(current_config_yaml_ribbon, 'w')
+        config_yaml_ribbon_handle.write('chr_sort_order: optimal-chr-or\n')
+        if plot_all is True:
+            config_yaml_ribbon_handle.write('plot_all: True\n')
+        else:
+            config_yaml_ribbon_handle.write('plot_all: False\n')
+        config_yaml_ribbon_handle.write('\n')
+
+        # write out species_order section
+        config_yaml_ribbon_handle.write('species_order:\n')
+        for species in species_order_list:
+            config_yaml_ribbon_handle.write('  - %s\n' % species)
+        config_yaml_ribbon_handle.write('\n')
+
+        # write out chromorder section
+        config_yaml_ribbon_handle.write('chromorder:\n')
+        if chrom_order_txt is not None:
+            for each_s in chrom_order_dict:
+                config_yaml_ribbon_handle.write('  %s:\n' % each_s)
+                for each_chrom in chrom_order_dict[each_s]:
+                    config_yaml_ribbon_handle.write('    - %s\n' % each_chrom)
+            config_yaml_ribbon_handle.write('\n')
+        else:
+            for each_species in species_order_list:
+                current_chrom_list = species_to_chrom_dict.get(each_species, [])
+                if len(current_chrom_list) > 0:
+                    config_yaml_ribbon_handle.write('  %s:\n' % each_species)
+                    for each_chrom in current_chrom_list:
+                        config_yaml_ribbon_handle.write('    - %s\n' % each_chrom)
+                config_yaml_ribbon_handle.write('\n')
+
+        # write out rbh_directory section
+        config_yaml_ribbon_handle.write('rbh_directory: %s\n' % current_synteny_dir)
+        config_yaml_ribbon_handle.write('\n')
+
+        # write out species section
+        config_yaml_ribbon_handle.write('species:\n')
+        for each_species in species_order_list:
+            current_fa    = '%s/%s.fa'    % (fa_in_abspath, each_species)
+            current_pep   = '%s/%s.pep'   % (fa_in_abspath, each_species)
+            current_chrom = '%s/%s.chrom' % (fa_in_abspath, each_species)
+            config_yaml_ribbon_handle.write('  %s:\n' % each_species)
+            config_yaml_ribbon_handle.write('    proteins:    %s\n' % current_pep)
+            config_yaml_ribbon_handle.write('    chrom:       %s\n' % current_chrom)
+            config_yaml_ribbon_handle.write('    genome:      %s\n' % current_fa)
+            config_yaml_ribbon_handle.write('    minscafsize: %s\n' % minscafsize)
+        config_yaml_ribbon_handle.close()
+
+    ################################################## run snakemake ###################################################
+
     # get ribbon diagram
-    print(snakemake_cmd_ribbon)
-    os.chdir(get_ribbon_diagram_wd_abspath)
-    os.system(snakemake_cmd_ribbon)
+    for color_setting in synteny_plot_list:
+
+        current_wd              = '%s/%s'           % (get_ribbon_diagram_wd_abspath, color_setting)
+        pwd_plot_file           = '%s/output.pdf'   % current_wd
+        pwd_plot_file_relocated = '%s/%s.pdf'       % (get_ribbon_diagram_wd_abspath, color_setting)
+
+        print(snakemake_cmd_ribbon)
+        os.chdir(current_wd)
+        os.system(snakemake_cmd_ribbon)
+
+        if os.path.isfile(pwd_plot_file) is True:
+            os.system('mv %s %s' % (pwd_plot_file, pwd_plot_file_relocated))
 
     ################################################### final report ###################################################
 
-    print('Ribbon diagram exported to %s/output.pdf' % get_ribbon_diagram_wd)
+    print('Ribbon diagram exported to %s' % get_ribbon_diagram_wd)
     print('Done!')
 
     ####################################################################################################################
 
 
 if __name__ == '__main__':
 
@@ -263,9 +283,9 @@
     args = vars(ribbon_parser.parse_args())
     ribbon(args)
 
 
 '''
 
 python3 /Users/songweizhi/PycharmProjects/BioSAK/BioSAK/ribbon.py -o demo -fa example_files -f -odp /scratch/PI/ocessongwz/Software/odp/scripts/odp -odp_rbh_to_ribbon /scratch/PI/ocessongwz/Software/odp/scripts/odp_rbh_to_ribbon
-plot_LGs
+
 '''
```

### Comparing `BioSAK-1.86.2/BioSAK/sam2bam.py` & `BioSAK-1.86.3/BioSAK/sam2bam.py`

 * *Files identical despite different names*

### Comparing `BioSAK-1.86.2/BioSAK/sampling_GTDB_gnms.py` & `BioSAK-1.86.3/BioSAK/sampling_GTDB_gnms.py`

 * *Files identical despite different names*

### Comparing `BioSAK-1.86.2/BioSAK/select_seq.py` & `BioSAK-1.86.3/BioSAK/select_seq.py`

 * *Files identical despite different names*

### Comparing `BioSAK-1.86.2/BioSAK/sep_reads_by_barcode.py` & `BioSAK-1.86.3/BioSAK/sep_reads_by_barcode.py`

 * *Files identical despite different names*

### Comparing `BioSAK-1.86.2/BioSAK/slice_seq.py` & `BioSAK-1.86.3/BioSAK/slice_seq.py`

 * *Files identical despite different names*

### Comparing `BioSAK-1.86.2/BioSAK/split_fasta.py` & `BioSAK-1.86.3/BioSAK/split_fasta.py`

 * *Files identical despite different names*

### Comparing `BioSAK-1.86.2/BioSAK/split_folder.py` & `BioSAK-1.86.3/BioSAK/split_folder.py`

 * *Files identical despite different names*

### Comparing `BioSAK-1.86.2/BioSAK/split_sam.py` & `BioSAK-1.86.3/BioSAK/split_sam.py`

 * *Files identical despite different names*

### Comparing `BioSAK-1.86.2/BioSAK/submitHPC.py` & `BioSAK-1.86.3/BioSAK/submitHPC.py`

 * *Files identical despite different names*

### Comparing `BioSAK-1.86.2/BioSAK/subset_GTDB_meta.py` & `BioSAK-1.86.3/BioSAK/subset_GTDB_meta.py`

 * *Files identical despite different names*

### Comparing `BioSAK-1.86.2/BioSAK/subset_df.py` & `BioSAK-1.86.3/BioSAK/subset_df.py`

 * *Files identical despite different names*

### Comparing `BioSAK-1.86.2/BioSAK/subset_tree.py` & `BioSAK-1.86.3/BioSAK/subset_tree.py`

 * *Files identical despite different names*

### Comparing `BioSAK-1.86.2/BioSAK/top_16S_hits.py` & `BioSAK-1.86.3/BioSAK/top_16S_hits.py`

 * *Files identical despite different names*

### Comparing `BioSAK-1.86.2/BioSAK/top_hits_in_a_group.py` & `BioSAK-1.86.3/BioSAK/top_hits_in_a_group.py`

 * *Files identical despite different names*

### Comparing `BioSAK-1.86.2/BioSAK/transpose.py` & `BioSAK-1.86.3/BioSAK/transpose.py`

 * *Files identical despite different names*

### Comparing `BioSAK-1.86.2/BioSAK/usearch_uc.py` & `BioSAK-1.86.3/BioSAK/usearch_uc.py`

 * *Files identical despite different names*

### Comparing `BioSAK-1.86.2/BioSAK/wilcox.py` & `BioSAK-1.86.3/BioSAK/wilcox.py`

 * *Files identical despite different names*

### Comparing `BioSAK-1.86.2/BioSAK.egg-info/SOURCES.txt` & `BioSAK-1.86.3/BioSAK.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `BioSAK-1.86.2/LICENSE` & `BioSAK-1.86.3/LICENSE`

 * *Files identical despite different names*

### Comparing `BioSAK-1.86.2/README.md` & `BioSAK-1.86.3/README.md`

 * *Files identical despite different names*

### Comparing `BioSAK-1.86.2/bin/BioSAK` & `BioSAK-1.86.3/bin/BioSAK`

 * *Files identical despite different names*

### Comparing `BioSAK-1.86.2/setup.py` & `BioSAK-1.86.3/setup.py`

 * *Files identical despite different names*

