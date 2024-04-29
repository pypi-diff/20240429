# Comparing `tmp/nci_cidc_schemas-0.26.29.tar.gz` & `tmp/nci_cidc_schemas-0.26.32.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nci_cidc_schemas-0.26.29.tar", last modified: Thu Mar  7 15:35:19 2024, max compression
+gzip compressed data, was "nci_cidc_schemas-0.26.32.tar", last modified: Mon Apr 29 19:04:33 2024, max compression
```

## Comparing `nci_cidc_schemas-0.26.29.tar` & `nci_cidc_schemas-0.26.32.tar`

### file list

```diff
@@ -1,260 +1,264 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-07 15:35:19.182578 nci_cidc_schemas-0.26.29/
--rw-r--r--   0 runner    (1001) docker     (127)     1072 2024-03-07 15:35:12.000000 nci_cidc_schemas-0.26.29/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      315 2024-03-07 15:35:12.000000 nci_cidc_schemas-0.26.29/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     4422 2024-03-07 15:35:19.182578 nci_cidc_schemas-0.26.29/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3365 2024-03-07 15:35:12.000000 nci_cidc_schemas-0.26.29/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-07 15:35:19.142577 nci_cidc_schemas-0.26.29/cidc_schemas/
--rw-r--r--   0 runner    (1001) docker     (127)      136 2024-03-07 15:35:12.000000 nci_cidc_schemas-0.26.29/cidc_schemas/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4099 2024-03-07 15:35:12.000000 nci_cidc_schemas-0.26.29/cidc_schemas/cli.py
--rw-r--r--   0 runner    (1001) docker     (127)      698 2024-03-07 15:35:12.000000 nci_cidc_schemas-0.26.29/cidc_schemas/constants.py
--rw-r--r--   0 runner    (1001) docker     (127)    20025 2024-03-07 15:35:12.000000 nci_cidc_schemas-0.26.29/cidc_schemas/json_validation.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-07 15:35:19.142577 nci_cidc_schemas-0.26.29/cidc_schemas/metaschema/
--rw-r--r--   0 runner    (1001) docker     (127)     6428 2024-03-07 15:35:12.000000 nci_cidc_schemas-0.26.29/cidc_schemas/metaschema/strict_meta_schema.json
--rw-r--r--   0 runner    (1001) docker     (127)    14766 2024-03-07 15:35:12.000000 nci_cidc_schemas-0.26.29/cidc_schemas/migrations.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-07 15:35:19.142577 nci_cidc_schemas-0.26.29/cidc_schemas/pipeline_configs/
--rw-r--r--   0 runner    (1001) docker     (127)     2832 2024-03-07 15:35:12.000000 nci_cidc_schemas-0.26.29/cidc_schemas/pipeline_configs/rna_level1_analysis_config.yaml.j2
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-07 15:35:19.142577 nci_cidc_schemas-0.26.29/cidc_schemas/prism/
--rw-r--r--   0 runner    (1001) docker     (127)      530 2024-03-07 15:35:12.000000 nci_cidc_schemas-0.26.29/cidc_schemas/prism/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2325 2024-03-07 15:35:12.000000 nci_cidc_schemas-0.26.29/cidc_schemas/prism/constants.py
--rw-r--r--   0 runner    (1001) docker     (127)    19293 2024-03-07 15:35:12.000000 nci_cidc_schemas-0.26.29/cidc_schemas/prism/core.py
--rw-r--r--   0 runner    (1001) docker     (127)     8558 2024-03-07 15:35:12.000000 nci_cidc_schemas-0.26.29/cidc_schemas/prism/extra_metadata.py
--rw-r--r--   0 runner    (1001) docker     (127)    12431 2024-03-07 15:35:12.000000 nci_cidc_schemas-0.26.29/cidc_schemas/prism/merger.py
--rw-r--r--   0 runner    (1001) docker     (127)    33530 2024-03-07 15:35:12.000000 nci_cidc_schemas-0.26.29/cidc_schemas/prism/pipelines.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-07 15:35:19.142577 nci_cidc_schemas-0.26.29/cidc_schemas/schemas/
--rw-r--r--   0 runner    (1001) docker     (127)     1943 2024-03-07 15:35:12.000000 nci_cidc_schemas-0.26.29/cidc_schemas/schemas/aliquot.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-07 15:35:19.150577 nci_cidc_schemas-0.26.29/cidc_schemas/schemas/artifacts/
--rw-r--r--   0 runner    (1001) docker     (127)     1653 2024-03-07 15:35:12.000000 nci_cidc_schemas-0.26.29/cidc_schemas/schemas/artifacts/artifact_bam.json
--rw-r--r--   0 runner    (1001) docker     (127)     1671 2024-03-07 15:35:12.000000 nci_cidc_schemas-0.26.29/cidc_schemas/schemas/artifacts/artifact_bam_bai.json
--rw-r--r--   0 runner    (1001) docker     (127)     1653 2024-03-07 15:35:12.000000 nci_cidc_schemas-0.26.29/cidc_schemas/schemas/artifacts/artifact_bed.json
--rw-r--r--   0 runner    (1001) docker     (127)     1665 2024-03-07 15:35:12.000000 nci_cidc_schemas-0.26.29/cidc_schemas/schemas/artifacts/artifact_bigwig.json
--rw-r--r--   0 runner    (1001) docker     (127)     1665 2024-03-07 15:35:12.000000 nci_cidc_schemas-0.26.29/cidc_schemas/schemas/artifacts/artifact_binary.json
--rw-r--r--   0 runner    (1001) docker     (127)     2114 2024-03-07 15:35:12.000000 nci_cidc_schemas-0.26.29/cidc_schemas/schemas/artifacts/artifact_clinical_csv.json
--rw-r--r--   0 runner    (1001) docker     (127)     2232 2024-03-07 15:35:12.000000 nci_cidc_schemas-0.26.29/cidc_schemas/schemas/artifacts/artifact_clinical_docx.json
--rw-r--r--   0 runner    (1001) docker     (127)     2232 2024-03-07 15:35:12.000000 nci_cidc_schemas-0.26.29/cidc_schemas/schemas/artifacts/artifact_clinical_xlsx.json
--rw-r--r--   0 runner    (1001) docker     (127)     1657 2024-03-07 15:35:12.000000 nci_cidc_schemas-0.26.29/cidc_schemas/schemas/artifacts/artifact_cncf.json
--rw-r--r--   0 runner    (1001) docker     (127)     1653 2024-03-07 15:35:12.000000 nci_cidc_schemas-0.26.29/cidc_schemas/schemas/artifacts/artifact_cns.json
--rw-r--r--   0 runner    (1001) docker     (127)     3123 2024-03-07 15:35:12.000000 nci_cidc_schemas-0.26.29/cidc_schemas/schemas/artifacts/artifact_core.json
--rw-r--r--   0 runner    (1001) docker     (127)     1665 2024-03-07 15:35:12.000000 nci_cidc_schemas-0.26.29/cidc_schemas/schemas/artifacts/artifact_csv.json
--rw-r--r--   0 runner    (1001) docker     (127)     2216 2024-03-07 15:35:12.000000 nci_cidc_schemas-0.26.29/cidc_schemas/schemas/artifacts/artifact_elisa_xlsx.json
--rw-r--r--   0 runner    (1001) docker     (127)     1683 2024-03-07 15:35:12.000000 nci_cidc_schemas-0.26.29/cidc_schemas/schemas/artifacts/artifact_fastq_gz.json
--rw-r--r--   0 runner    (1001) docker     (127)     1653 2024-03-07 15:35:12.000000 nci_cidc_schemas-0.26.29/cidc_schemas/schemas/artifacts/artifact_fcs.json
--rw-r--r--   0 runner    (1001) docker     (127)     1668 2024-03-07 15:35:12.000000 nci_cidc_schemas-0.26.29/cidc_schemas/schemas/artifacts/artifact_file.json
--rw-r--r--   0 runner    (1001) docker     (127)     1649 2024-03-07 15:35:12.000000 nci_cidc_schemas-0.26.29/cidc_schemas/schemas/artifacts/artifact_gz.json
--rw-r--r--   0 runner    (1001) docker     (127)     2015 2024-03-07 15:35:12.000000 nci_cidc_schemas-0.26.29/cidc_schemas/schemas/artifacts/artifact_image.json
--rw-r--r--   0 runner    (1001) docker     (127)     1653 2024-03-07 15:35:12.000000 nci_cidc_schemas-0.26.29/cidc_schemas/schemas/artifacts/artifact_jpg.json
--rw-r--r--   0 runner    (1001) docker     (127)     1657 2024-03-07 15:35:12.000000 nci_cidc_schemas-0.26.29/cidc_schemas/schemas/artifacts/artifact_json.json
--rw-r--r--   0 runner    (1001) docker     (127)     1775 2024-03-07 15:35:12.000000 nci_cidc_schemas-0.26.29/cidc_schemas/schemas/artifacts/artifact_junction.json
--rw-r--r--   0 runner    (1001) docker     (127)     1755 2024-03-07 15:35:12.000000 nci_cidc_schemas-0.26.29/cidc_schemas/schemas/artifacts/artifact_log.json
--rw-r--r--   0 runner    (1001) docker     (127)     1653 2024-03-07 15:35:12.000000 nci_cidc_schemas-0.26.29/cidc_schemas/schemas/artifacts/artifact_maf.json
--rw-r--r--   0 runner    (1001) docker     (127)     1681 2024-03-07 15:35:12.000000 nci_cidc_schemas-0.26.29/cidc_schemas/schemas/artifacts/artifact_narrowPeak.json
--rw-r--r--   0 runner    (1001) docker     (127)     2134 2024-03-07 15:35:12.000000 nci_cidc_schemas-0.26.29/cidc_schemas/schemas/artifacts/artifact_npx.json
--rw-r--r--   0 runner    (1001) docker     (127)     1674 2024-03-07 15:35:12.000000 nci_cidc_schemas-0.26.29/cidc_schemas/schemas/artifacts/artifact_pdf.json
--rw-r--r--   0 runner    (1001) docker     (127)     1653 2024-03-07 15:35:12.000000 nci_cidc_schemas-0.26.29/cidc_schemas/schemas/artifacts/artifact_png.json
--rw-r--r--   0 runner    (1001) docker     (127)     1704 2024-03-07 15:35:12.000000 nci_cidc_schemas-0.26.29/cidc_schemas/schemas/artifacts/artifact_rcc.json
--rw-r--r--   0 runner    (1001) docker     (127)     1661 2024-03-07 15:35:12.000000 nci_cidc_schemas-0.26.29/cidc_schemas/schemas/artifacts/artifact_tbi.json
--rw-r--r--   0 runner    (1001) docker     (127)     1657 2024-03-07 15:35:12.000000 nci_cidc_schemas-0.26.29/cidc_schemas/schemas/artifacts/artifact_text.json
--rw-r--r--   0 runner    (1001) docker     (127)     1663 2024-03-07 15:35:12.000000 nci_cidc_schemas-0.26.29/cidc_schemas/schemas/artifacts/artifact_tsv.json
--rw-r--r--   0 runner    (1001) docker     (127)     1653 2024-03-07 15:35:12.000000 nci_cidc_schemas-0.26.29/cidc_schemas/schemas/artifacts/artifact_vcf.json
--rw-r--r--   0 runner    (1001) docker     (127)     1675 2024-03-07 15:35:12.000000 nci_cidc_schemas-0.26.29/cidc_schemas/schemas/artifacts/artifact_vcf_gz.json
--rw-r--r--   0 runner    (1001) docker     (127)     1659 2024-03-07 15:35:12.000000 nci_cidc_schemas-0.26.29/cidc_schemas/schemas/artifacts/artifact_xlsx.json
--rw-r--r--   0 runner    (1001) docker     (127)     1657 2024-03-07 15:35:12.000000 nci_cidc_schemas-0.26.29/cidc_schemas/schemas/artifacts/artifact_yaml.json
--rw-r--r--   0 runner    (1001) docker     (127)     1653 2024-03-07 15:35:12.000000 nci_cidc_schemas-0.26.29/cidc_schemas/schemas/artifacts/artifact_zip.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-07 15:35:19.154577 nci_cidc_schemas-0.26.29/cidc_schemas/schemas/assays/
--rw-r--r--   0 runner    (1001) docker     (127)     2547 2024-03-07 15:35:12.000000 nci_cidc_schemas-0.26.29/cidc_schemas/schemas/assays/atacseq_assay.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-07 15:35:19.158577 nci_cidc_schemas-0.26.29/cidc_schemas/schemas/assays/components/
--rw-r--r--   0 runner    (1001) docker     (127)      960 2024-03-07 15:35:12.000000 nci_cidc_schemas-0.26.29/cidc_schemas/schemas/assays/components/antibody.json
--rw-r--r--   0 runner    (1001) docker     (127)      485 2024-03-07 15:35:12.000000 nci_cidc_schemas-0.26.29/cidc_schemas/schemas/assays/components/assay_core.json
--rw-r--r--   0 runner    (1001) docker     (127)     3540 2024-03-07 15:35:12.000000 nci_cidc_schemas-0.26.29/cidc_schemas/schemas/assays/components/available_assays.json
--rw-r--r--   0 runner    (1001) docker     (127)     1163 2024-03-07 15:35:12.000000 nci_cidc_schemas-0.26.29/cidc_schemas/schemas/assays/components/available_ngs_analyses.json
--rw-r--r--   0 runner    (1001) docker     (127)      733 2024-03-07 15:35:12.000000 nci_cidc_schemas-0.26.29/cidc_schemas/schemas/assays/components/composite_image.json
--rw-r--r--   0 runner    (1001) docker     (127)      458 2024-03-07 15:35:12.000000 nci_cidc_schemas-0.26.29/cidc_schemas/schemas/assays/components/controls.json
--rw-r--r--   0 runner    (1001) docker     (127)      813 2024-03-07 15:35:12.000000 nci_cidc_schemas-0.26.29/cidc_schemas/schemas/assays/components/enrichment_core.json
--rw-r--r--   0 runner    (1001) docker     (127)      663 2024-03-07 15:35:12.000000 nci_cidc_schemas-0.26.29/cidc_schemas/schemas/assays/components/excluded_samples.json
--rw-r--r--   0 runner    (1001) docker     (127)     1260 2024-03-07 15:35:12.000000 nci_cidc_schemas-0.26.29/cidc_schemas/schemas/assays/components/image.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-07 15:35:19.158577 nci_cidc_schemas-0.26.29/cidc_schemas/schemas/assays/components/imaging/
--rw-r--r--   0 runner    (1001) docker     (127)      546 2024-03-07 15:35:12.000000 nci_cidc_schemas-0.26.29/cidc_schemas/schemas/assays/components/imaging/mif_entry.json
--rw-r--r--   0 runner    (1001) docker     (127)     1728 2024-03-07 15:35:12.000000 nci_cidc_schemas-0.26.29/cidc_schemas/schemas/assays/components/imaging/mif_export.json
--rw-r--r--   0 runner    (1001) docker     (127)     1000 2024-03-07 15:35:12.000000 nci_cidc_schemas-0.26.29/cidc_schemas/schemas/assays/components/imaging/mif_input.json
--rw-r--r--   0 runner    (1001) docker     (127)     1112 2024-03-07 15:35:12.000000 nci_cidc_schemas-0.26.29/cidc_schemas/schemas/assays/components/imaging/mif_roi.json
--rw-r--r--   0 runner    (1001) docker     (127)      926 2024-03-07 15:35:12.000000 nci_cidc_schemas-0.26.29/cidc_schemas/schemas/assays/components/imaging_data.json
--rw-r--r--   0 runner    (1001) docker     (127)      405 2024-03-07 15:35:12.000000 nci_cidc_schemas-0.26.29/cidc_schemas/schemas/assays/components/local_file.json
--rw-r--r--   0 runner    (1001) docker     (127)     1663 2024-03-07 15:35:12.000000 nci_cidc_schemas-0.26.29/cidc_schemas/schemas/assays/components/mapping.json
--rw-r--r--   0 runner    (1001) docker     (127)     1831 2024-03-07 15:35:12.000000 nci_cidc_schemas-0.26.29/cidc_schemas/schemas/assays/components/mibi_antibody.json
--rw-r--r--   0 runner    (1001) docker     (127)     2191 2024-03-07 15:35:12.000000 nci_cidc_schemas-0.26.29/cidc_schemas/schemas/assays/components/mif_antibody.json
--rw-r--r--   0 runner    (1001) docker     (127)      480 2024-03-07 15:35:12.000000 nci_cidc_schemas-0.26.29/cidc_schemas/schemas/assays/components/multiple_local_files.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-07 15:35:19.158577 nci_cidc_schemas-0.26.29/cidc_schemas/schemas/assays/components/ngs/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-07 15:35:19.158577 nci_cidc_schemas-0.26.29/cidc_schemas/schemas/assays/components/ngs/atacseq/
--rw-r--r--   0 runner    (1001) docker     (127)     2283 2024-03-07 15:35:12.000000 nci_cidc_schemas-0.26.29/cidc_schemas/schemas/assays/components/ngs/atacseq/atacseq_analysis.json
--rw-r--r--   0 runner    (1001) docker     (127)      615 2024-03-07 15:35:12.000000 nci_cidc_schemas-0.26.29/cidc_schemas/schemas/assays/components/ngs/ngs_assay_record.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-07 15:35:19.162577 nci_cidc_schemas-0.26.29/cidc_schemas/schemas/assays/components/ngs/rna/
--rw-r--r--   0 runner    (1001) docker     (127)      392 2024-03-07 15:35:12.000000 nci_cidc_schemas-0.26.29/cidc_schemas/schemas/assays/components/ngs/rna/fusion.json
--rw-r--r--   0 runner    (1001) docker     (127)      395 2024-03-07 15:35:12.000000 nci_cidc_schemas-0.26.29/cidc_schemas/schemas/assays/components/ngs/rna/microbiome.json
--rw-r--r--   0 runner    (1001) docker     (127)      398 2024-03-07 15:35:12.000000 nci_cidc_schemas-0.26.29/cidc_schemas/schemas/assays/components/ngs/rna/msisensor.json
--rw-r--r--   0 runner    (1001) docker     (127)      385 2024-03-07 15:35:12.000000 nci_cidc_schemas-0.26.29/cidc_schemas/schemas/assays/components/ngs/rna/neoantigen.json
--rw-r--r--   0 runner    (1001) docker     (127)      605 2024-03-07 15:35:12.000000 nci_cidc_schemas-0.26.29/cidc_schemas/schemas/assays/components/ngs/rna/rna_analysis.json
--rw-r--r--   0 runner    (1001) docker     (127)     1432 2024-03-07 15:35:12.000000 nci_cidc_schemas-0.26.29/cidc_schemas/schemas/assays/components/ngs/rna/rna_level1_analysis.json
--rw-r--r--   0 runner    (1001) docker     (127)      541 2024-03-07 15:35:12.000000 nci_cidc_schemas-0.26.29/cidc_schemas/schemas/assays/components/ngs/rna/rseqc.json
--rw-r--r--   0 runner    (1001) docker     (127)     1375 2024-03-07 15:35:12.000000 nci_cidc_schemas-0.26.29/cidc_schemas/schemas/assays/components/ngs/rna/salmon.json
--rw-r--r--   0 runner    (1001) docker     (127)      772 2024-03-07 15:35:12.000000 nci_cidc_schemas-0.26.29/cidc_schemas/schemas/assays/components/ngs/rna/star.json
--rw-r--r--   0 runner    (1001) docker     (127)      382 2024-03-07 15:35:12.000000 nci_cidc_schemas-0.26.29/cidc_schemas/schemas/assays/components/ngs/rna/trust4.json
--rw-r--r--   0 runner    (1001) docker     (127)     1229 2024-03-07 15:35:12.000000 nci_cidc_schemas-0.26.29/cidc_schemas/schemas/assays/components/ngs_assay_core.json
--rw-r--r--   0 runner    (1001) docker     (127)      615 2024-03-07 15:35:12.000000 nci_cidc_schemas-0.26.29/cidc_schemas/schemas/assays/components/ngs_assay_record.json
--rw-r--r--   0 runner    (1001) docker     (127)     1139 2024-03-07 15:35:12.000000 nci_cidc_schemas-0.26.29/cidc_schemas/schemas/assays/components/reads_core.json
--rw-r--r--   0 runner    (1001) docker     (127)     1091 2024-03-07 15:35:12.000000 nci_cidc_schemas-0.26.29/cidc_schemas/schemas/assays/components/reads_with_index.json
--rw-r--r--   0 runner    (1001) docker     (127)     3274 2024-03-07 15:35:12.000000 nci_cidc_schemas-0.26.29/cidc_schemas/schemas/assays/ctdna_assay.json
--rw-r--r--   0 runner    (1001) docker     (127)     3659 2024-03-07 15:35:12.000000 nci_cidc_schemas-0.26.29/cidc_schemas/schemas/assays/cytof_assay.json
--rw-r--r--   0 runner    (1001) docker     (127)     8828 2024-03-07 15:35:12.000000 nci_cidc_schemas-0.26.29/cidc_schemas/schemas/assays/cytof_assay_core.json
--rw-r--r--   0 runner    (1001) docker     (127)     2233 2024-03-07 15:35:12.000000 nci_cidc_schemas-0.26.29/cidc_schemas/schemas/assays/elisa_assay.json
--rw-r--r--   0 runner    (1001) docker     (127)     3192 2024-03-07 15:35:12.000000 nci_cidc_schemas-0.26.29/cidc_schemas/schemas/assays/hande_assay.json
--rw-r--r--   0 runner    (1001) docker     (127)     6697 2024-03-07 15:35:12.000000 nci_cidc_schemas-0.26.29/cidc_schemas/schemas/assays/ihc_assay.json
--rw-r--r--   0 runner    (1001) docker     (127)     4187 2024-03-07 15:35:12.000000 nci_cidc_schemas-0.26.29/cidc_schemas/schemas/assays/mibi_assay.json
--rw-r--r--   0 runner    (1001) docker     (127)     2078 2024-03-07 15:35:12.000000 nci_cidc_schemas-0.26.29/cidc_schemas/schemas/assays/microbiome_assay.json
--rw-r--r--   0 runner    (1001) docker     (127)     2599 2024-03-07 15:35:12.000000 nci_cidc_schemas-0.26.29/cidc_schemas/schemas/assays/mif_assay.json
--rw-r--r--   0 runner    (1001) docker     (127)     2005 2024-03-07 15:35:12.000000 nci_cidc_schemas-0.26.29/cidc_schemas/schemas/assays/misc_data.json
--rw-r--r--   0 runner    (1001) docker     (127)     2599 2024-03-07 15:35:12.000000 nci_cidc_schemas-0.26.29/cidc_schemas/schemas/assays/nanostring_assay.json
--rw-r--r--   0 runner    (1001) docker     (127)     5193 2024-03-07 15:35:12.000000 nci_cidc_schemas-0.26.29/cidc_schemas/schemas/assays/olink_assay.json
--rw-r--r--   0 runner    (1001) docker     (127)     3043 2024-03-07 15:35:12.000000 nci_cidc_schemas-0.26.29/cidc_schemas/schemas/assays/rna_assay-v0.json
--rw-r--r--   0 runner    (1001) docker     (127)      409 2024-03-07 15:35:12.000000 nci_cidc_schemas-0.26.29/cidc_schemas/schemas/assays/rna_assay.json
--rw-r--r--   0 runner    (1001) docker     (127)     2380 2024-03-07 15:35:12.000000 nci_cidc_schemas-0.26.29/cidc_schemas/schemas/assays/tcr_analysis.json
--rw-r--r--   0 runner    (1001) docker     (127)     4691 2024-03-07 15:35:12.000000 nci_cidc_schemas-0.26.29/cidc_schemas/schemas/assays/tcr_assay.json
--rw-r--r--   0 runner    (1001) docker     (127)     2771 2024-03-07 15:35:12.000000 nci_cidc_schemas-0.26.29/cidc_schemas/schemas/assays/wes_analysis.json
--rw-r--r--   0 runner    (1001) docker     (127)     3776 2024-03-07 15:35:12.000000 nci_cidc_schemas-0.26.29/cidc_schemas/schemas/assays/wes_assay.json
--rw-r--r--   0 runner    (1001) docker     (127)    12858 2024-03-07 15:35:12.000000 nci_cidc_schemas-0.26.29/cidc_schemas/schemas/assays/wes_core.json
--rw-r--r--   0 runner    (1001) docker     (127)     2018 2024-03-07 15:35:12.000000 nci_cidc_schemas-0.26.29/cidc_schemas/schemas/assays/wes_tumor_only_analysis.json
--rw-r--r--   0 runner    (1001) docker     (127)     1474 2024-03-07 15:35:12.000000 nci_cidc_schemas-0.26.29/cidc_schemas/schemas/clinical_data.json
--rw-r--r--   0 runner    (1001) docker     (127)     4652 2024-03-07 15:35:12.000000 nci_cidc_schemas-0.26.29/cidc_schemas/schemas/clinical_trial.json
--rw-r--r--   0 runner    (1001) docker     (127)     2991 2024-03-07 15:35:12.000000 nci_cidc_schemas-0.26.29/cidc_schemas/schemas/participant.json
--rw-r--r--   0 runner    (1001) docker     (127)    16296 2024-03-07 15:35:12.000000 nci_cidc_schemas-0.26.29/cidc_schemas/schemas/sample.json
--rw-r--r--   0 runner    (1001) docker     (127)     3299 2024-03-07 15:35:12.000000 nci_cidc_schemas-0.26.29/cidc_schemas/schemas/shipping_core.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-07 15:35:19.134577 nci_cidc_schemas-0.26.29/cidc_schemas/schemas/templates/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-07 15:35:19.162577 nci_cidc_schemas-0.26.29/cidc_schemas/schemas/templates/analyses/
--rw-r--r--   0 runner    (1001) docker     (127)     5403 2024-03-07 15:35:12.000000 nci_cidc_schemas-0.26.29/cidc_schemas/schemas/templates/analyses/atacseq_analysis_template.json
--rw-r--r--   0 runner    (1001) docker     (127)     6381 2024-03-07 15:35:12.000000 nci_cidc_schemas-0.26.29/cidc_schemas/schemas/templates/analyses/cytof_analysis_template.json
--rw-r--r--   0 runner    (1001) docker     (127)    15944 2024-03-07 15:35:12.000000 nci_cidc_schemas-0.26.29/cidc_schemas/schemas/templates/analyses/rna_level1_analysis_template.json
--rw-r--r--   0 runner    (1001) docker     (127)     3054 2024-03-07 15:35:12.000000 nci_cidc_schemas-0.26.29/cidc_schemas/schemas/templates/analyses/tcr_analysis_template.json
--rw-r--r--   0 runner    (1001) docker     (127)    35033 2024-03-07 15:35:12.000000 nci_cidc_schemas-0.26.29/cidc_schemas/schemas/templates/analyses/wes_analysis_template.json
--rw-r--r--   0 runner    (1001) docker     (127)    16240 2024-03-07 15:35:12.000000 nci_cidc_schemas-0.26.29/cidc_schemas/schemas/templates/analyses/wes_tumor_only_analysis_template.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-07 15:35:19.166577 nci_cidc_schemas-0.26.29/cidc_schemas/schemas/templates/assays/
--rw-r--r--   0 runner    (1001) docker     (127)     3928 2024-03-07 15:35:12.000000 nci_cidc_schemas-0.26.29/cidc_schemas/schemas/templates/assays/atacseq_fastq_template.json
--rw-r--r--   0 runner    (1001) docker     (127)     2193 2024-03-07 15:35:12.000000 nci_cidc_schemas-0.26.29/cidc_schemas/schemas/templates/assays/clinical_data_template.json
--rw-r--r--   0 runner    (1001) docker     (127)     4919 2024-03-07 15:35:12.000000 nci_cidc_schemas-0.26.29/cidc_schemas/schemas/templates/assays/ctdna_template.json
--rw-r--r--   0 runner    (1001) docker     (127)    13328 2024-03-07 15:35:12.000000 nci_cidc_schemas-0.26.29/cidc_schemas/schemas/templates/assays/cytof_template.json
--rw-r--r--   0 runner    (1001) docker     (127)     2259 2024-03-07 15:35:12.000000 nci_cidc_schemas-0.26.29/cidc_schemas/schemas/templates/assays/elisa_template.json
--rw-r--r--   0 runner    (1001) docker     (127)     4293 2024-03-07 15:35:12.000000 nci_cidc_schemas-0.26.29/cidc_schemas/schemas/templates/assays/hande_template.json
--rw-r--r--   0 runner    (1001) docker     (127)     7341 2024-03-07 15:35:12.000000 nci_cidc_schemas-0.26.29/cidc_schemas/schemas/templates/assays/ihc_template.json
--rw-r--r--   0 runner    (1001) docker     (127)     8984 2024-03-07 15:35:12.000000 nci_cidc_schemas-0.26.29/cidc_schemas/schemas/templates/assays/mibi_template.json
--rw-r--r--   0 runner    (1001) docker     (127)     3578 2024-03-07 15:35:12.000000 nci_cidc_schemas-0.26.29/cidc_schemas/schemas/templates/assays/microbiome_template.json
--rw-r--r--   0 runner    (1001) docker     (127)    19272 2024-03-07 15:35:12.000000 nci_cidc_schemas-0.26.29/cidc_schemas/schemas/templates/assays/mif_template.json
--rw-r--r--   0 runner    (1001) docker     (127)     1896 2024-03-07 15:35:12.000000 nci_cidc_schemas-0.26.29/cidc_schemas/schemas/templates/assays/misc_data_template.json
--rw-r--r--   0 runner    (1001) docker     (127)     3214 2024-03-07 15:35:12.000000 nci_cidc_schemas-0.26.29/cidc_schemas/schemas/templates/assays/nanostring_template.json
--rw-r--r--   0 runner    (1001) docker     (127)     6335 2024-03-07 15:35:12.000000 nci_cidc_schemas-0.26.29/cidc_schemas/schemas/templates/assays/olink_template.json
--rw-r--r--   0 runner    (1001) docker     (127)     3084 2024-03-07 15:35:12.000000 nci_cidc_schemas-0.26.29/cidc_schemas/schemas/templates/assays/rna_bam_template.json
--rw-r--r--   0 runner    (1001) docker     (127)     3344 2024-03-07 15:35:12.000000 nci_cidc_schemas-0.26.29/cidc_schemas/schemas/templates/assays/rna_fastq_template.json
--rw-r--r--   0 runner    (1001) docker     (127)     3269 2024-03-07 15:35:12.000000 nci_cidc_schemas-0.26.29/cidc_schemas/schemas/templates/assays/tcr_adaptive_template.json
--rw-r--r--   0 runner    (1001) docker     (127)     3457 2024-03-07 15:35:12.000000 nci_cidc_schemas-0.26.29/cidc_schemas/schemas/templates/assays/tcr_fastq_template.json
--rw-r--r--   0 runner    (1001) docker     (127)     2724 2024-03-07 15:35:12.000000 nci_cidc_schemas-0.26.29/cidc_schemas/schemas/templates/assays/wes_bam_template.json
--rw-r--r--   0 runner    (1001) docker     (127)     3143 2024-03-07 15:35:12.000000 nci_cidc_schemas-0.26.29/cidc_schemas/schemas/templates/assays/wes_fastq_template.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-07 15:35:19.166577 nci_cidc_schemas-0.26.29/cidc_schemas/schemas/templates/manifests/
--rw-r--r--   0 runner    (1001) docker     (127)    12475 2024-03-07 15:35:12.000000 nci_cidc_schemas-0.26.29/cidc_schemas/schemas/templates/manifests/h_and_e_template.json
--rw-r--r--   0 runner    (1001) docker     (127)    11829 2024-03-07 15:35:12.000000 nci_cidc_schemas-0.26.29/cidc_schemas/schemas/templates/manifests/microbiome_dna_template.json
--rw-r--r--   0 runner    (1001) docker     (127)    13346 2024-03-07 15:35:12.000000 nci_cidc_schemas-0.26.29/cidc_schemas/schemas/templates/manifests/normal_blood_dna_template.json
--rw-r--r--   0 runner    (1001) docker     (127)    12989 2024-03-07 15:35:12.000000 nci_cidc_schemas-0.26.29/cidc_schemas/schemas/templates/manifests/normal_tissue_dna_template.json
--rw-r--r--   0 runner    (1001) docker     (127)    17530 2024-03-07 15:35:12.000000 nci_cidc_schemas-0.26.29/cidc_schemas/schemas/templates/manifests/pbmc_template.json
--rw-r--r--   0 runner    (1001) docker     (127)    15099 2024-03-07 15:35:12.000000 nci_cidc_schemas-0.26.29/cidc_schemas/schemas/templates/manifests/plasma_template.json
--rw-r--r--   0 runner    (1001) docker     (127)    11024 2024-03-07 15:35:12.000000 nci_cidc_schemas-0.26.29/cidc_schemas/schemas/templates/manifests/tissue_slide_template.json
--rw-r--r--   0 runner    (1001) docker     (127)     2797 2024-03-07 15:35:12.000000 nci_cidc_schemas-0.26.29/cidc_schemas/schemas/templates/manifests/tumor_normal_pairing_template.json
--rw-r--r--   0 runner    (1001) docker     (127)    13276 2024-03-07 15:35:12.000000 nci_cidc_schemas-0.26.29/cidc_schemas/schemas/templates/manifests/tumor_tissue_dna_template.json
--rw-r--r--   0 runner    (1001) docker     (127)    12568 2024-03-07 15:35:12.000000 nci_cidc_schemas-0.26.29/cidc_schemas/schemas/templates/manifests/tumor_tissue_rna_template.json
--rw-r--r--   0 runner    (1001) docker     (127)    49836 2024-03-07 15:35:12.000000 nci_cidc_schemas-0.26.29/cidc_schemas/template.py
--rw-r--r--   0 runner    (1001) docker     (127)    13119 2024-03-07 15:35:12.000000 nci_cidc_schemas-0.26.29/cidc_schemas/template_reader.py
--rw-r--r--   0 runner    (1001) docker     (127)    18236 2024-03-07 15:35:12.000000 nci_cidc_schemas-0.26.29/cidc_schemas/template_writer.py
--rw-r--r--   0 runner    (1001) docker     (127)    13324 2024-03-07 15:35:12.000000 nci_cidc_schemas-0.26.29/cidc_schemas/unprism.py
--rw-r--r--   0 runner    (1001) docker     (127)     4348 2024-03-07 15:35:12.000000 nci_cidc_schemas-0.26.29/cidc_schemas/util.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-07 15:35:19.182578 nci_cidc_schemas-0.26.29/nci_cidc_schemas.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     4422 2024-03-07 15:35:19.000000 nci_cidc_schemas-0.26.29/nci_cidc_schemas.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    10605 2024-03-07 15:35:19.000000 nci_cidc_schemas-0.26.29/nci_cidc_schemas.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-07 15:35:19.000000 nci_cidc_schemas-0.26.29/nci_cidc_schemas.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       55 2024-03-07 15:35:19.000000 nci_cidc_schemas-0.26.29/nci_cidc_schemas.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-07 15:35:18.000000 nci_cidc_schemas-0.26.29/nci_cidc_schemas.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)      244 2024-03-07 15:35:19.000000 nci_cidc_schemas-0.26.29/nci_cidc_schemas.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       13 2024-03-07 15:35:19.000000 nci_cidc_schemas-0.26.29/nci_cidc_schemas.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      244 2024-03-07 15:35:12.000000 nci_cidc_schemas-0.26.29/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)      395 2024-03-07 15:35:19.186578 nci_cidc_schemas-0.26.29/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1252 2024-03-07 15:35:12.000000 nci_cidc_schemas-0.26.29/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-07 15:35:19.174578 nci_cidc_schemas-0.26.29/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-07 15:35:12.000000 nci_cidc_schemas-0.26.29/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1905 2024-03-07 15:35:12.000000 nci_cidc_schemas-0.26.29/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (127)      341 2024-03-07 15:35:12.000000 nci_cidc_schemas-0.26.29/tests/constants.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-07 15:35:19.174578 nci_cidc_schemas-0.26.29/tests/data/
--rw-r--r--   0 runner    (1001) docker     (127)      223 2024-03-07 15:35:12.000000 nci_cidc_schemas-0.26.29/tests/data/clinical_test_file.1.csv
--rw-r--r--   0 runner    (1001) docker     (127)    10265 2024-03-07 15:35:12.000000 nci_cidc_schemas-0.26.29/tests/data/clinical_test_file.1.xlsx
--rw-r--r--   0 runner    (1001) docker     (127)      251 2024-03-07 15:35:12.000000 nci_cidc_schemas-0.26.29/tests/data/clinical_test_file.2.bom.csv
--rw-r--r--   0 runner    (1001) docker     (127)      248 2024-03-07 15:35:12.000000 nci_cidc_schemas-0.26.29/tests/data/clinical_test_file.2.csv
--rw-r--r--   0 runner    (1001) docker     (127)     9833 2024-03-07 15:35:12.000000 nci_cidc_schemas-0.26.29/tests/data/clinical_test_file.2.xlsx
--rw-r--r--   0 runner    (1001) docker     (127)    10204 2024-03-07 15:35:12.000000 nci_cidc_schemas-0.26.29/tests/data/clinical_test_file.3.xlsx
--rw-r--r--   0 runner    (1001) docker     (127)     4232 2024-03-07 15:35:12.000000 nci_cidc_schemas-0.26.29/tests/data/clinical_test_file.docx
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-07 15:35:19.174578 nci_cidc_schemas-0.26.29/tests/data/clinicaltrial_examples/
--rw-r--r--   0 runner    (1001) docker     (127)    19111 2024-03-07 15:35:12.000000 nci_cidc_schemas-0.26.29/tests/data/clinicaltrial_examples/CT_1.json
--rw-r--r--   0 runner    (1001) docker     (127)    24203 2024-03-07 15:35:12.000000 nci_cidc_schemas-0.26.29/tests/data/clinicaltrial_examples/CT_1PA_multiWES.json
--rw-r--r--   0 runner    (1001) docker     (127)    14837 2024-03-07 15:35:12.000000 nci_cidc_schemas-0.26.29/tests/data/clinicaltrial_examples/CT_cytof_with_analysis.json
--rw-r--r--   0 runner    (1001) docker     (127)     6098 2024-03-07 15:35:12.000000 nci_cidc_schemas-0.26.29/tests/data/clinicaltrial_examples/CT_ihc.json
--rw-r--r--   0 runner    (1001) docker     (127)     1451 2024-03-07 15:35:12.000000 nci_cidc_schemas-0.26.29/tests/data/clinicaltrial_examples/CT_minimal.json
--rw-r--r--   0 runner    (1001) docker     (127)     5215 2024-03-07 15:35:12.000000 nci_cidc_schemas-0.26.29/tests/data/date_examples.xlsx
--rw-r--r--   0 runner    (1001) docker     (127)     5954 2024-03-07 15:35:12.000000 nci_cidc_schemas-0.26.29/tests/data/elisa_test_file.1.xlsx
--rw-r--r--   0 runner    (1001) docker     (127)    12084 2024-03-07 15:35:12.000000 nci_cidc_schemas-0.26.29/tests/data/elisa_test_file.2.xlsx
--rw-r--r--   0 runner    (1001) docker     (127)    26605 2024-03-07 15:35:12.000000 nci_cidc_schemas-0.26.29/tests/data/hande_err_template.xlsx
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-07 15:35:19.178578 nci_cidc_schemas-0.26.29/tests/data/olink/
--rw-r--r--   0 runner    (1001) docker     (127)    13070 2024-03-07 15:35:12.000000 nci_cidc_schemas-0.26.29/tests/data/olink/invalid_olink_assay_1_NPX.xlsx
--rw-r--r--   0 runner    (1001) docker     (127)    17905 2024-03-07 15:35:12.000000 nci_cidc_schemas-0.26.29/tests/data/olink/olink_assay_1_NPX.xlsx
--rw-r--r--   0 runner    (1001) docker     (127)    12969 2024-03-07 15:35:12.000000 nci_cidc_schemas-0.26.29/tests/data/olink/olink_assay_2_NPX.xlsx
--rw-r--r--   0 runner    (1001) docker     (127)    21276 2024-03-07 15:35:12.000000 nci_cidc_schemas-0.26.29/tests/data/olink/olink_assay_combined.xlsx
--rw-r--r--   0 runner    (1001) docker     (127)    13301 2024-03-07 15:35:12.000000 nci_cidc_schemas-0.26.29/tests/data/pbmc_invalid.xlsx
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-07 15:35:19.178578 nci_cidc_schemas-0.26.29/tests/data/schemas/
--rw-r--r--   0 runner    (1001) docker     (127)      144 2024-03-07 15:35:12.000000 nci_cidc_schemas-0.26.29/tests/data/schemas/1.json
--rw-r--r--   0 runner    (1001) docker     (127)      199 2024-03-07 15:35:12.000000 nci_cidc_schemas-0.26.29/tests/data/schemas/a.json
--rw-r--r--   0 runner    (1001) docker     (127)      407 2024-03-07 15:35:12.000000 nci_cidc_schemas-0.26.29/tests/data/schemas/b.json
--rw-r--r--   0 runner    (1001) docker     (127)      189 2024-03-07 15:35:12.000000 nci_cidc_schemas-0.26.29/tests/data/schemas/c.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-07 15:35:19.178578 nci_cidc_schemas-0.26.29/tests/data/schemas/d1/
--rw-r--r--   0 runner    (1001) docker     (127)      127 2024-03-07 15:35:12.000000 nci_cidc_schemas-0.26.29/tests/data/schemas/d1/3.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-07 15:35:19.178578 nci_cidc_schemas-0.26.29/tests/data/schemas/d1/d2/
--rw-r--r--   0 runner    (1001) docker     (127)      141 2024-03-07 15:35:12.000000 nci_cidc_schemas-0.26.29/tests/data/schemas/d1/d2/2.json
--rw-r--r--   0 runner    (1001) docker     (127)      149 2024-03-07 15:35:12.000000 nci_cidc_schemas-0.26.29/tests/data/schemas/invalid_ref.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-07 15:35:19.178578 nci_cidc_schemas-0.26.29/tests/data/schemas/target-templates/
--rw-r--r--   0 runner    (1001) docker     (127)     5403 2024-03-07 15:35:12.000000 nci_cidc_schemas-0.26.29/tests/data/schemas/target-templates/atacseq_analysis_template.json
--rw-r--r--   0 runner    (1001) docker     (127)    12507 2024-03-07 15:35:12.000000 nci_cidc_schemas-0.26.29/tests/data/schemas/target-templates/rna_level1_analysis_template.json
--rw-r--r--   0 runner    (1001) docker     (127)    35065 2024-03-07 15:35:12.000000 nci_cidc_schemas-0.26.29/tests/data/schemas/target-templates/wes_analysis_template.json
--rw-r--r--   0 runner    (1001) docker     (127)    16256 2024-03-07 15:35:12.000000 nci_cidc_schemas-0.26.29/tests/data/schemas/target-templates/wes_tumor_only_analysis_template.json
--rw-r--r--   0 runner    (1001) docker     (127)     5464 2024-03-07 15:35:12.000000 nci_cidc_schemas-0.26.29/tests/data/tiny_invalid_manifest.xlsx
--rw-r--r--   0 runner    (1001) docker     (127)     5455 2024-03-07 15:35:12.000000 nci_cidc_schemas-0.26.29/tests/data/tiny_valid_manifest.xlsx
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-07 15:35:19.178578 nci_cidc_schemas-0.26.29/tests/prism/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-07 15:35:12.000000 nci_cidc_schemas-0.26.29/tests/prism/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-07 15:35:19.182578 nci_cidc_schemas-0.26.29/tests/prism/cidc_test_data/
--rw-r--r--   0 runner    (1001) docker     (127)      409 2024-03-07 15:35:12.000000 nci_cidc_schemas-0.26.29/tests/prism/cidc_test_data/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)   135759 2024-03-07 15:35:12.000000 nci_cidc_schemas-0.26.29/tests/prism/cidc_test_data/analysis_data.py
--rw-r--r--   0 runner    (1001) docker     (127)   164904 2024-03-07 15:35:12.000000 nci_cidc_schemas-0.26.29/tests/prism/cidc_test_data/assay_data.py
--rw-r--r--   0 runner    (1001) docker     (127)   104350 2024-03-07 15:35:12.000000 nci_cidc_schemas-0.26.29/tests/prism/cidc_test_data/manifest_data.py
--rw-r--r--   0 runner    (1001) docker     (127)     3035 2024-03-07 15:35:12.000000 nci_cidc_schemas-0.26.29/tests/prism/cidc_test_data/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-07 15:35:19.182578 nci_cidc_schemas-0.26.29/tests/prism/schema/
--rw-r--r--   0 runner    (1001) docker     (127)     2676 2024-03-07 15:35:12.000000 nci_cidc_schemas-0.26.29/tests/prism/schema/test_schema.json
--rw-r--r--   0 runner    (1001) docker     (127)     7119 2024-03-07 15:35:12.000000 nci_cidc_schemas-0.26.29/tests/prism/test_cidc_data_model.py
--rw-r--r--   0 runner    (1001) docker     (127)      410 2024-03-07 15:35:12.000000 nci_cidc_schemas-0.26.29/tests/prism/test_constants.py
--rw-r--r--   0 runner    (1001) docker     (127)    31915 2024-03-07 15:35:12.000000 nci_cidc_schemas-0.26.29/tests/prism/test_core.py
--rw-r--r--   0 runner    (1001) docker     (127)     5574 2024-03-07 15:35:12.000000 nci_cidc_schemas-0.26.29/tests/prism/test_extra_metadata.py
--rw-r--r--   0 runner    (1001) docker     (127)    13863 2024-03-07 15:35:12.000000 nci_cidc_schemas-0.26.29/tests/prism/test_merger.py
--rw-r--r--   0 runner    (1001) docker     (127)    29144 2024-03-07 15:35:12.000000 nci_cidc_schemas-0.26.29/tests/prism/test_pipelines.py
--rw-r--r--   0 runner    (1001) docker     (127)     4467 2024-03-07 15:35:12.000000 nci_cidc_schemas-0.26.29/tests/test_artifacts.py
--rw-r--r--   0 runner    (1001) docker     (127)    17446 2024-03-07 15:35:12.000000 nci_cidc_schemas-0.26.29/tests/test_assays.py
--rw-r--r--   0 runner    (1001) docker     (127)     1443 2024-03-07 15:35:12.000000 nci_cidc_schemas-0.26.29/tests/test_clinicaltrial_examples.py
--rw-r--r--   0 runner    (1001) docker     (127)    14541 2024-03-07 15:35:12.000000 nci_cidc_schemas-0.26.29/tests/test_json_validation.py
--rw-r--r--   0 runner    (1001) docker     (127)    15991 2024-03-07 15:35:12.000000 nci_cidc_schemas-0.26.29/tests/test_migrations.py
--rw-r--r--   0 runner    (1001) docker     (127)     1389 2024-03-07 15:35:12.000000 nci_cidc_schemas-0.26.29/tests/test_schemas.py
--rw-r--r--   0 runner    (1001) docker     (127)     2925 2024-03-07 15:35:12.000000 nci_cidc_schemas-0.26.29/tests/test_strict_meta_schema.py
--rw-r--r--   0 runner    (1001) docker     (127)    25566 2024-03-07 15:35:12.000000 nci_cidc_schemas-0.26.29/tests/test_template.py
--rw-r--r--   0 runner    (1001) docker     (127)     7390 2024-03-07 15:35:12.000000 nci_cidc_schemas-0.26.29/tests/test_template_reader.py
--rw-r--r--   0 runner    (1001) docker     (127)     2162 2024-03-07 15:35:12.000000 nci_cidc_schemas-0.26.29/tests/test_template_writer.py
--rw-r--r--   0 runner    (1001) docker     (127)     4499 2024-03-07 15:35:12.000000 nci_cidc_schemas-0.26.29/tests/test_templates.py
--rw-r--r--   0 runner    (1001) docker     (127)     4001 2024-03-07 15:35:12.000000 nci_cidc_schemas-0.26.29/tests/test_trial_core.py
--rw-r--r--   0 runner    (1001) docker     (127)    10655 2024-03-07 15:35:12.000000 nci_cidc_schemas-0.26.29/tests/test_unprism.py
--rw-r--r--   0 runner    (1001) docker     (127)     3294 2024-03-07 15:35:12.000000 nci_cidc_schemas-0.26.29/tests/test_util.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-07 15:35:19.182578 nci_cidc_schemas-0.26.29/tests/utils/
--rw-r--r--   0 runner    (1001) docker     (127)     2793 2024-03-07 15:35:12.000000 nci_cidc_schemas-0.26.29/tests/utils/test_template_generator.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 19:04:33.343147 nci_cidc_schemas-0.26.32/
+-rw-r--r--   0 runner    (1001) docker     (127)     1072 2024-04-29 19:04:27.000000 nci_cidc_schemas-0.26.32/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      315 2024-04-29 19:04:27.000000 nci_cidc_schemas-0.26.32/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     4422 2024-04-29 19:04:33.343147 nci_cidc_schemas-0.26.32/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3365 2024-04-29 19:04:27.000000 nci_cidc_schemas-0.26.32/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 19:04:33.295146 nci_cidc_schemas-0.26.32/cidc_schemas/
+-rw-r--r--   0 runner    (1001) docker     (127)      136 2024-04-29 19:04:27.000000 nci_cidc_schemas-0.26.32/cidc_schemas/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4099 2024-04-29 19:04:27.000000 nci_cidc_schemas-0.26.32/cidc_schemas/cli.py
+-rw-r--r--   0 runner    (1001) docker     (127)      698 2024-04-29 19:04:27.000000 nci_cidc_schemas-0.26.32/cidc_schemas/constants.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20035 2024-04-29 19:04:27.000000 nci_cidc_schemas-0.26.32/cidc_schemas/json_validation.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 19:04:33.295146 nci_cidc_schemas-0.26.32/cidc_schemas/metaschema/
+-rw-r--r--   0 runner    (1001) docker     (127)     6428 2024-04-29 19:04:27.000000 nci_cidc_schemas-0.26.32/cidc_schemas/metaschema/strict_meta_schema.json
+-rw-r--r--   0 runner    (1001) docker     (127)    14766 2024-04-29 19:04:27.000000 nci_cidc_schemas-0.26.32/cidc_schemas/migrations.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 19:04:33.299146 nci_cidc_schemas-0.26.32/cidc_schemas/pipeline_configs/
+-rw-r--r--   0 runner    (1001) docker     (127)     2832 2024-04-29 19:04:27.000000 nci_cidc_schemas-0.26.32/cidc_schemas/pipeline_configs/rna_level1_analysis_config.yaml.j2
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 19:04:33.299146 nci_cidc_schemas-0.26.32/cidc_schemas/prism/
+-rw-r--r--   0 runner    (1001) docker     (127)      530 2024-04-29 19:04:27.000000 nci_cidc_schemas-0.26.32/cidc_schemas/prism/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2379 2024-04-29 19:04:27.000000 nci_cidc_schemas-0.26.32/cidc_schemas/prism/constants.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19294 2024-04-29 19:04:27.000000 nci_cidc_schemas-0.26.32/cidc_schemas/prism/core.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8559 2024-04-29 19:04:27.000000 nci_cidc_schemas-0.26.32/cidc_schemas/prism/extra_metadata.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12431 2024-04-29 19:04:27.000000 nci_cidc_schemas-0.26.32/cidc_schemas/prism/merger.py
+-rw-r--r--   0 runner    (1001) docker     (127)    33532 2024-04-29 19:04:27.000000 nci_cidc_schemas-0.26.32/cidc_schemas/prism/pipelines.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 19:04:33.299146 nci_cidc_schemas-0.26.32/cidc_schemas/schemas/
+-rw-r--r--   0 runner    (1001) docker     (127)     1943 2024-04-29 19:04:27.000000 nci_cidc_schemas-0.26.32/cidc_schemas/schemas/aliquot.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 19:04:33.307146 nci_cidc_schemas-0.26.32/cidc_schemas/schemas/artifacts/
+-rw-r--r--   0 runner    (1001) docker     (127)     1653 2024-04-29 19:04:27.000000 nci_cidc_schemas-0.26.32/cidc_schemas/schemas/artifacts/artifact_bam.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1671 2024-04-29 19:04:27.000000 nci_cidc_schemas-0.26.32/cidc_schemas/schemas/artifacts/artifact_bam_bai.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1653 2024-04-29 19:04:27.000000 nci_cidc_schemas-0.26.32/cidc_schemas/schemas/artifacts/artifact_bed.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1665 2024-04-29 19:04:27.000000 nci_cidc_schemas-0.26.32/cidc_schemas/schemas/artifacts/artifact_bigwig.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1665 2024-04-29 19:04:27.000000 nci_cidc_schemas-0.26.32/cidc_schemas/schemas/artifacts/artifact_binary.json
+-rw-r--r--   0 runner    (1001) docker     (127)     2114 2024-04-29 19:04:27.000000 nci_cidc_schemas-0.26.32/cidc_schemas/schemas/artifacts/artifact_clinical_csv.json
+-rw-r--r--   0 runner    (1001) docker     (127)     2232 2024-04-29 19:04:27.000000 nci_cidc_schemas-0.26.32/cidc_schemas/schemas/artifacts/artifact_clinical_docx.json
+-rw-r--r--   0 runner    (1001) docker     (127)     2232 2024-04-29 19:04:27.000000 nci_cidc_schemas-0.26.32/cidc_schemas/schemas/artifacts/artifact_clinical_xlsx.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1657 2024-04-29 19:04:27.000000 nci_cidc_schemas-0.26.32/cidc_schemas/schemas/artifacts/artifact_cncf.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1653 2024-04-29 19:04:27.000000 nci_cidc_schemas-0.26.32/cidc_schemas/schemas/artifacts/artifact_cns.json
+-rw-r--r--   0 runner    (1001) docker     (127)     3140 2024-04-29 19:04:27.000000 nci_cidc_schemas-0.26.32/cidc_schemas/schemas/artifacts/artifact_core.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1665 2024-04-29 19:04:27.000000 nci_cidc_schemas-0.26.32/cidc_schemas/schemas/artifacts/artifact_csv.json
+-rw-r--r--   0 runner    (1001) docker     (127)     2216 2024-04-29 19:04:27.000000 nci_cidc_schemas-0.26.32/cidc_schemas/schemas/artifacts/artifact_elisa_xlsx.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1683 2024-04-29 19:04:27.000000 nci_cidc_schemas-0.26.32/cidc_schemas/schemas/artifacts/artifact_fastq_gz.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1653 2024-04-29 19:04:27.000000 nci_cidc_schemas-0.26.32/cidc_schemas/schemas/artifacts/artifact_fcs.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1668 2024-04-29 19:04:27.000000 nci_cidc_schemas-0.26.32/cidc_schemas/schemas/artifacts/artifact_file.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1649 2024-04-29 19:04:27.000000 nci_cidc_schemas-0.26.32/cidc_schemas/schemas/artifacts/artifact_gz.json
+-rw-r--r--   0 runner    (1001) docker     (127)     2015 2024-04-29 19:04:27.000000 nci_cidc_schemas-0.26.32/cidc_schemas/schemas/artifacts/artifact_image.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1653 2024-04-29 19:04:27.000000 nci_cidc_schemas-0.26.32/cidc_schemas/schemas/artifacts/artifact_jpg.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1657 2024-04-29 19:04:27.000000 nci_cidc_schemas-0.26.32/cidc_schemas/schemas/artifacts/artifact_json.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1775 2024-04-29 19:04:27.000000 nci_cidc_schemas-0.26.32/cidc_schemas/schemas/artifacts/artifact_junction.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1755 2024-04-29 19:04:27.000000 nci_cidc_schemas-0.26.32/cidc_schemas/schemas/artifacts/artifact_log.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1653 2024-04-29 19:04:27.000000 nci_cidc_schemas-0.26.32/cidc_schemas/schemas/artifacts/artifact_maf.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1681 2024-04-29 19:04:27.000000 nci_cidc_schemas-0.26.32/cidc_schemas/schemas/artifacts/artifact_narrowPeak.json
+-rw-r--r--   0 runner    (1001) docker     (127)     2134 2024-04-29 19:04:27.000000 nci_cidc_schemas-0.26.32/cidc_schemas/schemas/artifacts/artifact_npx.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1674 2024-04-29 19:04:27.000000 nci_cidc_schemas-0.26.32/cidc_schemas/schemas/artifacts/artifact_pdf.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1653 2024-04-29 19:04:27.000000 nci_cidc_schemas-0.26.32/cidc_schemas/schemas/artifacts/artifact_png.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1704 2024-04-29 19:04:27.000000 nci_cidc_schemas-0.26.32/cidc_schemas/schemas/artifacts/artifact_rcc.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1661 2024-04-29 19:04:27.000000 nci_cidc_schemas-0.26.32/cidc_schemas/schemas/artifacts/artifact_rdata.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1661 2024-04-29 19:04:27.000000 nci_cidc_schemas-0.26.32/cidc_schemas/schemas/artifacts/artifact_tbi.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1657 2024-04-29 19:04:27.000000 nci_cidc_schemas-0.26.32/cidc_schemas/schemas/artifacts/artifact_text.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1663 2024-04-29 19:04:27.000000 nci_cidc_schemas-0.26.32/cidc_schemas/schemas/artifacts/artifact_tsv.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1653 2024-04-29 19:04:27.000000 nci_cidc_schemas-0.26.32/cidc_schemas/schemas/artifacts/artifact_vcf.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1675 2024-04-29 19:04:27.000000 nci_cidc_schemas-0.26.32/cidc_schemas/schemas/artifacts/artifact_vcf_gz.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1659 2024-04-29 19:04:27.000000 nci_cidc_schemas-0.26.32/cidc_schemas/schemas/artifacts/artifact_xlsx.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1657 2024-04-29 19:04:27.000000 nci_cidc_schemas-0.26.32/cidc_schemas/schemas/artifacts/artifact_yaml.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1653 2024-04-29 19:04:27.000000 nci_cidc_schemas-0.26.32/cidc_schemas/schemas/artifacts/artifact_zip.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 19:04:33.311147 nci_cidc_schemas-0.26.32/cidc_schemas/schemas/assays/
+-rw-r--r--   0 runner    (1001) docker     (127)     2547 2024-04-29 19:04:27.000000 nci_cidc_schemas-0.26.32/cidc_schemas/schemas/assays/atacseq_assay.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 19:04:33.315147 nci_cidc_schemas-0.26.32/cidc_schemas/schemas/assays/components/
+-rw-r--r--   0 runner    (1001) docker     (127)      960 2024-04-29 19:04:27.000000 nci_cidc_schemas-0.26.32/cidc_schemas/schemas/assays/components/antibody.json
+-rw-r--r--   0 runner    (1001) docker     (127)      485 2024-04-29 19:04:27.000000 nci_cidc_schemas-0.26.32/cidc_schemas/schemas/assays/components/assay_core.json
+-rw-r--r--   0 runner    (1001) docker     (127)     3540 2024-04-29 19:04:27.000000 nci_cidc_schemas-0.26.32/cidc_schemas/schemas/assays/components/available_assays.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1237 2024-04-29 19:04:27.000000 nci_cidc_schemas-0.26.32/cidc_schemas/schemas/assays/components/available_ngs_analyses.json
+-rw-r--r--   0 runner    (1001) docker     (127)      733 2024-04-29 19:04:27.000000 nci_cidc_schemas-0.26.32/cidc_schemas/schemas/assays/components/composite_image.json
+-rw-r--r--   0 runner    (1001) docker     (127)      458 2024-04-29 19:04:27.000000 nci_cidc_schemas-0.26.32/cidc_schemas/schemas/assays/components/controls.json
+-rw-r--r--   0 runner    (1001) docker     (127)      813 2024-04-29 19:04:27.000000 nci_cidc_schemas-0.26.32/cidc_schemas/schemas/assays/components/enrichment_core.json
+-rw-r--r--   0 runner    (1001) docker     (127)      663 2024-04-29 19:04:27.000000 nci_cidc_schemas-0.26.32/cidc_schemas/schemas/assays/components/excluded_samples.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1260 2024-04-29 19:04:27.000000 nci_cidc_schemas-0.26.32/cidc_schemas/schemas/assays/components/image.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 19:04:33.315147 nci_cidc_schemas-0.26.32/cidc_schemas/schemas/assays/components/imaging/
+-rw-r--r--   0 runner    (1001) docker     (127)      546 2024-04-29 19:04:27.000000 nci_cidc_schemas-0.26.32/cidc_schemas/schemas/assays/components/imaging/mif_entry.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1728 2024-04-29 19:04:27.000000 nci_cidc_schemas-0.26.32/cidc_schemas/schemas/assays/components/imaging/mif_export.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1000 2024-04-29 19:04:27.000000 nci_cidc_schemas-0.26.32/cidc_schemas/schemas/assays/components/imaging/mif_input.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1112 2024-04-29 19:04:27.000000 nci_cidc_schemas-0.26.32/cidc_schemas/schemas/assays/components/imaging/mif_roi.json
+-rw-r--r--   0 runner    (1001) docker     (127)      926 2024-04-29 19:04:27.000000 nci_cidc_schemas-0.26.32/cidc_schemas/schemas/assays/components/imaging_data.json
+-rw-r--r--   0 runner    (1001) docker     (127)      405 2024-04-29 19:04:27.000000 nci_cidc_schemas-0.26.32/cidc_schemas/schemas/assays/components/local_file.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1663 2024-04-29 19:04:27.000000 nci_cidc_schemas-0.26.32/cidc_schemas/schemas/assays/components/mapping.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1831 2024-04-29 19:04:27.000000 nci_cidc_schemas-0.26.32/cidc_schemas/schemas/assays/components/mibi_antibody.json
+-rw-r--r--   0 runner    (1001) docker     (127)     2191 2024-04-29 19:04:27.000000 nci_cidc_schemas-0.26.32/cidc_schemas/schemas/assays/components/mif_antibody.json
+-rw-r--r--   0 runner    (1001) docker     (127)      480 2024-04-29 19:04:27.000000 nci_cidc_schemas-0.26.32/cidc_schemas/schemas/assays/components/multiple_local_files.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 19:04:33.315147 nci_cidc_schemas-0.26.32/cidc_schemas/schemas/assays/components/ngs/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 19:04:33.315147 nci_cidc_schemas-0.26.32/cidc_schemas/schemas/assays/components/ngs/atacseq/
+-rw-r--r--   0 runner    (1001) docker     (127)     2283 2024-04-29 19:04:27.000000 nci_cidc_schemas-0.26.32/cidc_schemas/schemas/assays/components/ngs/atacseq/atacseq_analysis.json
+-rw-r--r--   0 runner    (1001) docker     (127)      615 2024-04-29 19:04:27.000000 nci_cidc_schemas-0.26.32/cidc_schemas/schemas/assays/components/ngs/ngs_assay_record.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 19:04:33.319147 nci_cidc_schemas-0.26.32/cidc_schemas/schemas/assays/components/ngs/rna/
+-rw-r--r--   0 runner    (1001) docker     (127)      392 2024-04-29 19:04:27.000000 nci_cidc_schemas-0.26.32/cidc_schemas/schemas/assays/components/ngs/rna/fusion.json
+-rw-r--r--   0 runner    (1001) docker     (127)      395 2024-04-29 19:04:27.000000 nci_cidc_schemas-0.26.32/cidc_schemas/schemas/assays/components/ngs/rna/microbiome.json
+-rw-r--r--   0 runner    (1001) docker     (127)      398 2024-04-29 19:04:27.000000 nci_cidc_schemas-0.26.32/cidc_schemas/schemas/assays/components/ngs/rna/msisensor.json
+-rw-r--r--   0 runner    (1001) docker     (127)      385 2024-04-29 19:04:27.000000 nci_cidc_schemas-0.26.32/cidc_schemas/schemas/assays/components/ngs/rna/neoantigen.json
+-rw-r--r--   0 runner    (1001) docker     (127)      605 2024-04-29 19:04:27.000000 nci_cidc_schemas-0.26.32/cidc_schemas/schemas/assays/components/ngs/rna/rna_analysis.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1432 2024-04-29 19:04:27.000000 nci_cidc_schemas-0.26.32/cidc_schemas/schemas/assays/components/ngs/rna/rna_level1_analysis.json
+-rw-r--r--   0 runner    (1001) docker     (127)      541 2024-04-29 19:04:27.000000 nci_cidc_schemas-0.26.32/cidc_schemas/schemas/assays/components/ngs/rna/rseqc.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1375 2024-04-29 19:04:27.000000 nci_cidc_schemas-0.26.32/cidc_schemas/schemas/assays/components/ngs/rna/salmon.json
+-rw-r--r--   0 runner    (1001) docker     (127)      772 2024-04-29 19:04:27.000000 nci_cidc_schemas-0.26.32/cidc_schemas/schemas/assays/components/ngs/rna/star.json
+-rw-r--r--   0 runner    (1001) docker     (127)      382 2024-04-29 19:04:27.000000 nci_cidc_schemas-0.26.32/cidc_schemas/schemas/assays/components/ngs/rna/trust4.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1229 2024-04-29 19:04:27.000000 nci_cidc_schemas-0.26.32/cidc_schemas/schemas/assays/components/ngs_assay_core.json
+-rw-r--r--   0 runner    (1001) docker     (127)      615 2024-04-29 19:04:27.000000 nci_cidc_schemas-0.26.32/cidc_schemas/schemas/assays/components/ngs_assay_record.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1139 2024-04-29 19:04:27.000000 nci_cidc_schemas-0.26.32/cidc_schemas/schemas/assays/components/reads_core.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1091 2024-04-29 19:04:27.000000 nci_cidc_schemas-0.26.32/cidc_schemas/schemas/assays/components/reads_with_index.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1513 2024-04-29 19:04:27.000000 nci_cidc_schemas-0.26.32/cidc_schemas/schemas/assays/ctdna_analysis.json
+-rw-r--r--   0 runner    (1001) docker     (127)     3503 2024-04-29 19:04:27.000000 nci_cidc_schemas-0.26.32/cidc_schemas/schemas/assays/ctdna_assay.json
+-rw-r--r--   0 runner    (1001) docker     (127)     3659 2024-04-29 19:04:27.000000 nci_cidc_schemas-0.26.32/cidc_schemas/schemas/assays/cytof_assay.json
+-rw-r--r--   0 runner    (1001) docker     (127)     8828 2024-04-29 19:04:27.000000 nci_cidc_schemas-0.26.32/cidc_schemas/schemas/assays/cytof_assay_core.json
+-rw-r--r--   0 runner    (1001) docker     (127)     2233 2024-04-29 19:04:27.000000 nci_cidc_schemas-0.26.32/cidc_schemas/schemas/assays/elisa_assay.json
+-rw-r--r--   0 runner    (1001) docker     (127)     3192 2024-04-29 19:04:27.000000 nci_cidc_schemas-0.26.32/cidc_schemas/schemas/assays/hande_assay.json
+-rw-r--r--   0 runner    (1001) docker     (127)     6738 2024-04-29 19:04:27.000000 nci_cidc_schemas-0.26.32/cidc_schemas/schemas/assays/ihc_assay.json
+-rw-r--r--   0 runner    (1001) docker     (127)     4187 2024-04-29 19:04:27.000000 nci_cidc_schemas-0.26.32/cidc_schemas/schemas/assays/mibi_assay.json
+-rw-r--r--   0 runner    (1001) docker     (127)     2078 2024-04-29 19:04:27.000000 nci_cidc_schemas-0.26.32/cidc_schemas/schemas/assays/microbiome_assay.json
+-rw-r--r--   0 runner    (1001) docker     (127)     2599 2024-04-29 19:04:27.000000 nci_cidc_schemas-0.26.32/cidc_schemas/schemas/assays/mif_assay.json
+-rw-r--r--   0 runner    (1001) docker     (127)     2005 2024-04-29 19:04:27.000000 nci_cidc_schemas-0.26.32/cidc_schemas/schemas/assays/misc_data.json
+-rw-r--r--   0 runner    (1001) docker     (127)     2599 2024-04-29 19:04:27.000000 nci_cidc_schemas-0.26.32/cidc_schemas/schemas/assays/nanostring_assay.json
+-rw-r--r--   0 runner    (1001) docker     (127)     5193 2024-04-29 19:04:27.000000 nci_cidc_schemas-0.26.32/cidc_schemas/schemas/assays/olink_assay.json
+-rw-r--r--   0 runner    (1001) docker     (127)     3043 2024-04-29 19:04:27.000000 nci_cidc_schemas-0.26.32/cidc_schemas/schemas/assays/rna_assay-v0.json
+-rw-r--r--   0 runner    (1001) docker     (127)      409 2024-04-29 19:04:27.000000 nci_cidc_schemas-0.26.32/cidc_schemas/schemas/assays/rna_assay.json
+-rw-r--r--   0 runner    (1001) docker     (127)     2380 2024-04-29 19:04:27.000000 nci_cidc_schemas-0.26.32/cidc_schemas/schemas/assays/tcr_analysis.json
+-rw-r--r--   0 runner    (1001) docker     (127)     4691 2024-04-29 19:04:27.000000 nci_cidc_schemas-0.26.32/cidc_schemas/schemas/assays/tcr_assay.json
+-rw-r--r--   0 runner    (1001) docker     (127)     2771 2024-04-29 19:04:27.000000 nci_cidc_schemas-0.26.32/cidc_schemas/schemas/assays/wes_analysis.json
+-rw-r--r--   0 runner    (1001) docker     (127)     3776 2024-04-29 19:04:27.000000 nci_cidc_schemas-0.26.32/cidc_schemas/schemas/assays/wes_assay.json
+-rw-r--r--   0 runner    (1001) docker     (127)    12858 2024-04-29 19:04:27.000000 nci_cidc_schemas-0.26.32/cidc_schemas/schemas/assays/wes_core.json
+-rw-r--r--   0 runner    (1001) docker     (127)     2018 2024-04-29 19:04:27.000000 nci_cidc_schemas-0.26.32/cidc_schemas/schemas/assays/wes_tumor_only_analysis.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1474 2024-04-29 19:04:27.000000 nci_cidc_schemas-0.26.32/cidc_schemas/schemas/clinical_data.json
+-rw-r--r--   0 runner    (1001) docker     (127)     4652 2024-04-29 19:04:27.000000 nci_cidc_schemas-0.26.32/cidc_schemas/schemas/clinical_trial.json
+-rw-r--r--   0 runner    (1001) docker     (127)     2991 2024-04-29 19:04:27.000000 nci_cidc_schemas-0.26.32/cidc_schemas/schemas/participant.json
+-rw-r--r--   0 runner    (1001) docker     (127)    16296 2024-04-29 19:04:27.000000 nci_cidc_schemas-0.26.32/cidc_schemas/schemas/sample.json
+-rw-r--r--   0 runner    (1001) docker     (127)     3299 2024-04-29 19:04:27.000000 nci_cidc_schemas-0.26.32/cidc_schemas/schemas/shipping_core.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 19:04:33.291146 nci_cidc_schemas-0.26.32/cidc_schemas/schemas/templates/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 19:04:33.319147 nci_cidc_schemas-0.26.32/cidc_schemas/schemas/templates/analyses/
+-rw-r--r--   0 runner    (1001) docker     (127)     5403 2024-04-29 19:04:27.000000 nci_cidc_schemas-0.26.32/cidc_schemas/schemas/templates/analyses/atacseq_analysis_template.json
+-rw-r--r--   0 runner    (1001) docker     (127)     7408 2024-04-29 19:04:27.000000 nci_cidc_schemas-0.26.32/cidc_schemas/schemas/templates/analyses/ctdna_analysis_template.json
+-rw-r--r--   0 runner    (1001) docker     (127)     6381 2024-04-29 19:04:27.000000 nci_cidc_schemas-0.26.32/cidc_schemas/schemas/templates/analyses/cytof_analysis_template.json
+-rw-r--r--   0 runner    (1001) docker     (127)    15944 2024-04-29 19:04:27.000000 nci_cidc_schemas-0.26.32/cidc_schemas/schemas/templates/analyses/rna_level1_analysis_template.json
+-rw-r--r--   0 runner    (1001) docker     (127)     3054 2024-04-29 19:04:27.000000 nci_cidc_schemas-0.26.32/cidc_schemas/schemas/templates/analyses/tcr_analysis_template.json
+-rw-r--r--   0 runner    (1001) docker     (127)    35033 2024-04-29 19:04:27.000000 nci_cidc_schemas-0.26.32/cidc_schemas/schemas/templates/analyses/wes_analysis_template.json
+-rw-r--r--   0 runner    (1001) docker     (127)    16240 2024-04-29 19:04:27.000000 nci_cidc_schemas-0.26.32/cidc_schemas/schemas/templates/analyses/wes_tumor_only_analysis_template.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 19:04:33.323147 nci_cidc_schemas-0.26.32/cidc_schemas/schemas/templates/assays/
+-rw-r--r--   0 runner    (1001) docker     (127)     3928 2024-04-29 19:04:27.000000 nci_cidc_schemas-0.26.32/cidc_schemas/schemas/templates/assays/atacseq_fastq_template.json
+-rw-r--r--   0 runner    (1001) docker     (127)     2193 2024-04-29 19:04:27.000000 nci_cidc_schemas-0.26.32/cidc_schemas/schemas/templates/assays/clinical_data_template.json
+-rw-r--r--   0 runner    (1001) docker     (127)     5966 2024-04-29 19:04:27.000000 nci_cidc_schemas-0.26.32/cidc_schemas/schemas/templates/assays/ctdna_template.json
+-rw-r--r--   0 runner    (1001) docker     (127)    13328 2024-04-29 19:04:27.000000 nci_cidc_schemas-0.26.32/cidc_schemas/schemas/templates/assays/cytof_template.json
+-rw-r--r--   0 runner    (1001) docker     (127)     2259 2024-04-29 19:04:27.000000 nci_cidc_schemas-0.26.32/cidc_schemas/schemas/templates/assays/elisa_template.json
+-rw-r--r--   0 runner    (1001) docker     (127)     4293 2024-04-29 19:04:27.000000 nci_cidc_schemas-0.26.32/cidc_schemas/schemas/templates/assays/hande_template.json
+-rw-r--r--   0 runner    (1001) docker     (127)     7341 2024-04-29 19:04:27.000000 nci_cidc_schemas-0.26.32/cidc_schemas/schemas/templates/assays/ihc_template.json
+-rw-r--r--   0 runner    (1001) docker     (127)     8984 2024-04-29 19:04:27.000000 nci_cidc_schemas-0.26.32/cidc_schemas/schemas/templates/assays/mibi_template.json
+-rw-r--r--   0 runner    (1001) docker     (127)     3578 2024-04-29 19:04:27.000000 nci_cidc_schemas-0.26.32/cidc_schemas/schemas/templates/assays/microbiome_template.json
+-rw-r--r--   0 runner    (1001) docker     (127)    19272 2024-04-29 19:04:27.000000 nci_cidc_schemas-0.26.32/cidc_schemas/schemas/templates/assays/mif_template.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1896 2024-04-29 19:04:27.000000 nci_cidc_schemas-0.26.32/cidc_schemas/schemas/templates/assays/misc_data_template.json
+-rw-r--r--   0 runner    (1001) docker     (127)     3214 2024-04-29 19:04:27.000000 nci_cidc_schemas-0.26.32/cidc_schemas/schemas/templates/assays/nanostring_template.json
+-rw-r--r--   0 runner    (1001) docker     (127)     6335 2024-04-29 19:04:27.000000 nci_cidc_schemas-0.26.32/cidc_schemas/schemas/templates/assays/olink_template.json
+-rw-r--r--   0 runner    (1001) docker     (127)     3084 2024-04-29 19:04:27.000000 nci_cidc_schemas-0.26.32/cidc_schemas/schemas/templates/assays/rna_bam_template.json
+-rw-r--r--   0 runner    (1001) docker     (127)     3344 2024-04-29 19:04:27.000000 nci_cidc_schemas-0.26.32/cidc_schemas/schemas/templates/assays/rna_fastq_template.json
+-rw-r--r--   0 runner    (1001) docker     (127)     3269 2024-04-29 19:04:27.000000 nci_cidc_schemas-0.26.32/cidc_schemas/schemas/templates/assays/tcr_adaptive_template.json
+-rw-r--r--   0 runner    (1001) docker     (127)     3457 2024-04-29 19:04:27.000000 nci_cidc_schemas-0.26.32/cidc_schemas/schemas/templates/assays/tcr_fastq_template.json
+-rw-r--r--   0 runner    (1001) docker     (127)     2724 2024-04-29 19:04:27.000000 nci_cidc_schemas-0.26.32/cidc_schemas/schemas/templates/assays/wes_bam_template.json
+-rw-r--r--   0 runner    (1001) docker     (127)     3143 2024-04-29 19:04:27.000000 nci_cidc_schemas-0.26.32/cidc_schemas/schemas/templates/assays/wes_fastq_template.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 19:04:33.327147 nci_cidc_schemas-0.26.32/cidc_schemas/schemas/templates/manifests/
+-rw-r--r--   0 runner    (1001) docker     (127)    12475 2024-04-29 19:04:27.000000 nci_cidc_schemas-0.26.32/cidc_schemas/schemas/templates/manifests/h_and_e_template.json
+-rw-r--r--   0 runner    (1001) docker     (127)    11829 2024-04-29 19:04:27.000000 nci_cidc_schemas-0.26.32/cidc_schemas/schemas/templates/manifests/microbiome_dna_template.json
+-rw-r--r--   0 runner    (1001) docker     (127)    13346 2024-04-29 19:04:27.000000 nci_cidc_schemas-0.26.32/cidc_schemas/schemas/templates/manifests/normal_blood_dna_template.json
+-rw-r--r--   0 runner    (1001) docker     (127)    12989 2024-04-29 19:04:27.000000 nci_cidc_schemas-0.26.32/cidc_schemas/schemas/templates/manifests/normal_tissue_dna_template.json
+-rw-r--r--   0 runner    (1001) docker     (127)    17530 2024-04-29 19:04:27.000000 nci_cidc_schemas-0.26.32/cidc_schemas/schemas/templates/manifests/pbmc_template.json
+-rw-r--r--   0 runner    (1001) docker     (127)    15099 2024-04-29 19:04:27.000000 nci_cidc_schemas-0.26.32/cidc_schemas/schemas/templates/manifests/plasma_template.json
+-rw-r--r--   0 runner    (1001) docker     (127)    11024 2024-04-29 19:04:27.000000 nci_cidc_schemas-0.26.32/cidc_schemas/schemas/templates/manifests/tissue_slide_template.json
+-rw-r--r--   0 runner    (1001) docker     (127)     2797 2024-04-29 19:04:27.000000 nci_cidc_schemas-0.26.32/cidc_schemas/schemas/templates/manifests/tumor_normal_pairing_template.json
+-rw-r--r--   0 runner    (1001) docker     (127)    13276 2024-04-29 19:04:27.000000 nci_cidc_schemas-0.26.32/cidc_schemas/schemas/templates/manifests/tumor_tissue_dna_template.json
+-rw-r--r--   0 runner    (1001) docker     (127)    12568 2024-04-29 19:04:27.000000 nci_cidc_schemas-0.26.32/cidc_schemas/schemas/templates/manifests/tumor_tissue_rna_template.json
+-rw-r--r--   0 runner    (1001) docker     (127)    49891 2024-04-29 19:04:27.000000 nci_cidc_schemas-0.26.32/cidc_schemas/template.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13119 2024-04-29 19:04:27.000000 nci_cidc_schemas-0.26.32/cidc_schemas/template_reader.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18236 2024-04-29 19:04:27.000000 nci_cidc_schemas-0.26.32/cidc_schemas/template_writer.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13325 2024-04-29 19:04:27.000000 nci_cidc_schemas-0.26.32/cidc_schemas/unprism.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4348 2024-04-29 19:04:27.000000 nci_cidc_schemas-0.26.32/cidc_schemas/util.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 19:04:33.343147 nci_cidc_schemas-0.26.32/nci_cidc_schemas.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     4422 2024-04-29 19:04:33.000000 nci_cidc_schemas-0.26.32/nci_cidc_schemas.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    10838 2024-04-29 19:04:33.000000 nci_cidc_schemas-0.26.32/nci_cidc_schemas.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-29 19:04:33.000000 nci_cidc_schemas-0.26.32/nci_cidc_schemas.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       55 2024-04-29 19:04:33.000000 nci_cidc_schemas-0.26.32/nci_cidc_schemas.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-29 19:04:33.000000 nci_cidc_schemas-0.26.32/nci_cidc_schemas.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)      244 2024-04-29 19:04:33.000000 nci_cidc_schemas-0.26.32/nci_cidc_schemas.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       13 2024-04-29 19:04:33.000000 nci_cidc_schemas-0.26.32/nci_cidc_schemas.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      244 2024-04-29 19:04:27.000000 nci_cidc_schemas-0.26.32/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      395 2024-04-29 19:04:33.343147 nci_cidc_schemas-0.26.32/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1252 2024-04-29 19:04:27.000000 nci_cidc_schemas-0.26.32/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 19:04:33.331147 nci_cidc_schemas-0.26.32/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-29 19:04:27.000000 nci_cidc_schemas-0.26.32/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1905 2024-04-29 19:04:27.000000 nci_cidc_schemas-0.26.32/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (127)      341 2024-04-29 19:04:27.000000 nci_cidc_schemas-0.26.32/tests/constants.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 19:04:33.335147 nci_cidc_schemas-0.26.32/tests/data/
+-rw-r--r--   0 runner    (1001) docker     (127)      223 2024-04-29 19:04:27.000000 nci_cidc_schemas-0.26.32/tests/data/clinical_test_file.1.csv
+-rw-r--r--   0 runner    (1001) docker     (127)    10265 2024-04-29 19:04:27.000000 nci_cidc_schemas-0.26.32/tests/data/clinical_test_file.1.xlsx
+-rw-r--r--   0 runner    (1001) docker     (127)      251 2024-04-29 19:04:27.000000 nci_cidc_schemas-0.26.32/tests/data/clinical_test_file.2.bom.csv
+-rw-r--r--   0 runner    (1001) docker     (127)      248 2024-04-29 19:04:27.000000 nci_cidc_schemas-0.26.32/tests/data/clinical_test_file.2.csv
+-rw-r--r--   0 runner    (1001) docker     (127)     9833 2024-04-29 19:04:27.000000 nci_cidc_schemas-0.26.32/tests/data/clinical_test_file.2.xlsx
+-rw-r--r--   0 runner    (1001) docker     (127)    10204 2024-04-29 19:04:27.000000 nci_cidc_schemas-0.26.32/tests/data/clinical_test_file.3.xlsx
+-rw-r--r--   0 runner    (1001) docker     (127)     4232 2024-04-29 19:04:27.000000 nci_cidc_schemas-0.26.32/tests/data/clinical_test_file.docx
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 19:04:33.335147 nci_cidc_schemas-0.26.32/tests/data/clinicaltrial_examples/
+-rw-r--r--   0 runner    (1001) docker     (127)    19111 2024-04-29 19:04:27.000000 nci_cidc_schemas-0.26.32/tests/data/clinicaltrial_examples/CT_1.json
+-rw-r--r--   0 runner    (1001) docker     (127)    24203 2024-04-29 19:04:27.000000 nci_cidc_schemas-0.26.32/tests/data/clinicaltrial_examples/CT_1PA_multiWES.json
+-rw-r--r--   0 runner    (1001) docker     (127)    14837 2024-04-29 19:04:27.000000 nci_cidc_schemas-0.26.32/tests/data/clinicaltrial_examples/CT_cytof_with_analysis.json
+-rw-r--r--   0 runner    (1001) docker     (127)     6098 2024-04-29 19:04:27.000000 nci_cidc_schemas-0.26.32/tests/data/clinicaltrial_examples/CT_ihc.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1451 2024-04-29 19:04:27.000000 nci_cidc_schemas-0.26.32/tests/data/clinicaltrial_examples/CT_minimal.json
+-rw-r--r--   0 runner    (1001) docker     (127)     5215 2024-04-29 19:04:27.000000 nci_cidc_schemas-0.26.32/tests/data/date_examples.xlsx
+-rw-r--r--   0 runner    (1001) docker     (127)     5954 2024-04-29 19:04:27.000000 nci_cidc_schemas-0.26.32/tests/data/elisa_test_file.1.xlsx
+-rw-r--r--   0 runner    (1001) docker     (127)    12084 2024-04-29 19:04:27.000000 nci_cidc_schemas-0.26.32/tests/data/elisa_test_file.2.xlsx
+-rw-r--r--   0 runner    (1001) docker     (127)    26605 2024-04-29 19:04:27.000000 nci_cidc_schemas-0.26.32/tests/data/hande_err_template.xlsx
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 19:04:33.335147 nci_cidc_schemas-0.26.32/tests/data/olink/
+-rw-r--r--   0 runner    (1001) docker     (127)    13070 2024-04-29 19:04:27.000000 nci_cidc_schemas-0.26.32/tests/data/olink/invalid_olink_assay_1_NPX.xlsx
+-rw-r--r--   0 runner    (1001) docker     (127)    17905 2024-04-29 19:04:27.000000 nci_cidc_schemas-0.26.32/tests/data/olink/olink_assay_1_NPX.xlsx
+-rw-r--r--   0 runner    (1001) docker     (127)    12969 2024-04-29 19:04:27.000000 nci_cidc_schemas-0.26.32/tests/data/olink/olink_assay_2_NPX.xlsx
+-rw-r--r--   0 runner    (1001) docker     (127)    21276 2024-04-29 19:04:27.000000 nci_cidc_schemas-0.26.32/tests/data/olink/olink_assay_combined.xlsx
+-rw-r--r--   0 runner    (1001) docker     (127)    13301 2024-04-29 19:04:27.000000 nci_cidc_schemas-0.26.32/tests/data/pbmc_invalid.xlsx
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 19:04:33.335147 nci_cidc_schemas-0.26.32/tests/data/schemas/
+-rw-r--r--   0 runner    (1001) docker     (127)      144 2024-04-29 19:04:27.000000 nci_cidc_schemas-0.26.32/tests/data/schemas/1.json
+-rw-r--r--   0 runner    (1001) docker     (127)      199 2024-04-29 19:04:27.000000 nci_cidc_schemas-0.26.32/tests/data/schemas/a.json
+-rw-r--r--   0 runner    (1001) docker     (127)      407 2024-04-29 19:04:27.000000 nci_cidc_schemas-0.26.32/tests/data/schemas/b.json
+-rw-r--r--   0 runner    (1001) docker     (127)      189 2024-04-29 19:04:27.000000 nci_cidc_schemas-0.26.32/tests/data/schemas/c.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 19:04:33.335147 nci_cidc_schemas-0.26.32/tests/data/schemas/d1/
+-rw-r--r--   0 runner    (1001) docker     (127)      127 2024-04-29 19:04:27.000000 nci_cidc_schemas-0.26.32/tests/data/schemas/d1/3.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 19:04:33.335147 nci_cidc_schemas-0.26.32/tests/data/schemas/d1/d2/
+-rw-r--r--   0 runner    (1001) docker     (127)      141 2024-04-29 19:04:27.000000 nci_cidc_schemas-0.26.32/tests/data/schemas/d1/d2/2.json
+-rw-r--r--   0 runner    (1001) docker     (127)      149 2024-04-29 19:04:27.000000 nci_cidc_schemas-0.26.32/tests/data/schemas/invalid_ref.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 19:04:33.339147 nci_cidc_schemas-0.26.32/tests/data/schemas/target-templates/
+-rw-r--r--   0 runner    (1001) docker     (127)     5403 2024-04-29 19:04:27.000000 nci_cidc_schemas-0.26.32/tests/data/schemas/target-templates/atacseq_analysis_template.json
+-rw-r--r--   0 runner    (1001) docker     (127)     7231 2024-04-29 19:04:27.000000 nci_cidc_schemas-0.26.32/tests/data/schemas/target-templates/ctdna_analysis_template.json
+-rw-r--r--   0 runner    (1001) docker     (127)    12507 2024-04-29 19:04:27.000000 nci_cidc_schemas-0.26.32/tests/data/schemas/target-templates/rna_level1_analysis_template.json
+-rw-r--r--   0 runner    (1001) docker     (127)    35065 2024-04-29 19:04:27.000000 nci_cidc_schemas-0.26.32/tests/data/schemas/target-templates/wes_analysis_template.json
+-rw-r--r--   0 runner    (1001) docker     (127)    16256 2024-04-29 19:04:27.000000 nci_cidc_schemas-0.26.32/tests/data/schemas/target-templates/wes_tumor_only_analysis_template.json
+-rw-r--r--   0 runner    (1001) docker     (127)     5464 2024-04-29 19:04:27.000000 nci_cidc_schemas-0.26.32/tests/data/tiny_invalid_manifest.xlsx
+-rw-r--r--   0 runner    (1001) docker     (127)     5455 2024-04-29 19:04:27.000000 nci_cidc_schemas-0.26.32/tests/data/tiny_valid_manifest.xlsx
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 19:04:33.339147 nci_cidc_schemas-0.26.32/tests/prism/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-29 19:04:27.000000 nci_cidc_schemas-0.26.32/tests/prism/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 19:04:33.343147 nci_cidc_schemas-0.26.32/tests/prism/cidc_test_data/
+-rw-r--r--   0 runner    (1001) docker     (127)      409 2024-04-29 19:04:27.000000 nci_cidc_schemas-0.26.32/tests/prism/cidc_test_data/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)   146616 2024-04-29 19:04:27.000000 nci_cidc_schemas-0.26.32/tests/prism/cidc_test_data/analysis_data.py
+-rw-r--r--   0 runner    (1001) docker     (127)   167922 2024-04-29 19:04:27.000000 nci_cidc_schemas-0.26.32/tests/prism/cidc_test_data/assay_data.py
+-rw-r--r--   0 runner    (1001) docker     (127)   104350 2024-04-29 19:04:27.000000 nci_cidc_schemas-0.26.32/tests/prism/cidc_test_data/manifest_data.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3035 2024-04-29 19:04:27.000000 nci_cidc_schemas-0.26.32/tests/prism/cidc_test_data/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 19:04:33.343147 nci_cidc_schemas-0.26.32/tests/prism/schema/
+-rw-r--r--   0 runner    (1001) docker     (127)     2676 2024-04-29 19:04:27.000000 nci_cidc_schemas-0.26.32/tests/prism/schema/test_schema.json
+-rw-r--r--   0 runner    (1001) docker     (127)     7119 2024-04-29 19:04:27.000000 nci_cidc_schemas-0.26.32/tests/prism/test_cidc_data_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)      410 2024-04-29 19:04:27.000000 nci_cidc_schemas-0.26.32/tests/prism/test_constants.py
+-rw-r--r--   0 runner    (1001) docker     (127)    31916 2024-04-29 19:04:27.000000 nci_cidc_schemas-0.26.32/tests/prism/test_core.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5574 2024-04-29 19:04:27.000000 nci_cidc_schemas-0.26.32/tests/prism/test_extra_metadata.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13867 2024-04-29 19:04:27.000000 nci_cidc_schemas-0.26.32/tests/prism/test_merger.py
+-rw-r--r--   0 runner    (1001) docker     (127)    29150 2024-04-29 19:04:27.000000 nci_cidc_schemas-0.26.32/tests/prism/test_pipelines.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4467 2024-04-29 19:04:27.000000 nci_cidc_schemas-0.26.32/tests/test_artifacts.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17706 2024-04-29 19:04:27.000000 nci_cidc_schemas-0.26.32/tests/test_assays.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1443 2024-04-29 19:04:27.000000 nci_cidc_schemas-0.26.32/tests/test_clinicaltrial_examples.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14541 2024-04-29 19:04:27.000000 nci_cidc_schemas-0.26.32/tests/test_json_validation.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15991 2024-04-29 19:04:27.000000 nci_cidc_schemas-0.26.32/tests/test_migrations.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1389 2024-04-29 19:04:27.000000 nci_cidc_schemas-0.26.32/tests/test_schemas.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2925 2024-04-29 19:04:27.000000 nci_cidc_schemas-0.26.32/tests/test_strict_meta_schema.py
+-rw-r--r--   0 runner    (1001) docker     (127)    26123 2024-04-29 19:04:27.000000 nci_cidc_schemas-0.26.32/tests/test_template.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7390 2024-04-29 19:04:27.000000 nci_cidc_schemas-0.26.32/tests/test_template_reader.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2162 2024-04-29 19:04:27.000000 nci_cidc_schemas-0.26.32/tests/test_template_writer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4473 2024-04-29 19:04:27.000000 nci_cidc_schemas-0.26.32/tests/test_templates.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4001 2024-04-29 19:04:27.000000 nci_cidc_schemas-0.26.32/tests/test_trial_core.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10653 2024-04-29 19:04:27.000000 nci_cidc_schemas-0.26.32/tests/test_unprism.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3294 2024-04-29 19:04:27.000000 nci_cidc_schemas-0.26.32/tests/test_util.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 19:04:33.343147 nci_cidc_schemas-0.26.32/tests/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)     2793 2024-04-29 19:04:27.000000 nci_cidc_schemas-0.26.32/tests/utils/test_template_generator.py
```

### Comparing `nci_cidc_schemas-0.26.29/LICENSE` & `nci_cidc_schemas-0.26.32/LICENSE`

 * *Files identical despite different names*

### Comparing `nci_cidc_schemas-0.26.29/PKG-INFO` & `nci_cidc_schemas-0.26.32/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nci_cidc_schemas
-Version: 0.26.29
+Version: 0.26.32
 Summary: The CIDC data model and tools for working with it.
 Home-page: https://github.com/NCI-CIDC/cidc-schemas
 Author: NCI
 Author-email: nci-cidc-tools-admin@mail.nih.gov
 License: MIT license
 Keywords: cidc_schemas
 Classifier: Development Status :: 2 - Pre-Alpha
```

### Comparing `nci_cidc_schemas-0.26.29/README.md` & `nci_cidc_schemas-0.26.32/README.md`

 * *Files identical despite different names*

### Comparing `nci_cidc_schemas-0.26.29/cidc_schemas/cli.py` & `nci_cidc_schemas-0.26.32/cidc_schemas/cli.py`

 * *Files identical despite different names*

### Comparing `nci_cidc_schemas-0.26.29/cidc_schemas/constants.py` & `nci_cidc_schemas-0.26.32/cidc_schemas/constants.py`

 * *Files identical despite different names*

### Comparing `nci_cidc_schemas-0.26.29/cidc_schemas/json_validation.py` & `nci_cidc_schemas-0.26.32/cidc_schemas/json_validation.py`

 * *Files 1% similar despite different names*

```diff
@@ -106,18 +106,18 @@
             if "matched_paths" in search:
                 for path in search["matched_paths"]:
                     scope = {"root": self.schema}
                     exec(f"ref_path_pattern = {path}", scope)
                     ref_path_pattern = scope["ref_path_pattern"]
                     # If there are no cached values for this ref path pattern, collect them
                     if ref_path_pattern not in self._in_doc_refs_cache:
-                        self._in_doc_refs_cache[
-                            ref_path_pattern
-                        ] = self._get_values_for_path_pattern(
-                            ref_path_pattern, instance
+                        self._in_doc_refs_cache[ref_path_pattern] = (
+                            self._get_values_for_path_pattern(
+                                ref_path_pattern, instance
+                            )
                         )
 
         # see: https://docs.python.org/3/library/contextlib.html
         try:
             yield
         finally:
             self._in_doc_refs_cache = None
```

### Comparing `nci_cidc_schemas-0.26.29/cidc_schemas/metaschema/strict_meta_schema.json` & `nci_cidc_schemas-0.26.32/cidc_schemas/metaschema/strict_meta_schema.json`

 * *Files identical despite different names*

### Comparing `nci_cidc_schemas-0.26.29/cidc_schemas/migrations.py` & `nci_cidc_schemas-0.26.32/cidc_schemas/migrations.py`

 * *Files identical despite different names*

### Comparing `nci_cidc_schemas-0.26.29/cidc_schemas/pipeline_configs/rna_level1_analysis_config.yaml.j2` & `nci_cidc_schemas-0.26.32/cidc_schemas/pipeline_configs/rna_level1_analysis_config.yaml.j2`

 * *Files identical despite different names*

### Comparing `nci_cidc_schemas-0.26.29/cidc_schemas/prism/__init__.py` & `nci_cidc_schemas-0.26.32/cidc_schemas/prism/__init__.py`

 * *Files identical despite different names*

### Comparing `nci_cidc_schemas-0.26.29/cidc_schemas/prism/constants.py` & `nci_cidc_schemas-0.26.32/cidc_schemas/prism/constants.py`

 * *Files 2% similar despite different names*

```diff
@@ -47,25 +47,27 @@
 SUPPORTED_ANALYSES = [
     "atacseq_analysis",
     "cytof_analysis",
     "rna_level1_analysis",
     "tcr_analysis",
     "wes_analysis",
     "wes_tumor_only_analysis",
+    "ctdna_analysis",
 ]
 
 SUPPORTED_TEMPLATES = SUPPORTED_ASSAYS + SUPPORTED_MANIFESTS + SUPPORTED_ANALYSES
 
 # provide a way to get file-path prefix for each upload_type
 ASSAY_TO_FILEPATH: Dict[str, str] = {
     # analysis is removed on some
     "atacseq_analysis": "atacseq/",
     "rna_level1_analysis": "rna/",
     "wes_analysis": "wes/",
     "wes_tumor_only_analysis": "wes_tumor_only/",
+    "ctdna_analysis": "ctdna/",
     # assay specifics removed
     "atacseq_fastq": "atacseq/",
     "rna_bam": "rna/",
     "rna_fastq": "rna/",
     "tcr_adaptive": "tcr/",
     "tcr_fastq": "tcr/",
     "wes_bam": "wes/",
```

### Comparing `nci_cidc_schemas-0.26.29/cidc_schemas/prism/core.py` & `nci_cidc_schemas-0.26.32/cidc_schemas/prism/core.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """Build metadata dictionaries from Excel files."""
+
 import logging
 import base64
 import hmac
 from typing import List, Tuple, Union
 
 from cidc_schemas.json_validation import load_and_validate_schema
 from cidc_schemas.template import (
```

### Comparing `nci_cidc_schemas-0.26.29/cidc_schemas/prism/extra_metadata.py` & `nci_cidc_schemas-0.26.32/cidc_schemas/prism/extra_metadata.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """Parsers for extracting extra metadata from files containing molecular data."""
+
 import logging
 import re
 from codecs import BOM_UTF8
 from typing import BinaryIO
 
 import openpyxl
 import pandas as pd
```

### Comparing `nci_cidc_schemas-0.26.29/cidc_schemas/prism/merger.py` & `nci_cidc_schemas-0.26.32/cidc_schemas/prism/merger.py`

 * *Files identical despite different names*

### Comparing `nci_cidc_schemas-0.26.29/cidc_schemas/prism/pipelines.py` & `nci_cidc_schemas-0.26.32/cidc_schemas/prism/pipelines.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """Analysis pipeline configuration generators."""
+
 from collections import defaultdict
 from datetime import datetime
 from io import BytesIO
 import logging
 from tempfile import NamedTemporaryFile
 from typing import Dict, List, NamedTuple, Union
 
@@ -11,14 +12,15 @@
 
 from .constants import PROTOCOL_ID_FIELD_NAME, SUPPORTED_SHIPPING_MANIFESTS
 from ..template import Template
 from ..util import load_pipeline_config_template, participant_id_from_cimac
 
 logger = logging.getLogger(__file__)
 
+
 # Note, bucket names must be all lowercase, dash, and underscore
 # https://cloud.google.com/storage/docs/naming-buckets#requirements
 def RNA_GOOGLE_BUCKET_PATH_FN(trial_id: str, batch_num: int) -> str:
     return f"gs://repro_{trial_id.lower()}/RNA/set{batch_num+1}"
 
 
 def RNA_INSTANCE_NAME_FN(trial_id: str, batch_num: int) -> str:
```

### Comparing `nci_cidc_schemas-0.26.29/cidc_schemas/schemas/aliquot.json` & `nci_cidc_schemas-0.26.32/cidc_schemas/schemas/aliquot.json`

 * *Files identical despite different names*

### Comparing `nci_cidc_schemas-0.26.29/cidc_schemas/schemas/artifacts/artifact_bam.json` & `nci_cidc_schemas-0.26.32/cidc_schemas/schemas/artifacts/artifact_bam.json`

 * *Files identical despite different names*

### Comparing `nci_cidc_schemas-0.26.29/cidc_schemas/schemas/artifacts/artifact_bam_bai.json` & `nci_cidc_schemas-0.26.32/cidc_schemas/schemas/artifacts/artifact_bam_bai.json`

 * *Files identical despite different names*

### Comparing `nci_cidc_schemas-0.26.29/cidc_schemas/schemas/artifacts/artifact_bed.json` & `nci_cidc_schemas-0.26.32/cidc_schemas/schemas/artifacts/artifact_bed.json`

 * *Files identical despite different names*

### Comparing `nci_cidc_schemas-0.26.29/cidc_schemas/schemas/artifacts/artifact_bigwig.json` & `nci_cidc_schemas-0.26.32/cidc_schemas/schemas/artifacts/artifact_bigwig.json`

 * *Files identical despite different names*

### Comparing `nci_cidc_schemas-0.26.29/cidc_schemas/schemas/artifacts/artifact_binary.json` & `nci_cidc_schemas-0.26.32/cidc_schemas/schemas/artifacts/artifact_binary.json`

 * *Files identical despite different names*

### Comparing `nci_cidc_schemas-0.26.29/cidc_schemas/schemas/artifacts/artifact_clinical_csv.json` & `nci_cidc_schemas-0.26.32/cidc_schemas/schemas/artifacts/artifact_clinical_csv.json`

 * *Files identical despite different names*

### Comparing `nci_cidc_schemas-0.26.29/cidc_schemas/schemas/artifacts/artifact_clinical_docx.json` & `nci_cidc_schemas-0.26.32/cidc_schemas/schemas/artifacts/artifact_clinical_docx.json`

 * *Files identical despite different names*

### Comparing `nci_cidc_schemas-0.26.29/cidc_schemas/schemas/artifacts/artifact_clinical_xlsx.json` & `nci_cidc_schemas-0.26.32/cidc_schemas/schemas/artifacts/artifact_clinical_xlsx.json`

 * *Files identical despite different names*

### Comparing `nci_cidc_schemas-0.26.29/cidc_schemas/schemas/artifacts/artifact_cncf.json` & `nci_cidc_schemas-0.26.32/cidc_schemas/schemas/artifacts/artifact_cncf.json`

 * *Files identical despite different names*

### Comparing `nci_cidc_schemas-0.26.29/cidc_schemas/schemas/artifacts/artifact_cns.json` & `nci_cidc_schemas-0.26.32/cidc_schemas/schemas/artifacts/artifact_cns.json`

 * *Files identical despite different names*

### Comparing `nci_cidc_schemas-0.26.29/cidc_schemas/schemas/artifacts/artifact_core.json` & `nci_cidc_schemas-0.26.32/cidc_schemas/schemas/artifacts/artifact_core.json`

 * *Files 1% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9999844990079365%*

 * *Differences: {"'properties'": "{'data_format': {'enum': {insert: [(22, 'RDATA')]}}}"}*

```diff
@@ -73,14 +73,15 @@
                 "ZIP",
                 "FCS",
                 "GZ",
                 "RCC",
                 "JSON",
                 "YAML",
                 "PDF",
+                "RDATA",
                 "[NOT SET]"
             ],
             "type": "string"
         },
         "facet_group": {
             "description": "The internal data category for this artifact",
             "type": "string"
```

### Comparing `nci_cidc_schemas-0.26.29/cidc_schemas/schemas/artifacts/artifact_csv.json` & `nci_cidc_schemas-0.26.32/cidc_schemas/schemas/artifacts/artifact_csv.json`

 * *Files identical despite different names*

### Comparing `nci_cidc_schemas-0.26.29/cidc_schemas/schemas/artifacts/artifact_elisa_xlsx.json` & `nci_cidc_schemas-0.26.32/cidc_schemas/schemas/artifacts/artifact_elisa_xlsx.json`

 * *Files identical despite different names*

### Comparing `nci_cidc_schemas-0.26.29/cidc_schemas/schemas/artifacts/artifact_fastq_gz.json` & `nci_cidc_schemas-0.26.32/cidc_schemas/schemas/artifacts/artifact_fastq_gz.json`

 * *Files identical despite different names*

### Comparing `nci_cidc_schemas-0.26.29/cidc_schemas/schemas/artifacts/artifact_fcs.json` & `nci_cidc_schemas-0.26.32/cidc_schemas/schemas/artifacts/artifact_fcs.json`

 * *Files identical despite different names*

### Comparing `nci_cidc_schemas-0.26.29/cidc_schemas/schemas/artifacts/artifact_file.json` & `nci_cidc_schemas-0.26.32/cidc_schemas/schemas/artifacts/artifact_file.json`

 * *Files identical despite different names*

### Comparing `nci_cidc_schemas-0.26.29/cidc_schemas/schemas/artifacts/artifact_gz.json` & `nci_cidc_schemas-0.26.32/cidc_schemas/schemas/artifacts/artifact_gz.json`

 * *Files identical despite different names*

### Comparing `nci_cidc_schemas-0.26.29/cidc_schemas/schemas/artifacts/artifact_image.json` & `nci_cidc_schemas-0.26.32/cidc_schemas/schemas/artifacts/artifact_image.json`

 * *Files identical despite different names*

### Comparing `nci_cidc_schemas-0.26.29/cidc_schemas/schemas/artifacts/artifact_jpg.json` & `nci_cidc_schemas-0.26.32/cidc_schemas/schemas/artifacts/artifact_jpg.json`

 * *Files identical despite different names*

### Comparing `nci_cidc_schemas-0.26.29/cidc_schemas/schemas/artifacts/artifact_json.json` & `nci_cidc_schemas-0.26.32/cidc_schemas/schemas/artifacts/artifact_json.json`

 * *Files identical despite different names*

### Comparing `nci_cidc_schemas-0.26.29/cidc_schemas/schemas/artifacts/artifact_junction.json` & `nci_cidc_schemas-0.26.32/cidc_schemas/schemas/artifacts/artifact_junction.json`

 * *Files identical despite different names*

### Comparing `nci_cidc_schemas-0.26.29/cidc_schemas/schemas/artifacts/artifact_log.json` & `nci_cidc_schemas-0.26.32/cidc_schemas/schemas/artifacts/artifact_log.json`

 * *Files identical despite different names*

### Comparing `nci_cidc_schemas-0.26.29/cidc_schemas/schemas/artifacts/artifact_maf.json` & `nci_cidc_schemas-0.26.32/cidc_schemas/schemas/artifacts/artifact_maf.json`

 * *Files identical despite different names*

### Comparing `nci_cidc_schemas-0.26.29/cidc_schemas/schemas/artifacts/artifact_narrowPeak.json` & `nci_cidc_schemas-0.26.32/cidc_schemas/schemas/artifacts/artifact_narrowPeak.json`

 * *Files identical despite different names*

### Comparing `nci_cidc_schemas-0.26.29/cidc_schemas/schemas/artifacts/artifact_npx.json` & `nci_cidc_schemas-0.26.32/cidc_schemas/schemas/artifacts/artifact_npx.json`

 * *Files identical despite different names*

### Comparing `nci_cidc_schemas-0.26.29/cidc_schemas/schemas/artifacts/artifact_pdf.json` & `nci_cidc_schemas-0.26.32/cidc_schemas/schemas/artifacts/artifact_pdf.json`

 * *Files identical despite different names*

### Comparing `nci_cidc_schemas-0.26.29/cidc_schemas/schemas/artifacts/artifact_png.json` & `nci_cidc_schemas-0.26.32/cidc_schemas/schemas/artifacts/artifact_png.json`

 * *Files identical despite different names*

### Comparing `nci_cidc_schemas-0.26.29/cidc_schemas/schemas/artifacts/artifact_rcc.json` & `nci_cidc_schemas-0.26.32/cidc_schemas/schemas/artifacts/artifact_rcc.json`

 * *Files identical despite different names*

### Comparing `nci_cidc_schemas-0.26.29/cidc_schemas/schemas/artifacts/artifact_tbi.json` & `nci_cidc_schemas-0.26.32/cidc_schemas/schemas/artifacts/artifact_tbi.json`

 * *Files identical despite different names*

### Comparing `nci_cidc_schemas-0.26.29/cidc_schemas/schemas/artifacts/artifact_text.json` & `nci_cidc_schemas-0.26.32/cidc_schemas/schemas/artifacts/artifact_text.json`

 * *Files identical despite different names*

### Comparing `nci_cidc_schemas-0.26.29/cidc_schemas/schemas/artifacts/artifact_tsv.json` & `nci_cidc_schemas-0.26.32/cidc_schemas/schemas/artifacts/artifact_tsv.json`

 * *Files identical despite different names*

### Comparing `nci_cidc_schemas-0.26.29/cidc_schemas/schemas/artifacts/artifact_vcf.json` & `nci_cidc_schemas-0.26.32/cidc_schemas/schemas/artifacts/artifact_vcf.json`

 * *Files identical despite different names*

### Comparing `nci_cidc_schemas-0.26.29/cidc_schemas/schemas/artifacts/artifact_vcf_gz.json` & `nci_cidc_schemas-0.26.32/cidc_schemas/schemas/artifacts/artifact_vcf_gz.json`

 * *Files identical despite different names*

### Comparing `nci_cidc_schemas-0.26.29/cidc_schemas/schemas/artifacts/artifact_xlsx.json` & `nci_cidc_schemas-0.26.32/cidc_schemas/schemas/artifacts/artifact_xlsx.json`

 * *Files identical despite different names*

### Comparing `nci_cidc_schemas-0.26.29/cidc_schemas/schemas/artifacts/artifact_yaml.json` & `nci_cidc_schemas-0.26.32/cidc_schemas/schemas/artifacts/artifact_yaml.json`

 * *Files identical despite different names*

### Comparing `nci_cidc_schemas-0.26.29/cidc_schemas/schemas/artifacts/artifact_zip.json` & `nci_cidc_schemas-0.26.32/cidc_schemas/schemas/artifacts/artifact_zip.json`

 * *Files identical despite different names*

### Comparing `nci_cidc_schemas-0.26.29/cidc_schemas/schemas/assays/atacseq_assay.json` & `nci_cidc_schemas-0.26.32/cidc_schemas/schemas/assays/atacseq_assay.json`

 * *Files identical despite different names*

### Comparing `nci_cidc_schemas-0.26.29/cidc_schemas/schemas/assays/components/antibody.json` & `nci_cidc_schemas-0.26.32/cidc_schemas/schemas/assays/components/antibody.json`

 * *Files identical despite different names*

### Comparing `nci_cidc_schemas-0.26.29/cidc_schemas/schemas/assays/components/available_assays.json` & `nci_cidc_schemas-0.26.32/cidc_schemas/schemas/assays/components/available_assays.json`

 * *Files identical despite different names*

### Comparing `nci_cidc_schemas-0.26.29/cidc_schemas/schemas/assays/components/available_ngs_analyses.json` & `nci_cidc_schemas-0.26.32/cidc_schemas/schemas/assays/components/available_ngs_analyses.json`

 * *Files 17% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9921875%*

 * *Differences: {"'properties'": "{'ctdna_analysis': OrderedDict([('$ref', 'assays/ctdna_analysis.json')])}"}*

```diff
@@ -12,14 +12,17 @@
             },
             "mergeOptions": {
                 "idRef": "batch_id"
             },
             "mergeStrategy": "arrayMergeById",
             "type": "array"
         },
+        "ctdna_analysis": {
+            "$ref": "assays/ctdna_analysis.json"
+        },
         "rna_analysis": {
             "$ref": "assays/components/ngs/rna/rna_analysis.json"
         },
         "tcr_analysis": {
             "$ref": "assays/tcr_analysis.json"
         },
         "wes_analysis": {
```

### Comparing `nci_cidc_schemas-0.26.29/cidc_schemas/schemas/assays/components/composite_image.json` & `nci_cidc_schemas-0.26.32/cidc_schemas/schemas/assays/components/composite_image.json`

 * *Files identical despite different names*

### Comparing `nci_cidc_schemas-0.26.29/cidc_schemas/schemas/assays/components/enrichment_core.json` & `nci_cidc_schemas-0.26.32/cidc_schemas/schemas/assays/components/enrichment_core.json`

 * *Files identical despite different names*

### Comparing `nci_cidc_schemas-0.26.29/cidc_schemas/schemas/assays/components/excluded_samples.json` & `nci_cidc_schemas-0.26.32/cidc_schemas/schemas/assays/components/excluded_samples.json`

 * *Files identical despite different names*

### Comparing `nci_cidc_schemas-0.26.29/cidc_schemas/schemas/assays/components/image.json` & `nci_cidc_schemas-0.26.32/cidc_schemas/schemas/assays/components/image.json`

 * *Files identical despite different names*

### Comparing `nci_cidc_schemas-0.26.29/cidc_schemas/schemas/assays/components/imaging/mif_entry.json` & `nci_cidc_schemas-0.26.32/cidc_schemas/schemas/assays/components/imaging/mif_entry.json`

 * *Files identical despite different names*

### Comparing `nci_cidc_schemas-0.26.29/cidc_schemas/schemas/assays/components/imaging/mif_export.json` & `nci_cidc_schemas-0.26.32/cidc_schemas/schemas/assays/components/imaging/mif_export.json`

 * *Files identical despite different names*

### Comparing `nci_cidc_schemas-0.26.29/cidc_schemas/schemas/assays/components/imaging/mif_input.json` & `nci_cidc_schemas-0.26.32/cidc_schemas/schemas/assays/components/imaging/mif_input.json`

 * *Files identical despite different names*

### Comparing `nci_cidc_schemas-0.26.29/cidc_schemas/schemas/assays/components/imaging/mif_roi.json` & `nci_cidc_schemas-0.26.32/cidc_schemas/schemas/assays/components/imaging/mif_roi.json`

 * *Files identical despite different names*

### Comparing `nci_cidc_schemas-0.26.29/cidc_schemas/schemas/assays/components/imaging_data.json` & `nci_cidc_schemas-0.26.32/cidc_schemas/schemas/assays/components/imaging_data.json`

 * *Files identical despite different names*

### Comparing `nci_cidc_schemas-0.26.29/cidc_schemas/schemas/assays/components/mapping.json` & `nci_cidc_schemas-0.26.32/cidc_schemas/schemas/assays/components/mapping.json`

 * *Files identical despite different names*

### Comparing `nci_cidc_schemas-0.26.29/cidc_schemas/schemas/assays/components/mibi_antibody.json` & `nci_cidc_schemas-0.26.32/cidc_schemas/schemas/assays/components/mibi_antibody.json`

 * *Files identical despite different names*

### Comparing `nci_cidc_schemas-0.26.29/cidc_schemas/schemas/assays/components/mif_antibody.json` & `nci_cidc_schemas-0.26.32/cidc_schemas/schemas/assays/components/mif_antibody.json`

 * *Files identical despite different names*

### Comparing `nci_cidc_schemas-0.26.29/cidc_schemas/schemas/assays/components/ngs/atacseq/atacseq_analysis.json` & `nci_cidc_schemas-0.26.32/cidc_schemas/schemas/assays/components/ngs/atacseq/atacseq_analysis.json`

 * *Files identical despite different names*

### Comparing `nci_cidc_schemas-0.26.29/cidc_schemas/schemas/assays/components/ngs/ngs_assay_record.json` & `nci_cidc_schemas-0.26.32/cidc_schemas/schemas/assays/components/ngs/ngs_assay_record.json`

 * *Files identical despite different names*

### Comparing `nci_cidc_schemas-0.26.29/cidc_schemas/schemas/assays/components/ngs/rna/rna_analysis.json` & `nci_cidc_schemas-0.26.32/cidc_schemas/schemas/assays/components/ngs/rna/rna_analysis.json`

 * *Files identical despite different names*

### Comparing `nci_cidc_schemas-0.26.29/cidc_schemas/schemas/assays/components/ngs/rna/rna_level1_analysis.json` & `nci_cidc_schemas-0.26.32/cidc_schemas/schemas/assays/components/ngs/rna/rna_level1_analysis.json`

 * *Files identical despite different names*

### Comparing `nci_cidc_schemas-0.26.29/cidc_schemas/schemas/assays/components/ngs/rna/rseqc.json` & `nci_cidc_schemas-0.26.32/cidc_schemas/schemas/assays/components/ngs/rna/rseqc.json`

 * *Files identical despite different names*

### Comparing `nci_cidc_schemas-0.26.29/cidc_schemas/schemas/assays/components/ngs/rna/salmon.json` & `nci_cidc_schemas-0.26.32/cidc_schemas/schemas/assays/components/ngs/rna/salmon.json`

 * *Files identical despite different names*

### Comparing `nci_cidc_schemas-0.26.29/cidc_schemas/schemas/assays/components/ngs/rna/star.json` & `nci_cidc_schemas-0.26.32/cidc_schemas/schemas/assays/components/ngs/rna/star.json`

 * *Files identical despite different names*

### Comparing `nci_cidc_schemas-0.26.29/cidc_schemas/schemas/assays/components/ngs_assay_core.json` & `nci_cidc_schemas-0.26.32/cidc_schemas/schemas/assays/components/ngs_assay_core.json`

 * *Files identical despite different names*

### Comparing `nci_cidc_schemas-0.26.29/cidc_schemas/schemas/assays/components/ngs_assay_record.json` & `nci_cidc_schemas-0.26.32/cidc_schemas/schemas/assays/components/ngs_assay_record.json`

 * *Files identical despite different names*

### Comparing `nci_cidc_schemas-0.26.29/cidc_schemas/schemas/assays/components/reads_core.json` & `nci_cidc_schemas-0.26.32/cidc_schemas/schemas/assays/components/reads_core.json`

 * *Files identical despite different names*

### Comparing `nci_cidc_schemas-0.26.29/cidc_schemas/schemas/assays/components/reads_with_index.json` & `nci_cidc_schemas-0.26.32/cidc_schemas/schemas/assays/components/reads_with_index.json`

 * *Files identical despite different names*

### Comparing `nci_cidc_schemas-0.26.29/cidc_schemas/schemas/assays/ctdna_assay.json` & `nci_cidc_schemas-0.26.32/cidc_schemas/schemas/assays/ctdna_assay.json`

 * *Files 6% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9996936274509803%*

 * *Differences: {"'definitions'": "{'entry': {'properties': {'on_premise_corrected_depth_file': "*

 * *                  "OrderedDict([('$ref', 'artifacts/artifact_text.json')]), "*

 * *                  "'on_premise_parameters_file': OrderedDict([('$ref', "*

 * *                  "'artifacts/artifact_text.json')]), 'on_premise_rdata_file': "*

 * *                  "OrderedDict([('$ref', 'artifacts/artifact_rdata.json')])}}}"}*

```diff
@@ -45,14 +45,23 @@
                 "gc_map_correction_mad": {
                     "description": "Measure of the noise in the data following GC-content bias correction. Computed as the median absolute deviation of differences between adjacent bins.",
                     "type": "number"
                 },
                 "genome-wide_plots": {
                     "$ref": "artifacts/artifact_pdf.json"
                 },
+                "on_premise_corrected_depth_file": {
+                    "$ref": "artifacts/artifact_text.json"
+                },
+                "on_premise_parameters_file": {
+                    "$ref": "artifacts/artifact_text.json"
+                },
+                "on_premise_rdata_file": {
+                    "$ref": "artifacts/artifact_rdata.json"
+                },
                 "optimal_solution": {
                     "$ref": "artifacts/artifact_zip.json"
                 },
                 "other_solutions": {
                     "$ref": "artifacts/artifact_zip.json"
                 },
                 "subclone_fraction": {
```

### Comparing `nci_cidc_schemas-0.26.29/cidc_schemas/schemas/assays/cytof_assay.json` & `nci_cidc_schemas-0.26.32/cidc_schemas/schemas/assays/cytof_assay.json`

 * *Files identical despite different names*

### Comparing `nci_cidc_schemas-0.26.29/cidc_schemas/schemas/assays/cytof_assay_core.json` & `nci_cidc_schemas-0.26.32/cidc_schemas/schemas/assays/cytof_assay_core.json`

 * *Files identical despite different names*

### Comparing `nci_cidc_schemas-0.26.29/cidc_schemas/schemas/assays/elisa_assay.json` & `nci_cidc_schemas-0.26.32/cidc_schemas/schemas/assays/elisa_assay.json`

 * *Files identical despite different names*

### Comparing `nci_cidc_schemas-0.26.29/cidc_schemas/schemas/assays/hande_assay.json` & `nci_cidc_schemas-0.26.32/cidc_schemas/schemas/assays/hande_assay.json`

 * *Files identical despite different names*

### Comparing `nci_cidc_schemas-0.26.29/cidc_schemas/schemas/assays/ihc_assay.json` & `nci_cidc_schemas-0.26.32/cidc_schemas/schemas/assays/ihc_assay.json`

 * *Files 1% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9998553240740741%*

 * *Differences: {"'properties'": "{'slide_scanner_model': {'enum': {insert: [(3, 'Akoya PhenoImager HT')]}}}"}*

```diff
@@ -213,15 +213,16 @@
             "type": "array"
         },
         "slide_scanner_model": {
             "description": "Model version of the slide scanner instrument.",
             "enum": [
                 "Vectra 2.0",
                 "Hamamatsu",
-                "AT2 Turbo"
+                "AT2 Turbo",
+                "Akoya PhenoImager HT"
             ],
             "type": "string"
         },
         "staining_platform": {
             "description": "Staining platform used for tissue sample labeling.",
             "enum": [
                 "auto",
```

### Comparing `nci_cidc_schemas-0.26.29/cidc_schemas/schemas/assays/mibi_assay.json` & `nci_cidc_schemas-0.26.32/cidc_schemas/schemas/assays/mibi_assay.json`

 * *Files identical despite different names*

### Comparing `nci_cidc_schemas-0.26.29/cidc_schemas/schemas/assays/microbiome_assay.json` & `nci_cidc_schemas-0.26.32/cidc_schemas/schemas/assays/microbiome_assay.json`

 * *Files identical despite different names*

### Comparing `nci_cidc_schemas-0.26.29/cidc_schemas/schemas/assays/mif_assay.json` & `nci_cidc_schemas-0.26.32/cidc_schemas/schemas/assays/mif_assay.json`

 * *Files identical despite different names*

### Comparing `nci_cidc_schemas-0.26.29/cidc_schemas/schemas/assays/misc_data.json` & `nci_cidc_schemas-0.26.32/cidc_schemas/schemas/assays/misc_data.json`

 * *Files identical despite different names*

### Comparing `nci_cidc_schemas-0.26.29/cidc_schemas/schemas/assays/nanostring_assay.json` & `nci_cidc_schemas-0.26.32/cidc_schemas/schemas/assays/nanostring_assay.json`

 * *Files identical despite different names*

### Comparing `nci_cidc_schemas-0.26.29/cidc_schemas/schemas/assays/olink_assay.json` & `nci_cidc_schemas-0.26.32/cidc_schemas/schemas/assays/olink_assay.json`

 * *Files identical despite different names*

### Comparing `nci_cidc_schemas-0.26.29/cidc_schemas/schemas/assays/rna_assay-v0.json` & `nci_cidc_schemas-0.26.32/cidc_schemas/schemas/assays/rna_assay-v0.json`

 * *Files identical despite different names*

### Comparing `nci_cidc_schemas-0.26.29/cidc_schemas/schemas/assays/tcr_analysis.json` & `nci_cidc_schemas-0.26.32/cidc_schemas/schemas/assays/tcr_analysis.json`

 * *Files identical despite different names*

### Comparing `nci_cidc_schemas-0.26.29/cidc_schemas/schemas/assays/tcr_assay.json` & `nci_cidc_schemas-0.26.32/cidc_schemas/schemas/assays/tcr_assay.json`

 * *Files identical despite different names*

### Comparing `nci_cidc_schemas-0.26.29/cidc_schemas/schemas/assays/wes_analysis.json` & `nci_cidc_schemas-0.26.32/cidc_schemas/schemas/assays/wes_analysis.json`

 * *Files identical despite different names*

### Comparing `nci_cidc_schemas-0.26.29/cidc_schemas/schemas/assays/wes_assay.json` & `nci_cidc_schemas-0.26.32/cidc_schemas/schemas/assays/wes_assay.json`

 * *Files identical despite different names*

### Comparing `nci_cidc_schemas-0.26.29/cidc_schemas/schemas/assays/wes_core.json` & `nci_cidc_schemas-0.26.32/cidc_schemas/schemas/assays/wes_core.json`

 * *Files identical despite different names*

### Comparing `nci_cidc_schemas-0.26.29/cidc_schemas/schemas/assays/wes_tumor_only_analysis.json` & `nci_cidc_schemas-0.26.32/cidc_schemas/schemas/assays/wes_tumor_only_analysis.json`

 * *Files identical despite different names*

### Comparing `nci_cidc_schemas-0.26.29/cidc_schemas/schemas/clinical_data.json` & `nci_cidc_schemas-0.26.32/cidc_schemas/schemas/clinical_data.json`

 * *Files identical despite different names*

### Comparing `nci_cidc_schemas-0.26.29/cidc_schemas/schemas/clinical_trial.json` & `nci_cidc_schemas-0.26.32/cidc_schemas/schemas/clinical_trial.json`

 * *Files identical despite different names*

### Comparing `nci_cidc_schemas-0.26.29/cidc_schemas/schemas/participant.json` & `nci_cidc_schemas-0.26.32/cidc_schemas/schemas/participant.json`

 * *Files identical despite different names*

### Comparing `nci_cidc_schemas-0.26.29/cidc_schemas/schemas/sample.json` & `nci_cidc_schemas-0.26.32/cidc_schemas/schemas/sample.json`

 * *Files identical despite different names*

### Comparing `nci_cidc_schemas-0.26.29/cidc_schemas/schemas/shipping_core.json` & `nci_cidc_schemas-0.26.32/cidc_schemas/schemas/shipping_core.json`

 * *Files identical despite different names*

### Comparing `nci_cidc_schemas-0.26.29/cidc_schemas/schemas/templates/analyses/atacseq_analysis_template.json` & `nci_cidc_schemas-0.26.32/cidc_schemas/schemas/templates/analyses/atacseq_analysis_template.json`

 * *Files identical despite different names*

### Comparing `nci_cidc_schemas-0.26.29/cidc_schemas/schemas/templates/analyses/cytof_analysis_template.json` & `nci_cidc_schemas-0.26.32/cidc_schemas/schemas/templates/analyses/cytof_analysis_template.json`

 * *Files identical despite different names*

### Comparing `nci_cidc_schemas-0.26.29/cidc_schemas/schemas/templates/analyses/rna_level1_analysis_template.json` & `nci_cidc_schemas-0.26.32/cidc_schemas/schemas/templates/analyses/rna_level1_analysis_template.json`

 * *Files identical despite different names*

### Comparing `nci_cidc_schemas-0.26.29/cidc_schemas/schemas/templates/analyses/tcr_analysis_template.json` & `nci_cidc_schemas-0.26.32/cidc_schemas/schemas/templates/analyses/tcr_analysis_template.json`

 * *Files identical despite different names*

### Comparing `nci_cidc_schemas-0.26.29/cidc_schemas/schemas/templates/analyses/wes_analysis_template.json` & `nci_cidc_schemas-0.26.32/cidc_schemas/schemas/templates/analyses/wes_analysis_template.json`

 * *Files identical despite different names*

### Comparing `nci_cidc_schemas-0.26.29/cidc_schemas/schemas/templates/analyses/wes_tumor_only_analysis_template.json` & `nci_cidc_schemas-0.26.32/cidc_schemas/schemas/templates/analyses/wes_tumor_only_analysis_template.json`

 * *Files identical despite different names*

### Comparing `nci_cidc_schemas-0.26.29/cidc_schemas/schemas/templates/assays/atacseq_fastq_template.json` & `nci_cidc_schemas-0.26.32/cidc_schemas/schemas/templates/assays/atacseq_fastq_template.json`

 * *Files identical despite different names*

### Comparing `nci_cidc_schemas-0.26.29/cidc_schemas/schemas/templates/assays/clinical_data_template.json` & `nci_cidc_schemas-0.26.32/cidc_schemas/schemas/templates/assays/clinical_data_template.json`

 * *Files identical despite different names*

### Comparing `nci_cidc_schemas-0.26.29/cidc_schemas/schemas/templates/assays/ctdna_template.json` & `nci_cidc_schemas-0.26.32/tests/data/schemas/target-templates/atacseq_analysis_template.json`

 * *Files 20% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.35%*

 * *Differences: {"'description'": "'Assay by Transposase-Accessible Chromatin by Sequencing (ATACseq) analysis "*

 * *                  "submission.'",*

 * * "'prism_template_root_object_pointer'": "'/analysis/atacseq_analysis/0'",*

 * * "'prism_template_root_object_schema'": "'assays/components/ngs/atacseq/atacseq_analysis.json'",*

 * * "'properties'": "{'worksheets': {replace: OrderedDict([('ATACseq Analysis', "*

 * *                 "OrderedDict([('preamble_rows', OrderedDict([('protocol identifier', "*

 * *                 "OrderedDict([('merge_poi […]*

```diff
@@ -1,106 +1,93 @@
 {
-    "description": "Metadata information for Circulating Tumor DNA (ctDNA) Assay data submission.",
+    "description": "Assay by Transposase-Accessible Chromatin by Sequencing (ATACseq) analysis submission.",
+    "prism_template_root_object_pointer": "/analysis/atacseq_analysis/0",
+    "prism_template_root_object_schema": "assays/components/ngs/atacseq/atacseq_analysis.json",
     "properties": {
         "worksheets": {
-            "ctDNA": {
+            "ATACseq Analysis": {
                 "data_columns": {
-                    "Samples": {
-                        "bias qc plots": {
-                            "gcs_uri_format": "{protocol identifier}/ctdna/{batch id}/{cimac id}/bias_qc_plots.pdf",
-                            "is_artifact": 1,
-                            "merge_pointer": "0/bias_qc_plots",
-                            "type_ref": "assays/components/local_file.json#properties/file_path"
-                        },
+                    "ATACseq Runs": {
                         "cimac id": {
-                            "merge_pointer": "0/cimac_id",
+                            "merge_pointer": "/cimac_id",
+                            "process_as": [
+                                {
+                                    "gcs_uri_format": "{protocol identifier}/atacseq/{cimac id}/analysis/peaks/sorted_peaks.bed",
+                                    "is_artifact": 1,
+                                    "merge_pointer": "0/peaks/sorted_peaks_bed",
+                                    "parse_through": "lambda id: f'{folder or \"\"}analysis/peaks/{id}.rep1/{id}.rep1_sorted_peaks.bed'",
+                                    "type_ref": "assays/components/local_file.json#properties/file_path"
+                                },
+                                {
+                                    "gcs_uri_format": "{protocol identifier}/atacseq/{cimac id}/analysis/peaks/sorted_summits.bed",
+                                    "is_artifact": 1,
+                                    "merge_pointer": "0/peaks/sorted_summits",
+                                    "parse_through": "lambda id: f'{folder or \"\"}analysis/peaks/{id}.rep1/{id}.rep1_sorted_summits.bed'",
+                                    "type_ref": "assays/components/local_file.json#properties/file_path"
+                                },
+                                {
+                                    "gcs_uri_format": "{protocol identifier}/atacseq/{cimac id}/analysis/peaks/sorted_peaks.narrowPeak",
+                                    "is_artifact": 1,
+                                    "merge_pointer": "0/peaks/sorted_peaks_narrowpeak",
+                                    "parse_through": "lambda id: f'{folder or \"\"}analysis/peaks/{id}.rep1/{id}.rep1_sorted_peaks.narrowPeak'",
+                                    "type_ref": "assays/components/local_file.json#properties/file_path"
+                                },
+                                {
+                                    "gcs_uri_format": "{protocol identifier}/atacseq/{cimac id}/analysis/peaks/treat_pileup.bw",
+                                    "is_artifact": 1,
+                                    "merge_pointer": "0/peaks/treat_pileup",
+                                    "parse_through": "lambda id: f'{folder or \"\"}analysis/peaks/{id}.rep1/{id}.rep1_treat_pileup.bw'",
+                                    "type_ref": "assays/components/local_file.json#properties/file_path"
+                                },
+                                {
+                                    "gcs_uri_format": "{protocol identifier}/atacseq/{cimac id}/analysis/aligned_sorted.bam",
+                                    "is_artifact": 1,
+                                    "merge_pointer": "0/aligned_sorted_bam",
+                                    "parse_through": "lambda id: f'{folder or \"\"}analysis/align/{id}/{id}.sorted.bam'",
+                                    "type_ref": "assays/components/local_file.json#properties/file_path"
+                                }
+                            ],
                             "type_ref": "sample.json#properties/cimac_id"
                         },
                         "comments": {
                             "allow_empty": true,
                             "merge_pointer": "0/comments",
-                            "type_ref": "assays/ctdna_assay.json#definitions/entry/properties/comments"
-                        },
-                        "demultiplexed bam": {
-                            "gcs_uri_format": "{protocol identifier}/ctdna/{batch id}/{cimac id}/demultiplexed.bam",
-                            "is_artifact": 1,
-                            "merge_pointer": "0/demultiplexed_bam",
-                            "type_ref": "assays/components/local_file.json#properties/file_path"
-                        },
-                        "demultiplexed bam index": {
-                            "gcs_uri_format": "{protocol identifier}/ctdna/{batch id}/{cimac id}/demultiplexed.bam.bai",
-                            "is_artifact": 1,
-                            "merge_pointer": "0/demultiplexed_bam_index",
-                            "type_ref": "assays/components/local_file.json#properties/file_path"
-                        },
-                        "fraction cna subclonal": {
-                            "merge_pointer": "0/fraction_cna_subclonal",
-                            "type_ref": "assays/ctdna_assay.json#definitions/entry/properties/fraction_cna_subclonal"
-                        },
-                        "fraction genome subclonal": {
-                            "merge_pointer": "0/fraction_genome_subclonal",
-                            "type_ref": "assays/ctdna_assay.json#definitions/entry/properties/fraction_genome_subclonal"
-                        },
-                        "gc map correction mad": {
-                            "merge_pointer": "0/gc_map_correction_mad",
-                            "type_ref": "assays/ctdna_assay.json#definitions/entry/properties/gc_map_correction_mad"
-                        },
-                        "genome-wide plots": {
-                            "gcs_uri_format": "{protocol identifier}/ctdna/{batch id}/{cimac id}/genome-wide_plots.pdf",
-                            "is_artifact": 1,
-                            "merge_pointer": "0/genome-wide_plots",
-                            "type_ref": "assays/components/local_file.json#properties/file_path"
-                        },
-                        "optimal solution": {
-                            "gcs_uri_format": "{protocol identifier}/ctdna/{batch id}/{cimac id}/optimal_solution.zip",
-                            "is_artifact": 1,
-                            "merge_pointer": "0/optimal_solution",
-                            "type_ref": "assays/components/local_file.json#properties/file_path"
-                        },
-                        "other solutions": {
-                            "gcs_uri_format": "{protocol identifier}/ctdna/{batch id}/{cimac id}/other_solutions.zip",
-                            "is_artifact": 1,
-                            "merge_pointer": "0/other_solutions",
-                            "type_ref": "assays/components/local_file.json#properties/file_path"
-                        },
-                        "subclone fraction": {
-                            "merge_pointer": "0/subclone_fraction",
-                            "type_ref": "assays/ctdna_assay.json#definitions/entry/properties/subclone_fraction"
-                        },
-                        "tumor fraction": {
-                            "merge_pointer": "0/tumor_fraction",
-                            "type_ref": "assays/ctdna_assay.json#definitions/entry/properties/tumor_fraction"
-                        },
-                        "tumor ploidy": {
-                            "merge_pointer": "0/tumor_ploidy",
-                            "type_ref": "assays/ctdna_assay.json#definitions/entry/properties/tumor_ploidy"
+                            "type_ref": "assays/components/ngs/atacseq/atacseq_analysis.json#definitions/entry/properties/comments"
                         }
                     }
                 },
                 "preamble_rows": {
-                    "assay creator": {
-                        "merge_pointer": "0/assay_creator",
-                        "type_ref": "assays/components/assay_core.json#properties/assay_creator"
-                    },
                     "batch id": {
                         "merge_pointer": "0/batch_id",
-                        "type_ref": "assays/ctdna_assay.json#properties/batch_id"
+                        "type_ref": "assays/atacseq_assay.json#properties/batch_id"
+                    },
+                    "folder": {
+                        "allow_empty": true,
+                        "do_not_merge": true,
+                        "type": "string"
                     },
                     "protocol identifier": {
                         "merge_pointer": "3/protocol_identifier",
                         "type_ref": "clinical_trial.json#properties/protocol_identifier"
-                    },
-                    "summary plots": {
-                        "gcs_uri_format": "{protocol identifier}/ctdna/{batch id}/summary_plots.pdf",
-                        "is_artifact": 1,
-                        "merge_pointer": "0/summary_plots",
-                        "type_ref": "assays/components/local_file.json#properties/file_path"
                     }
                 },
-                "prism_data_object_pointer": "/records/-",
-                "prism_preamble_object_pointer": "/assays/ctdna/-",
-                "prism_preamble_object_schema": "assays/ctdna_assay.json"
+                "prism_data_object_pointer": "/records/-"
+            },
+            "Excluded Samples": {
+                "data_columns": {
+                    "Samples Excluded From Analysis": {
+                        "cimac id": {
+                            "merge_pointer": "0/cimac_id",
+                            "type_ref": "sample.json#properties/cimac_id"
+                        },
+                        "reason": {
+                            "merge_pointer": "0/reason_excluded",
+                            "type_ref": "assays/components/excluded_samples.json#items/properties/reason_excluded"
+                        }
+                    }
+                },
+                "prism_data_object_pointer": "/excluded_samples/-"
             }
         }
     },
-    "title": "Metadata file for ctDNA Assay"
+    "title": "ATACseq analysis template"
 }
```

### Comparing `nci_cidc_schemas-0.26.29/cidc_schemas/schemas/templates/assays/cytof_template.json` & `nci_cidc_schemas-0.26.32/cidc_schemas/schemas/templates/assays/cytof_template.json`

 * *Files identical despite different names*

### Comparing `nci_cidc_schemas-0.26.29/cidc_schemas/schemas/templates/assays/elisa_template.json` & `nci_cidc_schemas-0.26.32/cidc_schemas/schemas/templates/assays/elisa_template.json`

 * *Files identical despite different names*

### Comparing `nci_cidc_schemas-0.26.29/cidc_schemas/schemas/templates/assays/hande_template.json` & `nci_cidc_schemas-0.26.32/cidc_schemas/schemas/templates/assays/hande_template.json`

 * *Files identical despite different names*

### Comparing `nci_cidc_schemas-0.26.29/cidc_schemas/schemas/templates/assays/ihc_template.json` & `nci_cidc_schemas-0.26.32/cidc_schemas/schemas/templates/assays/ihc_template.json`

 * *Files identical despite different names*

### Comparing `nci_cidc_schemas-0.26.29/cidc_schemas/schemas/templates/assays/mibi_template.json` & `nci_cidc_schemas-0.26.32/cidc_schemas/schemas/templates/assays/mibi_template.json`

 * *Files identical despite different names*

### Comparing `nci_cidc_schemas-0.26.29/cidc_schemas/schemas/templates/assays/microbiome_template.json` & `nci_cidc_schemas-0.26.32/cidc_schemas/schemas/templates/assays/microbiome_template.json`

 * *Files identical despite different names*

### Comparing `nci_cidc_schemas-0.26.29/cidc_schemas/schemas/templates/assays/mif_template.json` & `nci_cidc_schemas-0.26.32/cidc_schemas/schemas/templates/assays/mif_template.json`

 * *Files identical despite different names*

### Comparing `nci_cidc_schemas-0.26.29/cidc_schemas/schemas/templates/assays/misc_data_template.json` & `nci_cidc_schemas-0.26.32/cidc_schemas/schemas/templates/assays/misc_data_template.json`

 * *Files identical despite different names*

### Comparing `nci_cidc_schemas-0.26.29/cidc_schemas/schemas/templates/assays/nanostring_template.json` & `nci_cidc_schemas-0.26.32/cidc_schemas/schemas/templates/assays/nanostring_template.json`

 * *Files identical despite different names*

### Comparing `nci_cidc_schemas-0.26.29/cidc_schemas/schemas/templates/assays/olink_template.json` & `nci_cidc_schemas-0.26.32/cidc_schemas/schemas/templates/assays/olink_template.json`

 * *Files identical despite different names*

### Comparing `nci_cidc_schemas-0.26.29/cidc_schemas/schemas/templates/assays/rna_bam_template.json` & `nci_cidc_schemas-0.26.32/cidc_schemas/schemas/templates/assays/rna_bam_template.json`

 * *Files identical despite different names*

### Comparing `nci_cidc_schemas-0.26.29/cidc_schemas/schemas/templates/assays/rna_fastq_template.json` & `nci_cidc_schemas-0.26.32/cidc_schemas/schemas/templates/assays/rna_fastq_template.json`

 * *Files identical despite different names*

### Comparing `nci_cidc_schemas-0.26.29/cidc_schemas/schemas/templates/assays/tcr_adaptive_template.json` & `nci_cidc_schemas-0.26.32/cidc_schemas/schemas/templates/assays/tcr_adaptive_template.json`

 * *Files identical despite different names*

### Comparing `nci_cidc_schemas-0.26.29/cidc_schemas/schemas/templates/assays/tcr_fastq_template.json` & `nci_cidc_schemas-0.26.32/cidc_schemas/schemas/templates/assays/tcr_fastq_template.json`

 * *Files identical despite different names*

### Comparing `nci_cidc_schemas-0.26.29/cidc_schemas/schemas/templates/assays/wes_bam_template.json` & `nci_cidc_schemas-0.26.32/cidc_schemas/schemas/templates/assays/wes_bam_template.json`

 * *Files identical despite different names*

### Comparing `nci_cidc_schemas-0.26.29/cidc_schemas/schemas/templates/assays/wes_fastq_template.json` & `nci_cidc_schemas-0.26.32/cidc_schemas/schemas/templates/assays/wes_fastq_template.json`

 * *Files identical despite different names*

### Comparing `nci_cidc_schemas-0.26.29/cidc_schemas/schemas/templates/manifests/h_and_e_template.json` & `nci_cidc_schemas-0.26.32/cidc_schemas/schemas/templates/manifests/h_and_e_template.json`

 * *Files identical despite different names*

### Comparing `nci_cidc_schemas-0.26.29/cidc_schemas/schemas/templates/manifests/microbiome_dna_template.json` & `nci_cidc_schemas-0.26.32/cidc_schemas/schemas/templates/manifests/microbiome_dna_template.json`

 * *Files identical despite different names*

### Comparing `nci_cidc_schemas-0.26.29/cidc_schemas/schemas/templates/manifests/normal_blood_dna_template.json` & `nci_cidc_schemas-0.26.32/cidc_schemas/schemas/templates/manifests/normal_blood_dna_template.json`

 * *Files identical despite different names*

### Comparing `nci_cidc_schemas-0.26.29/cidc_schemas/schemas/templates/manifests/normal_tissue_dna_template.json` & `nci_cidc_schemas-0.26.32/cidc_schemas/schemas/templates/manifests/normal_tissue_dna_template.json`

 * *Files identical despite different names*

### Comparing `nci_cidc_schemas-0.26.29/cidc_schemas/schemas/templates/manifests/pbmc_template.json` & `nci_cidc_schemas-0.26.32/cidc_schemas/schemas/templates/manifests/pbmc_template.json`

 * *Files identical despite different names*

### Comparing `nci_cidc_schemas-0.26.29/cidc_schemas/schemas/templates/manifests/plasma_template.json` & `nci_cidc_schemas-0.26.32/cidc_schemas/schemas/templates/manifests/plasma_template.json`

 * *Files identical despite different names*

### Comparing `nci_cidc_schemas-0.26.29/cidc_schemas/schemas/templates/manifests/tissue_slide_template.json` & `nci_cidc_schemas-0.26.32/cidc_schemas/schemas/templates/manifests/tissue_slide_template.json`

 * *Files identical despite different names*

### Comparing `nci_cidc_schemas-0.26.29/cidc_schemas/schemas/templates/manifests/tumor_normal_pairing_template.json` & `nci_cidc_schemas-0.26.32/cidc_schemas/schemas/templates/manifests/tumor_normal_pairing_template.json`

 * *Files identical despite different names*

### Comparing `nci_cidc_schemas-0.26.29/cidc_schemas/schemas/templates/manifests/tumor_tissue_dna_template.json` & `nci_cidc_schemas-0.26.32/cidc_schemas/schemas/templates/manifests/tumor_tissue_dna_template.json`

 * *Files identical despite different names*

### Comparing `nci_cidc_schemas-0.26.29/cidc_schemas/schemas/templates/manifests/tumor_tissue_rna_template.json` & `nci_cidc_schemas-0.26.32/cidc_schemas/schemas/templates/manifests/tumor_tissue_rna_template.json`

 * *Files identical despite different names*

### Comparing `nci_cidc_schemas-0.26.29/cidc_schemas/template.py` & `nci_cidc_schemas-0.26.32/cidc_schemas/template.py`

 * *Files 0% similar despite different names*

```diff
@@ -228,14 +228,15 @@
     )
 
     expanded_name = {
         "atacseq": f"Assay by Transposase-Accessible Chromatin by Sequencing (ATACseq)",
         "rna": "RNA sequencing Level 1",
         "wes": "Whole Exome Sequencing (WES) Tumor-Normal Paired",
         "wes_tumor_only": "Whole Exome Sequencing (WES) Tumor-Only",
+        "ctDNA": "ctDNA",
     }[name]
 
     # static
     template = {
         "title": f"{title} analysis template",
         "description": f"{expanded_name} analysis submission.",
         "prism_template_root_object_schema": obj_root_schema,
@@ -415,14 +416,15 @@
 
     # so many different ways of writing it
     title = {
         "atacseq": "ATACseq",
         "rna": "RNAseq level 1",
         "wes": "WES",
         "wes_tumor_only": "WES tumor-only",
+        "ctdna": "ctDNA",
     }[name]
 
     pointer = [
         k
         for k, subschema in assay_schema["properties"].items()
         if k != "excluded_samples" and "items" in subschema
     ]
@@ -821,15 +823,15 @@
                 file_uuid = self.coerce(local_path)
 
                 artifact, facet_group = self._format_single_artifact(
                     local_path=local_path,
                     uuid=file_uuid,
                     format_context=dict(
                         format_context,
-                        num=num  # add num to be able to generate
+                        num=num,  # add num to be able to generate
                         # different gcs keys for each multi-artifact file.
                     ),
                 )
 
                 val.append(
                     {"upload_placeholder": file_uuid, "facet_group": facet_group}
                 )
@@ -998,17 +1000,17 @@
                 processed_worksheet[section_name] = process_fields(section_schema)
             elif section_name == "data_columns":
                 data_schemas = {}
                 for table_name, table_schema in section_schema.items():
                     data_schemas[table_name] = process_fields(table_schema)
                 processed_worksheet[section_name] = data_schemas
             elif section_name == "prism_arbitrary_data_merge_pointer":
-                processed_worksheet[
-                    "prism_arbitrary_data_merge_pointer"
-                ] = section_schema
+                processed_worksheet["prism_arbitrary_data_merge_pointer"] = (
+                    section_schema
+                )
 
         return processed_worksheet
 
     def _get_ref_coerce(self, ref: str):
         """
         This function takes a json-schema style $ref pointer,
         opens the schema and determines the best python
```

### Comparing `nci_cidc_schemas-0.26.29/cidc_schemas/template_reader.py` & `nci_cidc_schemas-0.26.32/cidc_schemas/template_reader.py`

 * *Files identical despite different names*

### Comparing `nci_cidc_schemas-0.26.29/cidc_schemas/template_writer.py` & `nci_cidc_schemas-0.26.32/cidc_schemas/template_writer.py`

 * *Files identical despite different names*

### Comparing `nci_cidc_schemas-0.26.29/cidc_schemas/unprism.py` & `nci_cidc_schemas-0.26.32/cidc_schemas/unprism.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """Tools from extracting information from trial metadata blobs."""
+
 from io import StringIO, BytesIO
 from typing import Callable, Dict, List, NamedTuple, Optional, Union
 
 import pandas as pd
 
 from . import prism
 from .util import participant_id_from_cimac
```

### Comparing `nci_cidc_schemas-0.26.29/cidc_schemas/util.py` & `nci_cidc_schemas-0.26.32/cidc_schemas/util.py`

 * *Files identical despite different names*

### Comparing `nci_cidc_schemas-0.26.29/nci_cidc_schemas.egg-info/PKG-INFO` & `nci_cidc_schemas-0.26.32/nci_cidc_schemas.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nci_cidc_schemas
-Version: 0.26.29
+Version: 0.26.32
 Summary: The CIDC data model and tools for working with it.
 Home-page: https://github.com/NCI-CIDC/cidc-schemas
 Author: NCI
 Author-email: nci-cidc-tools-admin@mail.nih.gov
 License: MIT license
 Keywords: cidc_schemas
 Classifier: Development Status :: 2 - Pre-Alpha
```

### Comparing `nci_cidc_schemas-0.26.29/nci_cidc_schemas.egg-info/SOURCES.txt` & `nci_cidc_schemas-0.26.32/nci_cidc_schemas.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -52,23 +52,25 @@
 cidc_schemas/schemas/artifacts/artifact_log.json
 cidc_schemas/schemas/artifacts/artifact_maf.json
 cidc_schemas/schemas/artifacts/artifact_narrowPeak.json
 cidc_schemas/schemas/artifacts/artifact_npx.json
 cidc_schemas/schemas/artifacts/artifact_pdf.json
 cidc_schemas/schemas/artifacts/artifact_png.json
 cidc_schemas/schemas/artifacts/artifact_rcc.json
+cidc_schemas/schemas/artifacts/artifact_rdata.json
 cidc_schemas/schemas/artifacts/artifact_tbi.json
 cidc_schemas/schemas/artifacts/artifact_text.json
 cidc_schemas/schemas/artifacts/artifact_tsv.json
 cidc_schemas/schemas/artifacts/artifact_vcf.json
 cidc_schemas/schemas/artifacts/artifact_vcf_gz.json
 cidc_schemas/schemas/artifacts/artifact_xlsx.json
 cidc_schemas/schemas/artifacts/artifact_yaml.json
 cidc_schemas/schemas/artifacts/artifact_zip.json
 cidc_schemas/schemas/assays/atacseq_assay.json
+cidc_schemas/schemas/assays/ctdna_analysis.json
 cidc_schemas/schemas/assays/ctdna_assay.json
 cidc_schemas/schemas/assays/cytof_assay.json
 cidc_schemas/schemas/assays/cytof_assay_core.json
 cidc_schemas/schemas/assays/elisa_assay.json
 cidc_schemas/schemas/assays/hande_assay.json
 cidc_schemas/schemas/assays/ihc_assay.json
 cidc_schemas/schemas/assays/mibi_assay.json
@@ -117,14 +119,15 @@
 cidc_schemas/schemas/assays/components/ngs/rna/rna_analysis.json
 cidc_schemas/schemas/assays/components/ngs/rna/rna_level1_analysis.json
 cidc_schemas/schemas/assays/components/ngs/rna/rseqc.json
 cidc_schemas/schemas/assays/components/ngs/rna/salmon.json
 cidc_schemas/schemas/assays/components/ngs/rna/star.json
 cidc_schemas/schemas/assays/components/ngs/rna/trust4.json
 cidc_schemas/schemas/templates/analyses/atacseq_analysis_template.json
+cidc_schemas/schemas/templates/analyses/ctdna_analysis_template.json
 cidc_schemas/schemas/templates/analyses/cytof_analysis_template.json
 cidc_schemas/schemas/templates/analyses/rna_level1_analysis_template.json
 cidc_schemas/schemas/templates/analyses/tcr_analysis_template.json
 cidc_schemas/schemas/templates/analyses/wes_analysis_template.json
 cidc_schemas/schemas/templates/analyses/wes_tumor_only_analysis_template.json
 cidc_schemas/schemas/templates/assays/atacseq_fastq_template.json
 cidc_schemas/schemas/templates/assays/clinical_data_template.json
@@ -206,14 +209,15 @@
 tests/data/schemas/a.json
 tests/data/schemas/b.json
 tests/data/schemas/c.json
 tests/data/schemas/invalid_ref.json
 tests/data/schemas/d1/3.json
 tests/data/schemas/d1/d2/2.json
 tests/data/schemas/target-templates/atacseq_analysis_template.json
+tests/data/schemas/target-templates/ctdna_analysis_template.json
 tests/data/schemas/target-templates/rna_level1_analysis_template.json
 tests/data/schemas/target-templates/wes_analysis_template.json
 tests/data/schemas/target-templates/wes_tumor_only_analysis_template.json
 tests/prism/__init__.py
 tests/prism/test_cidc_data_model.py
 tests/prism/test_constants.py
 tests/prism/test_core.py
```

### Comparing `nci_cidc_schemas-0.26.29/setup.py` & `nci_cidc_schemas-0.26.32/setup.py`

 * *Files identical despite different names*

### Comparing `nci_cidc_schemas-0.26.29/tests/conftest.py` & `nci_cidc_schemas-0.26.32/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `nci_cidc_schemas-0.26.29/tests/data/clinical_test_file.1.xlsx` & `nci_cidc_schemas-0.26.32/tests/data/clinical_test_file.1.xlsx`

 * *Files identical despite different names*

### Comparing `nci_cidc_schemas-0.26.29/tests/data/clinical_test_file.2.xlsx` & `nci_cidc_schemas-0.26.32/tests/data/clinical_test_file.2.xlsx`

 * *Files identical despite different names*

### Comparing `nci_cidc_schemas-0.26.29/tests/data/clinical_test_file.3.xlsx` & `nci_cidc_schemas-0.26.32/tests/data/clinical_test_file.3.xlsx`

 * *Files identical despite different names*

### Comparing `nci_cidc_schemas-0.26.29/tests/data/clinical_test_file.docx` & `nci_cidc_schemas-0.26.32/tests/data/clinical_test_file.docx`

 * *Files identical despite different names*

### Comparing `nci_cidc_schemas-0.26.29/tests/data/clinicaltrial_examples/CT_1.json` & `nci_cidc_schemas-0.26.32/tests/data/clinicaltrial_examples/CT_1.json`

 * *Files identical despite different names*

### Comparing `nci_cidc_schemas-0.26.29/tests/data/clinicaltrial_examples/CT_1PA_multiWES.json` & `nci_cidc_schemas-0.26.32/tests/data/clinicaltrial_examples/CT_1PA_multiWES.json`

 * *Files identical despite different names*

### Comparing `nci_cidc_schemas-0.26.29/tests/data/clinicaltrial_examples/CT_cytof_with_analysis.json` & `nci_cidc_schemas-0.26.32/tests/data/clinicaltrial_examples/CT_cytof_with_analysis.json`

 * *Files identical despite different names*

### Comparing `nci_cidc_schemas-0.26.29/tests/data/clinicaltrial_examples/CT_ihc.json` & `nci_cidc_schemas-0.26.32/tests/data/clinicaltrial_examples/CT_ihc.json`

 * *Files identical despite different names*

### Comparing `nci_cidc_schemas-0.26.29/tests/data/clinicaltrial_examples/CT_minimal.json` & `nci_cidc_schemas-0.26.32/tests/data/clinicaltrial_examples/CT_minimal.json`

 * *Files identical despite different names*

### Comparing `nci_cidc_schemas-0.26.29/tests/data/date_examples.xlsx` & `nci_cidc_schemas-0.26.32/tests/data/date_examples.xlsx`

 * *Files identical despite different names*

### Comparing `nci_cidc_schemas-0.26.29/tests/data/elisa_test_file.1.xlsx` & `nci_cidc_schemas-0.26.32/tests/data/elisa_test_file.1.xlsx`

 * *Files identical despite different names*

### Comparing `nci_cidc_schemas-0.26.29/tests/data/elisa_test_file.2.xlsx` & `nci_cidc_schemas-0.26.32/tests/data/elisa_test_file.2.xlsx`

 * *Files identical despite different names*

### Comparing `nci_cidc_schemas-0.26.29/tests/data/hande_err_template.xlsx` & `nci_cidc_schemas-0.26.32/tests/data/hande_err_template.xlsx`

 * *Files identical despite different names*

### Comparing `nci_cidc_schemas-0.26.29/tests/data/olink/invalid_olink_assay_1_NPX.xlsx` & `nci_cidc_schemas-0.26.32/tests/data/olink/invalid_olink_assay_1_NPX.xlsx`

 * *Files identical despite different names*

### Comparing `nci_cidc_schemas-0.26.29/tests/data/olink/olink_assay_1_NPX.xlsx` & `nci_cidc_schemas-0.26.32/tests/data/olink/olink_assay_1_NPX.xlsx`

 * *Files identical despite different names*

### Comparing `nci_cidc_schemas-0.26.29/tests/data/olink/olink_assay_2_NPX.xlsx` & `nci_cidc_schemas-0.26.32/tests/data/olink/olink_assay_2_NPX.xlsx`

 * *Files identical despite different names*

### Comparing `nci_cidc_schemas-0.26.29/tests/data/olink/olink_assay_combined.xlsx` & `nci_cidc_schemas-0.26.32/tests/data/olink/olink_assay_combined.xlsx`

 * *Files identical despite different names*

### Comparing `nci_cidc_schemas-0.26.29/tests/data/pbmc_invalid.xlsx` & `nci_cidc_schemas-0.26.32/tests/data/pbmc_invalid.xlsx`

 * *Files identical despite different names*

### Comparing `nci_cidc_schemas-0.26.29/tests/data/schemas/target-templates/atacseq_analysis_template.json` & `nci_cidc_schemas-0.26.32/cidc_schemas/schemas/templates/assays/ctdna_template.json`

 * *Files 17% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.35%*

 * *Differences: {"'description'": "'Metadata information for Circulating Tumor DNA (ctDNA) Assay data submission.'",*

 * * "'properties'": "{'worksheets': {replace: OrderedDict([('ctDNA', "*

 * *                 "OrderedDict([('prism_preamble_object_schema', 'assays/ctdna_assay.json'), "*

 * *                 "('prism_preamble_object_pointer', '/assays/ctdna/-'), "*

 * *                 "('prism_data_object_pointer', '/records/-'), ('preamble_rows', "*

 * *                 "OrderedDict([('protocol identifier', OrderedDict([('merge_pointer', "*

 * *     […]*

```diff
@@ -1,93 +1,124 @@
 {
-    "description": "Assay by Transposase-Accessible Chromatin by Sequencing (ATACseq) analysis submission.",
-    "prism_template_root_object_pointer": "/analysis/atacseq_analysis/0",
-    "prism_template_root_object_schema": "assays/components/ngs/atacseq/atacseq_analysis.json",
+    "description": "Metadata information for Circulating Tumor DNA (ctDNA) Assay data submission.",
     "properties": {
         "worksheets": {
-            "ATACseq Analysis": {
+            "ctDNA": {
                 "data_columns": {
-                    "ATACseq Runs": {
+                    "Samples": {
+                        "bias qc plots": {
+                            "gcs_uri_format": "{protocol identifier}/ctdna/{batch id}/{cimac id}/bias_qc_plots.pdf",
+                            "is_artifact": 1,
+                            "merge_pointer": "0/bias_qc_plots",
+                            "type_ref": "assays/components/local_file.json#properties/file_path"
+                        },
                         "cimac id": {
-                            "merge_pointer": "/cimac_id",
-                            "process_as": [
-                                {
-                                    "gcs_uri_format": "{protocol identifier}/atacseq/{cimac id}/analysis/peaks/sorted_peaks.bed",
-                                    "is_artifact": 1,
-                                    "merge_pointer": "0/peaks/sorted_peaks_bed",
-                                    "parse_through": "lambda id: f'{folder or \"\"}analysis/peaks/{id}.rep1/{id}.rep1_sorted_peaks.bed'",
-                                    "type_ref": "assays/components/local_file.json#properties/file_path"
-                                },
-                                {
-                                    "gcs_uri_format": "{protocol identifier}/atacseq/{cimac id}/analysis/peaks/sorted_summits.bed",
-                                    "is_artifact": 1,
-                                    "merge_pointer": "0/peaks/sorted_summits",
-                                    "parse_through": "lambda id: f'{folder or \"\"}analysis/peaks/{id}.rep1/{id}.rep1_sorted_summits.bed'",
-                                    "type_ref": "assays/components/local_file.json#properties/file_path"
-                                },
-                                {
-                                    "gcs_uri_format": "{protocol identifier}/atacseq/{cimac id}/analysis/peaks/sorted_peaks.narrowPeak",
-                                    "is_artifact": 1,
-                                    "merge_pointer": "0/peaks/sorted_peaks_narrowpeak",
-                                    "parse_through": "lambda id: f'{folder or \"\"}analysis/peaks/{id}.rep1/{id}.rep1_sorted_peaks.narrowPeak'",
-                                    "type_ref": "assays/components/local_file.json#properties/file_path"
-                                },
-                                {
-                                    "gcs_uri_format": "{protocol identifier}/atacseq/{cimac id}/analysis/peaks/treat_pileup.bw",
-                                    "is_artifact": 1,
-                                    "merge_pointer": "0/peaks/treat_pileup",
-                                    "parse_through": "lambda id: f'{folder or \"\"}analysis/peaks/{id}.rep1/{id}.rep1_treat_pileup.bw'",
-                                    "type_ref": "assays/components/local_file.json#properties/file_path"
-                                },
-                                {
-                                    "gcs_uri_format": "{protocol identifier}/atacseq/{cimac id}/analysis/aligned_sorted.bam",
-                                    "is_artifact": 1,
-                                    "merge_pointer": "0/aligned_sorted_bam",
-                                    "parse_through": "lambda id: f'{folder or \"\"}analysis/align/{id}/{id}.sorted.bam'",
-                                    "type_ref": "assays/components/local_file.json#properties/file_path"
-                                }
-                            ],
+                            "merge_pointer": "0/cimac_id",
                             "type_ref": "sample.json#properties/cimac_id"
                         },
                         "comments": {
                             "allow_empty": true,
                             "merge_pointer": "0/comments",
-                            "type_ref": "assays/components/ngs/atacseq/atacseq_analysis.json#definitions/entry/properties/comments"
+                            "type_ref": "assays/ctdna_assay.json#definitions/entry/properties/comments"
+                        },
+                        "demultiplexed bam": {
+                            "gcs_uri_format": "{protocol identifier}/ctdna/{batch id}/{cimac id}/demultiplexed.bam",
+                            "is_artifact": 1,
+                            "merge_pointer": "0/demultiplexed_bam",
+                            "type_ref": "assays/components/local_file.json#properties/file_path"
+                        },
+                        "demultiplexed bam index": {
+                            "gcs_uri_format": "{protocol identifier}/ctdna/{batch id}/{cimac id}/demultiplexed.bam.bai",
+                            "is_artifact": 1,
+                            "merge_pointer": "0/demultiplexed_bam_index",
+                            "type_ref": "assays/components/local_file.json#properties/file_path"
+                        },
+                        "fraction cna subclonal": {
+                            "merge_pointer": "0/fraction_cna_subclonal",
+                            "type_ref": "assays/ctdna_assay.json#definitions/entry/properties/fraction_cna_subclonal"
+                        },
+                        "fraction genome subclonal": {
+                            "merge_pointer": "0/fraction_genome_subclonal",
+                            "type_ref": "assays/ctdna_assay.json#definitions/entry/properties/fraction_genome_subclonal"
+                        },
+                        "gc map correction mad": {
+                            "merge_pointer": "0/gc_map_correction_mad",
+                            "type_ref": "assays/ctdna_assay.json#definitions/entry/properties/gc_map_correction_mad"
+                        },
+                        "genome-wide plots": {
+                            "gcs_uri_format": "{protocol identifier}/ctdna/{batch id}/{cimac id}/genome-wide_plots.pdf",
+                            "is_artifact": 1,
+                            "merge_pointer": "0/genome-wide_plots",
+                            "type_ref": "assays/components/local_file.json#properties/file_path"
+                        },
+                        "on premise corrected depth file": {
+                            "gcs_uri_format": "{protocol identifier}/ctdna/{batch id}/{cimac id}/OnPrem.correctedDepth.txt",
+                            "is_artifact": 1,
+                            "merge_pointer": "0/on_premise_corrected_depth_file",
+                            "type_ref": "assays/components/local_file.json#properties/file_path"
+                        },
+                        "on premise parameters file": {
+                            "gcs_uri_format": "{protocol identifier}/ctdna/{batch id}/{cimac id}/OnPrem.params.txt",
+                            "is_artifact": 1,
+                            "merge_pointer": "0/on_premise_parameters_file",
+                            "type_ref": "assays/components/local_file.json#properties/file_path"
+                        },
+                        "on premise rdata file": {
+                            "gcs_uri_format": "{protocol identifier}/ctdna/{batch id}/{cimac id}/OnPrem.RData",
+                            "is_artifact": 1,
+                            "merge_pointer": "0/on_premise_rdata_file",
+                            "type_ref": "assays/components/local_file.json#properties/file_path"
+                        },
+                        "optimal solution": {
+                            "gcs_uri_format": "{protocol identifier}/ctdna/{batch id}/{cimac id}/optimal_solution.zip",
+                            "is_artifact": 1,
+                            "merge_pointer": "0/optimal_solution",
+                            "type_ref": "assays/components/local_file.json#properties/file_path"
+                        },
+                        "other solutions": {
+                            "gcs_uri_format": "{protocol identifier}/ctdna/{batch id}/{cimac id}/other_solutions.zip",
+                            "is_artifact": 1,
+                            "merge_pointer": "0/other_solutions",
+                            "type_ref": "assays/components/local_file.json#properties/file_path"
+                        },
+                        "subclone fraction": {
+                            "merge_pointer": "0/subclone_fraction",
+                            "type_ref": "assays/ctdna_assay.json#definitions/entry/properties/subclone_fraction"
+                        },
+                        "tumor fraction": {
+                            "merge_pointer": "0/tumor_fraction",
+                            "type_ref": "assays/ctdna_assay.json#definitions/entry/properties/tumor_fraction"
+                        },
+                        "tumor ploidy": {
+                            "merge_pointer": "0/tumor_ploidy",
+                            "type_ref": "assays/ctdna_assay.json#definitions/entry/properties/tumor_ploidy"
                         }
                     }
                 },
                 "preamble_rows": {
+                    "assay creator": {
+                        "merge_pointer": "0/assay_creator",
+                        "type_ref": "assays/components/assay_core.json#properties/assay_creator"
+                    },
                     "batch id": {
                         "merge_pointer": "0/batch_id",
-                        "type_ref": "assays/atacseq_assay.json#properties/batch_id"
-                    },
-                    "folder": {
-                        "allow_empty": true,
-                        "do_not_merge": true,
-                        "type": "string"
+                        "type_ref": "assays/ctdna_assay.json#properties/batch_id"
                     },
                     "protocol identifier": {
                         "merge_pointer": "3/protocol_identifier",
                         "type_ref": "clinical_trial.json#properties/protocol_identifier"
+                    },
+                    "summary plots": {
+                        "gcs_uri_format": "{protocol identifier}/ctdna/{batch id}/summary_plots.pdf",
+                        "is_artifact": 1,
+                        "merge_pointer": "0/summary_plots",
+                        "type_ref": "assays/components/local_file.json#properties/file_path"
                     }
                 },
-                "prism_data_object_pointer": "/records/-"
-            },
-            "Excluded Samples": {
-                "data_columns": {
-                    "Samples Excluded From Analysis": {
-                        "cimac id": {
-                            "merge_pointer": "0/cimac_id",
-                            "type_ref": "sample.json#properties/cimac_id"
-                        },
-                        "reason": {
-                            "merge_pointer": "0/reason_excluded",
-                            "type_ref": "assays/components/excluded_samples.json#items/properties/reason_excluded"
-                        }
-                    }
-                },
-                "prism_data_object_pointer": "/excluded_samples/-"
+                "prism_data_object_pointer": "/records/-",
+                "prism_preamble_object_pointer": "/assays/ctdna/-",
+                "prism_preamble_object_schema": "assays/ctdna_assay.json"
             }
         }
     },
-    "title": "ATACseq analysis template"
+    "title": "Metadata file for ctDNA Assay"
 }
```

### Comparing `nci_cidc_schemas-0.26.29/tests/data/schemas/target-templates/rna_level1_analysis_template.json` & `nci_cidc_schemas-0.26.32/tests/data/schemas/target-templates/rna_level1_analysis_template.json`

 * *Files identical despite different names*

### Comparing `nci_cidc_schemas-0.26.29/tests/data/schemas/target-templates/wes_analysis_template.json` & `nci_cidc_schemas-0.26.32/tests/data/schemas/target-templates/wes_analysis_template.json`

 * *Files identical despite different names*

### Comparing `nci_cidc_schemas-0.26.29/tests/data/schemas/target-templates/wes_tumor_only_analysis_template.json` & `nci_cidc_schemas-0.26.32/tests/data/schemas/target-templates/wes_tumor_only_analysis_template.json`

 * *Files identical despite different names*

### Comparing `nci_cidc_schemas-0.26.29/tests/data/tiny_invalid_manifest.xlsx` & `nci_cidc_schemas-0.26.32/tests/data/tiny_invalid_manifest.xlsx`

 * *Files identical despite different names*

### Comparing `nci_cidc_schemas-0.26.29/tests/data/tiny_valid_manifest.xlsx` & `nci_cidc_schemas-0.26.32/tests/data/tiny_valid_manifest.xlsx`

 * *Files identical despite different names*

### Comparing `nci_cidc_schemas-0.26.29/tests/prism/cidc_test_data/analysis_data.py` & `nci_cidc_schemas-0.26.32/tests/prism/cidc_test_data/analysis_data.py`

 * *Files 2% similar despite different names*

```diff
@@ -1238,14 +1238,236 @@
         upload_entries,
         base_trial,
         target_trial,
     )
 
 
 @analysis_data_generator
+def ctdna_analysis() -> PrismTestData:
+    upload_type = "ctdna_analysis"
+    prismify_args = get_prismify_args(upload_type)
+    prismify_patch = {
+        "analysis": {
+            "ctdna_analysis": {
+                "runs": [
+                    {
+                        "run_id": "run_1",
+                        "error": {
+                            "upload_placeholder": "msi18d7a-fd96-4e75-b265-1590c703a303"
+                        },
+                        "tumor": {
+                            "cimac_id": "CTTTPP111.00",
+                            "alignment": {
+                                "align_sorted_dedup": {
+                                    "upload_placeholder": "3068ae50-3ce7-4b0c-ba56-f678233dd098"
+                                },
+                                "align_sorted_dedup_index": {
+                                    "upload_placeholder": "dc4ce43e-bc4f-4a93-b482-454f874421a8"
+                                },
+                                "align_recalibrated": {
+                                    "upload_placeholder": "c86ab143-a925-433c-bb13-030c0684365e"
+                                },
+                                "align_recalibrated_index": {
+                                    "upload_placeholder": "64991cf3-b1b9-4b4a-830d-4eade9ef1321"
+                                },
+                            },
+                            "hla": {
+                                "hla_final_result": {
+                                    "upload_placeholder": "95989077-49e4-44c6-8788-3b19357d3122"
+                                },
+                                "optitype_result": {
+                                    "upload_placeholder": "b5899d73-7373-4041-85f9-6cc4324be817"
+                                },
+                                "xhla_report_hla": {
+                                    "upload_placeholder": "3f3307bd-960e-4735-b831-f93d20fe8d37"
+                                },
+                            },
+                        },
+                    },
+                    {
+                        "run_id": "run_2",
+                        "error": {
+                            "upload_placeholder": "msi28d7a-fd96-4e75-b265-1590c703a303"
+                        },
+                        "tumor": {
+                            "cimac_id": "CTTTPP121.00",
+                            "alignment": {
+                                "align_sorted_dedup": {
+                                    "upload_placeholder": "e23d0858-eabb-4e9d-ad42-9bb4edadfd59"
+                                },
+                                "align_sorted_dedup_index": {
+                                    "upload_placeholder": "fa9a388b-d679-4a77-845f-2c4073425128"
+                                },
+                                "align_recalibrated": {
+                                    "upload_placeholder": "d187bcfe-b454-46a5-bf85-e2a2d5f7a9a5"
+                                },
+                                "align_recalibrated_index": {
+                                    "upload_placeholder": "ca2984c0-f7e6-470c-95ef-e4b33cbdea48"
+                                },
+                            },
+                            "hla": {
+                                "hla_final_result": {
+                                    "upload_placeholder": "86824763-fb9f-58b4-c7c4-8175759933f6"
+                                },
+                                "optitype_result": {
+                                    "upload_placeholder": "771d710e-f245-4d2b-8732-2774e26aec10"
+                                },
+                                "xhla_report_hla": {
+                                    "upload_placeholder": "5807aaa5-bafa-4fe5-89e9-73f9d734b971"
+                                },
+                            },
+                        },
+                    },
+                ],
+                "batch_id": "XYZ",
+                "excluded_samples": [
+                    {"cimac_id": "CTTTPP111.00", "reason_excluded": "low coverage"},
+                    {"cimac_id": "CTTTPP122.00", "reason_excluded": "module failed"},
+                ],
+            }
+        },
+        "protocol_identifier": "test_prism_trial_id",
+    }
+    upload_entries = [
+        LocalFileUploadEntry(
+            local_path="gs://results/analysis/hlahd/CTTTPP111.00/result/CTTTPP111.00_final.result.txt",
+            gs_key="test_prism_trial_id/ctdna/run_1/analysis/tumor/CTTTPP111.00/hla_final_result.txt",
+            upload_placeholder="95989077-49e4-44c6-8788-3b19357d3122",
+            metadata_availability=False,
+            allow_empty=False,
+        ),
+        LocalFileUploadEntry(
+            local_path="gs://results/analysis/run_1_error.yaml",
+            gs_key="test_prism_trial_id/ctdna/run_1/analysis/error.yaml",
+            upload_placeholder="msi18d7a-fd96-4e75-b265-1590c703a303",
+            metadata_availability=False,
+            allow_empty=True,
+        ),
+        LocalFileUploadEntry(
+            local_path="gs://results/analysis/align/CTTTPP111.00/CTTTPP111.00_recalibrated.bam",
+            gs_key="test_prism_trial_id/ctdna/run_1/analysis/tumor/CTTTPP111.00/recalibrated.bam",
+            upload_placeholder="c86ab143-a925-433c-bb13-030c0684365e",
+            metadata_availability=False,
+            allow_empty=False,
+        ),
+        LocalFileUploadEntry(
+            local_path="gs://results/analysis/align/CTTTPP111.00/CTTTPP111.00_recalibrated.bam.bai",
+            gs_key="test_prism_trial_id/ctdna/run_1/analysis/tumor/CTTTPP111.00/recalibrated.bam.bai",
+            upload_placeholder="64991cf3-b1b9-4b4a-830d-4eade9ef1321",
+            metadata_availability=False,
+            allow_empty=False,
+        ),
+        LocalFileUploadEntry(
+            local_path="gs://results/analysis/align/CTTTPP111.00/CTTTPP111.00.sorted.dedup.bam",
+            gs_key="test_prism_trial_id/ctdna/run_1/analysis/tumor/CTTTPP111.00/sorted.dedup.bam",
+            upload_placeholder="3068ae50-3ce7-4b0c-ba56-f678233dd098",
+            metadata_availability=False,
+            allow_empty=False,
+        ),
+        LocalFileUploadEntry(
+            local_path="gs://results/analysis/align/CTTTPP111.00/CTTTPP111.00.sorted.dedup.bam.bai",
+            gs_key="test_prism_trial_id/ctdna/run_1/analysis/tumor/CTTTPP111.00/sorted.dedup.bam.bai",
+            upload_placeholder="dc4ce43e-bc4f-4a93-b482-454f874421a8",
+            metadata_availability=False,
+            allow_empty=False,
+        ),
+        LocalFileUploadEntry(
+            local_path="gs://results/analysis/optitype/CTTTPP111.00/CTTTPP111.00_result.tsv",
+            gs_key="test_prism_trial_id/ctdna/run_1/analysis/tumor/CTTTPP111.00/optitype_result.tsv",
+            upload_placeholder="b5899d73-7373-4041-85f9-6cc4324be817",
+            metadata_availability=False,
+            allow_empty=False,
+        ),
+        LocalFileUploadEntry(
+            local_path="gs://results/analysis/xhla/CTTTPP111.00/report-CTTTPP111.00-hla.json",
+            gs_key="test_prism_trial_id/ctdna/run_1/analysis/tumor/CTTTPP111.00/xhla_report_hla.json",
+            upload_placeholder="3f3307bd-960e-4735-b831-f93d20fe8d37",
+            metadata_availability=False,
+            allow_empty=False,
+        ),
+        LocalFileUploadEntry(
+            local_path="gs://results/analysis/align/CTTTPP121.00/CTTTPP121.00_recalibrated.bam",
+            gs_key="test_prism_trial_id/ctdna/run_2/analysis/tumor/CTTTPP121.00/recalibrated.bam",
+            upload_placeholder="d187bcfe-b454-46a5-bf85-e2a2d5f7a9a5",
+            metadata_availability=False,
+            allow_empty=False,
+        ),
+        LocalFileUploadEntry(
+            local_path="gs://results/analysis/align/CTTTPP121.00/CTTTPP121.00_recalibrated.bam.bai",
+            gs_key="test_prism_trial_id/ctdna/run_2/analysis/tumor/CTTTPP121.00/recalibrated.bam.bai",
+            upload_placeholder="ca2984c0-f7e6-470c-95ef-e4b33cbdea48",
+            metadata_availability=False,
+            allow_empty=False,
+        ),
+        LocalFileUploadEntry(
+            local_path="gs://results/analysis/run_2_error.yaml",
+            gs_key="test_prism_trial_id/ctdna/run_2/analysis/error.yaml",
+            upload_placeholder="msi28d7a-fd96-4e75-b265-1590c703a303",
+            metadata_availability=False,
+            allow_empty=True,
+        ),
+        LocalFileUploadEntry(
+            local_path="gs://results/analysis/hlahd/CTTTPP121.00/result/CTTTPP121.00_final.result.txt",
+            gs_key="test_prism_trial_id/ctdna/run_2/analysis/tumor/CTTTPP121.00/hla_final_result.txt",
+            upload_placeholder="86824763-fb9f-58b4-c7c4-8175759933f6",
+            metadata_availability=False,
+            allow_empty=False,
+        ),
+        LocalFileUploadEntry(
+            local_path="gs://results/analysis/align/CTTTPP121.00/CTTTPP121.00.sorted.dedup.bam",
+            gs_key="test_prism_trial_id/ctdna/run_2/analysis/tumor/CTTTPP121.00/sorted.dedup.bam",
+            upload_placeholder="e23d0858-eabb-4e9d-ad42-9bb4edadfd59",
+            metadata_availability=False,
+            allow_empty=False,
+        ),
+        LocalFileUploadEntry(
+            local_path="gs://results/analysis/align/CTTTPP121.00/CTTTPP121.00.sorted.dedup.bam.bai",
+            gs_key="test_prism_trial_id/ctdna/run_2/analysis/tumor/CTTTPP121.00/sorted.dedup.bam.bai",
+            upload_placeholder="fa9a388b-d679-4a77-845f-2c4073425128",
+            metadata_availability=False,
+            allow_empty=False,
+        ),
+        LocalFileUploadEntry(
+            local_path="gs://results/analysis/optitype/CTTTPP121.00/CTTTPP121.00_result.tsv",
+            gs_key="test_prism_trial_id/ctdna/run_2/analysis/tumor/CTTTPP121.00/optitype_result.tsv",
+            upload_placeholder="771d710e-f245-4d2b-8732-2774e26aec10",
+            metadata_availability=False,
+            allow_empty=False,
+        ),
+        LocalFileUploadEntry(
+            local_path="gs://results/analysis/xhla/CTTTPP121.00/report-CTTTPP121.00-hla.json",
+            gs_key="test_prism_trial_id/ctdna/run_2/analysis/tumor/CTTTPP121.00/xhla_report_hla.json",
+            upload_placeholder="5807aaa5-bafa-4fe5-89e9-73f9d734b971",
+            metadata_availability=False,
+            allow_empty=False,
+        ),
+    ]
+
+    cimac_ids = [
+        run["tumor"]["cimac_id"]
+        for run in prismify_patch["analysis"]["ctdna_analysis"]["runs"]
+    ] + [
+        sample["cimac_id"]
+        for sample in prismify_patch["analysis"]["ctdna_analysis"]["excluded_samples"]
+    ]
+    base_trial = get_test_trial(cimac_ids)
+
+    target_trial = copy_dict_with_branch(base_trial, prismify_patch, "analysis")
+
+    return PrismTestData(
+        upload_type,
+        prismify_args,
+        prismify_patch,
+        upload_entries,
+        base_trial,
+        target_trial,
+    )
+
+
+@analysis_data_generator
 def wes_tumor_only_analysis() -> PrismTestData:
     upload_type = "wes_tumor_only_analysis"
     prismify_args = get_prismify_args(upload_type)
     prismify_patch = {
         "analysis": {
             "wes_tumor_only_analysis": {
                 "runs": [
```

### Comparing `nci_cidc_schemas-0.26.29/tests/prism/cidc_test_data/assay_data.py` & `nci_cidc_schemas-0.26.32/tests/prism/cidc_test_data/assay_data.py`

 * *Files 2% similar despite different names*

```diff
@@ -3491,14 +3491,23 @@
                             },
                             "optimal_solution": {
                                 "upload_placeholder": "dbc2e076-2c89-4f07-a371-be39d80e7b47"
                             },
                             "other_solutions": {
                                 "upload_placeholder": "4c409c82-dff7-4f78-801c-0544b3e28d71"
                             },
+                            "on_premise_corrected_depth_file": {
+                                "upload_placeholder": "4c409c82-dff7-4f78-801c-11ddf"
+                            },
+                            "on_premise_parameters_file": {
+                                "upload_placeholder": "4c409c82-dff7-4f78-801c-33ssf"
+                            },
+                            "on_premise_rdata_file": {
+                                "upload_placeholder": "4c409c82-dff7-4f78-801c-222ssff"
+                            },
                             "fraction_cna_subclonal": 0.1,
                             "fraction_genome_subclonal": 0.2,
                             "gc_map_correction_mad": 0.04,
                             "subclone_fraction": 0.15,
                             "tumor_fraction": 0.25,
                             "tumor_ploidy": 2.599,
                         },
@@ -3518,14 +3527,23 @@
                             },
                             "optimal_solution": {
                                 "upload_placeholder": "289068fe-4c00-4a67-9a98-74223266c1e0"
                             },
                             "other_solutions": {
                                 "upload_placeholder": "f63988e4-948d-4d55-8822-600754d5259c"
                             },
+                            "on_premise_corrected_depth_file": {
+                                "upload_placeholder": "4c409c82-dff7-4f78-801c-1222"
+                            },
+                            "on_premise_parameters_file": {
+                                "upload_placeholder": "4c409c82-dff7-4f78-801c-111"
+                            },
+                            "on_premise_rdata_file": {
+                                "upload_placeholder": "4c409c82-dff7-4f78-801c-323fff"
+                            },
                             "fraction_cna_subclonal": 0.2,
                             "fraction_genome_subclonal": 0.3,
                             "gc_map_correction_mad": 0.05,
                             "subclone_fraction": 0.16,
                             "tumor_fraction": 0.26,
                             "tumor_ploidy": 2.699,
                             "comments": "note about sample 2",
@@ -3575,14 +3593,56 @@
             local_path="CTTTPP111.00/outSolutions.zip",
             upload_placeholder="4c409c82-dff7-4f78-801c-0544b3e28d71",
             gs_key="test_prism_trial_id/ctdna/test_batch/CTTTPP111.00/other_solutions.zip",
             metadata_availability=False,
             allow_empty=False,
         ),
         LocalFileUploadEntry(
+            local_path="CTTTPP111.00/OnPrem.correctedDepth.txt",
+            upload_placeholder="4c409c82-dff7-4f78-801c-11ddf",
+            gs_key="test_prism_trial_id/ctdna/test_batch/CTTTPP111.00/OnPrem.correctedDepth.txt",
+            metadata_availability=False,
+            allow_empty=False,
+        ),
+        LocalFileUploadEntry(
+            local_path="CTTTPP121.00/OnPrem.correctedDepth.txt",
+            upload_placeholder="4c409c82-dff7-4f78-801c-1222",
+            gs_key="test_prism_trial_id/ctdna/test_batch/CTTTPP121.00/OnPrem.correctedDepth.txt",
+            metadata_availability=False,
+            allow_empty=False,
+        ),
+        LocalFileUploadEntry(
+            local_path="CTTTPP111.00/OnPrem.params.txt",
+            upload_placeholder="4c409c82-dff7-4f78-801c-33ssf",
+            gs_key="test_prism_trial_id/ctdna/test_batch/CTTTPP111.00/OnPrem.params.txt",
+            metadata_availability=False,
+            allow_empty=False,
+        ),
+        LocalFileUploadEntry(
+            local_path="CTTTPP121.00/OnPrem.params.txt",
+            upload_placeholder="4c409c82-dff7-4f78-801c-111",
+            gs_key="test_prism_trial_id/ctdna/test_batch/CTTTPP121.00/OnPrem.params.txt",
+            metadata_availability=False,
+            allow_empty=False,
+        ),
+        LocalFileUploadEntry(
+            local_path="CTTTPP111.00/OnPrem.RData",
+            upload_placeholder="4c409c82-dff7-4f78-801c-222ssff",
+            gs_key="test_prism_trial_id/ctdna/test_batch/CTTTPP111.00/OnPrem.RData",
+            metadata_availability=False,
+            allow_empty=False,
+        ),
+        LocalFileUploadEntry(
+            local_path="CTTTPP121.00/OnPrem.RData",
+            upload_placeholder="4c409c82-dff7-4f78-801c-323fff",
+            gs_key="test_prism_trial_id/ctdna/test_batch/CTTTPP121.00/OnPrem.RData",
+            metadata_availability=False,
+            allow_empty=False,
+        ),
+        LocalFileUploadEntry(
             local_path="CTTTPP121_00.bam",
             upload_placeholder="189068fe-4c00-4a67-9a98-74223266c1e0",
             gs_key="test_prism_trial_id/ctdna/test_batch/CTTTPP121.00/demultiplexed.bam",
             metadata_availability=False,
             allow_empty=False,
         ),
         LocalFileUploadEntry(
```

### Comparing `nci_cidc_schemas-0.26.29/tests/prism/cidc_test_data/manifest_data.py` & `nci_cidc_schemas-0.26.32/tests/prism/cidc_test_data/manifest_data.py`

 * *Files identical despite different names*

### Comparing `nci_cidc_schemas-0.26.29/tests/prism/cidc_test_data/utils.py` & `nci_cidc_schemas-0.26.32/tests/prism/cidc_test_data/utils.py`

 * *Files identical despite different names*

### Comparing `nci_cidc_schemas-0.26.29/tests/prism/schema/test_schema.json` & `nci_cidc_schemas-0.26.32/tests/prism/schema/test_schema.json`

 * *Files identical despite different names*

### Comparing `nci_cidc_schemas-0.26.29/tests/prism/test_cidc_data_model.py` & `nci_cidc_schemas-0.26.32/tests/prism/test_cidc_data_model.py`

 * *Files identical despite different names*

### Comparing `nci_cidc_schemas-0.26.29/tests/prism/test_core.py` & `nci_cidc_schemas-0.26.32/tests/prism/test_core.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 """Tests for generic prismification functionality.
 
 TODO: some of these tests currently use the CIDC data model, but they 
 should probably use an unrelated test data model instead.
 """
+
 import os
 import base64
 import hmac
 from unittest.mock import MagicMock
 from collections import namedtuple
 
 import pytest
```

### Comparing `nci_cidc_schemas-0.26.29/tests/prism/test_extra_metadata.py` & `nci_cidc_schemas-0.26.32/tests/prism/test_extra_metadata.py`

 * *Files identical despite different names*

### Comparing `nci_cidc_schemas-0.26.29/tests/prism/test_merger.py` & `nci_cidc_schemas-0.26.32/tests/prism/test_merger.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """Tests for generic merging functionality."""
+
 from copy import deepcopy
 from uuid import uuid4
 from unittest.mock import MagicMock
 
 import pytest
 from jsonmerge import Merger
 
@@ -18,14 +19,15 @@
     single_npx_metadata,
     combined_npx_metadata,
     elisa_metadata_1,
     clinical_file_path_1_csv,
     clinical_metadata_1,
 )
 
+
 #### MERGE STRATEGY TESTS ####
 def test_throw_on_mismatch():
     """Test the custom ThrowOnMismatch merge strategy"""
     schema = {
         "type": "object",
         "properties": {
             "participants": {
```

### Comparing `nci_cidc_schemas-0.26.29/tests/prism/test_pipelines.py` & `nci_cidc_schemas-0.26.32/tests/prism/test_pipelines.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """Tests for pipeline config generation."""
+
 from collections import defaultdict
 import os
 import copy
 from tempfile import NamedTemporaryFile
 from typing import Dict, List, Tuple, Union
 import openpyxl
 import pandas as pd
@@ -88,17 +89,17 @@
 
 def get_patch_for_staging(template_type: str) -> dict:
     preassay_xlsx_path = os.path.join(
         TEMPLATE_EXAMPLES_DIR, template_type + "_template.xlsx"
     )
     preassay_xlsx, _ = XlTemplateReader.from_excel(preassay_xlsx_path)
     preassay_template = Template.from_type(template_type)
-    prism_res: Tuple[
-        dict, List[LocalFileUploadEntry], List[Union[Exception, str]]
-    ] = core.prismify(preassay_xlsx, preassay_template)
+    prism_res: Tuple[dict, List[LocalFileUploadEntry], List[Union[Exception, str]]] = (
+        core.prismify(preassay_xlsx, preassay_template)
+    )
 
     patch_with_artifacts: dict = prism_patch_stage_artifacts(prism_res, template_type)
     return patch_with_artifacts
 
 
 def stage_assay(template_type: str, full_ct: dict) -> dict:
     patch_with_artifacts = get_patch_for_staging(template_type)
@@ -327,17 +328,17 @@
             "CTTTPP515.00,On_Treatment,,,,,\n"
             "CTTTPP516.00,On_Treatment,,,,,\n"
             "CTTTPP517.00,On_Treatment,,TRUE,,,"
         )
 
     # only generated for pairing manifest
     if "pairing" in template.type:
-        all_tumor_cimac_ids: List[
-            str
-        ] = []  # to make sure all are caught across configs
+        all_tumor_cimac_ids: List[str] = (
+            []
+        )  # to make sure all are caught across configs
         for fname, conf in res.items():
             # check the ingestion template excels
             if "template" in fname:
                 # openpyxl needs to file to have an .xlsx extension to open it
                 with NamedTemporaryFile(suffix=".xlsx") as tmp:
                     tmp.write(conf)
                     tmp.seek(0)
```

### Comparing `nci_cidc_schemas-0.26.29/tests/test_artifacts.py` & `nci_cidc_schemas-0.26.32/tests/test_artifacts.py`

 * *Files identical despite different names*

### Comparing `nci_cidc_schemas-0.26.29/tests/test_assays.py` & `nci_cidc_schemas-0.26.32/tests/test_assays.py`

 * *Files 1% similar despite different names*

```diff
@@ -549,26 +549,33 @@
     # set up BAM and BAI
     bam = ARTIFACT_OBJ.copy()
     bam["data_format"] = "BAM"
     bai = ARTIFACT_OBJ.copy()
     bai["data_format"] = "BAM.BAI"
     pdf = ARTIFACT_OBJ.copy()
     pdf["data_format"] = "PDF"
+    txt = ARTIFACT_OBJ.copy()
+    txt["data_format"] = "TEXT"
+    rdata = ARTIFACT_OBJ.copy()
+    rdata["data_format"] = "RDATA"
     zip = ARTIFACT_OBJ.copy()
     zip["data_format"] = "ZIP"
 
     # create the record
     record = {
         "cimac_id": "CTTTPPPSA.00",
         "demultiplexed_bam": bam,
         "demultiplexed_bam_index": bai,
         "genome-wide_plots": pdf,
         "bias_qc_plots": pdf,
         "optimal_solution": zip,
         "other_solutions": zip,
+        "on_premise_corrected_depth_file": txt,
+        "on_premise_parameters_file": txt,
+        "on_premise_rdata_file": rdata,
         "fraction_cna_subclonal": 0.1,
         "fraction_genome_subclonal": 0.2,
         "gc_map_correction_mad": 0.04,
         "subclone_fraction": 0.15,
         "tumor_fraction": 0.25,
         "tumor_ploidy": 2.5,
     }
```

### Comparing `nci_cidc_schemas-0.26.29/tests/test_clinicaltrial_examples.py` & `nci_cidc_schemas-0.26.32/tests/test_clinicaltrial_examples.py`

 * *Files identical despite different names*

### Comparing `nci_cidc_schemas-0.26.29/tests/test_json_validation.py` & `nci_cidc_schemas-0.26.32/tests/test_json_validation.py`

 * *Files identical despite different names*

### Comparing `nci_cidc_schemas-0.26.29/tests/test_migrations.py` & `nci_cidc_schemas-0.26.32/tests/test_migrations.py`

 * *Files identical despite different names*

### Comparing `nci_cidc_schemas-0.26.29/tests/test_schemas.py` & `nci_cidc_schemas-0.26.32/tests/test_schemas.py`

 * *Files identical despite different names*

### Comparing `nci_cidc_schemas-0.26.29/tests/test_strict_meta_schema.py` & `nci_cidc_schemas-0.26.32/tests/test_strict_meta_schema.py`

 * *Files identical despite different names*

### Comparing `nci_cidc_schemas-0.26.29/tests/test_template.py` & `nci_cidc_schemas-0.26.32/tests/test_template.py`

 * *Files 3% similar despite different names*

```diff
@@ -645,7 +645,18 @@
     good_wes_tumor_only = json.load(
         open(os.path.join(test_dir, "wes_tumor_only_analysis_template.json"))
     )
     new_wes_tumor_only = json.load(
         open(tmpdir.join("wes_tumor_only_analysis_template.json"))
     )
     assert DeepDiff(good_wes_tumor_only, new_wes_tumor_only) == {}
+
+
+# TODO update ./cidc_ngs_pipeline_api/output_API.schema.json first before enable it
+# def test_generate_analysis_template_schemas_ctdna(tmpdir):
+#     generate_analysis_template_schemas(
+#         tmpdir.strpath, lambda file: f"{file}_analysis_template.json"
+#     )
+#     test_dir = os.path.join(TEST_SCHEMA_DIR, "target-templates")
+#     good_ctdna = json.load(open(os.path.join(test_dir, "ctdna_analysis_template.json")))
+#     new_ctdna = json.load(open(tmpdir.join("ctdna_analysis_template.json")))
+#     assert DeepDiff(good_ctdna, new_ctdna) == {}
```

### Comparing `nci_cidc_schemas-0.26.29/tests/test_template_reader.py` & `nci_cidc_schemas-0.26.32/tests/test_template_reader.py`

 * *Files identical despite different names*

### Comparing `nci_cidc_schemas-0.26.29/tests/test_template_writer.py` & `nci_cidc_schemas-0.26.32/tests/test_template_writer.py`

 * *Files identical despite different names*

### Comparing `nci_cidc_schemas-0.26.29/tests/test_templates.py` & `nci_cidc_schemas-0.26.32/tests/test_templates.py`

 * *Files 4% similar despite different names*

```diff
@@ -104,24 +104,22 @@
         assert name in generated.grouped_rows, error(
             f"missing worksheet {name} in generated template"
         )
         gen_ws = generated.grouped_rows[name]
         ref_ws = reference.grouped_rows[name]
 
         # Compare preamble rows
-        for (gen_row, ref_row) in zip(
-            gen_ws[RowType.PREAMBLE], ref_ws[RowType.PREAMBLE]
-        ):
+        for gen_row, ref_row in zip(gen_ws[RowType.PREAMBLE], ref_ws[RowType.PREAMBLE]):
             gen_key, ref_key = gen_row.values[0], ref_row.values[0]
             assert gen_key.lower() == ref_key.lower(), error(
                 f"preamble: generated template had key {gen_key} where reference had {ref_key}"
             )
 
         assert len(gen_ws[RowType.HEADER]) == len(ref_ws[RowType.HEADER])
         for gen_headers, ref_headers in zip(
             gen_ws[RowType.HEADER], ref_ws[RowType.HEADER]
         ):
             # Compare data headers
-            for (gen_h, ref_h) in zip(gen_headers.values, ref_headers.values):
+            for gen_h, ref_h in zip(gen_headers.values, ref_headers.values):
                 assert (gen_h and gen_h.lower()) == (ref_h and ref_h.lower()), error(
                     f"data: generated template had header {gen_h!r} where reference had {ref_h!r}"
                 )
```

### Comparing `nci_cidc_schemas-0.26.29/tests/test_trial_core.py` & `nci_cidc_schemas-0.26.32/tests/test_trial_core.py`

 * *Files identical despite different names*

### Comparing `nci_cidc_schemas-0.26.29/tests/test_unprism.py` & `nci_cidc_schemas-0.26.32/tests/test_unprism.py`

 * *Files 1% similar despite different names*

```diff
@@ -255,15 +255,15 @@
         "cell_counts_profiling": {
             "B Cell (CD27-) CD1chi CD38hi": "138hi",
             "B Cell (CD27-) CD1chi CD38lo": "138lo",
         },
     }
 
     def fetch_artifact(url: str, as_string: bool) -> StringIO:
-        for (ftype, data) in artifact_format_specific_data.items():
+        for ftype, data in artifact_format_specific_data.items():
             if ftype in url:
                 csv = '"","CellSubset","N"\n'
                 csv += "\n".join(
                     f'"{i}","{k}",{v}' for i, (k, v) in enumerate(data.items())
                 )
 
                 return StringIO(csv)
```

### Comparing `nci_cidc_schemas-0.26.29/tests/test_util.py` & `nci_cidc_schemas-0.26.32/tests/test_util.py`

 * *Files identical despite different names*

### Comparing `nci_cidc_schemas-0.26.29/tests/utils/test_template_generator.py` & `nci_cidc_schemas-0.26.32/tests/utils/test_template_generator.py`

 * *Files identical despite different names*

