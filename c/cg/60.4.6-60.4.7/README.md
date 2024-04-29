# Comparing `tmp/cg-60.4.6.tar.gz` & `tmp/cg-60.4.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cg-60.4.6.tar", max compression
+gzip compressed data, was "cg-60.4.7.tar", max compression
```

## Comparing `cg-60.4.6.tar` & `cg-60.4.7.tar`

### file list

```diff
@@ -1,1318 +1,1320 @@
--rw-r--r--   0        0        0     2686 2024-04-29 07:40:13.698239 cg-60.4.6/README.md
--rw-r--r--   0        0        0       40 2024-04-29 07:40:13.702239 cg-60.4.6/cg/__init__.py
--rw-r--r--   0        0        0      315 2024-04-29 07:40:13.702239 cg-60.4.6/cg/apps/__init__.py
--rw-r--r--   0        0        0       27 2024-04-29 07:40:13.702239 cg-60.4.6/cg/apps/coverage/__init__.py
--rw-r--r--   0        0        0     2940 2024-04-29 07:40:13.702239 cg-60.4.6/cg/apps/coverage/api.py
--rw-r--r--   0        0        0       56 2024-04-29 07:40:13.702239 cg-60.4.6/cg/apps/crunchy/__init__.py
--rw-r--r--   0        0        0    12783 2024-04-29 07:40:13.702239 cg-60.4.6/cg/apps/crunchy/crunchy.py
--rw-r--r--   0        0        0     4502 2024-04-29 07:40:13.702239 cg-60.4.6/cg/apps/crunchy/files.py
--rw-r--r--   0        0        0      430 2024-04-29 07:40:13.702239 cg-60.4.6/cg/apps/crunchy/models.py
--rw-r--r--   0        0        0      910 2024-04-29 07:40:13.702239 cg-60.4.6/cg/apps/crunchy/sbatch.py
--rw-r--r--   0        0        0        0 2024-04-29 07:40:13.702239 cg-60.4.6/cg/apps/demultiplex/__init__.py
--rw-r--r--   0        0        0    11299 2024-04-29 07:40:13.702239 cg-60.4.6/cg/apps/demultiplex/demultiplex_api.py
--rw-r--r--   0        0        0        0 2024-04-29 07:40:13.702239 cg-60.4.6/cg/apps/demultiplex/sample_sheet/__init__.py
--rw-r--r--   0        0        0    11227 2024-04-29 07:40:13.702239 cg-60.4.6/cg/apps/demultiplex/sample_sheet/api.py
--rw-r--r--   0        0        0     2183 2024-04-29 07:40:13.702239 cg-60.4.6/cg/apps/demultiplex/sample_sheet/index.py
--rw-r--r--   0        0        0     7341 2024-04-29 07:40:13.702239 cg-60.4.6/cg/apps/demultiplex/sample_sheet/override_cycles_validator.py
--rw-r--r--   0        0        0     3188 2024-04-29 07:40:13.702239 cg-60.4.6/cg/apps/demultiplex/sample_sheet/read_sample_sheet.py
--rw-r--r--   0        0        0     7071 2024-04-29 07:40:13.702239 cg-60.4.6/cg/apps/demultiplex/sample_sheet/sample_models.py
--rw-r--r--   0        0        0     6076 2024-04-29 07:40:13.702239 cg-60.4.6/cg/apps/demultiplex/sample_sheet/sample_sheet_creator.py
--rw-r--r--   0        0        0     1372 2024-04-29 07:40:13.702239 cg-60.4.6/cg/apps/demultiplex/sample_sheet/sample_sheet_models.py
--rw-r--r--   0        0        0     8092 2024-04-29 07:40:13.702239 cg-60.4.6/cg/apps/demultiplex/sample_sheet/sample_sheet_validator.py
--rw-r--r--   0        0        0      824 2024-04-29 07:40:13.702239 cg-60.4.6/cg/apps/demultiplex/sample_sheet/validators.py
--rw-r--r--   0        0        0      677 2024-04-29 07:40:13.702239 cg-60.4.6/cg/apps/demultiplex/sbatch.py
--rw-r--r--   0        0        0        0 2024-04-29 07:40:13.702239 cg-60.4.6/cg/apps/downsample/__init__.py
--rw-r--r--   0        0        0     6160 2024-04-29 07:40:13.702239 cg-60.4.6/cg/apps/downsample/downsample.py
--rw-r--r--   0        0        0     2125 2024-04-29 07:40:13.702239 cg-60.4.6/cg/apps/downsample/utils.py
--rw-r--r--   0        0        0      298 2024-04-29 07:40:13.702239 cg-60.4.6/cg/apps/environ.py
--rw-r--r--   0        0        0     1741 2024-04-29 07:40:13.702239 cg-60.4.6/cg/apps/gens.py
--rw-r--r--   0        0        0     3419 2024-04-29 07:40:13.702239 cg-60.4.6/cg/apps/gt.py
--rw-r--r--   0        0        0        0 2024-04-29 07:40:13.702239 cg-60.4.6/cg/apps/hermes/__init__.py
--rw-r--r--   0        0        0     2249 2024-04-29 07:40:13.702239 cg-60.4.6/cg/apps/hermes/hermes_api.py
--rw-r--r--   0        0        0     1298 2024-04-29 07:40:13.702239 cg-60.4.6/cg/apps/hermes/models.py
--rw-r--r--   0        0        0        0 2024-04-29 07:40:13.702239 cg-60.4.6/cg/apps/housekeeper/__init__.py
--rw-r--r--   0        0        0    30395 2024-04-29 07:40:13.702239 cg-60.4.6/cg/apps/housekeeper/hk.py
--rw-r--r--   0        0        0      326 2024-04-29 07:40:13.702239 cg-60.4.6/cg/apps/housekeeper/models.py
--rw-r--r--   0        0        0       32 2024-04-29 07:40:13.702239 cg-60.4.6/cg/apps/invoice/__init__.py
--rw-r--r--   0        0        0     4804 2024-04-29 07:40:13.702239 cg-60.4.6/cg/apps/invoice/render.py
--rw-r--r--   0        0        0   113467 2024-04-29 07:40:13.702239 cg-60.4.6/cg/apps/invoice/templates/KI_pool_invoice.xlsx
--rw-r--r--   0        0        0    75562 2024-04-29 07:40:13.702239 cg-60.4.6/cg/apps/invoice/templates/KI_sample_invoice.xlsx
--rw-r--r--   0        0        0   113512 2024-04-29 07:40:13.702239 cg-60.4.6/cg/apps/invoice/templates/KTH_pool_invoice.xlsx
--rw-r--r--   0        0        0    75459 2024-04-29 07:40:13.702239 cg-60.4.6/cg/apps/invoice/templates/KTH_sample_invoice.xlsx
--rw-r--r--   0        0        0       25 2024-04-29 07:40:13.702239 cg-60.4.6/cg/apps/lims/__init__.py
--rw-r--r--   0        0        0    18873 2024-04-29 07:40:13.702239 cg-60.4.6/cg/apps/lims/api.py
--rw-r--r--   0        0        0     2652 2024-04-29 07:40:13.702239 cg-60.4.6/cg/apps/lims/batch.py
--rw-r--r--   0        0        0     8129 2024-04-29 07:40:13.702239 cg-60.4.6/cg/apps/lims/order.py
--rw-r--r--   0        0        0     3118 2024-04-29 07:40:13.702239 cg-60.4.6/cg/apps/lims/sample_sheet.py
--rw-r--r--   0        0        0     4866 2024-04-29 07:40:13.702239 cg-60.4.6/cg/apps/loqus.py
--rw-r--r--   0        0        0       35 2024-04-29 07:40:13.706239 cg-60.4.6/cg/apps/madeline/__init__.py
--rw-r--r--   0        0        0     3213 2024-04-29 07:40:13.706239 cg-60.4.6/cg/apps/madeline/api.py
--rw-r--r--   0        0        0       23 2024-04-29 07:40:13.706239 cg-60.4.6/cg/apps/mip/__init__.py
--rw-r--r--   0        0        0     3564 2024-04-29 07:40:13.706239 cg-60.4.6/cg/apps/mip/confighandler.py
--rw-r--r--   0        0        0     2207 2024-04-29 07:40:13.706239 cg-60.4.6/cg/apps/mutacc_auto.py
--rw-r--r--   0        0        0        0 2024-04-29 07:40:13.706239 cg-60.4.6/cg/apps/orderform/__init__.py
--rw-r--r--   0        0        0     9498 2024-04-29 07:40:13.706239 cg-60.4.6/cg/apps/orderform/excel_orderform_parser.py
--rw-r--r--   0        0        0     3051 2024-04-29 07:40:13.706239 cg-60.4.6/cg/apps/orderform/json_orderform_parser.py
--rw-r--r--   0        0        0     6419 2024-04-29 07:40:13.706239 cg-60.4.6/cg/apps/orderform/orderform_parser.py
--rw-r--r--   0        0        0      252 2024-04-29 07:40:13.706239 cg-60.4.6/cg/apps/orderform/utils.py
--rw-r--r--   0        0        0     2537 2024-04-29 07:40:13.706239 cg-60.4.6/cg/apps/osticket.py
--rw-r--r--   0        0        0        0 2024-04-29 07:40:13.706239 cg-60.4.6/cg/apps/scout/__init__.py
--rw-r--r--   0        0        0     3177 2024-04-29 07:40:13.706239 cg-60.4.6/cg/apps/scout/scout_export.py
--rw-r--r--   0        0        0    11108 2024-04-29 07:40:13.706239 cg-60.4.6/cg/apps/scout/scoutapi.py
--rw-r--r--   0        0        0      444 2024-04-29 07:40:13.706239 cg-60.4.6/cg/apps/scout/validators.py
--rw-r--r--   0        0        0        0 2024-04-29 07:40:13.706239 cg-60.4.6/cg/apps/sequencing_metrics_parser/__init__.py
--rw-r--r--   0        0        0     3457 2024-04-29 07:40:13.706239 cg-60.4.6/cg/apps/sequencing_metrics_parser/api.py
--rw-r--r--   0        0        0      923 2024-04-29 07:40:13.706239 cg-60.4.6/cg/apps/sequencing_metrics_parser/models.py
--rw-r--r--   0        0        0     6658 2024-04-29 07:40:13.706239 cg-60.4.6/cg/apps/sequencing_metrics_parser/parser.py
--rw-r--r--   0        0        0        0 2024-04-29 07:40:13.706239 cg-60.4.6/cg/apps/slurm/__init__.py
--rw-r--r--   0        0        0     1277 2024-04-29 07:40:13.706239 cg-60.4.6/cg/apps/slurm/sbatch.py
--rw-r--r--   0        0        0     3559 2024-04-29 07:40:13.706239 cg-60.4.6/cg/apps/slurm/slurm_api.py
--rw-r--r--   0        0        0       32 2024-04-29 07:40:13.706239 cg-60.4.6/cg/apps/tb/__init__.py
--rw-r--r--   0        0        0     7995 2024-04-29 07:40:13.706239 cg-60.4.6/cg/apps/tb/api.py
--rw-r--r--   0        0        0      152 2024-04-29 07:40:13.706239 cg-60.4.6/cg/apps/tb/dto/create_job_request.py
--rw-r--r--   0        0        0      250 2024-04-29 07:40:13.706239 cg-60.4.6/cg/apps/tb/dto/summary_response.py
--rw-r--r--   0        0        0     1305 2024-04-29 07:40:13.706239 cg-60.4.6/cg/apps/tb/models.py
--rw-r--r--   0        0        0      305 2024-04-29 07:40:13.706239 cg-60.4.6/cg/apps/tb/validators.py
--rw-r--r--   0        0        0        0 2024-04-29 07:40:13.706239 cg-60.4.6/cg/cli/__init__.py
--rw-r--r--   0        0        0    11558 2024-04-29 07:40:13.706239 cg-60.4.6/cg/cli/add.py
--rw-r--r--   0        0        0     2653 2024-04-29 07:40:13.706239 cg-60.4.6/cg/cli/archive.py
--rw-r--r--   0        0        0    10118 2024-04-29 07:40:13.706239 cg-60.4.6/cg/cli/backup.py
--rw-r--r--   0        0        0     3852 2024-04-29 07:40:13.706239 cg-60.4.6/cg/cli/base.py
--rw-r--r--   0        0        0    10506 2024-04-29 07:40:13.706239 cg-60.4.6/cg/cli/clean.py
--rw-r--r--   0        0        0        0 2024-04-29 07:40:13.706239 cg-60.4.6/cg/cli/compress/__init__.py
--rw-r--r--   0        0        0     2135 2024-04-29 07:40:13.706239 cg-60.4.6/cg/cli/compress/base.py
--rw-r--r--   0        0        0     6706 2024-04-29 07:40:13.706239 cg-60.4.6/cg/cli/compress/fastq.py
--rw-r--r--   0        0        0     8163 2024-04-29 07:40:13.706239 cg-60.4.6/cg/cli/compress/helpers.py
--rw-r--r--   0        0        0        0 2024-04-29 07:40:13.706239 cg-60.4.6/cg/cli/delete/__init__.py
--rw-r--r--   0        0        0      564 2024-04-29 07:40:13.706239 cg-60.4.6/cg/cli/delete/base.py
--rw-r--r--   0        0        0     4603 2024-04-29 07:40:13.706239 cg-60.4.6/cg/cli/delete/case.py
--rw-r--r--   0        0        0     1884 2024-04-29 07:40:13.706239 cg-60.4.6/cg/cli/delete/cases.py
--rw-r--r--   0        0        0     2633 2024-04-29 07:40:13.706239 cg-60.4.6/cg/cli/delete/observations.py
--rw-r--r--   0        0        0        0 2024-04-29 07:40:13.706239 cg-60.4.6/cg/cli/deliver/__init__.py
--rw-r--r--   0        0        0     6030 2024-04-29 07:40:13.706239 cg-60.4.6/cg/cli/deliver/base.py
--rw-r--r--   0        0        0        0 2024-04-29 07:40:13.706239 cg-60.4.6/cg/cli/demultiplex/__init__.py
--rw-r--r--   0        0        0      829 2024-04-29 07:40:13.706239 cg-60.4.6/cg/cli/demultiplex/base.py
--rw-r--r--   0        0        0     4905 2024-04-29 07:40:13.706239 cg-60.4.6/cg/cli/demultiplex/copy_novaseqx_demultiplex_data.py
--rw-r--r--   0        0        0     7726 2024-04-29 07:40:13.706239 cg-60.4.6/cg/cli/demultiplex/demux.py
--rw-r--r--   0        0        0     1473 2024-04-29 07:40:13.706239 cg-60.4.6/cg/cli/demultiplex/finish.py
--rw-r--r--   0        0        0     3119 2024-04-29 07:40:13.706239 cg-60.4.6/cg/cli/demultiplex/sample_sheet.py
--rw-r--r--   0        0        0     2995 2024-04-29 07:40:13.706239 cg-60.4.6/cg/cli/downsample.py
--rw-r--r--   0        0        0        0 2024-04-29 07:40:13.706239 cg-60.4.6/cg/cli/generate/__init__.py
--rw-r--r--   0        0        0      356 2024-04-29 07:40:13.706239 cg-60.4.6/cg/cli/generate/base.py
--rw-r--r--   0        0        0        0 2024-04-29 07:40:13.706239 cg-60.4.6/cg/cli/generate/report/__init__.py
--rw-r--r--   0        0        0     4636 2024-04-29 07:40:13.706239 cg-60.4.6/cg/cli/generate/report/base.py
--rw-r--r--   0        0        0      854 2024-04-29 07:40:13.706239 cg-60.4.6/cg/cli/generate/report/options.py
--rw-r--r--   0        0        0     5340 2024-04-29 07:40:13.706239 cg-60.4.6/cg/cli/generate/report/utils.py
--rw-r--r--   0        0        0     8327 2024-04-29 07:40:13.706239 cg-60.4.6/cg/cli/get.py
--rw-r--r--   0        0        0        0 2024-04-29 07:40:13.706239 cg-60.4.6/cg/cli/set/__init__.py
--rw-r--r--   0        0        0     9856 2024-04-29 07:40:13.706239 cg-60.4.6/cg/cli/set/base.py
--rw-r--r--   0        0        0     4384 2024-04-29 07:40:13.706239 cg-60.4.6/cg/cli/set/case.py
--rw-r--r--   0        0        0     2595 2024-04-29 07:40:13.706239 cg-60.4.6/cg/cli/set/cases.py
--rw-r--r--   0        0        0        0 2024-04-29 07:40:13.706239 cg-60.4.6/cg/cli/store/__init__.py
--rw-r--r--   0        0        0     1093 2024-04-29 07:40:13.706239 cg-60.4.6/cg/cli/store/base.py
--rw-r--r--   0        0        0     6191 2024-04-29 07:40:13.706239 cg-60.4.6/cg/cli/store/store.py
--rw-r--r--   0        0        0     1761 2024-04-29 07:40:13.706239 cg-60.4.6/cg/cli/transfer.py
--rw-r--r--   0        0        0        1 2024-04-29 07:40:13.706239 cg-60.4.6/cg/cli/upload/__init__.py
--rw-r--r--   0        0        0     5706 2024-04-29 07:40:13.706239 cg-60.4.6/cg/cli/upload/base.py
--rw-r--r--   0        0        0     5503 2024-04-29 07:40:13.706239 cg-60.4.6/cg/cli/upload/clinical_delivery.py
--rw-r--r--   0        0        0     1175 2024-04-29 07:40:13.706239 cg-60.4.6/cg/cli/upload/coverage.py
--rw-r--r--   0        0        0     1528 2024-04-29 07:40:13.706239 cg-60.4.6/cg/cli/upload/delivery_report.py
--rw-r--r--   0        0        0     4022 2024-04-29 07:40:13.706239 cg-60.4.6/cg/cli/upload/fohm.py
--rw-r--r--   0        0        0     1463 2024-04-29 07:40:13.706239 cg-60.4.6/cg/cli/upload/genotype.py
--rw-r--r--   0        0        0     1885 2024-04-29 07:40:13.706239 cg-60.4.6/cg/cli/upload/gens.py
--rw-r--r--   0        0        0      584 2024-04-29 07:40:13.706239 cg-60.4.6/cg/cli/upload/gisaid.py
--rw-r--r--   0        0        0     2645 2024-04-29 07:40:13.706239 cg-60.4.6/cg/cli/upload/mutacc.py
--rw-r--r--   0        0        0       23 2024-04-29 07:40:13.706239 cg-60.4.6/cg/cli/upload/nipt/__init__.py
--rw-r--r--   0        0        0     3006 2024-04-29 07:40:13.706239 cg-60.4.6/cg/cli/upload/nipt/base.py
--rw-r--r--   0        0        0     2275 2024-04-29 07:40:13.706239 cg-60.4.6/cg/cli/upload/nipt/ftp.py
--rw-r--r--   0        0        0     1596 2024-04-29 07:40:13.706239 cg-60.4.6/cg/cli/upload/nipt/statina.py
--rw-r--r--   0        0        0      112 2024-04-29 07:40:13.706239 cg-60.4.6/cg/cli/upload/observations/__init__.py
--rw-r--r--   0        0        0     2672 2024-04-29 07:40:13.706239 cg-60.4.6/cg/cli/upload/observations/observations.py
--rw-r--r--   0        0        0     2904 2024-04-29 07:40:13.706239 cg-60.4.6/cg/cli/upload/observations/utils.py
--rw-r--r--   0        0        0     9970 2024-04-29 07:40:13.710239 cg-60.4.6/cg/cli/upload/scout.py
--rw-r--r--   0        0        0      650 2024-04-29 07:40:13.710239 cg-60.4.6/cg/cli/upload/utils.py
--rw-r--r--   0        0        0     1667 2024-04-29 07:40:13.710239 cg-60.4.6/cg/cli/upload/validate.py
--rw-r--r--   0        0        0      105 2024-04-29 07:40:13.710239 cg-60.4.6/cg/cli/utils.py
--rw-r--r--   0        0        0       18 2024-04-29 07:40:13.710239 cg-60.4.6/cg/cli/workflow/__init__.py
--rw-r--r--   0        0        0       22 2024-04-29 07:40:13.710239 cg-60.4.6/cg/cli/workflow/balsamic/__init__.py
--rw-r--r--   0        0        0     8925 2024-04-29 07:40:13.710239 cg-60.4.6/cg/cli/workflow/balsamic/base.py
--rw-r--r--   0        0        0     1980 2024-04-29 07:40:13.710239 cg-60.4.6/cg/cli/workflow/balsamic/options.py
--rw-r--r--   0        0        0      881 2024-04-29 07:40:13.710239 cg-60.4.6/cg/cli/workflow/balsamic/pon.py
--rw-r--r--   0        0        0     1162 2024-04-29 07:40:13.710239 cg-60.4.6/cg/cli/workflow/balsamic/qc.py
--rw-r--r--   0        0        0     1177 2024-04-29 07:40:13.710239 cg-60.4.6/cg/cli/workflow/balsamic/umi.py
--rw-r--r--   0        0        0     1342 2024-04-29 07:40:13.710239 cg-60.4.6/cg/cli/workflow/base.py
--rw-r--r--   0        0        0    12379 2024-04-29 07:40:13.710239 cg-60.4.6/cg/cli/workflow/commands.py
--rw-r--r--   0        0        0        0 2024-04-29 07:40:13.710239 cg-60.4.6/cg/cli/workflow/fastq/__init__.py
--rw-r--r--   0        0        0     1490 2024-04-29 07:40:13.710239 cg-60.4.6/cg/cli/workflow/fastq/base.py
--rw-r--r--   0        0        0     1787 2024-04-29 07:40:13.710239 cg-60.4.6/cg/cli/workflow/fastq/fastq_service.py
--rw-r--r--   0        0        0        0 2024-04-29 07:40:13.710239 cg-60.4.6/cg/cli/workflow/fluffy/__init__.py
--rw-r--r--   0        0        0     4177 2024-04-29 07:40:13.710239 cg-60.4.6/cg/cli/workflow/fluffy/base.py
--rw-r--r--   0        0        0       22 2024-04-29 07:40:13.710239 cg-60.4.6/cg/cli/workflow/jasen/__init__.py
--rw-r--r--   0        0        0      535 2024-04-29 07:40:13.710239 cg-60.4.6/cg/cli/workflow/jasen/base.py
--rw-r--r--   0        0        0       22 2024-04-29 07:40:13.710239 cg-60.4.6/cg/cli/workflow/microsalt/__init__.py
--rw-r--r--   0        0        0     7810 2024-04-29 07:40:13.710239 cg-60.4.6/cg/cli/workflow/microsalt/base.py
--rw-r--r--   0        0        0       22 2024-04-29 07:40:13.710239 cg-60.4.6/cg/cli/workflow/mip/__init__.py
--rw-r--r--   0        0        0     6596 2024-04-29 07:40:13.710239 cg-60.4.6/cg/cli/workflow/mip/base.py
--rw-r--r--   0        0        0     1268 2024-04-29 07:40:13.710239 cg-60.4.6/cg/cli/workflow/mip/options.py
--rw-r--r--   0        0        0       22 2024-04-29 07:40:13.710239 cg-60.4.6/cg/cli/workflow/mip_dna/__init__.py
--rw-r--r--   0        0        0     1013 2024-04-29 07:40:13.710239 cg-60.4.6/cg/cli/workflow/mip_dna/base.py
--rw-r--r--   0        0        0       22 2024-04-29 07:40:13.710239 cg-60.4.6/cg/cli/workflow/mip_rna/__init__.py
--rw-r--r--   0        0        0      916 2024-04-29 07:40:13.710239 cg-60.4.6/cg/cli/workflow/mip_rna/base.py
--rw-r--r--   0        0        0        0 2024-04-29 07:40:13.710239 cg-60.4.6/cg/cli/workflow/mutant/__init__.py
--rw-r--r--   0        0        0     3413 2024-04-29 07:40:13.710239 cg-60.4.6/cg/cli/workflow/mutant/base.py
--rw-r--r--   0        0        0     9010 2024-04-29 07:40:13.710239 cg-60.4.6/cg/cli/workflow/nf_analysis.py
--rw-r--r--   0        0        0       22 2024-04-29 07:40:13.710239 cg-60.4.6/cg/cli/workflow/raredisease/__init__.py
--rw-r--r--   0        0        0     2210 2024-04-29 07:40:13.710239 cg-60.4.6/cg/cli/workflow/raredisease/base.py
--rw-r--r--   0        0        0       22 2024-04-29 07:40:13.710239 cg-60.4.6/cg/cli/workflow/rnafusion/__init__.py
--rw-r--r--   0        0        0     1179 2024-04-29 07:40:13.710239 cg-60.4.6/cg/cli/workflow/rnafusion/base.py
--rw-r--r--   0        0        0       22 2024-04-29 07:40:13.710239 cg-60.4.6/cg/cli/workflow/taxprofiler/__init__.py
--rw-r--r--   0        0        0     1211 2024-04-29 07:40:13.710239 cg-60.4.6/cg/cli/workflow/taxprofiler/base.py
--rw-r--r--   0        0        0     1111 2024-04-29 07:40:13.710239 cg-60.4.6/cg/cli/workflow/tomte/base.py
--rw-r--r--   0        0        0        0 2024-04-29 07:40:13.710239 cg-60.4.6/cg/clients/__init__.py
--rw-r--r--   0        0        0     1363 2024-04-29 07:40:13.710239 cg-60.4.6/cg/clients/arnold/api.py
--rw-r--r--   0        0        0      160 2024-04-29 07:40:13.710239 cg-60.4.6/cg/clients/arnold/dto/create_case_request.py
--rw-r--r--   0        0        0      384 2024-04-29 07:40:13.710239 cg-60.4.6/cg/clients/arnold/exceptions.py
--rw-r--r--   0        0        0        0 2024-04-29 07:40:13.710239 cg-60.4.6/cg/clients/janus/__init__.py
--rw-r--r--   0        0        0     1246 2024-04-29 07:40:13.710239 cg-60.4.6/cg/clients/janus/api.py
--rw-r--r--   0        0        0        0 2024-04-29 07:40:13.710239 cg-60.4.6/cg/clients/janus/dto/__init__.py
--rw-r--r--   0        0        0      503 2024-04-29 07:40:13.710239 cg-60.4.6/cg/clients/janus/dto/create_qc_metrics_request.py
--rw-r--r--   0        0        0      420 2024-04-29 07:40:13.710239 cg-60.4.6/cg/clients/janus/exceptions.py
--rw-r--r--   0        0        0      937 2024-04-29 07:40:13.710239 cg-60.4.6/cg/constants/__init__.py
--rw-r--r--   0        0        0      253 2024-04-29 07:40:13.710239 cg-60.4.6/cg/constants/archiving.py
--rw-r--r--   0        0        0       35 2024-04-29 07:40:13.710239 cg-60.4.6/cg/constants/backup.py
--rw-r--r--   0        0        0      769 2024-04-29 07:40:13.710239 cg-60.4.6/cg/constants/bcl_convert_metrics.py
--rw-r--r--   0        0        0      469 2024-04-29 07:40:13.710239 cg-60.4.6/cg/constants/compression.py
--rw-r--r--   0        0        0     6613 2024-04-29 07:40:13.710239 cg-60.4.6/cg/constants/constants.py
--rw-r--r--   0        0        0     6033 2024-04-29 07:40:13.710239 cg-60.4.6/cg/constants/delivery.py
--rw-r--r--   0        0        0     7321 2024-04-29 07:40:13.710239 cg-60.4.6/cg/constants/demultiplexing.py
--rw-r--r--   0        0        0     1422 2024-04-29 07:40:13.710239 cg-60.4.6/cg/constants/encryption.py
--rw-r--r--   0        0        0      372 2024-04-29 07:40:13.710239 cg-60.4.6/cg/constants/extraction.py
--rw-r--r--   0        0        0     2157 2024-04-29 07:40:13.710239 cg-60.4.6/cg/constants/gene_panel.py
--rw-r--r--   0        0        0     6704 2024-04-29 07:40:13.710239 cg-60.4.6/cg/constants/housekeeper_tags.py
--rw-r--r--   0        0        0       95 2024-04-29 07:40:13.710239 cg-60.4.6/cg/constants/invoice.py
--rw-r--r--   0        0        0     5815 2024-04-29 07:40:13.710239 cg-60.4.6/cg/constants/lims.py
--rw-r--r--   0        0        0      743 2024-04-29 07:40:13.710239 cg-60.4.6/cg/constants/metrics.py
--rw-r--r--   0        0        0      231 2024-04-29 07:40:13.710239 cg-60.4.6/cg/constants/nanopore_files.py
--rw-r--r--   0        0        0      650 2024-04-29 07:40:13.710239 cg-60.4.6/cg/constants/nextflow.py
--rw-r--r--   0        0        0     1529 2024-04-29 07:40:13.710239 cg-60.4.6/cg/constants/nf_analysis.py
--rw-r--r--   0        0        0       19 2024-04-29 07:40:13.710239 cg-60.4.6/cg/constants/nipt.py
--rw-r--r--   0        0        0     2257 2024-04-29 07:40:13.710239 cg-60.4.6/cg/constants/observations.py
--rw-r--r--   0        0        0     1216 2024-04-29 07:40:13.710239 cg-60.4.6/cg/constants/orderforms.py
--rw-r--r--   0        0        0       96 2024-04-29 07:40:13.710239 cg-60.4.6/cg/constants/paths.py
--rw-r--r--   0        0        0      266 2024-04-29 07:40:13.710239 cg-60.4.6/cg/constants/pdc.py
--rw-r--r--   0        0        0      160 2024-04-29 07:40:13.710239 cg-60.4.6/cg/constants/pedigree.py
--rw-r--r--   0        0        0     1044 2024-04-29 07:40:13.710239 cg-60.4.6/cg/constants/priority.py
--rw-r--r--   0        0        0       79 2024-04-29 07:40:13.710239 cg-60.4.6/cg/constants/process.py
--rw-r--r--   0        0        0     5474 2024-04-29 07:40:13.710239 cg-60.4.6/cg/constants/report.py
--rw-r--r--   0        0        0      569 2024-04-29 07:40:13.710239 cg-60.4.6/cg/constants/sample_sources.py
--rw-r--r--   0        0        0     3111 2024-04-29 07:40:13.710239 cg-60.4.6/cg/constants/scout.py
--rw-r--r--   0        0        0     1669 2024-04-29 07:40:13.710239 cg-60.4.6/cg/constants/sequencing.py
--rw-r--r--   0        0        0      313 2024-04-29 07:40:13.710239 cg-60.4.6/cg/constants/slurm.py
--rw-r--r--   0        0        0      529 2024-04-29 07:40:13.710239 cg-60.4.6/cg/constants/subject.py
--rw-r--r--   0        0        0       55 2024-04-29 07:40:13.710239 cg-60.4.6/cg/constants/symbols.py
--rw-r--r--   0        0        0      435 2024-04-29 07:40:13.710239 cg-60.4.6/cg/constants/tb.py
--rw-r--r--   0        0        0      161 2024-04-29 07:40:13.710239 cg-60.4.6/cg/constants/time.py
--rw-r--r--   0        0        0     6639 2024-04-29 07:40:13.710239 cg-60.4.6/cg/exc.py
--rw-r--r--   0        0        0        0 2024-04-29 07:40:13.710239 cg-60.4.6/cg/io/__init__.py
--rw-r--r--   0        0        0     1037 2024-04-29 07:40:13.710239 cg-60.4.6/cg/io/api.py
--rw-r--r--   0        0        0      621 2024-04-29 07:40:13.710239 cg-60.4.6/cg/io/config.py
--rw-r--r--   0        0        0     2978 2024-04-29 07:40:13.710239 cg-60.4.6/cg/io/controller.py
--rw-r--r--   0        0        0     1763 2024-04-29 07:40:13.710239 cg-60.4.6/cg/io/csv.py
--rw-r--r--   0        0        0      210 2024-04-29 07:40:13.710239 cg-60.4.6/cg/io/gzip.py
--rw-r--r--   0        0        0      662 2024-04-29 07:40:13.710239 cg-60.4.6/cg/io/json.py
--rw-r--r--   0        0        0      525 2024-04-29 07:40:13.710239 cg-60.4.6/cg/io/png.py
--rw-r--r--   0        0        0     1094 2024-04-29 07:40:13.710239 cg-60.4.6/cg/io/txt.py
--rw-r--r--   0        0        0      552 2024-04-29 07:40:13.714239 cg-60.4.6/cg/io/validate_path.py
--rw-r--r--   0        0        0     1289 2024-04-29 07:40:13.714239 cg-60.4.6/cg/io/xml.py
--rw-r--r--   0        0        0     1153 2024-04-29 07:40:13.714239 cg-60.4.6/cg/io/yaml.py
--rw-r--r--   0        0        0      281 2024-04-29 07:40:13.714239 cg-60.4.6/cg/meta/__init__.py
--rw-r--r--   0        0        0        0 2024-04-29 07:40:13.714239 cg-60.4.6/cg/meta/archive/__init__.py
--rw-r--r--   0        0        0    15193 2024-04-29 07:40:13.714239 cg-60.4.6/cg/meta/archive/archive.py
--rw-r--r--   0        0        0        0 2024-04-29 07:40:13.714239 cg-60.4.6/cg/meta/archive/ddn/__init__.py
--rw-r--r--   0        0        0     1727 2024-04-29 07:40:13.714239 cg-60.4.6/cg/meta/archive/ddn/constants.py
--rw-r--r--   0        0        0    10852 2024-04-29 07:40:13.714239 cg-60.4.6/cg/meta/archive/ddn/ddn_data_flow_client.py
--rw-r--r--   0        0        0     3704 2024-04-29 07:40:13.714239 cg-60.4.6/cg/meta/archive/ddn/models.py
--rw-r--r--   0        0        0     1250 2024-04-29 07:40:13.714239 cg-60.4.6/cg/meta/archive/ddn/utils.py
--rw-r--r--   0        0        0     2024 2024-04-29 07:40:13.714239 cg-60.4.6/cg/meta/archive/models.py
--rw-r--r--   0        0        0        0 2024-04-29 07:40:13.714239 cg-60.4.6/cg/meta/backup/__init__.py
--rw-r--r--   0        0        0    17426 2024-04-29 07:40:13.714239 cg-60.4.6/cg/meta/backup/backup.py
--rw-r--r--   0        0        0     5397 2024-04-29 07:40:13.714239 cg-60.4.6/cg/meta/backup/pdc.py
--rw-r--r--   0        0        0        0 2024-04-29 07:40:13.714239 cg-60.4.6/cg/meta/clean/__init__.py
--rw-r--r--   0        0        0     3901 2024-04-29 07:40:13.714239 cg-60.4.6/cg/meta/clean/api.py
--rw-r--r--   0        0        0     7738 2024-04-29 07:40:13.714239 cg-60.4.6/cg/meta/clean/clean_flow_cells.py
--rw-r--r--   0        0        0     1841 2024-04-29 07:40:13.714239 cg-60.4.6/cg/meta/clean/clean_retrieved_spring_files.py
--rw-r--r--   0        0        0       34 2024-04-29 07:40:13.714239 cg-60.4.6/cg/meta/compress/__init__.py
--rw-r--r--   0        0        0    14557 2024-04-29 07:40:13.714239 cg-60.4.6/cg/meta/compress/compress.py
--rw-r--r--   0        0        0     4947 2024-04-29 07:40:13.714239 cg-60.4.6/cg/meta/compress/files.py
--rw-r--r--   0        0        0       77 2024-04-29 07:40:13.714239 cg-60.4.6/cg/meta/deliver/__init__.py
--rw-r--r--   0        0        0    14905 2024-04-29 07:40:13.714239 cg-60.4.6/cg/meta/deliver/deliver.py
--rw-r--r--   0        0        0     4502 2024-04-29 07:40:13.714239 cg-60.4.6/cg/meta/deliver/deliver_ticket.py
--rw-r--r--   0        0        0      904 2024-04-29 07:40:13.714239 cg-60.4.6/cg/meta/deliver/fastq_path_generator.py
--rw-r--r--   0        0        0        0 2024-04-29 07:40:13.714239 cg-60.4.6/cg/meta/delivery/__init__.py
--rw-r--r--   0        0        0     8458 2024-04-29 07:40:13.714239 cg-60.4.6/cg/meta/delivery/delivery.py
--rw-r--r--   0        0        0        0 2024-04-29 07:40:13.714239 cg-60.4.6/cg/meta/demultiplex/__init__.py
--rw-r--r--   0        0        0     2592 2024-04-29 07:40:13.714239 cg-60.4.6/cg/meta/demultiplex/combine_sequencing_metrics.py
--rw-r--r--   0        0        0     5719 2024-04-29 07:40:13.714239 cg-60.4.6/cg/meta/demultiplex/demux_post_processing.py
--rw-r--r--   0        0        0     4135 2024-04-29 07:40:13.714239 cg-60.4.6/cg/meta/demultiplex/files.py
--rw-r--r--   0        0        0     7777 2024-04-29 07:40:13.714239 cg-60.4.6/cg/meta/demultiplex/housekeeper_storage_functions.py
--rw-r--r--   0        0        0     6126 2024-04-29 07:40:13.714239 cg-60.4.6/cg/meta/demultiplex/status_db_storage_functions.py
--rw-r--r--   0        0        0    10690 2024-04-29 07:40:13.714239 cg-60.4.6/cg/meta/demultiplex/utils.py
--rw-r--r--   0        0        0     2855 2024-04-29 07:40:13.714239 cg-60.4.6/cg/meta/demultiplex/validation.py
--rw-r--r--   0        0        0        0 2024-04-29 07:40:13.714239 cg-60.4.6/cg/meta/encryption/__init__.py
--rw-r--r--   0        0        0    20271 2024-04-29 07:40:13.714239 cg-60.4.6/cg/meta/encryption/encryption.py
--rw-r--r--   0        0        0      537 2024-04-29 07:40:13.714239 cg-60.4.6/cg/meta/encryption/sbatch.py
--rw-r--r--   0        0        0    10922 2024-04-29 07:40:13.714239 cg-60.4.6/cg/meta/invoice.py
--rw-r--r--   0        0        0     2360 2024-04-29 07:40:13.714239 cg-60.4.6/cg/meta/meta.py
--rw-r--r--   0        0        0        0 2024-04-29 07:40:13.714239 cg-60.4.6/cg/meta/observations/__init__.py
--rw-r--r--   0        0        0     6008 2024-04-29 07:40:13.714239 cg-60.4.6/cg/meta/observations/balsamic_observations_api.py
--rw-r--r--   0        0        0     5277 2024-04-29 07:40:13.714239 cg-60.4.6/cg/meta/observations/mip_dna_observations_api.py
--rw-r--r--   0        0        0     5364 2024-04-29 07:40:13.714239 cg-60.4.6/cg/meta/observations/observations_api.py
--rw-r--r--   0        0        0       27 2024-04-29 07:40:13.714239 cg-60.4.6/cg/meta/orders/__init__.py
--rw-r--r--   0        0        0     3637 2024-04-29 07:40:13.714239 cg-60.4.6/cg/meta/orders/api.py
--rw-r--r--   0        0        0      121 2024-04-29 07:40:13.714239 cg-60.4.6/cg/meta/orders/balsamic_qc_submitter.py
--rw-r--r--   0        0        0      107 2024-04-29 07:40:13.714239 cg-60.4.6/cg/meta/orders/balsamic_submitter.py
--rw-r--r--   0        0        0      122 2024-04-29 07:40:13.714239 cg-60.4.6/cg/meta/orders/balsamic_umi_submitter.py
--rw-r--r--   0        0        0    15262 2024-04-29 07:40:13.714239 cg-60.4.6/cg/meta/orders/case_submitter.py
--rw-r--r--   0        0        0     6102 2024-04-29 07:40:13.714239 cg-60.4.6/cg/meta/orders/fastq_submitter.py
--rw-r--r--   0        0        0      105 2024-04-29 07:40:13.714239 cg-60.4.6/cg/meta/orders/fluffy_submitter.py
--rw-r--r--   0        0        0     1254 2024-04-29 07:40:13.714239 cg-60.4.6/cg/meta/orders/lims.py
--rw-r--r--   0        0        0     5782 2024-04-29 07:40:13.714239 cg-60.4.6/cg/meta/orders/metagenome_submitter.py
--rw-r--r--   0        0        0     6337 2024-04-29 07:40:13.714239 cg-60.4.6/cg/meta/orders/microbial_submitter.py
--rw-r--r--   0        0        0      123 2024-04-29 07:40:13.714239 cg-60.4.6/cg/meta/orders/microsalt_submitter.py
--rw-r--r--   0        0        0      105 2024-04-29 07:40:13.714239 cg-60.4.6/cg/meta/orders/mip_dna_submitter.py
--rw-r--r--   0        0        0      105 2024-04-29 07:40:13.714239 cg-60.4.6/cg/meta/orders/mip_rna_submitter.py
--rw-r--r--   0        0        0     7761 2024-04-29 07:40:13.714239 cg-60.4.6/cg/meta/orders/pool_submitter.py
--rw-r--r--   0        0        0      102 2024-04-29 07:40:13.714239 cg-60.4.6/cg/meta/orders/rml_submitter.py
--rw-r--r--   0        0        0      718 2024-04-29 07:40:13.714239 cg-60.4.6/cg/meta/orders/rnafusion_submitter.py
--rw-r--r--   0        0        0     1268 2024-04-29 07:40:13.714239 cg-60.4.6/cg/meta/orders/sars_cov_2_submitter.py
--rw-r--r--   0        0        0     1754 2024-04-29 07:40:13.714239 cg-60.4.6/cg/meta/orders/submitter.py
--rw-r--r--   0        0        0     7880 2024-04-29 07:40:13.714239 cg-60.4.6/cg/meta/orders/ticket_handler.py
--rw-r--r--   0        0        0     4105 2024-04-29 07:40:13.714239 cg-60.4.6/cg/meta/qc_metrics/collect_qc_metrics.py
--rw-r--r--   0        0        0        0 2024-04-29 07:40:13.714239 cg-60.4.6/cg/meta/report/__init__.py
--rw-r--r--   0        0        0     8168 2024-04-29 07:40:13.714239 cg-60.4.6/cg/meta/report/balsamic.py
--rw-r--r--   0        0        0      562 2024-04-29 07:40:13.714239 cg-60.4.6/cg/meta/report/balsamic_qc.py
--rw-r--r--   0        0        0      717 2024-04-29 07:40:13.714239 cg-60.4.6/cg/meta/report/balsamic_umi.py
--rw-r--r--   0        0        0     4171 2024-04-29 07:40:13.714239 cg-60.4.6/cg/meta/report/field_validators.py
--rw-r--r--   0        0        0     6620 2024-04-29 07:40:13.714239 cg-60.4.6/cg/meta/report/mip_dna.py
--rw-r--r--   0        0        0    18543 2024-04-29 07:40:13.714239 cg-60.4.6/cg/meta/report/report_api.py
--rw-r--r--   0        0        0     5625 2024-04-29 07:40:13.714239 cg-60.4.6/cg/meta/report/rnafusion.py
--rw-r--r--   0        0        0     1911 2024-04-29 07:40:13.714239 cg-60.4.6/cg/meta/report/templates/delivery-report.html
--rw-r--r--   0        0        0     4236 2024-04-29 07:40:13.718239 cg-60.4.6/cg/meta/report/templates/macros/data_analysis/data_analysis.html
--rw-r--r--   0        0        0     1049 2024-04-29 07:40:13.718239 cg-60.4.6/cg/meta/report/templates/macros/data_analysis/limitations.html
--rw-r--r--   0        0        0     3351 2024-04-29 07:40:13.718239 cg-60.4.6/cg/meta/report/templates/macros/data_analysis/qc_metrics/balsamic_qc_metrics.html
--rw-r--r--   0        0        0     1364 2024-04-29 07:40:13.718239 cg-60.4.6/cg/meta/report/templates/macros/data_analysis/qc_metrics/mip_dna_qc_metrics.html
--rw-r--r--   0        0        0      753 2024-04-29 07:40:13.718239 cg-60.4.6/cg/meta/report/templates/macros/data_analysis/qc_metrics/qc_metrics.html
--rw-r--r--   0        0        0     3284 2024-04-29 07:40:13.718239 cg-60.4.6/cg/meta/report/templates/macros/data_analysis/qc_metrics/rnafusion_qc_metrics.html
--rw-r--r--   0        0        0     3670 2024-04-29 07:40:13.718239 cg-60.4.6/cg/meta/report/templates/macros/data_analysis/qc_metrics/tomte_qc_metrics.html
--rw-r--r--   0        0        0     2332 2024-04-29 07:40:13.718239 cg-60.4.6/cg/meta/report/templates/macros/header.html
--rw-r--r--   0        0        0     2066 2024-04-29 07:40:13.718239 cg-60.4.6/cg/meta/report/templates/macros/order.html
--rw-r--r--   0        0        0     2243 2024-04-29 07:40:13.718239 cg-60.4.6/cg/meta/report/templates/macros/sample_prep.html
--rw-r--r--   0        0        0      472 2024-04-29 07:40:13.718239 cg-60.4.6/cg/meta/report/templates/macros/ticket_system.html
--rw-r--r--   0        0        0     1165 2024-04-29 07:40:13.718239 cg-60.4.6/cg/meta/report/templates/macros/uploaded_files/balsamic_uploaded_files.html
--rw-r--r--   0        0        0     1538 2024-04-29 07:40:13.718239 cg-60.4.6/cg/meta/report/templates/macros/uploaded_files/mip_dna_uploaded_files.html
--rw-r--r--   0        0        0      428 2024-04-29 07:40:13.718239 cg-60.4.6/cg/meta/report/templates/macros/uploaded_files/rnafusion_uploaded_files.html
--rw-r--r--   0        0        0     4266 2024-04-29 07:40:13.718239 cg-60.4.6/cg/meta/report/templates/macros/uploaded_files/uploaded_files.html
--rw-r--r--   0        0        0       80 2024-04-29 07:40:13.718239 cg-60.4.6/cg/meta/report/templates/partials/footer.html
--rw-r--r--   0        0        0      172 2024-04-29 07:40:13.718239 cg-60.4.6/cg/meta/report/templates/partials/signature.html
--rw-r--r--   0        0        0   232803 2024-04-29 07:40:13.718239 cg-60.4.6/cg/meta/report/templates/static/css/bootstrap.min.css
--rw-r--r--   0        0        0       33 2024-04-29 07:40:13.718239 cg-60.4.6/cg/meta/report/templates/static/css/custom.css
--rw-r--r--   0        0        0    30068 2024-04-29 07:40:13.718239 cg-60.4.6/cg/meta/report/templates/static/images/SWEDAC_logo.png
--rw-r--r--   0        0        0     3925 2024-04-29 07:40:13.718239 cg-60.4.6/cg/meta/report/tomte.py
--rw-r--r--   0        0        0       32 2024-04-29 07:40:13.718239 cg-60.4.6/cg/meta/rsync/__init__.py
--rw-r--r--   0        0        0    12291 2024-04-29 07:40:13.718239 cg-60.4.6/cg/meta/rsync/rsync_api.py
--rw-r--r--   0        0        0      387 2024-04-29 07:40:13.718239 cg-60.4.6/cg/meta/rsync/sbatch.py
--rw-r--r--   0        0        0        0 2024-04-29 07:40:13.718239 cg-60.4.6/cg/meta/tar/__init__.py
--rw-r--r--   0        0        0     1694 2024-04-29 07:40:13.718239 cg-60.4.6/cg/meta/tar/tar.py
--rw-r--r--   0        0        0       71 2024-04-29 07:40:13.718239 cg-60.4.6/cg/meta/transfer/__init__.py
--rw-r--r--   0        0        0    10016 2024-04-29 07:40:13.718239 cg-60.4.6/cg/meta/transfer/external_data.py
--rw-r--r--   0        0        0     5814 2024-04-29 07:40:13.718239 cg-60.4.6/cg/meta/transfer/lims.py
--rw-r--r--   0        0        0        0 2024-04-29 07:40:13.718239 cg-60.4.6/cg/meta/upload/__init__.py
--rw-r--r--   0        0        0        0 2024-04-29 07:40:13.718239 cg-60.4.6/cg/meta/upload/balsamic/__init__.py
--rw-r--r--   0        0        0     3107 2024-04-29 07:40:13.718239 cg-60.4.6/cg/meta/upload/balsamic/balsamic.py
--rw-r--r--   0        0        0     2224 2024-04-29 07:40:13.718239 cg-60.4.6/cg/meta/upload/coverage.py
--rw-r--r--   0        0        0        0 2024-04-29 07:40:13.718239 cg-60.4.6/cg/meta/upload/fohm/__init__.py
--rw-r--r--   0        0        0    12102 2024-04-29 07:40:13.718239 cg-60.4.6/cg/meta/upload/fohm/fohm.py
--rw-r--r--   0        0        0       30 2024-04-29 07:40:13.718239 cg-60.4.6/cg/meta/upload/gisaid/__init__.py
--rw-r--r--   0        0        0      928 2024-04-29 07:40:13.718239 cg-60.4.6/cg/meta/upload/gisaid/constants.py
--rw-r--r--   0        0        0    13521 2024-04-29 07:40:13.718239 cg-60.4.6/cg/meta/upload/gisaid/gisaid.py
--rw-r--r--   0        0        0     3312 2024-04-29 07:40:13.718239 cg-60.4.6/cg/meta/upload/gisaid/models.py
--rw-r--r--   0        0        0     5310 2024-04-29 07:40:13.718239 cg-60.4.6/cg/meta/upload/gt.py
--rw-r--r--   0        0        0      898 2024-04-29 07:40:13.718239 cg-60.4.6/cg/meta/upload/microsalt/microsalt_upload_api.py
--rw-r--r--   0        0        0        0 2024-04-29 07:40:13.718239 cg-60.4.6/cg/meta/upload/mip/__init__.py
--rw-r--r--   0        0        0     2546 2024-04-29 07:40:13.718239 cg-60.4.6/cg/meta/upload/mip/mip_dna.py
--rw-r--r--   0        0        0     1400 2024-04-29 07:40:13.718239 cg-60.4.6/cg/meta/upload/mip/mip_rna.py
--rw-r--r--   0        0        0     7294 2024-04-29 07:40:13.718239 cg-60.4.6/cg/meta/upload/mutacc.py
--rw-r--r--   0        0        0     1853 2024-04-29 07:40:13.718239 cg-60.4.6/cg/meta/upload/nf_analysis.py
--rw-r--r--   0        0        0       32 2024-04-29 07:40:13.718239 cg-60.4.6/cg/meta/upload/nipt/__init__.py
--rw-r--r--   0        0        0      696 2024-04-29 07:40:13.718239 cg-60.4.6/cg/meta/upload/nipt/models.py
--rw-r--r--   0        0        0     8106 2024-04-29 07:40:13.718239 cg-60.4.6/cg/meta/upload/nipt/nipt.py
--rw-r--r--   0        0        0        0 2024-04-29 07:40:13.718239 cg-60.4.6/cg/meta/upload/scout/__init__.py
--rw-r--r--   0        0        0     4009 2024-04-29 07:40:13.718239 cg-60.4.6/cg/meta/upload/scout/balsamic_config_builder.py
--rw-r--r--   0        0        0     1491 2024-04-29 07:40:13.718239 cg-60.4.6/cg/meta/upload/scout/balsamic_umi_config_builder.py
--rw-r--r--   0        0        0     3322 2024-04-29 07:40:13.718239 cg-60.4.6/cg/meta/upload/scout/hk_tags.py
--rw-r--r--   0        0        0     9103 2024-04-29 07:40:13.718239 cg-60.4.6/cg/meta/upload/scout/mip_config_builder.py
--rw-r--r--   0        0        0     3495 2024-04-29 07:40:13.718239 cg-60.4.6/cg/meta/upload/scout/rnafusion_config_builder.py
--rw-r--r--   0        0        0     7231 2024-04-29 07:40:13.718239 cg-60.4.6/cg/meta/upload/scout/scout_config_builder.py
--rw-r--r--   0        0        0    23146 2024-04-29 07:40:13.718239 cg-60.4.6/cg/meta/upload/scout/uploadscoutapi.py
--rw-r--r--   0        0        0     3197 2024-04-29 07:40:13.718239 cg-60.4.6/cg/meta/upload/upload_api.py
--rw-r--r--   0        0        0        0 2024-04-29 07:40:13.718239 cg-60.4.6/cg/meta/workflow/__init__.py
--rw-r--r--   0        0        0    31068 2024-04-29 07:40:13.722239 cg-60.4.6/cg/meta/workflow/analysis.py
--rw-r--r--   0        0        0    27751 2024-04-29 07:40:13.722239 cg-60.4.6/cg/meta/workflow/balsamic.py
--rw-r--r--   0        0        0     2700 2024-04-29 07:40:13.722239 cg-60.4.6/cg/meta/workflow/balsamic_pon.py
--rw-r--r--   0        0        0      553 2024-04-29 07:40:13.722239 cg-60.4.6/cg/meta/workflow/balsamic_qc.py
--rw-r--r--   0        0        0      556 2024-04-29 07:40:13.722239 cg-60.4.6/cg/meta/workflow/balsamic_umi.py
--rw-r--r--   0        0        0        0 2024-04-29 07:40:13.722239 cg-60.4.6/cg/meta/workflow/downsample/__init__.py
--rw-r--r--   0        0        0     3922 2024-04-29 07:40:13.722239 cg-60.4.6/cg/meta/workflow/downsample/downsample.py
--rw-r--r--   0        0        0      711 2024-04-29 07:40:13.722239 cg-60.4.6/cg/meta/workflow/downsample/sbatch.py
--rw-r--r--   0        0        0     8913 2024-04-29 07:40:13.722239 cg-60.4.6/cg/meta/workflow/fastq.py
--rw-r--r--   0        0        0    10603 2024-04-29 07:40:13.722239 cg-60.4.6/cg/meta/workflow/fluffy.py
--rw-r--r--   0        0        0      521 2024-04-29 07:40:13.722239 cg-60.4.6/cg/meta/workflow/jasen.py
--rw-r--r--   0        0        0       70 2024-04-29 07:40:13.722239 cg-60.4.6/cg/meta/workflow/microsalt/__init__.py
--rw-r--r--   0        0        0      116 2024-04-29 07:40:13.722239 cg-60.4.6/cg/meta/workflow/microsalt/constants.py
--rw-r--r--   0        0        0      174 2024-04-29 07:40:13.722239 cg-60.4.6/cg/meta/workflow/microsalt/metrics_parser/__init__.py
--rw-r--r--   0        0        0      366 2024-04-29 07:40:13.722239 cg-60.4.6/cg/meta/workflow/microsalt/metrics_parser/metrics_parser.py
--rw-r--r--   0        0        0      903 2024-04-29 07:40:13.722239 cg-60.4.6/cg/meta/workflow/microsalt/metrics_parser/models.py
--rw-r--r--   0        0        0    13173 2024-04-29 07:40:13.722239 cg-60.4.6/cg/meta/workflow/microsalt/microsalt.py
--rw-r--r--   0        0        0      113 2024-04-29 07:40:13.722239 cg-60.4.6/cg/meta/workflow/microsalt/quality_controller/__init__.py
--rw-r--r--   0        0        0      712 2024-04-29 07:40:13.722239 cg-60.4.6/cg/meta/workflow/microsalt/quality_controller/models.py
--rw-r--r--   0        0        0     5697 2024-04-29 07:40:13.722239 cg-60.4.6/cg/meta/workflow/microsalt/quality_controller/quality_controller.py
--rw-r--r--   0        0        0     1217 2024-04-29 07:40:13.722239 cg-60.4.6/cg/meta/workflow/microsalt/quality_controller/report_generator.py
--rw-r--r--   0        0        0     2373 2024-04-29 07:40:13.722239 cg-60.4.6/cg/meta/workflow/microsalt/quality_controller/result_logger.py
--rw-r--r--   0        0        0     5641 2024-04-29 07:40:13.722239 cg-60.4.6/cg/meta/workflow/microsalt/quality_controller/utils.py
--rw-r--r--   0        0        0     1220 2024-04-29 07:40:13.722239 cg-60.4.6/cg/meta/workflow/microsalt/utils.py
--rw-r--r--   0        0        0    12611 2024-04-29 07:40:13.722239 cg-60.4.6/cg/meta/workflow/mip.py
--rw-r--r--   0        0        0     2948 2024-04-29 07:40:13.722239 cg-60.4.6/cg/meta/workflow/mip_dna.py
--rw-r--r--   0        0        0     2124 2024-04-29 07:40:13.722239 cg-60.4.6/cg/meta/workflow/mip_rna.py
--rw-r--r--   0        0        0    10974 2024-04-29 07:40:13.722239 cg-60.4.6/cg/meta/workflow/mutant.py
--rw-r--r--   0        0        0    37934 2024-04-29 07:40:13.722239 cg-60.4.6/cg/meta/workflow/nf_analysis.py
--rw-r--r--   0        0        0     6161 2024-04-29 07:40:13.722239 cg-60.4.6/cg/meta/workflow/nf_handlers.py
--rw-r--r--   0        0        0     6357 2024-04-29 07:40:13.722239 cg-60.4.6/cg/meta/workflow/prepare_fastq.py
--rw-r--r--   0        0        0     4785 2024-04-29 07:40:13.722239 cg-60.4.6/cg/meta/workflow/raredisease.py
--rw-r--r--   0        0        0     5403 2024-04-29 07:40:13.722239 cg-60.4.6/cg/meta/workflow/rnafusion.py
--rw-r--r--   0        0        0     4427 2024-04-29 07:40:13.722239 cg-60.4.6/cg/meta/workflow/taxprofiler.py
--rw-r--r--   0        0        0     3576 2024-04-29 07:40:13.722239 cg-60.4.6/cg/meta/workflow/tomte.py
--rw-r--r--   0        0        0      113 2024-04-29 07:40:13.722239 cg-60.4.6/cg/models/__init__.py
--rw-r--r--   0        0        0      367 2024-04-29 07:40:13.722239 cg-60.4.6/cg/models/analysis.py
--rw-r--r--   0        0        0        0 2024-04-29 07:40:13.722239 cg-60.4.6/cg/models/balsamic/__init__.py
--rw-r--r--   0        0        0      459 2024-04-29 07:40:13.722239 cg-60.4.6/cg/models/balsamic/analysis.py
--rw-r--r--   0        0        0     4550 2024-04-29 07:40:13.722239 cg-60.4.6/cg/models/balsamic/config.py
--rw-r--r--   0        0        0     1986 2024-04-29 07:40:13.722239 cg-60.4.6/cg/models/balsamic/metrics.py
--rw-r--r--   0        0        0    17539 2024-04-29 07:40:13.722239 cg-60.4.6/cg/models/cg_config.py
--rw-r--r--   0        0        0     4302 2024-04-29 07:40:13.722239 cg-60.4.6/cg/models/compression_data.py
--rw-r--r--   0        0        0        0 2024-04-29 07:40:13.722239 cg-60.4.6/cg/models/deliverables/__init__.py
--rw-r--r--   0        0        0     5213 2024-04-29 07:40:13.722239 cg-60.4.6/cg/models/deliverables/metric_deliverables.py
--rw-r--r--   0        0        0      243 2024-04-29 07:40:13.722239 cg-60.4.6/cg/models/delivery/delivery.py
--rw-r--r--   0        0        0        0 2024-04-29 07:40:13.722239 cg-60.4.6/cg/models/demultiplex/__init__.py
--rw-r--r--   0        0        0    12040 2024-04-29 07:40:13.722239 cg-60.4.6/cg/models/demultiplex/run_parameters.py
--rw-r--r--   0        0        0      539 2024-04-29 07:40:13.722239 cg-60.4.6/cg/models/demultiplex/sbatch.py
--rw-r--r--   0        0        0     7006 2024-04-29 07:40:13.722239 cg-60.4.6/cg/models/downsample/downsample_data.py
--rw-r--r--   0        0        0      255 2024-04-29 07:40:13.722239 cg-60.4.6/cg/models/email.py
--rw-r--r--   0        0        0     1046 2024-04-29 07:40:13.722239 cg-60.4.6/cg/models/fastq.py
--rw-r--r--   0        0        0     2157 2024-04-29 07:40:13.722239 cg-60.4.6/cg/models/file_data.py
--rw-r--r--   0        0        0        0 2024-04-29 07:40:13.722239 cg-60.4.6/cg/models/flow_cell/__init__.py
--rw-r--r--   0        0        0     9984 2024-04-29 07:40:13.722239 cg-60.4.6/cg/models/flow_cell/flow_cell.py
--rw-r--r--   0        0        0      317 2024-04-29 07:40:13.722239 cg-60.4.6/cg/models/flow_cell/utils.py
--rw-r--r--   0        0        0        0 2024-04-29 07:40:13.722239 cg-60.4.6/cg/models/invoice/__init__.py
--rw-r--r--   0        0        0     1254 2024-04-29 07:40:13.722239 cg-60.4.6/cg/models/invoice/invoice.py
--rw-r--r--   0        0        0        0 2024-04-29 07:40:13.722239 cg-60.4.6/cg/models/lims/__init__.py
--rw-r--r--   0        0        0     2019 2024-04-29 07:40:13.722239 cg-60.4.6/cg/models/lims/sample.py
--rw-r--r--   0        0        0        0 2024-04-29 07:40:13.722239 cg-60.4.6/cg/models/mip/__init__.py
--rw-r--r--   0        0        0      337 2024-04-29 07:40:13.722239 cg-60.4.6/cg/models/mip/mip_analysis.py
--rw-r--r--   0        0        0     1564 2024-04-29 07:40:13.722239 cg-60.4.6/cg/models/mip/mip_config.py
--rw-r--r--   0        0        0     4696 2024-04-29 07:40:13.722239 cg-60.4.6/cg/models/mip/mip_metrics_deliverables.py
--rw-r--r--   0        0        0     2550 2024-04-29 07:40:13.722239 cg-60.4.6/cg/models/mip/mip_sample_info.py
--rw-r--r--   0        0        0     2472 2024-04-29 07:40:13.722239 cg-60.4.6/cg/models/nf_analysis.py
--rw-r--r--   0        0        0        0 2024-04-29 07:40:13.722239 cg-60.4.6/cg/models/observations/__init__.py
--rw-r--r--   0        0        0      688 2024-04-29 07:40:13.722239 cg-60.4.6/cg/models/observations/input_files.py
--rw-r--r--   0        0        0        0 2024-04-29 07:40:13.722239 cg-60.4.6/cg/models/orders/__init__.py
--rw-r--r--   0        0        0     2659 2024-04-29 07:40:13.722239 cg-60.4.6/cg/models/orders/constants.py
--rw-r--r--   0        0        0     5604 2024-04-29 07:40:13.722239 cg-60.4.6/cg/models/orders/excel_sample.py
--rw-r--r--   0        0        0      898 2024-04-29 07:40:13.722239 cg-60.4.6/cg/models/orders/json_sample.py
--rw-r--r--   0        0        0     1449 2024-04-29 07:40:13.722239 cg-60.4.6/cg/models/orders/order.py
--rw-r--r--   0        0        0      811 2024-04-29 07:40:13.722239 cg-60.4.6/cg/models/orders/orderform_schema.py
--rw-r--r--   0        0        0     4212 2024-04-29 07:40:13.726239 cg-60.4.6/cg/models/orders/sample_base.py
--rw-r--r--   0        0        0     9668 2024-04-29 07:40:13.726239 cg-60.4.6/cg/models/orders/samples.py
--rw-r--r--   0        0        0        0 2024-04-29 07:40:13.726239 cg-60.4.6/cg/models/orders/validators/__init__.py
--rw-r--r--   0        0        0     2300 2024-04-29 07:40:13.726239 cg-60.4.6/cg/models/orders/validators/excel_sample_validators.py
--rw-r--r--   0        0        0      576 2024-04-29 07:40:13.726239 cg-60.4.6/cg/models/orders/validators/json_sample_validators.py
--rw-r--r--   0        0        0       71 2024-04-29 07:40:13.726239 cg-60.4.6/cg/models/orders/validators/sample_base_validators.py
--rw-r--r--   0        0        0      101 2024-04-29 07:40:13.726239 cg-60.4.6/cg/models/qc_metrics.py
--rw-r--r--   0        0        0        0 2024-04-29 07:40:13.726239 cg-60.4.6/cg/models/raredisease/__init__.py
--rw-r--r--   0        0        0     1875 2024-04-29 07:40:13.726239 cg-60.4.6/cg/models/raredisease/raredisease.py
--rw-r--r--   0        0        0        0 2024-04-29 07:40:13.726239 cg-60.4.6/cg/models/report/__init__.py
--rw-r--r--   0        0        0     7461 2024-04-29 07:40:13.726239 cg-60.4.6/cg/models/report/metadata.py
--rw-r--r--   0        0        0     6180 2024-04-29 07:40:13.726239 cg-60.4.6/cg/models/report/report.py
--rw-r--r--   0        0        0     5221 2024-04-29 07:40:13.726239 cg-60.4.6/cg/models/report/sample.py
--rw-r--r--   0        0        0     3004 2024-04-29 07:40:13.726239 cg-60.4.6/cg/models/report/validators.py
--rw-r--r--   0        0        0        0 2024-04-29 07:40:13.726239 cg-60.4.6/cg/models/rnafusion/__init__.py
--rw-r--r--   0        0        0     1865 2024-04-29 07:40:13.726239 cg-60.4.6/cg/models/rnafusion/rnafusion.py
--rw-r--r--   0        0        0        0 2024-04-29 07:40:13.726239 cg-60.4.6/cg/models/scout/__init__.py
--rw-r--r--   0        0        0     4783 2024-04-29 07:40:13.726239 cg-60.4.6/cg/models/scout/scout_load_config.py
--rw-r--r--   0        0        0      116 2024-04-29 07:40:13.726239 cg-60.4.6/cg/models/scout/validators.py
--rw-r--r--   0        0        0        0 2024-04-29 07:40:13.726239 cg-60.4.6/cg/models/slurm/__init__.py
--rw-r--r--   0        0        0      617 2024-04-29 07:40:13.726239 cg-60.4.6/cg/models/slurm/sbatch.py
--rw-r--r--   0        0        0        0 2024-04-29 07:40:13.726239 cg-60.4.6/cg/models/taxprofiler/__init__.py
--rw-r--r--   0        0        0     2443 2024-04-29 07:40:13.726239 cg-60.4.6/cg/models/taxprofiler/taxprofiler.py
--rw-r--r--   0        0        0     2588 2024-04-29 07:40:13.726239 cg-60.4.6/cg/models/tomte/tomte.py
--rw-r--r--   0        0        0        0 2024-04-29 07:40:13.726239 cg-60.4.6/cg/models/workflow/__init__.py
--rw-r--r--   0        0        0      685 2024-04-29 07:40:13.726239 cg-60.4.6/cg/models/workflow/mutant.py
--rw-r--r--   0        0        0       70 2024-04-29 07:40:13.726239 cg-60.4.6/cg/models/workflow/validators.py
--rw-r--r--   0        0        0      842 2024-04-29 07:40:13.726239 cg-60.4.6/cg/resources/__init__.py
--rw-r--r--   0        0        0     3493 2024-04-29 07:40:13.726239 cg-60.4.6/cg/resources/rnafusion_bundle_filenames.yaml
--rw-r--r--   0        0        0     2434 2024-04-29 07:40:13.726239 cg-60.4.6/cg/resources/taxprofiler_bundle_filenames.yaml
--rw-r--r--   0        0        0     3732 2024-04-29 07:40:13.726239 cg-60.4.6/cg/resources/tomte_bundle_filenames.yaml
--rw-r--r--   0        0        0        0 2024-04-29 07:40:13.726239 cg-60.4.6/cg/server/__init__.py
--rw-r--r--   0        0        0    20299 2024-04-29 07:40:13.726239 cg-60.4.6/cg/server/admin.py
--rw-r--r--   0        0        0    22743 2024-04-29 07:40:13.726239 cg-60.4.6/cg/server/api.py
--rw-r--r--   0        0        0     4887 2024-04-29 07:40:13.726239 cg-60.4.6/cg/server/app.py
--rw-r--r--   0        0        0       48 2024-04-29 07:40:13.726239 cg-60.4.6/cg/server/auto.py
--rw-r--r--   0        0        0     1184 2024-04-29 07:40:13.726239 cg-60.4.6/cg/server/config.py
--rw-r--r--   0        0        0        0 2024-04-29 07:40:13.726239 cg-60.4.6/cg/server/dto/__init__.py
--rw-r--r--   0        0        0        0 2024-04-29 07:40:13.726239 cg-60.4.6/cg/server/dto/delivery_message/__init__.py
--rw-r--r--   0        0        0      300 2024-04-29 07:40:13.726239 cg-60.4.6/cg/server/dto/delivery_message/delivery_message_request.py
--rw-r--r--   0        0        0      183 2024-04-29 07:40:13.726239 cg-60.4.6/cg/server/dto/delivery_message/delivery_message_response.py
--rw-r--r--   0        0        0        0 2024-04-29 07:40:13.726239 cg-60.4.6/cg/server/dto/orders/__init__.py
--rw-r--r--   0        0        0      165 2024-04-29 07:40:13.726239 cg-60.4.6/cg/server/dto/orders/order_delivery_update_request.py
--rw-r--r--   0        0        0       91 2024-04-29 07:40:13.726239 cg-60.4.6/cg/server/dto/orders/order_patch_request.py
--rw-r--r--   0        0        0      662 2024-04-29 07:40:13.726239 cg-60.4.6/cg/server/dto/orders/orders_request.py
--rw-r--r--   0        0        0      413 2024-04-29 07:40:13.726239 cg-60.4.6/cg/server/dto/orders/orders_response.py
--rw-r--r--   0        0        0     2598 2024-04-29 07:40:13.726239 cg-60.4.6/cg/server/ext.py
--rw-r--r--   0        0        0       29 2024-04-29 07:40:13.726239 cg-60.4.6/cg/server/invoices/__init__.py
--rw-r--r--   0        0        0     4793 2024-04-29 07:40:13.726239 cg-60.4.6/cg/server/invoices/templates/invoices/index.html
--rw-r--r--   0        0        0     8171 2024-04-29 07:40:13.726239 cg-60.4.6/cg/server/invoices/templates/invoices/invoice.html
--rw-r--r--   0        0        0     2838 2024-04-29 07:40:13.726239 cg-60.4.6/cg/server/invoices/templates/invoices/layout.html
--rw-r--r--   0        0        0     4956 2024-04-29 07:40:13.726239 cg-60.4.6/cg/server/invoices/templates/invoices/new.html
--rw-r--r--   0        0        0     7708 2024-04-29 07:40:13.726239 cg-60.4.6/cg/server/invoices/views.py
--rw-r--r--   0        0        0      354 2024-04-29 07:40:13.726239 cg-60.4.6/cg/server/templates/admin/index.html
--rw-r--r--   0        0        0        0 2024-04-29 07:40:13.726239 cg-60.4.6/cg/services/__init__.py
--rw-r--r--   0        0        0        0 2024-04-29 07:40:13.726239 cg-60.4.6/cg/services/analysis_service/__init__.py
--rw-r--r--   0        0        0      482 2024-04-29 07:40:13.726239 cg-60.4.6/cg/services/analysis_service/analysis_service.py
--rw-r--r--   0        0        0        0 2024-04-29 07:40:13.726239 cg-60.4.6/cg/services/delivery_message/__init__.py
--rw-r--r--   0        0        0     2531 2024-04-29 07:40:13.726239 cg-60.4.6/cg/services/delivery_message/delivery_message_service.py
--rw-r--r--   0        0        0      792 2024-04-29 07:40:13.726239 cg-60.4.6/cg/services/delivery_message/messages/__init__.py
--rw-r--r--   0        0        0     1366 2024-04-29 07:40:13.726239 cg-60.4.6/cg/services/delivery_message/messages/analysis_scout_message.py
--rw-r--r--   0        0        0      791 2024-04-29 07:40:13.726239 cg-60.4.6/cg/services/delivery_message/messages/covid_message.py
--rw-r--r--   0        0        0      189 2024-04-29 07:40:13.726239 cg-60.4.6/cg/services/delivery_message/messages/delivery_message.py
--rw-r--r--   0        0        0     1391 2024-04-29 07:40:13.726239 cg-60.4.6/cg/services/delivery_message/messages/fastq_analysis_scout_message.py
--rw-r--r--   0        0        0      535 2024-04-29 07:40:13.726239 cg-60.4.6/cg/services/delivery_message/messages/fastq_message.py
--rw-r--r--   0        0        0     1358 2024-04-29 07:40:13.726239 cg-60.4.6/cg/services/delivery_message/messages/fastq_scout_message.py
--rw-r--r--   0        0        0      604 2024-04-29 07:40:13.726239 cg-60.4.6/cg/services/delivery_message/messages/microsalt_mwr_message.py
--rw-r--r--   0        0        0      592 2024-04-29 07:40:13.726239 cg-60.4.6/cg/services/delivery_message/messages/microsalt_mwx_message.py
--rw-r--r--   0        0        0      903 2024-04-29 07:40:13.726239 cg-60.4.6/cg/services/delivery_message/messages/scout_message.py
--rw-r--r--   0        0        0      512 2024-04-29 07:40:13.726239 cg-60.4.6/cg/services/delivery_message/messages/statina_message.py
--rw-r--r--   0        0        0      779 2024-04-29 07:40:13.726239 cg-60.4.6/cg/services/delivery_message/messages/utils.py
--rw-r--r--   0        0        0     3300 2024-04-29 07:40:13.726239 cg-60.4.6/cg/services/delivery_message/utils.py
--rw-r--r--   0        0        0        0 2024-04-29 07:40:13.726239 cg-60.4.6/cg/services/fastq_file_service/__init__.py
--rw-r--r--   0        0        0      101 2024-04-29 07:40:13.726239 cg-60.4.6/cg/services/fastq_file_service/exceptions.py
--rw-r--r--   0        0        0     1092 2024-04-29 07:40:13.726239 cg-60.4.6/cg/services/fastq_file_service/fastq_file_service.py
--rw-r--r--   0        0        0     2991 2024-04-29 07:40:13.726239 cg-60.4.6/cg/services/fastq_file_service/utils.py
--rw-r--r--   0        0        0        0 2024-04-29 07:40:13.726239 cg-60.4.6/cg/services/orders/__init__.py
--rw-r--r--   0        0        0        0 2024-04-29 07:40:13.726239 cg-60.4.6/cg/services/orders/order_service/__init__.py
--rw-r--r--   0        0        0     2684 2024-04-29 07:40:13.726239 cg-60.4.6/cg/services/orders/order_service/order_service.py
--rw-r--r--   0        0        0     1214 2024-04-29 07:40:13.726239 cg-60.4.6/cg/services/orders/order_service/utils.py
--rw-r--r--   0        0        0       94 2024-04-29 07:40:13.726239 cg-60.4.6/cg/services/orders/order_status_service/__init__.py
--rw-r--r--   0        0        0        0 2024-04-29 07:40:13.726239 cg-60.4.6/cg/services/orders/order_status_service/dto/__init__.py
--rw-r--r--   0        0        0      192 2024-04-29 07:40:13.726239 cg-60.4.6/cg/services/orders/order_status_service/dto/case_summary.py
--rw-r--r--   0        0        0      289 2024-04-29 07:40:13.726239 cg-60.4.6/cg/services/orders/order_status_service/dto/order_summary.py
--rw-r--r--   0        0        0     1768 2024-04-29 07:40:13.726239 cg-60.4.6/cg/services/orders/order_status_service/order_summary_service.py
--rw-r--r--   0        0        0     1737 2024-04-29 07:40:13.726239 cg-60.4.6/cg/services/orders/order_status_service/utils.py
--rw-r--r--   0        0        0       95 2024-04-29 07:40:13.726239 cg-60.4.6/cg/services/quality_controller/__init__.py
--rw-r--r--   0        0        0     1819 2024-04-29 07:40:13.726239 cg-60.4.6/cg/services/quality_controller/quality_checks/checks.py
--rw-r--r--   0        0        0     4987 2024-04-29 07:40:13.730239 cg-60.4.6/cg/services/quality_controller/quality_checks/utils.py
--rw-r--r--   0        0        0     1040 2024-04-29 07:40:13.730239 cg-60.4.6/cg/services/quality_controller/quality_controller_service.py
--rw-r--r--   0        0        0        0 2024-04-29 07:40:13.730239 cg-60.4.6/cg/services/slurm_service/__init__.py
--rw-r--r--   0        0        0      703 2024-04-29 07:40:13.730239 cg-60.4.6/cg/services/slurm_service/slurm_cli_service.py
--rw-r--r--   0        0        0      242 2024-04-29 07:40:13.730239 cg-60.4.6/cg/services/slurm_service/slurm_service.py
--rw-r--r--   0        0        0        0 2024-04-29 07:40:13.730239 cg-60.4.6/cg/services/slurm_upload_service/__init__.py
--rw-r--r--   0        0        0      175 2024-04-29 07:40:13.730239 cg-60.4.6/cg/services/slurm_upload_service/slurm_upload_config.py
--rw-r--r--   0        0        0     2074 2024-04-29 07:40:13.730239 cg-60.4.6/cg/services/slurm_upload_service/slurm_upload_service.py
--rw-r--r--   0        0        0      203 2024-04-29 07:40:13.730239 cg-60.4.6/cg/services/slurm_upload_service/utils.py
--rw-r--r--   0        0        0        0 2024-04-29 07:40:13.730239 cg-60.4.6/cg/store/__init__.py
--rw-r--r--   0        0        0     4650 2024-04-29 07:40:13.730239 cg-60.4.6/cg/store/base.py
--rw-r--r--   0        0        0        0 2024-04-29 07:40:13.730239 cg-60.4.6/cg/store/crud/__init__.py
--rw-r--r--   0        0        0    13100 2024-04-29 07:40:13.730239 cg-60.4.6/cg/store/crud/create.py
--rw-r--r--   0        0        0     2144 2024-04-29 07:40:13.730239 cg-60.4.6/cg/store/crud/delete.py
--rw-r--r--   0        0        0    60036 2024-04-29 07:40:13.730239 cg-60.4.6/cg/store/crud/read.py
--rw-r--r--   0        0        0     1121 2024-04-29 07:40:13.730239 cg-60.4.6/cg/store/crud/update.py
--rw-r--r--   0        0        0     1662 2024-04-29 07:40:13.730239 cg-60.4.6/cg/store/database.py
--rw-r--r--   0        0        0        0 2024-04-29 07:40:13.730239 cg-60.4.6/cg/store/filters/__init__.py
--rw-r--r--   0        0        0     5371 2024-04-29 07:40:13.730239 cg-60.4.6/cg/store/filters/status_analysis_filters.py
--rw-r--r--   0        0        0     1712 2024-04-29 07:40:13.730239 cg-60.4.6/cg/store/filters/status_application_filters.py
--rw-r--r--   0        0        0     1440 2024-04-29 07:40:13.730239 cg-60.4.6/cg/store/filters/status_application_limitations_filters.py
--rw-r--r--   0        0        0     2523 2024-04-29 07:40:13.730239 cg-60.4.6/cg/store/filters/status_application_version_filters.py
--rw-r--r--   0        0        0     1390 2024-04-29 07:40:13.730239 cg-60.4.6/cg/store/filters/status_bed_filters.py
--rw-r--r--   0        0        0     1317 2024-04-29 07:40:13.730239 cg-60.4.6/cg/store/filters/status_bed_version_filters.py
--rw-r--r--   0        0        0    10787 2024-04-29 07:40:13.730239 cg-60.4.6/cg/store/filters/status_case_filters.py
--rw-r--r--   0        0        0     3272 2024-04-29 07:40:13.730239 cg-60.4.6/cg/store/filters/status_case_sample_filters.py
--rw-r--r--   0        0        0      903 2024-04-29 07:40:13.730239 cg-60.4.6/cg/store/filters/status_collaboration_filters.py
--rw-r--r--   0        0        0     1412 2024-04-29 07:40:13.730239 cg-60.4.6/cg/store/filters/status_customer_filters.py
--rw-r--r--   0        0        0     1880 2024-04-29 07:40:13.730239 cg-60.4.6/cg/store/filters/status_flow_cell_filters.py
--rw-r--r--   0        0        0     1255 2024-04-29 07:40:13.730239 cg-60.4.6/cg/store/filters/status_invoice_filters.py
--rw-r--r--   0        0        0     2792 2024-04-29 07:40:13.730239 cg-60.4.6/cg/store/filters/status_metrics_filters.py
--rw-r--r--   0        0        0     3225 2024-04-29 07:40:13.730239 cg-60.4.6/cg/store/filters/status_order_filters.py
--rw-r--r--   0        0        0      851 2024-04-29 07:40:13.730239 cg-60.4.6/cg/store/filters/status_organism_filters.py
--rw-r--r--   0        0        0      783 2024-04-29 07:40:13.730239 cg-60.4.6/cg/store/filters/status_panel_filters.py
--rw-r--r--   0        0        0     3923 2024-04-29 07:40:13.730239 cg-60.4.6/cg/store/filters/status_pool_filters.py
--rw-r--r--   0        0        0     8660 2024-04-29 07:40:13.730239 cg-60.4.6/cg/store/filters/status_sample_filters.py
--rw-r--r--   0        0        0      731 2024-04-29 07:40:13.730239 cg-60.4.6/cg/store/filters/status_user_filters.py
--rw-r--r--   0        0        0    36081 2024-04-29 07:40:13.730239 cg-60.4.6/cg/store/models.py
--rw-r--r--   0        0        0      593 2024-04-29 07:40:13.730239 cg-60.4.6/cg/store/store.py
--rw-r--r--   0        0        0       30 2024-04-29 07:40:13.730239 cg-60.4.6/cg/utils/__init__.py
--rw-r--r--   0        0        0      187 2024-04-29 07:40:13.730239 cg-60.4.6/cg/utils/calculations.py
--rw-r--r--   0        0        0        0 2024-04-29 07:40:13.730239 cg-60.4.6/cg/utils/checksum/__init__.py
--rw-r--r--   0        0        0     1579 2024-04-29 07:40:13.730239 cg-60.4.6/cg/utils/checksum/checksum.py
--rw-r--r--   0        0        0     1655 2024-04-29 07:40:13.730239 cg-60.4.6/cg/utils/click/EnumChoice.py
--rw-r--r--   0        0        0        0 2024-04-29 07:40:13.730239 cg-60.4.6/cg/utils/click/__init__.py
--rw-r--r--   0        0        0     4910 2024-04-29 07:40:13.730239 cg-60.4.6/cg/utils/commands.py
--rw-r--r--   0        0        0     1811 2024-04-29 07:40:13.730239 cg-60.4.6/cg/utils/date.py
--rw-r--r--   0        0        0      635 2024-04-29 07:40:13.730239 cg-60.4.6/cg/utils/dict.py
--rw-r--r--   0        0        0     2111 2024-04-29 07:40:13.730239 cg-60.4.6/cg/utils/dispatcher.py
--rw-r--r--   0        0        0     1251 2024-04-29 07:40:13.730239 cg-60.4.6/cg/utils/email.py
--rw-r--r--   0        0        0      134 2024-04-29 07:40:13.730239 cg-60.4.6/cg/utils/enums.py
--rw-r--r--   0        0        0     3178 2024-04-29 07:40:13.730239 cg-60.4.6/cg/utils/files.py
--rw-r--r--   0        0        0        0 2024-04-29 07:40:13.730239 cg-60.4.6/cg/utils/flask/__init__.py
--rw-r--r--   0        0        0     1052 2024-04-29 07:40:13.730239 cg-60.4.6/cg/utils/flask/enum.py
--rw-r--r--   0        0        0      233 2024-04-29 07:40:13.730239 cg-60.4.6/cg/utils/flow_cell.py
--rw-r--r--   0        0        0      834 2024-04-29 07:40:13.730239 cg-60.4.6/cg/utils/time.py
--rw-r--r--   0        0        0     1410 2024-04-29 07:40:13.730239 cg-60.4.6/cg/utils/utils.py
--rw-r--r--   0        0        0     1697 2024-04-29 07:40:13.734239 cg-60.4.6/pyproject.toml
--rw-r--r--   0        0        0        0 2024-04-29 07:40:13.734239 cg-60.4.6/tests/__init__.py
--rw-r--r--   0        0        0     1158 2024-04-29 07:40:13.734239 cg-60.4.6/tests/apps/conftest.py
--rw-r--r--   0        0        0      231 2024-04-29 07:40:13.734239 cg-60.4.6/tests/apps/coverage/conftest.py
--rw-r--r--   0        0        0     6188 2024-04-29 07:40:13.734239 cg-60.4.6/tests/apps/coverage/test_coverage.py
--rw-r--r--   0        0        0     1693 2024-04-29 07:40:13.734239 cg-60.4.6/tests/apps/crunchy/conftest.py
--rw-r--r--   0        0        0     5438 2024-04-29 07:40:13.734239 cg-60.4.6/tests/apps/crunchy/test_compress_fastq.py
--rw-r--r--   0        0        0     2283 2024-04-29 07:40:13.734239 cg-60.4.6/tests/apps/crunchy/test_config.py
--rw-r--r--   0        0        0    14032 2024-04-29 07:40:13.734239 cg-60.4.6/tests/apps/crunchy/test_crunchy.py
--rw-r--r--   0        0        0     9109 2024-04-29 07:40:13.734239 cg-60.4.6/tests/apps/crunchy/test_spring_decompression.py
--rw-r--r--   0        0        0        0 2024-04-29 07:40:13.734239 cg-60.4.6/tests/apps/demultiplex/__init__.py
--rw-r--r--   0        0        0     4994 2024-04-29 07:40:13.734239 cg-60.4.6/tests/apps/demultiplex/conftest.py
--rw-r--r--   0        0        0     4010 2024-04-29 07:40:13.734239 cg-60.4.6/tests/apps/demultiplex/test_create_sample_sheet.py
--rw-r--r--   0        0        0     7986 2024-04-29 07:40:13.734239 cg-60.4.6/tests/apps/demultiplex/test_demultiplex_api.py
--rw-r--r--   0        0        0     4782 2024-04-29 07:40:13.734239 cg-60.4.6/tests/apps/demultiplex/test_index.py
--rw-r--r--   0        0        0     9468 2024-04-29 07:40:13.734239 cg-60.4.6/tests/apps/demultiplex/test_override_cycles_validator.py
--rw-r--r--   0        0        0     4042 2024-04-29 07:40:13.734239 cg-60.4.6/tests/apps/demultiplex/test_read_sample_sheet.py
--rw-r--r--   0        0        0    12389 2024-04-29 07:40:13.734239 cg-60.4.6/tests/apps/demultiplex/test_sample_models.py
--rw-r--r--   0        0        0      951 2024-04-29 07:40:13.734239 cg-60.4.6/tests/apps/demultiplex/test_sample_sheet_creator.py
--rw-r--r--   0        0        0     3175 2024-04-29 07:40:13.734239 cg-60.4.6/tests/apps/demultiplex/test_sample_sheet_models.py
--rw-r--r--   0        0        0    10932 2024-04-29 07:40:13.734239 cg-60.4.6/tests/apps/demultiplex/test_sample_sheet_validator.py
--rw-r--r--   0        0        0     4896 2024-04-29 07:40:13.734239 cg-60.4.6/tests/apps/demultiplex/test_translate_sample_sheet.py
--rw-r--r--   0        0        0     1450 2024-04-29 07:40:13.734239 cg-60.4.6/tests/apps/demultiplex/test_validate.py
--rw-r--r--   0        0        0     5094 2024-04-29 07:40:13.734239 cg-60.4.6/tests/apps/downsample/test_downsample.py
--rw-r--r--   0        0        0     1419 2024-04-29 07:40:13.734239 cg-60.4.6/tests/apps/downsample/test_downsample_utils.py
--rw-r--r--   0        0        0     1716 2024-04-29 07:40:13.734239 cg-60.4.6/tests/apps/gens/test_gens_api.py
--rw-r--r--   0        0        0     1950 2024-04-29 07:40:13.734239 cg-60.4.6/tests/apps/gt/conftest.py
--rw-r--r--   0        0        0     4276 2024-04-29 07:40:13.734239 cg-60.4.6/tests/apps/gt/test_gt_api.py
--rw-r--r--   0        0        0     1453 2024-04-29 07:40:13.734239 cg-60.4.6/tests/apps/hk/conftest.py
--rw-r--r--   0        0        0      684 2024-04-29 07:40:13.734239 cg-60.4.6/tests/apps/hk/test__getattr__.py
--rw-r--r--   0        0        0     1593 2024-04-29 07:40:13.734239 cg-60.4.6/tests/apps/hk/test_add_file.py
--rw-r--r--   0        0        0     3523 2024-04-29 07:40:13.734239 cg-60.4.6/tests/apps/hk/test_bundles.py
--rw-r--r--   0        0        0      871 2024-04-29 07:40:13.734239 cg-60.4.6/tests/apps/hk/test_core.py
--rw-r--r--   0        0        0    31172 2024-04-29 07:40:13.734239 cg-60.4.6/tests/apps/hk/test_file.py
--rw-r--r--   0        0        0     5080 2024-04-29 07:40:13.734239 cg-60.4.6/tests/apps/hk/test_version.py
--rw-r--r--   0        0        0     1840 2024-04-29 07:40:13.734239 cg-60.4.6/tests/apps/lims/conftest.py
--rw-r--r--   0        0        0     3197 2024-04-29 07:40:13.734239 cg-60.4.6/tests/apps/lims/test_api.py
--rw-r--r--   0        0        0     1451 2024-04-29 07:40:13.734239 cg-60.4.6/tests/apps/lims/test_sample_sheet.py
--rw-r--r--   0        0        0     9223 2024-04-29 07:40:13.734239 cg-60.4.6/tests/apps/loqus/conftest.py
--rw-r--r--   0        0        0     8994 2024-04-29 07:40:13.734239 cg-60.4.6/tests/apps/loqus/test_loqusdb_api.py
--rw-r--r--   0        0        0     2439 2024-04-29 07:40:13.734239 cg-60.4.6/tests/apps/madeline/conftest.py
--rw-r--r--   0        0        0     4653 2024-04-29 07:40:13.734239 cg-60.4.6/tests/apps/madeline/test_madeline.py
--rw-r--r--   0        0        0     3328 2024-04-29 07:40:13.734239 cg-60.4.6/tests/apps/mip/conftest.py
--rw-r--r--   0        0        0     2487 2024-04-29 07:40:13.734239 cg-60.4.6/tests/apps/mip/test_config_mip.py
--rw-r--r--   0        0        0      883 2024-04-29 07:40:13.734239 cg-60.4.6/tests/apps/mutacc_auto/conftest.py
--rw-r--r--   0        0        0     2473 2024-04-29 07:40:13.734239 cg-60.4.6/tests/apps/mutacc_auto/test_mutacc_auto.py
--rw-r--r--   0        0        0    11930 2024-04-29 07:40:13.734239 cg-60.4.6/tests/apps/orderform/conftest.py
--rw-r--r--   0        0        0     9484 2024-04-29 07:40:13.734239 cg-60.4.6/tests/apps/orderform/test_excel_orderform_parser.py
--rw-r--r--   0        0        0     4351 2024-04-29 07:40:13.734239 cg-60.4.6/tests/apps/orderform/test_excel_sample_schema.py
--rw-r--r--   0        0        0     1032 2024-04-29 07:40:13.734239 cg-60.4.6/tests/apps/orderform/test_json_orderform_parser.py
--rw-r--r--   0        0        0     2474 2024-04-29 07:40:13.734239 cg-60.4.6/tests/apps/orderform/test_orderform_parser.py
--rw-r--r--   0        0        0    16002 2024-04-29 07:40:13.734239 cg-60.4.6/tests/apps/orderform/validators/test_excel_sample_validators.py
--rw-r--r--   0        0        0     3670 2024-04-29 07:40:13.738239 cg-60.4.6/tests/apps/scout/conftest.py
--rw-r--r--   0        0        0     2269 2024-04-29 07:40:13.738239 cg-60.4.6/tests/apps/scout/test_get_causative_variants.py
--rw-r--r--   0        0        0     1376 2024-04-29 07:40:13.738239 cg-60.4.6/tests/apps/scout/test_get_scout_cases.py
--rw-r--r--   0        0        0     1840 2024-04-29 07:40:13.738239 cg-60.4.6/tests/apps/scout/test_scout_load_config.py
--rw-r--r--   0        0        0     7047 2024-04-29 07:40:13.738239 cg-60.4.6/tests/apps/scout/test_scout_models.py
--rw-r--r--   0        0        0        0 2024-04-29 07:40:13.738239 cg-60.4.6/tests/apps/sequencing_metrics_parser/__init__.py
--rw-r--r--   0        0        0     2639 2024-04-29 07:40:13.738239 cg-60.4.6/tests/apps/sequencing_metrics_parser/conftest.py
--rw-r--r--   0        0        0     7069 2024-04-29 07:40:13.738239 cg-60.4.6/tests/apps/sequencing_metrics_parser/parsers/test_bclconvert.py
--rw-r--r--   0        0        0     2958 2024-04-29 07:40:13.738239 cg-60.4.6/tests/apps/sequencing_metrics_parser/parsers/test_sequencing_metrics_parser_api.py
--rw-r--r--   0        0        0     1131 2024-04-29 07:40:13.738239 cg-60.4.6/tests/apps/slurm/conftest.py
--rw-r--r--   0        0        0     4412 2024-04-29 07:40:13.738239 cg-60.4.6/tests/apps/slurm/test_slurm_api.py
--rw-r--r--   0        0        0      831 2024-04-29 07:40:13.738239 cg-60.4.6/tests/apps/test_apps_environ.py
--rw-r--r--   0        0        0      957 2024-04-29 07:40:13.738239 cg-60.4.6/tests/apps/test_osticket.py
--rw-r--r--   0        0        0        0 2024-04-29 07:40:13.738239 cg-60.4.6/tests/cli/__init__.py
--rw-r--r--   0        0        0        0 2024-04-29 07:40:13.738239 cg-60.4.6/tests/cli/add/__init__.py
--rw-r--r--   0        0        0     1174 2024-04-29 07:40:13.738239 cg-60.4.6/tests/cli/add/test_cli_add.py
--rw-r--r--   0        0        0     2471 2024-04-29 07:40:13.738239 cg-60.4.6/tests/cli/add/test_cli_add_customer.py
--rw-r--r--   0        0        0     6841 2024-04-29 07:40:13.738239 cg-60.4.6/tests/cli/add/test_cli_add_family.py
--rw-r--r--   0        0        0     7588 2024-04-29 07:40:13.738239 cg-60.4.6/tests/cli/add/test_cli_add_relationship.py
--rw-r--r--   0        0        0     8382 2024-04-29 07:40:13.738239 cg-60.4.6/tests/cli/add/test_cli_add_sample.py
--rw-r--r--   0        0        0        0 2024-04-29 07:40:13.738239 cg-60.4.6/tests/cli/backup/__init__.py
--rw-r--r--   0        0        0      705 2024-04-29 07:40:13.738239 cg-60.4.6/tests/cli/backup/conftest.py
--rw-r--r--   0        0        0    11101 2024-04-29 07:40:13.738239 cg-60.4.6/tests/cli/backup/test_backup_command.py
--rw-r--r--   0        0        0     6865 2024-04-29 07:40:13.738239 cg-60.4.6/tests/cli/clean/conftest.py
--rw-r--r--   0        0        0     5536 2024-04-29 07:40:13.738239 cg-60.4.6/tests/cli/clean/test_balsamic_clean.py
--rw-r--r--   0        0        0     2557 2024-04-29 07:40:13.738239 cg-60.4.6/tests/cli/clean/test_clean_flow_cell.py
--rw-r--r--   0        0        0     1830 2024-04-29 07:40:13.738239 cg-60.4.6/tests/cli/clean/test_clean_hk_bundle_files.py
--rw-r--r--   0        0        0     2098 2024-04-29 07:40:13.738239 cg-60.4.6/tests/cli/clean/test_hk_bundle_files.py
--rw-r--r--   0        0        0     4610 2024-04-29 07:40:13.738239 cg-60.4.6/tests/cli/clean/test_hk_case_bundle_files.py
--rw-r--r--   0        0        0     3585 2024-04-29 07:40:13.738239 cg-60.4.6/tests/cli/clean/test_microbial_clean.py
--rw-r--r--   0        0        0     1881 2024-04-29 07:40:13.738239 cg-60.4.6/tests/cli/clean/test_rsync_past_run_dirs.py
--rw-r--r--   0        0        0     9707 2024-04-29 07:40:13.738239 cg-60.4.6/tests/cli/compress/conftest.py
--rw-r--r--   0        0        0     7709 2024-04-29 07:40:13.738239 cg-60.4.6/tests/cli/compress/test_cli_compress_fastq.py
--rw-r--r--   0        0        0     1416 2024-04-29 07:40:13.738239 cg-60.4.6/tests/cli/compress/test_cli_decompress_spring.py
--rw-r--r--   0        0        0     5205 2024-04-29 07:40:13.738239 cg-60.4.6/tests/cli/compress/test_compress_helpers.py
--rw-r--r--   0        0        0     1239 2024-04-29 07:40:13.738239 cg-60.4.6/tests/cli/compress/test_store_fastq.py
--rw-r--r--   0        0        0     7558 2024-04-29 07:40:13.738239 cg-60.4.6/tests/cli/conftest.py
--rw-r--r--   0        0        0    12747 2024-04-29 07:40:13.738239 cg-60.4.6/tests/cli/delete/test_cli_delete_case.py
--rw-r--r--   0        0        0     1873 2024-04-29 07:40:13.738239 cg-60.4.6/tests/cli/delete/test_cli_delete_cases.py
--rw-r--r--   0        0        0     3794 2024-04-29 07:40:13.738239 cg-60.4.6/tests/cli/deliver/conftest.py
--rw-r--r--   0        0        0     4428 2024-04-29 07:40:13.738239 cg-60.4.6/tests/cli/deliver/test_deliver_base.py
--rw-r--r--   0        0        0     1166 2024-04-29 07:40:13.738239 cg-60.4.6/tests/cli/deliver/test_rsync_base.py
--rw-r--r--   0        0        0     8569 2024-04-29 07:40:13.738239 cg-60.4.6/tests/cli/deliver/test_run_deliver_cmd.py
--rw-r--r--   0        0        0        0 2024-04-29 07:40:13.738239 cg-60.4.6/tests/cli/demultiplex/__init__.py
--rw-r--r--   0        0        0     5109 2024-04-29 07:40:13.738239 cg-60.4.6/tests/cli/demultiplex/test_create_sample_sheet.py
--rw-r--r--   0        0        0     4799 2024-04-29 07:40:13.738239 cg-60.4.6/tests/cli/demultiplex/test_demultiplex_flowcell.py
--rw-r--r--   0        0        0     1639 2024-04-29 07:40:13.738239 cg-60.4.6/tests/cli/demultiplex/test_finish_demux.py
--rw-r--r--   0        0        0     3015 2024-04-29 07:40:13.738239 cg-60.4.6/tests/cli/demultiplex/test_validate_sample_sheet.py
--rw-r--r--   0        0        0     4291 2024-04-29 07:40:13.738239 cg-60.4.6/tests/cli/demultiplex/test_verify_syncing.py
--rw-r--r--   0        0        0     1585 2024-04-29 07:40:13.738239 cg-60.4.6/tests/cli/downsample/test_cli_downsample.py
--rw-r--r--   0        0        0        0 2024-04-29 07:40:13.738239 cg-60.4.6/tests/cli/generate/__init__.py
--rw-r--r--   0        0        0        0 2024-04-29 07:40:13.738239 cg-60.4.6/tests/cli/generate/report/__init__.py
--rw-r--r--   0        0        0     1622 2024-04-29 07:40:13.738239 cg-60.4.6/tests/cli/generate/report/conftest.py
--rw-r--r--   0        0        0     2477 2024-04-29 07:40:13.738239 cg-60.4.6/tests/cli/generate/report/test_cli_delivery_report.py
--rw-r--r--   0        0        0     2760 2024-04-29 07:40:13.738239 cg-60.4.6/tests/cli/generate/report/test_utils.py
--rw-r--r--   0        0        0      563 2024-04-29 07:40:13.738239 cg-60.4.6/tests/cli/generate/test_cli_base.py
--rw-r--r--   0        0        0        0 2024-04-29 07:40:13.738239 cg-60.4.6/tests/cli/get/__init__.py
--rw-r--r--   0        0        0      863 2024-04-29 07:40:13.738239 cg-60.4.6/tests/cli/get/test_cli_get.py
--rw-r--r--   0        0        0     1526 2024-04-29 07:40:13.738239 cg-60.4.6/tests/cli/get/test_cli_get_analysis.py
--rw-r--r--   0        0        0     1242 2024-04-29 07:40:13.738239 cg-60.4.6/tests/cli/get/test_cli_get_case.py
--rw-r--r--   0        0        0     6208 2024-04-29 07:40:13.738239 cg-60.4.6/tests/cli/get/test_cli_get_flow_cell.py
--rw-r--r--   0        0        0     8835 2024-04-29 07:40:13.738239 cg-60.4.6/tests/cli/get/test_cli_get_sample.py
--rw-r--r--   0        0        0     1364 2024-04-29 07:40:13.738239 cg-60.4.6/tests/cli/set/conftest.py
--rw-r--r--   0        0        0     7311 2024-04-29 07:40:13.738239 cg-60.4.6/tests/cli/set/test_cli_set_case.py
--rw-r--r--   0        0        0     1460 2024-04-29 07:40:13.738239 cg-60.4.6/tests/cli/set/test_cli_set_cases.py
--rw-r--r--   0        0        0     2016 2024-04-29 07:40:13.738239 cg-60.4.6/tests/cli/set/test_cli_set_flowcell.py
--rw-r--r--   0        0        0     1685 2024-04-29 07:40:13.738239 cg-60.4.6/tests/cli/set/test_cli_set_list_keys.py
--rw-r--r--   0        0        0    12450 2024-04-29 07:40:13.738239 cg-60.4.6/tests/cli/set/test_cli_set_sample.py
--rw-r--r--   0        0        0     6124 2024-04-29 07:40:13.738239 cg-60.4.6/tests/cli/set/test_cli_set_samples.py
--rw-r--r--   0        0        0     7015 2024-04-29 07:40:13.738239 cg-60.4.6/tests/cli/store/test_store.py
--rw-r--r--   0        0        0     2332 2024-04-29 07:40:13.738239 cg-60.4.6/tests/cli/test_base.py
--rw-r--r--   0        0        0        0 2024-04-29 07:40:13.738239 cg-60.4.6/tests/cli/upload/__init__.py
--rw-r--r--   0        0        0    10057 2024-04-29 07:40:13.738239 cg-60.4.6/tests/cli/upload/conftest.py
--rw-r--r--   0        0        0     2295 2024-04-29 07:40:13.738239 cg-60.4.6/tests/cli/upload/test_cli_scout.py
--rw-r--r--   0        0        0     1789 2024-04-29 07:40:13.738239 cg-60.4.6/tests/cli/upload/test_cli_upload.py
--rw-r--r--   0        0        0      971 2024-04-29 07:40:13.738239 cg-60.4.6/tests/cli/upload/test_cli_upload_auto.py
--rw-r--r--   0        0        0     1669 2024-04-29 07:40:13.738239 cg-60.4.6/tests/cli/upload/test_cli_upload_delivery_report.py
--rw-r--r--   0        0        0      895 2024-04-29 07:40:13.738239 cg-60.4.6/tests/cli/upload/test_cli_upload_fastq.py
--rw-r--r--   0        0        0     1199 2024-04-29 07:40:13.738239 cg-60.4.6/tests/cli/upload/test_cli_upload_genotype.py
--rw-r--r--   0        0        0      694 2024-04-29 07:40:13.738239 cg-60.4.6/tests/cli/upload/test_cli_upload_gens.py
--rw-r--r--   0        0        0     9965 2024-04-29 07:40:13.738239 cg-60.4.6/tests/cli/upload/test_cli_upload_nipt.py
--rw-r--r--   0        0        0     4684 2024-04-29 07:40:13.742239 cg-60.4.6/tests/cli/upload/test_cli_upload_nipt_ftp.py
--rw-r--r--   0        0        0     1839 2024-04-29 07:40:13.742239 cg-60.4.6/tests/cli/upload/test_cli_upload_nipt_statina.py
--rw-r--r--   0        0        0     6177 2024-04-29 07:40:13.742239 cg-60.4.6/tests/cli/upload/test_cli_upload_observations.py
--rw-r--r--   0        0        0        0 2024-04-29 07:40:13.742239 cg-60.4.6/tests/cli/workflow/__init__.py
--rw-r--r--   0        0        0    31369 2024-04-29 07:40:13.742239 cg-60.4.6/tests/cli/workflow/balsamic/conftest.py
--rw-r--r--   0        0        0    13938 2024-04-29 07:40:13.742239 cg-60.4.6/tests/cli/workflow/balsamic/test_cli_balsamic_config_case.py
--rw-r--r--   0        0        0     7984 2024-04-29 07:40:13.742239 cg-60.4.6/tests/cli/workflow/balsamic/test_compound_commands.py
--rw-r--r--   0        0        0     2336 2024-04-29 07:40:13.742239 cg-60.4.6/tests/cli/workflow/balsamic/test_link.py
--rw-r--r--   0        0        0     3554 2024-04-29 07:40:13.742239 cg-60.4.6/tests/cli/workflow/balsamic/test_report_deliver.py
--rw-r--r--   0        0        0     6209 2024-04-29 07:40:13.742239 cg-60.4.6/tests/cli/workflow/balsamic/test_run.py
--rw-r--r--   0        0        0     6934 2024-04-29 07:40:13.742239 cg-60.4.6/tests/cli/workflow/balsamic/test_store_housekeeper.py
--rw-r--r--   0        0        0     8458 2024-04-29 07:40:13.742239 cg-60.4.6/tests/cli/workflow/conftest.py
--rw-r--r--   0        0        0        0 2024-04-29 07:40:13.742239 cg-60.4.6/tests/cli/workflow/fastq/__init__.py
--rw-r--r--   0        0        0     2332 2024-04-29 07:40:13.742239 cg-60.4.6/tests/cli/workflow/fastq/test_fastq_base.py
--rw-r--r--   0        0        0        0 2024-04-29 07:40:13.742239 cg-60.4.6/tests/cli/workflow/fluffy/__init__.py
--rw-r--r--   0        0        0     5237 2024-04-29 07:40:13.742239 cg-60.4.6/tests/cli/workflow/fluffy/conftest.py
--rw-r--r--   0        0        0     5687 2024-04-29 07:40:13.742239 cg-60.4.6/tests/cli/workflow/fluffy/test_cli_create_samplesheet.py
--rw-r--r--   0        0        0     3302 2024-04-29 07:40:13.742239 cg-60.4.6/tests/cli/workflow/fluffy/test_cli_link.py
--rw-r--r--   0        0        0     1896 2024-04-29 07:40:13.742239 cg-60.4.6/tests/cli/workflow/fluffy/test_cli_run.py
--rw-r--r--   0        0        0     2968 2024-04-29 07:40:13.742239 cg-60.4.6/tests/cli/workflow/fluffy/test_cli_start.py
--rw-r--r--   0        0        0     7815 2024-04-29 07:40:13.742239 cg-60.4.6/tests/cli/workflow/fluffy/test_cli_store.py
--rw-r--r--   0        0        0     2775 2024-04-29 07:40:13.742239 cg-60.4.6/tests/cli/workflow/microsalt/conftest.py
--rw-r--r--   0        0        0     6926 2024-04-29 07:40:13.742239 cg-60.4.6/tests/cli/workflow/microsalt/test_microsalt_case_config.py
--rw-r--r--   0        0        0     1000 2024-04-29 07:40:13.742239 cg-60.4.6/tests/cli/workflow/microsalt/test_microsalt_run.py
--rw-r--r--   0        0        0     6544 2024-04-29 07:40:13.742239 cg-60.4.6/tests/cli/workflow/mip/conftest.py
--rw-r--r--   0        0        0     7011 2024-04-29 07:40:13.742239 cg-60.4.6/tests/cli/workflow/mip/test_cli_mip_base.py
--rw-r--r--   0        0        0     1542 2024-04-29 07:40:13.742239 cg-60.4.6/tests/cli/workflow/mip/test_cli_mip_dna_config_case.py
--rw-r--r--   0        0        0      431 2024-04-29 07:40:13.742239 cg-60.4.6/tests/cli/workflow/mip/test_cli_mip_dna_link.py
--rw-r--r--   0        0        0     2108 2024-04-29 07:40:13.742239 cg-60.4.6/tests/cli/workflow/mip/test_cli_mip_dna_manged_variants.py
--rw-r--r--   0        0        0     1273 2024-04-29 07:40:13.742239 cg-60.4.6/tests/cli/workflow/mip/test_cli_mip_dna_panel.py
--rw-r--r--   0        0        0     3595 2024-04-29 07:40:13.742239 cg-60.4.6/tests/cli/workflow/mip/test_cli_mip_dna_run.py
--rw-r--r--   0        0        0     3884 2024-04-29 07:40:13.742239 cg-60.4.6/tests/cli/workflow/mip/test_cli_mip_dna_start.py
--rw-r--r--   0        0        0     1004 2024-04-29 07:40:13.742239 cg-60.4.6/tests/cli/workflow/mip/test_cli_mip_rna_config_case.py
--rw-r--r--   0        0        0      527 2024-04-29 07:40:13.742239 cg-60.4.6/tests/cli/workflow/mip/test_cli_mip_rna_link.py
--rw-r--r--   0        0        0      716 2024-04-29 07:40:13.742239 cg-60.4.6/tests/cli/workflow/mip/test_cli_mip_rna_run.py
--rw-r--r--   0        0        0     8559 2024-04-29 07:40:13.742239 cg-60.4.6/tests/cli/workflow/mip/test_cli_mip_store.py
--rw-r--r--   0        0        0        0 2024-04-29 07:40:13.742239 cg-60.4.6/tests/cli/workflow/nf_analysis/__init__.py
--rw-r--r--   0        0        0     9318 2024-04-29 07:40:13.742239 cg-60.4.6/tests/cli/workflow/nf_analysis/test_cli_config_case.py
--rw-r--r--   0        0        0     3831 2024-04-29 07:40:13.742239 cg-60.4.6/tests/cli/workflow/nf_analysis/test_cli_metrics_deliver.py
--rw-r--r--   0        0        0     5087 2024-04-29 07:40:13.742239 cg-60.4.6/tests/cli/workflow/nf_analysis/test_cli_report_deliver.py
--rw-r--r--   0        0        0     9211 2024-04-29 07:40:13.742239 cg-60.4.6/tests/cli/workflow/nf_analysis/test_cli_run.py
--rw-r--r--   0        0        0     3267 2024-04-29 07:40:13.742239 cg-60.4.6/tests/cli/workflow/nf_analysis/test_cli_start.py
--rw-r--r--   0        0        0     9877 2024-04-29 07:40:13.742239 cg-60.4.6/tests/cli/workflow/nf_analysis/test_cli_store.py
--rw-r--r--   0        0        0    10373 2024-04-29 07:40:13.742239 cg-60.4.6/tests/cli/workflow/nf_analysis/test_cli_store_housekeeper.py
--rw-r--r--   0        0        0      978 2024-04-29 07:40:13.742239 cg-60.4.6/tests/cli/workflow/nf_analysis/test_cli_workflow_base.py
--rw-r--r--   0        0        0        0 2024-04-29 07:40:13.742239 cg-60.4.6/tests/cli/workflow/raredisease/__init__.py
--rw-r--r--   0        0        0     3940 2024-04-29 07:40:13.742239 cg-60.4.6/tests/cli/workflow/raredisease/test_cli_raredisease_compound_commands.py
--rw-r--r--   0        0        0      921 2024-04-29 07:40:13.742239 cg-60.4.6/tests/cli/workflow/test_cli_workflow.py
--rw-r--r--   0        0        0     4310 2024-04-29 07:40:13.742239 cg-60.4.6/tests/cli/workflow/test_cli_workflow_clean.py
--rw-r--r--   0        0        0        0 2024-04-29 07:40:13.742239 cg-60.4.6/tests/clients/__init__.py
--rw-r--r--   0        0        0        0 2024-04-29 07:40:13.742239 cg-60.4.6/tests/clients/arnold/__init__.py
--rw-r--r--   0        0        0     1080 2024-04-29 07:40:13.742239 cg-60.4.6/tests/clients/arnold/conftest.py
--rw-r--r--   0        0        0     1503 2024-04-29 07:40:13.742239 cg-60.4.6/tests/clients/arnold/test_arnold_api_client.py
--rw-r--r--   0        0        0        0 2024-04-29 07:40:13.742239 cg-60.4.6/tests/clients/janus/__init__.py
--rw-r--r--   0        0        0     2381 2024-04-29 07:40:13.742239 cg-60.4.6/tests/clients/janus/conftest.py
--rw-r--r--   0        0        0     1716 2024-04-29 07:40:13.742239 cg-60.4.6/tests/clients/janus/test_janus_api_client.py
--rw-r--r--   0        0        0   129141 2024-04-29 07:40:13.742239 cg-60.4.6/tests/conftest.py
--rw-r--r--   0        0        0        0 2024-04-29 07:40:13.742239 cg-60.4.6/tests/fixture_plugins/__init__.py
--rw-r--r--   0        0        0        0 2024-04-29 07:40:13.742239 cg-60.4.6/tests/fixture_plugins/delivery_fixtures/__init__.py
--rw-r--r--   0        0        0     2653 2024-04-29 07:40:13.742239 cg-60.4.6/tests/fixture_plugins/delivery_fixtures/bundle_fixtures.py
--rw-r--r--   0        0        0     4972 2024-04-29 07:40:13.742239 cg-60.4.6/tests/fixture_plugins/delivery_fixtures/context_fixtures.py
--rw-r--r--   0        0        0     1494 2024-04-29 07:40:13.742239 cg-60.4.6/tests/fixture_plugins/delivery_fixtures/path_fixtures.py
--rw-r--r--   0        0        0        0 2024-04-29 07:40:13.742239 cg-60.4.6/tests/fixture_plugins/demultiplex_fixtures/__init__.py
--rw-r--r--   0        0        0     4636 2024-04-29 07:40:13.742239 cg-60.4.6/tests/fixture_plugins/demultiplex_fixtures/flow_cell_fixtures.py
--rw-r--r--   0        0        0     3413 2024-04-29 07:40:13.742239 cg-60.4.6/tests/fixture_plugins/demultiplex_fixtures/name_fixtures.py
--rw-r--r--   0        0        0    20458 2024-04-29 07:40:13.742239 cg-60.4.6/tests/fixture_plugins/demultiplex_fixtures/path_fixtures.py
--rw-r--r--   0        0        0     3412 2024-04-29 07:40:13.742239 cg-60.4.6/tests/fixture_plugins/demultiplex_fixtures/run_parameters_fixtures.py
--rw-r--r--   0        0        0     5988 2024-04-29 07:40:13.742239 cg-60.4.6/tests/fixture_plugins/demultiplex_fixtures/sample_fixtures.py
--rw-r--r--   0        0        0     8960 2024-04-29 07:40:13.742239 cg-60.4.6/tests/fixture_plugins/demultiplex_fixtures/sample_sheet_fixtures.py
--rw-r--r--   0        0        0     3174 2024-04-29 07:40:13.742239 cg-60.4.6/tests/fixture_plugins/quality_controller_fixtures/sequencing_qc_check_scenario.py
--rw-r--r--   0        0        0     4801 2024-04-29 07:40:13.742239 cg-60.4.6/tests/fixture_plugins/quality_controller_fixtures/sequencing_qc_fixtures.py
--rw-r--r--   0        0        0     1304 2024-04-29 07:40:13.742239 cg-60.4.6/tests/fixture_plugins/timestamp_fixtures.py
--rw-r--r--   0        0        0        0 2024-04-29 07:40:13.746239 cg-60.4.6/tests/fixtures/analysis/balsamic/tn_wgs/adm1.cram
--rw-r--r--   0        0        0        0 2024-04-29 07:40:13.746239 cg-60.4.6/tests/fixtures/analysis/balsamic/tn_wgs/ascat.output.pdf
--rw-r--r--   0        0        0        0 2024-04-29 07:40:13.746239 cg-60.4.6/tests/fixtures/analysis/balsamic/tn_wgs/snv.vcf
--rw-r--r--   0        0        0        0 2024-04-29 07:40:13.746239 cg-60.4.6/tests/fixtures/analysis/balsamic/tn_wgs/sv.vcf
--rw-r--r--   0        0        0    14644 2024-04-29 07:40:13.746239 cg-60.4.6/tests/fixtures/analysis/microsalt/ACC11111_qc_fail/ACC11111_qc_fail.json
--rw-r--r--   0        0        0    15921 2024-04-29 07:40:13.746239 cg-60.4.6/tests/fixtures/analysis/microsalt/ACC22222_qc_pass/ACC22222_qc_pass.json
--rw-r--r--   0        0        0        0 2024-04-29 07:40:13.746239 cg-60.4.6/tests/fixtures/analysis/mip/dna/ADM1.baf.bed.gz
--rw-r--r--   0        0        0        0 2024-04-29 07:40:13.746239 cg-60.4.6/tests/fixtures/analysis/mip/dna/ADM1.cov.bed.gz
--rw-r--r--   0        0        0        0 2024-04-29 07:40:13.746239 cg-60.4.6/tests/fixtures/analysis/mip/dna/ADM2.cram
--rw-r--r--   0        0        0        0 2024-04-29 07:40:13.746239 cg-60.4.6/tests/fixtures/analysis/mip/dna/ADM3.cram
--rw-r--r--   0        0        0        0 2024-04-29 07:40:13.746239 cg-60.4.6/tests/fixtures/analysis/mip/dna/adm1.cram
--rw-r--r--   0        0        0        0 2024-04-29 07:40:13.746239 cg-60.4.6/tests/fixtures/analysis/mip/dna/adm1.mt.bam
--rw-r--r--   0        0        0        0 2024-04-29 07:40:13.746239 cg-60.4.6/tests/fixtures/analysis/mip/dna/multiqc.html
--rw-r--r--   0        0        0        0 2024-04-29 07:40:13.746239 cg-60.4.6/tests/fixtures/analysis/mip/dna/report.pdf
--rw-r--r--   0        0        0        0 2024-04-29 07:40:13.746239 cg-60.4.6/tests/fixtures/analysis/mip/dna/smn.vcf
--rw-r--r--   0        0        0        0 2024-04-29 07:40:13.746239 cg-60.4.6/tests/fixtures/analysis/mip/dna/snv.vcf
--rw-r--r--   0        0        0        0 2024-04-29 07:40:13.746239 cg-60.4.6/tests/fixtures/analysis/mip/dna/snv_research.vcf
--rw-r--r--   0        0        0        0 2024-04-29 07:40:13.746239 cg-60.4.6/tests/fixtures/analysis/mip/dna/str.vcf
--rw-r--r--   0        0        0        0 2024-04-29 07:40:13.746239 cg-60.4.6/tests/fixtures/analysis/mip/dna/sv.vcf
--rw-r--r--   0        0        0        0 2024-04-29 07:40:13.746239 cg-60.4.6/tests/fixtures/analysis/mip/dna/sv_research.vcf
--rw-r--r--   0        0        0        0 2024-04-29 07:40:13.746239 cg-60.4.6/tests/fixtures/analysis/mip/dna/vcf2cytosure.txt
--rw-r--r--   0        0        0       70 2024-04-29 07:40:13.746239 cg-60.4.6/tests/fixtures/analysis/nf-analysis/pipeline_params.config
--rw-r--r--   0        0        0      195 2024-04-29 07:40:13.746239 cg-60.4.6/tests/fixtures/analysis/nf-analysis/pipeline_resource_optimisation.config
--rw-r--r--   0        0        0      195 2024-04-29 07:40:13.746239 cg-60.4.6/tests/fixtures/analysis/nf-analysis/platform.config
--rw-r--r--   0        0        0     8173 2024-04-29 07:40:13.746239 cg-60.4.6/tests/fixtures/analysis/raredisease/multiqc_data.json
--rw-r--r--   0        0        0    20005 2024-04-29 07:40:13.746239 cg-60.4.6/tests/fixtures/analysis/raredisease/raredisease_case_enough_reads_metrics_deliverables.yaml
--rw-r--r--   0        0        0     5497 2024-04-29 07:40:13.746239 cg-60.4.6/tests/fixtures/analysis/rnafusion/multiqc_data.json
--rw-r--r--   0        0        0    12499 2024-04-29 07:40:13.746239 cg-60.4.6/tests/fixtures/analysis/rnafusion/rnafusion_case_enough_reads_metrics_deliverables.yaml
--rw-r--r--   0        0        0     2873 2024-04-29 07:40:13.746239 cg-60.4.6/tests/fixtures/analysis/sample_coverage.bed
--rw-r--r--   0        0        0     6506 2024-04-29 07:40:13.746239 cg-60.4.6/tests/fixtures/analysis/taxprofiler/multiqc_data.json
--rw-r--r--   0        0        0    10513 2024-04-29 07:40:13.746239 cg-60.4.6/tests/fixtures/analysis/taxprofiler/taxprofiler_case_metrics_deliverables.yaml
--rw-r--r--   0        0        0     5771 2024-04-29 07:40:13.746239 cg-60.4.6/tests/fixtures/analysis/tomte/multiqc_data.json
--rw-r--r--   0        0        0    14859 2024-04-29 07:40:13.746239 cg-60.4.6/tests/fixtures/analysis/tomte/tomte_case_enough_reads_metrics_deliverables.yaml
--rw-r--r--   0        0        0    10961 2024-04-29 07:40:13.746239 cg-60.4.6/tests/fixtures/apps/balsamic/case/config.json
--rw-r--r--   0        0        0     3465 2024-04-29 07:40:13.746239 cg-60.4.6/tests/fixtures/apps/balsamic/case/metadata.yml
--rw-r--r--   0        0        0       63 2024-04-29 07:40:13.746239 cg-60.4.6/tests/fixtures/apps/balsamic/case/metadata_directory.yml
--rw-r--r--   0        0        0      165 2024-04-29 07:40:13.746239 cg-60.4.6/tests/fixtures/apps/balsamic/case/metadata_file_tags.yml
--rw-r--r--   0        0        0     2705 2024-04-29 07:40:13.746239 cg-60.4.6/tests/fixtures/apps/balsamic/case/metrics_deliverables.yaml
--rw-r--r--   0        0        0      692 2024-04-29 07:40:13.746239 cg-60.4.6/tests/fixtures/apps/crunchy/spring_metadata.json
--rw-r--r--   0        0        0        0 2024-04-29 07:40:13.746239 cg-60.4.6/tests/fixtures/apps/demultiplexing/demultiplexed-runs/170517_ST-E00266_0210_BHJCFFALXX/ACC2655A1_S2_L002_R1_001.fastq.gz
--rw-r--r--   0        0        0        0 2024-04-29 07:40:13.746239 cg-60.4.6/tests/fixtures/apps/demultiplexing/demultiplexed-runs/170517_ST-E00266_0210_BHJCFFALXX/ACC2655A1_S2_L002_R2_001.fastq.gz
--rw-r--r--   0        0        0      412 2024-04-29 07:40:13.746239 cg-60.4.6/tests/fixtures/apps/demultiplexing/demultiplexed-runs/170517_ST-E00266_0210_BHJCFFALXX/Reports/Adapter_Metrics.csv
--rw-r--r--   0        0        0      484 2024-04-29 07:40:13.746239 cg-60.4.6/tests/fixtures/apps/demultiplexing/demultiplexed-runs/170517_ST-E00266_0210_BHJCFFALXX/Reports/Demultiplex_Stats.csv
--rw-r--r--   0        0        0      658 2024-04-29 07:40:13.746239 cg-60.4.6/tests/fixtures/apps/demultiplexing/demultiplexed-runs/170517_ST-E00266_0210_BHJCFFALXX/Reports/Quality_Metrics.csv
--rw-r--r--   0        0        0        0 2024-04-29 07:40:13.746239 cg-60.4.6/tests/fixtures/apps/demultiplexing/demultiplexed-runs/170517_ST-E00266_0210_BHJCFFALXX/SVE2648A1_S1_L001_R1_001.fastq.gz
--rw-r--r--   0        0        0        0 2024-04-29 07:40:13.746239 cg-60.4.6/tests/fixtures/apps/demultiplexing/demultiplexed-runs/170517_ST-E00266_0210_BHJCFFALXX/SVE2648A1_S1_L001_R2_001.fastq.gz
--rw-r--r--   0        0        0        0 2024-04-29 07:40:13.746239 cg-60.4.6/tests/fixtures/apps/demultiplexing/demultiplexed-runs/170517_ST-E00266_0210_BHJCFFALXX/Undetermined_S0_L001_R1_001.fastq.gz
--rw-r--r--   0        0        0        0 2024-04-29 07:40:13.746239 cg-60.4.6/tests/fixtures/apps/demultiplexing/demultiplexed-runs/170517_ST-E00266_0210_BHJCFFALXX/Undetermined_S0_L001_R2_001.fastq.gz
--rw-r--r--   0        0        0        0 2024-04-29 07:40:13.746239 cg-60.4.6/tests/fixtures/apps/demultiplexing/demultiplexed-runs/170517_ST-E00266_0210_BHJCFFALXX/demuxcomplete.txt
--rw-r--r--   0        0        0     1757 2024-04-29 07:40:13.746239 cg-60.4.6/tests/fixtures/apps/demultiplexing/demultiplexed-runs/201203_D00483_0200_AHVKJCDRXX/HVKJCDRXX_demultiplex.stderr
--rw-r--r--   0        0        0        7 2024-04-29 07:40:13.746239 cg-60.4.6/tests/fixtures/apps/demultiplexing/demultiplexed-runs/201203_D00483_0200_AHVKJCDRXX/SampleSheet.csv
--rw-r--r--   0        0        0        0 2024-04-29 07:40:13.746239 cg-60.4.6/tests/fixtures/apps/demultiplexing/demultiplexed-runs/201203_D00483_0200_AHVKJCDRXX/Unaligned/Project_150392/Sample_ACC7769A10/HN3FKDSXY_AL-P-00425491-N-03103120-KH20210330-PN20210331_S1_L001_R1_001.fastq.gz
--rw-r--r--   0        0        0        0 2024-04-29 07:40:13.746239 cg-60.4.6/tests/fixtures/apps/demultiplexing/demultiplexed-runs/201203_D00483_0200_AHVKJCDRXX/Unaligned/Project_150392/Sample_ACC7769A10/HN3FKDSXY_AL-P-00425491-N-03103120-KH20210330-PN20210331_S1_L001_R2_001.fastq.gz
--rw-r--r--   0        0        0     6034 2024-04-29 07:40:13.746239 cg-60.4.6/tests/fixtures/apps/demultiplexing/demultiplexed-runs/201203_D00483_0200_AHVKJCDRXX/Unaligned/Stats/ConversionStats.xml
--rw-r--r--   0        0        0     1172 2024-04-29 07:40:13.746239 cg-60.4.6/tests/fixtures/apps/demultiplexing/demultiplexed-runs/201203_D00483_0200_AHVKJCDRXX/Unaligned/Stats/DemultiplexingStats.xml
--rw-r--r--   0        0        0        7 2024-04-29 07:40:13.746239 cg-60.4.6/tests/fixtures/apps/demultiplexing/demultiplexed-runs/201203_D00483_0200_AHVKJCDRXX/fastq_1.fastq.gz
--rw-r--r--   0        0        0        7 2024-04-29 07:40:13.746239 cg-60.4.6/tests/fixtures/apps/demultiplexing/demultiplexed-runs/201203_D00483_0200_AHVKJCDRXX/fastq_2.fastq.gz
--rw-r--r--   0        0        0        0 2024-04-29 07:40:13.746239 cg-60.4.6/tests/fixtures/apps/demultiplexing/demultiplexed-runs/20231108_LH00188_0028_B22F52TLT3/BCLConvert/fastq/ACC13169A1_S1_L001_R1_001.fastq.gz
--rw-r--r--   0        0        0        0 2024-04-29 07:40:13.746239 cg-60.4.6/tests/fixtures/apps/demultiplexing/demultiplexed-runs/20231108_LH00188_0028_B22F52TLT3/BCLConvert/fastq/ACC13169A1_S1_L001_R2_001.fastq.gz
--rw-r--r--   0        0        0        0 2024-04-29 07:40:13.746239 cg-60.4.6/tests/fixtures/apps/demultiplexing/demultiplexed-runs/20231108_LH00188_0028_B22F52TLT3/BCLConvert/fastq/ACC13170A6_S2_L002_R1_001.fastq.gz
--rw-r--r--   0        0        0        0 2024-04-29 07:40:13.746239 cg-60.4.6/tests/fixtures/apps/demultiplexing/demultiplexed-runs/20231108_LH00188_0028_B22F52TLT3/BCLConvert/fastq/ACC13170A6_S2_L002_R2_001.fastq.gz
--rw-r--r--   0        0        0        0 2024-04-29 07:40:13.746239 cg-60.4.6/tests/fixtures/apps/demultiplexing/demultiplexed-runs/20231108_LH00188_0028_B22F52TLT3/BCLConvert/fastq/Undetermined_S0_L001_R1_001.fastq.gz
--rw-r--r--   0        0        0        0 2024-04-29 07:40:13.746239 cg-60.4.6/tests/fixtures/apps/demultiplexing/demultiplexed-runs/20231108_LH00188_0028_B22F52TLT3/BCLConvert/fastq/Undetermined_S0_L001_R2_001.fastq.gz
--rw-r--r--   0        0        0      288 2024-04-29 07:40:13.746239 cg-60.4.6/tests/fixtures/apps/demultiplexing/demultiplexed-runs/20231108_LH00188_0028_B22F52TLT3/Reports/Adapter_Metrics.csv
--rw-r--r--   0        0        0      361 2024-04-29 07:40:13.746239 cg-60.4.6/tests/fixtures/apps/demultiplexing/demultiplexed-runs/20231108_LH00188_0028_B22F52TLT3/Reports/Demultiplex_Stats.csv
--rw-r--r--   0        0        0      414 2024-04-29 07:40:13.746239 cg-60.4.6/tests/fixtures/apps/demultiplexing/demultiplexed-runs/20231108_LH00188_0028_B22F52TLT3/Reports/Quality_Metrics.csv
--rw-r--r--   0        0        0        0 2024-04-29 07:40:13.746239 cg-60.4.6/tests/fixtures/apps/demultiplexing/demultiplexed-runs/20231108_LH00188_0028_B22F52TLT3/demuxcomplete.txt
--rw-r--r--   0        0        0      315 2024-04-29 07:40:13.746239 cg-60.4.6/tests/fixtures/apps/demultiplexing/demultiplexed-runs/211101_A00187_0615_AHLG5GDRZZ/Unaligned/Reports/Adapter_Metrics.csv
--rw-r--r--   0        0        0      434 2024-04-29 07:40:13.746239 cg-60.4.6/tests/fixtures/apps/demultiplexing/demultiplexed-runs/211101_A00187_0615_AHLG5GDRZZ/Unaligned/Reports/Quality_Metrics.csv
--rw-r--r--   0        0        0     8624 2024-04-29 07:40:13.746239 cg-60.4.6/tests/fixtures/apps/demultiplexing/demultiplexed-runs/211101_A00187_0615_AHLG5GDRZZ/Unaligned/Reports/RunInfo.xml
--rw-r--r--   0        0        0        0 2024-04-29 07:40:13.746239 cg-60.4.6/tests/fixtures/apps/demultiplexing/demultiplexed-runs/230912_A00187_1009_AHK33MDRX3/ACC12642A4_S2_L002_R1_001.fastq.gz
--rw-r--r--   0        0        0        0 2024-04-29 07:40:13.746239 cg-60.4.6/tests/fixtures/apps/demultiplexing/demultiplexed-runs/230912_A00187_1009_AHK33MDRX3/ACC12642A4_S2_L002_R2_001.fastq.gz
--rw-r--r--   0        0        0        0 2024-04-29 07:40:13.746239 cg-60.4.6/tests/fixtures/apps/demultiplexing/demultiplexed-runs/230912_A00187_1009_AHK33MDRX3/ACC12642A7_S1_L001_R1_001.fastq.gz
--rw-r--r--   0        0        0        0 2024-04-29 07:40:13.746239 cg-60.4.6/tests/fixtures/apps/demultiplexing/demultiplexed-runs/230912_A00187_1009_AHK33MDRX3/ACC12642A7_S1_L001_R2_001.fastq.gz
--rw-r--r--   0        0        0      303 2024-04-29 07:40:13.746239 cg-60.4.6/tests/fixtures/apps/demultiplexing/demultiplexed-runs/230912_A00187_1009_AHK33MDRX3/Reports/Adapter_Metrics.csv
--rw-r--r--   0        0        0      364 2024-04-29 07:40:13.746239 cg-60.4.6/tests/fixtures/apps/demultiplexing/demultiplexed-runs/230912_A00187_1009_AHK33MDRX3/Reports/Demultiplex_Stats.csv
--rw-r--r--   0        0        0      427 2024-04-29 07:40:13.750239 cg-60.4.6/tests/fixtures/apps/demultiplexing/demultiplexed-runs/230912_A00187_1009_AHK33MDRX3/Reports/Quality_Metrics.csv
--rw-r--r--   0        0        0        0 2024-04-29 07:40:13.750239 cg-60.4.6/tests/fixtures/apps/demultiplexing/demultiplexed-runs/230912_A00187_1009_AHK33MDRX3/Undetermined_S0_L001_R1_001.fastq.gz
--rw-r--r--   0        0        0        0 2024-04-29 07:40:13.750239 cg-60.4.6/tests/fixtures/apps/demultiplexing/demultiplexed-runs/230912_A00187_1009_AHK33MDRX3/Undetermined_S0_L001_R2_001.fastq.gz
--rw-r--r--   0        0        0        0 2024-04-29 07:40:13.750239 cg-60.4.6/tests/fixtures/apps/demultiplexing/demultiplexed-runs/230912_A00187_1009_AHK33MDRX3/demuxcomplete.txt
--rw-r--r--   0        0        0        0 2024-04-29 07:40:13.746239 cg-60.4.6/tests/fixtures/apps/demultiplexing/demultiplexed-runs-unfinished/201203_D00483_0200_AHVKJCDRXX/Unaligned/150392/ACC7769A10/AL-P-00425491-N-03103120-KH20210330-PN20210331_S1_L001_R1_001.fastq.gz
--rw-r--r--   0        0        0        0 2024-04-29 07:40:13.746239 cg-60.4.6/tests/fixtures/apps/demultiplexing/demultiplexed-runs-unfinished/201203_D00483_0200_AHVKJCDRXX/Unaligned/150392/ACC7769A10/AL-P-00425491-N-03103120-KH20210330-PN20210331_S1_L001_R2_001.fastq.gz
--rw-r--r--   0        0        0     4439 2024-04-29 07:40:13.746239 cg-60.4.6/tests/fixtures/apps/demultiplexing/demultiplexed-runs-unfinished/201203_D00483_0200_AHVKJCDRXX/Unaligned/Stats/ConversionStats.xml
--rw-r--r--   0        0        0     1172 2024-04-29 07:40:13.746239 cg-60.4.6/tests/fixtures/apps/demultiplexing/demultiplexed-runs-unfinished/201203_D00483_0200_AHVKJCDRXX/Unaligned/Stats/DemultiplexingStats.xml
--rw-r--r--   0        0        0        0 2024-04-29 07:40:13.746239 cg-60.4.6/tests/fixtures/apps/demultiplexing/demultiplexed-runs-unfinished/201203_D00483_0200_AHVKJCDRXX/Unaligned/Undetermined_S0_L001_R1_001.fastq.gz
--rw-r--r--   0        0        0        0 2024-04-29 07:40:13.746239 cg-60.4.6/tests/fixtures/apps/demultiplexing/demultiplexed-runs-unfinished/201203_D00483_0200_AHVKJCDRXX/Unaligned/Undetermined_S0_L001_R2_001.fastq.gz
--rw-r--r--   0        0        0        0 2024-04-29 07:40:13.746239 cg-60.4.6/tests/fixtures/apps/demultiplexing/demultiplexed-runs-unfinished/201203_D00483_0200_AHVKJCDRXX/Unaligned/Undetermined_S0_L002_R1_001.fastq.gz
--rw-r--r--   0        0        0        0 2024-04-29 07:40:13.746239 cg-60.4.6/tests/fixtures/apps/demultiplexing/demultiplexed-runs-unfinished/201203_D00483_0200_AHVKJCDRXX/Unaligned/Undetermined_S0_L002_R2_001.fastq.gz
--rw-r--r--   0        0        0     5127 2024-04-29 07:40:13.746239 cg-60.4.6/tests/fixtures/apps/demultiplexing/demultiplexed-runs-unfinished/230912_A00187_1009_AHK33MDRX3/SampleSheet.csv
--rw-r--r--   0        0        0       43 2024-04-29 07:40:13.750239 cg-60.4.6/tests/fixtures/apps/demultiplexing/fastq/dummy_run_R1_001.fastq.gz
--rw-r--r--   0        0        0       67 2024-04-29 07:40:13.750239 cg-60.4.6/tests/fixtures/apps/demultiplexing/fastq/dummy_run_R1_001.fastq.gz.md5
--rw-r--r--   0        0        0   338370 2024-04-29 07:40:13.750239 cg-60.4.6/tests/fixtures/apps/demultiplexing/fastq/fastq_run_R1_001.fastq.gz
--rw-r--r--   0        0        0       67 2024-04-29 07:40:13.750239 cg-60.4.6/tests/fixtures/apps/demultiplexing/fastq/fastq_run_R1_001.fastq.gz.md5
--rw-r--r--   0        0        0   338349 2024-04-29 07:40:13.750239 cg-60.4.6/tests/fixtures/apps/demultiplexing/fastq/fastq_run_R2_001.fastq.gz
--rw-r--r--   0        0        0        0 2024-04-29 07:40:13.750239 cg-60.4.6/tests/fixtures/apps/demultiplexing/flow_cells/170517_ST-E00266_0210_BHJCFFALXX/CopyComplete.txt
--rw-r--r--   0        0        0     2126 2024-04-29 07:40:13.750239 cg-60.4.6/tests/fixtures/apps/demultiplexing/flow_cells/170517_ST-E00266_0210_BHJCFFALXX/HJCFFALXX_bcl2fastq_raw.json
--rw-r--r--   0        0        0     1827 2024-04-29 07:40:13.750239 cg-60.4.6/tests/fixtures/apps/demultiplexing/flow_cells/170517_ST-E00266_0210_BHJCFFALXX/HJCFFALXX_bcl_convert_raw.json
--rw-r--r--   0        0        0       78 2024-04-29 07:40:13.750239 cg-60.4.6/tests/fixtures/apps/demultiplexing/flow_cells/170517_ST-E00266_0210_BHJCFFALXX/README.txt
--rw-r--r--   0        0        0        0 2024-04-29 07:40:13.750239 cg-60.4.6/tests/fixtures/apps/demultiplexing/flow_cells/170517_ST-E00266_0210_BHJCFFALXX/RTAComplete.txt
--rw-r--r--   0        0        0     6895 2024-04-29 07:40:13.750239 cg-60.4.6/tests/fixtures/apps/demultiplexing/flow_cells/170517_ST-E00266_0210_BHJCFFALXX/RTAConfiguration.xml
--rw-r--r--   0        0        0       37 2024-04-29 07:40:13.750239 cg-60.4.6/tests/fixtures/apps/demultiplexing/flow_cells/170517_ST-E00266_0210_BHJCFFALXX/RTARead1Complete.txt
--rw-r--r--   0        0        0       36 2024-04-29 07:40:13.750239 cg-60.4.6/tests/fixtures/apps/demultiplexing/flow_cells/170517_ST-E00266_0210_BHJCFFALXX/RTARead2Complete.txt
--rw-r--r--   0        0        0       36 2024-04-29 07:40:13.750239 cg-60.4.6/tests/fixtures/apps/demultiplexing/flow_cells/170517_ST-E00266_0210_BHJCFFALXX/RTARead3Complete.txt
--rw-r--r--   0        0        0    24755 2024-04-29 07:40:13.750239 cg-60.4.6/tests/fixtures/apps/demultiplexing/flow_cells/170517_ST-E00266_0210_BHJCFFALXX/RunInfo.xml
--rw-r--r--   0        0        0      692 2024-04-29 07:40:13.750239 cg-60.4.6/tests/fixtures/apps/demultiplexing/flow_cells/170517_ST-E00266_0210_BHJCFFALXX/SampleSheet.csv
--rw-r--r--   0        0        0      724 2024-04-29 07:40:13.750239 cg-60.4.6/tests/fixtures/apps/demultiplexing/flow_cells/170517_ST-E00266_0210_BHJCFFALXX/SampleSheet_bcl2fastq.csv
--rw-r--r--   0        0        0       61 2024-04-29 07:40:13.750239 cg-60.4.6/tests/fixtures/apps/demultiplexing/flow_cells/170517_ST-E00266_0210_BHJCFFALXX/SequencingComplete.txt
--rw-r--r--   0        0        0     5775 2024-04-29 07:40:13.750239 cg-60.4.6/tests/fixtures/apps/demultiplexing/flow_cells/170517_ST-E00266_0210_BHJCFFALXX/runParameters.xml
--rw-r--r--   0        0        0        0 2024-04-29 07:40:13.750239 cg-60.4.6/tests/fixtures/apps/demultiplexing/flow_cells/180508_ST-E00269_0269_AHL32LCCXY/CopyComplete.txt
--rw-r--r--   0        0        0     2282 2024-04-29 07:40:13.750239 cg-60.4.6/tests/fixtures/apps/demultiplexing/flow_cells/180508_ST-E00269_0269_AHL32LCCXY/HL32LCCXY_bcl2fastq_raw.json
--rw-r--r--   0        0        0     1632 2024-04-29 07:40:13.750239 cg-60.4.6/tests/fixtures/apps/demultiplexing/flow_cells/180508_ST-E00269_0269_AHL32LCCXY/HL32LCCXY_bcl_convert_raw.json
--rw-r--r--   0        0        0       76 2024-04-29 07:40:13.750239 cg-60.4.6/tests/fixtures/apps/demultiplexing/flow_cells/180508_ST-E00269_0269_AHL32LCCXY/README.txt
--rw-r--r--   0        0        0        0 2024-04-29 07:40:13.750239 cg-60.4.6/tests/fixtures/apps/demultiplexing/flow_cells/180508_ST-E00269_0269_AHL32LCCXY/RTAComplete.txt
--rw-r--r--   0        0        0     6912 2024-04-29 07:40:13.750239 cg-60.4.6/tests/fixtures/apps/demultiplexing/flow_cells/180508_ST-E00269_0269_AHL32LCCXY/RTAConfiguration.xml
--rw-r--r--   0        0        0       36 2024-04-29 07:40:13.750239 cg-60.4.6/tests/fixtures/apps/demultiplexing/flow_cells/180508_ST-E00269_0269_AHL32LCCXY/RTARead1Complete.txt
--rw-r--r--   0        0        0       36 2024-04-29 07:40:13.750239 cg-60.4.6/tests/fixtures/apps/demultiplexing/flow_cells/180508_ST-E00269_0269_AHL32LCCXY/RTARead2Complete.txt
--rw-r--r--   0        0        0       36 2024-04-29 07:40:13.750239 cg-60.4.6/tests/fixtures/apps/demultiplexing/flow_cells/180508_ST-E00269_0269_AHL32LCCXY/RTARead3Complete.txt
--rw-r--r--   0        0        0       36 2024-04-29 07:40:13.750239 cg-60.4.6/tests/fixtures/apps/demultiplexing/flow_cells/180508_ST-E00269_0269_AHL32LCCXY/RTARead4Complete.txt
--rw-r--r--   0        0        0    24814 2024-04-29 07:40:13.750239 cg-60.4.6/tests/fixtures/apps/demultiplexing/flow_cells/180508_ST-E00269_0269_AHL32LCCXY/RunInfo.xml
--rw-r--r--   0        0        0      814 2024-04-29 07:40:13.750239 cg-60.4.6/tests/fixtures/apps/demultiplexing/flow_cells/180508_ST-E00269_0269_AHL32LCCXY/SampleSheet.csv
--rw-r--r--   0        0        0      660 2024-04-29 07:40:13.750239 cg-60.4.6/tests/fixtures/apps/demultiplexing/flow_cells/180508_ST-E00269_0269_AHL32LCCXY/SampleSheet_bcl2fastq.csv
--rw-r--r--   0        0        0       61 2024-04-29 07:40:13.750239 cg-60.4.6/tests/fixtures/apps/demultiplexing/flow_cells/180508_ST-E00269_0269_AHL32LCCXY/SequencingComplete.txt
--rw-r--r--   0        0        0     5853 2024-04-29 07:40:13.750239 cg-60.4.6/tests/fixtures/apps/demultiplexing/flow_cells/180508_ST-E00269_0269_AHL32LCCXY/runParameters.xml
--rw-r--r--   0        0        0        0 2024-04-29 07:40:13.750239 cg-60.4.6/tests/fixtures/apps/demultiplexing/flow_cells/180509_D00450_0598_BHGYFNBCX2/CopyComplete.txt
--rw-r--r--   0        0        0    21848 2024-04-29 07:40:13.750239 cg-60.4.6/tests/fixtures/apps/demultiplexing/flow_cells/180509_D00450_0598_BHGYFNBCX2/HGYFNBCX2_bcl2fastq_raw.json
--rw-r--r--   0        0        0    15512 2024-04-29 07:40:13.750239 cg-60.4.6/tests/fixtures/apps/demultiplexing/flow_cells/180509_D00450_0598_BHGYFNBCX2/HGYFNBCX2_bcl_convert_raw.json
--rw-r--r--   0        0        0       79 2024-04-29 07:40:13.750239 cg-60.4.6/tests/fixtures/apps/demultiplexing/flow_cells/180509_D00450_0598_BHGYFNBCX2/README.txt
--rw-r--r--   0        0        0        0 2024-04-29 07:40:13.750239 cg-60.4.6/tests/fixtures/apps/demultiplexing/flow_cells/180509_D00450_0598_BHGYFNBCX2/RTAComplete.txt
--rw-r--r--   0        0        0      756 2024-04-29 07:40:13.750239 cg-60.4.6/tests/fixtures/apps/demultiplexing/flow_cells/180509_D00450_0598_BHGYFNBCX2/RunInfo.xml
--rw-r--r--   0        0        0     4118 2024-04-29 07:40:13.750239 cg-60.4.6/tests/fixtures/apps/demultiplexing/flow_cells/180509_D00450_0598_BHGYFNBCX2/SampleSheet.csv
--rw-r--r--   0        0        0     1408 2024-04-29 07:40:13.750239 cg-60.4.6/tests/fixtures/apps/demultiplexing/flow_cells/180509_D00450_0598_BHGYFNBCX2/SampleSheet_bcl2fastq.csv
--rw-r--r--   0        0        0     5326 2024-04-29 07:40:13.750239 cg-60.4.6/tests/fixtures/apps/demultiplexing/flow_cells/180509_D00450_0598_BHGYFNBCX2/runParameters.xml
--rw-r--r--   0        0        0        0 2024-04-29 07:40:13.750239 cg-60.4.6/tests/fixtures/apps/demultiplexing/flow_cells/181005_D00410_0735_BHM2LNBCX2/CopyComplete.txt
--rw-r--r--   0        0        0    15041 2024-04-29 07:40:13.750239 cg-60.4.6/tests/fixtures/apps/demultiplexing/flow_cells/181005_D00410_0735_BHM2LNBCX2/HM2LNBCX2_bcl2fastq_raw.json
--rw-r--r--   0        0        0    10649 2024-04-29 07:40:13.750239 cg-60.4.6/tests/fixtures/apps/demultiplexing/flow_cells/181005_D00410_0735_BHM2LNBCX2/HM2LNBCX2_bcl_convert_raw.json
--rw-r--r--   0        0        0       81 2024-04-29 07:40:13.750239 cg-60.4.6/tests/fixtures/apps/demultiplexing/flow_cells/181005_D00410_0735_BHM2LNBCX2/README.txt
--rw-r--r--   0        0        0        0 2024-04-29 07:40:13.750239 cg-60.4.6/tests/fixtures/apps/demultiplexing/flow_cells/181005_D00410_0735_BHM2LNBCX2/RTAComplete.txt
--rw-r--r--   0        0        0      755 2024-04-29 07:40:13.750239 cg-60.4.6/tests/fixtures/apps/demultiplexing/flow_cells/181005_D00410_0735_BHM2LNBCX2/RunInfo.xml
--rw-r--r--   0        0        0     2878 2024-04-29 07:40:13.750239 cg-60.4.6/tests/fixtures/apps/demultiplexing/flow_cells/181005_D00410_0735_BHM2LNBCX2/SampleSheet.csv
--rw-r--r--   0        0        0      928 2024-04-29 07:40:13.750239 cg-60.4.6/tests/fixtures/apps/demultiplexing/flow_cells/181005_D00410_0735_BHM2LNBCX2/SampleSheet_bcl2fastq.csv
--rw-r--r--   0        0        0     5359 2024-04-29 07:40:13.750239 cg-60.4.6/tests/fixtures/apps/demultiplexing/flow_cells/181005_D00410_0735_BHM2LNBCX2/runParameters.xml
--rw-r--r--   0        0        0        0 2024-04-29 07:40:13.750239 cg-60.4.6/tests/fixtures/apps/demultiplexing/flow_cells/190927_A00689_0069_BHLYWYDSXX/CopyComplete.txt
--rw-r--r--   0        0        0    27887 2024-04-29 07:40:13.750239 cg-60.4.6/tests/fixtures/apps/demultiplexing/flow_cells/190927_A00689_0069_BHLYWYDSXX/CorrectSampleSheet.csv
--rw-r--r--   0        0        0   141870 2024-04-29 07:40:13.754239 cg-60.4.6/tests/fixtures/apps/demultiplexing/flow_cells/190927_A00689_0069_BHLYWYDSXX/HLYWYDSXX_bcl2fastq_raw.json
--rwxr-xr-x   0        0        0   122682 2024-04-29 07:40:13.754239 cg-60.4.6/tests/fixtures/apps/demultiplexing/flow_cells/190927_A00689_0069_BHLYWYDSXX/HLYWYDSXX_bcl_convert_raw.json
--rw-r--r--   0        0        0      243 2024-04-29 07:40:13.754239 cg-60.4.6/tests/fixtures/apps/demultiplexing/flow_cells/190927_A00689_0069_BHLYWYDSXX/README.txt
--rw-r--r--   0        0        0    28230 2024-04-29 07:40:13.754239 cg-60.4.6/tests/fixtures/apps/demultiplexing/flow_cells/190927_A00689_0069_BHLYWYDSXX/RTA3.cfg
--rw-r--r--   0        0        0        0 2024-04-29 07:40:13.754239 cg-60.4.6/tests/fixtures/apps/demultiplexing/flow_cells/190927_A00689_0069_BHLYWYDSXX/RTAComplete.txt
--rw-r--r--   0        0        0    94426 2024-04-29 07:40:13.754239 cg-60.4.6/tests/fixtures/apps/demultiplexing/flow_cells/190927_A00689_0069_BHLYWYDSXX/RunInfo.xml
--rw-r--r--   0        0        0     5819 2024-04-29 07:40:13.754239 cg-60.4.6/tests/fixtures/apps/demultiplexing/flow_cells/190927_A00689_0069_BHLYWYDSXX/RunParameters.xml
--rw-r--r--   0        0        0        0 2024-04-29 07:40:13.754239 cg-60.4.6/tests/fixtures/apps/demultiplexing/flow_cells/190927_A00689_0069_BHLYWYDSXX/SequenceComplete.txt
--rw-r--r--   0        0        0     1757 2024-04-29 07:40:13.754239 cg-60.4.6/tests/fixtures/apps/demultiplexing/flow_cells/201203_D00483_0200_AHVKJCDRXX/HVKJCDRXX_demultiplex.stderr
--rw-r--r--   0        0        0     1757 2024-04-29 07:40:13.754239 cg-60.4.6/tests/fixtures/apps/demultiplexing/flow_cells/201203_D00483_0200_AHVKJCDRXX/HVKJCDRXX_demultiplex.stdout
--rw-r--r--   0        0        0    47522 2024-04-29 07:40:13.754239 cg-60.4.6/tests/fixtures/apps/demultiplexing/flow_cells/201203_D00483_0200_AHVKJCDRXX/HVKJCDRXX_raw.json
--rw-r--r--   0        0        0       12 2024-04-29 07:40:13.754239 cg-60.4.6/tests/fixtures/apps/demultiplexing/flow_cells/201203_D00483_0200_AHVKJCDRXX/README.txt
--rw-r--r--   0        0        0        0 2024-04-29 07:40:13.754239 cg-60.4.6/tests/fixtures/apps/demultiplexing/flow_cells/201203_D00483_0200_AHVKJCDRXX/RTAComplete.txt
--rw-r--r--   0        0        0     6666 2024-04-29 07:40:13.754239 cg-60.4.6/tests/fixtures/apps/demultiplexing/flow_cells/201203_D00483_0200_AHVKJCDRXX/RunParameters.xml
--rw-r--r--   0        0        0      254 2024-04-29 07:40:13.754239 cg-60.4.6/tests/fixtures/apps/demultiplexing/flow_cells/201203_D00483_0200_AHVKJCDRXX/SampleSheet.csv
--rw-r--r--   0        0        0        0 2024-04-29 07:40:13.754239 cg-60.4.6/tests/fixtures/apps/demultiplexing/flow_cells/201203_D00483_0200_AHVKJCDRXX/copycomplete.txt
--rw-r--r--   0        0        0        0 2024-04-29 07:40:13.754239 cg-60.4.6/tests/fixtures/apps/demultiplexing/flow_cells/201203_D00483_0200_AHVKJCDRXX/delivery.txt
--rw-r--r--   0        0        0        0 2024-04-29 07:40:13.754239 cg-60.4.6/tests/fixtures/apps/demultiplexing/flow_cells/201203_D00483_0200_AHVKJCDRXX/demuxstarted.txt
--rwxr-xr-x   0        0        0    47434 2024-04-29 07:40:13.754239 cg-60.4.6/tests/fixtures/apps/demultiplexing/flow_cells/20231108_LH00188_0028_B22F52TLT3/22F52TLT3_raw.json
--rw-r--r--   0        0        0        0 2024-04-29 07:40:13.754239 cg-60.4.6/tests/fixtures/apps/demultiplexing/flow_cells/20231108_LH00188_0028_B22F52TLT3/CopyComplete.txt
--rw-r--r--   0        0        0    10950 2024-04-29 07:40:13.754239 cg-60.4.6/tests/fixtures/apps/demultiplexing/flow_cells/20231108_LH00188_0028_B22F52TLT3/CorrectSampleSheet.csv
--rw-r--r--   0        0        0      225 2024-04-29 07:40:13.754239 cg-60.4.6/tests/fixtures/apps/demultiplexing/flow_cells/20231108_LH00188_0028_B22F52TLT3/Manifest.tsv
--rw-r--r--   0        0        0       55 2024-04-29 07:40:13.754239 cg-60.4.6/tests/fixtures/apps/demultiplexing/flow_cells/20231108_LH00188_0028_B22F52TLT3/README.txt
--rwxr-xr-x   0        0        0     2493 2024-04-29 07:40:13.754239 cg-60.4.6/tests/fixtures/apps/demultiplexing/flow_cells/20231108_LH00188_0028_B22F52TLT3/RTA.cfg
--rwxr-xr-x   0        0        0        1 2024-04-29 07:40:13.754239 cg-60.4.6/tests/fixtures/apps/demultiplexing/flow_cells/20231108_LH00188_0028_B22F52TLT3/RTAComplete.txt
--rwxr-xr-x   0        0        0        2 2024-04-29 07:40:13.754239 cg-60.4.6/tests/fixtures/apps/demultiplexing/flow_cells/20231108_LH00188_0028_B22F52TLT3/RTAExited.txt
--rwxr-xr-x   0        0        0      730 2024-04-29 07:40:13.754239 cg-60.4.6/tests/fixtures/apps/demultiplexing/flow_cells/20231108_LH00188_0028_B22F52TLT3/RunCompletionStatus.xml
--rwxr-xr-x   0        0        0    79277 2024-04-29 07:40:13.754239 cg-60.4.6/tests/fixtures/apps/demultiplexing/flow_cells/20231108_LH00188_0028_B22F52TLT3/RunInfo.xml
--rwxr-xr-x   0        0        0     2694 2024-04-29 07:40:13.754239 cg-60.4.6/tests/fixtures/apps/demultiplexing/flow_cells/20231108_LH00188_0028_B22F52TLT3/RunParameters.xml
--rw-r--r--   0        0        0    10950 2024-04-29 07:40:13.754239 cg-60.4.6/tests/fixtures/apps/demultiplexing/flow_cells/20231108_LH00188_0028_B22F52TLT3/SampleSheet.csv
--rw-r--r--   0        0        0        0 2024-04-29 07:40:13.754239 cg-60.4.6/tests/fixtures/apps/demultiplexing/flow_cells/211101_A00187_0615_AHLG5GDRZZ/CopyComplete.txt
--rw-r--r--   0        0        0      509 2024-04-29 07:40:13.754239 cg-60.4.6/tests/fixtures/apps/demultiplexing/flow_cells/211101_A00187_0615_AHLG5GDRZZ/HLG5GDRZZ_demultiplex.stderr
--rw-r--r--   0        0        0     2229 2024-04-29 07:40:13.754239 cg-60.4.6/tests/fixtures/apps/demultiplexing/flow_cells/211101_A00187_0615_AHLG5GDRZZ/HLG5GDRZZ_demultiplex.stdout
--rw-r--r--   0        0        0        0 2024-04-29 07:40:13.754239 cg-60.4.6/tests/fixtures/apps/demultiplexing/flow_cells/211101_A00187_0615_AHLG5GDRZZ/RTAComplete.txt
--rw-r--r--   0        0        0     6665 2024-04-29 07:40:13.754239 cg-60.4.6/tests/fixtures/apps/demultiplexing/flow_cells/211101_A00187_0615_AHLG5GDRZZ/RunParameters.xml
--rw-r--r--   0        0        0      619 2024-04-29 07:40:13.754239 cg-60.4.6/tests/fixtures/apps/demultiplexing/flow_cells/211101_A00187_0615_AHLG5GDRZZ/SampleSheet.csv
--rw-r--r--   0        0        0        0 2024-04-29 07:40:13.754239 cg-60.4.6/tests/fixtures/apps/demultiplexing/flow_cells/230912_A00187_1009_AHK33MDRX3/CopyComplete.txt
--rw-r--r--   0        0        0     4941 2024-04-29 07:40:13.754239 cg-60.4.6/tests/fixtures/apps/demultiplexing/flow_cells/230912_A00187_1009_AHK33MDRX3/CorrectSampleSheet.csv
--rwxr-xr-x   0        0        0    20050 2024-04-29 07:40:13.754239 cg-60.4.6/tests/fixtures/apps/demultiplexing/flow_cells/230912_A00187_1009_AHK33MDRX3/HK33MDRX3_bcl_convert_raw.json
--rw-r--r--   0        0        0        0 2024-04-29 07:40:13.754239 cg-60.4.6/tests/fixtures/apps/demultiplexing/flow_cells/230912_A00187_1009_AHK33MDRX3/HK33MDRX3_demultiplex.stderr
--rw-r--r--   0        0        0        0 2024-04-29 07:40:13.754239 cg-60.4.6/tests/fixtures/apps/demultiplexing/flow_cells/230912_A00187_1009_AHK33MDRX3/HK33MDRX3_demultiplex.stdout
--rw-r--r--   0        0        0      244 2024-04-29 07:40:13.754239 cg-60.4.6/tests/fixtures/apps/demultiplexing/flow_cells/230912_A00187_1009_AHK33MDRX3/README.txt
--rw-r--r--   0        0        0     6391 2024-04-29 07:40:13.754239 cg-60.4.6/tests/fixtures/apps/demultiplexing/flow_cells/230912_A00187_1009_AHK33MDRX3/RTA3.cfg
--rw-r--r--   0        0        0        0 2024-04-29 07:40:13.754239 cg-60.4.6/tests/fixtures/apps/demultiplexing/flow_cells/230912_A00187_1009_AHK33MDRX3/RTAComplete.txt
--rw-r--r--   0        0        0    16428 2024-04-29 07:40:13.754239 cg-60.4.6/tests/fixtures/apps/demultiplexing/flow_cells/230912_A00187_1009_AHK33MDRX3/RunInfo.xml
--rw-r--r--   0        0        0     6728 2024-04-29 07:40:13.754239 cg-60.4.6/tests/fixtures/apps/demultiplexing/flow_cells/230912_A00187_1009_AHK33MDRX3/RunParameters.xml
--rw-r--r--   0        0        0     5127 2024-04-29 07:40:13.754239 cg-60.4.6/tests/fixtures/apps/demultiplexing/flow_cells/230912_A00187_1009_AHK33MDRX3/SampleSheet.csv
--rw-r--r--   0        0        0        0 2024-04-29 07:40:13.754239 cg-60.4.6/tests/fixtures/apps/demultiplexing/flow_cells/230912_A00187_1009_AHK33MDRX3/SequenceComplete.txt
--rw-r--r--   0        0        0        0 2024-04-29 07:40:13.754239 cg-60.4.6/tests/fixtures/apps/demultiplexing/flow_cells/230912_A00187_1009_AHK33MDRX3/demuxstarted.txt
--rw-r--r--   0        0        0      133 2024-04-29 07:40:13.754239 cg-60.4.6/tests/fixtures/apps/demultiplexing/flow_cells_broken/170517_ST-E00266_0210_BHJCFFALXX/README.txt
--rw-r--r--   0        0        0      724 2024-04-29 07:40:13.754239 cg-60.4.6/tests/fixtures/apps/demultiplexing/flow_cells_broken/170517_ST-E00266_0210_BHJCFFALXX/SampleSheet.csv
--rw-r--r--   0        0        0     5775 2024-04-29 07:40:13.754239 cg-60.4.6/tests/fixtures/apps/demultiplexing/flow_cells_broken/170517_ST-E00266_0210_BHJCFFALXX/runParameters.xml
--rw-r--r--   0        0        0      124 2024-04-29 07:40:13.754239 cg-60.4.6/tests/fixtures/apps/demultiplexing/flow_cells_broken/180509_D00450_0598_BHGYFNBCX2/README.txt
--rw-r--r--   0        0        0      310 2024-04-29 07:40:13.754239 cg-60.4.6/tests/fixtures/apps/demultiplexing/flow_cells_broken/190927_A00689_0069_BHLYWYDSXX/README.txt
--rw-r--r--   0        0        0     5819 2024-04-29 07:40:13.754239 cg-60.4.6/tests/fixtures/apps/demultiplexing/flow_cells_broken/190927_A00689_0069_BHLYWYDSXX/RunParameters.xml
--rw-r--r--   0        0        0      122 2024-04-29 07:40:13.754239 cg-60.4.6/tests/fixtures/apps/demultiplexing/flow_cells_broken/20231108_LH00188_0028_B22F52TLT3/README.txt
--rwxr-xr-x   0        0        0     2694 2024-04-29 07:40:13.754239 cg-60.4.6/tests/fixtures/apps/demultiplexing/flow_cells_broken/20231108_LH00188_0028_B22F52TLT3/RunParameters.xml
--rw-r--r--   0        0        0      311 2024-04-29 07:40:13.754239 cg-60.4.6/tests/fixtures/apps/demultiplexing/flow_cells_broken/230912_A00187_1009_AHK33MDRX3/README.txt
--rw-r--r--   0        0        0     6728 2024-04-29 07:40:13.754239 cg-60.4.6/tests/fixtures/apps/demultiplexing/flow_cells_broken/230912_A00187_1009_AHK33MDRX3/RunParameters.xml
--rw-r--r--   0        0        0        0 2024-04-29 07:40:13.754239 cg-60.4.6/tests/fixtures/apps/demultiplexing/flow_cells_demux_all/211101_A00187_0615_AHLG5GDRXY/CopyComplete.txt
--rw-r--r--   0        0        0      509 2024-04-29 07:40:13.754239 cg-60.4.6/tests/fixtures/apps/demultiplexing/flow_cells_demux_all/211101_A00187_0615_AHLG5GDRXY/HLG5GDRXY_demultiplex.stderr
--rw-r--r--   0        0        0     2229 2024-04-29 07:40:13.754239 cg-60.4.6/tests/fixtures/apps/demultiplexing/flow_cells_demux_all/211101_A00187_0615_AHLG5GDRXY/HLG5GDRXY_demultiplex.stdout
--rw-r--r--   0        0        0        0 2024-04-29 07:40:13.754239 cg-60.4.6/tests/fixtures/apps/demultiplexing/flow_cells_demux_all/211101_A00187_0615_AHLG5GDRXY/RTAComplete.txt
--rw-r--r--   0        0        0     6665 2024-04-29 07:40:13.754239 cg-60.4.6/tests/fixtures/apps/demultiplexing/flow_cells_demux_all/211101_A00187_0615_AHLG5GDRXY/RunParameters.xml
--rw-r--r--   0        0        0      399 2024-04-29 07:40:13.754239 cg-60.4.6/tests/fixtures/apps/demultiplexing/flow_cells_demux_all/211101_A00187_0615_AHLG5GDRXY/SampleSheet.csv
--rw-r--r--   0        0        0        0 2024-04-29 07:40:13.754239 cg-60.4.6/tests/fixtures/apps/demultiplexing/flow_cells_demux_all/211101_A00187_0615_AHLG5GDRZZ/CopyComplete.txt
--rw-r--r--   0        0        0      509 2024-04-29 07:40:13.754239 cg-60.4.6/tests/fixtures/apps/demultiplexing/flow_cells_demux_all/211101_A00187_0615_AHLG5GDRZZ/HLG5GDRZZ_demultiplex.stderr
--rw-r--r--   0        0        0     2229 2024-04-29 07:40:13.758239 cg-60.4.6/tests/fixtures/apps/demultiplexing/flow_cells_demux_all/211101_A00187_0615_AHLG5GDRZZ/HLG5GDRZZ_demultiplex.stdout
--rw-r--r--   0        0        0        0 2024-04-29 07:40:13.758239 cg-60.4.6/tests/fixtures/apps/demultiplexing/flow_cells_demux_all/211101_A00187_0615_AHLG5GDRZZ/RTAComplete.txt
--rw-r--r--   0        0        0     6665 2024-04-29 07:40:13.758239 cg-60.4.6/tests/fixtures/apps/demultiplexing/flow_cells_demux_all/211101_A00187_0615_AHLG5GDRZZ/RunParameters.xml
--rw-r--r--   0        0        0      399 2024-04-29 07:40:13.758239 cg-60.4.6/tests/fixtures/apps/demultiplexing/flow_cells_demux_all/211101_A00187_0615_AHLG5GDRZZ/SampleSheet.csv
--rw-r--r--   0        0        0        0 2024-04-29 07:40:13.758239 cg-60.4.6/tests/fixtures/apps/demultiplexing/nanopore/experiment_name/sample_1/20231205_1618_3B_PAS86456_72d9fceb/fastq_pass/PAS86456_pass_72d9fceb_8a4fd683_0.fastq.gz
--rw-r--r--   0        0        0        0 2024-04-29 07:40:13.758239 cg-60.4.6/tests/fixtures/apps/demultiplexing/nanopore/experiment_name/sample_1/20231205_1618_3B_PAS86456_72d9fceb/fastq_pass/PAS86456_pass_72d9fceb_8a4fd683_1.fastq.gz
--rw-r--r--   0        0        0        0 2024-04-29 07:40:13.758239 cg-60.4.6/tests/fixtures/apps/demultiplexing/nanopore/experiment_name/sample_1/20231205_1618_3B_PAS86456_72d9fceb/final_summary_PAS86456_72d9fceb_8a4fd683.txt
--rw-r--r--   0        0        0        0 2024-04-29 07:40:13.758239 cg-60.4.6/tests/fixtures/apps/demultiplexing/nanopore/experiment_name/sample_1/20231205_1618_3B_PAS86456_72d9fceb/pod5_pass/PAS86456_pass_72d9fceb_8a4fd683_0.pod5
--rw-r--r--   0        0        0        0 2024-04-29 07:40:13.758239 cg-60.4.6/tests/fixtures/apps/demultiplexing/nanopore/experiment_name/sample_1/20231205_1618_3B_PAS86456_72d9fceb/pod5_pass/PAS86456_pass_72d9fceb_8a4fd683_1.pod5
--rw-r--r--   0        0        0        0 2024-04-29 07:40:13.758239 cg-60.4.6/tests/fixtures/apps/demultiplexing/nanopore/experiment_name/sample_2/20231205_1618_3D_PAS97781_595b5663/fastq_pass/PAS97781_pass_595b5663_efc7f02e_0.fastq.gz
--rw-r--r--   0        0        0        0 2024-04-29 07:40:13.758239 cg-60.4.6/tests/fixtures/apps/demultiplexing/nanopore/experiment_name/sample_2/20231205_1618_3D_PAS97781_595b5663/fastq_pass/PAS97781_pass_595b5663_efc7f02e_1.fastq.gz
--rw-r--r--   0        0        0        0 2024-04-29 07:40:13.758239 cg-60.4.6/tests/fixtures/apps/demultiplexing/nanopore/experiment_name/sample_2/20231205_1618_3D_PAS97781_595b5663/final_summary_PAS97781_595b5663_efc7f02e.txt
--rw-r--r--   0        0        0        0 2024-04-29 07:40:13.758239 cg-60.4.6/tests/fixtures/apps/demultiplexing/nanopore/experiment_name/sample_2/20231205_1618_3D_PAS97781_595b5663/pod5_pass/PAS97781_pass_595b5663_efc7f02e_0.pod5
--rw-r--r--   0        0        0        0 2024-04-29 07:40:13.758239 cg-60.4.6/tests/fixtures/apps/demultiplexing/nanopore/experiment_name/sample_2/20231205_1618_3D_PAS97781_595b5663/pod5_pass/PAS97781_pass_595b5663_efc7f02e_1.pod5
--rw-r--r--   0        0        0     5319 2024-04-29 07:40:13.758239 cg-60.4.6/tests/fixtures/apps/demultiplexing/run_parameters/RunParameters_hiseq_2500_different_index_cycles.xml
--rw-r--r--   0        0        0     5944 2024-04-29 07:40:13.758239 cg-60.4.6/tests/fixtures/apps/demultiplexing/run_parameters/RunParameters_novaseq_6000_different_index_cycles.xml
--rwxr-xr-x   0        0        0     2603 2024-04-29 07:40:13.758239 cg-60.4.6/tests/fixtures/apps/demultiplexing/run_parameters/RunParameters_novaseq_X_different_index_cycles.xml
--rwxr-xr-x   0        0        0     2597 2024-04-29 07:40:13.758239 cg-60.4.6/tests/fixtures/apps/demultiplexing/run_parameters/RunParameters_novaseq_X_wrong_instrument.xml
--rw-r--r--   0        0        0     5899 2024-04-29 07:40:13.758239 cg-60.4.6/tests/fixtures/apps/demultiplexing/run_parameters/RunParameters_novaseq_no_software_nor_reagent_version.xml
--rw-r--r--   0        0        0     4941 2024-04-29 07:40:13.758239 cg-60.4.6/tests/fixtures/apps/demultiplexing/sample_sheets/novaseq_6000_sample_sheet_with_reversed_cycles.csv
--rw-r--r--   0        0        0    10950 2024-04-29 07:40:13.758239 cg-60.4.6/tests/fixtures/apps/demultiplexing/sample_sheets/novaseq_x_sample_sheet_with_forward_cycles.csv
--rw-r--r--   0        0        0        0 2024-04-29 07:40:13.758239 cg-60.4.6/tests/fixtures/apps/demultiplexing/spring/dummy_run_001.spring
--rw-r--r--   0        0        0        0 2024-04-29 07:40:13.758239 cg-60.4.6/tests/fixtures/apps/demultiplexing/spring/dummy_run_002.spring
--rw-r--r--   0        0        0        0 2024-04-29 07:40:13.758239 cg-60.4.6/tests/fixtures/apps/demultiplexing/spring/dummy_spring_meta_data.json
--rw-r--r--   0        0        0        0 2024-04-29 07:40:13.758239 cg-60.4.6/tests/fixtures/apps/fluffy/2020-23219-05/2020-23219-05.WCXpredict_aberrations.filt.bed
--rw-r--r--   0        0        0     5554 2024-04-29 07:40:13.758239 cg-60.4.6/tests/fixtures/apps/fluffy/SampleSheet.csv
--rw-r--r--   0        0        0      901 2024-04-29 07:40:13.758239 cg-60.4.6/tests/fixtures/apps/fluffy/deliverables.yaml
--rw-r--r--   0        0        0        0 2024-04-29 07:40:13.758239 cg-60.4.6/tests/fixtures/apps/fluffy/fluffy_fastq.fastq.gz
--rw-r--r--   0        0        0        0 2024-04-29 07:40:13.758239 cg-60.4.6/tests/fixtures/apps/fluffy/multiqc_report.html
--rw-r--r--   0        0        0        0 2024-04-29 07:40:13.758239 cg-60.4.6/tests/fixtures/apps/fluffy/summary.csv
--rw-r--r--   0        0        0        0 2024-04-29 07:40:13.758239 cg-60.4.6/tests/fixtures/apps/gt/yellowhog.bcf
--rw-r--r--   0        0        0     5114 2024-04-29 07:40:13.758239 cg-60.4.6/tests/fixtures/apps/madeline/madeline.xml
--rw-r--r--   0        0        0        0 2024-04-29 07:40:13.758239 cg-60.4.6/tests/fixtures/apps/mip/case_file.txt
--rw-r--r--   0        0        0     3241 2024-04-29 07:40:13.758239 cg-60.4.6/tests/fixtures/apps/mip/case_metrics_deliverables.yaml
--rw-r--r--   0        0        0    21811 2024-04-29 07:40:13.758239 cg-60.4.6/tests/fixtures/apps/mip/dna/store/case_config.yaml
--rw-r--r--   0        0        0    23364 2024-04-29 07:40:13.758239 cg-60.4.6/tests/fixtures/apps/mip/dna/store/case_id_deliverables.yaml
--rw-r--r--   0        0        0    37367 2024-04-29 07:40:13.758239 cg-60.4.6/tests/fixtures/apps/mip/dna/store/case_qc_sample_info.yaml
--rw-r--r--   0        0        0       16 2024-04-29 07:40:13.758239 cg-60.4.6/tests/fixtures/apps/mip/dna/store/empty_case_config.yaml
--rw-r--r--   0        0        0       16 2024-04-29 07:40:13.758239 cg-60.4.6/tests/fixtures/apps/mip/dna/store/empty_case_metrics_deliverables.yaml
--rw-r--r--   0        0        0       16 2024-04-29 07:40:13.758239 cg-60.4.6/tests/fixtures/apps/mip/dna/store/empty_case_qc_sample_info.yaml
--rw-r--r--   0        0        0      123 2024-04-29 07:40:13.758239 cg-60.4.6/tests/fixtures/apps/mip/dna/store/empty_delivery_report.html
--rw-r--r--   0        0        0    62741 2024-04-29 07:40:13.758239 cg-60.4.6/tests/fixtures/apps/mip/dna/store/yellowhog_clinical_selected.vcf
--rw-r--r--   0        0        0    11242 2024-04-29 07:40:13.758239 cg-60.4.6/tests/fixtures/apps/mip/rna/case_config.yaml
--rw-r--r--   0        0        0    12164 2024-04-29 07:40:13.758239 cg-60.4.6/tests/fixtures/apps/mip/rna/case_qc_sampleinfo.yaml
--rw-r--r--   0        0        0     5231 2024-04-29 07:40:13.758239 cg-60.4.6/tests/fixtures/apps/mip/rna/store/bundle_data.yaml
--rw-r--r--   0        0        0     9774 2024-04-29 07:40:13.758239 cg-60.4.6/tests/fixtures/apps/mip/rna/store/case_config.yaml
--rw-r--r--   0        0        0     4624 2024-04-29 07:40:13.758239 cg-60.4.6/tests/fixtures/apps/mip/rna/store/case_id_deliverables.yaml
--rw-r--r--   0        0        0    13666 2024-04-29 07:40:13.758239 cg-60.4.6/tests/fixtures/apps/mip/rna/store/case_qc_sample_info.yaml
--rw-r--r--   0        0        0        0 2024-04-29 07:40:13.758239 cg-60.4.6/tests/fixtures/apps/mip/sample_file.txt
--rw-r--r--   0        0        0     1885 2024-04-29 07:40:13.758239 cg-60.4.6/tests/fixtures/apps/scout/643594.config.yaml
--rw-r--r--   0        0        0     6027 2024-04-29 07:40:13.758239 cg-60.4.6/tests/fixtures/apps/scout/case_export.json
--rw-r--r--   0        0        0     9349 2024-04-29 07:40:13.758239 cg-60.4.6/tests/fixtures/apps/scout/export_causatives.json
--rw-r--r--   0        0        0     1315 2024-04-29 07:40:13.758239 cg-60.4.6/tests/fixtures/apps/scout/none_case_export.json
--rw-r--r--   0        0        0     3518 2024-04-29 07:40:13.758239 cg-60.4.6/tests/fixtures/apps/scout/other_sex_case.json
--rw-r--r--   0        0        0     8874 2024-04-29 07:40:13.758239 cg-60.4.6/tests/fixtures/apps/scout/panel_export.bed
--rw-r--r--   0        0        0     4169 2024-04-29 07:40:13.758239 cg-60.4.6/tests/fixtures/apps/scout/panel_export.csv
--rw-r--r--   0        0        0      619 2024-04-29 07:40:13.758239 cg-60.4.6/tests/fixtures/apps/sequencing_metrics_parser/230622_A00621_0864_AHY7FFDRX2/SampleSheet.csv
--rw-r--r--   0        0        0    63569 2024-04-29 07:40:13.758239 cg-60.4.6/tests/fixtures/apps/sequencing_metrics_parser/230622_A00621_0864_AHY7FFDRX2/Unaligned/Reports/Adapter_Metrics.csv
--rw-r--r--   0        0        0    42478 2024-04-29 07:40:13.758239 cg-60.4.6/tests/fixtures/apps/sequencing_metrics_parser/230622_A00621_0864_AHY7FFDRX2/Unaligned/Reports/Demultiplex_Stats.csv
--rw-r--r--   0        0        0    69708 2024-04-29 07:40:13.762239 cg-60.4.6/tests/fixtures/apps/sequencing_metrics_parser/230622_A00621_0864_AHY7FFDRX2/Unaligned/Reports/Quality_Metrics.csv
--rw-r--r--   0        0        0       42 2024-04-29 07:40:13.762239 cg-60.4.6/tests/fixtures/apps/shipping/scout-deploy.yaml
--rw-r--r--   0        0        0     1036 2024-04-29 07:40:13.762239 cg-60.4.6/tests/fixtures/cgweb_orders/balsamic.json
--rw-r--r--   0        0        0     1104 2024-04-29 07:40:13.762239 cg-60.4.6/tests/fixtures/cgweb_orders/fastq.json
--rw-r--r--   0        0        0     1313 2024-04-29 07:40:13.762239 cg-60.4.6/tests/fixtures/cgweb_orders/metagenome.json
--rw-r--r--   0        0        0     3038 2024-04-29 07:40:13.762239 cg-60.4.6/tests/fixtures/cgweb_orders/microsalt.json
--rw-r--r--   0        0        0     3705 2024-04-29 07:40:13.762239 cg-60.4.6/tests/fixtures/cgweb_orders/mip.json
--rw-r--r--   0        0        0     1364 2024-04-29 07:40:13.762239 cg-60.4.6/tests/fixtures/cgweb_orders/mip_rna.json
--rw-r--r--   0        0        0     2125 2024-04-29 07:40:13.762239 cg-60.4.6/tests/fixtures/cgweb_orders/rml.json
--rw-r--r--   0        0        0     1368 2024-04-29 07:40:13.762239 cg-60.4.6/tests/fixtures/cgweb_orders/rnafusion.json
--rw-r--r--   0        0        0     4684 2024-04-29 07:40:13.762239 cg-60.4.6/tests/fixtures/cgweb_orders/sarscov2.json
--rw-r--r--   0        0        0     5609 2024-04-29 07:40:13.762239 cg-60.4.6/tests/fixtures/data/SampleSheet.csv
--rw-r--r--   0        0        0      511 2024-04-29 07:40:13.762239 cg-60.4.6/tests/fixtures/data/bcl_convert_sample_sheet.csv
--rw-r--r--   0        0        0   258048 2024-04-29 07:40:13.762239 cg-60.4.6/tests/fixtures/data/cgfixture.db
--rw-r--r--   0        0        0        0 2024-04-29 07:40:13.762239 cg-60.4.6/tests/fixtures/data/fastq.fastq.gz
--rw-r--r--   0        0        0    49152 2024-04-29 07:40:13.762239 cg-60.4.6/tests/fixtures/data/hkstore.db
--rw-r--r--   0        0        0       73 2024-04-29 07:40:13.762239 cg-60.4.6/tests/fixtures/data/yellowhog/pedigree.yaml
--rw-r--r--   0        0        0       76 2024-04-29 07:40:13.762239 cg-60.4.6/tests/fixtures/io/casava_five_parts.fastq.gz
--rw-r--r--   0        0        0       90 2024-04-29 07:40:13.762239 cg-60.4.6/tests/fixtures/io/casava_seven_parts.fastq.gz
--rw-r--r--   0        0        0       96 2024-04-29 07:40:13.762239 cg-60.4.6/tests/fixtures/io/casava_ten_parts.fastq.gz
--rw-r--r--   0        0        0      153 2024-04-29 07:40:13.762239 cg-60.4.6/tests/fixtures/io/example.csv
--rw-r--r--   0        0        0       46 2024-04-29 07:40:13.762239 cg-60.4.6/tests/fixtures/io/example.gz
--rw-r--r--   0        0        0      147 2024-04-29 07:40:13.762239 cg-60.4.6/tests/fixtures/io/example.tsv
--rw-r--r--   0        0        0       20 2024-04-29 07:40:13.762239 cg-60.4.6/tests/fixtures/io/example.txt
--rw-r--r--   0        0        0       20 2024-04-29 07:40:13.762239 cg-60.4.6/tests/fixtures/io/example2.txt
--rw-r--r--   0        0        0      582 2024-04-29 07:40:13.762239 cg-60.4.6/tests/fixtures/io/example_json.json
--rw-r--r--   0        0        0      103 2024-04-29 07:40:13.762239 cg-60.4.6/tests/fixtures/io/example_xml.xml
--rw-r--r--   0        0        0       20 2024-04-29 07:40:13.762239 cg-60.4.6/tests/fixtures/meta/qc_metrics/file_with_right_tags.json
--rw-r--r--   0        0        0       20 2024-04-29 07:40:13.762239 cg-60.4.6/tests/fixtures/meta/qc_metrics/file_without_right_tags.json
--rw-r--r--   0        0        0   156910 2024-04-29 07:40:13.766239 cg-60.4.6/tests/fixtures/orderforms/1508.30.balsamic.xlsx
--rw-r--r--   0        0        0   156770 2024-04-29 07:40:13.766239 cg-60.4.6/tests/fixtures/orderforms/1508.30.balsamic_qc.xlsx
--rw-r--r--   0        0        0   156737 2024-04-29 07:40:13.766239 cg-60.4.6/tests/fixtures/orderforms/1508.30.balsamic_umi.xlsx
--rw-r--r--   0        0        0   156582 2024-04-29 07:40:13.766239 cg-60.4.6/tests/fixtures/orderforms/1508.30.fastq.xlsx
--rw-r--r--   0        0        0   155627 2024-04-29 07:40:13.766239 cg-60.4.6/tests/fixtures/orderforms/1508.30.metagenome.xlsx
--rw-r--r--   0        0        0   156850 2024-04-29 07:40:13.766239 cg-60.4.6/tests/fixtures/orderforms/1508.30.mip.xlsx
--rw-r--r--   0        0        0   258580 2024-04-29 07:40:13.766239 cg-60.4.6/tests/fixtures/orderforms/1508.30.mip_rna.xlsx
--rw-r--r--   0        0        0   258342 2024-04-29 07:40:13.766239 cg-60.4.6/tests/fixtures/orderforms/1508.30.rnafusion.xlsx
--rw-r--r--   0        0        0    82677 2024-04-29 07:40:13.770239 cg-60.4.6/tests/fixtures/orderforms/1603.11.microbial.xlsx
--rw-r--r--   0        0        0   149394 2024-04-29 07:40:13.770239 cg-60.4.6/tests/fixtures/orderforms/1604.17.rml.xlsx
--rw-r--r--   0        0        0   223184 2024-04-29 07:40:13.770239 cg-60.4.6/tests/fixtures/orderforms/2184.9.sarscov2.xlsx
--rw-r--r--   0        0        0    18639 2024-04-29 07:40:13.770239 cg-60.4.6/tests/fixtures/orderforms/NIPT-json.json
--rw-r--r--   0        0        0     6052 2024-04-29 07:40:13.770239 cg-60.4.6/tests/fixtures/orderforms/balsamic_uploaded_json_orderform.json
--rw-r--r--   0        0        0     6611 2024-04-29 07:40:13.770239 cg-60.4.6/tests/fixtures/orderforms/mip_uploaded_json_orderform.json
--rw-r--r--   0        0        0     1417 2024-04-29 07:40:13.770239 cg-60.4.6/tests/fixtures/report/case_data.json
--rw-r--r--   0        0        0     1109 2024-04-29 07:40:13.770239 cg-60.4.6/tests/fixtures/report/lims_exported_samples.json
--rw-r--r--   0        0        0     1562 2024-04-29 07:40:13.770239 cg-60.4.6/tests/fixtures/report/lims_family.json
--rw-r--r--   0        0        0     3296 2024-04-29 07:40:13.770239 cg-60.4.6/tests/io/conftest.py
--rw-r--r--   0        0        0      431 2024-04-29 07:40:13.770239 cg-60.4.6/tests/io/test_io_config.py
--rw-r--r--   0        0        0     8639 2024-04-29 07:40:13.770239 cg-60.4.6/tests/io/test_io_controller.py
--rw-r--r--   0        0        0     3877 2024-04-29 07:40:13.770239 cg-60.4.6/tests/io/test_io_csv.py
--rw-r--r--   0        0        0      482 2024-04-29 07:40:13.770239 cg-60.4.6/tests/io/test_io_gzip.py
--rw-r--r--   0        0        0     1779 2024-04-29 07:40:13.770239 cg-60.4.6/tests/io/test_io_json.py
--rw-r--r--   0        0        0     2914 2024-04-29 07:40:13.770239 cg-60.4.6/tests/io/test_io_txt.py
--rw-r--r--   0        0        0     1027 2024-04-29 07:40:13.770239 cg-60.4.6/tests/io/test_io_xml.py
--rw-r--r--   0        0        0     2131 2024-04-29 07:40:13.770239 cg-60.4.6/tests/io/test_io_yaml.py
--rw-r--r--   0        0        0     1233 2024-04-29 07:40:13.770239 cg-60.4.6/tests/io/test_validate_path.py
--rw-r--r--   0        0        0        0 2024-04-29 07:40:13.770239 cg-60.4.6/tests/meta/__init__.py
--rw-r--r--   0        0        0        0 2024-04-29 07:40:13.770239 cg-60.4.6/tests/meta/archive/__init__.py
--rw-r--r--   0        0        0    13131 2024-04-29 07:40:13.770239 cg-60.4.6/tests/meta/archive/conftest.py
--rw-r--r--   0        0        0    16858 2024-04-29 07:40:13.770239 cg-60.4.6/tests/meta/archive/test_archive_api.py
--rw-r--r--   0        0        0    10246 2024-04-29 07:40:13.770239 cg-60.4.6/tests/meta/archive/test_archive_cli.py
--rw-r--r--   0        0        0    15766 2024-04-29 07:40:13.770239 cg-60.4.6/tests/meta/archive/test_archiving.py
--rw-r--r--   0        0        0     3807 2024-04-29 07:40:13.770239 cg-60.4.6/tests/meta/backup/conftest.py
--rw-r--r--   0        0        0    26368 2024-04-29 07:40:13.770239 cg-60.4.6/tests/meta/backup/test_meta_backup.py
--rw-r--r--   0        0        0    10055 2024-04-29 07:40:13.770239 cg-60.4.6/tests/meta/backup/test_meta_pdc.py
--rw-r--r--   0        0        0    12570 2024-04-29 07:40:13.770239 cg-60.4.6/tests/meta/clean/conftest.py
--rw-r--r--   0        0        0    16944 2024-04-29 07:40:13.770239 cg-60.4.6/tests/meta/clean/test_clean_flow_cells_api.py
--rw-r--r--   0        0        0     2286 2024-04-29 07:40:13.770239 cg-60.4.6/tests/meta/clean/test_clean_retrieved_spring_files.py
--rw-r--r--   0        0        0     7691 2024-04-29 07:40:13.770239 cg-60.4.6/tests/meta/compress/conftest.py
--rw-r--r--   0        0        0     7961 2024-04-29 07:40:13.770239 cg-60.4.6/tests/meta/compress/test_clean_fastq.py
--rw-r--r--   0        0        0     1778 2024-04-29 07:40:13.770239 cg-60.4.6/tests/meta/compress/test_compress_files.py
--rw-r--r--   0        0        0     3644 2024-04-29 07:40:13.770239 cg-60.4.6/tests/meta/compress/test_compress_meta_fastq.py
--rw-r--r--   0        0        0     1180 2024-04-29 07:40:13.770239 cg-60.4.6/tests/meta/compress/test_decompress_spring_meta.py
--rw-r--r--   0        0        0     7045 2024-04-29 07:40:13.770239 cg-60.4.6/tests/meta/compress/test_meta_compress_update_hk.py
--rw-r--r--   0        0        0     8269 2024-04-29 07:40:13.770239 cg-60.4.6/tests/meta/conftest.py
--rw-r--r--   0        0        0        0 2024-04-29 07:40:13.770239 cg-60.4.6/tests/meta/deliver/__init__.py
--rw-r--r--   0        0        0     3471 2024-04-29 07:40:13.770239 cg-60.4.6/tests/meta/deliver/conftest.py
--rw-r--r--   0        0        0     5533 2024-04-29 07:40:13.770239 cg-60.4.6/tests/meta/deliver/test_deliver_ticket.py
--rw-r--r--   0        0        0    10277 2024-04-29 07:40:13.770239 cg-60.4.6/tests/meta/deliver/test_delivery_api.py
--rw-r--r--   0        0        0     1057 2024-04-29 07:40:13.770239 cg-60.4.6/tests/meta/deliver/test_fastq_path_generator.py
--rw-r--r--   0        0        0        0 2024-04-29 07:40:13.770239 cg-60.4.6/tests/meta/delivery/__init__.py
--rw-r--r--   0        0        0    16660 2024-04-29 07:40:13.770239 cg-60.4.6/tests/meta/delivery/test_delivery_api.py
--rw-r--r--   0        0        0     8066 2024-04-29 07:40:13.770239 cg-60.4.6/tests/meta/demultiplex/conftest.py
--rw-r--r--   0        0        0     5382 2024-04-29 07:40:13.770239 cg-60.4.6/tests/meta/demultiplex/test_combine_sequencing_metrics.py
--rw-r--r--   0        0        0     8445 2024-04-29 07:40:13.774239 cg-60.4.6/tests/meta/demultiplex/test_demux_post_processing.py
--rw-r--r--   0        0        0    12406 2024-04-29 07:40:13.774239 cg-60.4.6/tests/meta/demultiplex/test_housekeeper_storage_functions.py
--rw-r--r--   0        0        0     4392 2024-04-29 07:40:13.774239 cg-60.4.6/tests/meta/demultiplex/test_status_db_storage_functions.py
--rw-r--r--   0        0        0    22787 2024-04-29 07:40:13.774239 cg-60.4.6/tests/meta/demultiplex/test_utils.py
--rw-r--r--   0        0        0     6258 2024-04-29 07:40:13.774239 cg-60.4.6/tests/meta/demultiplex/test_validation.py
--rw-r--r--   0        0        0     4943 2024-04-29 07:40:13.774239 cg-60.4.6/tests/meta/encryption/conftest.py
--rw-r--r--   0        0        0    18133 2024-04-29 07:40:13.774239 cg-60.4.6/tests/meta/encryption/test_encryption.py
--rw-r--r--   0        0        0     3122 2024-04-29 07:40:13.774239 cg-60.4.6/tests/meta/observations/conftest.py
--rw-r--r--   0        0        0    16164 2024-04-29 07:40:13.774239 cg-60.4.6/tests/meta/observations/test_meta_upload_observations.py
--rw-r--r--   0        0        0     4974 2024-04-29 07:40:13.774239 cg-60.4.6/tests/meta/orders/conftest.py
--rw-r--r--   0        0        0     1749 2024-04-29 07:40:13.774239 cg-60.4.6/tests/meta/orders/test_PoolSubmitter_validate_order.py
--rw-r--r--   0        0        0     1470 2024-04-29 07:40:13.774239 cg-60.4.6/tests/meta/orders/test_SarsCov2Submitter_order_to_status.py
--rw-r--r--   0        0        0     1768 2024-04-29 07:40:13.774239 cg-60.4.6/tests/meta/orders/test_SarsCov2Submitter_store_order.py
--rw-r--r--   0        0        0     2032 2024-04-29 07:40:13.774239 cg-60.4.6/tests/meta/orders/test_SarsCov2Submitter_validate_order.py
--rw-r--r--   0        0        0    19783 2024-04-29 07:40:13.774239 cg-60.4.6/tests/meta/orders/test_meta_orders_api.py
--rw-r--r--   0        0        0     7086 2024-04-29 07:40:13.774239 cg-60.4.6/tests/meta/orders/test_meta_orders_lims.py
--rw-r--r--   0        0        0    29515 2024-04-29 07:40:13.774239 cg-60.4.6/tests/meta/orders/test_meta_orders_status.py
--rw-r--r--   0        0        0     1677 2024-04-29 07:40:13.774239 cg-60.4.6/tests/meta/orders/test_rnafusion_submitter.py
--rw-r--r--   0        0        0     1068 2024-04-29 07:40:13.774239 cg-60.4.6/tests/meta/orders/test_ticket_handler.py
--rw-r--r--   0        0        0     4336 2024-04-29 07:40:13.774239 cg-60.4.6/tests/meta/qc_metrics/conftest.py
--rw-r--r--   0        0        0     1972 2024-04-29 07:40:13.774239 cg-60.4.6/tests/meta/qc_metrics/test_collect_qc_metrics.py
--rw-r--r--   0        0        0        0 2024-04-29 07:40:13.774239 cg-60.4.6/tests/meta/report/__init__.py
--rw-r--r--   0        0        0     6512 2024-04-29 07:40:13.774239 cg-60.4.6/tests/meta/report/conftest.py
--rw-r--r--   0        0        0      434 2024-04-29 07:40:13.774239 cg-60.4.6/tests/meta/report/helper.py
--rw-r--r--   0        0        0     2604 2024-04-29 07:40:13.774239 cg-60.4.6/tests/meta/report/test_balsamic_api.py
--rw-r--r--   0        0        0     4056 2024-04-29 07:40:13.774239 cg-60.4.6/tests/meta/report/test_field_validators.py
--rw-r--r--   0        0        0     2858 2024-04-29 07:40:13.774239 cg-60.4.6/tests/meta/report/test_mip_dna_api.py
--rw-r--r--   0        0        0    16042 2024-04-29 07:40:13.774239 cg-60.4.6/tests/meta/report/test_report_api.py
--rw-r--r--   0        0        0     1365 2024-04-29 07:40:13.774239 cg-60.4.6/tests/meta/report/test_rnafusion_api.py
--rw-r--r--   0        0        0     1250 2024-04-29 07:40:13.774239 cg-60.4.6/tests/meta/report/test_tomte_api.py
--rw-r--r--   0        0        0        0 2024-04-29 07:40:13.774239 cg-60.4.6/tests/meta/rsync/__init__.py
--rw-r--r--   0        0        0      916 2024-04-29 07:40:13.774239 cg-60.4.6/tests/meta/rsync/conftest.py
--rw-r--r--   0        0        0     9442 2024-04-29 07:40:13.774239 cg-60.4.6/tests/meta/rsync/test_rsync.py
--rw-r--r--   0        0        0     3147 2024-04-29 07:40:13.774239 cg-60.4.6/tests/meta/test_invoice.py
--rw-r--r--   0        0        0     1220 2024-04-29 07:40:13.774239 cg-60.4.6/tests/meta/transfer/conftest.py
--rw-r--r--   0        0        0     9892 2024-04-29 07:40:13.774239 cg-60.4.6/tests/meta/transfer/test_external_data.py
--rw-r--r--   0        0        0     4395 2024-04-29 07:40:13.774239 cg-60.4.6/tests/meta/transfer/test_meta_transfer_lims.py
--rw-r--r--   0        0        0        0 2024-04-29 07:40:13.774239 cg-60.4.6/tests/meta/upload/__init__.py
--rw-r--r--   0        0        0     2210 2024-04-29 07:40:13.774239 cg-60.4.6/tests/meta/upload/balsamic/test_balsamic.py
--rw-r--r--   0        0        0     4002 2024-04-29 07:40:13.774239 cg-60.4.6/tests/meta/upload/conftest.py
--rw-r--r--   0        0        0        0 2024-04-29 07:40:13.774239 cg-60.4.6/tests/meta/upload/gisaid/__init__.py
--rw-r--r--   0        0        0     2557 2024-04-29 07:40:13.774239 cg-60.4.6/tests/meta/upload/gisaid/fixtures/four_samples.csv
--rw-r--r--   0        0        0        0 2024-04-29 07:40:13.774239 cg-60.4.6/tests/meta/upload/gisaid/fixtures/invalid_housekeeper.fasta
--rw-r--r--   0        0        0      211 2024-04-29 07:40:13.774239 cg-60.4.6/tests/meta/upload/gisaid/fixtures/valid_gisaid.fasta
--rw-r--r--   0        0        0      371 2024-04-29 07:40:13.774239 cg-60.4.6/tests/meta/upload/gisaid/fixtures/valid_housekeeper.fasta
--rw-r--r--   0        0        0        0 2024-04-29 07:40:13.774239 cg-60.4.6/tests/meta/upload/mutacc/__init__.py
--rw-r--r--   0        0        0     3684 2024-04-29 07:40:13.774239 cg-60.4.6/tests/meta/upload/mutacc/conftest.py
--rw-r--r--   0        0        0     4188 2024-04-29 07:40:13.774239 cg-60.4.6/tests/meta/upload/mutacc/test_meta_upload_mutacc.py
--rw-r--r--   0        0        0     1149 2024-04-29 07:40:13.774239 cg-60.4.6/tests/meta/upload/nipt/conftest.py
--rw-r--r--   0        0        0     1683 2024-04-29 07:40:13.774239 cg-60.4.6/tests/meta/upload/nipt/test_models.py
--rw-r--r--   0        0        0     1242 2024-04-29 07:40:13.774239 cg-60.4.6/tests/meta/upload/nipt/test_nipt_upload_api.py
--rw-r--r--   0        0        0        0 2024-04-29 07:40:13.774239 cg-60.4.6/tests/meta/upload/scout/__init__.py
--rw-r--r--   0        0        0    23954 2024-04-29 07:40:13.774239 cg-60.4.6/tests/meta/upload/scout/conftest.py
--rw-r--r--   0        0        0     4734 2024-04-29 07:40:13.774239 cg-60.4.6/tests/meta/upload/scout/test_generate_load_config.py
--rw-r--r--   0        0        0     4182 2024-04-29 07:40:13.774239 cg-60.4.6/tests/meta/upload/scout/test_meta_upload_scoutapi.py
--rw-r--r--   0        0        0    33260 2024-04-29 07:40:13.774239 cg-60.4.6/tests/meta/upload/scout/test_meta_upload_scoutapi_rna.py
--rw-r--r--   0        0        0     7372 2024-04-29 07:40:13.774239 cg-60.4.6/tests/meta/upload/scout/test_scout_config_builder.py
--rw-r--r--   0        0        0     2511 2024-04-29 07:40:13.774239 cg-60.4.6/tests/meta/upload/test_meta_upload_coverage.py
--rw-r--r--   0        0        0     1473 2024-04-29 07:40:13.774239 cg-60.4.6/tests/meta/upload/test_upload_api.py
--rw-r--r--   0        0        0     2547 2024-04-29 07:40:13.774239 cg-60.4.6/tests/meta/upload/test_upload_genotypes_api.py
--rw-r--r--   0        0        0        0 2024-04-29 07:40:13.774239 cg-60.4.6/tests/meta/workflow/__init__.py
--rw-r--r--   0        0        0    10262 2024-04-29 07:40:13.774239 cg-60.4.6/tests/meta/workflow/conftest.py
--rw-r--r--   0        0        0     3679 2024-04-29 07:40:13.774239 cg-60.4.6/tests/meta/workflow/microsalt/conftest.py
--rw-r--r--   0        0        0      318 2024-04-29 07:40:13.774239 cg-60.4.6/tests/meta/workflow/microsalt/test_parsing_metrics.py
--rw-r--r--   0        0        0     3759 2024-04-29 07:40:13.774239 cg-60.4.6/tests/meta/workflow/microsalt/test_quality_controller.py
--rw-r--r--   0        0        0    14367 2024-04-29 07:40:13.774239 cg-60.4.6/tests/meta/workflow/microsalt/test_quality_controller_utils.py
--rw-r--r--   0        0        0      825 2024-04-29 07:40:13.774239 cg-60.4.6/tests/meta/workflow/microsalt/test_report_generation.py
--rw-r--r--   0        0        0    20860 2024-04-29 07:40:13.774239 cg-60.4.6/tests/meta/workflow/test_analysis.py
--rw-r--r--   0        0        0     7934 2024-04-29 07:40:13.774239 cg-60.4.6/tests/meta/workflow/test_balsamic.py
--rw-r--r--   0        0        0     3034 2024-04-29 07:40:13.774239 cg-60.4.6/tests/meta/workflow/test_fastq.py
--rw-r--r--   0        0        0     1532 2024-04-29 07:40:13.774239 cg-60.4.6/tests/meta/workflow/test_microsalt.py
--rw-r--r--   0        0        0     2721 2024-04-29 07:40:13.774239 cg-60.4.6/tests/meta/workflow/test_nf_analysis.py
--rw-r--r--   0        0        0     7741 2024-04-29 07:40:13.778239 cg-60.4.6/tests/meta/workflow/test_prepare_fastq_api.py
--rw-r--r--   0        0        0     1920 2024-04-29 07:40:13.778239 cg-60.4.6/tests/meta/workflow/test_raredisease.py
--rw-r--r--   0        0        0     1674 2024-04-29 07:40:13.778239 cg-60.4.6/tests/meta/workflow/test_rnafusion.py
--rw-r--r--   0        0        0        0 2024-04-29 07:40:13.778239 cg-60.4.6/tests/mocks/__init__.py
--rw-r--r--   0        0        0     1168 2024-04-29 07:40:13.778239 cg-60.4.6/tests/mocks/balsamic_analysis_mock.py
--rw-r--r--   0        0        0     3500 2024-04-29 07:40:13.778239 cg-60.4.6/tests/mocks/crunchy.py
--rw-r--r--   0        0        0    21778 2024-04-29 07:40:13.778239 cg-60.4.6/tests/mocks/hk_mock.py
--rw-r--r--   0        0        0     4106 2024-04-29 07:40:13.778239 cg-60.4.6/tests/mocks/limsmock.py
--rw-r--r--   0        0        0      572 2024-04-29 07:40:13.778239 cg-60.4.6/tests/mocks/madeline.py
--rw-r--r--   0        0        0     1297 2024-04-29 07:40:13.778239 cg-60.4.6/tests/mocks/mip_analysis_mock.py
--rw-r--r--   0        0        0     1525 2024-04-29 07:40:13.778239 cg-60.4.6/tests/mocks/osticket.py
--rw-r--r--   0        0        0     3239 2024-04-29 07:40:13.778239 cg-60.4.6/tests/mocks/process_mock.py
--rw-r--r--   0        0        0     4713 2024-04-29 07:40:13.778239 cg-60.4.6/tests/mocks/report.py
--rw-r--r--   0        0        0     3915 2024-04-29 07:40:13.778239 cg-60.4.6/tests/mocks/scout.py
--rw-r--r--   0        0        0      750 2024-04-29 07:40:13.778239 cg-60.4.6/tests/mocks/store_model.py
--rw-r--r--   0        0        0     1620 2024-04-29 07:40:13.778239 cg-60.4.6/tests/mocks/tb_mock.py
--rw-r--r--   0        0        0        0 2024-04-29 07:40:13.778239 cg-60.4.6/tests/models/__init__.py
--rw-r--r--   0        0        0        0 2024-04-29 07:40:13.778239 cg-60.4.6/tests/models/balsamic/__init__.py
--rw-r--r--   0        0        0     1194 2024-04-29 07:40:13.778239 cg-60.4.6/tests/models/balsamic/conftest.py
--rw-r--r--   0        0        0     1030 2024-04-29 07:40:13.778239 cg-60.4.6/tests/models/balsamic/test_balsamic_analysis.py
--rw-r--r--   0        0        0     1050 2024-04-29 07:40:13.778239 cg-60.4.6/tests/models/conftest.py
--rw-r--r--   0        0        0        0 2024-04-29 07:40:13.778239 cg-60.4.6/tests/models/demultiplexing/__init__.py
--rw-r--r--   0        0        0    11723 2024-04-29 07:40:13.778239 cg-60.4.6/tests/models/demultiplexing/test_run_parameters.py
--rw-r--r--   0        0        0        0 2024-04-29 07:40:13.778239 cg-60.4.6/tests/models/downsample/__init__.py
--rw-r--r--   0        0        0     2096 2024-04-29 07:40:13.778239 cg-60.4.6/tests/models/downsample/test_down_sample_meta_data.py
--rw-r--r--   0        0        0        0 2024-04-29 07:40:13.778239 cg-60.4.6/tests/models/flow_cell/__init__.py
--rw-r--r--   0        0        0     6723 2024-04-29 07:40:13.778239 cg-60.4.6/tests/models/flow_cell/test_flowcell_model.py
--rw-r--r--   0        0        0     6637 2024-04-29 07:40:13.778239 cg-60.4.6/tests/models/mip/conftest.py
--rw-r--r--   0        0        0     1239 2024-04-29 07:40:13.778239 cg-60.4.6/tests/models/mip/test_mip_analysis.py
--rw-r--r--   0        0        0     2348 2024-04-29 07:40:13.778239 cg-60.4.6/tests/models/mip/test_mip_config.py
--rw-r--r--   0        0        0     6392 2024-04-29 07:40:13.778239 cg-60.4.6/tests/models/mip/test_mip_metrics_deliverables.py
--rw-r--r--   0        0        0     3959 2024-04-29 07:40:13.778239 cg-60.4.6/tests/models/mip/test_mip_sample_info.py
--rw-r--r--   0        0        0     3314 2024-04-29 07:40:13.778239 cg-60.4.6/tests/models/nextflow/test_nextflow_deliver.py
--rw-r--r--   0        0        0     1602 2024-04-29 07:40:13.778239 cg-60.4.6/tests/models/observations/conftest.py
--rw-r--r--   0        0        0     2579 2024-04-29 07:40:13.778239 cg-60.4.6/tests/models/observations/test_observations_input_files.py
--rw-r--r--   0        0        0        0 2024-04-29 07:40:13.778239 cg-60.4.6/tests/models/report/__init__.py
--rw-r--r--   0        0        0     7327 2024-04-29 07:40:13.778239 cg-60.4.6/tests/models/report/test_validators.py
--rw-r--r--   0        0        0     3855 2024-04-29 07:40:13.778239 cg-60.4.6/tests/models/rnafusion/test_rnafusion_sample.py
--rw-r--r--   0        0        0     1374 2024-04-29 07:40:13.778239 cg-60.4.6/tests/models/test_cg_models.py
--rw-r--r--   0        0        0      990 2024-04-29 07:40:13.778239 cg-60.4.6/tests/models/test_compression_data.py
--rw-r--r--   0        0        0      729 2024-04-29 07:40:13.778239 cg-60.4.6/tests/models/test_fastq.py
--rw-r--r--   0        0        0     2860 2024-04-29 07:40:13.778239 cg-60.4.6/tests/models/test_file_data.py
--rw-r--r--   0        0        0     4539 2024-04-29 07:40:13.778239 cg-60.4.6/tests/server/conftest.py
--rw-r--r--   0        0        0     3135 2024-04-29 07:40:13.778239 cg-60.4.6/tests/server/endpoints/test_delivery_message_endpoint.py
--rw-r--r--   0        0        0     3239 2024-04-29 07:40:13.778239 cg-60.4.6/tests/server/endpoints/test_orders_endpoint.py
--rw-r--r--   0        0        0      271 2024-04-29 07:40:13.778239 cg-60.4.6/tests/server/test_server_auto.py
--rw-r--r--   0        0        0     1047 2024-04-29 07:40:13.778239 cg-60.4.6/tests/services/fastq_file_service/conftest.py
--rw-r--r--   0        0        0     3634 2024-04-29 07:40:13.778239 cg-60.4.6/tests/services/fastq_file_service/test_fastq_file_service.py
--rw-r--r--   0        0        0     4861 2024-04-29 07:40:13.778239 cg-60.4.6/tests/services/orders/order_status_service/conftest.py
--rw-r--r--   0        0        0     2865 2024-04-29 07:40:13.778239 cg-60.4.6/tests/services/orders/order_status_service/test_order_summary_service.py
--rw-r--r--   0        0        0     9595 2024-04-29 07:40:13.778239 cg-60.4.6/tests/services/quality_controller/test_sequencing_quality_checks_utils.py
--rw-r--r--   0        0        0      318 2024-04-29 07:40:13.778239 cg-60.4.6/tests/small_helpers.py
--rw-r--r--   0        0        0        0 2024-04-29 07:40:13.778239 cg-60.4.6/tests/store/__init__.py
--rw-r--r--   0        0        0        0 2024-04-29 07:40:13.778239 cg-60.4.6/tests/store/api/__init__.py
--rw-r--r--   0        0        0     3032 2024-04-29 07:40:13.778239 cg-60.4.6/tests/store/api/conftest.py
--rw-r--r--   0        0        0     1557 2024-04-29 07:40:13.778239 cg-60.4.6/tests/store/api/test_base.py
--rw-r--r--   0        0        0    20096 2024-04-29 07:40:13.778239 cg-60.4.6/tests/store/conftest.py
--rw-r--r--   0        0        0        0 2024-04-29 07:40:13.778239 cg-60.4.6/tests/store/crud/__init__.py
--rw-r--r--   0        0        0        0 2024-04-29 07:40:13.778239 cg-60.4.6/tests/store/crud/add/__init__.py
--rw-r--r--   0        0        0     1497 2024-04-29 07:40:13.778239 cg-60.4.6/tests/store/crud/add/test_store_add_application_version.py
--rw-r--r--   0        0        0     3958 2024-04-29 07:40:13.778239 cg-60.4.6/tests/store/crud/add/test_store_add_base.py
--rw-r--r--   0        0        0     2502 2024-04-29 07:40:13.778239 cg-60.4.6/tests/store/crud/add/test_store_add_customer.py
--rw-r--r--   0        0        0     1704 2024-04-29 07:40:13.778239 cg-60.4.6/tests/store/crud/add/test_store_add_flow_celll.py
--rw-r--r--   0        0        0    12290 2024-04-29 07:40:13.778239 cg-60.4.6/tests/store/crud/conftest.py
--rw-r--r--   0        0        0        0 2024-04-29 07:40:13.778239 cg-60.4.6/tests/store/crud/delete/__init__.py
--rw-r--r--   0        0        0     5611 2024-04-29 07:40:13.778239 cg-60.4.6/tests/store/crud/delete/test_delete.py
--rw-r--r--   0        0        0        0 2024-04-29 07:40:13.778239 cg-60.4.6/tests/store/crud/read/__init__.py
--rw-r--r--   0        0        0    56073 2024-04-29 07:40:13.778239 cg-60.4.6/tests/store/crud/read/test_read.py
--rw-r--r--   0        0        0     5461 2024-04-29 07:40:13.778239 cg-60.4.6/tests/store/crud/read/test_read_analyses_to_clean.py
--rw-r--r--   0        0        0     3553 2024-04-29 07:40:13.778239 cg-60.4.6/tests/store/crud/read/test_read_analyses_to_delivery_report.py
--rw-r--r--   0        0        0    17328 2024-04-29 07:40:13.778239 cg-60.4.6/tests/store/crud/read/test_read_analysis.py
--rw-r--r--   0        0        0     2743 2024-04-29 07:40:13.778239 cg-60.4.6/tests/store/crud/read/test_read_application_version.py
--rw-r--r--   0        0        0     1105 2024-04-29 07:40:13.778239 cg-60.4.6/tests/store/crud/read/test_read_customer.py
--rw-r--r--   0        0        0     1530 2024-04-29 07:40:13.778239 cg-60.4.6/tests/store/crud/read/test_read_pool.py
--rw-r--r--   0        0        0    21503 2024-04-29 07:40:13.782239 cg-60.4.6/tests/store/crud/read/test_read_sample.py
--rw-r--r--   0        0        0        0 2024-04-29 07:40:13.782239 cg-60.4.6/tests/store/crud/update/__init__.py
--rw-r--r--   0        0        0      737 2024-04-29 07:40:13.782239 cg-60.4.6/tests/store/crud/update/test_update.py
--rw-r--r--   0        0        0    11693 2024-04-29 07:40:13.782239 cg-60.4.6/tests/store/filters/test_status_analyses_filters.py
--rw-r--r--   0        0        0     3397 2024-04-29 07:40:13.782239 cg-60.4.6/tests/store/filters/test_status_application_filters.py
--rw-r--r--   0        0        0     2073 2024-04-29 07:40:13.782239 cg-60.4.6/tests/store/filters/test_status_application_limitations_filters.py
--rw-r--r--   0        0        0    10452 2024-04-29 07:40:13.782239 cg-60.4.6/tests/store/filters/test_status_application_version_filters.py
--rw-r--r--   0        0        0     2804 2024-04-29 07:40:13.782239 cg-60.4.6/tests/store/filters/test_status_bed_filters.py
--rw-r--r--   0        0        0     2362 2024-04-29 07:40:13.782239 cg-60.4.6/tests/store/filters/test_status_bed_version_filters.py
--rw-r--r--   0        0        0     3495 2024-04-29 07:40:13.782239 cg-60.4.6/tests/store/filters/test_status_case_sample_filters.py
--rw-r--r--   0        0        0    39100 2024-04-29 07:40:13.782239 cg-60.4.6/tests/store/filters/test_status_cases_filters.py
--rw-r--r--   0        0        0     1345 2024-04-29 07:40:13.782239 cg-60.4.6/tests/store/filters/test_status_collaboration_filters.py
--rw-r--r--   0        0        0     2482 2024-04-29 07:40:13.782239 cg-60.4.6/tests/store/filters/test_status_customer_filters.py
--rw-r--r--   0        0        0     5153 2024-04-29 07:40:13.782239 cg-60.4.6/tests/store/filters/test_status_flow_cell_filters.py
--rw-r--r--   0        0        0     2226 2024-04-29 07:40:13.782239 cg-60.4.6/tests/store/filters/test_status_invoice_filters.py
--rw-r--r--   0        0        0     5871 2024-04-29 07:40:13.782239 cg-60.4.6/tests/store/filters/test_status_metrics_filters.py
--rw-r--r--   0        0        0     2404 2024-04-29 07:40:13.782239 cg-60.4.6/tests/store/filters/test_status_organism_filters.py
--rw-r--r--   0        0        0     1804 2024-04-29 07:40:13.782239 cg-60.4.6/tests/store/filters/test_status_panel_filters.py
--rw-r--r--   0        0        0     8720 2024-04-29 07:40:13.782239 cg-60.4.6/tests/store/filters/test_status_pool_filters.py
--rw-r--r--   0        0        0    22875 2024-04-29 07:40:13.782239 cg-60.4.6/tests/store/filters/test_status_samples_filters.py
--rw-r--r--   0        0        0     1576 2024-04-29 07:40:13.782239 cg-60.4.6/tests/store/filters/test_status_user_filters.py
--rw-r--r--   0        0        0     2147 2024-04-29 07:40:13.782239 cg-60.4.6/tests/store/test_delivery.py
--rw-r--r--   0        0        0     4127 2024-04-29 07:40:13.782239 cg-60.4.6/tests/store/test_store_models.py
--rw-r--r--   0        0        0    37125 2024-04-29 07:40:13.782239 cg-60.4.6/tests/store_helpers.py
--rw-r--r--   0        0        0     4988 2024-04-29 07:40:13.782239 cg-60.4.6/tests/test_copy_novaseqx_flow_cell.py
--rw-r--r--   0        0        0      911 2024-04-29 07:40:13.782239 cg-60.4.6/tests/test_store_helpers.py
--rw-r--r--   0        0        0        0 2024-04-29 07:40:13.782239 cg-60.4.6/tests/utils/__init__.py
--rw-r--r--   0        0        0     1754 2024-04-29 07:40:13.782239 cg-60.4.6/tests/utils/conftest.py
--rw-r--r--   0        0        0      371 2024-04-29 07:40:13.782239 cg-60.4.6/tests/utils/test_calculations.py
--rw-r--r--   0        0        0     2920 2024-04-29 07:40:13.782239 cg-60.4.6/tests/utils/test_commands.py
--rw-r--r--   0        0        0      953 2024-04-29 07:40:13.782239 cg-60.4.6/tests/utils/test_date.py
--rw-r--r--   0        0        0     1508 2024-04-29 07:40:13.782239 cg-60.4.6/tests/utils/test_dict.py
--rw-r--r--   0        0        0     7154 2024-04-29 07:40:13.782239 cg-60.4.6/tests/utils/test_dispatcher.py
--rw-r--r--   0        0        0     4100 2024-04-29 07:40:13.782239 cg-60.4.6/tests/utils/test_files.py
--rw-r--r--   0        0        0     1170 2024-04-29 07:40:13.782239 cg-60.4.6/tests/utils/test_time.py
--rw-r--r--   0        0        0     2366 2024-04-29 07:40:13.782239 cg-60.4.6/tests/utils/test_utils.py
--rw-r--r--   0        0        0     4369 1970-01-01 00:00:00.000000 cg-60.4.6/PKG-INFO
+-rw-r--r--   0        0        0     2686 2024-04-29 07:50:37.553871 cg-60.4.7/README.md
+-rw-r--r--   0        0        0       40 2024-04-29 07:50:37.557872 cg-60.4.7/cg/__init__.py
+-rw-r--r--   0        0        0      315 2024-04-29 07:50:37.557872 cg-60.4.7/cg/apps/__init__.py
+-rw-r--r--   0        0        0       27 2024-04-29 07:50:37.557872 cg-60.4.7/cg/apps/coverage/__init__.py
+-rw-r--r--   0        0        0     2940 2024-04-29 07:50:37.557872 cg-60.4.7/cg/apps/coverage/api.py
+-rw-r--r--   0        0        0       56 2024-04-29 07:50:37.557872 cg-60.4.7/cg/apps/crunchy/__init__.py
+-rw-r--r--   0        0        0    12783 2024-04-29 07:50:37.557872 cg-60.4.7/cg/apps/crunchy/crunchy.py
+-rw-r--r--   0        0        0     4502 2024-04-29 07:50:37.557872 cg-60.4.7/cg/apps/crunchy/files.py
+-rw-r--r--   0        0        0      430 2024-04-29 07:50:37.557872 cg-60.4.7/cg/apps/crunchy/models.py
+-rw-r--r--   0        0        0      910 2024-04-29 07:50:37.557872 cg-60.4.7/cg/apps/crunchy/sbatch.py
+-rw-r--r--   0        0        0        0 2024-04-29 07:50:37.557872 cg-60.4.7/cg/apps/demultiplex/__init__.py
+-rw-r--r--   0        0        0    11299 2024-04-29 07:50:37.557872 cg-60.4.7/cg/apps/demultiplex/demultiplex_api.py
+-rw-r--r--   0        0        0        0 2024-04-29 07:50:37.557872 cg-60.4.7/cg/apps/demultiplex/sample_sheet/__init__.py
+-rw-r--r--   0        0        0    11227 2024-04-29 07:50:37.557872 cg-60.4.7/cg/apps/demultiplex/sample_sheet/api.py
+-rw-r--r--   0        0        0     2183 2024-04-29 07:50:37.557872 cg-60.4.7/cg/apps/demultiplex/sample_sheet/index.py
+-rw-r--r--   0        0        0     7341 2024-04-29 07:50:37.557872 cg-60.4.7/cg/apps/demultiplex/sample_sheet/override_cycles_validator.py
+-rw-r--r--   0        0        0     3188 2024-04-29 07:50:37.557872 cg-60.4.7/cg/apps/demultiplex/sample_sheet/read_sample_sheet.py
+-rw-r--r--   0        0        0     7071 2024-04-29 07:50:37.557872 cg-60.4.7/cg/apps/demultiplex/sample_sheet/sample_models.py
+-rw-r--r--   0        0        0     6076 2024-04-29 07:50:37.557872 cg-60.4.7/cg/apps/demultiplex/sample_sheet/sample_sheet_creator.py
+-rw-r--r--   0        0        0     1372 2024-04-29 07:50:37.557872 cg-60.4.7/cg/apps/demultiplex/sample_sheet/sample_sheet_models.py
+-rw-r--r--   0        0        0     8092 2024-04-29 07:50:37.557872 cg-60.4.7/cg/apps/demultiplex/sample_sheet/sample_sheet_validator.py
+-rw-r--r--   0        0        0      824 2024-04-29 07:50:37.557872 cg-60.4.7/cg/apps/demultiplex/sample_sheet/validators.py
+-rw-r--r--   0        0        0      677 2024-04-29 07:50:37.557872 cg-60.4.7/cg/apps/demultiplex/sbatch.py
+-rw-r--r--   0        0        0        0 2024-04-29 07:50:37.557872 cg-60.4.7/cg/apps/downsample/__init__.py
+-rw-r--r--   0        0        0     6160 2024-04-29 07:50:37.557872 cg-60.4.7/cg/apps/downsample/downsample.py
+-rw-r--r--   0        0        0     2125 2024-04-29 07:50:37.557872 cg-60.4.7/cg/apps/downsample/utils.py
+-rw-r--r--   0        0        0      298 2024-04-29 07:50:37.557872 cg-60.4.7/cg/apps/environ.py
+-rw-r--r--   0        0        0     1741 2024-04-29 07:50:37.557872 cg-60.4.7/cg/apps/gens.py
+-rw-r--r--   0        0        0     3419 2024-04-29 07:50:37.557872 cg-60.4.7/cg/apps/gt.py
+-rw-r--r--   0        0        0        0 2024-04-29 07:50:37.557872 cg-60.4.7/cg/apps/hermes/__init__.py
+-rw-r--r--   0        0        0     2249 2024-04-29 07:50:37.557872 cg-60.4.7/cg/apps/hermes/hermes_api.py
+-rw-r--r--   0        0        0     1298 2024-04-29 07:50:37.557872 cg-60.4.7/cg/apps/hermes/models.py
+-rw-r--r--   0        0        0        0 2024-04-29 07:50:37.557872 cg-60.4.7/cg/apps/housekeeper/__init__.py
+-rw-r--r--   0        0        0    30395 2024-04-29 07:50:37.557872 cg-60.4.7/cg/apps/housekeeper/hk.py
+-rw-r--r--   0        0        0      326 2024-04-29 07:50:37.557872 cg-60.4.7/cg/apps/housekeeper/models.py
+-rw-r--r--   0        0        0       32 2024-04-29 07:50:37.557872 cg-60.4.7/cg/apps/invoice/__init__.py
+-rw-r--r--   0        0        0     4804 2024-04-29 07:50:37.561872 cg-60.4.7/cg/apps/invoice/render.py
+-rw-r--r--   0        0        0   113467 2024-04-29 07:50:37.561872 cg-60.4.7/cg/apps/invoice/templates/KI_pool_invoice.xlsx
+-rw-r--r--   0        0        0    75562 2024-04-29 07:50:37.561872 cg-60.4.7/cg/apps/invoice/templates/KI_sample_invoice.xlsx
+-rw-r--r--   0        0        0   113512 2024-04-29 07:50:37.561872 cg-60.4.7/cg/apps/invoice/templates/KTH_pool_invoice.xlsx
+-rw-r--r--   0        0        0    75459 2024-04-29 07:50:37.561872 cg-60.4.7/cg/apps/invoice/templates/KTH_sample_invoice.xlsx
+-rw-r--r--   0        0        0       25 2024-04-29 07:50:37.561872 cg-60.4.7/cg/apps/lims/__init__.py
+-rw-r--r--   0        0        0    18873 2024-04-29 07:50:37.561872 cg-60.4.7/cg/apps/lims/api.py
+-rw-r--r--   0        0        0     2652 2024-04-29 07:50:37.561872 cg-60.4.7/cg/apps/lims/batch.py
+-rw-r--r--   0        0        0     8129 2024-04-29 07:50:37.561872 cg-60.4.7/cg/apps/lims/order.py
+-rw-r--r--   0        0        0     3118 2024-04-29 07:50:37.561872 cg-60.4.7/cg/apps/lims/sample_sheet.py
+-rw-r--r--   0        0        0     4866 2024-04-29 07:50:37.561872 cg-60.4.7/cg/apps/loqus.py
+-rw-r--r--   0        0        0       35 2024-04-29 07:50:37.561872 cg-60.4.7/cg/apps/madeline/__init__.py
+-rw-r--r--   0        0        0     3213 2024-04-29 07:50:37.561872 cg-60.4.7/cg/apps/madeline/api.py
+-rw-r--r--   0        0        0       23 2024-04-29 07:50:37.561872 cg-60.4.7/cg/apps/mip/__init__.py
+-rw-r--r--   0        0        0     3564 2024-04-29 07:50:37.561872 cg-60.4.7/cg/apps/mip/confighandler.py
+-rw-r--r--   0        0        0     2207 2024-04-29 07:50:37.561872 cg-60.4.7/cg/apps/mutacc_auto.py
+-rw-r--r--   0        0        0        0 2024-04-29 07:50:37.561872 cg-60.4.7/cg/apps/orderform/__init__.py
+-rw-r--r--   0        0        0     9498 2024-04-29 07:50:37.561872 cg-60.4.7/cg/apps/orderform/excel_orderform_parser.py
+-rw-r--r--   0        0        0     3051 2024-04-29 07:50:37.561872 cg-60.4.7/cg/apps/orderform/json_orderform_parser.py
+-rw-r--r--   0        0        0     6419 2024-04-29 07:50:37.561872 cg-60.4.7/cg/apps/orderform/orderform_parser.py
+-rw-r--r--   0        0        0      252 2024-04-29 07:50:37.561872 cg-60.4.7/cg/apps/orderform/utils.py
+-rw-r--r--   0        0        0     2537 2024-04-29 07:50:37.561872 cg-60.4.7/cg/apps/osticket.py
+-rw-r--r--   0        0        0        0 2024-04-29 07:50:37.561872 cg-60.4.7/cg/apps/scout/__init__.py
+-rw-r--r--   0        0        0     3177 2024-04-29 07:50:37.561872 cg-60.4.7/cg/apps/scout/scout_export.py
+-rw-r--r--   0        0        0    11108 2024-04-29 07:50:37.561872 cg-60.4.7/cg/apps/scout/scoutapi.py
+-rw-r--r--   0        0        0      444 2024-04-29 07:50:37.561872 cg-60.4.7/cg/apps/scout/validators.py
+-rw-r--r--   0        0        0        0 2024-04-29 07:50:37.561872 cg-60.4.7/cg/apps/sequencing_metrics_parser/__init__.py
+-rw-r--r--   0        0        0     3457 2024-04-29 07:50:37.561872 cg-60.4.7/cg/apps/sequencing_metrics_parser/api.py
+-rw-r--r--   0        0        0      923 2024-04-29 07:50:37.561872 cg-60.4.7/cg/apps/sequencing_metrics_parser/models.py
+-rw-r--r--   0        0        0     6658 2024-04-29 07:50:37.561872 cg-60.4.7/cg/apps/sequencing_metrics_parser/parser.py
+-rw-r--r--   0        0        0        0 2024-04-29 07:50:37.561872 cg-60.4.7/cg/apps/slurm/__init__.py
+-rw-r--r--   0        0        0     1277 2024-04-29 07:50:37.561872 cg-60.4.7/cg/apps/slurm/sbatch.py
+-rw-r--r--   0        0        0     3559 2024-04-29 07:50:37.561872 cg-60.4.7/cg/apps/slurm/slurm_api.py
+-rw-r--r--   0        0        0       32 2024-04-29 07:50:37.561872 cg-60.4.7/cg/apps/tb/__init__.py
+-rw-r--r--   0        0        0     7995 2024-04-29 07:50:37.561872 cg-60.4.7/cg/apps/tb/api.py
+-rw-r--r--   0        0        0      152 2024-04-29 07:50:37.561872 cg-60.4.7/cg/apps/tb/dto/create_job_request.py
+-rw-r--r--   0        0        0      250 2024-04-29 07:50:37.561872 cg-60.4.7/cg/apps/tb/dto/summary_response.py
+-rw-r--r--   0        0        0     1305 2024-04-29 07:50:37.561872 cg-60.4.7/cg/apps/tb/models.py
+-rw-r--r--   0        0        0      305 2024-04-29 07:50:37.561872 cg-60.4.7/cg/apps/tb/validators.py
+-rw-r--r--   0        0        0        0 2024-04-29 07:50:37.561872 cg-60.4.7/cg/cli/__init__.py
+-rw-r--r--   0        0        0    11558 2024-04-29 07:50:37.561872 cg-60.4.7/cg/cli/add.py
+-rw-r--r--   0        0        0     2653 2024-04-29 07:50:37.561872 cg-60.4.7/cg/cli/archive.py
+-rw-r--r--   0        0        0    10118 2024-04-29 07:50:37.561872 cg-60.4.7/cg/cli/backup.py
+-rw-r--r--   0        0        0     3852 2024-04-29 07:50:37.561872 cg-60.4.7/cg/cli/base.py
+-rw-r--r--   0        0        0    10506 2024-04-29 07:50:37.561872 cg-60.4.7/cg/cli/clean.py
+-rw-r--r--   0        0        0        0 2024-04-29 07:50:37.561872 cg-60.4.7/cg/cli/compress/__init__.py
+-rw-r--r--   0        0        0     2135 2024-04-29 07:50:37.561872 cg-60.4.7/cg/cli/compress/base.py
+-rw-r--r--   0        0        0     6706 2024-04-29 07:50:37.561872 cg-60.4.7/cg/cli/compress/fastq.py
+-rw-r--r--   0        0        0     8163 2024-04-29 07:50:37.561872 cg-60.4.7/cg/cli/compress/helpers.py
+-rw-r--r--   0        0        0        0 2024-04-29 07:50:37.561872 cg-60.4.7/cg/cli/delete/__init__.py
+-rw-r--r--   0        0        0      564 2024-04-29 07:50:37.561872 cg-60.4.7/cg/cli/delete/base.py
+-rw-r--r--   0        0        0     4603 2024-04-29 07:50:37.561872 cg-60.4.7/cg/cli/delete/case.py
+-rw-r--r--   0        0        0     1884 2024-04-29 07:50:37.565872 cg-60.4.7/cg/cli/delete/cases.py
+-rw-r--r--   0        0        0     2633 2024-04-29 07:50:37.565872 cg-60.4.7/cg/cli/delete/observations.py
+-rw-r--r--   0        0        0        0 2024-04-29 07:50:37.565872 cg-60.4.7/cg/cli/deliver/__init__.py
+-rw-r--r--   0        0        0     6030 2024-04-29 07:50:37.565872 cg-60.4.7/cg/cli/deliver/base.py
+-rw-r--r--   0        0        0        0 2024-04-29 07:50:37.565872 cg-60.4.7/cg/cli/demultiplex/__init__.py
+-rw-r--r--   0        0        0      829 2024-04-29 07:50:37.565872 cg-60.4.7/cg/cli/demultiplex/base.py
+-rw-r--r--   0        0        0     4905 2024-04-29 07:50:37.565872 cg-60.4.7/cg/cli/demultiplex/copy_novaseqx_demultiplex_data.py
+-rw-r--r--   0        0        0     7726 2024-04-29 07:50:37.565872 cg-60.4.7/cg/cli/demultiplex/demux.py
+-rw-r--r--   0        0        0     1473 2024-04-29 07:50:37.565872 cg-60.4.7/cg/cli/demultiplex/finish.py
+-rw-r--r--   0        0        0     3119 2024-04-29 07:50:37.565872 cg-60.4.7/cg/cli/demultiplex/sample_sheet.py
+-rw-r--r--   0        0        0     2995 2024-04-29 07:50:37.565872 cg-60.4.7/cg/cli/downsample.py
+-rw-r--r--   0        0        0        0 2024-04-29 07:50:37.565872 cg-60.4.7/cg/cli/generate/__init__.py
+-rw-r--r--   0        0        0      356 2024-04-29 07:50:37.565872 cg-60.4.7/cg/cli/generate/base.py
+-rw-r--r--   0        0        0        0 2024-04-29 07:50:37.565872 cg-60.4.7/cg/cli/generate/report/__init__.py
+-rw-r--r--   0        0        0     4636 2024-04-29 07:50:37.565872 cg-60.4.7/cg/cli/generate/report/base.py
+-rw-r--r--   0        0        0      854 2024-04-29 07:50:37.565872 cg-60.4.7/cg/cli/generate/report/options.py
+-rw-r--r--   0        0        0     5615 2024-04-29 07:50:37.565872 cg-60.4.7/cg/cli/generate/report/utils.py
+-rw-r--r--   0        0        0     8327 2024-04-29 07:50:37.565872 cg-60.4.7/cg/cli/get.py
+-rw-r--r--   0        0        0        0 2024-04-29 07:50:37.565872 cg-60.4.7/cg/cli/set/__init__.py
+-rw-r--r--   0        0        0     9856 2024-04-29 07:50:37.565872 cg-60.4.7/cg/cli/set/base.py
+-rw-r--r--   0        0        0     4384 2024-04-29 07:50:37.565872 cg-60.4.7/cg/cli/set/case.py
+-rw-r--r--   0        0        0     2595 2024-04-29 07:50:37.565872 cg-60.4.7/cg/cli/set/cases.py
+-rw-r--r--   0        0        0        0 2024-04-29 07:50:37.565872 cg-60.4.7/cg/cli/store/__init__.py
+-rw-r--r--   0        0        0     1093 2024-04-29 07:50:37.565872 cg-60.4.7/cg/cli/store/base.py
+-rw-r--r--   0        0        0     6191 2024-04-29 07:50:37.565872 cg-60.4.7/cg/cli/store/store.py
+-rw-r--r--   0        0        0     1761 2024-04-29 07:50:37.565872 cg-60.4.7/cg/cli/transfer.py
+-rw-r--r--   0        0        0        1 2024-04-29 07:50:37.565872 cg-60.4.7/cg/cli/upload/__init__.py
+-rw-r--r--   0        0        0     5706 2024-04-29 07:50:37.565872 cg-60.4.7/cg/cli/upload/base.py
+-rw-r--r--   0        0        0     5503 2024-04-29 07:50:37.565872 cg-60.4.7/cg/cli/upload/clinical_delivery.py
+-rw-r--r--   0        0        0     1175 2024-04-29 07:50:37.565872 cg-60.4.7/cg/cli/upload/coverage.py
+-rw-r--r--   0        0        0     1528 2024-04-29 07:50:37.565872 cg-60.4.7/cg/cli/upload/delivery_report.py
+-rw-r--r--   0        0        0     4022 2024-04-29 07:50:37.565872 cg-60.4.7/cg/cli/upload/fohm.py
+-rw-r--r--   0        0        0     1463 2024-04-29 07:50:37.565872 cg-60.4.7/cg/cli/upload/genotype.py
+-rw-r--r--   0        0        0     1885 2024-04-29 07:50:37.565872 cg-60.4.7/cg/cli/upload/gens.py
+-rw-r--r--   0        0        0      584 2024-04-29 07:50:37.565872 cg-60.4.7/cg/cli/upload/gisaid.py
+-rw-r--r--   0        0        0     2645 2024-04-29 07:50:37.565872 cg-60.4.7/cg/cli/upload/mutacc.py
+-rw-r--r--   0        0        0       23 2024-04-29 07:50:37.565872 cg-60.4.7/cg/cli/upload/nipt/__init__.py
+-rw-r--r--   0        0        0     3006 2024-04-29 07:50:37.565872 cg-60.4.7/cg/cli/upload/nipt/base.py
+-rw-r--r--   0        0        0     2275 2024-04-29 07:50:37.565872 cg-60.4.7/cg/cli/upload/nipt/ftp.py
+-rw-r--r--   0        0        0     1596 2024-04-29 07:50:37.565872 cg-60.4.7/cg/cli/upload/nipt/statina.py
+-rw-r--r--   0        0        0      112 2024-04-29 07:50:37.565872 cg-60.4.7/cg/cli/upload/observations/__init__.py
+-rw-r--r--   0        0        0     2672 2024-04-29 07:50:37.565872 cg-60.4.7/cg/cli/upload/observations/observations.py
+-rw-r--r--   0        0        0     2904 2024-04-29 07:50:37.565872 cg-60.4.7/cg/cli/upload/observations/utils.py
+-rw-r--r--   0        0        0     9970 2024-04-29 07:50:37.565872 cg-60.4.7/cg/cli/upload/scout.py
+-rw-r--r--   0        0        0      650 2024-04-29 07:50:37.565872 cg-60.4.7/cg/cli/upload/utils.py
+-rw-r--r--   0        0        0     1667 2024-04-29 07:50:37.565872 cg-60.4.7/cg/cli/upload/validate.py
+-rw-r--r--   0        0        0      105 2024-04-29 07:50:37.565872 cg-60.4.7/cg/cli/utils.py
+-rw-r--r--   0        0        0       18 2024-04-29 07:50:37.565872 cg-60.4.7/cg/cli/workflow/__init__.py
+-rw-r--r--   0        0        0       22 2024-04-29 07:50:37.565872 cg-60.4.7/cg/cli/workflow/balsamic/__init__.py
+-rw-r--r--   0        0        0     8925 2024-04-29 07:50:37.565872 cg-60.4.7/cg/cli/workflow/balsamic/base.py
+-rw-r--r--   0        0        0     1980 2024-04-29 07:50:37.565872 cg-60.4.7/cg/cli/workflow/balsamic/options.py
+-rw-r--r--   0        0        0      881 2024-04-29 07:50:37.565872 cg-60.4.7/cg/cli/workflow/balsamic/pon.py
+-rw-r--r--   0        0        0     1162 2024-04-29 07:50:37.565872 cg-60.4.7/cg/cli/workflow/balsamic/qc.py
+-rw-r--r--   0        0        0     1177 2024-04-29 07:50:37.565872 cg-60.4.7/cg/cli/workflow/balsamic/umi.py
+-rw-r--r--   0        0        0     1342 2024-04-29 07:50:37.565872 cg-60.4.7/cg/cli/workflow/base.py
+-rw-r--r--   0        0        0    12379 2024-04-29 07:50:37.565872 cg-60.4.7/cg/cli/workflow/commands.py
+-rw-r--r--   0        0        0        0 2024-04-29 07:50:37.565872 cg-60.4.7/cg/cli/workflow/fastq/__init__.py
+-rw-r--r--   0        0        0     1490 2024-04-29 07:50:37.565872 cg-60.4.7/cg/cli/workflow/fastq/base.py
+-rw-r--r--   0        0        0     1787 2024-04-29 07:50:37.565872 cg-60.4.7/cg/cli/workflow/fastq/fastq_service.py
+-rw-r--r--   0        0        0        0 2024-04-29 07:50:37.565872 cg-60.4.7/cg/cli/workflow/fluffy/__init__.py
+-rw-r--r--   0        0        0     4177 2024-04-29 07:50:37.565872 cg-60.4.7/cg/cli/workflow/fluffy/base.py
+-rw-r--r--   0        0        0       22 2024-04-29 07:50:37.565872 cg-60.4.7/cg/cli/workflow/jasen/__init__.py
+-rw-r--r--   0        0        0      535 2024-04-29 07:50:37.565872 cg-60.4.7/cg/cli/workflow/jasen/base.py
+-rw-r--r--   0        0        0       22 2024-04-29 07:50:37.565872 cg-60.4.7/cg/cli/workflow/microsalt/__init__.py
+-rw-r--r--   0        0        0     7810 2024-04-29 07:50:37.565872 cg-60.4.7/cg/cli/workflow/microsalt/base.py
+-rw-r--r--   0        0        0       22 2024-04-29 07:50:37.565872 cg-60.4.7/cg/cli/workflow/mip/__init__.py
+-rw-r--r--   0        0        0     6596 2024-04-29 07:50:37.565872 cg-60.4.7/cg/cli/workflow/mip/base.py
+-rw-r--r--   0        0        0     1268 2024-04-29 07:50:37.565872 cg-60.4.7/cg/cli/workflow/mip/options.py
+-rw-r--r--   0        0        0       22 2024-04-29 07:50:37.565872 cg-60.4.7/cg/cli/workflow/mip_dna/__init__.py
+-rw-r--r--   0        0        0     1013 2024-04-29 07:50:37.565872 cg-60.4.7/cg/cli/workflow/mip_dna/base.py
+-rw-r--r--   0        0        0       22 2024-04-29 07:50:37.565872 cg-60.4.7/cg/cli/workflow/mip_rna/__init__.py
+-rw-r--r--   0        0        0      916 2024-04-29 07:50:37.569872 cg-60.4.7/cg/cli/workflow/mip_rna/base.py
+-rw-r--r--   0        0        0        0 2024-04-29 07:50:37.569872 cg-60.4.7/cg/cli/workflow/mutant/__init__.py
+-rw-r--r--   0        0        0     3413 2024-04-29 07:50:37.569872 cg-60.4.7/cg/cli/workflow/mutant/base.py
+-rw-r--r--   0        0        0     9010 2024-04-29 07:50:37.569872 cg-60.4.7/cg/cli/workflow/nf_analysis.py
+-rw-r--r--   0        0        0       22 2024-04-29 07:50:37.569872 cg-60.4.7/cg/cli/workflow/raredisease/__init__.py
+-rw-r--r--   0        0        0     2210 2024-04-29 07:50:37.569872 cg-60.4.7/cg/cli/workflow/raredisease/base.py
+-rw-r--r--   0        0        0       22 2024-04-29 07:50:37.569872 cg-60.4.7/cg/cli/workflow/rnafusion/__init__.py
+-rw-r--r--   0        0        0     1179 2024-04-29 07:50:37.569872 cg-60.4.7/cg/cli/workflow/rnafusion/base.py
+-rw-r--r--   0        0        0       22 2024-04-29 07:50:37.569872 cg-60.4.7/cg/cli/workflow/taxprofiler/__init__.py
+-rw-r--r--   0        0        0     1211 2024-04-29 07:50:37.569872 cg-60.4.7/cg/cli/workflow/taxprofiler/base.py
+-rw-r--r--   0        0        0     1111 2024-04-29 07:50:37.569872 cg-60.4.7/cg/cli/workflow/tomte/base.py
+-rw-r--r--   0        0        0        0 2024-04-29 07:50:37.569872 cg-60.4.7/cg/clients/__init__.py
+-rw-r--r--   0        0        0     1363 2024-04-29 07:50:37.569872 cg-60.4.7/cg/clients/arnold/api.py
+-rw-r--r--   0        0        0      160 2024-04-29 07:50:37.569872 cg-60.4.7/cg/clients/arnold/dto/create_case_request.py
+-rw-r--r--   0        0        0      384 2024-04-29 07:50:37.569872 cg-60.4.7/cg/clients/arnold/exceptions.py
+-rw-r--r--   0        0        0        0 2024-04-29 07:50:37.569872 cg-60.4.7/cg/clients/janus/__init__.py
+-rw-r--r--   0        0        0     1246 2024-04-29 07:50:37.569872 cg-60.4.7/cg/clients/janus/api.py
+-rw-r--r--   0        0        0        0 2024-04-29 07:50:37.569872 cg-60.4.7/cg/clients/janus/dto/__init__.py
+-rw-r--r--   0        0        0      503 2024-04-29 07:50:37.569872 cg-60.4.7/cg/clients/janus/dto/create_qc_metrics_request.py
+-rw-r--r--   0        0        0      420 2024-04-29 07:50:37.569872 cg-60.4.7/cg/clients/janus/exceptions.py
+-rw-r--r--   0        0        0      937 2024-04-29 07:50:37.569872 cg-60.4.7/cg/constants/__init__.py
+-rw-r--r--   0        0        0      253 2024-04-29 07:50:37.569872 cg-60.4.7/cg/constants/archiving.py
+-rw-r--r--   0        0        0       35 2024-04-29 07:50:37.569872 cg-60.4.7/cg/constants/backup.py
+-rw-r--r--   0        0        0      769 2024-04-29 07:50:37.569872 cg-60.4.7/cg/constants/bcl_convert_metrics.py
+-rw-r--r--   0        0        0      469 2024-04-29 07:50:37.569872 cg-60.4.7/cg/constants/compression.py
+-rw-r--r--   0        0        0     6650 2024-04-29 07:50:37.569872 cg-60.4.7/cg/constants/constants.py
+-rw-r--r--   0        0        0     6033 2024-04-29 07:50:37.569872 cg-60.4.7/cg/constants/delivery.py
+-rw-r--r--   0        0        0     7321 2024-04-29 07:50:37.569872 cg-60.4.7/cg/constants/demultiplexing.py
+-rw-r--r--   0        0        0     1422 2024-04-29 07:50:37.569872 cg-60.4.7/cg/constants/encryption.py
+-rw-r--r--   0        0        0      372 2024-04-29 07:50:37.569872 cg-60.4.7/cg/constants/extraction.py
+-rw-r--r--   0        0        0     2157 2024-04-29 07:50:37.569872 cg-60.4.7/cg/constants/gene_panel.py
+-rw-r--r--   0        0        0     6704 2024-04-29 07:50:37.569872 cg-60.4.7/cg/constants/housekeeper_tags.py
+-rw-r--r--   0        0        0       95 2024-04-29 07:50:37.569872 cg-60.4.7/cg/constants/invoice.py
+-rw-r--r--   0        0        0     5815 2024-04-29 07:50:37.569872 cg-60.4.7/cg/constants/lims.py
+-rw-r--r--   0        0        0      743 2024-04-29 07:50:37.569872 cg-60.4.7/cg/constants/metrics.py
+-rw-r--r--   0        0        0      231 2024-04-29 07:50:37.569872 cg-60.4.7/cg/constants/nanopore_files.py
+-rw-r--r--   0        0        0      650 2024-04-29 07:50:37.569872 cg-60.4.7/cg/constants/nextflow.py
+-rw-r--r--   0        0        0     1529 2024-04-29 07:50:37.569872 cg-60.4.7/cg/constants/nf_analysis.py
+-rw-r--r--   0        0        0       19 2024-04-29 07:50:37.569872 cg-60.4.7/cg/constants/nipt.py
+-rw-r--r--   0        0        0     2257 2024-04-29 07:50:37.569872 cg-60.4.7/cg/constants/observations.py
+-rw-r--r--   0        0        0     1216 2024-04-29 07:50:37.569872 cg-60.4.7/cg/constants/orderforms.py
+-rw-r--r--   0        0        0       96 2024-04-29 07:50:37.569872 cg-60.4.7/cg/constants/paths.py
+-rw-r--r--   0        0        0      266 2024-04-29 07:50:37.569872 cg-60.4.7/cg/constants/pdc.py
+-rw-r--r--   0        0        0      160 2024-04-29 07:50:37.569872 cg-60.4.7/cg/constants/pedigree.py
+-rw-r--r--   0        0        0     1044 2024-04-29 07:50:37.569872 cg-60.4.7/cg/constants/priority.py
+-rw-r--r--   0        0        0       79 2024-04-29 07:50:37.569872 cg-60.4.7/cg/constants/process.py
+-rw-r--r--   0        0        0     6019 2024-04-29 07:50:37.569872 cg-60.4.7/cg/constants/report.py
+-rw-r--r--   0        0        0      569 2024-04-29 07:50:37.569872 cg-60.4.7/cg/constants/sample_sources.py
+-rw-r--r--   0        0        0     3111 2024-04-29 07:50:37.569872 cg-60.4.7/cg/constants/scout.py
+-rw-r--r--   0        0        0     1669 2024-04-29 07:50:37.569872 cg-60.4.7/cg/constants/sequencing.py
+-rw-r--r--   0        0        0      313 2024-04-29 07:50:37.569872 cg-60.4.7/cg/constants/slurm.py
+-rw-r--r--   0        0        0      529 2024-04-29 07:50:37.569872 cg-60.4.7/cg/constants/subject.py
+-rw-r--r--   0        0        0       55 2024-04-29 07:50:37.569872 cg-60.4.7/cg/constants/symbols.py
+-rw-r--r--   0        0        0      435 2024-04-29 07:50:37.569872 cg-60.4.7/cg/constants/tb.py
+-rw-r--r--   0        0        0      161 2024-04-29 07:50:37.569872 cg-60.4.7/cg/constants/time.py
+-rw-r--r--   0        0        0     6639 2024-04-29 07:50:37.569872 cg-60.4.7/cg/exc.py
+-rw-r--r--   0        0        0        0 2024-04-29 07:50:37.569872 cg-60.4.7/cg/io/__init__.py
+-rw-r--r--   0        0        0     1037 2024-04-29 07:50:37.569872 cg-60.4.7/cg/io/api.py
+-rw-r--r--   0        0        0      621 2024-04-29 07:50:37.569872 cg-60.4.7/cg/io/config.py
+-rw-r--r--   0        0        0     2978 2024-04-29 07:50:37.569872 cg-60.4.7/cg/io/controller.py
+-rw-r--r--   0        0        0     1763 2024-04-29 07:50:37.569872 cg-60.4.7/cg/io/csv.py
+-rw-r--r--   0        0        0      210 2024-04-29 07:50:37.569872 cg-60.4.7/cg/io/gzip.py
+-rw-r--r--   0        0        0      662 2024-04-29 07:50:37.569872 cg-60.4.7/cg/io/json.py
+-rw-r--r--   0        0        0      525 2024-04-29 07:50:37.569872 cg-60.4.7/cg/io/png.py
+-rw-r--r--   0        0        0     1094 2024-04-29 07:50:37.569872 cg-60.4.7/cg/io/txt.py
+-rw-r--r--   0        0        0      552 2024-04-29 07:50:37.569872 cg-60.4.7/cg/io/validate_path.py
+-rw-r--r--   0        0        0     1289 2024-04-29 07:50:37.569872 cg-60.4.7/cg/io/xml.py
+-rw-r--r--   0        0        0     1153 2024-04-29 07:50:37.569872 cg-60.4.7/cg/io/yaml.py
+-rw-r--r--   0        0        0      281 2024-04-29 07:50:37.569872 cg-60.4.7/cg/meta/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-29 07:50:37.569872 cg-60.4.7/cg/meta/archive/__init__.py
+-rw-r--r--   0        0        0    15193 2024-04-29 07:50:37.569872 cg-60.4.7/cg/meta/archive/archive.py
+-rw-r--r--   0        0        0        0 2024-04-29 07:50:37.569872 cg-60.4.7/cg/meta/archive/ddn/__init__.py
+-rw-r--r--   0        0        0     1727 2024-04-29 07:50:37.569872 cg-60.4.7/cg/meta/archive/ddn/constants.py
+-rw-r--r--   0        0        0    10852 2024-04-29 07:50:37.569872 cg-60.4.7/cg/meta/archive/ddn/ddn_data_flow_client.py
+-rw-r--r--   0        0        0     3704 2024-04-29 07:50:37.569872 cg-60.4.7/cg/meta/archive/ddn/models.py
+-rw-r--r--   0        0        0     1250 2024-04-29 07:50:37.569872 cg-60.4.7/cg/meta/archive/ddn/utils.py
+-rw-r--r--   0        0        0     2024 2024-04-29 07:50:37.569872 cg-60.4.7/cg/meta/archive/models.py
+-rw-r--r--   0        0        0        0 2024-04-29 07:50:37.569872 cg-60.4.7/cg/meta/backup/__init__.py
+-rw-r--r--   0        0        0    17426 2024-04-29 07:50:37.569872 cg-60.4.7/cg/meta/backup/backup.py
+-rw-r--r--   0        0        0     5397 2024-04-29 07:50:37.569872 cg-60.4.7/cg/meta/backup/pdc.py
+-rw-r--r--   0        0        0        0 2024-04-29 07:50:37.569872 cg-60.4.7/cg/meta/clean/__init__.py
+-rw-r--r--   0        0        0     3901 2024-04-29 07:50:37.569872 cg-60.4.7/cg/meta/clean/api.py
+-rw-r--r--   0        0        0     7738 2024-04-29 07:50:37.569872 cg-60.4.7/cg/meta/clean/clean_flow_cells.py
+-rw-r--r--   0        0        0     1841 2024-04-29 07:50:37.569872 cg-60.4.7/cg/meta/clean/clean_retrieved_spring_files.py
+-rw-r--r--   0        0        0       34 2024-04-29 07:50:37.569872 cg-60.4.7/cg/meta/compress/__init__.py
+-rw-r--r--   0        0        0    14557 2024-04-29 07:50:37.569872 cg-60.4.7/cg/meta/compress/compress.py
+-rw-r--r--   0        0        0     4947 2024-04-29 07:50:37.569872 cg-60.4.7/cg/meta/compress/files.py
+-rw-r--r--   0        0        0       77 2024-04-29 07:50:37.569872 cg-60.4.7/cg/meta/deliver/__init__.py
+-rw-r--r--   0        0        0    14905 2024-04-29 07:50:37.569872 cg-60.4.7/cg/meta/deliver/deliver.py
+-rw-r--r--   0        0        0     4502 2024-04-29 07:50:37.573872 cg-60.4.7/cg/meta/deliver/deliver_ticket.py
+-rw-r--r--   0        0        0      904 2024-04-29 07:50:37.573872 cg-60.4.7/cg/meta/deliver/fastq_path_generator.py
+-rw-r--r--   0        0        0        0 2024-04-29 07:50:37.573872 cg-60.4.7/cg/meta/delivery/__init__.py
+-rw-r--r--   0        0        0     8458 2024-04-29 07:50:37.573872 cg-60.4.7/cg/meta/delivery/delivery.py
+-rw-r--r--   0        0        0        0 2024-04-29 07:50:37.573872 cg-60.4.7/cg/meta/demultiplex/__init__.py
+-rw-r--r--   0        0        0     2592 2024-04-29 07:50:37.573872 cg-60.4.7/cg/meta/demultiplex/combine_sequencing_metrics.py
+-rw-r--r--   0        0        0     5719 2024-04-29 07:50:37.573872 cg-60.4.7/cg/meta/demultiplex/demux_post_processing.py
+-rw-r--r--   0        0        0     4135 2024-04-29 07:50:37.573872 cg-60.4.7/cg/meta/demultiplex/files.py
+-rw-r--r--   0        0        0     7777 2024-04-29 07:50:37.573872 cg-60.4.7/cg/meta/demultiplex/housekeeper_storage_functions.py
+-rw-r--r--   0        0        0     6126 2024-04-29 07:50:37.573872 cg-60.4.7/cg/meta/demultiplex/status_db_storage_functions.py
+-rw-r--r--   0        0        0    10690 2024-04-29 07:50:37.573872 cg-60.4.7/cg/meta/demultiplex/utils.py
+-rw-r--r--   0        0        0     2855 2024-04-29 07:50:37.573872 cg-60.4.7/cg/meta/demultiplex/validation.py
+-rw-r--r--   0        0        0        0 2024-04-29 07:50:37.573872 cg-60.4.7/cg/meta/encryption/__init__.py
+-rw-r--r--   0        0        0    20271 2024-04-29 07:50:37.573872 cg-60.4.7/cg/meta/encryption/encryption.py
+-rw-r--r--   0        0        0      537 2024-04-29 07:50:37.573872 cg-60.4.7/cg/meta/encryption/sbatch.py
+-rw-r--r--   0        0        0    10922 2024-04-29 07:50:37.573872 cg-60.4.7/cg/meta/invoice.py
+-rw-r--r--   0        0        0     2360 2024-04-29 07:50:37.573872 cg-60.4.7/cg/meta/meta.py
+-rw-r--r--   0        0        0        0 2024-04-29 07:50:37.573872 cg-60.4.7/cg/meta/observations/__init__.py
+-rw-r--r--   0        0        0     6008 2024-04-29 07:50:37.573872 cg-60.4.7/cg/meta/observations/balsamic_observations_api.py
+-rw-r--r--   0        0        0     5277 2024-04-29 07:50:37.573872 cg-60.4.7/cg/meta/observations/mip_dna_observations_api.py
+-rw-r--r--   0        0        0     5364 2024-04-29 07:50:37.573872 cg-60.4.7/cg/meta/observations/observations_api.py
+-rw-r--r--   0        0        0       27 2024-04-29 07:50:37.573872 cg-60.4.7/cg/meta/orders/__init__.py
+-rw-r--r--   0        0        0     3637 2024-04-29 07:50:37.573872 cg-60.4.7/cg/meta/orders/api.py
+-rw-r--r--   0        0        0      121 2024-04-29 07:50:37.573872 cg-60.4.7/cg/meta/orders/balsamic_qc_submitter.py
+-rw-r--r--   0        0        0      107 2024-04-29 07:50:37.573872 cg-60.4.7/cg/meta/orders/balsamic_submitter.py
+-rw-r--r--   0        0        0      122 2024-04-29 07:50:37.573872 cg-60.4.7/cg/meta/orders/balsamic_umi_submitter.py
+-rw-r--r--   0        0        0    15262 2024-04-29 07:50:37.573872 cg-60.4.7/cg/meta/orders/case_submitter.py
+-rw-r--r--   0        0        0     6102 2024-04-29 07:50:37.573872 cg-60.4.7/cg/meta/orders/fastq_submitter.py
+-rw-r--r--   0        0        0      105 2024-04-29 07:50:37.573872 cg-60.4.7/cg/meta/orders/fluffy_submitter.py
+-rw-r--r--   0        0        0     1254 2024-04-29 07:50:37.573872 cg-60.4.7/cg/meta/orders/lims.py
+-rw-r--r--   0        0        0     5782 2024-04-29 07:50:37.573872 cg-60.4.7/cg/meta/orders/metagenome_submitter.py
+-rw-r--r--   0        0        0     6337 2024-04-29 07:50:37.573872 cg-60.4.7/cg/meta/orders/microbial_submitter.py
+-rw-r--r--   0        0        0      123 2024-04-29 07:50:37.573872 cg-60.4.7/cg/meta/orders/microsalt_submitter.py
+-rw-r--r--   0        0        0      105 2024-04-29 07:50:37.573872 cg-60.4.7/cg/meta/orders/mip_dna_submitter.py
+-rw-r--r--   0        0        0      105 2024-04-29 07:50:37.573872 cg-60.4.7/cg/meta/orders/mip_rna_submitter.py
+-rw-r--r--   0        0        0     7761 2024-04-29 07:50:37.573872 cg-60.4.7/cg/meta/orders/pool_submitter.py
+-rw-r--r--   0        0        0      102 2024-04-29 07:50:37.573872 cg-60.4.7/cg/meta/orders/rml_submitter.py
+-rw-r--r--   0        0        0      718 2024-04-29 07:50:37.573872 cg-60.4.7/cg/meta/orders/rnafusion_submitter.py
+-rw-r--r--   0        0        0     1268 2024-04-29 07:50:37.573872 cg-60.4.7/cg/meta/orders/sars_cov_2_submitter.py
+-rw-r--r--   0        0        0     1754 2024-04-29 07:50:37.573872 cg-60.4.7/cg/meta/orders/submitter.py
+-rw-r--r--   0        0        0     7880 2024-04-29 07:50:37.573872 cg-60.4.7/cg/meta/orders/ticket_handler.py
+-rw-r--r--   0        0        0     4105 2024-04-29 07:50:37.573872 cg-60.4.7/cg/meta/qc_metrics/collect_qc_metrics.py
+-rw-r--r--   0        0        0        0 2024-04-29 07:50:37.573872 cg-60.4.7/cg/meta/report/__init__.py
+-rw-r--r--   0        0        0     8168 2024-04-29 07:50:37.573872 cg-60.4.7/cg/meta/report/balsamic.py
+-rw-r--r--   0        0        0      562 2024-04-29 07:50:37.573872 cg-60.4.7/cg/meta/report/balsamic_qc.py
+-rw-r--r--   0        0        0      717 2024-04-29 07:50:37.573872 cg-60.4.7/cg/meta/report/balsamic_umi.py
+-rw-r--r--   0        0        0     4171 2024-04-29 07:50:37.573872 cg-60.4.7/cg/meta/report/field_validators.py
+-rw-r--r--   0        0        0     6620 2024-04-29 07:50:37.573872 cg-60.4.7/cg/meta/report/mip_dna.py
+-rw-r--r--   0        0        0    18543 2024-04-29 07:50:37.573872 cg-60.4.7/cg/meta/report/report_api.py
+-rw-r--r--   0        0        0     5625 2024-04-29 07:50:37.573872 cg-60.4.7/cg/meta/report/rnafusion.py
+-rw-r--r--   0        0        0     3737 2024-04-29 07:50:37.573872 cg-60.4.7/cg/meta/report/taxprofiler.py
+-rw-r--r--   0        0        0     1911 2024-04-29 07:50:37.573872 cg-60.4.7/cg/meta/report/templates/delivery-report.html
+-rw-r--r--   0        0        0     4756 2024-04-29 07:50:37.573872 cg-60.4.7/cg/meta/report/templates/macros/data_analysis/data_analysis.html
+-rw-r--r--   0        0        0     1049 2024-04-29 07:50:37.573872 cg-60.4.7/cg/meta/report/templates/macros/data_analysis/limitations.html
+-rw-r--r--   0        0        0     3351 2024-04-29 07:50:37.573872 cg-60.4.7/cg/meta/report/templates/macros/data_analysis/qc_metrics/balsamic_qc_metrics.html
+-rw-r--r--   0        0        0     1364 2024-04-29 07:50:37.573872 cg-60.4.7/cg/meta/report/templates/macros/data_analysis/qc_metrics/mip_dna_qc_metrics.html
+-rw-r--r--   0        0        0      753 2024-04-29 07:50:37.573872 cg-60.4.7/cg/meta/report/templates/macros/data_analysis/qc_metrics/qc_metrics.html
+-rw-r--r--   0        0        0     3284 2024-04-29 07:50:37.573872 cg-60.4.7/cg/meta/report/templates/macros/data_analysis/qc_metrics/rnafusion_qc_metrics.html
+-rw-r--r--   0        0        0     2311 2024-04-29 07:50:37.573872 cg-60.4.7/cg/meta/report/templates/macros/data_analysis/qc_metrics/taxprofiler_qc_metrics.html
+-rw-r--r--   0        0        0     3670 2024-04-29 07:50:37.573872 cg-60.4.7/cg/meta/report/templates/macros/data_analysis/qc_metrics/tomte_qc_metrics.html
+-rw-r--r--   0        0        0     2332 2024-04-29 07:50:37.573872 cg-60.4.7/cg/meta/report/templates/macros/header.html
+-rw-r--r--   0        0        0     2178 2024-04-29 07:50:37.573872 cg-60.4.7/cg/meta/report/templates/macros/order.html
+-rw-r--r--   0        0        0     2243 2024-04-29 07:50:37.573872 cg-60.4.7/cg/meta/report/templates/macros/sample_prep.html
+-rw-r--r--   0        0        0      472 2024-04-29 07:50:37.573872 cg-60.4.7/cg/meta/report/templates/macros/ticket_system.html
+-rw-r--r--   0        0        0     1165 2024-04-29 07:50:37.573872 cg-60.4.7/cg/meta/report/templates/macros/uploaded_files/balsamic_uploaded_files.html
+-rw-r--r--   0        0        0     1538 2024-04-29 07:50:37.573872 cg-60.4.7/cg/meta/report/templates/macros/uploaded_files/mip_dna_uploaded_files.html
+-rw-r--r--   0        0        0      428 2024-04-29 07:50:37.573872 cg-60.4.7/cg/meta/report/templates/macros/uploaded_files/rnafusion_uploaded_files.html
+-rw-r--r--   0        0        0     4266 2024-04-29 07:50:37.573872 cg-60.4.7/cg/meta/report/templates/macros/uploaded_files/uploaded_files.html
+-rw-r--r--   0        0        0       80 2024-04-29 07:50:37.573872 cg-60.4.7/cg/meta/report/templates/partials/footer.html
+-rw-r--r--   0        0        0      172 2024-04-29 07:50:37.573872 cg-60.4.7/cg/meta/report/templates/partials/signature.html
+-rw-r--r--   0        0        0   232803 2024-04-29 07:50:37.577872 cg-60.4.7/cg/meta/report/templates/static/css/bootstrap.min.css
+-rw-r--r--   0        0        0       33 2024-04-29 07:50:37.577872 cg-60.4.7/cg/meta/report/templates/static/css/custom.css
+-rw-r--r--   0        0        0    30068 2024-04-29 07:50:37.577872 cg-60.4.7/cg/meta/report/templates/static/images/SWEDAC_logo.png
+-rw-r--r--   0        0        0     3913 2024-04-29 07:50:37.577872 cg-60.4.7/cg/meta/report/tomte.py
+-rw-r--r--   0        0        0       32 2024-04-29 07:50:37.577872 cg-60.4.7/cg/meta/rsync/__init__.py
+-rw-r--r--   0        0        0    12291 2024-04-29 07:50:37.577872 cg-60.4.7/cg/meta/rsync/rsync_api.py
+-rw-r--r--   0        0        0      387 2024-04-29 07:50:37.577872 cg-60.4.7/cg/meta/rsync/sbatch.py
+-rw-r--r--   0        0        0        0 2024-04-29 07:50:37.577872 cg-60.4.7/cg/meta/tar/__init__.py
+-rw-r--r--   0        0        0     1694 2024-04-29 07:50:37.577872 cg-60.4.7/cg/meta/tar/tar.py
+-rw-r--r--   0        0        0       71 2024-04-29 07:50:37.577872 cg-60.4.7/cg/meta/transfer/__init__.py
+-rw-r--r--   0        0        0    10016 2024-04-29 07:50:37.577872 cg-60.4.7/cg/meta/transfer/external_data.py
+-rw-r--r--   0        0        0     5814 2024-04-29 07:50:37.577872 cg-60.4.7/cg/meta/transfer/lims.py
+-rw-r--r--   0        0        0        0 2024-04-29 07:50:37.577872 cg-60.4.7/cg/meta/upload/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-29 07:50:37.577872 cg-60.4.7/cg/meta/upload/balsamic/__init__.py
+-rw-r--r--   0        0        0     3107 2024-04-29 07:50:37.577872 cg-60.4.7/cg/meta/upload/balsamic/balsamic.py
+-rw-r--r--   0        0        0     2224 2024-04-29 07:50:37.577872 cg-60.4.7/cg/meta/upload/coverage.py
+-rw-r--r--   0        0        0        0 2024-04-29 07:50:37.577872 cg-60.4.7/cg/meta/upload/fohm/__init__.py
+-rw-r--r--   0        0        0    12102 2024-04-29 07:50:37.577872 cg-60.4.7/cg/meta/upload/fohm/fohm.py
+-rw-r--r--   0        0        0       30 2024-04-29 07:50:37.577872 cg-60.4.7/cg/meta/upload/gisaid/__init__.py
+-rw-r--r--   0        0        0      928 2024-04-29 07:50:37.577872 cg-60.4.7/cg/meta/upload/gisaid/constants.py
+-rw-r--r--   0        0        0    13521 2024-04-29 07:50:37.577872 cg-60.4.7/cg/meta/upload/gisaid/gisaid.py
+-rw-r--r--   0        0        0     3312 2024-04-29 07:50:37.577872 cg-60.4.7/cg/meta/upload/gisaid/models.py
+-rw-r--r--   0        0        0     5310 2024-04-29 07:50:37.577872 cg-60.4.7/cg/meta/upload/gt.py
+-rw-r--r--   0        0        0      898 2024-04-29 07:50:37.577872 cg-60.4.7/cg/meta/upload/microsalt/microsalt_upload_api.py
+-rw-r--r--   0        0        0        0 2024-04-29 07:50:37.577872 cg-60.4.7/cg/meta/upload/mip/__init__.py
+-rw-r--r--   0        0        0     2546 2024-04-29 07:50:37.577872 cg-60.4.7/cg/meta/upload/mip/mip_dna.py
+-rw-r--r--   0        0        0     1400 2024-04-29 07:50:37.577872 cg-60.4.7/cg/meta/upload/mip/mip_rna.py
+-rw-r--r--   0        0        0     7294 2024-04-29 07:50:37.577872 cg-60.4.7/cg/meta/upload/mutacc.py
+-rw-r--r--   0        0        0     1853 2024-04-29 07:50:37.577872 cg-60.4.7/cg/meta/upload/nf_analysis.py
+-rw-r--r--   0        0        0       32 2024-04-29 07:50:37.577872 cg-60.4.7/cg/meta/upload/nipt/__init__.py
+-rw-r--r--   0        0        0      696 2024-04-29 07:50:37.577872 cg-60.4.7/cg/meta/upload/nipt/models.py
+-rw-r--r--   0        0        0     8106 2024-04-29 07:50:37.577872 cg-60.4.7/cg/meta/upload/nipt/nipt.py
+-rw-r--r--   0        0        0        0 2024-04-29 07:50:37.577872 cg-60.4.7/cg/meta/upload/scout/__init__.py
+-rw-r--r--   0        0        0     4009 2024-04-29 07:50:37.577872 cg-60.4.7/cg/meta/upload/scout/balsamic_config_builder.py
+-rw-r--r--   0        0        0     1491 2024-04-29 07:50:37.577872 cg-60.4.7/cg/meta/upload/scout/balsamic_umi_config_builder.py
+-rw-r--r--   0        0        0     3322 2024-04-29 07:50:37.577872 cg-60.4.7/cg/meta/upload/scout/hk_tags.py
+-rw-r--r--   0        0        0     9103 2024-04-29 07:50:37.577872 cg-60.4.7/cg/meta/upload/scout/mip_config_builder.py
+-rw-r--r--   0        0        0     3495 2024-04-29 07:50:37.577872 cg-60.4.7/cg/meta/upload/scout/rnafusion_config_builder.py
+-rw-r--r--   0        0        0     7231 2024-04-29 07:50:37.577872 cg-60.4.7/cg/meta/upload/scout/scout_config_builder.py
+-rw-r--r--   0        0        0    23146 2024-04-29 07:50:37.577872 cg-60.4.7/cg/meta/upload/scout/uploadscoutapi.py
+-rw-r--r--   0        0        0     3197 2024-04-29 07:50:37.577872 cg-60.4.7/cg/meta/upload/upload_api.py
+-rw-r--r--   0        0        0        0 2024-04-29 07:50:37.577872 cg-60.4.7/cg/meta/workflow/__init__.py
+-rw-r--r--   0        0        0    31068 2024-04-29 07:50:37.577872 cg-60.4.7/cg/meta/workflow/analysis.py
+-rw-r--r--   0        0        0    27751 2024-04-29 07:50:37.577872 cg-60.4.7/cg/meta/workflow/balsamic.py
+-rw-r--r--   0        0        0     2700 2024-04-29 07:50:37.577872 cg-60.4.7/cg/meta/workflow/balsamic_pon.py
+-rw-r--r--   0        0        0      553 2024-04-29 07:50:37.577872 cg-60.4.7/cg/meta/workflow/balsamic_qc.py
+-rw-r--r--   0        0        0      556 2024-04-29 07:50:37.577872 cg-60.4.7/cg/meta/workflow/balsamic_umi.py
+-rw-r--r--   0        0        0        0 2024-04-29 07:50:37.577872 cg-60.4.7/cg/meta/workflow/downsample/__init__.py
+-rw-r--r--   0        0        0     3922 2024-04-29 07:50:37.577872 cg-60.4.7/cg/meta/workflow/downsample/downsample.py
+-rw-r--r--   0        0        0      711 2024-04-29 07:50:37.577872 cg-60.4.7/cg/meta/workflow/downsample/sbatch.py
+-rw-r--r--   0        0        0     8913 2024-04-29 07:50:37.577872 cg-60.4.7/cg/meta/workflow/fastq.py
+-rw-r--r--   0        0        0    10603 2024-04-29 07:50:37.577872 cg-60.4.7/cg/meta/workflow/fluffy.py
+-rw-r--r--   0        0        0      521 2024-04-29 07:50:37.577872 cg-60.4.7/cg/meta/workflow/jasen.py
+-rw-r--r--   0        0        0       70 2024-04-29 07:50:37.577872 cg-60.4.7/cg/meta/workflow/microsalt/__init__.py
+-rw-r--r--   0        0        0      116 2024-04-29 07:50:37.577872 cg-60.4.7/cg/meta/workflow/microsalt/constants.py
+-rw-r--r--   0        0        0      174 2024-04-29 07:50:37.577872 cg-60.4.7/cg/meta/workflow/microsalt/metrics_parser/__init__.py
+-rw-r--r--   0        0        0      366 2024-04-29 07:50:37.577872 cg-60.4.7/cg/meta/workflow/microsalt/metrics_parser/metrics_parser.py
+-rw-r--r--   0        0        0      903 2024-04-29 07:50:37.577872 cg-60.4.7/cg/meta/workflow/microsalt/metrics_parser/models.py
+-rw-r--r--   0        0        0    13173 2024-04-29 07:50:37.577872 cg-60.4.7/cg/meta/workflow/microsalt/microsalt.py
+-rw-r--r--   0        0        0      113 2024-04-29 07:50:37.577872 cg-60.4.7/cg/meta/workflow/microsalt/quality_controller/__init__.py
+-rw-r--r--   0        0        0      712 2024-04-29 07:50:37.577872 cg-60.4.7/cg/meta/workflow/microsalt/quality_controller/models.py
+-rw-r--r--   0        0        0     5697 2024-04-29 07:50:37.577872 cg-60.4.7/cg/meta/workflow/microsalt/quality_controller/quality_controller.py
+-rw-r--r--   0        0        0     1217 2024-04-29 07:50:37.577872 cg-60.4.7/cg/meta/workflow/microsalt/quality_controller/report_generator.py
+-rw-r--r--   0        0        0     2373 2024-04-29 07:50:37.577872 cg-60.4.7/cg/meta/workflow/microsalt/quality_controller/result_logger.py
+-rw-r--r--   0        0        0     5641 2024-04-29 07:50:37.577872 cg-60.4.7/cg/meta/workflow/microsalt/quality_controller/utils.py
+-rw-r--r--   0        0        0     1220 2024-04-29 07:50:37.577872 cg-60.4.7/cg/meta/workflow/microsalt/utils.py
+-rw-r--r--   0        0        0    12611 2024-04-29 07:50:37.581872 cg-60.4.7/cg/meta/workflow/mip.py
+-rw-r--r--   0        0        0     2948 2024-04-29 07:50:37.581872 cg-60.4.7/cg/meta/workflow/mip_dna.py
+-rw-r--r--   0        0        0     2124 2024-04-29 07:50:37.581872 cg-60.4.7/cg/meta/workflow/mip_rna.py
+-rw-r--r--   0        0        0    10974 2024-04-29 07:50:37.581872 cg-60.4.7/cg/meta/workflow/mutant.py
+-rw-r--r--   0        0        0    37934 2024-04-29 07:50:37.581872 cg-60.4.7/cg/meta/workflow/nf_analysis.py
+-rw-r--r--   0        0        0     6161 2024-04-29 07:50:37.581872 cg-60.4.7/cg/meta/workflow/nf_handlers.py
+-rw-r--r--   0        0        0     6357 2024-04-29 07:50:37.581872 cg-60.4.7/cg/meta/workflow/prepare_fastq.py
+-rw-r--r--   0        0        0     4785 2024-04-29 07:50:37.581872 cg-60.4.7/cg/meta/workflow/raredisease.py
+-rw-r--r--   0        0        0     5403 2024-04-29 07:50:37.581872 cg-60.4.7/cg/meta/workflow/rnafusion.py
+-rw-r--r--   0        0        0     4658 2024-04-29 07:50:37.581872 cg-60.4.7/cg/meta/workflow/taxprofiler.py
+-rw-r--r--   0        0        0     3576 2024-04-29 07:50:37.581872 cg-60.4.7/cg/meta/workflow/tomte.py
+-rw-r--r--   0        0        0      113 2024-04-29 07:50:37.581872 cg-60.4.7/cg/models/__init__.py
+-rw-r--r--   0        0        0      457 2024-04-29 07:50:37.581872 cg-60.4.7/cg/models/analysis.py
+-rw-r--r--   0        0        0        0 2024-04-29 07:50:37.581872 cg-60.4.7/cg/models/balsamic/__init__.py
+-rw-r--r--   0        0        0      459 2024-04-29 07:50:37.581872 cg-60.4.7/cg/models/balsamic/analysis.py
+-rw-r--r--   0        0        0     4550 2024-04-29 07:50:37.581872 cg-60.4.7/cg/models/balsamic/config.py
+-rw-r--r--   0        0        0     1986 2024-04-29 07:50:37.581872 cg-60.4.7/cg/models/balsamic/metrics.py
+-rw-r--r--   0        0        0    17539 2024-04-29 07:50:37.581872 cg-60.4.7/cg/models/cg_config.py
+-rw-r--r--   0        0        0     4302 2024-04-29 07:50:37.581872 cg-60.4.7/cg/models/compression_data.py
+-rw-r--r--   0        0        0        0 2024-04-29 07:50:37.581872 cg-60.4.7/cg/models/deliverables/__init__.py
+-rw-r--r--   0        0        0     5213 2024-04-29 07:50:37.581872 cg-60.4.7/cg/models/deliverables/metric_deliverables.py
+-rw-r--r--   0        0        0      243 2024-04-29 07:50:37.581872 cg-60.4.7/cg/models/delivery/delivery.py
+-rw-r--r--   0        0        0        0 2024-04-29 07:50:37.581872 cg-60.4.7/cg/models/demultiplex/__init__.py
+-rw-r--r--   0        0        0    12040 2024-04-29 07:50:37.581872 cg-60.4.7/cg/models/demultiplex/run_parameters.py
+-rw-r--r--   0        0        0      539 2024-04-29 07:50:37.581872 cg-60.4.7/cg/models/demultiplex/sbatch.py
+-rw-r--r--   0        0        0     7006 2024-04-29 07:50:37.581872 cg-60.4.7/cg/models/downsample/downsample_data.py
+-rw-r--r--   0        0        0      255 2024-04-29 07:50:37.581872 cg-60.4.7/cg/models/email.py
+-rw-r--r--   0        0        0     1046 2024-04-29 07:50:37.581872 cg-60.4.7/cg/models/fastq.py
+-rw-r--r--   0        0        0     2157 2024-04-29 07:50:37.581872 cg-60.4.7/cg/models/file_data.py
+-rw-r--r--   0        0        0        0 2024-04-29 07:50:37.581872 cg-60.4.7/cg/models/flow_cell/__init__.py
+-rw-r--r--   0        0        0     9984 2024-04-29 07:50:37.581872 cg-60.4.7/cg/models/flow_cell/flow_cell.py
+-rw-r--r--   0        0        0      317 2024-04-29 07:50:37.581872 cg-60.4.7/cg/models/flow_cell/utils.py
+-rw-r--r--   0        0        0        0 2024-04-29 07:50:37.581872 cg-60.4.7/cg/models/invoice/__init__.py
+-rw-r--r--   0        0        0     1254 2024-04-29 07:50:37.581872 cg-60.4.7/cg/models/invoice/invoice.py
+-rw-r--r--   0        0        0        0 2024-04-29 07:50:37.581872 cg-60.4.7/cg/models/lims/__init__.py
+-rw-r--r--   0        0        0     2019 2024-04-29 07:50:37.581872 cg-60.4.7/cg/models/lims/sample.py
+-rw-r--r--   0        0        0        0 2024-04-29 07:50:37.581872 cg-60.4.7/cg/models/mip/__init__.py
+-rw-r--r--   0        0        0      337 2024-04-29 07:50:37.581872 cg-60.4.7/cg/models/mip/mip_analysis.py
+-rw-r--r--   0        0        0     1564 2024-04-29 07:50:37.581872 cg-60.4.7/cg/models/mip/mip_config.py
+-rw-r--r--   0        0        0     4696 2024-04-29 07:50:37.581872 cg-60.4.7/cg/models/mip/mip_metrics_deliverables.py
+-rw-r--r--   0        0        0     2550 2024-04-29 07:50:37.581872 cg-60.4.7/cg/models/mip/mip_sample_info.py
+-rw-r--r--   0        0        0     2472 2024-04-29 07:50:37.581872 cg-60.4.7/cg/models/nf_analysis.py
+-rw-r--r--   0        0        0        0 2024-04-29 07:50:37.581872 cg-60.4.7/cg/models/observations/__init__.py
+-rw-r--r--   0        0        0      688 2024-04-29 07:50:37.581872 cg-60.4.7/cg/models/observations/input_files.py
+-rw-r--r--   0        0        0        0 2024-04-29 07:50:37.581872 cg-60.4.7/cg/models/orders/__init__.py
+-rw-r--r--   0        0        0     2659 2024-04-29 07:50:37.581872 cg-60.4.7/cg/models/orders/constants.py
+-rw-r--r--   0        0        0     5604 2024-04-29 07:50:37.581872 cg-60.4.7/cg/models/orders/excel_sample.py
+-rw-r--r--   0        0        0      898 2024-04-29 07:50:37.581872 cg-60.4.7/cg/models/orders/json_sample.py
+-rw-r--r--   0        0        0     1449 2024-04-29 07:50:37.581872 cg-60.4.7/cg/models/orders/order.py
+-rw-r--r--   0        0        0      811 2024-04-29 07:50:37.581872 cg-60.4.7/cg/models/orders/orderform_schema.py
+-rw-r--r--   0        0        0     4212 2024-04-29 07:50:37.581872 cg-60.4.7/cg/models/orders/sample_base.py
+-rw-r--r--   0        0        0     9668 2024-04-29 07:50:37.581872 cg-60.4.7/cg/models/orders/samples.py
+-rw-r--r--   0        0        0        0 2024-04-29 07:50:37.581872 cg-60.4.7/cg/models/orders/validators/__init__.py
+-rw-r--r--   0        0        0     2300 2024-04-29 07:50:37.581872 cg-60.4.7/cg/models/orders/validators/excel_sample_validators.py
+-rw-r--r--   0        0        0      576 2024-04-29 07:50:37.581872 cg-60.4.7/cg/models/orders/validators/json_sample_validators.py
+-rw-r--r--   0        0        0       71 2024-04-29 07:50:37.581872 cg-60.4.7/cg/models/orders/validators/sample_base_validators.py
+-rw-r--r--   0        0        0      101 2024-04-29 07:50:37.581872 cg-60.4.7/cg/models/qc_metrics.py
+-rw-r--r--   0        0        0        0 2024-04-29 07:50:37.581872 cg-60.4.7/cg/models/raredisease/__init__.py
+-rw-r--r--   0        0        0     1875 2024-04-29 07:50:37.581872 cg-60.4.7/cg/models/raredisease/raredisease.py
+-rw-r--r--   0        0        0        0 2024-04-29 07:50:37.581872 cg-60.4.7/cg/models/report/__init__.py
+-rw-r--r--   0        0        0     8507 2024-04-29 07:50:37.581872 cg-60.4.7/cg/models/report/metadata.py
+-rw-r--r--   0        0        0     6180 2024-04-29 07:50:37.581872 cg-60.4.7/cg/models/report/report.py
+-rw-r--r--   0        0        0     5298 2024-04-29 07:50:37.581872 cg-60.4.7/cg/models/report/sample.py
+-rw-r--r--   0        0        0     3004 2024-04-29 07:50:37.581872 cg-60.4.7/cg/models/report/validators.py
+-rw-r--r--   0        0        0        0 2024-04-29 07:50:37.581872 cg-60.4.7/cg/models/rnafusion/__init__.py
+-rw-r--r--   0        0        0     1865 2024-04-29 07:50:37.581872 cg-60.4.7/cg/models/rnafusion/rnafusion.py
+-rw-r--r--   0        0        0        0 2024-04-29 07:50:37.581872 cg-60.4.7/cg/models/scout/__init__.py
+-rw-r--r--   0        0        0     4783 2024-04-29 07:50:37.581872 cg-60.4.7/cg/models/scout/scout_load_config.py
+-rw-r--r--   0        0        0      116 2024-04-29 07:50:37.581872 cg-60.4.7/cg/models/scout/validators.py
+-rw-r--r--   0        0        0        0 2024-04-29 07:50:37.581872 cg-60.4.7/cg/models/slurm/__init__.py
+-rw-r--r--   0        0        0      617 2024-04-29 07:50:37.581872 cg-60.4.7/cg/models/slurm/sbatch.py
+-rw-r--r--   0        0        0        0 2024-04-29 07:50:37.581872 cg-60.4.7/cg/models/taxprofiler/__init__.py
+-rw-r--r--   0        0        0     2556 2024-04-29 07:50:37.581872 cg-60.4.7/cg/models/taxprofiler/taxprofiler.py
+-rw-r--r--   0        0        0     2588 2024-04-29 07:50:37.581872 cg-60.4.7/cg/models/tomte/tomte.py
+-rw-r--r--   0        0        0        0 2024-04-29 07:50:37.581872 cg-60.4.7/cg/models/workflow/__init__.py
+-rw-r--r--   0        0        0      685 2024-04-29 07:50:37.581872 cg-60.4.7/cg/models/workflow/mutant.py
+-rw-r--r--   0        0        0       70 2024-04-29 07:50:37.581872 cg-60.4.7/cg/models/workflow/validators.py
+-rw-r--r--   0        0        0      842 2024-04-29 07:50:37.581872 cg-60.4.7/cg/resources/__init__.py
+-rw-r--r--   0        0        0     3493 2024-04-29 07:50:37.581872 cg-60.4.7/cg/resources/rnafusion_bundle_filenames.yaml
+-rw-r--r--   0        0        0     2434 2024-04-29 07:50:37.581872 cg-60.4.7/cg/resources/taxprofiler_bundle_filenames.yaml
+-rw-r--r--   0        0        0     3732 2024-04-29 07:50:37.581872 cg-60.4.7/cg/resources/tomte_bundle_filenames.yaml
+-rw-r--r--   0        0        0        0 2024-04-29 07:50:37.581872 cg-60.4.7/cg/server/__init__.py
+-rw-r--r--   0        0        0    20299 2024-04-29 07:50:37.585872 cg-60.4.7/cg/server/admin.py
+-rw-r--r--   0        0        0    22743 2024-04-29 07:50:37.585872 cg-60.4.7/cg/server/api.py
+-rw-r--r--   0        0        0     4887 2024-04-29 07:50:37.585872 cg-60.4.7/cg/server/app.py
+-rw-r--r--   0        0        0       48 2024-04-29 07:50:37.585872 cg-60.4.7/cg/server/auto.py
+-rw-r--r--   0        0        0     1184 2024-04-29 07:50:37.585872 cg-60.4.7/cg/server/config.py
+-rw-r--r--   0        0        0        0 2024-04-29 07:50:37.585872 cg-60.4.7/cg/server/dto/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-29 07:50:37.585872 cg-60.4.7/cg/server/dto/delivery_message/__init__.py
+-rw-r--r--   0        0        0      300 2024-04-29 07:50:37.585872 cg-60.4.7/cg/server/dto/delivery_message/delivery_message_request.py
+-rw-r--r--   0        0        0      183 2024-04-29 07:50:37.585872 cg-60.4.7/cg/server/dto/delivery_message/delivery_message_response.py
+-rw-r--r--   0        0        0        0 2024-04-29 07:50:37.585872 cg-60.4.7/cg/server/dto/orders/__init__.py
+-rw-r--r--   0        0        0      165 2024-04-29 07:50:37.585872 cg-60.4.7/cg/server/dto/orders/order_delivery_update_request.py
+-rw-r--r--   0        0        0       91 2024-04-29 07:50:37.585872 cg-60.4.7/cg/server/dto/orders/order_patch_request.py
+-rw-r--r--   0        0        0      662 2024-04-29 07:50:37.585872 cg-60.4.7/cg/server/dto/orders/orders_request.py
+-rw-r--r--   0        0        0      413 2024-04-29 07:50:37.585872 cg-60.4.7/cg/server/dto/orders/orders_response.py
+-rw-r--r--   0        0        0     2598 2024-04-29 07:50:37.585872 cg-60.4.7/cg/server/ext.py
+-rw-r--r--   0        0        0       29 2024-04-29 07:50:37.585872 cg-60.4.7/cg/server/invoices/__init__.py
+-rw-r--r--   0        0        0     4793 2024-04-29 07:50:37.585872 cg-60.4.7/cg/server/invoices/templates/invoices/index.html
+-rw-r--r--   0        0        0     8171 2024-04-29 07:50:37.585872 cg-60.4.7/cg/server/invoices/templates/invoices/invoice.html
+-rw-r--r--   0        0        0     2838 2024-04-29 07:50:37.585872 cg-60.4.7/cg/server/invoices/templates/invoices/layout.html
+-rw-r--r--   0        0        0     4956 2024-04-29 07:50:37.585872 cg-60.4.7/cg/server/invoices/templates/invoices/new.html
+-rw-r--r--   0        0        0     7708 2024-04-29 07:50:37.585872 cg-60.4.7/cg/server/invoices/views.py
+-rw-r--r--   0        0        0      354 2024-04-29 07:50:37.585872 cg-60.4.7/cg/server/templates/admin/index.html
+-rw-r--r--   0        0        0        0 2024-04-29 07:50:37.585872 cg-60.4.7/cg/services/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-29 07:50:37.585872 cg-60.4.7/cg/services/analysis_service/__init__.py
+-rw-r--r--   0        0        0      482 2024-04-29 07:50:37.585872 cg-60.4.7/cg/services/analysis_service/analysis_service.py
+-rw-r--r--   0        0        0        0 2024-04-29 07:50:37.585872 cg-60.4.7/cg/services/delivery_message/__init__.py
+-rw-r--r--   0        0        0     2531 2024-04-29 07:50:37.585872 cg-60.4.7/cg/services/delivery_message/delivery_message_service.py
+-rw-r--r--   0        0        0      792 2024-04-29 07:50:37.585872 cg-60.4.7/cg/services/delivery_message/messages/__init__.py
+-rw-r--r--   0        0        0     1366 2024-04-29 07:50:37.585872 cg-60.4.7/cg/services/delivery_message/messages/analysis_scout_message.py
+-rw-r--r--   0        0        0      791 2024-04-29 07:50:37.585872 cg-60.4.7/cg/services/delivery_message/messages/covid_message.py
+-rw-r--r--   0        0        0      189 2024-04-29 07:50:37.585872 cg-60.4.7/cg/services/delivery_message/messages/delivery_message.py
+-rw-r--r--   0        0        0     1391 2024-04-29 07:50:37.585872 cg-60.4.7/cg/services/delivery_message/messages/fastq_analysis_scout_message.py
+-rw-r--r--   0        0        0      535 2024-04-29 07:50:37.585872 cg-60.4.7/cg/services/delivery_message/messages/fastq_message.py
+-rw-r--r--   0        0        0     1358 2024-04-29 07:50:37.585872 cg-60.4.7/cg/services/delivery_message/messages/fastq_scout_message.py
+-rw-r--r--   0        0        0      604 2024-04-29 07:50:37.585872 cg-60.4.7/cg/services/delivery_message/messages/microsalt_mwr_message.py
+-rw-r--r--   0        0        0      592 2024-04-29 07:50:37.585872 cg-60.4.7/cg/services/delivery_message/messages/microsalt_mwx_message.py
+-rw-r--r--   0        0        0      903 2024-04-29 07:50:37.585872 cg-60.4.7/cg/services/delivery_message/messages/scout_message.py
+-rw-r--r--   0        0        0      512 2024-04-29 07:50:37.585872 cg-60.4.7/cg/services/delivery_message/messages/statina_message.py
+-rw-r--r--   0        0        0      779 2024-04-29 07:50:37.585872 cg-60.4.7/cg/services/delivery_message/messages/utils.py
+-rw-r--r--   0        0        0     3300 2024-04-29 07:50:37.585872 cg-60.4.7/cg/services/delivery_message/utils.py
+-rw-r--r--   0        0        0        0 2024-04-29 07:50:37.585872 cg-60.4.7/cg/services/fastq_file_service/__init__.py
+-rw-r--r--   0        0        0      101 2024-04-29 07:50:37.585872 cg-60.4.7/cg/services/fastq_file_service/exceptions.py
+-rw-r--r--   0        0        0     1092 2024-04-29 07:50:37.585872 cg-60.4.7/cg/services/fastq_file_service/fastq_file_service.py
+-rw-r--r--   0        0        0     2991 2024-04-29 07:50:37.585872 cg-60.4.7/cg/services/fastq_file_service/utils.py
+-rw-r--r--   0        0        0        0 2024-04-29 07:50:37.585872 cg-60.4.7/cg/services/orders/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-29 07:50:37.585872 cg-60.4.7/cg/services/orders/order_service/__init__.py
+-rw-r--r--   0        0        0     2684 2024-04-29 07:50:37.585872 cg-60.4.7/cg/services/orders/order_service/order_service.py
+-rw-r--r--   0        0        0     1214 2024-04-29 07:50:37.585872 cg-60.4.7/cg/services/orders/order_service/utils.py
+-rw-r--r--   0        0        0       94 2024-04-29 07:50:37.585872 cg-60.4.7/cg/services/orders/order_status_service/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-29 07:50:37.585872 cg-60.4.7/cg/services/orders/order_status_service/dto/__init__.py
+-rw-r--r--   0        0        0      192 2024-04-29 07:50:37.585872 cg-60.4.7/cg/services/orders/order_status_service/dto/case_summary.py
+-rw-r--r--   0        0        0      289 2024-04-29 07:50:37.585872 cg-60.4.7/cg/services/orders/order_status_service/dto/order_summary.py
+-rw-r--r--   0        0        0     1768 2024-04-29 07:50:37.585872 cg-60.4.7/cg/services/orders/order_status_service/order_summary_service.py
+-rw-r--r--   0        0        0     1737 2024-04-29 07:50:37.585872 cg-60.4.7/cg/services/orders/order_status_service/utils.py
+-rw-r--r--   0        0        0       95 2024-04-29 07:50:37.585872 cg-60.4.7/cg/services/quality_controller/__init__.py
+-rw-r--r--   0        0        0     1819 2024-04-29 07:50:37.585872 cg-60.4.7/cg/services/quality_controller/quality_checks/checks.py
+-rw-r--r--   0        0        0     4987 2024-04-29 07:50:37.585872 cg-60.4.7/cg/services/quality_controller/quality_checks/utils.py
+-rw-r--r--   0        0        0     1040 2024-04-29 07:50:37.585872 cg-60.4.7/cg/services/quality_controller/quality_controller_service.py
+-rw-r--r--   0        0        0        0 2024-04-29 07:50:37.585872 cg-60.4.7/cg/services/slurm_service/__init__.py
+-rw-r--r--   0        0        0      703 2024-04-29 07:50:37.585872 cg-60.4.7/cg/services/slurm_service/slurm_cli_service.py
+-rw-r--r--   0        0        0      242 2024-04-29 07:50:37.585872 cg-60.4.7/cg/services/slurm_service/slurm_service.py
+-rw-r--r--   0        0        0        0 2024-04-29 07:50:37.585872 cg-60.4.7/cg/services/slurm_upload_service/__init__.py
+-rw-r--r--   0        0        0      175 2024-04-29 07:50:37.585872 cg-60.4.7/cg/services/slurm_upload_service/slurm_upload_config.py
+-rw-r--r--   0        0        0     2074 2024-04-29 07:50:37.585872 cg-60.4.7/cg/services/slurm_upload_service/slurm_upload_service.py
+-rw-r--r--   0        0        0      203 2024-04-29 07:50:37.585872 cg-60.4.7/cg/services/slurm_upload_service/utils.py
+-rw-r--r--   0        0        0        0 2024-04-29 07:50:37.585872 cg-60.4.7/cg/store/__init__.py
+-rw-r--r--   0        0        0     4650 2024-04-29 07:50:37.585872 cg-60.4.7/cg/store/base.py
+-rw-r--r--   0        0        0        0 2024-04-29 07:50:37.585872 cg-60.4.7/cg/store/crud/__init__.py
+-rw-r--r--   0        0        0    13100 2024-04-29 07:50:37.585872 cg-60.4.7/cg/store/crud/create.py
+-rw-r--r--   0        0        0     2144 2024-04-29 07:50:37.585872 cg-60.4.7/cg/store/crud/delete.py
+-rw-r--r--   0        0        0    60036 2024-04-29 07:50:37.585872 cg-60.4.7/cg/store/crud/read.py
+-rw-r--r--   0        0        0     1121 2024-04-29 07:50:37.585872 cg-60.4.7/cg/store/crud/update.py
+-rw-r--r--   0        0        0     1662 2024-04-29 07:50:37.585872 cg-60.4.7/cg/store/database.py
+-rw-r--r--   0        0        0        0 2024-04-29 07:50:37.585872 cg-60.4.7/cg/store/filters/__init__.py
+-rw-r--r--   0        0        0     5371 2024-04-29 07:50:37.585872 cg-60.4.7/cg/store/filters/status_analysis_filters.py
+-rw-r--r--   0        0        0     1712 2024-04-29 07:50:37.585872 cg-60.4.7/cg/store/filters/status_application_filters.py
+-rw-r--r--   0        0        0     1440 2024-04-29 07:50:37.585872 cg-60.4.7/cg/store/filters/status_application_limitations_filters.py
+-rw-r--r--   0        0        0     2523 2024-04-29 07:50:37.585872 cg-60.4.7/cg/store/filters/status_application_version_filters.py
+-rw-r--r--   0        0        0     1390 2024-04-29 07:50:37.585872 cg-60.4.7/cg/store/filters/status_bed_filters.py
+-rw-r--r--   0        0        0     1317 2024-04-29 07:50:37.585872 cg-60.4.7/cg/store/filters/status_bed_version_filters.py
+-rw-r--r--   0        0        0    10787 2024-04-29 07:50:37.585872 cg-60.4.7/cg/store/filters/status_case_filters.py
+-rw-r--r--   0        0        0     3272 2024-04-29 07:50:37.585872 cg-60.4.7/cg/store/filters/status_case_sample_filters.py
+-rw-r--r--   0        0        0      903 2024-04-29 07:50:37.585872 cg-60.4.7/cg/store/filters/status_collaboration_filters.py
+-rw-r--r--   0        0        0     1412 2024-04-29 07:50:37.585872 cg-60.4.7/cg/store/filters/status_customer_filters.py
+-rw-r--r--   0        0        0     1880 2024-04-29 07:50:37.585872 cg-60.4.7/cg/store/filters/status_flow_cell_filters.py
+-rw-r--r--   0        0        0     1255 2024-04-29 07:50:37.585872 cg-60.4.7/cg/store/filters/status_invoice_filters.py
+-rw-r--r--   0        0        0     2792 2024-04-29 07:50:37.585872 cg-60.4.7/cg/store/filters/status_metrics_filters.py
+-rw-r--r--   0        0        0     3225 2024-04-29 07:50:37.589872 cg-60.4.7/cg/store/filters/status_order_filters.py
+-rw-r--r--   0        0        0      851 2024-04-29 07:50:37.589872 cg-60.4.7/cg/store/filters/status_organism_filters.py
+-rw-r--r--   0        0        0      783 2024-04-29 07:50:37.589872 cg-60.4.7/cg/store/filters/status_panel_filters.py
+-rw-r--r--   0        0        0     3923 2024-04-29 07:50:37.589872 cg-60.4.7/cg/store/filters/status_pool_filters.py
+-rw-r--r--   0        0        0     8660 2024-04-29 07:50:37.589872 cg-60.4.7/cg/store/filters/status_sample_filters.py
+-rw-r--r--   0        0        0      731 2024-04-29 07:50:37.589872 cg-60.4.7/cg/store/filters/status_user_filters.py
+-rw-r--r--   0        0        0    36081 2024-04-29 07:50:37.589872 cg-60.4.7/cg/store/models.py
+-rw-r--r--   0        0        0      593 2024-04-29 07:50:37.589872 cg-60.4.7/cg/store/store.py
+-rw-r--r--   0        0        0       30 2024-04-29 07:50:37.589872 cg-60.4.7/cg/utils/__init__.py
+-rw-r--r--   0        0        0      187 2024-04-29 07:50:37.589872 cg-60.4.7/cg/utils/calculations.py
+-rw-r--r--   0        0        0        0 2024-04-29 07:50:37.589872 cg-60.4.7/cg/utils/checksum/__init__.py
+-rw-r--r--   0        0        0     1579 2024-04-29 07:50:37.589872 cg-60.4.7/cg/utils/checksum/checksum.py
+-rw-r--r--   0        0        0     1655 2024-04-29 07:50:37.589872 cg-60.4.7/cg/utils/click/EnumChoice.py
+-rw-r--r--   0        0        0        0 2024-04-29 07:50:37.589872 cg-60.4.7/cg/utils/click/__init__.py
+-rw-r--r--   0        0        0     4910 2024-04-29 07:50:37.589872 cg-60.4.7/cg/utils/commands.py
+-rw-r--r--   0        0        0     1811 2024-04-29 07:50:37.589872 cg-60.4.7/cg/utils/date.py
+-rw-r--r--   0        0        0      635 2024-04-29 07:50:37.589872 cg-60.4.7/cg/utils/dict.py
+-rw-r--r--   0        0        0     2111 2024-04-29 07:50:37.589872 cg-60.4.7/cg/utils/dispatcher.py
+-rw-r--r--   0        0        0     1251 2024-04-29 07:50:37.589872 cg-60.4.7/cg/utils/email.py
+-rw-r--r--   0        0        0      134 2024-04-29 07:50:37.589872 cg-60.4.7/cg/utils/enums.py
+-rw-r--r--   0        0        0     3178 2024-04-29 07:50:37.589872 cg-60.4.7/cg/utils/files.py
+-rw-r--r--   0        0        0        0 2024-04-29 07:50:37.589872 cg-60.4.7/cg/utils/flask/__init__.py
+-rw-r--r--   0        0        0     1052 2024-04-29 07:50:37.589872 cg-60.4.7/cg/utils/flask/enum.py
+-rw-r--r--   0        0        0      233 2024-04-29 07:50:37.589872 cg-60.4.7/cg/utils/flow_cell.py
+-rw-r--r--   0        0        0      834 2024-04-29 07:50:37.589872 cg-60.4.7/cg/utils/time.py
+-rw-r--r--   0        0        0     1410 2024-04-29 07:50:37.589872 cg-60.4.7/cg/utils/utils.py
+-rw-r--r--   0        0        0     1697 2024-04-29 07:50:37.589872 cg-60.4.7/pyproject.toml
+-rw-r--r--   0        0        0        0 2024-04-29 07:50:37.589872 cg-60.4.7/tests/__init__.py
+-rw-r--r--   0        0        0     1158 2024-04-29 07:50:37.589872 cg-60.4.7/tests/apps/conftest.py
+-rw-r--r--   0        0        0      231 2024-04-29 07:50:37.589872 cg-60.4.7/tests/apps/coverage/conftest.py
+-rw-r--r--   0        0        0     6188 2024-04-29 07:50:37.589872 cg-60.4.7/tests/apps/coverage/test_coverage.py
+-rw-r--r--   0        0        0     1693 2024-04-29 07:50:37.593872 cg-60.4.7/tests/apps/crunchy/conftest.py
+-rw-r--r--   0        0        0     5438 2024-04-29 07:50:37.593872 cg-60.4.7/tests/apps/crunchy/test_compress_fastq.py
+-rw-r--r--   0        0        0     2283 2024-04-29 07:50:37.593872 cg-60.4.7/tests/apps/crunchy/test_config.py
+-rw-r--r--   0        0        0    14032 2024-04-29 07:50:37.593872 cg-60.4.7/tests/apps/crunchy/test_crunchy.py
+-rw-r--r--   0        0        0     9109 2024-04-29 07:50:37.593872 cg-60.4.7/tests/apps/crunchy/test_spring_decompression.py
+-rw-r--r--   0        0        0        0 2024-04-29 07:50:37.593872 cg-60.4.7/tests/apps/demultiplex/__init__.py
+-rw-r--r--   0        0        0     4994 2024-04-29 07:50:37.593872 cg-60.4.7/tests/apps/demultiplex/conftest.py
+-rw-r--r--   0        0        0     4010 2024-04-29 07:50:37.593872 cg-60.4.7/tests/apps/demultiplex/test_create_sample_sheet.py
+-rw-r--r--   0        0        0     7986 2024-04-29 07:50:37.593872 cg-60.4.7/tests/apps/demultiplex/test_demultiplex_api.py
+-rw-r--r--   0        0        0     4782 2024-04-29 07:50:37.593872 cg-60.4.7/tests/apps/demultiplex/test_index.py
+-rw-r--r--   0        0        0     9468 2024-04-29 07:50:37.593872 cg-60.4.7/tests/apps/demultiplex/test_override_cycles_validator.py
+-rw-r--r--   0        0        0     4042 2024-04-29 07:50:37.593872 cg-60.4.7/tests/apps/demultiplex/test_read_sample_sheet.py
+-rw-r--r--   0        0        0    12389 2024-04-29 07:50:37.593872 cg-60.4.7/tests/apps/demultiplex/test_sample_models.py
+-rw-r--r--   0        0        0      951 2024-04-29 07:50:37.593872 cg-60.4.7/tests/apps/demultiplex/test_sample_sheet_creator.py
+-rw-r--r--   0        0        0     3175 2024-04-29 07:50:37.593872 cg-60.4.7/tests/apps/demultiplex/test_sample_sheet_models.py
+-rw-r--r--   0        0        0    10932 2024-04-29 07:50:37.593872 cg-60.4.7/tests/apps/demultiplex/test_sample_sheet_validator.py
+-rw-r--r--   0        0        0     4896 2024-04-29 07:50:37.593872 cg-60.4.7/tests/apps/demultiplex/test_translate_sample_sheet.py
+-rw-r--r--   0        0        0     1450 2024-04-29 07:50:37.593872 cg-60.4.7/tests/apps/demultiplex/test_validate.py
+-rw-r--r--   0        0        0     5094 2024-04-29 07:50:37.593872 cg-60.4.7/tests/apps/downsample/test_downsample.py
+-rw-r--r--   0        0        0     1419 2024-04-29 07:50:37.593872 cg-60.4.7/tests/apps/downsample/test_downsample_utils.py
+-rw-r--r--   0        0        0     1716 2024-04-29 07:50:37.593872 cg-60.4.7/tests/apps/gens/test_gens_api.py
+-rw-r--r--   0        0        0     1950 2024-04-29 07:50:37.593872 cg-60.4.7/tests/apps/gt/conftest.py
+-rw-r--r--   0        0        0     4276 2024-04-29 07:50:37.593872 cg-60.4.7/tests/apps/gt/test_gt_api.py
+-rw-r--r--   0        0        0     1453 2024-04-29 07:50:37.593872 cg-60.4.7/tests/apps/hk/conftest.py
+-rw-r--r--   0        0        0      684 2024-04-29 07:50:37.593872 cg-60.4.7/tests/apps/hk/test__getattr__.py
+-rw-r--r--   0        0        0     1593 2024-04-29 07:50:37.593872 cg-60.4.7/tests/apps/hk/test_add_file.py
+-rw-r--r--   0        0        0     3523 2024-04-29 07:50:37.593872 cg-60.4.7/tests/apps/hk/test_bundles.py
+-rw-r--r--   0        0        0      871 2024-04-29 07:50:37.593872 cg-60.4.7/tests/apps/hk/test_core.py
+-rw-r--r--   0        0        0    31172 2024-04-29 07:50:37.593872 cg-60.4.7/tests/apps/hk/test_file.py
+-rw-r--r--   0        0        0     5080 2024-04-29 07:50:37.593872 cg-60.4.7/tests/apps/hk/test_version.py
+-rw-r--r--   0        0        0     1840 2024-04-29 07:50:37.593872 cg-60.4.7/tests/apps/lims/conftest.py
+-rw-r--r--   0        0        0     3197 2024-04-29 07:50:37.593872 cg-60.4.7/tests/apps/lims/test_api.py
+-rw-r--r--   0        0        0     1451 2024-04-29 07:50:37.593872 cg-60.4.7/tests/apps/lims/test_sample_sheet.py
+-rw-r--r--   0        0        0     9223 2024-04-29 07:50:37.593872 cg-60.4.7/tests/apps/loqus/conftest.py
+-rw-r--r--   0        0        0     8994 2024-04-29 07:50:37.593872 cg-60.4.7/tests/apps/loqus/test_loqusdb_api.py
+-rw-r--r--   0        0        0     2439 2024-04-29 07:50:37.593872 cg-60.4.7/tests/apps/madeline/conftest.py
+-rw-r--r--   0        0        0     4653 2024-04-29 07:50:37.593872 cg-60.4.7/tests/apps/madeline/test_madeline.py
+-rw-r--r--   0        0        0     3328 2024-04-29 07:50:37.593872 cg-60.4.7/tests/apps/mip/conftest.py
+-rw-r--r--   0        0        0     2487 2024-04-29 07:50:37.593872 cg-60.4.7/tests/apps/mip/test_config_mip.py
+-rw-r--r--   0        0        0      883 2024-04-29 07:50:37.593872 cg-60.4.7/tests/apps/mutacc_auto/conftest.py
+-rw-r--r--   0        0        0     2473 2024-04-29 07:50:37.593872 cg-60.4.7/tests/apps/mutacc_auto/test_mutacc_auto.py
+-rw-r--r--   0        0        0    11930 2024-04-29 07:50:37.593872 cg-60.4.7/tests/apps/orderform/conftest.py
+-rw-r--r--   0        0        0     9484 2024-04-29 07:50:37.593872 cg-60.4.7/tests/apps/orderform/test_excel_orderform_parser.py
+-rw-r--r--   0        0        0     4351 2024-04-29 07:50:37.593872 cg-60.4.7/tests/apps/orderform/test_excel_sample_schema.py
+-rw-r--r--   0        0        0     1032 2024-04-29 07:50:37.593872 cg-60.4.7/tests/apps/orderform/test_json_orderform_parser.py
+-rw-r--r--   0        0        0     2474 2024-04-29 07:50:37.593872 cg-60.4.7/tests/apps/orderform/test_orderform_parser.py
+-rw-r--r--   0        0        0    16002 2024-04-29 07:50:37.593872 cg-60.4.7/tests/apps/orderform/validators/test_excel_sample_validators.py
+-rw-r--r--   0        0        0     3670 2024-04-29 07:50:37.593872 cg-60.4.7/tests/apps/scout/conftest.py
+-rw-r--r--   0        0        0     2269 2024-04-29 07:50:37.593872 cg-60.4.7/tests/apps/scout/test_get_causative_variants.py
+-rw-r--r--   0        0        0     1376 2024-04-29 07:50:37.593872 cg-60.4.7/tests/apps/scout/test_get_scout_cases.py
+-rw-r--r--   0        0        0     1840 2024-04-29 07:50:37.593872 cg-60.4.7/tests/apps/scout/test_scout_load_config.py
+-rw-r--r--   0        0        0     7047 2024-04-29 07:50:37.593872 cg-60.4.7/tests/apps/scout/test_scout_models.py
+-rw-r--r--   0        0        0        0 2024-04-29 07:50:37.593872 cg-60.4.7/tests/apps/sequencing_metrics_parser/__init__.py
+-rw-r--r--   0        0        0     2639 2024-04-29 07:50:37.593872 cg-60.4.7/tests/apps/sequencing_metrics_parser/conftest.py
+-rw-r--r--   0        0        0     7069 2024-04-29 07:50:37.593872 cg-60.4.7/tests/apps/sequencing_metrics_parser/parsers/test_bclconvert.py
+-rw-r--r--   0        0        0     2958 2024-04-29 07:50:37.593872 cg-60.4.7/tests/apps/sequencing_metrics_parser/parsers/test_sequencing_metrics_parser_api.py
+-rw-r--r--   0        0        0     1131 2024-04-29 07:50:37.593872 cg-60.4.7/tests/apps/slurm/conftest.py
+-rw-r--r--   0        0        0     4412 2024-04-29 07:50:37.593872 cg-60.4.7/tests/apps/slurm/test_slurm_api.py
+-rw-r--r--   0        0        0      831 2024-04-29 07:50:37.593872 cg-60.4.7/tests/apps/test_apps_environ.py
+-rw-r--r--   0        0        0      957 2024-04-29 07:50:37.593872 cg-60.4.7/tests/apps/test_osticket.py
+-rw-r--r--   0        0        0        0 2024-04-29 07:50:37.593872 cg-60.4.7/tests/cli/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-29 07:50:37.593872 cg-60.4.7/tests/cli/add/__init__.py
+-rw-r--r--   0        0        0     1174 2024-04-29 07:50:37.593872 cg-60.4.7/tests/cli/add/test_cli_add.py
+-rw-r--r--   0        0        0     2471 2024-04-29 07:50:37.593872 cg-60.4.7/tests/cli/add/test_cli_add_customer.py
+-rw-r--r--   0        0        0     6841 2024-04-29 07:50:37.593872 cg-60.4.7/tests/cli/add/test_cli_add_family.py
+-rw-r--r--   0        0        0     7588 2024-04-29 07:50:37.593872 cg-60.4.7/tests/cli/add/test_cli_add_relationship.py
+-rw-r--r--   0        0        0     8382 2024-04-29 07:50:37.593872 cg-60.4.7/tests/cli/add/test_cli_add_sample.py
+-rw-r--r--   0        0        0        0 2024-04-29 07:50:37.593872 cg-60.4.7/tests/cli/backup/__init__.py
+-rw-r--r--   0        0        0      705 2024-04-29 07:50:37.593872 cg-60.4.7/tests/cli/backup/conftest.py
+-rw-r--r--   0        0        0    11101 2024-04-29 07:50:37.593872 cg-60.4.7/tests/cli/backup/test_backup_command.py
+-rw-r--r--   0        0        0     6865 2024-04-29 07:50:37.593872 cg-60.4.7/tests/cli/clean/conftest.py
+-rw-r--r--   0        0        0     5536 2024-04-29 07:50:37.593872 cg-60.4.7/tests/cli/clean/test_balsamic_clean.py
+-rw-r--r--   0        0        0     2557 2024-04-29 07:50:37.597872 cg-60.4.7/tests/cli/clean/test_clean_flow_cell.py
+-rw-r--r--   0        0        0     1830 2024-04-29 07:50:37.597872 cg-60.4.7/tests/cli/clean/test_clean_hk_bundle_files.py
+-rw-r--r--   0        0        0     2098 2024-04-29 07:50:37.597872 cg-60.4.7/tests/cli/clean/test_hk_bundle_files.py
+-rw-r--r--   0        0        0     4610 2024-04-29 07:50:37.597872 cg-60.4.7/tests/cli/clean/test_hk_case_bundle_files.py
+-rw-r--r--   0        0        0     3585 2024-04-29 07:50:37.597872 cg-60.4.7/tests/cli/clean/test_microbial_clean.py
+-rw-r--r--   0        0        0     1881 2024-04-29 07:50:37.597872 cg-60.4.7/tests/cli/clean/test_rsync_past_run_dirs.py
+-rw-r--r--   0        0        0     9707 2024-04-29 07:50:37.597872 cg-60.4.7/tests/cli/compress/conftest.py
+-rw-r--r--   0        0        0     7709 2024-04-29 07:50:37.597872 cg-60.4.7/tests/cli/compress/test_cli_compress_fastq.py
+-rw-r--r--   0        0        0     1416 2024-04-29 07:50:37.597872 cg-60.4.7/tests/cli/compress/test_cli_decompress_spring.py
+-rw-r--r--   0        0        0     5205 2024-04-29 07:50:37.597872 cg-60.4.7/tests/cli/compress/test_compress_helpers.py
+-rw-r--r--   0        0        0     1239 2024-04-29 07:50:37.597872 cg-60.4.7/tests/cli/compress/test_store_fastq.py
+-rw-r--r--   0        0        0     7558 2024-04-29 07:50:37.597872 cg-60.4.7/tests/cli/conftest.py
+-rw-r--r--   0        0        0    12747 2024-04-29 07:50:37.597872 cg-60.4.7/tests/cli/delete/test_cli_delete_case.py
+-rw-r--r--   0        0        0     1873 2024-04-29 07:50:37.597872 cg-60.4.7/tests/cli/delete/test_cli_delete_cases.py
+-rw-r--r--   0        0        0     3794 2024-04-29 07:50:37.597872 cg-60.4.7/tests/cli/deliver/conftest.py
+-rw-r--r--   0        0        0     4428 2024-04-29 07:50:37.597872 cg-60.4.7/tests/cli/deliver/test_deliver_base.py
+-rw-r--r--   0        0        0     1166 2024-04-29 07:50:37.597872 cg-60.4.7/tests/cli/deliver/test_rsync_base.py
+-rw-r--r--   0        0        0     8569 2024-04-29 07:50:37.597872 cg-60.4.7/tests/cli/deliver/test_run_deliver_cmd.py
+-rw-r--r--   0        0        0        0 2024-04-29 07:50:37.597872 cg-60.4.7/tests/cli/demultiplex/__init__.py
+-rw-r--r--   0        0        0     5109 2024-04-29 07:50:37.597872 cg-60.4.7/tests/cli/demultiplex/test_create_sample_sheet.py
+-rw-r--r--   0        0        0     4799 2024-04-29 07:50:37.597872 cg-60.4.7/tests/cli/demultiplex/test_demultiplex_flowcell.py
+-rw-r--r--   0        0        0     1639 2024-04-29 07:50:37.597872 cg-60.4.7/tests/cli/demultiplex/test_finish_demux.py
+-rw-r--r--   0        0        0     3015 2024-04-29 07:50:37.597872 cg-60.4.7/tests/cli/demultiplex/test_validate_sample_sheet.py
+-rw-r--r--   0        0        0     4291 2024-04-29 07:50:37.597872 cg-60.4.7/tests/cli/demultiplex/test_verify_syncing.py
+-rw-r--r--   0        0        0     1585 2024-04-29 07:50:37.597872 cg-60.4.7/tests/cli/downsample/test_cli_downsample.py
+-rw-r--r--   0        0        0        0 2024-04-29 07:50:37.597872 cg-60.4.7/tests/cli/generate/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-29 07:50:37.597872 cg-60.4.7/tests/cli/generate/report/__init__.py
+-rw-r--r--   0        0        0     1622 2024-04-29 07:50:37.597872 cg-60.4.7/tests/cli/generate/report/conftest.py
+-rw-r--r--   0        0        0     2477 2024-04-29 07:50:37.597872 cg-60.4.7/tests/cli/generate/report/test_cli_delivery_report.py
+-rw-r--r--   0        0        0     2760 2024-04-29 07:50:37.597872 cg-60.4.7/tests/cli/generate/report/test_utils.py
+-rw-r--r--   0        0        0      563 2024-04-29 07:50:37.597872 cg-60.4.7/tests/cli/generate/test_cli_base.py
+-rw-r--r--   0        0        0        0 2024-04-29 07:50:37.597872 cg-60.4.7/tests/cli/get/__init__.py
+-rw-r--r--   0        0        0      863 2024-04-29 07:50:37.597872 cg-60.4.7/tests/cli/get/test_cli_get.py
+-rw-r--r--   0        0        0     1526 2024-04-29 07:50:37.597872 cg-60.4.7/tests/cli/get/test_cli_get_analysis.py
+-rw-r--r--   0        0        0     1242 2024-04-29 07:50:37.597872 cg-60.4.7/tests/cli/get/test_cli_get_case.py
+-rw-r--r--   0        0        0     6208 2024-04-29 07:50:37.597872 cg-60.4.7/tests/cli/get/test_cli_get_flow_cell.py
+-rw-r--r--   0        0        0     8835 2024-04-29 07:50:37.597872 cg-60.4.7/tests/cli/get/test_cli_get_sample.py
+-rw-r--r--   0        0        0     1364 2024-04-29 07:50:37.597872 cg-60.4.7/tests/cli/set/conftest.py
+-rw-r--r--   0        0        0     7311 2024-04-29 07:50:37.597872 cg-60.4.7/tests/cli/set/test_cli_set_case.py
+-rw-r--r--   0        0        0     1460 2024-04-29 07:50:37.597872 cg-60.4.7/tests/cli/set/test_cli_set_cases.py
+-rw-r--r--   0        0        0     2016 2024-04-29 07:50:37.597872 cg-60.4.7/tests/cli/set/test_cli_set_flowcell.py
+-rw-r--r--   0        0        0     1685 2024-04-29 07:50:37.597872 cg-60.4.7/tests/cli/set/test_cli_set_list_keys.py
+-rw-r--r--   0        0        0    12450 2024-04-29 07:50:37.597872 cg-60.4.7/tests/cli/set/test_cli_set_sample.py
+-rw-r--r--   0        0        0     6124 2024-04-29 07:50:37.597872 cg-60.4.7/tests/cli/set/test_cli_set_samples.py
+-rw-r--r--   0        0        0     7015 2024-04-29 07:50:37.597872 cg-60.4.7/tests/cli/store/test_store.py
+-rw-r--r--   0        0        0     2332 2024-04-29 07:50:37.597872 cg-60.4.7/tests/cli/test_base.py
+-rw-r--r--   0        0        0        0 2024-04-29 07:50:37.597872 cg-60.4.7/tests/cli/upload/__init__.py
+-rw-r--r--   0        0        0    10057 2024-04-29 07:50:37.597872 cg-60.4.7/tests/cli/upload/conftest.py
+-rw-r--r--   0        0        0     2295 2024-04-29 07:50:37.597872 cg-60.4.7/tests/cli/upload/test_cli_scout.py
+-rw-r--r--   0        0        0     1789 2024-04-29 07:50:37.597872 cg-60.4.7/tests/cli/upload/test_cli_upload.py
+-rw-r--r--   0        0        0      971 2024-04-29 07:50:37.597872 cg-60.4.7/tests/cli/upload/test_cli_upload_auto.py
+-rw-r--r--   0        0        0     1669 2024-04-29 07:50:37.597872 cg-60.4.7/tests/cli/upload/test_cli_upload_delivery_report.py
+-rw-r--r--   0        0        0      895 2024-04-29 07:50:37.597872 cg-60.4.7/tests/cli/upload/test_cli_upload_fastq.py
+-rw-r--r--   0        0        0     1199 2024-04-29 07:50:37.597872 cg-60.4.7/tests/cli/upload/test_cli_upload_genotype.py
+-rw-r--r--   0        0        0      694 2024-04-29 07:50:37.597872 cg-60.4.7/tests/cli/upload/test_cli_upload_gens.py
+-rw-r--r--   0        0        0     9965 2024-04-29 07:50:37.597872 cg-60.4.7/tests/cli/upload/test_cli_upload_nipt.py
+-rw-r--r--   0        0        0     4684 2024-04-29 07:50:37.597872 cg-60.4.7/tests/cli/upload/test_cli_upload_nipt_ftp.py
+-rw-r--r--   0        0        0     1839 2024-04-29 07:50:37.597872 cg-60.4.7/tests/cli/upload/test_cli_upload_nipt_statina.py
+-rw-r--r--   0        0        0     6177 2024-04-29 07:50:37.597872 cg-60.4.7/tests/cli/upload/test_cli_upload_observations.py
+-rw-r--r--   0        0        0        0 2024-04-29 07:50:37.597872 cg-60.4.7/tests/cli/workflow/__init__.py
+-rw-r--r--   0        0        0    31369 2024-04-29 07:50:37.597872 cg-60.4.7/tests/cli/workflow/balsamic/conftest.py
+-rw-r--r--   0        0        0    13938 2024-04-29 07:50:37.597872 cg-60.4.7/tests/cli/workflow/balsamic/test_cli_balsamic_config_case.py
+-rw-r--r--   0        0        0     7984 2024-04-29 07:50:37.597872 cg-60.4.7/tests/cli/workflow/balsamic/test_compound_commands.py
+-rw-r--r--   0        0        0     2336 2024-04-29 07:50:37.597872 cg-60.4.7/tests/cli/workflow/balsamic/test_link.py
+-rw-r--r--   0        0        0     3554 2024-04-29 07:50:37.597872 cg-60.4.7/tests/cli/workflow/balsamic/test_report_deliver.py
+-rw-r--r--   0        0        0     6209 2024-04-29 07:50:37.597872 cg-60.4.7/tests/cli/workflow/balsamic/test_run.py
+-rw-r--r--   0        0        0     6934 2024-04-29 07:50:37.597872 cg-60.4.7/tests/cli/workflow/balsamic/test_store_housekeeper.py
+-rw-r--r--   0        0        0     8458 2024-04-29 07:50:37.597872 cg-60.4.7/tests/cli/workflow/conftest.py
+-rw-r--r--   0        0        0        0 2024-04-29 07:50:37.597872 cg-60.4.7/tests/cli/workflow/fastq/__init__.py
+-rw-r--r--   0        0        0     2332 2024-04-29 07:50:37.597872 cg-60.4.7/tests/cli/workflow/fastq/test_fastq_base.py
+-rw-r--r--   0        0        0        0 2024-04-29 07:50:37.597872 cg-60.4.7/tests/cli/workflow/fluffy/__init__.py
+-rw-r--r--   0        0        0     5237 2024-04-29 07:50:37.597872 cg-60.4.7/tests/cli/workflow/fluffy/conftest.py
+-rw-r--r--   0        0        0     5687 2024-04-29 07:50:37.597872 cg-60.4.7/tests/cli/workflow/fluffy/test_cli_create_samplesheet.py
+-rw-r--r--   0        0        0     3302 2024-04-29 07:50:37.597872 cg-60.4.7/tests/cli/workflow/fluffy/test_cli_link.py
+-rw-r--r--   0        0        0     1896 2024-04-29 07:50:37.597872 cg-60.4.7/tests/cli/workflow/fluffy/test_cli_run.py
+-rw-r--r--   0        0        0     2968 2024-04-29 07:50:37.597872 cg-60.4.7/tests/cli/workflow/fluffy/test_cli_start.py
+-rw-r--r--   0        0        0     7815 2024-04-29 07:50:37.597872 cg-60.4.7/tests/cli/workflow/fluffy/test_cli_store.py
+-rw-r--r--   0        0        0     2775 2024-04-29 07:50:37.597872 cg-60.4.7/tests/cli/workflow/microsalt/conftest.py
+-rw-r--r--   0        0        0     6926 2024-04-29 07:50:37.597872 cg-60.4.7/tests/cli/workflow/microsalt/test_microsalt_case_config.py
+-rw-r--r--   0        0        0     1000 2024-04-29 07:50:37.601872 cg-60.4.7/tests/cli/workflow/microsalt/test_microsalt_run.py
+-rw-r--r--   0        0        0     6544 2024-04-29 07:50:37.601872 cg-60.4.7/tests/cli/workflow/mip/conftest.py
+-rw-r--r--   0        0        0     7011 2024-04-29 07:50:37.601872 cg-60.4.7/tests/cli/workflow/mip/test_cli_mip_base.py
+-rw-r--r--   0        0        0     1542 2024-04-29 07:50:37.601872 cg-60.4.7/tests/cli/workflow/mip/test_cli_mip_dna_config_case.py
+-rw-r--r--   0        0        0      431 2024-04-29 07:50:37.601872 cg-60.4.7/tests/cli/workflow/mip/test_cli_mip_dna_link.py
+-rw-r--r--   0        0        0     2108 2024-04-29 07:50:37.601872 cg-60.4.7/tests/cli/workflow/mip/test_cli_mip_dna_manged_variants.py
+-rw-r--r--   0        0        0     1273 2024-04-29 07:50:37.601872 cg-60.4.7/tests/cli/workflow/mip/test_cli_mip_dna_panel.py
+-rw-r--r--   0        0        0     3595 2024-04-29 07:50:37.601872 cg-60.4.7/tests/cli/workflow/mip/test_cli_mip_dna_run.py
+-rw-r--r--   0        0        0     3884 2024-04-29 07:50:37.601872 cg-60.4.7/tests/cli/workflow/mip/test_cli_mip_dna_start.py
+-rw-r--r--   0        0        0     1004 2024-04-29 07:50:37.601872 cg-60.4.7/tests/cli/workflow/mip/test_cli_mip_rna_config_case.py
+-rw-r--r--   0        0        0      527 2024-04-29 07:50:37.601872 cg-60.4.7/tests/cli/workflow/mip/test_cli_mip_rna_link.py
+-rw-r--r--   0        0        0      716 2024-04-29 07:50:37.601872 cg-60.4.7/tests/cli/workflow/mip/test_cli_mip_rna_run.py
+-rw-r--r--   0        0        0     8559 2024-04-29 07:50:37.601872 cg-60.4.7/tests/cli/workflow/mip/test_cli_mip_store.py
+-rw-r--r--   0        0        0        0 2024-04-29 07:50:37.601872 cg-60.4.7/tests/cli/workflow/nf_analysis/__init__.py
+-rw-r--r--   0        0        0     9318 2024-04-29 07:50:37.601872 cg-60.4.7/tests/cli/workflow/nf_analysis/test_cli_config_case.py
+-rw-r--r--   0        0        0     3831 2024-04-29 07:50:37.601872 cg-60.4.7/tests/cli/workflow/nf_analysis/test_cli_metrics_deliver.py
+-rw-r--r--   0        0        0     5087 2024-04-29 07:50:37.601872 cg-60.4.7/tests/cli/workflow/nf_analysis/test_cli_report_deliver.py
+-rw-r--r--   0        0        0     9211 2024-04-29 07:50:37.601872 cg-60.4.7/tests/cli/workflow/nf_analysis/test_cli_run.py
+-rw-r--r--   0        0        0     3267 2024-04-29 07:50:37.601872 cg-60.4.7/tests/cli/workflow/nf_analysis/test_cli_start.py
+-rw-r--r--   0        0        0     9877 2024-04-29 07:50:37.601872 cg-60.4.7/tests/cli/workflow/nf_analysis/test_cli_store.py
+-rw-r--r--   0        0        0    10373 2024-04-29 07:50:37.601872 cg-60.4.7/tests/cli/workflow/nf_analysis/test_cli_store_housekeeper.py
+-rw-r--r--   0        0        0      978 2024-04-29 07:50:37.601872 cg-60.4.7/tests/cli/workflow/nf_analysis/test_cli_workflow_base.py
+-rw-r--r--   0        0        0        0 2024-04-29 07:50:37.601872 cg-60.4.7/tests/cli/workflow/raredisease/__init__.py
+-rw-r--r--   0        0        0     3940 2024-04-29 07:50:37.601872 cg-60.4.7/tests/cli/workflow/raredisease/test_cli_raredisease_compound_commands.py
+-rw-r--r--   0        0        0      921 2024-04-29 07:50:37.601872 cg-60.4.7/tests/cli/workflow/test_cli_workflow.py
+-rw-r--r--   0        0        0     4310 2024-04-29 07:50:37.601872 cg-60.4.7/tests/cli/workflow/test_cli_workflow_clean.py
+-rw-r--r--   0        0        0        0 2024-04-29 07:50:37.601872 cg-60.4.7/tests/clients/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-29 07:50:37.601872 cg-60.4.7/tests/clients/arnold/__init__.py
+-rw-r--r--   0        0        0     1080 2024-04-29 07:50:37.601872 cg-60.4.7/tests/clients/arnold/conftest.py
+-rw-r--r--   0        0        0     1503 2024-04-29 07:50:37.601872 cg-60.4.7/tests/clients/arnold/test_arnold_api_client.py
+-rw-r--r--   0        0        0        0 2024-04-29 07:50:37.601872 cg-60.4.7/tests/clients/janus/__init__.py
+-rw-r--r--   0        0        0     2381 2024-04-29 07:50:37.601872 cg-60.4.7/tests/clients/janus/conftest.py
+-rw-r--r--   0        0        0     1716 2024-04-29 07:50:37.601872 cg-60.4.7/tests/clients/janus/test_janus_api_client.py
+-rw-r--r--   0        0        0   129141 2024-04-29 07:50:37.601872 cg-60.4.7/tests/conftest.py
+-rw-r--r--   0        0        0        0 2024-04-29 07:50:37.601872 cg-60.4.7/tests/fixture_plugins/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-29 07:50:37.601872 cg-60.4.7/tests/fixture_plugins/delivery_fixtures/__init__.py
+-rw-r--r--   0        0        0     2653 2024-04-29 07:50:37.601872 cg-60.4.7/tests/fixture_plugins/delivery_fixtures/bundle_fixtures.py
+-rw-r--r--   0        0        0     4972 2024-04-29 07:50:37.601872 cg-60.4.7/tests/fixture_plugins/delivery_fixtures/context_fixtures.py
+-rw-r--r--   0        0        0     1494 2024-04-29 07:50:37.601872 cg-60.4.7/tests/fixture_plugins/delivery_fixtures/path_fixtures.py
+-rw-r--r--   0        0        0        0 2024-04-29 07:50:37.601872 cg-60.4.7/tests/fixture_plugins/demultiplex_fixtures/__init__.py
+-rw-r--r--   0        0        0     4636 2024-04-29 07:50:37.601872 cg-60.4.7/tests/fixture_plugins/demultiplex_fixtures/flow_cell_fixtures.py
+-rw-r--r--   0        0        0     3413 2024-04-29 07:50:37.601872 cg-60.4.7/tests/fixture_plugins/demultiplex_fixtures/name_fixtures.py
+-rw-r--r--   0        0        0    20458 2024-04-29 07:50:37.601872 cg-60.4.7/tests/fixture_plugins/demultiplex_fixtures/path_fixtures.py
+-rw-r--r--   0        0        0     3412 2024-04-29 07:50:37.601872 cg-60.4.7/tests/fixture_plugins/demultiplex_fixtures/run_parameters_fixtures.py
+-rw-r--r--   0        0        0     5988 2024-04-29 07:50:37.601872 cg-60.4.7/tests/fixture_plugins/demultiplex_fixtures/sample_fixtures.py
+-rw-r--r--   0        0        0     8960 2024-04-29 07:50:37.601872 cg-60.4.7/tests/fixture_plugins/demultiplex_fixtures/sample_sheet_fixtures.py
+-rw-r--r--   0        0        0     3174 2024-04-29 07:50:37.601872 cg-60.4.7/tests/fixture_plugins/quality_controller_fixtures/sequencing_qc_check_scenario.py
+-rw-r--r--   0        0        0     4801 2024-04-29 07:50:37.601872 cg-60.4.7/tests/fixture_plugins/quality_controller_fixtures/sequencing_qc_fixtures.py
+-rw-r--r--   0        0        0     1304 2024-04-29 07:50:37.601872 cg-60.4.7/tests/fixture_plugins/timestamp_fixtures.py
+-rw-r--r--   0        0        0        0 2024-04-29 07:50:37.601872 cg-60.4.7/tests/fixtures/analysis/balsamic/tn_wgs/adm1.cram
+-rw-r--r--   0        0        0        0 2024-04-29 07:50:37.601872 cg-60.4.7/tests/fixtures/analysis/balsamic/tn_wgs/ascat.output.pdf
+-rw-r--r--   0        0        0        0 2024-04-29 07:50:37.601872 cg-60.4.7/tests/fixtures/analysis/balsamic/tn_wgs/snv.vcf
+-rw-r--r--   0        0        0        0 2024-04-29 07:50:37.601872 cg-60.4.7/tests/fixtures/analysis/balsamic/tn_wgs/sv.vcf
+-rw-r--r--   0        0        0    14644 2024-04-29 07:50:37.601872 cg-60.4.7/tests/fixtures/analysis/microsalt/ACC11111_qc_fail/ACC11111_qc_fail.json
+-rw-r--r--   0        0        0    15921 2024-04-29 07:50:37.601872 cg-60.4.7/tests/fixtures/analysis/microsalt/ACC22222_qc_pass/ACC22222_qc_pass.json
+-rw-r--r--   0        0        0        0 2024-04-29 07:50:37.601872 cg-60.4.7/tests/fixtures/analysis/mip/dna/ADM1.baf.bed.gz
+-rw-r--r--   0        0        0        0 2024-04-29 07:50:37.601872 cg-60.4.7/tests/fixtures/analysis/mip/dna/ADM1.cov.bed.gz
+-rw-r--r--   0        0        0        0 2024-04-29 07:50:37.601872 cg-60.4.7/tests/fixtures/analysis/mip/dna/ADM2.cram
+-rw-r--r--   0        0        0        0 2024-04-29 07:50:37.601872 cg-60.4.7/tests/fixtures/analysis/mip/dna/ADM3.cram
+-rw-r--r--   0        0        0        0 2024-04-29 07:50:37.605872 cg-60.4.7/tests/fixtures/analysis/mip/dna/adm1.cram
+-rw-r--r--   0        0        0        0 2024-04-29 07:50:37.605872 cg-60.4.7/tests/fixtures/analysis/mip/dna/adm1.mt.bam
+-rw-r--r--   0        0        0        0 2024-04-29 07:50:37.605872 cg-60.4.7/tests/fixtures/analysis/mip/dna/multiqc.html
+-rw-r--r--   0        0        0        0 2024-04-29 07:50:37.605872 cg-60.4.7/tests/fixtures/analysis/mip/dna/report.pdf
+-rw-r--r--   0        0        0        0 2024-04-29 07:50:37.605872 cg-60.4.7/tests/fixtures/analysis/mip/dna/smn.vcf
+-rw-r--r--   0        0        0        0 2024-04-29 07:50:37.605872 cg-60.4.7/tests/fixtures/analysis/mip/dna/snv.vcf
+-rw-r--r--   0        0        0        0 2024-04-29 07:50:37.605872 cg-60.4.7/tests/fixtures/analysis/mip/dna/snv_research.vcf
+-rw-r--r--   0        0        0        0 2024-04-29 07:50:37.605872 cg-60.4.7/tests/fixtures/analysis/mip/dna/str.vcf
+-rw-r--r--   0        0        0        0 2024-04-29 07:50:37.605872 cg-60.4.7/tests/fixtures/analysis/mip/dna/sv.vcf
+-rw-r--r--   0        0        0        0 2024-04-29 07:50:37.605872 cg-60.4.7/tests/fixtures/analysis/mip/dna/sv_research.vcf
+-rw-r--r--   0        0        0        0 2024-04-29 07:50:37.605872 cg-60.4.7/tests/fixtures/analysis/mip/dna/vcf2cytosure.txt
+-rw-r--r--   0        0        0       70 2024-04-29 07:50:37.605872 cg-60.4.7/tests/fixtures/analysis/nf-analysis/pipeline_params.config
+-rw-r--r--   0        0        0      195 2024-04-29 07:50:37.605872 cg-60.4.7/tests/fixtures/analysis/nf-analysis/pipeline_resource_optimisation.config
+-rw-r--r--   0        0        0      195 2024-04-29 07:50:37.605872 cg-60.4.7/tests/fixtures/analysis/nf-analysis/platform.config
+-rw-r--r--   0        0        0     8173 2024-04-29 07:50:37.605872 cg-60.4.7/tests/fixtures/analysis/raredisease/multiqc_data.json
+-rw-r--r--   0        0        0    20005 2024-04-29 07:50:37.605872 cg-60.4.7/tests/fixtures/analysis/raredisease/raredisease_case_enough_reads_metrics_deliverables.yaml
+-rw-r--r--   0        0        0     5497 2024-04-29 07:50:37.605872 cg-60.4.7/tests/fixtures/analysis/rnafusion/multiqc_data.json
+-rw-r--r--   0        0        0    12499 2024-04-29 07:50:37.605872 cg-60.4.7/tests/fixtures/analysis/rnafusion/rnafusion_case_enough_reads_metrics_deliverables.yaml
+-rw-r--r--   0        0        0     2873 2024-04-29 07:50:37.605872 cg-60.4.7/tests/fixtures/analysis/sample_coverage.bed
+-rw-r--r--   0        0        0     6506 2024-04-29 07:50:37.605872 cg-60.4.7/tests/fixtures/analysis/taxprofiler/multiqc_data.json
+-rw-r--r--   0        0        0    10513 2024-04-29 07:50:37.605872 cg-60.4.7/tests/fixtures/analysis/taxprofiler/taxprofiler_case_metrics_deliverables.yaml
+-rw-r--r--   0        0        0     5771 2024-04-29 07:50:37.605872 cg-60.4.7/tests/fixtures/analysis/tomte/multiqc_data.json
+-rw-r--r--   0        0        0    14859 2024-04-29 07:50:37.605872 cg-60.4.7/tests/fixtures/analysis/tomte/tomte_case_enough_reads_metrics_deliverables.yaml
+-rw-r--r--   0        0        0    10961 2024-04-29 07:50:37.605872 cg-60.4.7/tests/fixtures/apps/balsamic/case/config.json
+-rw-r--r--   0        0        0     3465 2024-04-29 07:50:37.605872 cg-60.4.7/tests/fixtures/apps/balsamic/case/metadata.yml
+-rw-r--r--   0        0        0       63 2024-04-29 07:50:37.605872 cg-60.4.7/tests/fixtures/apps/balsamic/case/metadata_directory.yml
+-rw-r--r--   0        0        0      165 2024-04-29 07:50:37.605872 cg-60.4.7/tests/fixtures/apps/balsamic/case/metadata_file_tags.yml
+-rw-r--r--   0        0        0     2705 2024-04-29 07:50:37.605872 cg-60.4.7/tests/fixtures/apps/balsamic/case/metrics_deliverables.yaml
+-rw-r--r--   0        0        0      692 2024-04-29 07:50:37.605872 cg-60.4.7/tests/fixtures/apps/crunchy/spring_metadata.json
+-rw-r--r--   0        0        0        0 2024-04-29 07:50:37.605872 cg-60.4.7/tests/fixtures/apps/demultiplexing/demultiplexed-runs/170517_ST-E00266_0210_BHJCFFALXX/ACC2655A1_S2_L002_R1_001.fastq.gz
+-rw-r--r--   0        0        0        0 2024-04-29 07:50:37.605872 cg-60.4.7/tests/fixtures/apps/demultiplexing/demultiplexed-runs/170517_ST-E00266_0210_BHJCFFALXX/ACC2655A1_S2_L002_R2_001.fastq.gz
+-rw-r--r--   0        0        0      412 2024-04-29 07:50:37.605872 cg-60.4.7/tests/fixtures/apps/demultiplexing/demultiplexed-runs/170517_ST-E00266_0210_BHJCFFALXX/Reports/Adapter_Metrics.csv
+-rw-r--r--   0        0        0      484 2024-04-29 07:50:37.605872 cg-60.4.7/tests/fixtures/apps/demultiplexing/demultiplexed-runs/170517_ST-E00266_0210_BHJCFFALXX/Reports/Demultiplex_Stats.csv
+-rw-r--r--   0        0        0      658 2024-04-29 07:50:37.605872 cg-60.4.7/tests/fixtures/apps/demultiplexing/demultiplexed-runs/170517_ST-E00266_0210_BHJCFFALXX/Reports/Quality_Metrics.csv
+-rw-r--r--   0        0        0        0 2024-04-29 07:50:37.605872 cg-60.4.7/tests/fixtures/apps/demultiplexing/demultiplexed-runs/170517_ST-E00266_0210_BHJCFFALXX/SVE2648A1_S1_L001_R1_001.fastq.gz
+-rw-r--r--   0        0        0        0 2024-04-29 07:50:37.605872 cg-60.4.7/tests/fixtures/apps/demultiplexing/demultiplexed-runs/170517_ST-E00266_0210_BHJCFFALXX/SVE2648A1_S1_L001_R2_001.fastq.gz
+-rw-r--r--   0        0        0        0 2024-04-29 07:50:37.605872 cg-60.4.7/tests/fixtures/apps/demultiplexing/demultiplexed-runs/170517_ST-E00266_0210_BHJCFFALXX/Undetermined_S0_L001_R1_001.fastq.gz
+-rw-r--r--   0        0        0        0 2024-04-29 07:50:37.605872 cg-60.4.7/tests/fixtures/apps/demultiplexing/demultiplexed-runs/170517_ST-E00266_0210_BHJCFFALXX/Undetermined_S0_L001_R2_001.fastq.gz
+-rw-r--r--   0        0        0        0 2024-04-29 07:50:37.605872 cg-60.4.7/tests/fixtures/apps/demultiplexing/demultiplexed-runs/170517_ST-E00266_0210_BHJCFFALXX/demuxcomplete.txt
+-rw-r--r--   0        0        0     1757 2024-04-29 07:50:37.605872 cg-60.4.7/tests/fixtures/apps/demultiplexing/demultiplexed-runs/201203_D00483_0200_AHVKJCDRXX/HVKJCDRXX_demultiplex.stderr
+-rw-r--r--   0        0        0        7 2024-04-29 07:50:37.605872 cg-60.4.7/tests/fixtures/apps/demultiplexing/demultiplexed-runs/201203_D00483_0200_AHVKJCDRXX/SampleSheet.csv
+-rw-r--r--   0        0        0        0 2024-04-29 07:50:37.605872 cg-60.4.7/tests/fixtures/apps/demultiplexing/demultiplexed-runs/201203_D00483_0200_AHVKJCDRXX/Unaligned/Project_150392/Sample_ACC7769A10/HN3FKDSXY_AL-P-00425491-N-03103120-KH20210330-PN20210331_S1_L001_R1_001.fastq.gz
+-rw-r--r--   0        0        0        0 2024-04-29 07:50:37.605872 cg-60.4.7/tests/fixtures/apps/demultiplexing/demultiplexed-runs/201203_D00483_0200_AHVKJCDRXX/Unaligned/Project_150392/Sample_ACC7769A10/HN3FKDSXY_AL-P-00425491-N-03103120-KH20210330-PN20210331_S1_L001_R2_001.fastq.gz
+-rw-r--r--   0        0        0     6034 2024-04-29 07:50:37.609872 cg-60.4.7/tests/fixtures/apps/demultiplexing/demultiplexed-runs/201203_D00483_0200_AHVKJCDRXX/Unaligned/Stats/ConversionStats.xml
+-rw-r--r--   0        0        0     1172 2024-04-29 07:50:37.609872 cg-60.4.7/tests/fixtures/apps/demultiplexing/demultiplexed-runs/201203_D00483_0200_AHVKJCDRXX/Unaligned/Stats/DemultiplexingStats.xml
+-rw-r--r--   0        0        0        7 2024-04-29 07:50:37.609872 cg-60.4.7/tests/fixtures/apps/demultiplexing/demultiplexed-runs/201203_D00483_0200_AHVKJCDRXX/fastq_1.fastq.gz
+-rw-r--r--   0        0        0        7 2024-04-29 07:50:37.609872 cg-60.4.7/tests/fixtures/apps/demultiplexing/demultiplexed-runs/201203_D00483_0200_AHVKJCDRXX/fastq_2.fastq.gz
+-rw-r--r--   0        0        0        0 2024-04-29 07:50:37.609872 cg-60.4.7/tests/fixtures/apps/demultiplexing/demultiplexed-runs/20231108_LH00188_0028_B22F52TLT3/BCLConvert/fastq/ACC13169A1_S1_L001_R1_001.fastq.gz
+-rw-r--r--   0        0        0        0 2024-04-29 07:50:37.609872 cg-60.4.7/tests/fixtures/apps/demultiplexing/demultiplexed-runs/20231108_LH00188_0028_B22F52TLT3/BCLConvert/fastq/ACC13169A1_S1_L001_R2_001.fastq.gz
+-rw-r--r--   0        0        0        0 2024-04-29 07:50:37.609872 cg-60.4.7/tests/fixtures/apps/demultiplexing/demultiplexed-runs/20231108_LH00188_0028_B22F52TLT3/BCLConvert/fastq/ACC13170A6_S2_L002_R1_001.fastq.gz
+-rw-r--r--   0        0        0        0 2024-04-29 07:50:37.609872 cg-60.4.7/tests/fixtures/apps/demultiplexing/demultiplexed-runs/20231108_LH00188_0028_B22F52TLT3/BCLConvert/fastq/ACC13170A6_S2_L002_R2_001.fastq.gz
+-rw-r--r--   0        0        0        0 2024-04-29 07:50:37.609872 cg-60.4.7/tests/fixtures/apps/demultiplexing/demultiplexed-runs/20231108_LH00188_0028_B22F52TLT3/BCLConvert/fastq/Undetermined_S0_L001_R1_001.fastq.gz
+-rw-r--r--   0        0        0        0 2024-04-29 07:50:37.609872 cg-60.4.7/tests/fixtures/apps/demultiplexing/demultiplexed-runs/20231108_LH00188_0028_B22F52TLT3/BCLConvert/fastq/Undetermined_S0_L001_R2_001.fastq.gz
+-rw-r--r--   0        0        0      288 2024-04-29 07:50:37.609872 cg-60.4.7/tests/fixtures/apps/demultiplexing/demultiplexed-runs/20231108_LH00188_0028_B22F52TLT3/Reports/Adapter_Metrics.csv
+-rw-r--r--   0        0        0      361 2024-04-29 07:50:37.609872 cg-60.4.7/tests/fixtures/apps/demultiplexing/demultiplexed-runs/20231108_LH00188_0028_B22F52TLT3/Reports/Demultiplex_Stats.csv
+-rw-r--r--   0        0        0      414 2024-04-29 07:50:37.609872 cg-60.4.7/tests/fixtures/apps/demultiplexing/demultiplexed-runs/20231108_LH00188_0028_B22F52TLT3/Reports/Quality_Metrics.csv
+-rw-r--r--   0        0        0        0 2024-04-29 07:50:37.609872 cg-60.4.7/tests/fixtures/apps/demultiplexing/demultiplexed-runs/20231108_LH00188_0028_B22F52TLT3/demuxcomplete.txt
+-rw-r--r--   0        0        0      315 2024-04-29 07:50:37.609872 cg-60.4.7/tests/fixtures/apps/demultiplexing/demultiplexed-runs/211101_A00187_0615_AHLG5GDRZZ/Unaligned/Reports/Adapter_Metrics.csv
+-rw-r--r--   0        0        0      434 2024-04-29 07:50:37.609872 cg-60.4.7/tests/fixtures/apps/demultiplexing/demultiplexed-runs/211101_A00187_0615_AHLG5GDRZZ/Unaligned/Reports/Quality_Metrics.csv
+-rw-r--r--   0        0        0     8624 2024-04-29 07:50:37.609872 cg-60.4.7/tests/fixtures/apps/demultiplexing/demultiplexed-runs/211101_A00187_0615_AHLG5GDRZZ/Unaligned/Reports/RunInfo.xml
+-rw-r--r--   0        0        0        0 2024-04-29 07:50:37.609872 cg-60.4.7/tests/fixtures/apps/demultiplexing/demultiplexed-runs/230912_A00187_1009_AHK33MDRX3/ACC12642A4_S2_L002_R1_001.fastq.gz
+-rw-r--r--   0        0        0        0 2024-04-29 07:50:37.609872 cg-60.4.7/tests/fixtures/apps/demultiplexing/demultiplexed-runs/230912_A00187_1009_AHK33MDRX3/ACC12642A4_S2_L002_R2_001.fastq.gz
+-rw-r--r--   0        0        0        0 2024-04-29 07:50:37.609872 cg-60.4.7/tests/fixtures/apps/demultiplexing/demultiplexed-runs/230912_A00187_1009_AHK33MDRX3/ACC12642A7_S1_L001_R1_001.fastq.gz
+-rw-r--r--   0        0        0        0 2024-04-29 07:50:37.609872 cg-60.4.7/tests/fixtures/apps/demultiplexing/demultiplexed-runs/230912_A00187_1009_AHK33MDRX3/ACC12642A7_S1_L001_R2_001.fastq.gz
+-rw-r--r--   0        0        0      303 2024-04-29 07:50:37.609872 cg-60.4.7/tests/fixtures/apps/demultiplexing/demultiplexed-runs/230912_A00187_1009_AHK33MDRX3/Reports/Adapter_Metrics.csv
+-rw-r--r--   0        0        0      364 2024-04-29 07:50:37.609872 cg-60.4.7/tests/fixtures/apps/demultiplexing/demultiplexed-runs/230912_A00187_1009_AHK33MDRX3/Reports/Demultiplex_Stats.csv
+-rw-r--r--   0        0        0      427 2024-04-29 07:50:37.609872 cg-60.4.7/tests/fixtures/apps/demultiplexing/demultiplexed-runs/230912_A00187_1009_AHK33MDRX3/Reports/Quality_Metrics.csv
+-rw-r--r--   0        0        0        0 2024-04-29 07:50:37.609872 cg-60.4.7/tests/fixtures/apps/demultiplexing/demultiplexed-runs/230912_A00187_1009_AHK33MDRX3/Undetermined_S0_L001_R1_001.fastq.gz
+-rw-r--r--   0        0        0        0 2024-04-29 07:50:37.609872 cg-60.4.7/tests/fixtures/apps/demultiplexing/demultiplexed-runs/230912_A00187_1009_AHK33MDRX3/Undetermined_S0_L001_R2_001.fastq.gz
+-rw-r--r--   0        0        0        0 2024-04-29 07:50:37.609872 cg-60.4.7/tests/fixtures/apps/demultiplexing/demultiplexed-runs/230912_A00187_1009_AHK33MDRX3/demuxcomplete.txt
+-rw-r--r--   0        0        0        0 2024-04-29 07:50:37.605872 cg-60.4.7/tests/fixtures/apps/demultiplexing/demultiplexed-runs-unfinished/201203_D00483_0200_AHVKJCDRXX/Unaligned/150392/ACC7769A10/AL-P-00425491-N-03103120-KH20210330-PN20210331_S1_L001_R1_001.fastq.gz
+-rw-r--r--   0        0        0        0 2024-04-29 07:50:37.605872 cg-60.4.7/tests/fixtures/apps/demultiplexing/demultiplexed-runs-unfinished/201203_D00483_0200_AHVKJCDRXX/Unaligned/150392/ACC7769A10/AL-P-00425491-N-03103120-KH20210330-PN20210331_S1_L001_R2_001.fastq.gz
+-rw-r--r--   0        0        0     4439 2024-04-29 07:50:37.605872 cg-60.4.7/tests/fixtures/apps/demultiplexing/demultiplexed-runs-unfinished/201203_D00483_0200_AHVKJCDRXX/Unaligned/Stats/ConversionStats.xml
+-rw-r--r--   0        0        0     1172 2024-04-29 07:50:37.605872 cg-60.4.7/tests/fixtures/apps/demultiplexing/demultiplexed-runs-unfinished/201203_D00483_0200_AHVKJCDRXX/Unaligned/Stats/DemultiplexingStats.xml
+-rw-r--r--   0        0        0        0 2024-04-29 07:50:37.605872 cg-60.4.7/tests/fixtures/apps/demultiplexing/demultiplexed-runs-unfinished/201203_D00483_0200_AHVKJCDRXX/Unaligned/Undetermined_S0_L001_R1_001.fastq.gz
+-rw-r--r--   0        0        0        0 2024-04-29 07:50:37.605872 cg-60.4.7/tests/fixtures/apps/demultiplexing/demultiplexed-runs-unfinished/201203_D00483_0200_AHVKJCDRXX/Unaligned/Undetermined_S0_L001_R2_001.fastq.gz
+-rw-r--r--   0        0        0        0 2024-04-29 07:50:37.605872 cg-60.4.7/tests/fixtures/apps/demultiplexing/demultiplexed-runs-unfinished/201203_D00483_0200_AHVKJCDRXX/Unaligned/Undetermined_S0_L002_R1_001.fastq.gz
+-rw-r--r--   0        0        0        0 2024-04-29 07:50:37.605872 cg-60.4.7/tests/fixtures/apps/demultiplexing/demultiplexed-runs-unfinished/201203_D00483_0200_AHVKJCDRXX/Unaligned/Undetermined_S0_L002_R2_001.fastq.gz
+-rw-r--r--   0        0        0     5127 2024-04-29 07:50:37.605872 cg-60.4.7/tests/fixtures/apps/demultiplexing/demultiplexed-runs-unfinished/230912_A00187_1009_AHK33MDRX3/SampleSheet.csv
+-rw-r--r--   0        0        0       43 2024-04-29 07:50:37.609872 cg-60.4.7/tests/fixtures/apps/demultiplexing/fastq/dummy_run_R1_001.fastq.gz
+-rw-r--r--   0        0        0       67 2024-04-29 07:50:37.609872 cg-60.4.7/tests/fixtures/apps/demultiplexing/fastq/dummy_run_R1_001.fastq.gz.md5
+-rw-r--r--   0        0        0   338370 2024-04-29 07:50:37.609872 cg-60.4.7/tests/fixtures/apps/demultiplexing/fastq/fastq_run_R1_001.fastq.gz
+-rw-r--r--   0        0        0       67 2024-04-29 07:50:37.609872 cg-60.4.7/tests/fixtures/apps/demultiplexing/fastq/fastq_run_R1_001.fastq.gz.md5
+-rw-r--r--   0        0        0   338349 2024-04-29 07:50:37.609872 cg-60.4.7/tests/fixtures/apps/demultiplexing/fastq/fastq_run_R2_001.fastq.gz
+-rw-r--r--   0        0        0        0 2024-04-29 07:50:37.613872 cg-60.4.7/tests/fixtures/apps/demultiplexing/flow_cells/170517_ST-E00266_0210_BHJCFFALXX/CopyComplete.txt
+-rw-r--r--   0        0        0     2126 2024-04-29 07:50:37.613872 cg-60.4.7/tests/fixtures/apps/demultiplexing/flow_cells/170517_ST-E00266_0210_BHJCFFALXX/HJCFFALXX_bcl2fastq_raw.json
+-rw-r--r--   0        0        0     1827 2024-04-29 07:50:37.613872 cg-60.4.7/tests/fixtures/apps/demultiplexing/flow_cells/170517_ST-E00266_0210_BHJCFFALXX/HJCFFALXX_bcl_convert_raw.json
+-rw-r--r--   0        0        0       78 2024-04-29 07:50:37.613872 cg-60.4.7/tests/fixtures/apps/demultiplexing/flow_cells/170517_ST-E00266_0210_BHJCFFALXX/README.txt
+-rw-r--r--   0        0        0        0 2024-04-29 07:50:37.613872 cg-60.4.7/tests/fixtures/apps/demultiplexing/flow_cells/170517_ST-E00266_0210_BHJCFFALXX/RTAComplete.txt
+-rw-r--r--   0        0        0     6895 2024-04-29 07:50:37.613872 cg-60.4.7/tests/fixtures/apps/demultiplexing/flow_cells/170517_ST-E00266_0210_BHJCFFALXX/RTAConfiguration.xml
+-rw-r--r--   0        0        0       37 2024-04-29 07:50:37.613872 cg-60.4.7/tests/fixtures/apps/demultiplexing/flow_cells/170517_ST-E00266_0210_BHJCFFALXX/RTARead1Complete.txt
+-rw-r--r--   0        0        0       36 2024-04-29 07:50:37.613872 cg-60.4.7/tests/fixtures/apps/demultiplexing/flow_cells/170517_ST-E00266_0210_BHJCFFALXX/RTARead2Complete.txt
+-rw-r--r--   0        0        0       36 2024-04-29 07:50:37.613872 cg-60.4.7/tests/fixtures/apps/demultiplexing/flow_cells/170517_ST-E00266_0210_BHJCFFALXX/RTARead3Complete.txt
+-rw-r--r--   0        0        0    24755 2024-04-29 07:50:37.613872 cg-60.4.7/tests/fixtures/apps/demultiplexing/flow_cells/170517_ST-E00266_0210_BHJCFFALXX/RunInfo.xml
+-rw-r--r--   0        0        0      692 2024-04-29 07:50:37.613872 cg-60.4.7/tests/fixtures/apps/demultiplexing/flow_cells/170517_ST-E00266_0210_BHJCFFALXX/SampleSheet.csv
+-rw-r--r--   0        0        0      724 2024-04-29 07:50:37.613872 cg-60.4.7/tests/fixtures/apps/demultiplexing/flow_cells/170517_ST-E00266_0210_BHJCFFALXX/SampleSheet_bcl2fastq.csv
+-rw-r--r--   0        0        0       61 2024-04-29 07:50:37.613872 cg-60.4.7/tests/fixtures/apps/demultiplexing/flow_cells/170517_ST-E00266_0210_BHJCFFALXX/SequencingComplete.txt
+-rw-r--r--   0        0        0     5775 2024-04-29 07:50:37.613872 cg-60.4.7/tests/fixtures/apps/demultiplexing/flow_cells/170517_ST-E00266_0210_BHJCFFALXX/runParameters.xml
+-rw-r--r--   0        0        0        0 2024-04-29 07:50:37.613872 cg-60.4.7/tests/fixtures/apps/demultiplexing/flow_cells/180508_ST-E00269_0269_AHL32LCCXY/CopyComplete.txt
+-rw-r--r--   0        0        0     2282 2024-04-29 07:50:37.613872 cg-60.4.7/tests/fixtures/apps/demultiplexing/flow_cells/180508_ST-E00269_0269_AHL32LCCXY/HL32LCCXY_bcl2fastq_raw.json
+-rw-r--r--   0        0        0     1632 2024-04-29 07:50:37.613872 cg-60.4.7/tests/fixtures/apps/demultiplexing/flow_cells/180508_ST-E00269_0269_AHL32LCCXY/HL32LCCXY_bcl_convert_raw.json
+-rw-r--r--   0        0        0       76 2024-04-29 07:50:37.613872 cg-60.4.7/tests/fixtures/apps/demultiplexing/flow_cells/180508_ST-E00269_0269_AHL32LCCXY/README.txt
+-rw-r--r--   0        0        0        0 2024-04-29 07:50:37.613872 cg-60.4.7/tests/fixtures/apps/demultiplexing/flow_cells/180508_ST-E00269_0269_AHL32LCCXY/RTAComplete.txt
+-rw-r--r--   0        0        0     6912 2024-04-29 07:50:37.613872 cg-60.4.7/tests/fixtures/apps/demultiplexing/flow_cells/180508_ST-E00269_0269_AHL32LCCXY/RTAConfiguration.xml
+-rw-r--r--   0        0        0       36 2024-04-29 07:50:37.613872 cg-60.4.7/tests/fixtures/apps/demultiplexing/flow_cells/180508_ST-E00269_0269_AHL32LCCXY/RTARead1Complete.txt
+-rw-r--r--   0        0        0       36 2024-04-29 07:50:37.613872 cg-60.4.7/tests/fixtures/apps/demultiplexing/flow_cells/180508_ST-E00269_0269_AHL32LCCXY/RTARead2Complete.txt
+-rw-r--r--   0        0        0       36 2024-04-29 07:50:37.613872 cg-60.4.7/tests/fixtures/apps/demultiplexing/flow_cells/180508_ST-E00269_0269_AHL32LCCXY/RTARead3Complete.txt
+-rw-r--r--   0        0        0       36 2024-04-29 07:50:37.613872 cg-60.4.7/tests/fixtures/apps/demultiplexing/flow_cells/180508_ST-E00269_0269_AHL32LCCXY/RTARead4Complete.txt
+-rw-r--r--   0        0        0    24814 2024-04-29 07:50:37.613872 cg-60.4.7/tests/fixtures/apps/demultiplexing/flow_cells/180508_ST-E00269_0269_AHL32LCCXY/RunInfo.xml
+-rw-r--r--   0        0        0      814 2024-04-29 07:50:37.613872 cg-60.4.7/tests/fixtures/apps/demultiplexing/flow_cells/180508_ST-E00269_0269_AHL32LCCXY/SampleSheet.csv
+-rw-r--r--   0        0        0      660 2024-04-29 07:50:37.613872 cg-60.4.7/tests/fixtures/apps/demultiplexing/flow_cells/180508_ST-E00269_0269_AHL32LCCXY/SampleSheet_bcl2fastq.csv
+-rw-r--r--   0        0        0       61 2024-04-29 07:50:37.613872 cg-60.4.7/tests/fixtures/apps/demultiplexing/flow_cells/180508_ST-E00269_0269_AHL32LCCXY/SequencingComplete.txt
+-rw-r--r--   0        0        0     5853 2024-04-29 07:50:37.613872 cg-60.4.7/tests/fixtures/apps/demultiplexing/flow_cells/180508_ST-E00269_0269_AHL32LCCXY/runParameters.xml
+-rw-r--r--   0        0        0        0 2024-04-29 07:50:37.613872 cg-60.4.7/tests/fixtures/apps/demultiplexing/flow_cells/180509_D00450_0598_BHGYFNBCX2/CopyComplete.txt
+-rw-r--r--   0        0        0    21848 2024-04-29 07:50:37.613872 cg-60.4.7/tests/fixtures/apps/demultiplexing/flow_cells/180509_D00450_0598_BHGYFNBCX2/HGYFNBCX2_bcl2fastq_raw.json
+-rw-r--r--   0        0        0    15512 2024-04-29 07:50:37.613872 cg-60.4.7/tests/fixtures/apps/demultiplexing/flow_cells/180509_D00450_0598_BHGYFNBCX2/HGYFNBCX2_bcl_convert_raw.json
+-rw-r--r--   0        0        0       79 2024-04-29 07:50:37.613872 cg-60.4.7/tests/fixtures/apps/demultiplexing/flow_cells/180509_D00450_0598_BHGYFNBCX2/README.txt
+-rw-r--r--   0        0        0        0 2024-04-29 07:50:37.613872 cg-60.4.7/tests/fixtures/apps/demultiplexing/flow_cells/180509_D00450_0598_BHGYFNBCX2/RTAComplete.txt
+-rw-r--r--   0        0        0      756 2024-04-29 07:50:37.613872 cg-60.4.7/tests/fixtures/apps/demultiplexing/flow_cells/180509_D00450_0598_BHGYFNBCX2/RunInfo.xml
+-rw-r--r--   0        0        0     4118 2024-04-29 07:50:37.613872 cg-60.4.7/tests/fixtures/apps/demultiplexing/flow_cells/180509_D00450_0598_BHGYFNBCX2/SampleSheet.csv
+-rw-r--r--   0        0        0     1408 2024-04-29 07:50:37.613872 cg-60.4.7/tests/fixtures/apps/demultiplexing/flow_cells/180509_D00450_0598_BHGYFNBCX2/SampleSheet_bcl2fastq.csv
+-rw-r--r--   0        0        0     5326 2024-04-29 07:50:37.613872 cg-60.4.7/tests/fixtures/apps/demultiplexing/flow_cells/180509_D00450_0598_BHGYFNBCX2/runParameters.xml
+-rw-r--r--   0        0        0        0 2024-04-29 07:50:37.613872 cg-60.4.7/tests/fixtures/apps/demultiplexing/flow_cells/181005_D00410_0735_BHM2LNBCX2/CopyComplete.txt
+-rw-r--r--   0        0        0    15041 2024-04-29 07:50:37.613872 cg-60.4.7/tests/fixtures/apps/demultiplexing/flow_cells/181005_D00410_0735_BHM2LNBCX2/HM2LNBCX2_bcl2fastq_raw.json
+-rw-r--r--   0        0        0    10649 2024-04-29 07:50:37.613872 cg-60.4.7/tests/fixtures/apps/demultiplexing/flow_cells/181005_D00410_0735_BHM2LNBCX2/HM2LNBCX2_bcl_convert_raw.json
+-rw-r--r--   0        0        0       81 2024-04-29 07:50:37.613872 cg-60.4.7/tests/fixtures/apps/demultiplexing/flow_cells/181005_D00410_0735_BHM2LNBCX2/README.txt
+-rw-r--r--   0        0        0        0 2024-04-29 07:50:37.613872 cg-60.4.7/tests/fixtures/apps/demultiplexing/flow_cells/181005_D00410_0735_BHM2LNBCX2/RTAComplete.txt
+-rw-r--r--   0        0        0      755 2024-04-29 07:50:37.613872 cg-60.4.7/tests/fixtures/apps/demultiplexing/flow_cells/181005_D00410_0735_BHM2LNBCX2/RunInfo.xml
+-rw-r--r--   0        0        0     2878 2024-04-29 07:50:37.613872 cg-60.4.7/tests/fixtures/apps/demultiplexing/flow_cells/181005_D00410_0735_BHM2LNBCX2/SampleSheet.csv
+-rw-r--r--   0        0        0      928 2024-04-29 07:50:37.613872 cg-60.4.7/tests/fixtures/apps/demultiplexing/flow_cells/181005_D00410_0735_BHM2LNBCX2/SampleSheet_bcl2fastq.csv
+-rw-r--r--   0        0        0     5359 2024-04-29 07:50:37.613872 cg-60.4.7/tests/fixtures/apps/demultiplexing/flow_cells/181005_D00410_0735_BHM2LNBCX2/runParameters.xml
+-rw-r--r--   0        0        0        0 2024-04-29 07:50:37.613872 cg-60.4.7/tests/fixtures/apps/demultiplexing/flow_cells/190927_A00689_0069_BHLYWYDSXX/CopyComplete.txt
+-rw-r--r--   0        0        0    27887 2024-04-29 07:50:37.613872 cg-60.4.7/tests/fixtures/apps/demultiplexing/flow_cells/190927_A00689_0069_BHLYWYDSXX/CorrectSampleSheet.csv
+-rw-r--r--   0        0        0   141870 2024-04-29 07:50:37.613872 cg-60.4.7/tests/fixtures/apps/demultiplexing/flow_cells/190927_A00689_0069_BHLYWYDSXX/HLYWYDSXX_bcl2fastq_raw.json
+-rwxr-xr-x   0        0        0   122682 2024-04-29 07:50:37.617872 cg-60.4.7/tests/fixtures/apps/demultiplexing/flow_cells/190927_A00689_0069_BHLYWYDSXX/HLYWYDSXX_bcl_convert_raw.json
+-rw-r--r--   0        0        0      243 2024-04-29 07:50:37.617872 cg-60.4.7/tests/fixtures/apps/demultiplexing/flow_cells/190927_A00689_0069_BHLYWYDSXX/README.txt
+-rw-r--r--   0        0        0    28230 2024-04-29 07:50:37.617872 cg-60.4.7/tests/fixtures/apps/demultiplexing/flow_cells/190927_A00689_0069_BHLYWYDSXX/RTA3.cfg
+-rw-r--r--   0        0        0        0 2024-04-29 07:50:37.617872 cg-60.4.7/tests/fixtures/apps/demultiplexing/flow_cells/190927_A00689_0069_BHLYWYDSXX/RTAComplete.txt
+-rw-r--r--   0        0        0    94426 2024-04-29 07:50:37.617872 cg-60.4.7/tests/fixtures/apps/demultiplexing/flow_cells/190927_A00689_0069_BHLYWYDSXX/RunInfo.xml
+-rw-r--r--   0        0        0     5819 2024-04-29 07:50:37.617872 cg-60.4.7/tests/fixtures/apps/demultiplexing/flow_cells/190927_A00689_0069_BHLYWYDSXX/RunParameters.xml
+-rw-r--r--   0        0        0        0 2024-04-29 07:50:37.617872 cg-60.4.7/tests/fixtures/apps/demultiplexing/flow_cells/190927_A00689_0069_BHLYWYDSXX/SequenceComplete.txt
+-rw-r--r--   0        0        0     1757 2024-04-29 07:50:37.617872 cg-60.4.7/tests/fixtures/apps/demultiplexing/flow_cells/201203_D00483_0200_AHVKJCDRXX/HVKJCDRXX_demultiplex.stderr
+-rw-r--r--   0        0        0     1757 2024-04-29 07:50:37.617872 cg-60.4.7/tests/fixtures/apps/demultiplexing/flow_cells/201203_D00483_0200_AHVKJCDRXX/HVKJCDRXX_demultiplex.stdout
+-rw-r--r--   0        0        0    47522 2024-04-29 07:50:37.617872 cg-60.4.7/tests/fixtures/apps/demultiplexing/flow_cells/201203_D00483_0200_AHVKJCDRXX/HVKJCDRXX_raw.json
+-rw-r--r--   0        0        0       12 2024-04-29 07:50:37.617872 cg-60.4.7/tests/fixtures/apps/demultiplexing/flow_cells/201203_D00483_0200_AHVKJCDRXX/README.txt
+-rw-r--r--   0        0        0        0 2024-04-29 07:50:37.617872 cg-60.4.7/tests/fixtures/apps/demultiplexing/flow_cells/201203_D00483_0200_AHVKJCDRXX/RTAComplete.txt
+-rw-r--r--   0        0        0     6666 2024-04-29 07:50:37.617872 cg-60.4.7/tests/fixtures/apps/demultiplexing/flow_cells/201203_D00483_0200_AHVKJCDRXX/RunParameters.xml
+-rw-r--r--   0        0        0      254 2024-04-29 07:50:37.617872 cg-60.4.7/tests/fixtures/apps/demultiplexing/flow_cells/201203_D00483_0200_AHVKJCDRXX/SampleSheet.csv
+-rw-r--r--   0        0        0        0 2024-04-29 07:50:37.617872 cg-60.4.7/tests/fixtures/apps/demultiplexing/flow_cells/201203_D00483_0200_AHVKJCDRXX/copycomplete.txt
+-rw-r--r--   0        0        0        0 2024-04-29 07:50:37.617872 cg-60.4.7/tests/fixtures/apps/demultiplexing/flow_cells/201203_D00483_0200_AHVKJCDRXX/delivery.txt
+-rw-r--r--   0        0        0        0 2024-04-29 07:50:37.617872 cg-60.4.7/tests/fixtures/apps/demultiplexing/flow_cells/201203_D00483_0200_AHVKJCDRXX/demuxstarted.txt
+-rwxr-xr-x   0        0        0    47434 2024-04-29 07:50:37.617872 cg-60.4.7/tests/fixtures/apps/demultiplexing/flow_cells/20231108_LH00188_0028_B22F52TLT3/22F52TLT3_raw.json
+-rw-r--r--   0        0        0        0 2024-04-29 07:50:37.617872 cg-60.4.7/tests/fixtures/apps/demultiplexing/flow_cells/20231108_LH00188_0028_B22F52TLT3/CopyComplete.txt
+-rw-r--r--   0        0        0    10950 2024-04-29 07:50:37.617872 cg-60.4.7/tests/fixtures/apps/demultiplexing/flow_cells/20231108_LH00188_0028_B22F52TLT3/CorrectSampleSheet.csv
+-rw-r--r--   0        0        0      225 2024-04-29 07:50:37.617872 cg-60.4.7/tests/fixtures/apps/demultiplexing/flow_cells/20231108_LH00188_0028_B22F52TLT3/Manifest.tsv
+-rw-r--r--   0        0        0       55 2024-04-29 07:50:37.617872 cg-60.4.7/tests/fixtures/apps/demultiplexing/flow_cells/20231108_LH00188_0028_B22F52TLT3/README.txt
+-rwxr-xr-x   0        0        0     2493 2024-04-29 07:50:37.617872 cg-60.4.7/tests/fixtures/apps/demultiplexing/flow_cells/20231108_LH00188_0028_B22F52TLT3/RTA.cfg
+-rwxr-xr-x   0        0        0        1 2024-04-29 07:50:37.617872 cg-60.4.7/tests/fixtures/apps/demultiplexing/flow_cells/20231108_LH00188_0028_B22F52TLT3/RTAComplete.txt
+-rwxr-xr-x   0        0        0        2 2024-04-29 07:50:37.617872 cg-60.4.7/tests/fixtures/apps/demultiplexing/flow_cells/20231108_LH00188_0028_B22F52TLT3/RTAExited.txt
+-rwxr-xr-x   0        0        0      730 2024-04-29 07:50:37.617872 cg-60.4.7/tests/fixtures/apps/demultiplexing/flow_cells/20231108_LH00188_0028_B22F52TLT3/RunCompletionStatus.xml
+-rwxr-xr-x   0        0        0    79277 2024-04-29 07:50:37.617872 cg-60.4.7/tests/fixtures/apps/demultiplexing/flow_cells/20231108_LH00188_0028_B22F52TLT3/RunInfo.xml
+-rwxr-xr-x   0        0        0     2694 2024-04-29 07:50:37.617872 cg-60.4.7/tests/fixtures/apps/demultiplexing/flow_cells/20231108_LH00188_0028_B22F52TLT3/RunParameters.xml
+-rw-r--r--   0        0        0    10950 2024-04-29 07:50:37.617872 cg-60.4.7/tests/fixtures/apps/demultiplexing/flow_cells/20231108_LH00188_0028_B22F52TLT3/SampleSheet.csv
+-rw-r--r--   0        0        0        0 2024-04-29 07:50:37.617872 cg-60.4.7/tests/fixtures/apps/demultiplexing/flow_cells/211101_A00187_0615_AHLG5GDRZZ/CopyComplete.txt
+-rw-r--r--   0        0        0      509 2024-04-29 07:50:37.617872 cg-60.4.7/tests/fixtures/apps/demultiplexing/flow_cells/211101_A00187_0615_AHLG5GDRZZ/HLG5GDRZZ_demultiplex.stderr
+-rw-r--r--   0        0        0     2229 2024-04-29 07:50:37.617872 cg-60.4.7/tests/fixtures/apps/demultiplexing/flow_cells/211101_A00187_0615_AHLG5GDRZZ/HLG5GDRZZ_demultiplex.stdout
+-rw-r--r--   0        0        0        0 2024-04-29 07:50:37.617872 cg-60.4.7/tests/fixtures/apps/demultiplexing/flow_cells/211101_A00187_0615_AHLG5GDRZZ/RTAComplete.txt
+-rw-r--r--   0        0        0     6665 2024-04-29 07:50:37.617872 cg-60.4.7/tests/fixtures/apps/demultiplexing/flow_cells/211101_A00187_0615_AHLG5GDRZZ/RunParameters.xml
+-rw-r--r--   0        0        0      619 2024-04-29 07:50:37.617872 cg-60.4.7/tests/fixtures/apps/demultiplexing/flow_cells/211101_A00187_0615_AHLG5GDRZZ/SampleSheet.csv
+-rw-r--r--   0        0        0        0 2024-04-29 07:50:37.617872 cg-60.4.7/tests/fixtures/apps/demultiplexing/flow_cells/230912_A00187_1009_AHK33MDRX3/CopyComplete.txt
+-rw-r--r--   0        0        0     4941 2024-04-29 07:50:37.617872 cg-60.4.7/tests/fixtures/apps/demultiplexing/flow_cells/230912_A00187_1009_AHK33MDRX3/CorrectSampleSheet.csv
+-rwxr-xr-x   0        0        0    20050 2024-04-29 07:50:37.617872 cg-60.4.7/tests/fixtures/apps/demultiplexing/flow_cells/230912_A00187_1009_AHK33MDRX3/HK33MDRX3_bcl_convert_raw.json
+-rw-r--r--   0        0        0        0 2024-04-29 07:50:37.617872 cg-60.4.7/tests/fixtures/apps/demultiplexing/flow_cells/230912_A00187_1009_AHK33MDRX3/HK33MDRX3_demultiplex.stderr
+-rw-r--r--   0        0        0        0 2024-04-29 07:50:37.617872 cg-60.4.7/tests/fixtures/apps/demultiplexing/flow_cells/230912_A00187_1009_AHK33MDRX3/HK33MDRX3_demultiplex.stdout
+-rw-r--r--   0        0        0      244 2024-04-29 07:50:37.617872 cg-60.4.7/tests/fixtures/apps/demultiplexing/flow_cells/230912_A00187_1009_AHK33MDRX3/README.txt
+-rw-r--r--   0        0        0     6391 2024-04-29 07:50:37.617872 cg-60.4.7/tests/fixtures/apps/demultiplexing/flow_cells/230912_A00187_1009_AHK33MDRX3/RTA3.cfg
+-rw-r--r--   0        0        0        0 2024-04-29 07:50:37.617872 cg-60.4.7/tests/fixtures/apps/demultiplexing/flow_cells/230912_A00187_1009_AHK33MDRX3/RTAComplete.txt
+-rw-r--r--   0        0        0    16428 2024-04-29 07:50:37.617872 cg-60.4.7/tests/fixtures/apps/demultiplexing/flow_cells/230912_A00187_1009_AHK33MDRX3/RunInfo.xml
+-rw-r--r--   0        0        0     6728 2024-04-29 07:50:37.617872 cg-60.4.7/tests/fixtures/apps/demultiplexing/flow_cells/230912_A00187_1009_AHK33MDRX3/RunParameters.xml
+-rw-r--r--   0        0        0     5127 2024-04-29 07:50:37.617872 cg-60.4.7/tests/fixtures/apps/demultiplexing/flow_cells/230912_A00187_1009_AHK33MDRX3/SampleSheet.csv
+-rw-r--r--   0        0        0        0 2024-04-29 07:50:37.617872 cg-60.4.7/tests/fixtures/apps/demultiplexing/flow_cells/230912_A00187_1009_AHK33MDRX3/SequenceComplete.txt
+-rw-r--r--   0        0        0        0 2024-04-29 07:50:37.617872 cg-60.4.7/tests/fixtures/apps/demultiplexing/flow_cells/230912_A00187_1009_AHK33MDRX3/demuxstarted.txt
+-rw-r--r--   0        0        0      133 2024-04-29 07:50:37.617872 cg-60.4.7/tests/fixtures/apps/demultiplexing/flow_cells_broken/170517_ST-E00266_0210_BHJCFFALXX/README.txt
+-rw-r--r--   0        0        0      724 2024-04-29 07:50:37.617872 cg-60.4.7/tests/fixtures/apps/demultiplexing/flow_cells_broken/170517_ST-E00266_0210_BHJCFFALXX/SampleSheet.csv
+-rw-r--r--   0        0        0     5775 2024-04-29 07:50:37.617872 cg-60.4.7/tests/fixtures/apps/demultiplexing/flow_cells_broken/170517_ST-E00266_0210_BHJCFFALXX/runParameters.xml
+-rw-r--r--   0        0        0      124 2024-04-29 07:50:37.617872 cg-60.4.7/tests/fixtures/apps/demultiplexing/flow_cells_broken/180509_D00450_0598_BHGYFNBCX2/README.txt
+-rw-r--r--   0        0        0      310 2024-04-29 07:50:37.617872 cg-60.4.7/tests/fixtures/apps/demultiplexing/flow_cells_broken/190927_A00689_0069_BHLYWYDSXX/README.txt
+-rw-r--r--   0        0        0     5819 2024-04-29 07:50:37.617872 cg-60.4.7/tests/fixtures/apps/demultiplexing/flow_cells_broken/190927_A00689_0069_BHLYWYDSXX/RunParameters.xml
+-rw-r--r--   0        0        0      122 2024-04-29 07:50:37.617872 cg-60.4.7/tests/fixtures/apps/demultiplexing/flow_cells_broken/20231108_LH00188_0028_B22F52TLT3/README.txt
+-rwxr-xr-x   0        0        0     2694 2024-04-29 07:50:37.617872 cg-60.4.7/tests/fixtures/apps/demultiplexing/flow_cells_broken/20231108_LH00188_0028_B22F52TLT3/RunParameters.xml
+-rw-r--r--   0        0        0      311 2024-04-29 07:50:37.617872 cg-60.4.7/tests/fixtures/apps/demultiplexing/flow_cells_broken/230912_A00187_1009_AHK33MDRX3/README.txt
+-rw-r--r--   0        0        0     6728 2024-04-29 07:50:37.617872 cg-60.4.7/tests/fixtures/apps/demultiplexing/flow_cells_broken/230912_A00187_1009_AHK33MDRX3/RunParameters.xml
+-rw-r--r--   0        0        0        0 2024-04-29 07:50:37.617872 cg-60.4.7/tests/fixtures/apps/demultiplexing/flow_cells_demux_all/211101_A00187_0615_AHLG5GDRXY/CopyComplete.txt
+-rw-r--r--   0        0        0      509 2024-04-29 07:50:37.617872 cg-60.4.7/tests/fixtures/apps/demultiplexing/flow_cells_demux_all/211101_A00187_0615_AHLG5GDRXY/HLG5GDRXY_demultiplex.stderr
+-rw-r--r--   0        0        0     2229 2024-04-29 07:50:37.617872 cg-60.4.7/tests/fixtures/apps/demultiplexing/flow_cells_demux_all/211101_A00187_0615_AHLG5GDRXY/HLG5GDRXY_demultiplex.stdout
+-rw-r--r--   0        0        0        0 2024-04-29 07:50:37.617872 cg-60.4.7/tests/fixtures/apps/demultiplexing/flow_cells_demux_all/211101_A00187_0615_AHLG5GDRXY/RTAComplete.txt
+-rw-r--r--   0        0        0     6665 2024-04-29 07:50:37.617872 cg-60.4.7/tests/fixtures/apps/demultiplexing/flow_cells_demux_all/211101_A00187_0615_AHLG5GDRXY/RunParameters.xml
+-rw-r--r--   0        0        0      399 2024-04-29 07:50:37.617872 cg-60.4.7/tests/fixtures/apps/demultiplexing/flow_cells_demux_all/211101_A00187_0615_AHLG5GDRXY/SampleSheet.csv
+-rw-r--r--   0        0        0        0 2024-04-29 07:50:37.617872 cg-60.4.7/tests/fixtures/apps/demultiplexing/flow_cells_demux_all/211101_A00187_0615_AHLG5GDRZZ/CopyComplete.txt
+-rw-r--r--   0        0        0      509 2024-04-29 07:50:37.617872 cg-60.4.7/tests/fixtures/apps/demultiplexing/flow_cells_demux_all/211101_A00187_0615_AHLG5GDRZZ/HLG5GDRZZ_demultiplex.stderr
+-rw-r--r--   0        0        0     2229 2024-04-29 07:50:37.617872 cg-60.4.7/tests/fixtures/apps/demultiplexing/flow_cells_demux_all/211101_A00187_0615_AHLG5GDRZZ/HLG5GDRZZ_demultiplex.stdout
+-rw-r--r--   0        0        0        0 2024-04-29 07:50:37.621872 cg-60.4.7/tests/fixtures/apps/demultiplexing/flow_cells_demux_all/211101_A00187_0615_AHLG5GDRZZ/RTAComplete.txt
+-rw-r--r--   0        0        0     6665 2024-04-29 07:50:37.621872 cg-60.4.7/tests/fixtures/apps/demultiplexing/flow_cells_demux_all/211101_A00187_0615_AHLG5GDRZZ/RunParameters.xml
+-rw-r--r--   0        0        0      399 2024-04-29 07:50:37.621872 cg-60.4.7/tests/fixtures/apps/demultiplexing/flow_cells_demux_all/211101_A00187_0615_AHLG5GDRZZ/SampleSheet.csv
+-rw-r--r--   0        0        0        0 2024-04-29 07:50:37.621872 cg-60.4.7/tests/fixtures/apps/demultiplexing/nanopore/experiment_name/sample_1/20231205_1618_3B_PAS86456_72d9fceb/fastq_pass/PAS86456_pass_72d9fceb_8a4fd683_0.fastq.gz
+-rw-r--r--   0        0        0        0 2024-04-29 07:50:37.621872 cg-60.4.7/tests/fixtures/apps/demultiplexing/nanopore/experiment_name/sample_1/20231205_1618_3B_PAS86456_72d9fceb/fastq_pass/PAS86456_pass_72d9fceb_8a4fd683_1.fastq.gz
+-rw-r--r--   0        0        0        0 2024-04-29 07:50:37.621872 cg-60.4.7/tests/fixtures/apps/demultiplexing/nanopore/experiment_name/sample_1/20231205_1618_3B_PAS86456_72d9fceb/final_summary_PAS86456_72d9fceb_8a4fd683.txt
+-rw-r--r--   0        0        0        0 2024-04-29 07:50:37.621872 cg-60.4.7/tests/fixtures/apps/demultiplexing/nanopore/experiment_name/sample_1/20231205_1618_3B_PAS86456_72d9fceb/pod5_pass/PAS86456_pass_72d9fceb_8a4fd683_0.pod5
+-rw-r--r--   0        0        0        0 2024-04-29 07:50:37.621872 cg-60.4.7/tests/fixtures/apps/demultiplexing/nanopore/experiment_name/sample_1/20231205_1618_3B_PAS86456_72d9fceb/pod5_pass/PAS86456_pass_72d9fceb_8a4fd683_1.pod5
+-rw-r--r--   0        0        0        0 2024-04-29 07:50:37.621872 cg-60.4.7/tests/fixtures/apps/demultiplexing/nanopore/experiment_name/sample_2/20231205_1618_3D_PAS97781_595b5663/fastq_pass/PAS97781_pass_595b5663_efc7f02e_0.fastq.gz
+-rw-r--r--   0        0        0        0 2024-04-29 07:50:37.621872 cg-60.4.7/tests/fixtures/apps/demultiplexing/nanopore/experiment_name/sample_2/20231205_1618_3D_PAS97781_595b5663/fastq_pass/PAS97781_pass_595b5663_efc7f02e_1.fastq.gz
+-rw-r--r--   0        0        0        0 2024-04-29 07:50:37.621872 cg-60.4.7/tests/fixtures/apps/demultiplexing/nanopore/experiment_name/sample_2/20231205_1618_3D_PAS97781_595b5663/final_summary_PAS97781_595b5663_efc7f02e.txt
+-rw-r--r--   0        0        0        0 2024-04-29 07:50:37.621872 cg-60.4.7/tests/fixtures/apps/demultiplexing/nanopore/experiment_name/sample_2/20231205_1618_3D_PAS97781_595b5663/pod5_pass/PAS97781_pass_595b5663_efc7f02e_0.pod5
+-rw-r--r--   0        0        0        0 2024-04-29 07:50:37.621872 cg-60.4.7/tests/fixtures/apps/demultiplexing/nanopore/experiment_name/sample_2/20231205_1618_3D_PAS97781_595b5663/pod5_pass/PAS97781_pass_595b5663_efc7f02e_1.pod5
+-rw-r--r--   0        0        0     5319 2024-04-29 07:50:37.621872 cg-60.4.7/tests/fixtures/apps/demultiplexing/run_parameters/RunParameters_hiseq_2500_different_index_cycles.xml
+-rw-r--r--   0        0        0     5944 2024-04-29 07:50:37.621872 cg-60.4.7/tests/fixtures/apps/demultiplexing/run_parameters/RunParameters_novaseq_6000_different_index_cycles.xml
+-rwxr-xr-x   0        0        0     2603 2024-04-29 07:50:37.621872 cg-60.4.7/tests/fixtures/apps/demultiplexing/run_parameters/RunParameters_novaseq_X_different_index_cycles.xml
+-rwxr-xr-x   0        0        0     2597 2024-04-29 07:50:37.621872 cg-60.4.7/tests/fixtures/apps/demultiplexing/run_parameters/RunParameters_novaseq_X_wrong_instrument.xml
+-rw-r--r--   0        0        0     5899 2024-04-29 07:50:37.621872 cg-60.4.7/tests/fixtures/apps/demultiplexing/run_parameters/RunParameters_novaseq_no_software_nor_reagent_version.xml
+-rw-r--r--   0        0        0     4941 2024-04-29 07:50:37.621872 cg-60.4.7/tests/fixtures/apps/demultiplexing/sample_sheets/novaseq_6000_sample_sheet_with_reversed_cycles.csv
+-rw-r--r--   0        0        0    10950 2024-04-29 07:50:37.621872 cg-60.4.7/tests/fixtures/apps/demultiplexing/sample_sheets/novaseq_x_sample_sheet_with_forward_cycles.csv
+-rw-r--r--   0        0        0        0 2024-04-29 07:50:37.621872 cg-60.4.7/tests/fixtures/apps/demultiplexing/spring/dummy_run_001.spring
+-rw-r--r--   0        0        0        0 2024-04-29 07:50:37.621872 cg-60.4.7/tests/fixtures/apps/demultiplexing/spring/dummy_run_002.spring
+-rw-r--r--   0        0        0        0 2024-04-29 07:50:37.621872 cg-60.4.7/tests/fixtures/apps/demultiplexing/spring/dummy_spring_meta_data.json
+-rw-r--r--   0        0        0        0 2024-04-29 07:50:37.621872 cg-60.4.7/tests/fixtures/apps/fluffy/2020-23219-05/2020-23219-05.WCXpredict_aberrations.filt.bed
+-rw-r--r--   0        0        0     5554 2024-04-29 07:50:37.621872 cg-60.4.7/tests/fixtures/apps/fluffy/SampleSheet.csv
+-rw-r--r--   0        0        0      901 2024-04-29 07:50:37.621872 cg-60.4.7/tests/fixtures/apps/fluffy/deliverables.yaml
+-rw-r--r--   0        0        0        0 2024-04-29 07:50:37.621872 cg-60.4.7/tests/fixtures/apps/fluffy/fluffy_fastq.fastq.gz
+-rw-r--r--   0        0        0        0 2024-04-29 07:50:37.621872 cg-60.4.7/tests/fixtures/apps/fluffy/multiqc_report.html
+-rw-r--r--   0        0        0        0 2024-04-29 07:50:37.621872 cg-60.4.7/tests/fixtures/apps/fluffy/summary.csv
+-rw-r--r--   0        0        0        0 2024-04-29 07:50:37.621872 cg-60.4.7/tests/fixtures/apps/gt/yellowhog.bcf
+-rw-r--r--   0        0        0     5114 2024-04-29 07:50:37.621872 cg-60.4.7/tests/fixtures/apps/madeline/madeline.xml
+-rw-r--r--   0        0        0        0 2024-04-29 07:50:37.621872 cg-60.4.7/tests/fixtures/apps/mip/case_file.txt
+-rw-r--r--   0        0        0     3241 2024-04-29 07:50:37.621872 cg-60.4.7/tests/fixtures/apps/mip/case_metrics_deliverables.yaml
+-rw-r--r--   0        0        0    21811 2024-04-29 07:50:37.621872 cg-60.4.7/tests/fixtures/apps/mip/dna/store/case_config.yaml
+-rw-r--r--   0        0        0    23364 2024-04-29 07:50:37.621872 cg-60.4.7/tests/fixtures/apps/mip/dna/store/case_id_deliverables.yaml
+-rw-r--r--   0        0        0    37367 2024-04-29 07:50:37.621872 cg-60.4.7/tests/fixtures/apps/mip/dna/store/case_qc_sample_info.yaml
+-rw-r--r--   0        0        0       16 2024-04-29 07:50:37.621872 cg-60.4.7/tests/fixtures/apps/mip/dna/store/empty_case_config.yaml
+-rw-r--r--   0        0        0       16 2024-04-29 07:50:37.621872 cg-60.4.7/tests/fixtures/apps/mip/dna/store/empty_case_metrics_deliverables.yaml
+-rw-r--r--   0        0        0       16 2024-04-29 07:50:37.621872 cg-60.4.7/tests/fixtures/apps/mip/dna/store/empty_case_qc_sample_info.yaml
+-rw-r--r--   0        0        0      123 2024-04-29 07:50:37.621872 cg-60.4.7/tests/fixtures/apps/mip/dna/store/empty_delivery_report.html
+-rw-r--r--   0        0        0    62741 2024-04-29 07:50:37.621872 cg-60.4.7/tests/fixtures/apps/mip/dna/store/yellowhog_clinical_selected.vcf
+-rw-r--r--   0        0        0    11242 2024-04-29 07:50:37.621872 cg-60.4.7/tests/fixtures/apps/mip/rna/case_config.yaml
+-rw-r--r--   0        0        0    12164 2024-04-29 07:50:37.621872 cg-60.4.7/tests/fixtures/apps/mip/rna/case_qc_sampleinfo.yaml
+-rw-r--r--   0        0        0     5231 2024-04-29 07:50:37.621872 cg-60.4.7/tests/fixtures/apps/mip/rna/store/bundle_data.yaml
+-rw-r--r--   0        0        0     9774 2024-04-29 07:50:37.621872 cg-60.4.7/tests/fixtures/apps/mip/rna/store/case_config.yaml
+-rw-r--r--   0        0        0     4624 2024-04-29 07:50:37.621872 cg-60.4.7/tests/fixtures/apps/mip/rna/store/case_id_deliverables.yaml
+-rw-r--r--   0        0        0    13666 2024-04-29 07:50:37.621872 cg-60.4.7/tests/fixtures/apps/mip/rna/store/case_qc_sample_info.yaml
+-rw-r--r--   0        0        0        0 2024-04-29 07:50:37.621872 cg-60.4.7/tests/fixtures/apps/mip/sample_file.txt
+-rw-r--r--   0        0        0     1885 2024-04-29 07:50:37.621872 cg-60.4.7/tests/fixtures/apps/scout/643594.config.yaml
+-rw-r--r--   0        0        0     6027 2024-04-29 07:50:37.621872 cg-60.4.7/tests/fixtures/apps/scout/case_export.json
+-rw-r--r--   0        0        0     9349 2024-04-29 07:50:37.621872 cg-60.4.7/tests/fixtures/apps/scout/export_causatives.json
+-rw-r--r--   0        0        0     1315 2024-04-29 07:50:37.621872 cg-60.4.7/tests/fixtures/apps/scout/none_case_export.json
+-rw-r--r--   0        0        0     3518 2024-04-29 07:50:37.621872 cg-60.4.7/tests/fixtures/apps/scout/other_sex_case.json
+-rw-r--r--   0        0        0     8874 2024-04-29 07:50:37.621872 cg-60.4.7/tests/fixtures/apps/scout/panel_export.bed
+-rw-r--r--   0        0        0     4169 2024-04-29 07:50:37.621872 cg-60.4.7/tests/fixtures/apps/scout/panel_export.csv
+-rw-r--r--   0        0        0      619 2024-04-29 07:50:37.621872 cg-60.4.7/tests/fixtures/apps/sequencing_metrics_parser/230622_A00621_0864_AHY7FFDRX2/SampleSheet.csv
+-rw-r--r--   0        0        0    63569 2024-04-29 07:50:37.621872 cg-60.4.7/tests/fixtures/apps/sequencing_metrics_parser/230622_A00621_0864_AHY7FFDRX2/Unaligned/Reports/Adapter_Metrics.csv
+-rw-r--r--   0        0        0    42478 2024-04-29 07:50:37.621872 cg-60.4.7/tests/fixtures/apps/sequencing_metrics_parser/230622_A00621_0864_AHY7FFDRX2/Unaligned/Reports/Demultiplex_Stats.csv
+-rw-r--r--   0        0        0    69708 2024-04-29 07:50:37.625872 cg-60.4.7/tests/fixtures/apps/sequencing_metrics_parser/230622_A00621_0864_AHY7FFDRX2/Unaligned/Reports/Quality_Metrics.csv
+-rw-r--r--   0        0        0       42 2024-04-29 07:50:37.625872 cg-60.4.7/tests/fixtures/apps/shipping/scout-deploy.yaml
+-rw-r--r--   0        0        0     1036 2024-04-29 07:50:37.625872 cg-60.4.7/tests/fixtures/cgweb_orders/balsamic.json
+-rw-r--r--   0        0        0     1104 2024-04-29 07:50:37.625872 cg-60.4.7/tests/fixtures/cgweb_orders/fastq.json
+-rw-r--r--   0        0        0     1313 2024-04-29 07:50:37.625872 cg-60.4.7/tests/fixtures/cgweb_orders/metagenome.json
+-rw-r--r--   0        0        0     3038 2024-04-29 07:50:37.625872 cg-60.4.7/tests/fixtures/cgweb_orders/microsalt.json
+-rw-r--r--   0        0        0     3705 2024-04-29 07:50:37.625872 cg-60.4.7/tests/fixtures/cgweb_orders/mip.json
+-rw-r--r--   0        0        0     1364 2024-04-29 07:50:37.625872 cg-60.4.7/tests/fixtures/cgweb_orders/mip_rna.json
+-rw-r--r--   0        0        0     2125 2024-04-29 07:50:37.625872 cg-60.4.7/tests/fixtures/cgweb_orders/rml.json
+-rw-r--r--   0        0        0     1368 2024-04-29 07:50:37.625872 cg-60.4.7/tests/fixtures/cgweb_orders/rnafusion.json
+-rw-r--r--   0        0        0     4684 2024-04-29 07:50:37.625872 cg-60.4.7/tests/fixtures/cgweb_orders/sarscov2.json
+-rw-r--r--   0        0        0     5609 2024-04-29 07:50:37.625872 cg-60.4.7/tests/fixtures/data/SampleSheet.csv
+-rw-r--r--   0        0        0      511 2024-04-29 07:50:37.625872 cg-60.4.7/tests/fixtures/data/bcl_convert_sample_sheet.csv
+-rw-r--r--   0        0        0   258048 2024-04-29 07:50:37.625872 cg-60.4.7/tests/fixtures/data/cgfixture.db
+-rw-r--r--   0        0        0        0 2024-04-29 07:50:37.625872 cg-60.4.7/tests/fixtures/data/fastq.fastq.gz
+-rw-r--r--   0        0        0    49152 2024-04-29 07:50:37.625872 cg-60.4.7/tests/fixtures/data/hkstore.db
+-rw-r--r--   0        0        0       73 2024-04-29 07:50:37.625872 cg-60.4.7/tests/fixtures/data/yellowhog/pedigree.yaml
+-rw-r--r--   0        0        0       76 2024-04-29 07:50:37.625872 cg-60.4.7/tests/fixtures/io/casava_five_parts.fastq.gz
+-rw-r--r--   0        0        0       90 2024-04-29 07:50:37.625872 cg-60.4.7/tests/fixtures/io/casava_seven_parts.fastq.gz
+-rw-r--r--   0        0        0       96 2024-04-29 07:50:37.625872 cg-60.4.7/tests/fixtures/io/casava_ten_parts.fastq.gz
+-rw-r--r--   0        0        0      153 2024-04-29 07:50:37.625872 cg-60.4.7/tests/fixtures/io/example.csv
+-rw-r--r--   0        0        0       46 2024-04-29 07:50:37.625872 cg-60.4.7/tests/fixtures/io/example.gz
+-rw-r--r--   0        0        0      147 2024-04-29 07:50:37.625872 cg-60.4.7/tests/fixtures/io/example.tsv
+-rw-r--r--   0        0        0       20 2024-04-29 07:50:37.625872 cg-60.4.7/tests/fixtures/io/example.txt
+-rw-r--r--   0        0        0       20 2024-04-29 07:50:37.625872 cg-60.4.7/tests/fixtures/io/example2.txt
+-rw-r--r--   0        0        0      582 2024-04-29 07:50:37.625872 cg-60.4.7/tests/fixtures/io/example_json.json
+-rw-r--r--   0        0        0      103 2024-04-29 07:50:37.625872 cg-60.4.7/tests/fixtures/io/example_xml.xml
+-rw-r--r--   0        0        0       20 2024-04-29 07:50:37.625872 cg-60.4.7/tests/fixtures/meta/qc_metrics/file_with_right_tags.json
+-rw-r--r--   0        0        0       20 2024-04-29 07:50:37.625872 cg-60.4.7/tests/fixtures/meta/qc_metrics/file_without_right_tags.json
+-rw-r--r--   0        0        0   156910 2024-04-29 07:50:37.629872 cg-60.4.7/tests/fixtures/orderforms/1508.30.balsamic.xlsx
+-rw-r--r--   0        0        0   156770 2024-04-29 07:50:37.629872 cg-60.4.7/tests/fixtures/orderforms/1508.30.balsamic_qc.xlsx
+-rw-r--r--   0        0        0   156737 2024-04-29 07:50:37.629872 cg-60.4.7/tests/fixtures/orderforms/1508.30.balsamic_umi.xlsx
+-rw-r--r--   0        0        0   156582 2024-04-29 07:50:37.629872 cg-60.4.7/tests/fixtures/orderforms/1508.30.fastq.xlsx
+-rw-r--r--   0        0        0   155627 2024-04-29 07:50:37.629872 cg-60.4.7/tests/fixtures/orderforms/1508.30.metagenome.xlsx
+-rw-r--r--   0        0        0   156850 2024-04-29 07:50:37.629872 cg-60.4.7/tests/fixtures/orderforms/1508.30.mip.xlsx
+-rw-r--r--   0        0        0   258580 2024-04-29 07:50:37.629872 cg-60.4.7/tests/fixtures/orderforms/1508.30.mip_rna.xlsx
+-rw-r--r--   0        0        0   258342 2024-04-29 07:50:37.629872 cg-60.4.7/tests/fixtures/orderforms/1508.30.rnafusion.xlsx
+-rw-r--r--   0        0        0    82677 2024-04-29 07:50:37.633872 cg-60.4.7/tests/fixtures/orderforms/1603.11.microbial.xlsx
+-rw-r--r--   0        0        0   149394 2024-04-29 07:50:37.633872 cg-60.4.7/tests/fixtures/orderforms/1604.17.rml.xlsx
+-rw-r--r--   0        0        0   223184 2024-04-29 07:50:37.633872 cg-60.4.7/tests/fixtures/orderforms/2184.9.sarscov2.xlsx
+-rw-r--r--   0        0        0    18639 2024-04-29 07:50:37.633872 cg-60.4.7/tests/fixtures/orderforms/NIPT-json.json
+-rw-r--r--   0        0        0     6052 2024-04-29 07:50:37.633872 cg-60.4.7/tests/fixtures/orderforms/balsamic_uploaded_json_orderform.json
+-rw-r--r--   0        0        0     6611 2024-04-29 07:50:37.633872 cg-60.4.7/tests/fixtures/orderforms/mip_uploaded_json_orderform.json
+-rw-r--r--   0        0        0     1417 2024-04-29 07:50:37.633872 cg-60.4.7/tests/fixtures/report/case_data.json
+-rw-r--r--   0        0        0     1109 2024-04-29 07:50:37.633872 cg-60.4.7/tests/fixtures/report/lims_exported_samples.json
+-rw-r--r--   0        0        0     1562 2024-04-29 07:50:37.633872 cg-60.4.7/tests/fixtures/report/lims_family.json
+-rw-r--r--   0        0        0     3296 2024-04-29 07:50:37.633872 cg-60.4.7/tests/io/conftest.py
+-rw-r--r--   0        0        0      431 2024-04-29 07:50:37.633872 cg-60.4.7/tests/io/test_io_config.py
+-rw-r--r--   0        0        0     8639 2024-04-29 07:50:37.633872 cg-60.4.7/tests/io/test_io_controller.py
+-rw-r--r--   0        0        0     3877 2024-04-29 07:50:37.633872 cg-60.4.7/tests/io/test_io_csv.py
+-rw-r--r--   0        0        0      482 2024-04-29 07:50:37.633872 cg-60.4.7/tests/io/test_io_gzip.py
+-rw-r--r--   0        0        0     1779 2024-04-29 07:50:37.633872 cg-60.4.7/tests/io/test_io_json.py
+-rw-r--r--   0        0        0     2914 2024-04-29 07:50:37.633872 cg-60.4.7/tests/io/test_io_txt.py
+-rw-r--r--   0        0        0     1027 2024-04-29 07:50:37.633872 cg-60.4.7/tests/io/test_io_xml.py
+-rw-r--r--   0        0        0     2131 2024-04-29 07:50:37.633872 cg-60.4.7/tests/io/test_io_yaml.py
+-rw-r--r--   0        0        0     1233 2024-04-29 07:50:37.633872 cg-60.4.7/tests/io/test_validate_path.py
+-rw-r--r--   0        0        0        0 2024-04-29 07:50:37.633872 cg-60.4.7/tests/meta/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-29 07:50:37.633872 cg-60.4.7/tests/meta/archive/__init__.py
+-rw-r--r--   0        0        0    13131 2024-04-29 07:50:37.633872 cg-60.4.7/tests/meta/archive/conftest.py
+-rw-r--r--   0        0        0    16858 2024-04-29 07:50:37.633872 cg-60.4.7/tests/meta/archive/test_archive_api.py
+-rw-r--r--   0        0        0    10246 2024-04-29 07:50:37.633872 cg-60.4.7/tests/meta/archive/test_archive_cli.py
+-rw-r--r--   0        0        0    15766 2024-04-29 07:50:37.633872 cg-60.4.7/tests/meta/archive/test_archiving.py
+-rw-r--r--   0        0        0     3807 2024-04-29 07:50:37.633872 cg-60.4.7/tests/meta/backup/conftest.py
+-rw-r--r--   0        0        0    26368 2024-04-29 07:50:37.633872 cg-60.4.7/tests/meta/backup/test_meta_backup.py
+-rw-r--r--   0        0        0    10055 2024-04-29 07:50:37.633872 cg-60.4.7/tests/meta/backup/test_meta_pdc.py
+-rw-r--r--   0        0        0    12570 2024-04-29 07:50:37.633872 cg-60.4.7/tests/meta/clean/conftest.py
+-rw-r--r--   0        0        0    16944 2024-04-29 07:50:37.633872 cg-60.4.7/tests/meta/clean/test_clean_flow_cells_api.py
+-rw-r--r--   0        0        0     2286 2024-04-29 07:50:37.633872 cg-60.4.7/tests/meta/clean/test_clean_retrieved_spring_files.py
+-rw-r--r--   0        0        0     7691 2024-04-29 07:50:37.633872 cg-60.4.7/tests/meta/compress/conftest.py
+-rw-r--r--   0        0        0     7961 2024-04-29 07:50:37.633872 cg-60.4.7/tests/meta/compress/test_clean_fastq.py
+-rw-r--r--   0        0        0     1778 2024-04-29 07:50:37.633872 cg-60.4.7/tests/meta/compress/test_compress_files.py
+-rw-r--r--   0        0        0     3644 2024-04-29 07:50:37.633872 cg-60.4.7/tests/meta/compress/test_compress_meta_fastq.py
+-rw-r--r--   0        0        0     1180 2024-04-29 07:50:37.633872 cg-60.4.7/tests/meta/compress/test_decompress_spring_meta.py
+-rw-r--r--   0        0        0     7045 2024-04-29 07:50:37.633872 cg-60.4.7/tests/meta/compress/test_meta_compress_update_hk.py
+-rw-r--r--   0        0        0     8269 2024-04-29 07:50:37.633872 cg-60.4.7/tests/meta/conftest.py
+-rw-r--r--   0        0        0        0 2024-04-29 07:50:37.633872 cg-60.4.7/tests/meta/deliver/__init__.py
+-rw-r--r--   0        0        0     3471 2024-04-29 07:50:37.633872 cg-60.4.7/tests/meta/deliver/conftest.py
+-rw-r--r--   0        0        0     5533 2024-04-29 07:50:37.633872 cg-60.4.7/tests/meta/deliver/test_deliver_ticket.py
+-rw-r--r--   0        0        0    10277 2024-04-29 07:50:37.633872 cg-60.4.7/tests/meta/deliver/test_delivery_api.py
+-rw-r--r--   0        0        0     1057 2024-04-29 07:50:37.633872 cg-60.4.7/tests/meta/deliver/test_fastq_path_generator.py
+-rw-r--r--   0        0        0        0 2024-04-29 07:50:37.633872 cg-60.4.7/tests/meta/delivery/__init__.py
+-rw-r--r--   0        0        0    16660 2024-04-29 07:50:37.633872 cg-60.4.7/tests/meta/delivery/test_delivery_api.py
+-rw-r--r--   0        0        0     8066 2024-04-29 07:50:37.633872 cg-60.4.7/tests/meta/demultiplex/conftest.py
+-rw-r--r--   0        0        0     5382 2024-04-29 07:50:37.633872 cg-60.4.7/tests/meta/demultiplex/test_combine_sequencing_metrics.py
+-rw-r--r--   0        0        0     8445 2024-04-29 07:50:37.633872 cg-60.4.7/tests/meta/demultiplex/test_demux_post_processing.py
+-rw-r--r--   0        0        0    12406 2024-04-29 07:50:37.633872 cg-60.4.7/tests/meta/demultiplex/test_housekeeper_storage_functions.py
+-rw-r--r--   0        0        0     4392 2024-04-29 07:50:37.637872 cg-60.4.7/tests/meta/demultiplex/test_status_db_storage_functions.py
+-rw-r--r--   0        0        0    22787 2024-04-29 07:50:37.637872 cg-60.4.7/tests/meta/demultiplex/test_utils.py
+-rw-r--r--   0        0        0     6258 2024-04-29 07:50:37.637872 cg-60.4.7/tests/meta/demultiplex/test_validation.py
+-rw-r--r--   0        0        0     4943 2024-04-29 07:50:37.637872 cg-60.4.7/tests/meta/encryption/conftest.py
+-rw-r--r--   0        0        0    18133 2024-04-29 07:50:37.637872 cg-60.4.7/tests/meta/encryption/test_encryption.py
+-rw-r--r--   0        0        0     3122 2024-04-29 07:50:37.637872 cg-60.4.7/tests/meta/observations/conftest.py
+-rw-r--r--   0        0        0    16164 2024-04-29 07:50:37.637872 cg-60.4.7/tests/meta/observations/test_meta_upload_observations.py
+-rw-r--r--   0        0        0     4974 2024-04-29 07:50:37.637872 cg-60.4.7/tests/meta/orders/conftest.py
+-rw-r--r--   0        0        0     1749 2024-04-29 07:50:37.637872 cg-60.4.7/tests/meta/orders/test_PoolSubmitter_validate_order.py
+-rw-r--r--   0        0        0     1470 2024-04-29 07:50:37.637872 cg-60.4.7/tests/meta/orders/test_SarsCov2Submitter_order_to_status.py
+-rw-r--r--   0        0        0     1768 2024-04-29 07:50:37.637872 cg-60.4.7/tests/meta/orders/test_SarsCov2Submitter_store_order.py
+-rw-r--r--   0        0        0     2032 2024-04-29 07:50:37.637872 cg-60.4.7/tests/meta/orders/test_SarsCov2Submitter_validate_order.py
+-rw-r--r--   0        0        0    19783 2024-04-29 07:50:37.637872 cg-60.4.7/tests/meta/orders/test_meta_orders_api.py
+-rw-r--r--   0        0        0     7086 2024-04-29 07:50:37.637872 cg-60.4.7/tests/meta/orders/test_meta_orders_lims.py
+-rw-r--r--   0        0        0    29515 2024-04-29 07:50:37.637872 cg-60.4.7/tests/meta/orders/test_meta_orders_status.py
+-rw-r--r--   0        0        0     1677 2024-04-29 07:50:37.637872 cg-60.4.7/tests/meta/orders/test_rnafusion_submitter.py
+-rw-r--r--   0        0        0     1068 2024-04-29 07:50:37.637872 cg-60.4.7/tests/meta/orders/test_ticket_handler.py
+-rw-r--r--   0        0        0     4336 2024-04-29 07:50:37.637872 cg-60.4.7/tests/meta/qc_metrics/conftest.py
+-rw-r--r--   0        0        0     1972 2024-04-29 07:50:37.637872 cg-60.4.7/tests/meta/qc_metrics/test_collect_qc_metrics.py
+-rw-r--r--   0        0        0        0 2024-04-29 07:50:37.637872 cg-60.4.7/tests/meta/report/__init__.py
+-rw-r--r--   0        0        0     6512 2024-04-29 07:50:37.637872 cg-60.4.7/tests/meta/report/conftest.py
+-rw-r--r--   0        0        0      434 2024-04-29 07:50:37.637872 cg-60.4.7/tests/meta/report/helper.py
+-rw-r--r--   0        0        0     2604 2024-04-29 07:50:37.637872 cg-60.4.7/tests/meta/report/test_balsamic_api.py
+-rw-r--r--   0        0        0     4056 2024-04-29 07:50:37.637872 cg-60.4.7/tests/meta/report/test_field_validators.py
+-rw-r--r--   0        0        0     2858 2024-04-29 07:50:37.637872 cg-60.4.7/tests/meta/report/test_mip_dna_api.py
+-rw-r--r--   0        0        0    16042 2024-04-29 07:50:37.637872 cg-60.4.7/tests/meta/report/test_report_api.py
+-rw-r--r--   0        0        0     1365 2024-04-29 07:50:37.637872 cg-60.4.7/tests/meta/report/test_rnafusion_api.py
+-rw-r--r--   0        0        0     1250 2024-04-29 07:50:37.637872 cg-60.4.7/tests/meta/report/test_tomte_api.py
+-rw-r--r--   0        0        0        0 2024-04-29 07:50:37.637872 cg-60.4.7/tests/meta/rsync/__init__.py
+-rw-r--r--   0        0        0      916 2024-04-29 07:50:37.637872 cg-60.4.7/tests/meta/rsync/conftest.py
+-rw-r--r--   0        0        0     9442 2024-04-29 07:50:37.637872 cg-60.4.7/tests/meta/rsync/test_rsync.py
+-rw-r--r--   0        0        0     3147 2024-04-29 07:50:37.637872 cg-60.4.7/tests/meta/test_invoice.py
+-rw-r--r--   0        0        0     1220 2024-04-29 07:50:37.637872 cg-60.4.7/tests/meta/transfer/conftest.py
+-rw-r--r--   0        0        0     9892 2024-04-29 07:50:37.637872 cg-60.4.7/tests/meta/transfer/test_external_data.py
+-rw-r--r--   0        0        0     4395 2024-04-29 07:50:37.637872 cg-60.4.7/tests/meta/transfer/test_meta_transfer_lims.py
+-rw-r--r--   0        0        0        0 2024-04-29 07:50:37.637872 cg-60.4.7/tests/meta/upload/__init__.py
+-rw-r--r--   0        0        0     2210 2024-04-29 07:50:37.637872 cg-60.4.7/tests/meta/upload/balsamic/test_balsamic.py
+-rw-r--r--   0        0        0     4002 2024-04-29 07:50:37.637872 cg-60.4.7/tests/meta/upload/conftest.py
+-rw-r--r--   0        0        0        0 2024-04-29 07:50:37.637872 cg-60.4.7/tests/meta/upload/gisaid/__init__.py
+-rw-r--r--   0        0        0     2557 2024-04-29 07:50:37.637872 cg-60.4.7/tests/meta/upload/gisaid/fixtures/four_samples.csv
+-rw-r--r--   0        0        0        0 2024-04-29 07:50:37.637872 cg-60.4.7/tests/meta/upload/gisaid/fixtures/invalid_housekeeper.fasta
+-rw-r--r--   0        0        0      211 2024-04-29 07:50:37.637872 cg-60.4.7/tests/meta/upload/gisaid/fixtures/valid_gisaid.fasta
+-rw-r--r--   0        0        0      371 2024-04-29 07:50:37.637872 cg-60.4.7/tests/meta/upload/gisaid/fixtures/valid_housekeeper.fasta
+-rw-r--r--   0        0        0        0 2024-04-29 07:50:37.637872 cg-60.4.7/tests/meta/upload/mutacc/__init__.py
+-rw-r--r--   0        0        0     3684 2024-04-29 07:50:37.637872 cg-60.4.7/tests/meta/upload/mutacc/conftest.py
+-rw-r--r--   0        0        0     4188 2024-04-29 07:50:37.637872 cg-60.4.7/tests/meta/upload/mutacc/test_meta_upload_mutacc.py
+-rw-r--r--   0        0        0     1149 2024-04-29 07:50:37.637872 cg-60.4.7/tests/meta/upload/nipt/conftest.py
+-rw-r--r--   0        0        0     1683 2024-04-29 07:50:37.637872 cg-60.4.7/tests/meta/upload/nipt/test_models.py
+-rw-r--r--   0        0        0     1242 2024-04-29 07:50:37.637872 cg-60.4.7/tests/meta/upload/nipt/test_nipt_upload_api.py
+-rw-r--r--   0        0        0        0 2024-04-29 07:50:37.637872 cg-60.4.7/tests/meta/upload/scout/__init__.py
+-rw-r--r--   0        0        0    23954 2024-04-29 07:50:37.637872 cg-60.4.7/tests/meta/upload/scout/conftest.py
+-rw-r--r--   0        0        0     4734 2024-04-29 07:50:37.637872 cg-60.4.7/tests/meta/upload/scout/test_generate_load_config.py
+-rw-r--r--   0        0        0     4182 2024-04-29 07:50:37.637872 cg-60.4.7/tests/meta/upload/scout/test_meta_upload_scoutapi.py
+-rw-r--r--   0        0        0    33260 2024-04-29 07:50:37.637872 cg-60.4.7/tests/meta/upload/scout/test_meta_upload_scoutapi_rna.py
+-rw-r--r--   0        0        0     7372 2024-04-29 07:50:37.637872 cg-60.4.7/tests/meta/upload/scout/test_scout_config_builder.py
+-rw-r--r--   0        0        0     2511 2024-04-29 07:50:37.637872 cg-60.4.7/tests/meta/upload/test_meta_upload_coverage.py
+-rw-r--r--   0        0        0     1473 2024-04-29 07:50:37.637872 cg-60.4.7/tests/meta/upload/test_upload_api.py
+-rw-r--r--   0        0        0     2547 2024-04-29 07:50:37.637872 cg-60.4.7/tests/meta/upload/test_upload_genotypes_api.py
+-rw-r--r--   0        0        0        0 2024-04-29 07:50:37.637872 cg-60.4.7/tests/meta/workflow/__init__.py
+-rw-r--r--   0        0        0    10262 2024-04-29 07:50:37.637872 cg-60.4.7/tests/meta/workflow/conftest.py
+-rw-r--r--   0        0        0     3679 2024-04-29 07:50:37.637872 cg-60.4.7/tests/meta/workflow/microsalt/conftest.py
+-rw-r--r--   0        0        0      318 2024-04-29 07:50:37.637872 cg-60.4.7/tests/meta/workflow/microsalt/test_parsing_metrics.py
+-rw-r--r--   0        0        0     3759 2024-04-29 07:50:37.637872 cg-60.4.7/tests/meta/workflow/microsalt/test_quality_controller.py
+-rw-r--r--   0        0        0    14367 2024-04-29 07:50:37.637872 cg-60.4.7/tests/meta/workflow/microsalt/test_quality_controller_utils.py
+-rw-r--r--   0        0        0      825 2024-04-29 07:50:37.637872 cg-60.4.7/tests/meta/workflow/microsalt/test_report_generation.py
+-rw-r--r--   0        0        0    20860 2024-04-29 07:50:37.637872 cg-60.4.7/tests/meta/workflow/test_analysis.py
+-rw-r--r--   0        0        0     7934 2024-04-29 07:50:37.637872 cg-60.4.7/tests/meta/workflow/test_balsamic.py
+-rw-r--r--   0        0        0     3034 2024-04-29 07:50:37.637872 cg-60.4.7/tests/meta/workflow/test_fastq.py
+-rw-r--r--   0        0        0     1532 2024-04-29 07:50:37.637872 cg-60.4.7/tests/meta/workflow/test_microsalt.py
+-rw-r--r--   0        0        0     2721 2024-04-29 07:50:37.637872 cg-60.4.7/tests/meta/workflow/test_nf_analysis.py
+-rw-r--r--   0        0        0     7741 2024-04-29 07:50:37.637872 cg-60.4.7/tests/meta/workflow/test_prepare_fastq_api.py
+-rw-r--r--   0        0        0     1920 2024-04-29 07:50:37.637872 cg-60.4.7/tests/meta/workflow/test_raredisease.py
+-rw-r--r--   0        0        0     1674 2024-04-29 07:50:37.637872 cg-60.4.7/tests/meta/workflow/test_rnafusion.py
+-rw-r--r--   0        0        0        0 2024-04-29 07:50:37.637872 cg-60.4.7/tests/mocks/__init__.py
+-rw-r--r--   0        0        0     1168 2024-04-29 07:50:37.637872 cg-60.4.7/tests/mocks/balsamic_analysis_mock.py
+-rw-r--r--   0        0        0     3500 2024-04-29 07:50:37.641872 cg-60.4.7/tests/mocks/crunchy.py
+-rw-r--r--   0        0        0    21778 2024-04-29 07:50:37.641872 cg-60.4.7/tests/mocks/hk_mock.py
+-rw-r--r--   0        0        0     4106 2024-04-29 07:50:37.641872 cg-60.4.7/tests/mocks/limsmock.py
+-rw-r--r--   0        0        0      572 2024-04-29 07:50:37.641872 cg-60.4.7/tests/mocks/madeline.py
+-rw-r--r--   0        0        0     1297 2024-04-29 07:50:37.641872 cg-60.4.7/tests/mocks/mip_analysis_mock.py
+-rw-r--r--   0        0        0     1525 2024-04-29 07:50:37.641872 cg-60.4.7/tests/mocks/osticket.py
+-rw-r--r--   0        0        0     3239 2024-04-29 07:50:37.641872 cg-60.4.7/tests/mocks/process_mock.py
+-rw-r--r--   0        0        0     4713 2024-04-29 07:50:37.641872 cg-60.4.7/tests/mocks/report.py
+-rw-r--r--   0        0        0     3915 2024-04-29 07:50:37.641872 cg-60.4.7/tests/mocks/scout.py
+-rw-r--r--   0        0        0      750 2024-04-29 07:50:37.641872 cg-60.4.7/tests/mocks/store_model.py
+-rw-r--r--   0        0        0     1620 2024-04-29 07:50:37.641872 cg-60.4.7/tests/mocks/tb_mock.py
+-rw-r--r--   0        0        0        0 2024-04-29 07:50:37.641872 cg-60.4.7/tests/models/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-29 07:50:37.641872 cg-60.4.7/tests/models/balsamic/__init__.py
+-rw-r--r--   0        0        0     1194 2024-04-29 07:50:37.641872 cg-60.4.7/tests/models/balsamic/conftest.py
+-rw-r--r--   0        0        0     1030 2024-04-29 07:50:37.641872 cg-60.4.7/tests/models/balsamic/test_balsamic_analysis.py
+-rw-r--r--   0        0        0     1050 2024-04-29 07:50:37.641872 cg-60.4.7/tests/models/conftest.py
+-rw-r--r--   0        0        0        0 2024-04-29 07:50:37.641872 cg-60.4.7/tests/models/demultiplexing/__init__.py
+-rw-r--r--   0        0        0    11723 2024-04-29 07:50:37.641872 cg-60.4.7/tests/models/demultiplexing/test_run_parameters.py
+-rw-r--r--   0        0        0        0 2024-04-29 07:50:37.641872 cg-60.4.7/tests/models/downsample/__init__.py
+-rw-r--r--   0        0        0     2096 2024-04-29 07:50:37.641872 cg-60.4.7/tests/models/downsample/test_down_sample_meta_data.py
+-rw-r--r--   0        0        0        0 2024-04-29 07:50:37.641872 cg-60.4.7/tests/models/flow_cell/__init__.py
+-rw-r--r--   0        0        0     6723 2024-04-29 07:50:37.641872 cg-60.4.7/tests/models/flow_cell/test_flowcell_model.py
+-rw-r--r--   0        0        0     6637 2024-04-29 07:50:37.641872 cg-60.4.7/tests/models/mip/conftest.py
+-rw-r--r--   0        0        0     1239 2024-04-29 07:50:37.641872 cg-60.4.7/tests/models/mip/test_mip_analysis.py
+-rw-r--r--   0        0        0     2348 2024-04-29 07:50:37.641872 cg-60.4.7/tests/models/mip/test_mip_config.py
+-rw-r--r--   0        0        0     6392 2024-04-29 07:50:37.641872 cg-60.4.7/tests/models/mip/test_mip_metrics_deliverables.py
+-rw-r--r--   0        0        0     3959 2024-04-29 07:50:37.641872 cg-60.4.7/tests/models/mip/test_mip_sample_info.py
+-rw-r--r--   0        0        0     3314 2024-04-29 07:50:37.641872 cg-60.4.7/tests/models/nextflow/test_nextflow_deliver.py
+-rw-r--r--   0        0        0     1602 2024-04-29 07:50:37.641872 cg-60.4.7/tests/models/observations/conftest.py
+-rw-r--r--   0        0        0     2579 2024-04-29 07:50:37.641872 cg-60.4.7/tests/models/observations/test_observations_input_files.py
+-rw-r--r--   0        0        0        0 2024-04-29 07:50:37.641872 cg-60.4.7/tests/models/report/__init__.py
+-rw-r--r--   0        0        0     7327 2024-04-29 07:50:37.641872 cg-60.4.7/tests/models/report/test_validators.py
+-rw-r--r--   0        0        0     3855 2024-04-29 07:50:37.641872 cg-60.4.7/tests/models/rnafusion/test_rnafusion_sample.py
+-rw-r--r--   0        0        0     1374 2024-04-29 07:50:37.641872 cg-60.4.7/tests/models/test_cg_models.py
+-rw-r--r--   0        0        0      990 2024-04-29 07:50:37.641872 cg-60.4.7/tests/models/test_compression_data.py
+-rw-r--r--   0        0        0      729 2024-04-29 07:50:37.641872 cg-60.4.7/tests/models/test_fastq.py
+-rw-r--r--   0        0        0     2860 2024-04-29 07:50:37.641872 cg-60.4.7/tests/models/test_file_data.py
+-rw-r--r--   0        0        0     4539 2024-04-29 07:50:37.641872 cg-60.4.7/tests/server/conftest.py
+-rw-r--r--   0        0        0     3135 2024-04-29 07:50:37.641872 cg-60.4.7/tests/server/endpoints/test_delivery_message_endpoint.py
+-rw-r--r--   0        0        0     3239 2024-04-29 07:50:37.641872 cg-60.4.7/tests/server/endpoints/test_orders_endpoint.py
+-rw-r--r--   0        0        0      271 2024-04-29 07:50:37.641872 cg-60.4.7/tests/server/test_server_auto.py
+-rw-r--r--   0        0        0     1047 2024-04-29 07:50:37.641872 cg-60.4.7/tests/services/fastq_file_service/conftest.py
+-rw-r--r--   0        0        0     3634 2024-04-29 07:50:37.641872 cg-60.4.7/tests/services/fastq_file_service/test_fastq_file_service.py
+-rw-r--r--   0        0        0     4861 2024-04-29 07:50:37.641872 cg-60.4.7/tests/services/orders/order_status_service/conftest.py
+-rw-r--r--   0        0        0     2865 2024-04-29 07:50:37.641872 cg-60.4.7/tests/services/orders/order_status_service/test_order_summary_service.py
+-rw-r--r--   0        0        0     9595 2024-04-29 07:50:37.641872 cg-60.4.7/tests/services/quality_controller/test_sequencing_quality_checks_utils.py
+-rw-r--r--   0        0        0      318 2024-04-29 07:50:37.641872 cg-60.4.7/tests/small_helpers.py
+-rw-r--r--   0        0        0        0 2024-04-29 07:50:37.641872 cg-60.4.7/tests/store/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-29 07:50:37.641872 cg-60.4.7/tests/store/api/__init__.py
+-rw-r--r--   0        0        0     3032 2024-04-29 07:50:37.641872 cg-60.4.7/tests/store/api/conftest.py
+-rw-r--r--   0        0        0     1557 2024-04-29 07:50:37.641872 cg-60.4.7/tests/store/api/test_base.py
+-rw-r--r--   0        0        0    20096 2024-04-29 07:50:37.641872 cg-60.4.7/tests/store/conftest.py
+-rw-r--r--   0        0        0        0 2024-04-29 07:50:37.641872 cg-60.4.7/tests/store/crud/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-29 07:50:37.641872 cg-60.4.7/tests/store/crud/add/__init__.py
+-rw-r--r--   0        0        0     1497 2024-04-29 07:50:37.641872 cg-60.4.7/tests/store/crud/add/test_store_add_application_version.py
+-rw-r--r--   0        0        0     3958 2024-04-29 07:50:37.641872 cg-60.4.7/tests/store/crud/add/test_store_add_base.py
+-rw-r--r--   0        0        0     2502 2024-04-29 07:50:37.641872 cg-60.4.7/tests/store/crud/add/test_store_add_customer.py
+-rw-r--r--   0        0        0     1704 2024-04-29 07:50:37.641872 cg-60.4.7/tests/store/crud/add/test_store_add_flow_celll.py
+-rw-r--r--   0        0        0    12290 2024-04-29 07:50:37.641872 cg-60.4.7/tests/store/crud/conftest.py
+-rw-r--r--   0        0        0        0 2024-04-29 07:50:37.641872 cg-60.4.7/tests/store/crud/delete/__init__.py
+-rw-r--r--   0        0        0     5611 2024-04-29 07:50:37.641872 cg-60.4.7/tests/store/crud/delete/test_delete.py
+-rw-r--r--   0        0        0        0 2024-04-29 07:50:37.641872 cg-60.4.7/tests/store/crud/read/__init__.py
+-rw-r--r--   0        0        0    56073 2024-04-29 07:50:37.641872 cg-60.4.7/tests/store/crud/read/test_read.py
+-rw-r--r--   0        0        0     5461 2024-04-29 07:50:37.641872 cg-60.4.7/tests/store/crud/read/test_read_analyses_to_clean.py
+-rw-r--r--   0        0        0     3553 2024-04-29 07:50:37.641872 cg-60.4.7/tests/store/crud/read/test_read_analyses_to_delivery_report.py
+-rw-r--r--   0        0        0    17328 2024-04-29 07:50:37.641872 cg-60.4.7/tests/store/crud/read/test_read_analysis.py
+-rw-r--r--   0        0        0     2743 2024-04-29 07:50:37.641872 cg-60.4.7/tests/store/crud/read/test_read_application_version.py
+-rw-r--r--   0        0        0     1105 2024-04-29 07:50:37.641872 cg-60.4.7/tests/store/crud/read/test_read_customer.py
+-rw-r--r--   0        0        0     1530 2024-04-29 07:50:37.641872 cg-60.4.7/tests/store/crud/read/test_read_pool.py
+-rw-r--r--   0        0        0    21503 2024-04-29 07:50:37.641872 cg-60.4.7/tests/store/crud/read/test_read_sample.py
+-rw-r--r--   0        0        0        0 2024-04-29 07:50:37.641872 cg-60.4.7/tests/store/crud/update/__init__.py
+-rw-r--r--   0        0        0      737 2024-04-29 07:50:37.641872 cg-60.4.7/tests/store/crud/update/test_update.py
+-rw-r--r--   0        0        0    11693 2024-04-29 07:50:37.641872 cg-60.4.7/tests/store/filters/test_status_analyses_filters.py
+-rw-r--r--   0        0        0     3397 2024-04-29 07:50:37.641872 cg-60.4.7/tests/store/filters/test_status_application_filters.py
+-rw-r--r--   0        0        0     2073 2024-04-29 07:50:37.645872 cg-60.4.7/tests/store/filters/test_status_application_limitations_filters.py
+-rw-r--r--   0        0        0    10452 2024-04-29 07:50:37.645872 cg-60.4.7/tests/store/filters/test_status_application_version_filters.py
+-rw-r--r--   0        0        0     2804 2024-04-29 07:50:37.645872 cg-60.4.7/tests/store/filters/test_status_bed_filters.py
+-rw-r--r--   0        0        0     2362 2024-04-29 07:50:37.645872 cg-60.4.7/tests/store/filters/test_status_bed_version_filters.py
+-rw-r--r--   0        0        0     3495 2024-04-29 07:50:37.645872 cg-60.4.7/tests/store/filters/test_status_case_sample_filters.py
+-rw-r--r--   0        0        0    39100 2024-04-29 07:50:37.645872 cg-60.4.7/tests/store/filters/test_status_cases_filters.py
+-rw-r--r--   0        0        0     1345 2024-04-29 07:50:37.645872 cg-60.4.7/tests/store/filters/test_status_collaboration_filters.py
+-rw-r--r--   0        0        0     2482 2024-04-29 07:50:37.645872 cg-60.4.7/tests/store/filters/test_status_customer_filters.py
+-rw-r--r--   0        0        0     5153 2024-04-29 07:50:37.645872 cg-60.4.7/tests/store/filters/test_status_flow_cell_filters.py
+-rw-r--r--   0        0        0     2226 2024-04-29 07:50:37.645872 cg-60.4.7/tests/store/filters/test_status_invoice_filters.py
+-rw-r--r--   0        0        0     5871 2024-04-29 07:50:37.645872 cg-60.4.7/tests/store/filters/test_status_metrics_filters.py
+-rw-r--r--   0        0        0     2404 2024-04-29 07:50:37.645872 cg-60.4.7/tests/store/filters/test_status_organism_filters.py
+-rw-r--r--   0        0        0     1804 2024-04-29 07:50:37.645872 cg-60.4.7/tests/store/filters/test_status_panel_filters.py
+-rw-r--r--   0        0        0     8720 2024-04-29 07:50:37.645872 cg-60.4.7/tests/store/filters/test_status_pool_filters.py
+-rw-r--r--   0        0        0    22875 2024-04-29 07:50:37.645872 cg-60.4.7/tests/store/filters/test_status_samples_filters.py
+-rw-r--r--   0        0        0     1576 2024-04-29 07:50:37.645872 cg-60.4.7/tests/store/filters/test_status_user_filters.py
+-rw-r--r--   0        0        0     2147 2024-04-29 07:50:37.645872 cg-60.4.7/tests/store/test_delivery.py
+-rw-r--r--   0        0        0     4127 2024-04-29 07:50:37.645872 cg-60.4.7/tests/store/test_store_models.py
+-rw-r--r--   0        0        0    37125 2024-04-29 07:50:37.645872 cg-60.4.7/tests/store_helpers.py
+-rw-r--r--   0        0        0     4988 2024-04-29 07:50:37.645872 cg-60.4.7/tests/test_copy_novaseqx_flow_cell.py
+-rw-r--r--   0        0        0      911 2024-04-29 07:50:37.645872 cg-60.4.7/tests/test_store_helpers.py
+-rw-r--r--   0        0        0        0 2024-04-29 07:50:37.645872 cg-60.4.7/tests/utils/__init__.py
+-rw-r--r--   0        0        0     1754 2024-04-29 07:50:37.645872 cg-60.4.7/tests/utils/conftest.py
+-rw-r--r--   0        0        0      371 2024-04-29 07:50:37.645872 cg-60.4.7/tests/utils/test_calculations.py
+-rw-r--r--   0        0        0     2920 2024-04-29 07:50:37.645872 cg-60.4.7/tests/utils/test_commands.py
+-rw-r--r--   0        0        0      953 2024-04-29 07:50:37.645872 cg-60.4.7/tests/utils/test_date.py
+-rw-r--r--   0        0        0     1508 2024-04-29 07:50:37.645872 cg-60.4.7/tests/utils/test_dict.py
+-rw-r--r--   0        0        0     7154 2024-04-29 07:50:37.645872 cg-60.4.7/tests/utils/test_dispatcher.py
+-rw-r--r--   0        0        0     4100 2024-04-29 07:50:37.645872 cg-60.4.7/tests/utils/test_files.py
+-rw-r--r--   0        0        0     1170 2024-04-29 07:50:37.645872 cg-60.4.7/tests/utils/test_time.py
+-rw-r--r--   0        0        0     2366 2024-04-29 07:50:37.645872 cg-60.4.7/tests/utils/test_utils.py
+-rw-r--r--   0        0        0     4369 1970-01-01 00:00:00.000000 cg-60.4.7/PKG-INFO
```

### Comparing `cg-60.4.6/README.md` & `cg-60.4.7/README.md`

 * *Files identical despite different names*

### Comparing `cg-60.4.6/cg/apps/coverage/api.py` & `cg-60.4.7/cg/apps/coverage/api.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.6/cg/apps/crunchy/crunchy.py` & `cg-60.4.7/cg/apps/crunchy/crunchy.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.6/cg/apps/crunchy/files.py` & `cg-60.4.7/cg/apps/crunchy/files.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.6/cg/apps/crunchy/sbatch.py` & `cg-60.4.7/cg/apps/crunchy/sbatch.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.6/cg/apps/demultiplex/demultiplex_api.py` & `cg-60.4.7/cg/apps/demultiplex/demultiplex_api.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.6/cg/apps/demultiplex/sample_sheet/api.py` & `cg-60.4.7/cg/apps/demultiplex/sample_sheet/api.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.6/cg/apps/demultiplex/sample_sheet/index.py` & `cg-60.4.7/cg/apps/demultiplex/sample_sheet/index.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.6/cg/apps/demultiplex/sample_sheet/override_cycles_validator.py` & `cg-60.4.7/cg/apps/demultiplex/sample_sheet/override_cycles_validator.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.6/cg/apps/demultiplex/sample_sheet/read_sample_sheet.py` & `cg-60.4.7/cg/apps/demultiplex/sample_sheet/read_sample_sheet.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.6/cg/apps/demultiplex/sample_sheet/sample_models.py` & `cg-60.4.7/cg/apps/demultiplex/sample_sheet/sample_models.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.6/cg/apps/demultiplex/sample_sheet/sample_sheet_creator.py` & `cg-60.4.7/cg/apps/demultiplex/sample_sheet/sample_sheet_creator.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.6/cg/apps/demultiplex/sample_sheet/sample_sheet_models.py` & `cg-60.4.7/cg/apps/demultiplex/sample_sheet/sample_sheet_models.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.6/cg/apps/demultiplex/sample_sheet/sample_sheet_validator.py` & `cg-60.4.7/cg/apps/demultiplex/sample_sheet/sample_sheet_validator.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.6/cg/apps/demultiplex/sample_sheet/validators.py` & `cg-60.4.7/cg/apps/demultiplex/sample_sheet/validators.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.6/cg/apps/demultiplex/sbatch.py` & `cg-60.4.7/cg/apps/demultiplex/sbatch.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.6/cg/apps/downsample/downsample.py` & `cg-60.4.7/cg/apps/downsample/downsample.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.6/cg/apps/downsample/utils.py` & `cg-60.4.7/cg/apps/downsample/utils.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.6/cg/apps/gens.py` & `cg-60.4.7/cg/apps/gens.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.6/cg/apps/gt.py` & `cg-60.4.7/cg/apps/gt.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.6/cg/apps/hermes/hermes_api.py` & `cg-60.4.7/cg/apps/hermes/hermes_api.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.6/cg/apps/hermes/models.py` & `cg-60.4.7/cg/apps/hermes/models.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.6/cg/apps/housekeeper/hk.py` & `cg-60.4.7/cg/apps/housekeeper/hk.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.6/cg/apps/invoice/render.py` & `cg-60.4.7/cg/apps/invoice/render.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.6/cg/apps/invoice/templates/KI_pool_invoice.xlsx` & `cg-60.4.7/cg/apps/invoice/templates/KI_pool_invoice.xlsx`

 * *Files identical despite different names*

### Comparing `cg-60.4.6/cg/apps/invoice/templates/KI_sample_invoice.xlsx` & `cg-60.4.7/cg/apps/invoice/templates/KI_sample_invoice.xlsx`

 * *Files identical despite different names*

### Comparing `cg-60.4.6/cg/apps/invoice/templates/KTH_pool_invoice.xlsx` & `cg-60.4.7/cg/apps/invoice/templates/KTH_pool_invoice.xlsx`

 * *Files identical despite different names*

### Comparing `cg-60.4.6/cg/apps/invoice/templates/KTH_sample_invoice.xlsx` & `cg-60.4.7/cg/apps/invoice/templates/KTH_sample_invoice.xlsx`

 * *Files identical despite different names*

### Comparing `cg-60.4.6/cg/apps/lims/api.py` & `cg-60.4.7/cg/apps/lims/api.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.6/cg/apps/lims/batch.py` & `cg-60.4.7/cg/apps/lims/batch.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.6/cg/apps/lims/order.py` & `cg-60.4.7/cg/apps/lims/order.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.6/cg/apps/lims/sample_sheet.py` & `cg-60.4.7/cg/apps/lims/sample_sheet.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.6/cg/apps/loqus.py` & `cg-60.4.7/cg/apps/loqus.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.6/cg/apps/madeline/api.py` & `cg-60.4.7/cg/apps/madeline/api.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.6/cg/apps/mip/confighandler.py` & `cg-60.4.7/cg/apps/mip/confighandler.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.6/cg/apps/mutacc_auto.py` & `cg-60.4.7/cg/apps/mutacc_auto.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.6/cg/apps/orderform/excel_orderform_parser.py` & `cg-60.4.7/cg/apps/orderform/excel_orderform_parser.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.6/cg/apps/orderform/json_orderform_parser.py` & `cg-60.4.7/cg/apps/orderform/json_orderform_parser.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.6/cg/apps/orderform/orderform_parser.py` & `cg-60.4.7/cg/apps/orderform/orderform_parser.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.6/cg/apps/osticket.py` & `cg-60.4.7/cg/apps/osticket.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.6/cg/apps/scout/scout_export.py` & `cg-60.4.7/cg/apps/scout/scout_export.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.6/cg/apps/scout/scoutapi.py` & `cg-60.4.7/cg/apps/scout/scoutapi.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.6/cg/apps/sequencing_metrics_parser/api.py` & `cg-60.4.7/cg/apps/sequencing_metrics_parser/api.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.6/cg/apps/sequencing_metrics_parser/models.py` & `cg-60.4.7/cg/apps/sequencing_metrics_parser/models.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.6/cg/apps/sequencing_metrics_parser/parser.py` & `cg-60.4.7/cg/apps/sequencing_metrics_parser/parser.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.6/cg/apps/slurm/sbatch.py` & `cg-60.4.7/cg/apps/slurm/sbatch.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.6/cg/apps/slurm/slurm_api.py` & `cg-60.4.7/cg/apps/slurm/slurm_api.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.6/cg/apps/tb/api.py` & `cg-60.4.7/cg/apps/tb/api.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.6/cg/apps/tb/models.py` & `cg-60.4.7/cg/apps/tb/models.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.6/cg/cli/add.py` & `cg-60.4.7/cg/cli/add.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.6/cg/cli/archive.py` & `cg-60.4.7/cg/cli/archive.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.6/cg/cli/backup.py` & `cg-60.4.7/cg/cli/backup.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.6/cg/cli/base.py` & `cg-60.4.7/cg/cli/base.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.6/cg/cli/clean.py` & `cg-60.4.7/cg/cli/clean.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.6/cg/cli/compress/base.py` & `cg-60.4.7/cg/cli/compress/base.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.6/cg/cli/compress/fastq.py` & `cg-60.4.7/cg/cli/compress/fastq.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.6/cg/cli/compress/helpers.py` & `cg-60.4.7/cg/cli/compress/helpers.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.6/cg/cli/delete/base.py` & `cg-60.4.7/cg/cli/delete/base.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.6/cg/cli/delete/case.py` & `cg-60.4.7/cg/cli/delete/case.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.6/cg/cli/delete/cases.py` & `cg-60.4.7/cg/cli/delete/cases.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.6/cg/cli/delete/observations.py` & `cg-60.4.7/cg/cli/delete/observations.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.6/cg/cli/deliver/base.py` & `cg-60.4.7/cg/cli/deliver/base.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.6/cg/cli/demultiplex/base.py` & `cg-60.4.7/cg/cli/demultiplex/base.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.6/cg/cli/demultiplex/copy_novaseqx_demultiplex_data.py` & `cg-60.4.7/cg/cli/demultiplex/copy_novaseqx_demultiplex_data.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.6/cg/cli/demultiplex/demux.py` & `cg-60.4.7/cg/cli/demultiplex/demux.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.6/cg/cli/demultiplex/finish.py` & `cg-60.4.7/cg/cli/demultiplex/finish.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.6/cg/cli/demultiplex/sample_sheet.py` & `cg-60.4.7/cg/cli/demultiplex/sample_sheet.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.6/cg/cli/downsample.py` & `cg-60.4.7/cg/cli/downsample.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.6/cg/cli/generate/report/base.py` & `cg-60.4.7/cg/cli/generate/report/base.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.6/cg/cli/generate/report/options.py` & `cg-60.4.7/cg/cli/generate/report/options.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.6/cg/cli/generate/report/utils.py` & `cg-60.4.7/cg/cli/generate/report/utils.py`

 * *Files 3% similar despite different names*

```diff
@@ -12,20 +12,22 @@
 )
 from cg.meta.report.balsamic import BalsamicReportAPI
 from cg.meta.report.balsamic_qc import BalsamicQCReportAPI
 from cg.meta.report.balsamic_umi import BalsamicUmiReportAPI
 from cg.meta.report.mip_dna import MipDNAReportAPI
 from cg.meta.report.report_api import ReportAPI
 from cg.meta.report.rnafusion import RnafusionReportAPI
+from cg.meta.report.taxprofiler import TaxprofilerReportAPI
 from cg.meta.report.tomte import TomteReportAPI
 from cg.meta.workflow.balsamic import BalsamicAnalysisAPI
 from cg.meta.workflow.balsamic_qc import BalsamicQCAnalysisAPI
 from cg.meta.workflow.balsamic_umi import BalsamicUmiAnalysisAPI
 from cg.meta.workflow.mip_dna import MipDNAAnalysisAPI
 from cg.meta.workflow.rnafusion import RnafusionAnalysisAPI
+from cg.meta.workflow.taxprofiler import TaxprofilerAnalysisAPI
 from cg.meta.workflow.tomte import TomteAnalysisAPI
 from cg.store.models import Case
 
 LOG = logging.getLogger(__name__)
 
 
 def get_report_case(context: click.Context, case_id: str) -> Case:
@@ -95,14 +97,17 @@
         ),
         Workflow.MIP_DNA: MipDNAReportAPI(
             config=context.obj, analysis_api=MipDNAAnalysisAPI(config=context.obj)
         ),
         Workflow.RNAFUSION: RnafusionReportAPI(
             config=context.obj, analysis_api=RnafusionAnalysisAPI(config=context.obj)
         ),
+        Workflow.TAXPROFILER: TaxprofilerReportAPI(
+            config=context.obj, analysis_api=TaxprofilerAnalysisAPI(config=context.obj)
+        ),
         Workflow.TOMTE: TomteReportAPI(
             config=context.obj, analysis_api=TomteAnalysisAPI(config=context.obj)
         ),
     }
     return dispatch_report_api.get(workflow)
```

### Comparing `cg-60.4.6/cg/cli/get.py` & `cg-60.4.7/cg/cli/get.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.6/cg/cli/set/base.py` & `cg-60.4.7/cg/cli/set/base.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.6/cg/cli/set/case.py` & `cg-60.4.7/cg/cli/set/case.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.6/cg/cli/set/cases.py` & `cg-60.4.7/cg/cli/set/cases.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.6/cg/cli/store/base.py` & `cg-60.4.7/cg/cli/store/base.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.6/cg/cli/store/store.py` & `cg-60.4.7/cg/cli/store/store.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.6/cg/cli/transfer.py` & `cg-60.4.7/cg/cli/transfer.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.6/cg/cli/upload/base.py` & `cg-60.4.7/cg/cli/upload/base.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.6/cg/cli/upload/clinical_delivery.py` & `cg-60.4.7/cg/cli/upload/clinical_delivery.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.6/cg/cli/upload/coverage.py` & `cg-60.4.7/cg/cli/upload/coverage.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.6/cg/cli/upload/delivery_report.py` & `cg-60.4.7/cg/cli/upload/delivery_report.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.6/cg/cli/upload/fohm.py` & `cg-60.4.7/cg/cli/upload/fohm.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.6/cg/cli/upload/genotype.py` & `cg-60.4.7/cg/cli/upload/genotype.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.6/cg/cli/upload/gens.py` & `cg-60.4.7/cg/cli/upload/gens.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.6/cg/cli/upload/gisaid.py` & `cg-60.4.7/cg/cli/upload/gisaid.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.6/cg/cli/upload/mutacc.py` & `cg-60.4.7/cg/cli/upload/mutacc.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.6/cg/cli/upload/nipt/base.py` & `cg-60.4.7/cg/cli/upload/nipt/base.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.6/cg/cli/upload/nipt/ftp.py` & `cg-60.4.7/cg/cli/upload/nipt/ftp.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.6/cg/cli/upload/nipt/statina.py` & `cg-60.4.7/cg/cli/upload/nipt/statina.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.6/cg/cli/upload/observations/observations.py` & `cg-60.4.7/cg/cli/upload/observations/observations.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.6/cg/cli/upload/observations/utils.py` & `cg-60.4.7/cg/cli/upload/observations/utils.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.6/cg/cli/upload/scout.py` & `cg-60.4.7/cg/cli/upload/scout.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.6/cg/cli/upload/utils.py` & `cg-60.4.7/cg/cli/upload/utils.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.6/cg/cli/upload/validate.py` & `cg-60.4.7/cg/cli/upload/validate.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.6/cg/cli/workflow/balsamic/base.py` & `cg-60.4.7/cg/cli/workflow/balsamic/base.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.6/cg/cli/workflow/balsamic/options.py` & `cg-60.4.7/cg/cli/workflow/balsamic/options.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.6/cg/cli/workflow/balsamic/pon.py` & `cg-60.4.7/cg/cli/workflow/balsamic/pon.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.6/cg/cli/workflow/balsamic/qc.py` & `cg-60.4.7/cg/cli/workflow/balsamic/qc.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.6/cg/cli/workflow/balsamic/umi.py` & `cg-60.4.7/cg/cli/workflow/balsamic/umi.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.6/cg/cli/workflow/base.py` & `cg-60.4.7/cg/cli/workflow/base.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.6/cg/cli/workflow/commands.py` & `cg-60.4.7/cg/cli/workflow/commands.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.6/cg/cli/workflow/fastq/base.py` & `cg-60.4.7/cg/cli/workflow/fastq/base.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.6/cg/cli/workflow/fastq/fastq_service.py` & `cg-60.4.7/cg/cli/workflow/fastq/fastq_service.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.6/cg/cli/workflow/fluffy/base.py` & `cg-60.4.7/cg/cli/workflow/fluffy/base.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.6/cg/cli/workflow/jasen/base.py` & `cg-60.4.7/cg/cli/workflow/jasen/base.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.6/cg/cli/workflow/microsalt/base.py` & `cg-60.4.7/cg/cli/workflow/microsalt/base.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.6/cg/cli/workflow/mip/base.py` & `cg-60.4.7/cg/cli/workflow/mip/base.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.6/cg/cli/workflow/mip/options.py` & `cg-60.4.7/cg/cli/workflow/mip/options.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.6/cg/cli/workflow/mip_dna/base.py` & `cg-60.4.7/cg/cli/workflow/mip_dna/base.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.6/cg/cli/workflow/mip_rna/base.py` & `cg-60.4.7/cg/cli/workflow/mip_rna/base.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.6/cg/cli/workflow/mutant/base.py` & `cg-60.4.7/cg/cli/workflow/mutant/base.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.6/cg/cli/workflow/nf_analysis.py` & `cg-60.4.7/cg/cli/workflow/nf_analysis.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.6/cg/cli/workflow/raredisease/base.py` & `cg-60.4.7/cg/cli/workflow/raredisease/base.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.6/cg/cli/workflow/rnafusion/base.py` & `cg-60.4.7/cg/cli/workflow/rnafusion/base.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.6/cg/cli/workflow/taxprofiler/base.py` & `cg-60.4.7/cg/cli/workflow/taxprofiler/base.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.6/cg/cli/workflow/tomte/base.py` & `cg-60.4.7/cg/cli/workflow/tomte/base.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.6/cg/clients/arnold/api.py` & `cg-60.4.7/cg/clients/arnold/api.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.6/cg/clients/janus/api.py` & `cg-60.4.7/cg/clients/janus/api.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.6/cg/constants/__init__.py` & `cg-60.4.7/cg/constants/__init__.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.6/cg/constants/bcl_convert_metrics.py` & `cg-60.4.7/cg/constants/bcl_convert_metrics.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.6/cg/constants/constants.py` & `cg-60.4.7/cg/constants/constants.py`

 * *Files 0% similar despite different names*

```diff
@@ -151,14 +151,15 @@
     YAML: str = "yaml"
 
 
 class GenomeVersion(StrEnum):
     hg19: str = "hg19"
     hg38: str = "hg38"
     canfam3: str = "canfam3"
+    T2T_CHM13: str = "T2T-CHM13v2.0"
 
 
 class SampleType(StrEnum):
     TUMOR: str = "tumor"
     NORMAL: str = "normal"
```

### Comparing `cg-60.4.6/cg/constants/delivery.py` & `cg-60.4.7/cg/constants/delivery.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.6/cg/constants/demultiplexing.py` & `cg-60.4.7/cg/constants/demultiplexing.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.6/cg/constants/encryption.py` & `cg-60.4.7/cg/constants/encryption.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.6/cg/constants/gene_panel.py` & `cg-60.4.7/cg/constants/gene_panel.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.6/cg/constants/housekeeper_tags.py` & `cg-60.4.7/cg/constants/housekeeper_tags.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.6/cg/constants/lims.py` & `cg-60.4.7/cg/constants/lims.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.6/cg/constants/metrics.py` & `cg-60.4.7/cg/constants/metrics.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.6/cg/constants/nextflow.py` & `cg-60.4.7/cg/constants/nextflow.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.6/cg/constants/nf_analysis.py` & `cg-60.4.7/cg/constants/nf_analysis.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.6/cg/constants/observations.py` & `cg-60.4.7/cg/constants/observations.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.6/cg/constants/orderforms.py` & `cg-60.4.7/cg/constants/orderforms.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.6/cg/constants/priority.py` & `cg-60.4.7/cg/constants/priority.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.6/cg/constants/report.py` & `cg-60.4.7/cg/constants/report.py`

 * *Files 4% similar despite different names*

```diff
@@ -18,14 +18,15 @@
 
 REPORT_SUPPORTED_WORKFLOW: tuple[Workflow, ...] = (
     Workflow.BALSAMIC,
     Workflow.BALSAMIC_QC,
     Workflow.BALSAMIC_UMI,
     Workflow.MIP_DNA,
     Workflow.RNAFUSION,
+    Workflow.TAXPROFILER,
     Workflow.TOMTE,
 )
 
 REPORT_SUPPORTED_DATA_DELIVERY: tuple[DataDelivery, ...] = (
     DataDelivery.ANALYSIS_FILES,
     DataDelivery.ANALYSIS_SCOUT,
     DataDelivery.FASTQ_ANALYSIS,
@@ -98,14 +99,16 @@
 REQUIRED_DATA_ANALYSIS_BALSAMIC_FIELDS: list[str] = REQUIRED_DATA_ANALYSIS_FIELDS + [
     "type",
     "variant_callers",
 ]
 
 REQUIRED_DATA_ANALYSIS_RNAFUSION_FIELDS: list[str] = REQUIRED_DATA_ANALYSIS_FIELDS
 
+REQUIRED_DATA_ANALYSIS_TAXPROFILER_FIELDS: list[str] = REQUIRED_DATA_ANALYSIS_FIELDS
+
 REQUIRED_DATA_ANALYSIS_TOMTE_FIELDS: list[str] = REQUIRED_DATA_ANALYSIS_FIELDS
 
 # Sample required fields
 _REQUIRED_SAMPLE_FIELDS: list[str] = [
     "name",
     "id",
     "ticket",
@@ -127,14 +130,16 @@
 
 REQUIRED_SAMPLE_MIP_DNA_FIELDS: list[str] = _REQUIRED_SAMPLE_RARE_DISEASE_FIELDS
 
 REQUIRED_SAMPLE_BALSAMIC_FIELDS: list[str] = _REQUIRED_SAMPLE_CANCER_FIELDS
 
 REQUIRED_SAMPLE_RNAFUSION_FIELDS: list[str] = _REQUIRED_SAMPLE_CANCER_FIELDS
 
+REQUIRED_SAMPLE_TAXPROFILER_FIELDS: list[str] = _REQUIRED_SAMPLE_FIELDS
+
 REQUIRED_SAMPLE_TOMTE_FIELDS: list[str] = _REQUIRED_SAMPLE_RARE_DISEASE_FIELDS
 
 # Methods required fields (OPTIONAL: "library_prep", "sequencing")
 REQUIRED_SAMPLE_METHODS_FIELDS: list[str] = []
 
 # Timestamp required fields (OPTIONAL: "prepared_at", "reads_updated_at")
 REQUIRED_SAMPLE_TIMESTAMP_FIELDS: list[str] = [
@@ -188,31 +193,45 @@
 REQUIRED_SAMPLE_METADATA_BALSAMIC_TN_WGS_FIELDS: list[str] = (
     REQUIRED_SAMPLE_METADATA_BALSAMIC_TO_WGS_FIELDS
     + [
         "pct_15x",
     ]
 )
 
-_REQUIRED_SAMPLE_METADATA_WTS_FIELDS: list[str] = _REQUIRED_SAMPLE_METADATA_FIELDS + [
-    "bias_5_3",
+_REQUIRED_SAMPLE_METADATA_SEQUENCING_FIELDS: list[str] = _REQUIRED_SAMPLE_METADATA_FIELDS + [
     "gc_content",
     "input_amount",
     "mean_length_r1",
+    "rin",
+]
+
+_REQUIRED_SAMPLE_METADATA_WTS_FIELDS: list[str] = _REQUIRED_SAMPLE_METADATA_SEQUENCING_FIELDS + [
+    "bias_5_3",
     "mrna_bases",
     "pct_adapter",
     "pct_surviving",
     "q20_rate",
     "q30_rate",
     "ribosomal_bases",
-    "rin",
     "uniquely_mapped_reads",
 ]
 
 REQUIRED_SAMPLE_METADATA_RNAFUSION_FIELDS: list[str] = _REQUIRED_SAMPLE_METADATA_WTS_FIELDS + [
     "mapped_reads",
 ]
 
 
+REQUIRED_SAMPLE_METADATA_TAXPROFILER_FIELDS: list[str] = (
+    _REQUIRED_SAMPLE_METADATA_SEQUENCING_FIELDS
+    + [
+        "average_read_length",
+        "mapped_reads",
+        "mean_length_r2",
+        "million_read_pairs_after_filtering",
+    ]
+)
+
+
 REQUIRED_SAMPLE_METADATA_TOMTE_FIELDS: list[str] = _REQUIRED_SAMPLE_METADATA_WTS_FIELDS + [
     "pct_intergenic_bases",
     "pct_intronic_bases",
 ]
```

### Comparing `cg-60.4.6/cg/constants/sample_sources.py` & `cg-60.4.7/cg/constants/sample_sources.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.6/cg/constants/scout.py` & `cg-60.4.7/cg/constants/scout.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.6/cg/constants/sequencing.py` & `cg-60.4.7/cg/constants/sequencing.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.6/cg/constants/subject.py` & `cg-60.4.7/cg/constants/subject.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.6/cg/exc.py` & `cg-60.4.7/cg/exc.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.6/cg/io/api.py` & `cg-60.4.7/cg/io/api.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.6/cg/io/config.py` & `cg-60.4.7/cg/io/config.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.6/cg/io/controller.py` & `cg-60.4.7/cg/io/controller.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.6/cg/io/csv.py` & `cg-60.4.7/cg/io/csv.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.6/cg/io/json.py` & `cg-60.4.7/cg/io/json.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.6/cg/io/png.py` & `cg-60.4.7/cg/io/png.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.6/cg/io/txt.py` & `cg-60.4.7/cg/io/txt.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.6/cg/io/validate_path.py` & `cg-60.4.7/cg/io/validate_path.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.6/cg/io/xml.py` & `cg-60.4.7/cg/io/xml.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.6/cg/io/yaml.py` & `cg-60.4.7/cg/io/yaml.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.6/cg/meta/archive/archive.py` & `cg-60.4.7/cg/meta/archive/archive.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.6/cg/meta/archive/ddn/constants.py` & `cg-60.4.7/cg/meta/archive/ddn/constants.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.6/cg/meta/archive/ddn/ddn_data_flow_client.py` & `cg-60.4.7/cg/meta/archive/ddn/ddn_data_flow_client.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.6/cg/meta/archive/ddn/models.py` & `cg-60.4.7/cg/meta/archive/ddn/models.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.6/cg/meta/archive/ddn/utils.py` & `cg-60.4.7/cg/meta/archive/ddn/utils.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.6/cg/meta/archive/models.py` & `cg-60.4.7/cg/meta/archive/models.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.6/cg/meta/backup/backup.py` & `cg-60.4.7/cg/meta/backup/backup.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.6/cg/meta/backup/pdc.py` & `cg-60.4.7/cg/meta/backup/pdc.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.6/cg/meta/clean/api.py` & `cg-60.4.7/cg/meta/clean/api.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.6/cg/meta/clean/clean_flow_cells.py` & `cg-60.4.7/cg/meta/clean/clean_flow_cells.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.6/cg/meta/clean/clean_retrieved_spring_files.py` & `cg-60.4.7/cg/meta/clean/clean_retrieved_spring_files.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.6/cg/meta/compress/compress.py` & `cg-60.4.7/cg/meta/compress/compress.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.6/cg/meta/compress/files.py` & `cg-60.4.7/cg/meta/compress/files.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.6/cg/meta/deliver/deliver.py` & `cg-60.4.7/cg/meta/deliver/deliver.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.6/cg/meta/deliver/deliver_ticket.py` & `cg-60.4.7/cg/meta/deliver/deliver_ticket.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.6/cg/meta/deliver/fastq_path_generator.py` & `cg-60.4.7/cg/meta/deliver/fastq_path_generator.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.6/cg/meta/delivery/delivery.py` & `cg-60.4.7/cg/meta/delivery/delivery.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.6/cg/meta/demultiplex/combine_sequencing_metrics.py` & `cg-60.4.7/cg/meta/demultiplex/combine_sequencing_metrics.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.6/cg/meta/demultiplex/demux_post_processing.py` & `cg-60.4.7/cg/meta/demultiplex/demux_post_processing.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.6/cg/meta/demultiplex/files.py` & `cg-60.4.7/cg/meta/demultiplex/files.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.6/cg/meta/demultiplex/housekeeper_storage_functions.py` & `cg-60.4.7/cg/meta/demultiplex/housekeeper_storage_functions.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.6/cg/meta/demultiplex/status_db_storage_functions.py` & `cg-60.4.7/cg/meta/demultiplex/status_db_storage_functions.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.6/cg/meta/demultiplex/utils.py` & `cg-60.4.7/cg/meta/demultiplex/utils.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.6/cg/meta/demultiplex/validation.py` & `cg-60.4.7/cg/meta/demultiplex/validation.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.6/cg/meta/encryption/encryption.py` & `cg-60.4.7/cg/meta/encryption/encryption.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.6/cg/meta/encryption/sbatch.py` & `cg-60.4.7/cg/meta/encryption/sbatch.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.6/cg/meta/invoice.py` & `cg-60.4.7/cg/meta/invoice.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.6/cg/meta/meta.py` & `cg-60.4.7/cg/meta/meta.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.6/cg/meta/observations/balsamic_observations_api.py` & `cg-60.4.7/cg/meta/observations/balsamic_observations_api.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.6/cg/meta/observations/mip_dna_observations_api.py` & `cg-60.4.7/cg/meta/observations/mip_dna_observations_api.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.6/cg/meta/observations/observations_api.py` & `cg-60.4.7/cg/meta/observations/observations_api.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.6/cg/meta/orders/api.py` & `cg-60.4.7/cg/meta/orders/api.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.6/cg/meta/orders/case_submitter.py` & `cg-60.4.7/cg/meta/orders/case_submitter.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.6/cg/meta/orders/fastq_submitter.py` & `cg-60.4.7/cg/meta/orders/fastq_submitter.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.6/cg/meta/orders/lims.py` & `cg-60.4.7/cg/meta/orders/lims.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.6/cg/meta/orders/metagenome_submitter.py` & `cg-60.4.7/cg/meta/orders/metagenome_submitter.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.6/cg/meta/orders/microbial_submitter.py` & `cg-60.4.7/cg/meta/orders/microbial_submitter.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.6/cg/meta/orders/pool_submitter.py` & `cg-60.4.7/cg/meta/orders/pool_submitter.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.6/cg/meta/orders/rnafusion_submitter.py` & `cg-60.4.7/cg/meta/orders/rnafusion_submitter.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.6/cg/meta/orders/sars_cov_2_submitter.py` & `cg-60.4.7/cg/meta/orders/sars_cov_2_submitter.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.6/cg/meta/orders/submitter.py` & `cg-60.4.7/cg/meta/orders/submitter.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.6/cg/meta/orders/ticket_handler.py` & `cg-60.4.7/cg/meta/orders/ticket_handler.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.6/cg/meta/qc_metrics/collect_qc_metrics.py` & `cg-60.4.7/cg/meta/qc_metrics/collect_qc_metrics.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.6/cg/meta/report/balsamic.py` & `cg-60.4.7/cg/meta/report/balsamic.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.6/cg/meta/report/balsamic_qc.py` & `cg-60.4.7/cg/meta/report/balsamic_qc.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.6/cg/meta/report/balsamic_umi.py` & `cg-60.4.7/cg/meta/report/balsamic_umi.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.6/cg/meta/report/field_validators.py` & `cg-60.4.7/cg/meta/report/field_validators.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.6/cg/meta/report/mip_dna.py` & `cg-60.4.7/cg/meta/report/mip_dna.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.6/cg/meta/report/report_api.py` & `cg-60.4.7/cg/meta/report/report_api.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.6/cg/meta/report/rnafusion.py` & `cg-60.4.7/cg/meta/report/rnafusion.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.6/cg/meta/report/templates/delivery-report.html` & `cg-60.4.7/cg/meta/report/templates/delivery-report.html`

 * *Files identical despite different names*

### Comparing `cg-60.4.6/cg/meta/report/templates/macros/data_analysis/data_analysis.html` & `cg-60.4.7/cg/meta/report/templates/macros/data_analysis/data_analysis.html`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 {% from "/macros/data_analysis/qc_metrics/balsamic_qc_metrics.html" import balsamic_qc_metrics %}
 {% from "/macros/data_analysis/qc_metrics/mip_dna_qc_metrics.html" import mip_dna_qc_metrics %}
 {% from "/macros/data_analysis/qc_metrics/rnafusion_qc_metrics.html" import rnafusion_qc_metrics %}
+{% from "/macros/data_analysis/qc_metrics/taxprofiler_qc_metrics.html" import taxprofiler_qc_metrics %}
 {% from "/macros/data_analysis/qc_metrics/tomte_qc_metrics.html" import tomte_qc_metrics %}
 {% from "/macros/data_analysis/limitations.html" import apptag_limitations %}
 
 {% macro data_analysis(case) %}
 {% set workflow = case.data_analysis.workflow %}
   <div class="container mb-5">
   <h3 class="mb-4">Analys</h3>
@@ -16,14 +17,17 @@
       {{ balsamic_qc_metrics(samples=case.samples, analysis_type=case.data_analysis.type) }}
     {% elif workflow == "mip-dna" %}
       <!-- MIP-DNA QC metrics -->
       {{ mip_dna_qc_metrics(samples=case.samples) }}
     {% elif workflow == "rnafusion" %}
       <!-- Rnafusion QC metrics -->
       {{ rnafusion_qc_metrics(samples=case.samples) }}
+    {% elif workflow == "taxprofiler" %}
+      <!-- Taxprofiler QC metrics -->
+      {{ taxprofiler_qc_metrics(samples=case.samples) }}
 	  {% elif workflow == "tomte" %}
       <!-- Tomte QC metrics -->
       {{ tomte_qc_metrics(samples=case.samples) }}
     {% endif %}
     <!-- Apptag limitations -->
     {{ apptag_limitations(applications=case.applications) }}
   </div>
@@ -76,14 +80,19 @@
         Inga fusionsvarianter upptäcktes.
       </div>
     {% endif %}
     <div class="alert alert-info" role="alert">
       Workflowinformation och bioinformatiska verktygsversioner:
       <a href="https://nf-co.re/rnafusion" class="alert-link">https://nf-co.re/rnafusion</a>.
     </div>
+	{% elif workflow == "taxprofiler" %}
+    <div class="alert alert-info" role="alert">
+      Workflowinformation och bioinformatiska verktygsversioner:
+      <a href="https://github.com/nf-core/taxprofiler" class="alert-link">https://github.com/nf-core/taxprofiler</a>.
+    </div>
   {% elif workflow == "tomte" %}
     <div class="alert alert-info" role="alert">
       Workflowinformation och bioinformatiska verktygsversioner:
       <a href="https://github.com/genomic-medicine-sweden/tomte" class="alert-link">https://github.com/genomic-medicine-sweden/tomte</a>.
     </div>
   {% endif %}
 {% endmacro %}
```

#### html2text {}

```diff
@@ -1,24 +1,26 @@
 {% from "/macros/data_analysis/qc_metrics/balsamic_qc_metrics.html" import
 balsamic_qc_metrics %} {% from "/macros/data_analysis/qc_metrics/
 mip_dna_qc_metrics.html" import mip_dna_qc_metrics %} {% from "/macros/
 data_analysis/qc_metrics/rnafusion_qc_metrics.html" import rnafusion_qc_metrics
-%} {% from "/macros/data_analysis/qc_metrics/tomte_qc_metrics.html" import
-tomte_qc_metrics %} {% from "/macros/data_analysis/limitations.html" import
-apptag_limitations %} {% macro data_analysis(case) %} {% set workflow =
-case.data_analysis.workflow %}
+%} {% from "/macros/data_analysis/qc_metrics/taxprofiler_qc_metrics.html"
+import taxprofiler_qc_metrics %} {% from "/macros/data_analysis/qc_metrics/
+tomte_qc_metrics.html" import tomte_qc_metrics %} {% from "/macros/
+data_analysis/limitations.html" import apptag_limitations %} {% macro
+data_analysis(case) %} {% set workflow = case.data_analysis.workflow %}
 ******** AAnnaallyyss ********
 {{ workflow_analysis(case=case) }}
 ****** KKvvaalliitteettsskkoonnttrroollllssmmeettrriikk ******
 {% if "balsamic" in workflow %} {{ balsamic_qc_metrics(samples=case.samples,
 analysis_type=case.data_analysis.type) }} {% elif workflow == "mip-dna" %} {
 { mip_dna_qc_metrics(samples=case.samples) }} {% elif workflow == "rnafusion"
-%} {{ rnafusion_qc_metrics(samples=case.samples) }} {% elif workflow == "tomte"
-%} {{ tomte_qc_metrics(samples=case.samples) }} {% endif %} {
-{ apptag_limitations(applications=case.applications) }}
+%} {{ rnafusion_qc_metrics(samples=case.samples) }} {% elif workflow ==
+"taxprofiler" %} {{ taxprofiler_qc_metrics(samples=case.samples) }} {% elif
+workflow == "tomte" %} {{ tomte_qc_metrics(samples=case.samples) }} {% endif %}
+{{ apptag_limitations(applications=case.applications) }}
 {% endmacro %} {% macro workflow_analysis(case) %} {% set workflow =
 case.data_analysis.workflow %}
 ****** DDaattaaaannaallyyss ******
                                                                               {{%% iiff ""bbaallssaammiicc"" iinn     {{%% iiff wwoorrkkffllooww iinn ((""bbaallssaammiicc"",,     {{%% iiff wwoorrkkffllooww iinn ((""mmiipp--
 FFaallll      BBiiooiinnffoorrmmaattiisskk aannaallyyss               GGeennoommvveerrssiioonn                    wwoorrkkffllooww %%}} AAnnaallyyssttyypp   ""bbaallssaammiicc--uummii"")) %%}} VVaarriiaannttaannrrooppaarree ddnnaa"",, ""rrnnaaffuussiioonn"",,
                                                                               {{%% eennddiiff %%}}             {{%% eennddiiff %%}}                        ""ttoommttee"")) %%}} GGeennppaanneelleerr {{%%
                                                                                                                                          eennddiiff %%}}
@@ -38,11 +40,14 @@
 case.data_analysis.scout_files.vcf_fusion != "N/A" %}
 Ingen filtrering har utfÃ¶rts. Alla upptÃ¤ckta varianter rapporteras.
 {% else %}
 Inga fusionsvarianter upptÃ¤cktes.
 {% endif %}
 Workflowinformation och bioinformatiska verktygsversioner: _h_t_t_p_s_:_/_/_n_f_-_c_o_._r_e_/
 _r_n_a_f_u_s_i_o_n.
+{% elif workflow == "taxprofiler" %}
+Workflowinformation och bioinformatiska verktygsversioner: _h_t_t_p_s_:_/_/_g_i_t_h_u_b_._c_o_m_/
+_n_f_-_c_o_r_e_/_t_a_x_p_r_o_f_i_l_e_r.
 {% elif workflow == "tomte" %}
 Workflowinformation och bioinformatiska verktygsversioner: _h_t_t_p_s_:_/_/_g_i_t_h_u_b_._c_o_m_/
 _g_e_n_o_m_i_c_-_m_e_d_i_c_i_n_e_-_s_w_e_d_e_n_/_t_o_m_t_e.
 {% endif %} {% endmacro %}
```

### Comparing `cg-60.4.6/cg/meta/report/templates/macros/data_analysis/limitations.html` & `cg-60.4.7/cg/meta/report/templates/macros/data_analysis/limitations.html`

 * *Files identical despite different names*

### Comparing `cg-60.4.6/cg/meta/report/templates/macros/data_analysis/qc_metrics/balsamic_qc_metrics.html` & `cg-60.4.7/cg/meta/report/templates/macros/data_analysis/qc_metrics/balsamic_qc_metrics.html`

 * *Files identical despite different names*

### Comparing `cg-60.4.6/cg/meta/report/templates/macros/data_analysis/qc_metrics/mip_dna_qc_metrics.html` & `cg-60.4.7/cg/meta/report/templates/macros/data_analysis/qc_metrics/mip_dna_qc_metrics.html`

 * *Files identical despite different names*

### Comparing `cg-60.4.6/cg/meta/report/templates/macros/data_analysis/qc_metrics/qc_metrics.html` & `cg-60.4.7/cg/meta/report/templates/macros/data_analysis/qc_metrics/qc_metrics.html`

 * *Files identical despite different names*

### Comparing `cg-60.4.6/cg/meta/report/templates/macros/data_analysis/qc_metrics/rnafusion_qc_metrics.html` & `cg-60.4.7/cg/meta/report/templates/macros/data_analysis/qc_metrics/rnafusion_qc_metrics.html`

 * *Files identical despite different names*

### Comparing `cg-60.4.6/cg/meta/report/templates/macros/data_analysis/qc_metrics/tomte_qc_metrics.html` & `cg-60.4.7/cg/meta/report/templates/macros/data_analysis/qc_metrics/tomte_qc_metrics.html`

 * *Files identical despite different names*

### Comparing `cg-60.4.6/cg/meta/report/templates/macros/header.html` & `cg-60.4.7/cg/meta/report/templates/macros/header.html`

 * *Files identical despite different names*

### Comparing `cg-60.4.6/cg/meta/report/templates/macros/order.html` & `cg-60.4.7/cg/meta/report/templates/macros/order.html`

 * *Files 7% similar despite different names*

```diff
@@ -7,15 +7,15 @@
         <tr>
           <th scope="col">Fall</th>
           <th scope="col">Bioinformatisk analys</th>
           <th scope="col">Prov</th>
           <th scope="col">Beställt</th>
           <th scope="col">Ticket</th>
           <th scope="col">Applikation</th>
-          <th scope="col">Kön</th>
+          <th scope="col">{% if customer_workflow != "taxprofiler" %} Kön {% endif %}</th>
           <th scope="col">Provtyp</th>
           <!-- Sample status -->
           {{ sample_status(workflow=customer_workflow) }}
         </tr>
       </thead>
       <tbody>
         <tr>
@@ -28,15 +28,15 @@
         </tr>
         {% for sample in case.samples %}
           <tr>
             <td>{{ sample.name }} ({{ sample.id }})</td>
             <td>{{ sample.timestamps.ordered_at }}</td>
             <td>{{ sample.ticket }}</td>
             <td>{{ sample.application.tag }}</td>
-            <td>{{ sample.gender }}</td>
+            <td>{% if customer_workflow != "taxprofiler" %} {{ sample.gender }} {% endif %}</td>
             <td>{{ sample.source }}</td>
             <!-- Sample status value -->
             {{ sample_status_value(workflow=customer_workflow, sample=sample) }}
           </tr>
         {% endfor %}
       </tbody>
     </table>
```

#### html2text {}

```diff
@@ -1,21 +1,25 @@
 {% macro order(case) %} {% set customer_workflow =
 case.data_analysis.customer_workflow %}
 ******** BBeesstt?Ã?¤llllnniinngg ********
-FFaallll        BBiiooiinnffoorrmmaattiisskk aannaallyyss                PPrroovv          BBeesstt?Ã?¤lllltt              TTiicckkeett        AApppplliikkaattiioonn   KK?Ã?¶nn PPrroovvttyypp
+                                                                                                                      {{%% iiff
+                                                                                                                      ccuussttoommeerr__wwoorrkkffllooww
+FFaallll        BBiiooiinnffoorrmmaattiisskk aannaallyyss                PPrroovv          BBeesstt?Ã?¤lllltt              TTiicckkeett            AApppplliikkaattiioonn   !!== ""ttaaxxpprrooffiilleerr""  PPrroovvttyypp
+                                                                                                                      %%}} KK?Ã?¶nn {{%% eennddiiff
+                                                                                                                      %%}}
 {{           {
 {{ ccaassee..nnaammee {
 }}}}          case.data_analysis.customer_workflow
             }}
-{
-{                                                {             {                      {             {
-sample.name {{ sample.timestamps.ordered_at }}   {             {                      {             {
-}} ({                                            sample.ticket sample.application.tag sample.gender sample.source
-{ sample.id                                      }}            }}                     }}            }}
-}})
+{                                                                                     {% if
+{                                                {             {                      customer_workflow {
+sample.name {{ sample.timestamps.ordered_at }}   {             {                      != "taxprofiler"  {
+}} ({                                            sample.ticket sample.application.tag %} {              sample.source
+{ sample.id                                      }}            }}                     { sample.gender   }}
+}})                                                                                   }} {% endif %}
 {% endmacro %} {% macro sample_status(workflow) %} {% if "balsamic" in workflow
 or workflow == "rnafusion" %}
 TumÃ¶r
 {% elif workflow in ("mip-dna", "tomte") %}
 Status
 {% endif %} {% endmacro %} {% macro sample_status_value(workflow, sample) %} {%
 if "balsamic" in workflow or workflow == "rnafusion" %}
```

### Comparing `cg-60.4.6/cg/meta/report/templates/macros/sample_prep.html` & `cg-60.4.7/cg/meta/report/templates/macros/sample_prep.html`

 * *Files identical despite different names*

### Comparing `cg-60.4.6/cg/meta/report/templates/macros/uploaded_files/balsamic_uploaded_files.html` & `cg-60.4.7/cg/meta/report/templates/macros/uploaded_files/balsamic_uploaded_files.html`

 * *Files identical despite different names*

### Comparing `cg-60.4.6/cg/meta/report/templates/macros/uploaded_files/mip_dna_uploaded_files.html` & `cg-60.4.7/cg/meta/report/templates/macros/uploaded_files/mip_dna_uploaded_files.html`

 * *Files identical despite different names*

### Comparing `cg-60.4.6/cg/meta/report/templates/macros/uploaded_files/uploaded_files.html` & `cg-60.4.7/cg/meta/report/templates/macros/uploaded_files/uploaded_files.html`

 * *Files identical despite different names*

### Comparing `cg-60.4.6/cg/meta/report/templates/static/css/bootstrap.min.css` & `cg-60.4.7/cg/meta/report/templates/static/css/bootstrap.min.css`

 * *Files identical despite different names*

### Comparing `cg-60.4.6/cg/meta/report/templates/static/images/SWEDAC_logo.png` & `cg-60.4.7/cg/meta/report/templates/static/images/SWEDAC_logo.png`

 * *Files identical despite different names*

### Comparing `cg-60.4.6/cg/meta/report/tomte.py` & `cg-60.4.7/cg/meta/report/tomte.py`

 * *Files 2% similar despite different names*

```diff
@@ -9,28 +9,28 @@
     REQUIRED_SAMPLE_METADATA_TOMTE_FIELDS,
     REQUIRED_SAMPLE_METHODS_FIELDS,
     REQUIRED_SAMPLE_TIMESTAMP_FIELDS,
     REQUIRED_SAMPLE_TOMTE_FIELDS,
 )
 from cg.meta.report.field_validators import get_million_read_pairs
 from cg.meta.report.report_api import ReportAPI
-from cg.meta.workflow.rnafusion import RnafusionAnalysisAPI
+from cg.meta.workflow.tomte import TomteAnalysisAPI
 from cg.models.analysis import AnalysisModel, NextflowAnalysis
 from cg.models.cg_config import CGConfig
 from cg.models.report.metadata import TomteSampleMetadataModel
 from cg.models.report.report import CaseModel
 from cg.models.report.sample import SampleModel
 from cg.models.tomte.tomte import TomteQCMetrics
 from cg.store.models import Case, Sample
 
 
 class TomteReportAPI(ReportAPI):
     """API to create Tomte delivery reports."""
 
-    def __init__(self, config: CGConfig, analysis_api: RnafusionAnalysisAPI):
+    def __init__(self, config: CGConfig, analysis_api: TomteAnalysisAPI):
         super().__init__(config=config, analysis_api=analysis_api)
 
     def get_sample_metadata(
         self, case: Case, sample: Sample, analysis_metadata: NextflowAnalysis
     ) -> TomteSampleMetadataModel:
         """Return Tomte sample metadata to include in the delivery report."""
         sample_metrics: TomteQCMetrics = analysis_metadata.sample_metrics[sample.internal_id]
```

### Comparing `cg-60.4.6/cg/meta/rsync/rsync_api.py` & `cg-60.4.7/cg/meta/rsync/rsync_api.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.6/cg/meta/tar/tar.py` & `cg-60.4.7/cg/meta/tar/tar.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.6/cg/meta/transfer/external_data.py` & `cg-60.4.7/cg/meta/transfer/external_data.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.6/cg/meta/transfer/lims.py` & `cg-60.4.7/cg/meta/transfer/lims.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.6/cg/meta/upload/balsamic/balsamic.py` & `cg-60.4.7/cg/meta/upload/balsamic/balsamic.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.6/cg/meta/upload/coverage.py` & `cg-60.4.7/cg/meta/upload/coverage.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.6/cg/meta/upload/fohm/fohm.py` & `cg-60.4.7/cg/meta/upload/fohm/fohm.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.6/cg/meta/upload/gisaid/constants.py` & `cg-60.4.7/cg/meta/upload/gisaid/constants.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.6/cg/meta/upload/gisaid/gisaid.py` & `cg-60.4.7/cg/meta/upload/gisaid/gisaid.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.6/cg/meta/upload/gisaid/models.py` & `cg-60.4.7/cg/meta/upload/gisaid/models.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.6/cg/meta/upload/gt.py` & `cg-60.4.7/cg/meta/upload/gt.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.6/cg/meta/upload/microsalt/microsalt_upload_api.py` & `cg-60.4.7/cg/meta/upload/microsalt/microsalt_upload_api.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.6/cg/meta/upload/mip/mip_dna.py` & `cg-60.4.7/cg/meta/upload/mip/mip_dna.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.6/cg/meta/upload/mip/mip_rna.py` & `cg-60.4.7/cg/meta/upload/mip/mip_rna.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.6/cg/meta/upload/mutacc.py` & `cg-60.4.7/cg/meta/upload/mutacc.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.6/cg/meta/upload/nf_analysis.py` & `cg-60.4.7/cg/meta/upload/nf_analysis.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.6/cg/meta/upload/nipt/models.py` & `cg-60.4.7/cg/meta/upload/nipt/models.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.6/cg/meta/upload/nipt/nipt.py` & `cg-60.4.7/cg/meta/upload/nipt/nipt.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.6/cg/meta/upload/scout/balsamic_config_builder.py` & `cg-60.4.7/cg/meta/upload/scout/balsamic_config_builder.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.6/cg/meta/upload/scout/balsamic_umi_config_builder.py` & `cg-60.4.7/cg/meta/upload/scout/balsamic_umi_config_builder.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.6/cg/meta/upload/scout/hk_tags.py` & `cg-60.4.7/cg/meta/upload/scout/hk_tags.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.6/cg/meta/upload/scout/mip_config_builder.py` & `cg-60.4.7/cg/meta/upload/scout/mip_config_builder.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.6/cg/meta/upload/scout/rnafusion_config_builder.py` & `cg-60.4.7/cg/meta/upload/scout/rnafusion_config_builder.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.6/cg/meta/upload/scout/scout_config_builder.py` & `cg-60.4.7/cg/meta/upload/scout/scout_config_builder.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.6/cg/meta/upload/scout/uploadscoutapi.py` & `cg-60.4.7/cg/meta/upload/scout/uploadscoutapi.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.6/cg/meta/upload/upload_api.py` & `cg-60.4.7/cg/meta/upload/upload_api.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.6/cg/meta/workflow/analysis.py` & `cg-60.4.7/cg/meta/workflow/analysis.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.6/cg/meta/workflow/balsamic.py` & `cg-60.4.7/cg/meta/workflow/balsamic.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.6/cg/meta/workflow/balsamic_pon.py` & `cg-60.4.7/cg/meta/workflow/balsamic_pon.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.6/cg/meta/workflow/balsamic_qc.py` & `cg-60.4.7/cg/meta/workflow/balsamic_qc.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.6/cg/meta/workflow/balsamic_umi.py` & `cg-60.4.7/cg/meta/workflow/balsamic_umi.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.6/cg/meta/workflow/downsample/downsample.py` & `cg-60.4.7/cg/meta/workflow/downsample/downsample.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.6/cg/meta/workflow/downsample/sbatch.py` & `cg-60.4.7/cg/meta/workflow/downsample/sbatch.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.6/cg/meta/workflow/fastq.py` & `cg-60.4.7/cg/meta/workflow/fastq.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.6/cg/meta/workflow/fluffy.py` & `cg-60.4.7/cg/meta/workflow/fluffy.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.6/cg/meta/workflow/jasen.py` & `cg-60.4.7/cg/meta/workflow/jasen.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.6/cg/meta/workflow/microsalt/metrics_parser/models.py` & `cg-60.4.7/cg/meta/workflow/microsalt/metrics_parser/models.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.6/cg/meta/workflow/microsalt/microsalt.py` & `cg-60.4.7/cg/meta/workflow/microsalt/microsalt.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.6/cg/meta/workflow/microsalt/quality_controller/models.py` & `cg-60.4.7/cg/meta/workflow/microsalt/quality_controller/models.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.6/cg/meta/workflow/microsalt/quality_controller/quality_controller.py` & `cg-60.4.7/cg/meta/workflow/microsalt/quality_controller/quality_controller.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.6/cg/meta/workflow/microsalt/quality_controller/report_generator.py` & `cg-60.4.7/cg/meta/workflow/microsalt/quality_controller/report_generator.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.6/cg/meta/workflow/microsalt/quality_controller/result_logger.py` & `cg-60.4.7/cg/meta/workflow/microsalt/quality_controller/result_logger.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.6/cg/meta/workflow/microsalt/quality_controller/utils.py` & `cg-60.4.7/cg/meta/workflow/microsalt/quality_controller/utils.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.6/cg/meta/workflow/microsalt/utils.py` & `cg-60.4.7/cg/meta/workflow/microsalt/utils.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.6/cg/meta/workflow/mip.py` & `cg-60.4.7/cg/meta/workflow/mip.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.6/cg/meta/workflow/mip_dna.py` & `cg-60.4.7/cg/meta/workflow/mip_dna.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.6/cg/meta/workflow/mip_rna.py` & `cg-60.4.7/cg/meta/workflow/mip_rna.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.6/cg/meta/workflow/mutant.py` & `cg-60.4.7/cg/meta/workflow/mutant.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.6/cg/meta/workflow/nf_analysis.py` & `cg-60.4.7/cg/meta/workflow/nf_analysis.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.6/cg/meta/workflow/nf_handlers.py` & `cg-60.4.7/cg/meta/workflow/nf_handlers.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.6/cg/meta/workflow/prepare_fastq.py` & `cg-60.4.7/cg/meta/workflow/prepare_fastq.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.6/cg/meta/workflow/raredisease.py` & `cg-60.4.7/cg/meta/workflow/raredisease.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.6/cg/meta/workflow/rnafusion.py` & `cg-60.4.7/cg/meta/workflow/rnafusion.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.6/cg/meta/workflow/taxprofiler.py` & `cg-60.4.7/cg/meta/workflow/taxprofiler.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 """Module for Taxprofiler Analysis API."""
 
 import logging
 from pathlib import Path
 
 from cg.constants import Workflow
+from cg.constants.constants import GenomeVersion
 from cg.constants.nf_analysis import MULTIQC_NEXFLOW_CONFIG
 from cg.constants.sequencing import SequencingPlatform
 from cg.constants.symbols import EMPTY_STRING
 from cg.meta.workflow.nf_analysis import NfAnalysisAPI
 from cg.models.cg_config import CGConfig
 from cg.models.taxprofiler.taxprofiler import TaxprofilerParameters, TaxprofilerSampleSheetEntry
 from cg.resources import TAXPROFILER_BUNDLE_FILENAMES_PATH
@@ -95,7 +96,11 @@
     def get_multiqc_search_patterns(self, case_id: str) -> dict:
         """Return search patterns for MultiQC for Taxprofiler."""
         samples: list[Sample] = self.status_db.get_samples_by_case_id(case_id=case_id)
         search_patterns: dict[str, str] = {
             f"{sample.name}_{sample.name}": sample.internal_id for sample in samples
         }
         return search_patterns
+
+    def get_genome_build(self, case_id: str) -> str:
+        """Return the reference genome build version of a Taxprofiler analysis."""
+        return GenomeVersion.T2T_CHM13.value
```

### Comparing `cg-60.4.6/cg/meta/workflow/tomte.py` & `cg-60.4.7/cg/meta/workflow/tomte.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.6/cg/models/balsamic/config.py` & `cg-60.4.7/cg/models/balsamic/config.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.6/cg/models/balsamic/metrics.py` & `cg-60.4.7/cg/models/balsamic/metrics.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.6/cg/models/cg_config.py` & `cg-60.4.7/cg/models/cg_config.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.6/cg/models/compression_data.py` & `cg-60.4.7/cg/models/compression_data.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.6/cg/models/deliverables/metric_deliverables.py` & `cg-60.4.7/cg/models/deliverables/metric_deliverables.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.6/cg/models/demultiplex/run_parameters.py` & `cg-60.4.7/cg/models/demultiplex/run_parameters.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.6/cg/models/demultiplex/sbatch.py` & `cg-60.4.7/cg/models/demultiplex/sbatch.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.6/cg/models/downsample/downsample_data.py` & `cg-60.4.7/cg/models/downsample/downsample_data.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.6/cg/models/fastq.py` & `cg-60.4.7/cg/models/fastq.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.6/cg/models/file_data.py` & `cg-60.4.7/cg/models/file_data.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.6/cg/models/flow_cell/flow_cell.py` & `cg-60.4.7/cg/models/flow_cell/flow_cell.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.6/cg/models/invoice/invoice.py` & `cg-60.4.7/cg/models/invoice/invoice.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.6/cg/models/lims/sample.py` & `cg-60.4.7/cg/models/lims/sample.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.6/cg/models/mip/mip_config.py` & `cg-60.4.7/cg/models/mip/mip_config.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.6/cg/models/mip/mip_metrics_deliverables.py` & `cg-60.4.7/cg/models/mip/mip_metrics_deliverables.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.6/cg/models/mip/mip_sample_info.py` & `cg-60.4.7/cg/models/mip/mip_sample_info.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.6/cg/models/nf_analysis.py` & `cg-60.4.7/cg/models/nf_analysis.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.6/cg/models/observations/input_files.py` & `cg-60.4.7/cg/models/observations/input_files.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.6/cg/models/orders/constants.py` & `cg-60.4.7/cg/models/orders/constants.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.6/cg/models/orders/excel_sample.py` & `cg-60.4.7/cg/models/orders/excel_sample.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.6/cg/models/orders/json_sample.py` & `cg-60.4.7/cg/models/orders/json_sample.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.6/cg/models/orders/order.py` & `cg-60.4.7/cg/models/orders/order.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.6/cg/models/orders/orderform_schema.py` & `cg-60.4.7/cg/models/orders/orderform_schema.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.6/cg/models/orders/sample_base.py` & `cg-60.4.7/cg/models/orders/sample_base.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.6/cg/models/orders/samples.py` & `cg-60.4.7/cg/models/orders/samples.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.6/cg/models/orders/validators/excel_sample_validators.py` & `cg-60.4.7/cg/models/orders/validators/excel_sample_validators.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.6/cg/models/orders/validators/json_sample_validators.py` & `cg-60.4.7/cg/models/orders/validators/json_sample_validators.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.6/cg/models/raredisease/raredisease.py` & `cg-60.4.7/cg/models/raredisease/raredisease.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.6/cg/models/report/metadata.py` & `cg-60.4.7/cg/models/report/metadata.py`

 * *Files 4% similar despite different names*

```diff
@@ -83,43 +83,51 @@
 
     median_coverage: Annotated[str, BeforeValidator(get_float_as_string)] = NA_FIELD
     pct_15x: Annotated[str, BeforeValidator(get_float_as_string)] = NA_FIELD
     pct_60x: Annotated[str, BeforeValidator(get_float_as_string)] = NA_FIELD
     pct_reads_improper_pairs: Annotated[str, BeforeValidator(get_float_as_string)] = NA_FIELD
 
 
-class WTSSampleMetadataModel(SampleMetadataModel):
-    """Metrics and trending data model associated to a WTS sample.
+class SequencingSampleMetadataModel(SampleMetadataModel):
+    """Metrics and trending data model associated to the sequencing of a sample."
 
     Attributes:
-        bias_5_3: bias is the ratio between read counts; source: workflow
         gc_content: percentage of GC bases calculated on trimmed reads; source: workflow
         input_amount: input amount in ng; source: LIMS
         mean_length_r1: average length of reads that pass QC filters; source: workflow
+        rin: RNA integrity number; source: LIMS
+    """
+
+    gc_content: Annotated[str, BeforeValidator(get_float_as_percentage)] = NA_FIELD
+    input_amount: Annotated[str, BeforeValidator(get_float_as_string)] = NA_FIELD
+    mean_length_r1: Annotated[str, BeforeValidator(get_float_as_string)] = NA_FIELD
+    rin: Annotated[str, BeforeValidator(get_float_as_string)] = NA_FIELD
+
+
+class WTSSampleMetadataModel(SequencingSampleMetadataModel):
+    """Metrics and trending data model associated to a WTS sample.
+
+    Attributes:
+        bias_5_3: bias is the ratio between read counts; source: workflow
         mrna_bases:  proportion of bases that originate from messenger RNA; source: workflow
         pct_adapter: proportion of reads that contain adapter sequences; source: workflow
         pct_surviving: percentage of reads that pass quality control filters; source: workflow
         q20_rate: proportion of bases with a minimum Phred score of 20; source: workflow
         q30_rate: proportion of bases with a minimum Phred score of 30; source: workflow
         ribosomal_bases: proportion of bases that originate from ribosomal RNA; source: workflow
-        rin: RNA integrity number; source: LIMS
         uniquely_mapped_reads: percentage of mapped reads; source: workflow
     """
 
     bias_5_3: Annotated[str, BeforeValidator(get_float_as_string)] = NA_FIELD
-    gc_content: Annotated[str, BeforeValidator(get_float_as_percentage)] = NA_FIELD
-    input_amount: Annotated[str, BeforeValidator(get_float_as_string)] = NA_FIELD
-    mean_length_r1: Annotated[str, BeforeValidator(get_float_as_string)] = NA_FIELD
     mrna_bases: Annotated[str, BeforeValidator(get_float_as_string)] = NA_FIELD
     pct_adapter: Annotated[str, BeforeValidator(get_float_as_string)] = NA_FIELD
     pct_surviving: Annotated[str, BeforeValidator(get_float_as_string)] = NA_FIELD
     q20_rate: Annotated[str, BeforeValidator(get_float_as_percentage)] = NA_FIELD
     q30_rate: Annotated[str, BeforeValidator(get_float_as_percentage)] = NA_FIELD
     ribosomal_bases: Annotated[str, BeforeValidator(get_float_as_percentage)] = NA_FIELD
-    rin: Annotated[str, BeforeValidator(get_float_as_string)] = NA_FIELD
     uniquely_mapped_reads: Annotated[str, BeforeValidator(get_float_as_string)] = NA_FIELD
 
 
 class RnafusionSampleMetadataModel(WTSSampleMetadataModel):
     """Metrics and trending data model associated to a specific Rnafusion sample.
 
     Attributes:
@@ -129,14 +137,32 @@
     """
 
     insert_size: Annotated[str, BeforeValidator(get_float_as_string)] = NA_FIELD
     insert_size_peak: Annotated[str, BeforeValidator(get_float_as_string)] = NA_FIELD
     mapped_reads: Annotated[str, BeforeValidator(get_float_as_percentage)] = NA_FIELD
 
 
+class TaxprofilerSampleMetadataModel(SequencingSampleMetadataModel):
+    """Metrics and trending data model associated to a Taxprofiler sample.
+
+    Attributes:
+        average_read_length: average length of reads; source: workflow
+        mapped_reads: reads aligned to the reference sequence; source: workflow
+        mean_length_r2: average length of reads for read2; source: workflow
+        million_read_pairs_after_filtering: number of reads after filtering; source: workflow
+    """
+
+    average_read_length: Annotated[str, BeforeValidator(get_float_as_string)] = NA_FIELD
+    mapped_reads: Annotated[str, BeforeValidator(get_float_as_string)] = NA_FIELD
+    mean_length_r2: Annotated[str, BeforeValidator(get_float_as_string)] = NA_FIELD
+    million_read_pairs_after_filtering: Annotated[str, BeforeValidator(get_float_as_string)] = (
+        NA_FIELD
+    )
+
+
 class TomteSampleMetadataModel(WTSSampleMetadataModel):
     """Metrics and trending data model associated to a Tomte sample.
 
     Attributes:
         pct_intergenic_bases: proportion of genomic bases located between genes; source: workflow
         pct_intronic_bases: proportion of genomic bases within intronic regions; source: workflow
     """
```

### Comparing `cg-60.4.6/cg/models/report/report.py` & `cg-60.4.7/cg/models/report/report.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.6/cg/models/report/sample.py` & `cg-60.4.7/cg/models/report/sample.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,14 +4,15 @@
 from cg.constants import NA_FIELD
 from cg.models.report.metadata import (
     BalsamicTargetedSampleMetadataModel,
     BalsamicWGSSampleMetadataModel,
     MipDNASampleMetadataModel,
     RnafusionSampleMetadataModel,
     TomteSampleMetadataModel,
+    TaxprofilerSampleMetadataModel,
 )
 from cg.models.report.validators import (
     get_boolean_as_string,
     get_date_as_string,
     get_delivered_files_as_file_names,
     get_gender_as_string,
     get_prep_category_as_string,
@@ -104,14 +105,15 @@
     application: ApplicationModel
     methods: MethodsModel
     metadata: (
         MipDNASampleMetadataModel
         | BalsamicTargetedSampleMetadataModel
         | BalsamicWGSSampleMetadataModel
         | RnafusionSampleMetadataModel
+        | TaxprofilerSampleMetadataModel
         | TomteSampleMetadataModel
     )
     timestamps: TimestampModel
     delivered_files: Annotated[
         list[str] | str, BeforeValidator(get_delivered_files_as_file_names)
     ] = None
     delivered_fastq_files: Annotated[
```

### Comparing `cg-60.4.6/cg/models/report/validators.py` & `cg-60.4.7/cg/models/report/validators.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.6/cg/models/rnafusion/rnafusion.py` & `cg-60.4.7/cg/models/rnafusion/rnafusion.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.6/cg/models/scout/scout_load_config.py` & `cg-60.4.7/cg/models/scout/scout_load_config.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.6/cg/models/slurm/sbatch.py` & `cg-60.4.7/cg/models/slurm/sbatch.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.6/cg/models/taxprofiler/taxprofiler.py` & `cg-60.4.7/cg/models/taxprofiler/taxprofiler.py`

 * *Files 7% similar despite different names*

```diff
@@ -4,18 +4,22 @@
 from cg.constants.sequencing import SequencingPlatform
 from cg.models.nf_analysis import NextflowSampleSheetEntry, WorkflowParameters
 
 
 class TaxprofilerQCMetrics(BaseModel):
     """Taxprofiler QC metrics."""
 
-    after_filtering_total_reads: float | None
-    reads_mapped: float | None
-    before_filtering_total_reads: float | None
-    paired_aligned_none: float | None
+    after_filtering_gc_content: float
+    after_filtering_read1_mean_length: float
+    after_filtering_read2_mean_length: float
+    after_filtering_total_reads: float
+    average_length: float
+    pct_duplication: float
+    raw_total_sequences: float
+    reads_mapped: float
 
 
 class TaxprofilerParameters(WorkflowParameters):
     """Model for Taxprofiler parameters."""
 
     databases: Path
     save_preprocessed_reads: bool = True
```

### Comparing `cg-60.4.6/cg/models/tomte/tomte.py` & `cg-60.4.7/cg/models/tomte/tomte.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.6/cg/models/workflow/mutant.py` & `cg-60.4.7/cg/models/workflow/mutant.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.6/cg/resources/__init__.py` & `cg-60.4.7/cg/resources/__init__.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.6/cg/resources/rnafusion_bundle_filenames.yaml` & `cg-60.4.7/cg/resources/rnafusion_bundle_filenames.yaml`

 * *Files identical despite different names*

### Comparing `cg-60.4.6/cg/resources/taxprofiler_bundle_filenames.yaml` & `cg-60.4.7/cg/resources/taxprofiler_bundle_filenames.yaml`

 * *Files identical despite different names*

### Comparing `cg-60.4.6/cg/resources/tomte_bundle_filenames.yaml` & `cg-60.4.7/cg/resources/tomte_bundle_filenames.yaml`

 * *Files identical despite different names*

### Comparing `cg-60.4.6/cg/server/admin.py` & `cg-60.4.7/cg/server/admin.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.6/cg/server/api.py` & `cg-60.4.7/cg/server/api.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.6/cg/server/app.py` & `cg-60.4.7/cg/server/app.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.6/cg/server/config.py` & `cg-60.4.7/cg/server/config.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.6/cg/server/dto/orders/orders_request.py` & `cg-60.4.7/cg/server/dto/orders/orders_request.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.6/cg/server/ext.py` & `cg-60.4.7/cg/server/ext.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.6/cg/server/invoices/templates/invoices/index.html` & `cg-60.4.7/cg/server/invoices/templates/invoices/index.html`

 * *Files identical despite different names*

### Comparing `cg-60.4.6/cg/server/invoices/templates/invoices/invoice.html` & `cg-60.4.7/cg/server/invoices/templates/invoices/invoice.html`

 * *Files identical despite different names*

### Comparing `cg-60.4.6/cg/server/invoices/templates/invoices/layout.html` & `cg-60.4.7/cg/server/invoices/templates/invoices/layout.html`

 * *Files identical despite different names*

### Comparing `cg-60.4.6/cg/server/invoices/templates/invoices/new.html` & `cg-60.4.7/cg/server/invoices/templates/invoices/new.html`

 * *Files identical despite different names*

### Comparing `cg-60.4.6/cg/server/invoices/views.py` & `cg-60.4.7/cg/server/invoices/views.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.6/cg/services/delivery_message/delivery_message_service.py` & `cg-60.4.7/cg/services/delivery_message/delivery_message_service.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.6/cg/services/delivery_message/messages/__init__.py` & `cg-60.4.7/cg/services/delivery_message/messages/__init__.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.6/cg/services/delivery_message/messages/analysis_scout_message.py` & `cg-60.4.7/cg/services/delivery_message/messages/analysis_scout_message.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.6/cg/services/delivery_message/messages/covid_message.py` & `cg-60.4.7/cg/services/delivery_message/messages/covid_message.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.6/cg/services/delivery_message/messages/fastq_analysis_scout_message.py` & `cg-60.4.7/cg/services/delivery_message/messages/fastq_analysis_scout_message.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.6/cg/services/delivery_message/messages/fastq_message.py` & `cg-60.4.7/cg/services/delivery_message/messages/fastq_message.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.6/cg/services/delivery_message/messages/fastq_scout_message.py` & `cg-60.4.7/cg/services/delivery_message/messages/fastq_scout_message.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.6/cg/services/delivery_message/messages/microsalt_mwr_message.py` & `cg-60.4.7/cg/services/delivery_message/messages/microsalt_mwr_message.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.6/cg/services/delivery_message/messages/microsalt_mwx_message.py` & `cg-60.4.7/cg/services/delivery_message/messages/microsalt_mwx_message.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.6/cg/services/delivery_message/messages/scout_message.py` & `cg-60.4.7/cg/services/delivery_message/messages/scout_message.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.6/cg/services/delivery_message/messages/statina_message.py` & `cg-60.4.7/cg/services/delivery_message/messages/statina_message.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.6/cg/services/delivery_message/messages/utils.py` & `cg-60.4.7/cg/services/delivery_message/messages/utils.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.6/cg/services/delivery_message/utils.py` & `cg-60.4.7/cg/services/delivery_message/utils.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.6/cg/services/fastq_file_service/fastq_file_service.py` & `cg-60.4.7/cg/services/fastq_file_service/fastq_file_service.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.6/cg/services/fastq_file_service/utils.py` & `cg-60.4.7/cg/services/fastq_file_service/utils.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.6/cg/services/orders/order_service/order_service.py` & `cg-60.4.7/cg/services/orders/order_service/order_service.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.6/cg/services/orders/order_service/utils.py` & `cg-60.4.7/cg/services/orders/order_service/utils.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.6/cg/services/orders/order_status_service/order_summary_service.py` & `cg-60.4.7/cg/services/orders/order_status_service/order_summary_service.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.6/cg/services/orders/order_status_service/utils.py` & `cg-60.4.7/cg/services/orders/order_status_service/utils.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.6/cg/services/quality_controller/quality_checks/checks.py` & `cg-60.4.7/cg/services/quality_controller/quality_checks/checks.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.6/cg/services/quality_controller/quality_checks/utils.py` & `cg-60.4.7/cg/services/quality_controller/quality_checks/utils.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.6/cg/services/quality_controller/quality_controller_service.py` & `cg-60.4.7/cg/services/quality_controller/quality_controller_service.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.6/cg/services/slurm_service/slurm_cli_service.py` & `cg-60.4.7/cg/services/slurm_service/slurm_cli_service.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.6/cg/services/slurm_upload_service/slurm_upload_service.py` & `cg-60.4.7/cg/services/slurm_upload_service/slurm_upload_service.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.6/cg/store/base.py` & `cg-60.4.7/cg/store/base.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.6/cg/store/crud/create.py` & `cg-60.4.7/cg/store/crud/create.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.6/cg/store/crud/delete.py` & `cg-60.4.7/cg/store/crud/delete.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.6/cg/store/crud/read.py` & `cg-60.4.7/cg/store/crud/read.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.6/cg/store/crud/update.py` & `cg-60.4.7/cg/store/crud/update.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.6/cg/store/database.py` & `cg-60.4.7/cg/store/database.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.6/cg/store/filters/status_analysis_filters.py` & `cg-60.4.7/cg/store/filters/status_analysis_filters.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.6/cg/store/filters/status_application_filters.py` & `cg-60.4.7/cg/store/filters/status_application_filters.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.6/cg/store/filters/status_application_limitations_filters.py` & `cg-60.4.7/cg/store/filters/status_application_limitations_filters.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.6/cg/store/filters/status_application_version_filters.py` & `cg-60.4.7/cg/store/filters/status_application_version_filters.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.6/cg/store/filters/status_bed_filters.py` & `cg-60.4.7/cg/store/filters/status_bed_filters.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.6/cg/store/filters/status_bed_version_filters.py` & `cg-60.4.7/cg/store/filters/status_bed_version_filters.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.6/cg/store/filters/status_case_filters.py` & `cg-60.4.7/cg/store/filters/status_case_filters.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.6/cg/store/filters/status_case_sample_filters.py` & `cg-60.4.7/cg/store/filters/status_case_sample_filters.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.6/cg/store/filters/status_collaboration_filters.py` & `cg-60.4.7/cg/store/filters/status_collaboration_filters.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.6/cg/store/filters/status_customer_filters.py` & `cg-60.4.7/cg/store/filters/status_customer_filters.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.6/cg/store/filters/status_flow_cell_filters.py` & `cg-60.4.7/cg/store/filters/status_flow_cell_filters.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.6/cg/store/filters/status_invoice_filters.py` & `cg-60.4.7/cg/store/filters/status_invoice_filters.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.6/cg/store/filters/status_metrics_filters.py` & `cg-60.4.7/cg/store/filters/status_metrics_filters.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.6/cg/store/filters/status_order_filters.py` & `cg-60.4.7/cg/store/filters/status_order_filters.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.6/cg/store/filters/status_organism_filters.py` & `cg-60.4.7/cg/store/filters/status_organism_filters.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.6/cg/store/filters/status_panel_filters.py` & `cg-60.4.7/cg/store/filters/status_panel_filters.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.6/cg/store/filters/status_pool_filters.py` & `cg-60.4.7/cg/store/filters/status_pool_filters.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.6/cg/store/filters/status_sample_filters.py` & `cg-60.4.7/cg/store/filters/status_sample_filters.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.6/cg/store/filters/status_user_filters.py` & `cg-60.4.7/cg/store/filters/status_user_filters.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.6/cg/store/models.py` & `cg-60.4.7/cg/store/models.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.6/cg/store/store.py` & `cg-60.4.7/cg/store/store.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.6/cg/utils/checksum/checksum.py` & `cg-60.4.7/cg/utils/checksum/checksum.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.6/cg/utils/click/EnumChoice.py` & `cg-60.4.7/cg/utils/click/EnumChoice.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.6/cg/utils/commands.py` & `cg-60.4.7/cg/utils/commands.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.6/cg/utils/date.py` & `cg-60.4.7/cg/utils/date.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.6/cg/utils/dict.py` & `cg-60.4.7/cg/utils/dict.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.6/cg/utils/dispatcher.py` & `cg-60.4.7/cg/utils/dispatcher.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.6/cg/utils/email.py` & `cg-60.4.7/cg/utils/email.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.6/cg/utils/files.py` & `cg-60.4.7/cg/utils/files.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.6/cg/utils/flask/enum.py` & `cg-60.4.7/cg/utils/flask/enum.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.6/cg/utils/time.py` & `cg-60.4.7/cg/utils/time.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.6/cg/utils/utils.py` & `cg-60.4.7/cg/utils/utils.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.6/pyproject.toml` & `cg-60.4.7/pyproject.toml`

 * *Files 9% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
 name = "cg"
-version = "60.4.6"
+version = "60.4.7"
 description = "Clinical Genomics command center"
 authors = ["Clinical Genomics <support@clinicalgenomics.se>"]
 readme = "README.md"
 homepage = "https://github.com/Clinical-Genomics/cg"
 repository = "https://github.com/Clinical-Genomics/cg"
 classifiers = [
   "Programming Language :: Python",
```

### Comparing `cg-60.4.6/tests/apps/conftest.py` & `cg-60.4.7/tests/apps/conftest.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.6/tests/apps/coverage/test_coverage.py` & `cg-60.4.7/tests/apps/coverage/test_coverage.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.6/tests/apps/crunchy/conftest.py` & `cg-60.4.7/tests/apps/crunchy/conftest.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.6/tests/apps/crunchy/test_compress_fastq.py` & `cg-60.4.7/tests/apps/crunchy/test_compress_fastq.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.6/tests/apps/crunchy/test_config.py` & `cg-60.4.7/tests/apps/crunchy/test_config.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.6/tests/apps/crunchy/test_crunchy.py` & `cg-60.4.7/tests/apps/crunchy/test_crunchy.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.6/tests/apps/crunchy/test_spring_decompression.py` & `cg-60.4.7/tests/apps/crunchy/test_spring_decompression.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.6/tests/apps/demultiplex/conftest.py` & `cg-60.4.7/tests/apps/demultiplex/conftest.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.6/tests/apps/demultiplex/test_create_sample_sheet.py` & `cg-60.4.7/tests/apps/demultiplex/test_create_sample_sheet.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.6/tests/apps/demultiplex/test_demultiplex_api.py` & `cg-60.4.7/tests/apps/demultiplex/test_demultiplex_api.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.6/tests/apps/demultiplex/test_index.py` & `cg-60.4.7/tests/apps/demultiplex/test_index.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.6/tests/apps/demultiplex/test_override_cycles_validator.py` & `cg-60.4.7/tests/apps/demultiplex/test_override_cycles_validator.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.6/tests/apps/demultiplex/test_read_sample_sheet.py` & `cg-60.4.7/tests/apps/demultiplex/test_read_sample_sheet.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.6/tests/apps/demultiplex/test_sample_models.py` & `cg-60.4.7/tests/apps/demultiplex/test_sample_models.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.6/tests/apps/demultiplex/test_sample_sheet_creator.py` & `cg-60.4.7/tests/apps/demultiplex/test_sample_sheet_creator.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.6/tests/apps/demultiplex/test_sample_sheet_models.py` & `cg-60.4.7/tests/apps/demultiplex/test_sample_sheet_models.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.6/tests/apps/demultiplex/test_sample_sheet_validator.py` & `cg-60.4.7/tests/apps/demultiplex/test_sample_sheet_validator.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.6/tests/apps/demultiplex/test_translate_sample_sheet.py` & `cg-60.4.7/tests/apps/demultiplex/test_translate_sample_sheet.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.6/tests/apps/demultiplex/test_validate.py` & `cg-60.4.7/tests/apps/demultiplex/test_validate.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.6/tests/apps/downsample/test_downsample.py` & `cg-60.4.7/tests/apps/downsample/test_downsample.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.6/tests/apps/downsample/test_downsample_utils.py` & `cg-60.4.7/tests/apps/downsample/test_downsample_utils.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.6/tests/apps/gens/test_gens_api.py` & `cg-60.4.7/tests/apps/gens/test_gens_api.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.6/tests/apps/gt/conftest.py` & `cg-60.4.7/tests/apps/gt/conftest.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.6/tests/apps/gt/test_gt_api.py` & `cg-60.4.7/tests/apps/gt/test_gt_api.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.6/tests/apps/hk/conftest.py` & `cg-60.4.7/tests/apps/hk/conftest.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.6/tests/apps/hk/test__getattr__.py` & `cg-60.4.7/tests/apps/hk/test__getattr__.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.6/tests/apps/hk/test_add_file.py` & `cg-60.4.7/tests/apps/hk/test_add_file.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.6/tests/apps/hk/test_bundles.py` & `cg-60.4.7/tests/apps/hk/test_bundles.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.6/tests/apps/hk/test_core.py` & `cg-60.4.7/tests/apps/hk/test_core.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.6/tests/apps/hk/test_file.py` & `cg-60.4.7/tests/apps/hk/test_file.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.6/tests/apps/hk/test_version.py` & `cg-60.4.7/tests/apps/hk/test_version.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.6/tests/apps/lims/conftest.py` & `cg-60.4.7/tests/apps/lims/conftest.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.6/tests/apps/lims/test_api.py` & `cg-60.4.7/tests/apps/lims/test_api.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.6/tests/apps/lims/test_sample_sheet.py` & `cg-60.4.7/tests/apps/lims/test_sample_sheet.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.6/tests/apps/loqus/conftest.py` & `cg-60.4.7/tests/apps/loqus/conftest.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.6/tests/apps/loqus/test_loqusdb_api.py` & `cg-60.4.7/tests/apps/loqus/test_loqusdb_api.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.6/tests/apps/madeline/conftest.py` & `cg-60.4.7/tests/apps/madeline/conftest.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.6/tests/apps/madeline/test_madeline.py` & `cg-60.4.7/tests/apps/madeline/test_madeline.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.6/tests/apps/mip/conftest.py` & `cg-60.4.7/tests/apps/mip/conftest.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.6/tests/apps/mip/test_config_mip.py` & `cg-60.4.7/tests/apps/mip/test_config_mip.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.6/tests/apps/mutacc_auto/conftest.py` & `cg-60.4.7/tests/apps/mutacc_auto/conftest.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.6/tests/apps/mutacc_auto/test_mutacc_auto.py` & `cg-60.4.7/tests/apps/mutacc_auto/test_mutacc_auto.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.6/tests/apps/orderform/conftest.py` & `cg-60.4.7/tests/apps/orderform/conftest.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.6/tests/apps/orderform/test_excel_orderform_parser.py` & `cg-60.4.7/tests/apps/orderform/test_excel_orderform_parser.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.6/tests/apps/orderform/test_excel_sample_schema.py` & `cg-60.4.7/tests/apps/orderform/test_excel_sample_schema.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.6/tests/apps/orderform/test_json_orderform_parser.py` & `cg-60.4.7/tests/apps/orderform/test_json_orderform_parser.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.6/tests/apps/orderform/test_orderform_parser.py` & `cg-60.4.7/tests/apps/orderform/test_orderform_parser.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.6/tests/apps/orderform/validators/test_excel_sample_validators.py` & `cg-60.4.7/tests/apps/orderform/validators/test_excel_sample_validators.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.6/tests/apps/scout/conftest.py` & `cg-60.4.7/tests/apps/scout/conftest.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.6/tests/apps/scout/test_get_causative_variants.py` & `cg-60.4.7/tests/apps/scout/test_get_causative_variants.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.6/tests/apps/scout/test_get_scout_cases.py` & `cg-60.4.7/tests/apps/scout/test_get_scout_cases.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.6/tests/apps/scout/test_scout_load_config.py` & `cg-60.4.7/tests/apps/scout/test_scout_load_config.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.6/tests/apps/scout/test_scout_models.py` & `cg-60.4.7/tests/apps/scout/test_scout_models.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.6/tests/apps/sequencing_metrics_parser/conftest.py` & `cg-60.4.7/tests/apps/sequencing_metrics_parser/conftest.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.6/tests/apps/sequencing_metrics_parser/parsers/test_bclconvert.py` & `cg-60.4.7/tests/apps/sequencing_metrics_parser/parsers/test_bclconvert.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.6/tests/apps/sequencing_metrics_parser/parsers/test_sequencing_metrics_parser_api.py` & `cg-60.4.7/tests/apps/sequencing_metrics_parser/parsers/test_sequencing_metrics_parser_api.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.6/tests/apps/slurm/conftest.py` & `cg-60.4.7/tests/apps/slurm/conftest.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.6/tests/apps/slurm/test_slurm_api.py` & `cg-60.4.7/tests/apps/slurm/test_slurm_api.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.6/tests/apps/test_apps_environ.py` & `cg-60.4.7/tests/apps/test_apps_environ.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.6/tests/apps/test_osticket.py` & `cg-60.4.7/tests/apps/test_osticket.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.6/tests/cli/add/test_cli_add.py` & `cg-60.4.7/tests/cli/add/test_cli_add.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.6/tests/cli/add/test_cli_add_customer.py` & `cg-60.4.7/tests/cli/add/test_cli_add_customer.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.6/tests/cli/add/test_cli_add_family.py` & `cg-60.4.7/tests/cli/add/test_cli_add_family.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.6/tests/cli/add/test_cli_add_relationship.py` & `cg-60.4.7/tests/cli/add/test_cli_add_relationship.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.6/tests/cli/add/test_cli_add_sample.py` & `cg-60.4.7/tests/cli/add/test_cli_add_sample.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.6/tests/cli/backup/conftest.py` & `cg-60.4.7/tests/cli/backup/conftest.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.6/tests/cli/backup/test_backup_command.py` & `cg-60.4.7/tests/cli/backup/test_backup_command.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.6/tests/cli/clean/conftest.py` & `cg-60.4.7/tests/cli/clean/conftest.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.6/tests/cli/clean/test_balsamic_clean.py` & `cg-60.4.7/tests/cli/clean/test_balsamic_clean.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.6/tests/cli/clean/test_clean_flow_cell.py` & `cg-60.4.7/tests/cli/clean/test_clean_flow_cell.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.6/tests/cli/clean/test_clean_hk_bundle_files.py` & `cg-60.4.7/tests/cli/clean/test_clean_hk_bundle_files.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.6/tests/cli/clean/test_hk_bundle_files.py` & `cg-60.4.7/tests/cli/clean/test_hk_bundle_files.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.6/tests/cli/clean/test_hk_case_bundle_files.py` & `cg-60.4.7/tests/cli/clean/test_hk_case_bundle_files.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.6/tests/cli/clean/test_microbial_clean.py` & `cg-60.4.7/tests/cli/clean/test_microbial_clean.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.6/tests/cli/clean/test_rsync_past_run_dirs.py` & `cg-60.4.7/tests/cli/clean/test_rsync_past_run_dirs.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.6/tests/cli/compress/conftest.py` & `cg-60.4.7/tests/cli/compress/conftest.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.6/tests/cli/compress/test_cli_compress_fastq.py` & `cg-60.4.7/tests/cli/compress/test_cli_compress_fastq.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.6/tests/cli/compress/test_cli_decompress_spring.py` & `cg-60.4.7/tests/cli/compress/test_cli_decompress_spring.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.6/tests/cli/compress/test_compress_helpers.py` & `cg-60.4.7/tests/cli/compress/test_compress_helpers.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.6/tests/cli/compress/test_store_fastq.py` & `cg-60.4.7/tests/cli/compress/test_store_fastq.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.6/tests/cli/conftest.py` & `cg-60.4.7/tests/cli/conftest.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.6/tests/cli/delete/test_cli_delete_case.py` & `cg-60.4.7/tests/cli/delete/test_cli_delete_case.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.6/tests/cli/delete/test_cli_delete_cases.py` & `cg-60.4.7/tests/cli/delete/test_cli_delete_cases.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.6/tests/cli/deliver/conftest.py` & `cg-60.4.7/tests/cli/deliver/conftest.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.6/tests/cli/deliver/test_deliver_base.py` & `cg-60.4.7/tests/cli/deliver/test_deliver_base.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.6/tests/cli/deliver/test_rsync_base.py` & `cg-60.4.7/tests/cli/deliver/test_rsync_base.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.6/tests/cli/deliver/test_run_deliver_cmd.py` & `cg-60.4.7/tests/cli/deliver/test_run_deliver_cmd.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.6/tests/cli/demultiplex/test_create_sample_sheet.py` & `cg-60.4.7/tests/cli/demultiplex/test_create_sample_sheet.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.6/tests/cli/demultiplex/test_demultiplex_flowcell.py` & `cg-60.4.7/tests/cli/demultiplex/test_demultiplex_flowcell.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.6/tests/cli/demultiplex/test_finish_demux.py` & `cg-60.4.7/tests/cli/demultiplex/test_finish_demux.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.6/tests/cli/demultiplex/test_validate_sample_sheet.py` & `cg-60.4.7/tests/cli/demultiplex/test_validate_sample_sheet.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.6/tests/cli/demultiplex/test_verify_syncing.py` & `cg-60.4.7/tests/cli/demultiplex/test_verify_syncing.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.6/tests/cli/downsample/test_cli_downsample.py` & `cg-60.4.7/tests/cli/downsample/test_cli_downsample.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.6/tests/cli/generate/report/conftest.py` & `cg-60.4.7/tests/cli/generate/report/conftest.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.6/tests/cli/generate/report/test_cli_delivery_report.py` & `cg-60.4.7/tests/cli/generate/report/test_cli_delivery_report.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.6/tests/cli/generate/report/test_utils.py` & `cg-60.4.7/tests/cli/generate/report/test_utils.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.6/tests/cli/generate/test_cli_base.py` & `cg-60.4.7/tests/cli/generate/test_cli_base.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.6/tests/cli/get/test_cli_get.py` & `cg-60.4.7/tests/cli/get/test_cli_get.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.6/tests/cli/get/test_cli_get_analysis.py` & `cg-60.4.7/tests/cli/get/test_cli_get_analysis.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.6/tests/cli/get/test_cli_get_case.py` & `cg-60.4.7/tests/cli/get/test_cli_get_case.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.6/tests/cli/get/test_cli_get_flow_cell.py` & `cg-60.4.7/tests/cli/get/test_cli_get_flow_cell.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.6/tests/cli/get/test_cli_get_sample.py` & `cg-60.4.7/tests/cli/get/test_cli_get_sample.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.6/tests/cli/set/conftest.py` & `cg-60.4.7/tests/cli/set/conftest.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.6/tests/cli/set/test_cli_set_case.py` & `cg-60.4.7/tests/cli/set/test_cli_set_case.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.6/tests/cli/set/test_cli_set_cases.py` & `cg-60.4.7/tests/cli/set/test_cli_set_cases.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.6/tests/cli/set/test_cli_set_flowcell.py` & `cg-60.4.7/tests/cli/set/test_cli_set_flowcell.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.6/tests/cli/set/test_cli_set_list_keys.py` & `cg-60.4.7/tests/cli/set/test_cli_set_list_keys.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.6/tests/cli/set/test_cli_set_sample.py` & `cg-60.4.7/tests/cli/set/test_cli_set_sample.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.6/tests/cli/set/test_cli_set_samples.py` & `cg-60.4.7/tests/cli/set/test_cli_set_samples.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.6/tests/cli/store/test_store.py` & `cg-60.4.7/tests/cli/store/test_store.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.6/tests/cli/test_base.py` & `cg-60.4.7/tests/cli/test_base.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.6/tests/cli/upload/conftest.py` & `cg-60.4.7/tests/cli/upload/conftest.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.6/tests/cli/upload/test_cli_scout.py` & `cg-60.4.7/tests/cli/upload/test_cli_scout.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.6/tests/cli/upload/test_cli_upload.py` & `cg-60.4.7/tests/cli/upload/test_cli_upload.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.6/tests/cli/upload/test_cli_upload_auto.py` & `cg-60.4.7/tests/cli/upload/test_cli_upload_auto.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.6/tests/cli/upload/test_cli_upload_delivery_report.py` & `cg-60.4.7/tests/cli/upload/test_cli_upload_delivery_report.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.6/tests/cli/upload/test_cli_upload_fastq.py` & `cg-60.4.7/tests/cli/upload/test_cli_upload_fastq.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.6/tests/cli/upload/test_cli_upload_genotype.py` & `cg-60.4.7/tests/cli/upload/test_cli_upload_genotype.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.6/tests/cli/upload/test_cli_upload_gens.py` & `cg-60.4.7/tests/cli/upload/test_cli_upload_gens.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.6/tests/cli/upload/test_cli_upload_nipt.py` & `cg-60.4.7/tests/cli/upload/test_cli_upload_nipt.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.6/tests/cli/upload/test_cli_upload_nipt_ftp.py` & `cg-60.4.7/tests/cli/upload/test_cli_upload_nipt_ftp.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.6/tests/cli/upload/test_cli_upload_nipt_statina.py` & `cg-60.4.7/tests/cli/upload/test_cli_upload_nipt_statina.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.6/tests/cli/upload/test_cli_upload_observations.py` & `cg-60.4.7/tests/cli/upload/test_cli_upload_observations.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.6/tests/cli/workflow/balsamic/conftest.py` & `cg-60.4.7/tests/cli/workflow/balsamic/conftest.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.6/tests/cli/workflow/balsamic/test_cli_balsamic_config_case.py` & `cg-60.4.7/tests/cli/workflow/balsamic/test_cli_balsamic_config_case.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.6/tests/cli/workflow/balsamic/test_compound_commands.py` & `cg-60.4.7/tests/cli/workflow/balsamic/test_compound_commands.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.6/tests/cli/workflow/balsamic/test_link.py` & `cg-60.4.7/tests/cli/workflow/balsamic/test_link.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.6/tests/cli/workflow/balsamic/test_report_deliver.py` & `cg-60.4.7/tests/cli/workflow/balsamic/test_report_deliver.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.6/tests/cli/workflow/balsamic/test_run.py` & `cg-60.4.7/tests/cli/workflow/balsamic/test_run.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.6/tests/cli/workflow/balsamic/test_store_housekeeper.py` & `cg-60.4.7/tests/cli/workflow/balsamic/test_store_housekeeper.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.6/tests/cli/workflow/conftest.py` & `cg-60.4.7/tests/cli/workflow/conftest.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.6/tests/cli/workflow/fastq/test_fastq_base.py` & `cg-60.4.7/tests/cli/workflow/fastq/test_fastq_base.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.6/tests/cli/workflow/fluffy/conftest.py` & `cg-60.4.7/tests/cli/workflow/fluffy/conftest.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.6/tests/cli/workflow/fluffy/test_cli_create_samplesheet.py` & `cg-60.4.7/tests/cli/workflow/fluffy/test_cli_create_samplesheet.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.6/tests/cli/workflow/fluffy/test_cli_link.py` & `cg-60.4.7/tests/cli/workflow/fluffy/test_cli_link.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.6/tests/cli/workflow/fluffy/test_cli_run.py` & `cg-60.4.7/tests/cli/workflow/fluffy/test_cli_run.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.6/tests/cli/workflow/fluffy/test_cli_start.py` & `cg-60.4.7/tests/cli/workflow/fluffy/test_cli_start.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.6/tests/cli/workflow/fluffy/test_cli_store.py` & `cg-60.4.7/tests/cli/workflow/fluffy/test_cli_store.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.6/tests/cli/workflow/microsalt/conftest.py` & `cg-60.4.7/tests/cli/workflow/microsalt/conftest.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.6/tests/cli/workflow/microsalt/test_microsalt_case_config.py` & `cg-60.4.7/tests/cli/workflow/microsalt/test_microsalt_case_config.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.6/tests/cli/workflow/microsalt/test_microsalt_run.py` & `cg-60.4.7/tests/cli/workflow/microsalt/test_microsalt_run.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.6/tests/cli/workflow/mip/conftest.py` & `cg-60.4.7/tests/cli/workflow/mip/conftest.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.6/tests/cli/workflow/mip/test_cli_mip_base.py` & `cg-60.4.7/tests/cli/workflow/mip/test_cli_mip_base.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.6/tests/cli/workflow/mip/test_cli_mip_dna_config_case.py` & `cg-60.4.7/tests/cli/workflow/mip/test_cli_mip_dna_config_case.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.6/tests/cli/workflow/mip/test_cli_mip_dna_manged_variants.py` & `cg-60.4.7/tests/cli/workflow/mip/test_cli_mip_dna_manged_variants.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.6/tests/cli/workflow/mip/test_cli_mip_dna_panel.py` & `cg-60.4.7/tests/cli/workflow/mip/test_cli_mip_dna_panel.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.6/tests/cli/workflow/mip/test_cli_mip_dna_run.py` & `cg-60.4.7/tests/cli/workflow/mip/test_cli_mip_dna_run.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.6/tests/cli/workflow/mip/test_cli_mip_dna_start.py` & `cg-60.4.7/tests/cli/workflow/mip/test_cli_mip_dna_start.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.6/tests/cli/workflow/mip/test_cli_mip_rna_config_case.py` & `cg-60.4.7/tests/cli/workflow/mip/test_cli_mip_rna_config_case.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.6/tests/cli/workflow/mip/test_cli_mip_rna_link.py` & `cg-60.4.7/tests/cli/workflow/mip/test_cli_mip_rna_link.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.6/tests/cli/workflow/mip/test_cli_mip_rna_run.py` & `cg-60.4.7/tests/cli/workflow/mip/test_cli_mip_rna_run.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.6/tests/cli/workflow/mip/test_cli_mip_store.py` & `cg-60.4.7/tests/cli/workflow/mip/test_cli_mip_store.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.6/tests/cli/workflow/nf_analysis/test_cli_config_case.py` & `cg-60.4.7/tests/cli/workflow/nf_analysis/test_cli_config_case.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.6/tests/cli/workflow/nf_analysis/test_cli_metrics_deliver.py` & `cg-60.4.7/tests/cli/workflow/nf_analysis/test_cli_metrics_deliver.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.6/tests/cli/workflow/nf_analysis/test_cli_report_deliver.py` & `cg-60.4.7/tests/cli/workflow/nf_analysis/test_cli_report_deliver.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.6/tests/cli/workflow/nf_analysis/test_cli_run.py` & `cg-60.4.7/tests/cli/workflow/nf_analysis/test_cli_run.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.6/tests/cli/workflow/nf_analysis/test_cli_start.py` & `cg-60.4.7/tests/cli/workflow/nf_analysis/test_cli_start.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.6/tests/cli/workflow/nf_analysis/test_cli_store.py` & `cg-60.4.7/tests/cli/workflow/nf_analysis/test_cli_store.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.6/tests/cli/workflow/nf_analysis/test_cli_store_housekeeper.py` & `cg-60.4.7/tests/cli/workflow/nf_analysis/test_cli_store_housekeeper.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.6/tests/cli/workflow/nf_analysis/test_cli_workflow_base.py` & `cg-60.4.7/tests/cli/workflow/nf_analysis/test_cli_workflow_base.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.6/tests/cli/workflow/raredisease/test_cli_raredisease_compound_commands.py` & `cg-60.4.7/tests/cli/workflow/raredisease/test_cli_raredisease_compound_commands.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.6/tests/cli/workflow/test_cli_workflow.py` & `cg-60.4.7/tests/cli/workflow/test_cli_workflow.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.6/tests/cli/workflow/test_cli_workflow_clean.py` & `cg-60.4.7/tests/cli/workflow/test_cli_workflow_clean.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.6/tests/clients/arnold/conftest.py` & `cg-60.4.7/tests/clients/arnold/conftest.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.6/tests/clients/arnold/test_arnold_api_client.py` & `cg-60.4.7/tests/clients/arnold/test_arnold_api_client.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.6/tests/clients/janus/conftest.py` & `cg-60.4.7/tests/clients/janus/conftest.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.6/tests/clients/janus/test_janus_api_client.py` & `cg-60.4.7/tests/clients/janus/test_janus_api_client.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.6/tests/conftest.py` & `cg-60.4.7/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.6/tests/fixture_plugins/delivery_fixtures/bundle_fixtures.py` & `cg-60.4.7/tests/fixture_plugins/delivery_fixtures/bundle_fixtures.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.6/tests/fixture_plugins/delivery_fixtures/context_fixtures.py` & `cg-60.4.7/tests/fixture_plugins/delivery_fixtures/context_fixtures.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.6/tests/fixture_plugins/delivery_fixtures/path_fixtures.py` & `cg-60.4.7/tests/fixture_plugins/delivery_fixtures/path_fixtures.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.6/tests/fixture_plugins/demultiplex_fixtures/flow_cell_fixtures.py` & `cg-60.4.7/tests/fixture_plugins/demultiplex_fixtures/flow_cell_fixtures.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.6/tests/fixture_plugins/demultiplex_fixtures/name_fixtures.py` & `cg-60.4.7/tests/fixture_plugins/demultiplex_fixtures/name_fixtures.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.6/tests/fixture_plugins/demultiplex_fixtures/path_fixtures.py` & `cg-60.4.7/tests/fixture_plugins/demultiplex_fixtures/path_fixtures.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.6/tests/fixture_plugins/demultiplex_fixtures/run_parameters_fixtures.py` & `cg-60.4.7/tests/fixture_plugins/demultiplex_fixtures/run_parameters_fixtures.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.6/tests/fixture_plugins/demultiplex_fixtures/sample_fixtures.py` & `cg-60.4.7/tests/fixture_plugins/demultiplex_fixtures/sample_fixtures.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.6/tests/fixture_plugins/demultiplex_fixtures/sample_sheet_fixtures.py` & `cg-60.4.7/tests/fixture_plugins/demultiplex_fixtures/sample_sheet_fixtures.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.6/tests/fixture_plugins/quality_controller_fixtures/sequencing_qc_check_scenario.py` & `cg-60.4.7/tests/fixture_plugins/quality_controller_fixtures/sequencing_qc_check_scenario.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.6/tests/fixture_plugins/quality_controller_fixtures/sequencing_qc_fixtures.py` & `cg-60.4.7/tests/fixture_plugins/quality_controller_fixtures/sequencing_qc_fixtures.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.6/tests/fixture_plugins/timestamp_fixtures.py` & `cg-60.4.7/tests/fixture_plugins/timestamp_fixtures.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.6/tests/fixtures/analysis/microsalt/ACC11111_qc_fail/ACC11111_qc_fail.json` & `cg-60.4.7/tests/fixtures/analysis/microsalt/ACC11111_qc_fail/ACC11111_qc_fail.json`

 * *Files identical despite different names*

### Comparing `cg-60.4.6/tests/fixtures/analysis/microsalt/ACC22222_qc_pass/ACC22222_qc_pass.json` & `cg-60.4.7/tests/fixtures/analysis/microsalt/ACC22222_qc_pass/ACC22222_qc_pass.json`

 * *Files identical despite different names*

### Comparing `cg-60.4.6/tests/fixtures/analysis/raredisease/multiqc_data.json` & `cg-60.4.7/tests/fixtures/analysis/raredisease/multiqc_data.json`

 * *Files identical despite different names*

### Comparing `cg-60.4.6/tests/fixtures/analysis/raredisease/raredisease_case_enough_reads_metrics_deliverables.yaml` & `cg-60.4.7/tests/fixtures/analysis/raredisease/raredisease_case_enough_reads_metrics_deliverables.yaml`

 * *Files identical despite different names*

### Comparing `cg-60.4.6/tests/fixtures/analysis/rnafusion/multiqc_data.json` & `cg-60.4.7/tests/fixtures/analysis/rnafusion/multiqc_data.json`

 * *Files identical despite different names*

### Comparing `cg-60.4.6/tests/fixtures/analysis/rnafusion/rnafusion_case_enough_reads_metrics_deliverables.yaml` & `cg-60.4.7/tests/fixtures/analysis/rnafusion/rnafusion_case_enough_reads_metrics_deliverables.yaml`

 * *Files identical despite different names*

### Comparing `cg-60.4.6/tests/fixtures/analysis/sample_coverage.bed` & `cg-60.4.7/tests/fixtures/analysis/sample_coverage.bed`

 * *Files identical despite different names*

### Comparing `cg-60.4.6/tests/fixtures/analysis/taxprofiler/multiqc_data.json` & `cg-60.4.7/tests/fixtures/analysis/taxprofiler/multiqc_data.json`

 * *Files identical despite different names*

### Comparing `cg-60.4.6/tests/fixtures/analysis/taxprofiler/taxprofiler_case_metrics_deliverables.yaml` & `cg-60.4.7/tests/fixtures/analysis/taxprofiler/taxprofiler_case_metrics_deliverables.yaml`

 * *Files identical despite different names*

### Comparing `cg-60.4.6/tests/fixtures/analysis/tomte/multiqc_data.json` & `cg-60.4.7/tests/fixtures/analysis/tomte/multiqc_data.json`

 * *Files identical despite different names*

### Comparing `cg-60.4.6/tests/fixtures/analysis/tomte/tomte_case_enough_reads_metrics_deliverables.yaml` & `cg-60.4.7/tests/fixtures/analysis/tomte/tomte_case_enough_reads_metrics_deliverables.yaml`

 * *Files identical despite different names*

### Comparing `cg-60.4.6/tests/fixtures/apps/balsamic/case/config.json` & `cg-60.4.7/tests/fixtures/apps/balsamic/case/config.json`

 * *Files identical despite different names*

### Comparing `cg-60.4.6/tests/fixtures/apps/balsamic/case/metadata.yml` & `cg-60.4.7/tests/fixtures/apps/balsamic/case/metadata.yml`

 * *Files identical despite different names*

### Comparing `cg-60.4.6/tests/fixtures/apps/balsamic/case/metrics_deliverables.yaml` & `cg-60.4.7/tests/fixtures/apps/balsamic/case/metrics_deliverables.yaml`

 * *Files identical despite different names*

### Comparing `cg-60.4.6/tests/fixtures/apps/crunchy/spring_metadata.json` & `cg-60.4.7/tests/fixtures/apps/crunchy/spring_metadata.json`

 * *Files identical despite different names*

### Comparing `cg-60.4.6/tests/fixtures/apps/demultiplexing/demultiplexed-runs/170517_ST-E00266_0210_BHJCFFALXX/Reports/Quality_Metrics.csv` & `cg-60.4.7/tests/fixtures/apps/demultiplexing/demultiplexed-runs/170517_ST-E00266_0210_BHJCFFALXX/Reports/Quality_Metrics.csv`

 * *Files identical despite different names*

### Comparing `cg-60.4.6/tests/fixtures/apps/demultiplexing/demultiplexed-runs/201203_D00483_0200_AHVKJCDRXX/HVKJCDRXX_demultiplex.stderr` & `cg-60.4.7/tests/fixtures/apps/demultiplexing/demultiplexed-runs/201203_D00483_0200_AHVKJCDRXX/HVKJCDRXX_demultiplex.stderr`

 * *Files identical despite different names*

### Comparing `cg-60.4.6/tests/fixtures/apps/demultiplexing/demultiplexed-runs/201203_D00483_0200_AHVKJCDRXX/Unaligned/Stats/ConversionStats.xml` & `cg-60.4.7/tests/fixtures/apps/demultiplexing/demultiplexed-runs/201203_D00483_0200_AHVKJCDRXX/Unaligned/Stats/ConversionStats.xml`

 * *Files identical despite different names*

### Comparing `cg-60.4.6/tests/fixtures/apps/demultiplexing/demultiplexed-runs/201203_D00483_0200_AHVKJCDRXX/Unaligned/Stats/DemultiplexingStats.xml` & `cg-60.4.7/tests/fixtures/apps/demultiplexing/demultiplexed-runs/201203_D00483_0200_AHVKJCDRXX/Unaligned/Stats/DemultiplexingStats.xml`

 * *Files identical despite different names*

### Comparing `cg-60.4.6/tests/fixtures/apps/demultiplexing/demultiplexed-runs/211101_A00187_0615_AHLG5GDRZZ/Unaligned/Reports/RunInfo.xml` & `cg-60.4.7/tests/fixtures/apps/demultiplexing/demultiplexed-runs/211101_A00187_0615_AHLG5GDRZZ/Unaligned/Reports/RunInfo.xml`

 * *Files identical despite different names*

### Comparing `cg-60.4.6/tests/fixtures/apps/demultiplexing/demultiplexed-runs-unfinished/201203_D00483_0200_AHVKJCDRXX/Unaligned/Stats/ConversionStats.xml` & `cg-60.4.7/tests/fixtures/apps/demultiplexing/demultiplexed-runs-unfinished/201203_D00483_0200_AHVKJCDRXX/Unaligned/Stats/ConversionStats.xml`

 * *Files identical despite different names*

### Comparing `cg-60.4.6/tests/fixtures/apps/demultiplexing/demultiplexed-runs-unfinished/201203_D00483_0200_AHVKJCDRXX/Unaligned/Stats/DemultiplexingStats.xml` & `cg-60.4.7/tests/fixtures/apps/demultiplexing/demultiplexed-runs-unfinished/201203_D00483_0200_AHVKJCDRXX/Unaligned/Stats/DemultiplexingStats.xml`

 * *Files identical despite different names*

### Comparing `cg-60.4.6/tests/fixtures/apps/demultiplexing/demultiplexed-runs-unfinished/230912_A00187_1009_AHK33MDRX3/SampleSheet.csv` & `cg-60.4.7/tests/fixtures/apps/demultiplexing/demultiplexed-runs-unfinished/230912_A00187_1009_AHK33MDRX3/SampleSheet.csv`

 * *Files identical despite different names*

### Comparing `cg-60.4.6/tests/fixtures/apps/demultiplexing/fastq/fastq_run_R1_001.fastq.gz` & `cg-60.4.7/tests/fixtures/apps/demultiplexing/fastq/fastq_run_R1_001.fastq.gz`

 * *Files identical despite different names*

### Comparing `cg-60.4.6/tests/fixtures/apps/demultiplexing/fastq/fastq_run_R2_001.fastq.gz` & `cg-60.4.7/tests/fixtures/apps/demultiplexing/fastq/fastq_run_R2_001.fastq.gz`

 * *Files identical despite different names*

### Comparing `cg-60.4.6/tests/fixtures/apps/demultiplexing/flow_cells/170517_ST-E00266_0210_BHJCFFALXX/HJCFFALXX_bcl2fastq_raw.json` & `cg-60.4.7/tests/fixtures/apps/demultiplexing/flow_cells/170517_ST-E00266_0210_BHJCFFALXX/HJCFFALXX_bcl2fastq_raw.json`

 * *Files identical despite different names*

### Comparing `cg-60.4.6/tests/fixtures/apps/demultiplexing/flow_cells/170517_ST-E00266_0210_BHJCFFALXX/HJCFFALXX_bcl_convert_raw.json` & `cg-60.4.7/tests/fixtures/apps/demultiplexing/flow_cells/170517_ST-E00266_0210_BHJCFFALXX/HJCFFALXX_bcl_convert_raw.json`

 * *Files identical despite different names*

### Comparing `cg-60.4.6/tests/fixtures/apps/demultiplexing/flow_cells/170517_ST-E00266_0210_BHJCFFALXX/RTAConfiguration.xml` & `cg-60.4.7/tests/fixtures/apps/demultiplexing/flow_cells/170517_ST-E00266_0210_BHJCFFALXX/RTAConfiguration.xml`

 * *Files identical despite different names*

### Comparing `cg-60.4.6/tests/fixtures/apps/demultiplexing/flow_cells/170517_ST-E00266_0210_BHJCFFALXX/RunInfo.xml` & `cg-60.4.7/tests/fixtures/apps/demultiplexing/flow_cells/170517_ST-E00266_0210_BHJCFFALXX/RunInfo.xml`

 * *Files identical despite different names*

### Comparing `cg-60.4.6/tests/fixtures/apps/demultiplexing/flow_cells/170517_ST-E00266_0210_BHJCFFALXX/SampleSheet.csv` & `cg-60.4.7/tests/fixtures/apps/demultiplexing/flow_cells/170517_ST-E00266_0210_BHJCFFALXX/SampleSheet.csv`

 * *Files identical despite different names*

### Comparing `cg-60.4.6/tests/fixtures/apps/demultiplexing/flow_cells/170517_ST-E00266_0210_BHJCFFALXX/SampleSheet_bcl2fastq.csv` & `cg-60.4.7/tests/fixtures/apps/demultiplexing/flow_cells/170517_ST-E00266_0210_BHJCFFALXX/SampleSheet_bcl2fastq.csv`

 * *Files identical despite different names*

### Comparing `cg-60.4.6/tests/fixtures/apps/demultiplexing/flow_cells/170517_ST-E00266_0210_BHJCFFALXX/runParameters.xml` & `cg-60.4.7/tests/fixtures/apps/demultiplexing/flow_cells/170517_ST-E00266_0210_BHJCFFALXX/runParameters.xml`

 * *Files identical despite different names*

### Comparing `cg-60.4.6/tests/fixtures/apps/demultiplexing/flow_cells/180508_ST-E00269_0269_AHL32LCCXY/HL32LCCXY_bcl2fastq_raw.json` & `cg-60.4.7/tests/fixtures/apps/demultiplexing/flow_cells/180508_ST-E00269_0269_AHL32LCCXY/HL32LCCXY_bcl2fastq_raw.json`

 * *Files identical despite different names*

### Comparing `cg-60.4.6/tests/fixtures/apps/demultiplexing/flow_cells/180508_ST-E00269_0269_AHL32LCCXY/HL32LCCXY_bcl_convert_raw.json` & `cg-60.4.7/tests/fixtures/apps/demultiplexing/flow_cells/180508_ST-E00269_0269_AHL32LCCXY/HL32LCCXY_bcl_convert_raw.json`

 * *Files identical despite different names*

### Comparing `cg-60.4.6/tests/fixtures/apps/demultiplexing/flow_cells/180508_ST-E00269_0269_AHL32LCCXY/RTAConfiguration.xml` & `cg-60.4.7/tests/fixtures/apps/demultiplexing/flow_cells/180508_ST-E00269_0269_AHL32LCCXY/RTAConfiguration.xml`

 * *Files identical despite different names*

### Comparing `cg-60.4.6/tests/fixtures/apps/demultiplexing/flow_cells/180508_ST-E00269_0269_AHL32LCCXY/RunInfo.xml` & `cg-60.4.7/tests/fixtures/apps/demultiplexing/flow_cells/180508_ST-E00269_0269_AHL32LCCXY/RunInfo.xml`

 * *Files identical despite different names*

### Comparing `cg-60.4.6/tests/fixtures/apps/demultiplexing/flow_cells/180508_ST-E00269_0269_AHL32LCCXY/SampleSheet.csv` & `cg-60.4.7/tests/fixtures/apps/demultiplexing/flow_cells/180508_ST-E00269_0269_AHL32LCCXY/SampleSheet.csv`

 * *Files identical despite different names*

### Comparing `cg-60.4.6/tests/fixtures/apps/demultiplexing/flow_cells/180508_ST-E00269_0269_AHL32LCCXY/SampleSheet_bcl2fastq.csv` & `cg-60.4.7/tests/fixtures/apps/demultiplexing/flow_cells/180508_ST-E00269_0269_AHL32LCCXY/SampleSheet_bcl2fastq.csv`

 * *Files identical despite different names*

### Comparing `cg-60.4.6/tests/fixtures/apps/demultiplexing/flow_cells/180508_ST-E00269_0269_AHL32LCCXY/runParameters.xml` & `cg-60.4.7/tests/fixtures/apps/demultiplexing/flow_cells/180508_ST-E00269_0269_AHL32LCCXY/runParameters.xml`

 * *Files identical despite different names*

### Comparing `cg-60.4.6/tests/fixtures/apps/demultiplexing/flow_cells/180509_D00450_0598_BHGYFNBCX2/HGYFNBCX2_bcl2fastq_raw.json` & `cg-60.4.7/tests/fixtures/apps/demultiplexing/flow_cells/180509_D00450_0598_BHGYFNBCX2/HGYFNBCX2_bcl2fastq_raw.json`

 * *Files identical despite different names*

### Comparing `cg-60.4.6/tests/fixtures/apps/demultiplexing/flow_cells/180509_D00450_0598_BHGYFNBCX2/HGYFNBCX2_bcl_convert_raw.json` & `cg-60.4.7/tests/fixtures/apps/demultiplexing/flow_cells/180509_D00450_0598_BHGYFNBCX2/HGYFNBCX2_bcl_convert_raw.json`

 * *Files identical despite different names*

### Comparing `cg-60.4.6/tests/fixtures/apps/demultiplexing/flow_cells/180509_D00450_0598_BHGYFNBCX2/RunInfo.xml` & `cg-60.4.7/tests/fixtures/apps/demultiplexing/flow_cells/180509_D00450_0598_BHGYFNBCX2/RunInfo.xml`

 * *Files identical despite different names*

### Comparing `cg-60.4.6/tests/fixtures/apps/demultiplexing/flow_cells/180509_D00450_0598_BHGYFNBCX2/SampleSheet.csv` & `cg-60.4.7/tests/fixtures/apps/demultiplexing/flow_cells/180509_D00450_0598_BHGYFNBCX2/SampleSheet.csv`

 * *Files identical despite different names*

### Comparing `cg-60.4.6/tests/fixtures/apps/demultiplexing/flow_cells/180509_D00450_0598_BHGYFNBCX2/SampleSheet_bcl2fastq.csv` & `cg-60.4.7/tests/fixtures/apps/demultiplexing/flow_cells/180509_D00450_0598_BHGYFNBCX2/SampleSheet_bcl2fastq.csv`

 * *Files identical despite different names*

### Comparing `cg-60.4.6/tests/fixtures/apps/demultiplexing/flow_cells/180509_D00450_0598_BHGYFNBCX2/runParameters.xml` & `cg-60.4.7/tests/fixtures/apps/demultiplexing/flow_cells/180509_D00450_0598_BHGYFNBCX2/runParameters.xml`

 * *Files identical despite different names*

### Comparing `cg-60.4.6/tests/fixtures/apps/demultiplexing/flow_cells/181005_D00410_0735_BHM2LNBCX2/HM2LNBCX2_bcl2fastq_raw.json` & `cg-60.4.7/tests/fixtures/apps/demultiplexing/flow_cells/181005_D00410_0735_BHM2LNBCX2/HM2LNBCX2_bcl2fastq_raw.json`

 * *Files identical despite different names*

### Comparing `cg-60.4.6/tests/fixtures/apps/demultiplexing/flow_cells/181005_D00410_0735_BHM2LNBCX2/HM2LNBCX2_bcl_convert_raw.json` & `cg-60.4.7/tests/fixtures/apps/demultiplexing/flow_cells/181005_D00410_0735_BHM2LNBCX2/HM2LNBCX2_bcl_convert_raw.json`

 * *Files identical despite different names*

### Comparing `cg-60.4.6/tests/fixtures/apps/demultiplexing/flow_cells/181005_D00410_0735_BHM2LNBCX2/RunInfo.xml` & `cg-60.4.7/tests/fixtures/apps/demultiplexing/flow_cells/181005_D00410_0735_BHM2LNBCX2/RunInfo.xml`

 * *Files identical despite different names*

### Comparing `cg-60.4.6/tests/fixtures/apps/demultiplexing/flow_cells/181005_D00410_0735_BHM2LNBCX2/SampleSheet.csv` & `cg-60.4.7/tests/fixtures/apps/demultiplexing/flow_cells/181005_D00410_0735_BHM2LNBCX2/SampleSheet.csv`

 * *Files identical despite different names*

### Comparing `cg-60.4.6/tests/fixtures/apps/demultiplexing/flow_cells/181005_D00410_0735_BHM2LNBCX2/SampleSheet_bcl2fastq.csv` & `cg-60.4.7/tests/fixtures/apps/demultiplexing/flow_cells/181005_D00410_0735_BHM2LNBCX2/SampleSheet_bcl2fastq.csv`

 * *Files identical despite different names*

### Comparing `cg-60.4.6/tests/fixtures/apps/demultiplexing/flow_cells/181005_D00410_0735_BHM2LNBCX2/runParameters.xml` & `cg-60.4.7/tests/fixtures/apps/demultiplexing/flow_cells/181005_D00410_0735_BHM2LNBCX2/runParameters.xml`

 * *Files identical despite different names*

### Comparing `cg-60.4.6/tests/fixtures/apps/demultiplexing/flow_cells/190927_A00689_0069_BHLYWYDSXX/CorrectSampleSheet.csv` & `cg-60.4.7/tests/fixtures/apps/demultiplexing/flow_cells/190927_A00689_0069_BHLYWYDSXX/CorrectSampleSheet.csv`

 * *Files identical despite different names*

### Comparing `cg-60.4.6/tests/fixtures/apps/demultiplexing/flow_cells/190927_A00689_0069_BHLYWYDSXX/HLYWYDSXX_bcl2fastq_raw.json` & `cg-60.4.7/tests/fixtures/apps/demultiplexing/flow_cells/190927_A00689_0069_BHLYWYDSXX/HLYWYDSXX_bcl2fastq_raw.json`

 * *Files identical despite different names*

### Comparing `cg-60.4.6/tests/fixtures/apps/demultiplexing/flow_cells/190927_A00689_0069_BHLYWYDSXX/HLYWYDSXX_bcl_convert_raw.json` & `cg-60.4.7/tests/fixtures/apps/demultiplexing/flow_cells/190927_A00689_0069_BHLYWYDSXX/HLYWYDSXX_bcl_convert_raw.json`

 * *Files identical despite different names*

### Comparing `cg-60.4.6/tests/fixtures/apps/demultiplexing/flow_cells/190927_A00689_0069_BHLYWYDSXX/RTA3.cfg` & `cg-60.4.7/tests/fixtures/apps/demultiplexing/flow_cells/190927_A00689_0069_BHLYWYDSXX/RTA3.cfg`

 * *Files identical despite different names*

### Comparing `cg-60.4.6/tests/fixtures/apps/demultiplexing/flow_cells/190927_A00689_0069_BHLYWYDSXX/RunInfo.xml` & `cg-60.4.7/tests/fixtures/apps/demultiplexing/flow_cells/190927_A00689_0069_BHLYWYDSXX/RunInfo.xml`

 * *Files identical despite different names*

### Comparing `cg-60.4.6/tests/fixtures/apps/demultiplexing/flow_cells/190927_A00689_0069_BHLYWYDSXX/RunParameters.xml` & `cg-60.4.7/tests/fixtures/apps/demultiplexing/flow_cells/190927_A00689_0069_BHLYWYDSXX/RunParameters.xml`

 * *Files identical despite different names*

### Comparing `cg-60.4.6/tests/fixtures/apps/demultiplexing/flow_cells/201203_D00483_0200_AHVKJCDRXX/HVKJCDRXX_demultiplex.stderr` & `cg-60.4.7/tests/fixtures/apps/demultiplexing/flow_cells/201203_D00483_0200_AHVKJCDRXX/HVKJCDRXX_demultiplex.stderr`

 * *Files identical despite different names*

### Comparing `cg-60.4.6/tests/fixtures/apps/demultiplexing/flow_cells/201203_D00483_0200_AHVKJCDRXX/HVKJCDRXX_demultiplex.stdout` & `cg-60.4.7/tests/fixtures/apps/demultiplexing/flow_cells/201203_D00483_0200_AHVKJCDRXX/HVKJCDRXX_demultiplex.stdout`

 * *Files identical despite different names*

### Comparing `cg-60.4.6/tests/fixtures/apps/demultiplexing/flow_cells/201203_D00483_0200_AHVKJCDRXX/HVKJCDRXX_raw.json` & `cg-60.4.7/tests/fixtures/apps/demultiplexing/flow_cells/201203_D00483_0200_AHVKJCDRXX/HVKJCDRXX_raw.json`

 * *Files identical despite different names*

### Comparing `cg-60.4.6/tests/fixtures/apps/demultiplexing/flow_cells/201203_D00483_0200_AHVKJCDRXX/RunParameters.xml` & `cg-60.4.7/tests/fixtures/apps/demultiplexing/flow_cells/201203_D00483_0200_AHVKJCDRXX/RunParameters.xml`

 * *Files identical despite different names*

### Comparing `cg-60.4.6/tests/fixtures/apps/demultiplexing/flow_cells/20231108_LH00188_0028_B22F52TLT3/22F52TLT3_raw.json` & `cg-60.4.7/tests/fixtures/apps/demultiplexing/flow_cells/20231108_LH00188_0028_B22F52TLT3/22F52TLT3_raw.json`

 * *Files identical despite different names*

### Comparing `cg-60.4.6/tests/fixtures/apps/demultiplexing/flow_cells/20231108_LH00188_0028_B22F52TLT3/CorrectSampleSheet.csv` & `cg-60.4.7/tests/fixtures/apps/demultiplexing/flow_cells/20231108_LH00188_0028_B22F52TLT3/CorrectSampleSheet.csv`

 * *Files identical despite different names*

### Comparing `cg-60.4.6/tests/fixtures/apps/demultiplexing/flow_cells/20231108_LH00188_0028_B22F52TLT3/RTA.cfg` & `cg-60.4.7/tests/fixtures/apps/demultiplexing/flow_cells/20231108_LH00188_0028_B22F52TLT3/RTA.cfg`

 * *Files identical despite different names*

### Comparing `cg-60.4.6/tests/fixtures/apps/demultiplexing/flow_cells/20231108_LH00188_0028_B22F52TLT3/RunCompletionStatus.xml` & `cg-60.4.7/tests/fixtures/apps/demultiplexing/flow_cells/20231108_LH00188_0028_B22F52TLT3/RunCompletionStatus.xml`

 * *Files identical despite different names*

### Comparing `cg-60.4.6/tests/fixtures/apps/demultiplexing/flow_cells/20231108_LH00188_0028_B22F52TLT3/RunInfo.xml` & `cg-60.4.7/tests/fixtures/apps/demultiplexing/flow_cells/20231108_LH00188_0028_B22F52TLT3/RunInfo.xml`

 * *Files identical despite different names*

### Comparing `cg-60.4.6/tests/fixtures/apps/demultiplexing/flow_cells/20231108_LH00188_0028_B22F52TLT3/RunParameters.xml` & `cg-60.4.7/tests/fixtures/apps/demultiplexing/flow_cells/20231108_LH00188_0028_B22F52TLT3/RunParameters.xml`

 * *Files identical despite different names*

### Comparing `cg-60.4.6/tests/fixtures/apps/demultiplexing/flow_cells/20231108_LH00188_0028_B22F52TLT3/SampleSheet.csv` & `cg-60.4.7/tests/fixtures/apps/demultiplexing/flow_cells/20231108_LH00188_0028_B22F52TLT3/SampleSheet.csv`

 * *Files identical despite different names*

### Comparing `cg-60.4.6/tests/fixtures/apps/demultiplexing/flow_cells/211101_A00187_0615_AHLG5GDRZZ/HLG5GDRZZ_demultiplex.stdout` & `cg-60.4.7/tests/fixtures/apps/demultiplexing/flow_cells/211101_A00187_0615_AHLG5GDRZZ/HLG5GDRZZ_demultiplex.stdout`

 * *Files identical despite different names*

### Comparing `cg-60.4.6/tests/fixtures/apps/demultiplexing/flow_cells/211101_A00187_0615_AHLG5GDRZZ/RunParameters.xml` & `cg-60.4.7/tests/fixtures/apps/demultiplexing/flow_cells/211101_A00187_0615_AHLG5GDRZZ/RunParameters.xml`

 * *Files identical despite different names*

### Comparing `cg-60.4.6/tests/fixtures/apps/demultiplexing/flow_cells/211101_A00187_0615_AHLG5GDRZZ/SampleSheet.csv` & `cg-60.4.7/tests/fixtures/apps/demultiplexing/flow_cells/211101_A00187_0615_AHLG5GDRZZ/SampleSheet.csv`

 * *Files identical despite different names*

### Comparing `cg-60.4.6/tests/fixtures/apps/demultiplexing/flow_cells/230912_A00187_1009_AHK33MDRX3/CorrectSampleSheet.csv` & `cg-60.4.7/tests/fixtures/apps/demultiplexing/flow_cells/230912_A00187_1009_AHK33MDRX3/CorrectSampleSheet.csv`

 * *Files identical despite different names*

### Comparing `cg-60.4.6/tests/fixtures/apps/demultiplexing/flow_cells/230912_A00187_1009_AHK33MDRX3/HK33MDRX3_bcl_convert_raw.json` & `cg-60.4.7/tests/fixtures/apps/demultiplexing/flow_cells/230912_A00187_1009_AHK33MDRX3/HK33MDRX3_bcl_convert_raw.json`

 * *Files identical despite different names*

### Comparing `cg-60.4.6/tests/fixtures/apps/demultiplexing/flow_cells/230912_A00187_1009_AHK33MDRX3/RTA3.cfg` & `cg-60.4.7/tests/fixtures/apps/demultiplexing/flow_cells/230912_A00187_1009_AHK33MDRX3/RTA3.cfg`

 * *Files identical despite different names*

### Comparing `cg-60.4.6/tests/fixtures/apps/demultiplexing/flow_cells/230912_A00187_1009_AHK33MDRX3/RunInfo.xml` & `cg-60.4.7/tests/fixtures/apps/demultiplexing/flow_cells/230912_A00187_1009_AHK33MDRX3/RunInfo.xml`

 * *Files identical despite different names*

### Comparing `cg-60.4.6/tests/fixtures/apps/demultiplexing/flow_cells/230912_A00187_1009_AHK33MDRX3/RunParameters.xml` & `cg-60.4.7/tests/fixtures/apps/demultiplexing/flow_cells/230912_A00187_1009_AHK33MDRX3/RunParameters.xml`

 * *Files identical despite different names*

### Comparing `cg-60.4.6/tests/fixtures/apps/demultiplexing/flow_cells/230912_A00187_1009_AHK33MDRX3/SampleSheet.csv` & `cg-60.4.7/tests/fixtures/apps/demultiplexing/flow_cells/230912_A00187_1009_AHK33MDRX3/SampleSheet.csv`

 * *Files identical despite different names*

### Comparing `cg-60.4.6/tests/fixtures/apps/demultiplexing/flow_cells_broken/170517_ST-E00266_0210_BHJCFFALXX/SampleSheet.csv` & `cg-60.4.7/tests/fixtures/apps/demultiplexing/flow_cells_broken/170517_ST-E00266_0210_BHJCFFALXX/SampleSheet.csv`

 * *Files identical despite different names*

### Comparing `cg-60.4.6/tests/fixtures/apps/demultiplexing/flow_cells_broken/170517_ST-E00266_0210_BHJCFFALXX/runParameters.xml` & `cg-60.4.7/tests/fixtures/apps/demultiplexing/flow_cells_broken/170517_ST-E00266_0210_BHJCFFALXX/runParameters.xml`

 * *Files identical despite different names*

### Comparing `cg-60.4.6/tests/fixtures/apps/demultiplexing/flow_cells_broken/190927_A00689_0069_BHLYWYDSXX/RunParameters.xml` & `cg-60.4.7/tests/fixtures/apps/demultiplexing/flow_cells_broken/190927_A00689_0069_BHLYWYDSXX/RunParameters.xml`

 * *Files identical despite different names*

### Comparing `cg-60.4.6/tests/fixtures/apps/demultiplexing/flow_cells_broken/20231108_LH00188_0028_B22F52TLT3/RunParameters.xml` & `cg-60.4.7/tests/fixtures/apps/demultiplexing/flow_cells_broken/20231108_LH00188_0028_B22F52TLT3/RunParameters.xml`

 * *Files identical despite different names*

### Comparing `cg-60.4.6/tests/fixtures/apps/demultiplexing/flow_cells_broken/230912_A00187_1009_AHK33MDRX3/RunParameters.xml` & `cg-60.4.7/tests/fixtures/apps/demultiplexing/flow_cells_broken/230912_A00187_1009_AHK33MDRX3/RunParameters.xml`

 * *Files identical despite different names*

### Comparing `cg-60.4.6/tests/fixtures/apps/demultiplexing/flow_cells_demux_all/211101_A00187_0615_AHLG5GDRXY/HLG5GDRXY_demultiplex.stdout` & `cg-60.4.7/tests/fixtures/apps/demultiplexing/flow_cells_demux_all/211101_A00187_0615_AHLG5GDRXY/HLG5GDRXY_demultiplex.stdout`

 * *Files identical despite different names*

### Comparing `cg-60.4.6/tests/fixtures/apps/demultiplexing/flow_cells_demux_all/211101_A00187_0615_AHLG5GDRXY/RunParameters.xml` & `cg-60.4.7/tests/fixtures/apps/demultiplexing/flow_cells_demux_all/211101_A00187_0615_AHLG5GDRXY/RunParameters.xml`

 * *Files identical despite different names*

### Comparing `cg-60.4.6/tests/fixtures/apps/demultiplexing/flow_cells_demux_all/211101_A00187_0615_AHLG5GDRZZ/HLG5GDRZZ_demultiplex.stdout` & `cg-60.4.7/tests/fixtures/apps/demultiplexing/flow_cells_demux_all/211101_A00187_0615_AHLG5GDRZZ/HLG5GDRZZ_demultiplex.stdout`

 * *Files identical despite different names*

### Comparing `cg-60.4.6/tests/fixtures/apps/demultiplexing/flow_cells_demux_all/211101_A00187_0615_AHLG5GDRZZ/RunParameters.xml` & `cg-60.4.7/tests/fixtures/apps/demultiplexing/flow_cells_demux_all/211101_A00187_0615_AHLG5GDRZZ/RunParameters.xml`

 * *Files identical despite different names*

### Comparing `cg-60.4.6/tests/fixtures/apps/demultiplexing/run_parameters/RunParameters_hiseq_2500_different_index_cycles.xml` & `cg-60.4.7/tests/fixtures/apps/demultiplexing/run_parameters/RunParameters_hiseq_2500_different_index_cycles.xml`

 * *Files identical despite different names*

### Comparing `cg-60.4.6/tests/fixtures/apps/demultiplexing/run_parameters/RunParameters_novaseq_6000_different_index_cycles.xml` & `cg-60.4.7/tests/fixtures/apps/demultiplexing/run_parameters/RunParameters_novaseq_6000_different_index_cycles.xml`

 * *Files identical despite different names*

### Comparing `cg-60.4.6/tests/fixtures/apps/demultiplexing/run_parameters/RunParameters_novaseq_X_different_index_cycles.xml` & `cg-60.4.7/tests/fixtures/apps/demultiplexing/run_parameters/RunParameters_novaseq_X_different_index_cycles.xml`

 * *Files identical despite different names*

### Comparing `cg-60.4.6/tests/fixtures/apps/demultiplexing/run_parameters/RunParameters_novaseq_X_wrong_instrument.xml` & `cg-60.4.7/tests/fixtures/apps/demultiplexing/run_parameters/RunParameters_novaseq_X_wrong_instrument.xml`

 * *Files identical despite different names*

### Comparing `cg-60.4.6/tests/fixtures/apps/demultiplexing/run_parameters/RunParameters_novaseq_no_software_nor_reagent_version.xml` & `cg-60.4.7/tests/fixtures/apps/demultiplexing/run_parameters/RunParameters_novaseq_no_software_nor_reagent_version.xml`

 * *Files identical despite different names*

### Comparing `cg-60.4.6/tests/fixtures/apps/demultiplexing/sample_sheets/novaseq_6000_sample_sheet_with_reversed_cycles.csv` & `cg-60.4.7/tests/fixtures/apps/demultiplexing/sample_sheets/novaseq_6000_sample_sheet_with_reversed_cycles.csv`

 * *Files identical despite different names*

### Comparing `cg-60.4.6/tests/fixtures/apps/demultiplexing/sample_sheets/novaseq_x_sample_sheet_with_forward_cycles.csv` & `cg-60.4.7/tests/fixtures/apps/demultiplexing/sample_sheets/novaseq_x_sample_sheet_with_forward_cycles.csv`

 * *Files identical despite different names*

### Comparing `cg-60.4.6/tests/fixtures/apps/fluffy/SampleSheet.csv` & `cg-60.4.7/tests/fixtures/apps/fluffy/SampleSheet.csv`

 * *Files identical despite different names*

### Comparing `cg-60.4.6/tests/fixtures/apps/fluffy/deliverables.yaml` & `cg-60.4.7/tests/fixtures/apps/fluffy/deliverables.yaml`

 * *Files identical despite different names*

### Comparing `cg-60.4.6/tests/fixtures/apps/madeline/madeline.xml` & `cg-60.4.7/tests/fixtures/apps/madeline/madeline.xml`

 * *Files identical despite different names*

### Comparing `cg-60.4.6/tests/fixtures/apps/mip/case_metrics_deliverables.yaml` & `cg-60.4.7/tests/fixtures/apps/mip/case_metrics_deliverables.yaml`

 * *Files identical despite different names*

### Comparing `cg-60.4.6/tests/fixtures/apps/mip/dna/store/case_config.yaml` & `cg-60.4.7/tests/fixtures/apps/mip/dna/store/case_config.yaml`

 * *Files identical despite different names*

### Comparing `cg-60.4.6/tests/fixtures/apps/mip/dna/store/case_id_deliverables.yaml` & `cg-60.4.7/tests/fixtures/apps/mip/dna/store/case_id_deliverables.yaml`

 * *Files identical despite different names*

### Comparing `cg-60.4.6/tests/fixtures/apps/mip/dna/store/case_qc_sample_info.yaml` & `cg-60.4.7/tests/fixtures/apps/mip/dna/store/case_qc_sample_info.yaml`

 * *Files identical despite different names*

### Comparing `cg-60.4.6/tests/fixtures/apps/mip/dna/store/yellowhog_clinical_selected.vcf` & `cg-60.4.7/tests/fixtures/apps/mip/dna/store/yellowhog_clinical_selected.vcf`

 * *Files identical despite different names*

### Comparing `cg-60.4.6/tests/fixtures/apps/mip/rna/case_config.yaml` & `cg-60.4.7/tests/fixtures/apps/mip/rna/case_config.yaml`

 * *Files identical despite different names*

### Comparing `cg-60.4.6/tests/fixtures/apps/mip/rna/case_qc_sampleinfo.yaml` & `cg-60.4.7/tests/fixtures/apps/mip/rna/case_qc_sampleinfo.yaml`

 * *Files identical despite different names*

### Comparing `cg-60.4.6/tests/fixtures/apps/mip/rna/store/bundle_data.yaml` & `cg-60.4.7/tests/fixtures/apps/mip/rna/store/bundle_data.yaml`

 * *Files identical despite different names*

### Comparing `cg-60.4.6/tests/fixtures/apps/mip/rna/store/case_config.yaml` & `cg-60.4.7/tests/fixtures/apps/mip/rna/store/case_config.yaml`

 * *Files identical despite different names*

### Comparing `cg-60.4.6/tests/fixtures/apps/mip/rna/store/case_id_deliverables.yaml` & `cg-60.4.7/tests/fixtures/apps/mip/rna/store/case_id_deliverables.yaml`

 * *Files identical despite different names*

### Comparing `cg-60.4.6/tests/fixtures/apps/mip/rna/store/case_qc_sample_info.yaml` & `cg-60.4.7/tests/fixtures/apps/mip/rna/store/case_qc_sample_info.yaml`

 * *Files identical despite different names*

### Comparing `cg-60.4.6/tests/fixtures/apps/scout/643594.config.yaml` & `cg-60.4.7/tests/fixtures/apps/scout/643594.config.yaml`

 * *Files identical despite different names*

### Comparing `cg-60.4.6/tests/fixtures/apps/scout/case_export.json` & `cg-60.4.7/tests/fixtures/apps/scout/case_export.json`

 * *Files identical despite different names*

### Comparing `cg-60.4.6/tests/fixtures/apps/scout/export_causatives.json` & `cg-60.4.7/tests/fixtures/apps/scout/export_causatives.json`

 * *Files identical despite different names*

### Comparing `cg-60.4.6/tests/fixtures/apps/scout/none_case_export.json` & `cg-60.4.7/tests/fixtures/apps/scout/none_case_export.json`

 * *Files identical despite different names*

### Comparing `cg-60.4.6/tests/fixtures/apps/scout/other_sex_case.json` & `cg-60.4.7/tests/fixtures/apps/scout/other_sex_case.json`

 * *Files identical despite different names*

### Comparing `cg-60.4.6/tests/fixtures/apps/scout/panel_export.bed` & `cg-60.4.7/tests/fixtures/apps/scout/panel_export.bed`

 * *Files identical despite different names*

### Comparing `cg-60.4.6/tests/fixtures/apps/scout/panel_export.csv` & `cg-60.4.7/tests/fixtures/apps/scout/panel_export.csv`

 * *Files identical despite different names*

### Comparing `cg-60.4.6/tests/fixtures/apps/sequencing_metrics_parser/230622_A00621_0864_AHY7FFDRX2/SampleSheet.csv` & `cg-60.4.7/tests/fixtures/apps/sequencing_metrics_parser/230622_A00621_0864_AHY7FFDRX2/SampleSheet.csv`

 * *Files identical despite different names*

### Comparing `cg-60.4.6/tests/fixtures/apps/sequencing_metrics_parser/230622_A00621_0864_AHY7FFDRX2/Unaligned/Reports/Adapter_Metrics.csv` & `cg-60.4.7/tests/fixtures/apps/sequencing_metrics_parser/230622_A00621_0864_AHY7FFDRX2/Unaligned/Reports/Adapter_Metrics.csv`

 * *Files identical despite different names*

### Comparing `cg-60.4.6/tests/fixtures/apps/sequencing_metrics_parser/230622_A00621_0864_AHY7FFDRX2/Unaligned/Reports/Demultiplex_Stats.csv` & `cg-60.4.7/tests/fixtures/apps/sequencing_metrics_parser/230622_A00621_0864_AHY7FFDRX2/Unaligned/Reports/Demultiplex_Stats.csv`

 * *Files identical despite different names*

### Comparing `cg-60.4.6/tests/fixtures/apps/sequencing_metrics_parser/230622_A00621_0864_AHY7FFDRX2/Unaligned/Reports/Quality_Metrics.csv` & `cg-60.4.7/tests/fixtures/apps/sequencing_metrics_parser/230622_A00621_0864_AHY7FFDRX2/Unaligned/Reports/Quality_Metrics.csv`

 * *Files identical despite different names*

### Comparing `cg-60.4.6/tests/fixtures/cgweb_orders/balsamic.json` & `cg-60.4.7/tests/fixtures/cgweb_orders/balsamic.json`

 * *Files identical despite different names*

### Comparing `cg-60.4.6/tests/fixtures/cgweb_orders/fastq.json` & `cg-60.4.7/tests/fixtures/cgweb_orders/fastq.json`

 * *Files identical despite different names*

### Comparing `cg-60.4.6/tests/fixtures/cgweb_orders/metagenome.json` & `cg-60.4.7/tests/fixtures/cgweb_orders/metagenome.json`

 * *Files identical despite different names*

### Comparing `cg-60.4.6/tests/fixtures/cgweb_orders/microsalt.json` & `cg-60.4.7/tests/fixtures/cgweb_orders/microsalt.json`

 * *Files identical despite different names*

### Comparing `cg-60.4.6/tests/fixtures/cgweb_orders/mip.json` & `cg-60.4.7/tests/fixtures/cgweb_orders/mip.json`

 * *Files identical despite different names*

### Comparing `cg-60.4.6/tests/fixtures/cgweb_orders/mip_rna.json` & `cg-60.4.7/tests/fixtures/cgweb_orders/mip_rna.json`

 * *Files identical despite different names*

### Comparing `cg-60.4.6/tests/fixtures/cgweb_orders/rml.json` & `cg-60.4.7/tests/fixtures/cgweb_orders/rml.json`

 * *Files identical despite different names*

### Comparing `cg-60.4.6/tests/fixtures/cgweb_orders/rnafusion.json` & `cg-60.4.7/tests/fixtures/cgweb_orders/rnafusion.json`

 * *Files identical despite different names*

### Comparing `cg-60.4.6/tests/fixtures/cgweb_orders/sarscov2.json` & `cg-60.4.7/tests/fixtures/cgweb_orders/sarscov2.json`

 * *Files identical despite different names*

### Comparing `cg-60.4.6/tests/fixtures/data/SampleSheet.csv` & `cg-60.4.7/tests/fixtures/data/SampleSheet.csv`

 * *Files identical despite different names*

### Comparing `cg-60.4.6/tests/fixtures/data/cgfixture.db` & `cg-60.4.7/tests/fixtures/data/cgfixture.db`

 * *Files identical despite different names*

### Comparing `cg-60.4.6/tests/fixtures/data/hkstore.db` & `cg-60.4.7/tests/fixtures/data/hkstore.db`

 * *Files identical despite different names*

### Comparing `cg-60.4.6/tests/fixtures/io/example_json.json` & `cg-60.4.7/tests/fixtures/io/example_json.json`

 * *Files identical despite different names*

### Comparing `cg-60.4.6/tests/fixtures/orderforms/1508.30.balsamic.xlsx` & `cg-60.4.7/tests/fixtures/orderforms/1508.30.balsamic.xlsx`

 * *Files identical despite different names*

### Comparing `cg-60.4.6/tests/fixtures/orderforms/1508.30.balsamic_qc.xlsx` & `cg-60.4.7/tests/fixtures/orderforms/1508.30.balsamic_qc.xlsx`

 * *Files identical despite different names*

### Comparing `cg-60.4.6/tests/fixtures/orderforms/1508.30.balsamic_umi.xlsx` & `cg-60.4.7/tests/fixtures/orderforms/1508.30.balsamic_umi.xlsx`

 * *Files identical despite different names*

### Comparing `cg-60.4.6/tests/fixtures/orderforms/1508.30.fastq.xlsx` & `cg-60.4.7/tests/fixtures/orderforms/1508.30.fastq.xlsx`

 * *Files identical despite different names*

### Comparing `cg-60.4.6/tests/fixtures/orderforms/1508.30.metagenome.xlsx` & `cg-60.4.7/tests/fixtures/orderforms/1508.30.metagenome.xlsx`

 * *Files identical despite different names*

### Comparing `cg-60.4.6/tests/fixtures/orderforms/1508.30.mip.xlsx` & `cg-60.4.7/tests/fixtures/orderforms/1508.30.mip.xlsx`

 * *Files identical despite different names*

### Comparing `cg-60.4.6/tests/fixtures/orderforms/1508.30.mip_rna.xlsx` & `cg-60.4.7/tests/fixtures/orderforms/1508.30.mip_rna.xlsx`

 * *Files identical despite different names*

### Comparing `cg-60.4.6/tests/fixtures/orderforms/1508.30.rnafusion.xlsx` & `cg-60.4.7/tests/fixtures/orderforms/1508.30.rnafusion.xlsx`

 * *Files identical despite different names*

### Comparing `cg-60.4.6/tests/fixtures/orderforms/1603.11.microbial.xlsx` & `cg-60.4.7/tests/fixtures/orderforms/1603.11.microbial.xlsx`

 * *Files identical despite different names*

### Comparing `cg-60.4.6/tests/fixtures/orderforms/1604.17.rml.xlsx` & `cg-60.4.7/tests/fixtures/orderforms/1604.17.rml.xlsx`

 * *Files identical despite different names*

### Comparing `cg-60.4.6/tests/fixtures/orderforms/2184.9.sarscov2.xlsx` & `cg-60.4.7/tests/fixtures/orderforms/2184.9.sarscov2.xlsx`

 * *Files identical despite different names*

### Comparing `cg-60.4.6/tests/fixtures/orderforms/NIPT-json.json` & `cg-60.4.7/tests/fixtures/orderforms/NIPT-json.json`

 * *Files identical despite different names*

### Comparing `cg-60.4.6/tests/fixtures/orderforms/balsamic_uploaded_json_orderform.json` & `cg-60.4.7/tests/fixtures/orderforms/balsamic_uploaded_json_orderform.json`

 * *Files identical despite different names*

### Comparing `cg-60.4.6/tests/fixtures/orderforms/mip_uploaded_json_orderform.json` & `cg-60.4.7/tests/fixtures/orderforms/mip_uploaded_json_orderform.json`

 * *Files identical despite different names*

### Comparing `cg-60.4.6/tests/fixtures/report/case_data.json` & `cg-60.4.7/tests/fixtures/report/case_data.json`

 * *Files identical despite different names*

### Comparing `cg-60.4.6/tests/fixtures/report/lims_exported_samples.json` & `cg-60.4.7/tests/fixtures/report/lims_exported_samples.json`

 * *Files identical despite different names*

### Comparing `cg-60.4.6/tests/fixtures/report/lims_family.json` & `cg-60.4.7/tests/fixtures/report/lims_family.json`

 * *Files identical despite different names*

### Comparing `cg-60.4.6/tests/io/conftest.py` & `cg-60.4.7/tests/io/conftest.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.6/tests/io/test_io_controller.py` & `cg-60.4.7/tests/io/test_io_controller.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.6/tests/io/test_io_csv.py` & `cg-60.4.7/tests/io/test_io_csv.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.6/tests/io/test_io_json.py` & `cg-60.4.7/tests/io/test_io_json.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.6/tests/io/test_io_txt.py` & `cg-60.4.7/tests/io/test_io_txt.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.6/tests/io/test_io_xml.py` & `cg-60.4.7/tests/io/test_io_xml.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.6/tests/io/test_io_yaml.py` & `cg-60.4.7/tests/io/test_io_yaml.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.6/tests/io/test_validate_path.py` & `cg-60.4.7/tests/io/test_validate_path.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.6/tests/meta/archive/conftest.py` & `cg-60.4.7/tests/meta/archive/conftest.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.6/tests/meta/archive/test_archive_api.py` & `cg-60.4.7/tests/meta/archive/test_archive_api.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.6/tests/meta/archive/test_archive_cli.py` & `cg-60.4.7/tests/meta/archive/test_archive_cli.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.6/tests/meta/archive/test_archiving.py` & `cg-60.4.7/tests/meta/archive/test_archiving.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.6/tests/meta/backup/conftest.py` & `cg-60.4.7/tests/meta/backup/conftest.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.6/tests/meta/backup/test_meta_backup.py` & `cg-60.4.7/tests/meta/backup/test_meta_backup.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.6/tests/meta/backup/test_meta_pdc.py` & `cg-60.4.7/tests/meta/backup/test_meta_pdc.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.6/tests/meta/clean/conftest.py` & `cg-60.4.7/tests/meta/clean/conftest.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.6/tests/meta/clean/test_clean_flow_cells_api.py` & `cg-60.4.7/tests/meta/clean/test_clean_flow_cells_api.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.6/tests/meta/clean/test_clean_retrieved_spring_files.py` & `cg-60.4.7/tests/meta/clean/test_clean_retrieved_spring_files.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.6/tests/meta/compress/conftest.py` & `cg-60.4.7/tests/meta/compress/conftest.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.6/tests/meta/compress/test_clean_fastq.py` & `cg-60.4.7/tests/meta/compress/test_clean_fastq.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.6/tests/meta/compress/test_compress_files.py` & `cg-60.4.7/tests/meta/compress/test_compress_files.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.6/tests/meta/compress/test_compress_meta_fastq.py` & `cg-60.4.7/tests/meta/compress/test_compress_meta_fastq.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.6/tests/meta/compress/test_decompress_spring_meta.py` & `cg-60.4.7/tests/meta/compress/test_decompress_spring_meta.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.6/tests/meta/compress/test_meta_compress_update_hk.py` & `cg-60.4.7/tests/meta/compress/test_meta_compress_update_hk.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.6/tests/meta/conftest.py` & `cg-60.4.7/tests/meta/conftest.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.6/tests/meta/deliver/conftest.py` & `cg-60.4.7/tests/meta/deliver/conftest.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.6/tests/meta/deliver/test_deliver_ticket.py` & `cg-60.4.7/tests/meta/deliver/test_deliver_ticket.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.6/tests/meta/deliver/test_delivery_api.py` & `cg-60.4.7/tests/meta/deliver/test_delivery_api.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.6/tests/meta/deliver/test_fastq_path_generator.py` & `cg-60.4.7/tests/meta/deliver/test_fastq_path_generator.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.6/tests/meta/delivery/test_delivery_api.py` & `cg-60.4.7/tests/meta/delivery/test_delivery_api.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.6/tests/meta/demultiplex/conftest.py` & `cg-60.4.7/tests/meta/demultiplex/conftest.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.6/tests/meta/demultiplex/test_combine_sequencing_metrics.py` & `cg-60.4.7/tests/meta/demultiplex/test_combine_sequencing_metrics.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.6/tests/meta/demultiplex/test_demux_post_processing.py` & `cg-60.4.7/tests/meta/demultiplex/test_demux_post_processing.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.6/tests/meta/demultiplex/test_housekeeper_storage_functions.py` & `cg-60.4.7/tests/meta/demultiplex/test_housekeeper_storage_functions.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.6/tests/meta/demultiplex/test_status_db_storage_functions.py` & `cg-60.4.7/tests/meta/demultiplex/test_status_db_storage_functions.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.6/tests/meta/demultiplex/test_utils.py` & `cg-60.4.7/tests/meta/demultiplex/test_utils.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.6/tests/meta/demultiplex/test_validation.py` & `cg-60.4.7/tests/meta/demultiplex/test_validation.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.6/tests/meta/encryption/conftest.py` & `cg-60.4.7/tests/meta/encryption/conftest.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.6/tests/meta/encryption/test_encryption.py` & `cg-60.4.7/tests/meta/encryption/test_encryption.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.6/tests/meta/observations/conftest.py` & `cg-60.4.7/tests/meta/observations/conftest.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.6/tests/meta/observations/test_meta_upload_observations.py` & `cg-60.4.7/tests/meta/observations/test_meta_upload_observations.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.6/tests/meta/orders/conftest.py` & `cg-60.4.7/tests/meta/orders/conftest.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.6/tests/meta/orders/test_PoolSubmitter_validate_order.py` & `cg-60.4.7/tests/meta/orders/test_PoolSubmitter_validate_order.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.6/tests/meta/orders/test_SarsCov2Submitter_order_to_status.py` & `cg-60.4.7/tests/meta/orders/test_SarsCov2Submitter_order_to_status.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.6/tests/meta/orders/test_SarsCov2Submitter_store_order.py` & `cg-60.4.7/tests/meta/orders/test_SarsCov2Submitter_store_order.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.6/tests/meta/orders/test_SarsCov2Submitter_validate_order.py` & `cg-60.4.7/tests/meta/orders/test_SarsCov2Submitter_validate_order.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.6/tests/meta/orders/test_meta_orders_api.py` & `cg-60.4.7/tests/meta/orders/test_meta_orders_api.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.6/tests/meta/orders/test_meta_orders_lims.py` & `cg-60.4.7/tests/meta/orders/test_meta_orders_lims.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.6/tests/meta/orders/test_meta_orders_status.py` & `cg-60.4.7/tests/meta/orders/test_meta_orders_status.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.6/tests/meta/orders/test_rnafusion_submitter.py` & `cg-60.4.7/tests/meta/orders/test_rnafusion_submitter.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.6/tests/meta/orders/test_ticket_handler.py` & `cg-60.4.7/tests/meta/orders/test_ticket_handler.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.6/tests/meta/qc_metrics/conftest.py` & `cg-60.4.7/tests/meta/qc_metrics/conftest.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.6/tests/meta/qc_metrics/test_collect_qc_metrics.py` & `cg-60.4.7/tests/meta/qc_metrics/test_collect_qc_metrics.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.6/tests/meta/report/conftest.py` & `cg-60.4.7/tests/meta/report/conftest.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.6/tests/meta/report/test_balsamic_api.py` & `cg-60.4.7/tests/meta/report/test_balsamic_api.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.6/tests/meta/report/test_field_validators.py` & `cg-60.4.7/tests/meta/report/test_field_validators.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.6/tests/meta/report/test_mip_dna_api.py` & `cg-60.4.7/tests/meta/report/test_mip_dna_api.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.6/tests/meta/report/test_report_api.py` & `cg-60.4.7/tests/meta/report/test_report_api.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.6/tests/meta/report/test_rnafusion_api.py` & `cg-60.4.7/tests/meta/report/test_rnafusion_api.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.6/tests/meta/report/test_tomte_api.py` & `cg-60.4.7/tests/meta/report/test_tomte_api.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.6/tests/meta/rsync/conftest.py` & `cg-60.4.7/tests/meta/rsync/conftest.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.6/tests/meta/rsync/test_rsync.py` & `cg-60.4.7/tests/meta/rsync/test_rsync.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.6/tests/meta/test_invoice.py` & `cg-60.4.7/tests/meta/test_invoice.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.6/tests/meta/transfer/conftest.py` & `cg-60.4.7/tests/meta/transfer/conftest.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.6/tests/meta/transfer/test_external_data.py` & `cg-60.4.7/tests/meta/transfer/test_external_data.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.6/tests/meta/transfer/test_meta_transfer_lims.py` & `cg-60.4.7/tests/meta/transfer/test_meta_transfer_lims.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.6/tests/meta/upload/balsamic/test_balsamic.py` & `cg-60.4.7/tests/meta/upload/balsamic/test_balsamic.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.6/tests/meta/upload/conftest.py` & `cg-60.4.7/tests/meta/upload/conftest.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.6/tests/meta/upload/gisaid/fixtures/four_samples.csv` & `cg-60.4.7/tests/meta/upload/gisaid/fixtures/four_samples.csv`

 * *Files identical despite different names*

### Comparing `cg-60.4.6/tests/meta/upload/mutacc/conftest.py` & `cg-60.4.7/tests/meta/upload/mutacc/conftest.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.6/tests/meta/upload/mutacc/test_meta_upload_mutacc.py` & `cg-60.4.7/tests/meta/upload/mutacc/test_meta_upload_mutacc.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.6/tests/meta/upload/nipt/conftest.py` & `cg-60.4.7/tests/meta/upload/nipt/conftest.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.6/tests/meta/upload/nipt/test_models.py` & `cg-60.4.7/tests/meta/upload/nipt/test_models.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.6/tests/meta/upload/nipt/test_nipt_upload_api.py` & `cg-60.4.7/tests/meta/upload/nipt/test_nipt_upload_api.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.6/tests/meta/upload/scout/conftest.py` & `cg-60.4.7/tests/meta/upload/scout/conftest.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.6/tests/meta/upload/scout/test_generate_load_config.py` & `cg-60.4.7/tests/meta/upload/scout/test_generate_load_config.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.6/tests/meta/upload/scout/test_meta_upload_scoutapi.py` & `cg-60.4.7/tests/meta/upload/scout/test_meta_upload_scoutapi.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.6/tests/meta/upload/scout/test_meta_upload_scoutapi_rna.py` & `cg-60.4.7/tests/meta/upload/scout/test_meta_upload_scoutapi_rna.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.6/tests/meta/upload/scout/test_scout_config_builder.py` & `cg-60.4.7/tests/meta/upload/scout/test_scout_config_builder.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.6/tests/meta/upload/test_meta_upload_coverage.py` & `cg-60.4.7/tests/meta/upload/test_meta_upload_coverage.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.6/tests/meta/upload/test_upload_api.py` & `cg-60.4.7/tests/meta/upload/test_upload_api.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.6/tests/meta/upload/test_upload_genotypes_api.py` & `cg-60.4.7/tests/meta/upload/test_upload_genotypes_api.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.6/tests/meta/workflow/conftest.py` & `cg-60.4.7/tests/meta/workflow/conftest.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.6/tests/meta/workflow/microsalt/conftest.py` & `cg-60.4.7/tests/meta/workflow/microsalt/conftest.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.6/tests/meta/workflow/microsalt/test_quality_controller.py` & `cg-60.4.7/tests/meta/workflow/microsalt/test_quality_controller.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.6/tests/meta/workflow/microsalt/test_quality_controller_utils.py` & `cg-60.4.7/tests/meta/workflow/microsalt/test_quality_controller_utils.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.6/tests/meta/workflow/microsalt/test_report_generation.py` & `cg-60.4.7/tests/meta/workflow/microsalt/test_report_generation.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.6/tests/meta/workflow/test_analysis.py` & `cg-60.4.7/tests/meta/workflow/test_analysis.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.6/tests/meta/workflow/test_balsamic.py` & `cg-60.4.7/tests/meta/workflow/test_balsamic.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.6/tests/meta/workflow/test_fastq.py` & `cg-60.4.7/tests/meta/workflow/test_fastq.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.6/tests/meta/workflow/test_microsalt.py` & `cg-60.4.7/tests/meta/workflow/test_microsalt.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.6/tests/meta/workflow/test_nf_analysis.py` & `cg-60.4.7/tests/meta/workflow/test_nf_analysis.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.6/tests/meta/workflow/test_prepare_fastq_api.py` & `cg-60.4.7/tests/meta/workflow/test_prepare_fastq_api.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.6/tests/meta/workflow/test_raredisease.py` & `cg-60.4.7/tests/meta/workflow/test_raredisease.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.6/tests/meta/workflow/test_rnafusion.py` & `cg-60.4.7/tests/meta/workflow/test_rnafusion.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.6/tests/mocks/balsamic_analysis_mock.py` & `cg-60.4.7/tests/mocks/balsamic_analysis_mock.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.6/tests/mocks/crunchy.py` & `cg-60.4.7/tests/mocks/crunchy.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.6/tests/mocks/hk_mock.py` & `cg-60.4.7/tests/mocks/hk_mock.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.6/tests/mocks/limsmock.py` & `cg-60.4.7/tests/mocks/limsmock.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.6/tests/mocks/madeline.py` & `cg-60.4.7/tests/mocks/madeline.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.6/tests/mocks/mip_analysis_mock.py` & `cg-60.4.7/tests/mocks/mip_analysis_mock.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.6/tests/mocks/osticket.py` & `cg-60.4.7/tests/mocks/osticket.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.6/tests/mocks/process_mock.py` & `cg-60.4.7/tests/mocks/process_mock.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.6/tests/mocks/report.py` & `cg-60.4.7/tests/mocks/report.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.6/tests/mocks/scout.py` & `cg-60.4.7/tests/mocks/scout.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.6/tests/mocks/store_model.py` & `cg-60.4.7/tests/mocks/store_model.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.6/tests/mocks/tb_mock.py` & `cg-60.4.7/tests/mocks/tb_mock.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.6/tests/models/balsamic/conftest.py` & `cg-60.4.7/tests/models/balsamic/conftest.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.6/tests/models/balsamic/test_balsamic_analysis.py` & `cg-60.4.7/tests/models/balsamic/test_balsamic_analysis.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.6/tests/models/conftest.py` & `cg-60.4.7/tests/models/conftest.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.6/tests/models/demultiplexing/test_run_parameters.py` & `cg-60.4.7/tests/models/demultiplexing/test_run_parameters.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.6/tests/models/downsample/test_down_sample_meta_data.py` & `cg-60.4.7/tests/models/downsample/test_down_sample_meta_data.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.6/tests/models/flow_cell/test_flowcell_model.py` & `cg-60.4.7/tests/models/flow_cell/test_flowcell_model.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.6/tests/models/mip/conftest.py` & `cg-60.4.7/tests/models/mip/conftest.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.6/tests/models/mip/test_mip_analysis.py` & `cg-60.4.7/tests/models/mip/test_mip_analysis.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.6/tests/models/mip/test_mip_config.py` & `cg-60.4.7/tests/models/mip/test_mip_config.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.6/tests/models/mip/test_mip_metrics_deliverables.py` & `cg-60.4.7/tests/models/mip/test_mip_metrics_deliverables.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.6/tests/models/mip/test_mip_sample_info.py` & `cg-60.4.7/tests/models/mip/test_mip_sample_info.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.6/tests/models/nextflow/test_nextflow_deliver.py` & `cg-60.4.7/tests/models/nextflow/test_nextflow_deliver.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.6/tests/models/observations/conftest.py` & `cg-60.4.7/tests/models/observations/conftest.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.6/tests/models/observations/test_observations_input_files.py` & `cg-60.4.7/tests/models/observations/test_observations_input_files.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.6/tests/models/report/test_validators.py` & `cg-60.4.7/tests/models/report/test_validators.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.6/tests/models/rnafusion/test_rnafusion_sample.py` & `cg-60.4.7/tests/models/rnafusion/test_rnafusion_sample.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.6/tests/models/test_cg_models.py` & `cg-60.4.7/tests/models/test_cg_models.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.6/tests/models/test_compression_data.py` & `cg-60.4.7/tests/models/test_compression_data.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.6/tests/models/test_fastq.py` & `cg-60.4.7/tests/models/test_fastq.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.6/tests/models/test_file_data.py` & `cg-60.4.7/tests/models/test_file_data.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.6/tests/server/conftest.py` & `cg-60.4.7/tests/server/conftest.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.6/tests/server/endpoints/test_delivery_message_endpoint.py` & `cg-60.4.7/tests/server/endpoints/test_delivery_message_endpoint.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.6/tests/server/endpoints/test_orders_endpoint.py` & `cg-60.4.7/tests/server/endpoints/test_orders_endpoint.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.6/tests/services/fastq_file_service/conftest.py` & `cg-60.4.7/tests/services/fastq_file_service/conftest.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.6/tests/services/fastq_file_service/test_fastq_file_service.py` & `cg-60.4.7/tests/services/fastq_file_service/test_fastq_file_service.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.6/tests/services/orders/order_status_service/conftest.py` & `cg-60.4.7/tests/services/orders/order_status_service/conftest.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.6/tests/services/orders/order_status_service/test_order_summary_service.py` & `cg-60.4.7/tests/services/orders/order_status_service/test_order_summary_service.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.6/tests/services/quality_controller/test_sequencing_quality_checks_utils.py` & `cg-60.4.7/tests/services/quality_controller/test_sequencing_quality_checks_utils.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.6/tests/store/api/conftest.py` & `cg-60.4.7/tests/store/api/conftest.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.6/tests/store/api/test_base.py` & `cg-60.4.7/tests/store/api/test_base.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.6/tests/store/conftest.py` & `cg-60.4.7/tests/store/conftest.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.6/tests/store/crud/add/test_store_add_application_version.py` & `cg-60.4.7/tests/store/crud/add/test_store_add_application_version.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.6/tests/store/crud/add/test_store_add_base.py` & `cg-60.4.7/tests/store/crud/add/test_store_add_base.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.6/tests/store/crud/add/test_store_add_customer.py` & `cg-60.4.7/tests/store/crud/add/test_store_add_customer.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.6/tests/store/crud/add/test_store_add_flow_celll.py` & `cg-60.4.7/tests/store/crud/add/test_store_add_flow_celll.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.6/tests/store/crud/conftest.py` & `cg-60.4.7/tests/store/crud/conftest.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.6/tests/store/crud/delete/test_delete.py` & `cg-60.4.7/tests/store/crud/delete/test_delete.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.6/tests/store/crud/read/test_read.py` & `cg-60.4.7/tests/store/crud/read/test_read.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.6/tests/store/crud/read/test_read_analyses_to_clean.py` & `cg-60.4.7/tests/store/crud/read/test_read_analyses_to_clean.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.6/tests/store/crud/read/test_read_analyses_to_delivery_report.py` & `cg-60.4.7/tests/store/crud/read/test_read_analyses_to_delivery_report.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.6/tests/store/crud/read/test_read_analysis.py` & `cg-60.4.7/tests/store/crud/read/test_read_analysis.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.6/tests/store/crud/read/test_read_application_version.py` & `cg-60.4.7/tests/store/crud/read/test_read_application_version.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.6/tests/store/crud/read/test_read_customer.py` & `cg-60.4.7/tests/store/crud/read/test_read_customer.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.6/tests/store/crud/read/test_read_pool.py` & `cg-60.4.7/tests/store/crud/read/test_read_pool.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.6/tests/store/crud/read/test_read_sample.py` & `cg-60.4.7/tests/store/crud/read/test_read_sample.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.6/tests/store/crud/update/test_update.py` & `cg-60.4.7/tests/store/crud/update/test_update.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.6/tests/store/filters/test_status_analyses_filters.py` & `cg-60.4.7/tests/store/filters/test_status_analyses_filters.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.6/tests/store/filters/test_status_application_filters.py` & `cg-60.4.7/tests/store/filters/test_status_application_filters.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.6/tests/store/filters/test_status_application_limitations_filters.py` & `cg-60.4.7/tests/store/filters/test_status_application_limitations_filters.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.6/tests/store/filters/test_status_application_version_filters.py` & `cg-60.4.7/tests/store/filters/test_status_application_version_filters.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.6/tests/store/filters/test_status_bed_filters.py` & `cg-60.4.7/tests/store/filters/test_status_bed_filters.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.6/tests/store/filters/test_status_bed_version_filters.py` & `cg-60.4.7/tests/store/filters/test_status_bed_version_filters.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.6/tests/store/filters/test_status_case_sample_filters.py` & `cg-60.4.7/tests/store/filters/test_status_case_sample_filters.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.6/tests/store/filters/test_status_cases_filters.py` & `cg-60.4.7/tests/store/filters/test_status_cases_filters.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.6/tests/store/filters/test_status_collaboration_filters.py` & `cg-60.4.7/tests/store/filters/test_status_collaboration_filters.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.6/tests/store/filters/test_status_customer_filters.py` & `cg-60.4.7/tests/store/filters/test_status_customer_filters.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.6/tests/store/filters/test_status_flow_cell_filters.py` & `cg-60.4.7/tests/store/filters/test_status_flow_cell_filters.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.6/tests/store/filters/test_status_invoice_filters.py` & `cg-60.4.7/tests/store/filters/test_status_invoice_filters.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.6/tests/store/filters/test_status_metrics_filters.py` & `cg-60.4.7/tests/store/filters/test_status_metrics_filters.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.6/tests/store/filters/test_status_organism_filters.py` & `cg-60.4.7/tests/store/filters/test_status_organism_filters.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.6/tests/store/filters/test_status_panel_filters.py` & `cg-60.4.7/tests/store/filters/test_status_panel_filters.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.6/tests/store/filters/test_status_pool_filters.py` & `cg-60.4.7/tests/store/filters/test_status_pool_filters.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.6/tests/store/filters/test_status_samples_filters.py` & `cg-60.4.7/tests/store/filters/test_status_samples_filters.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.6/tests/store/filters/test_status_user_filters.py` & `cg-60.4.7/tests/store/filters/test_status_user_filters.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.6/tests/store/test_delivery.py` & `cg-60.4.7/tests/store/test_delivery.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.6/tests/store/test_store_models.py` & `cg-60.4.7/tests/store/test_store_models.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.6/tests/store_helpers.py` & `cg-60.4.7/tests/store_helpers.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.6/tests/test_copy_novaseqx_flow_cell.py` & `cg-60.4.7/tests/test_copy_novaseqx_flow_cell.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.6/tests/test_store_helpers.py` & `cg-60.4.7/tests/test_store_helpers.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.6/tests/utils/conftest.py` & `cg-60.4.7/tests/utils/conftest.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.6/tests/utils/test_commands.py` & `cg-60.4.7/tests/utils/test_commands.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.6/tests/utils/test_date.py` & `cg-60.4.7/tests/utils/test_date.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.6/tests/utils/test_dict.py` & `cg-60.4.7/tests/utils/test_dict.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.6/tests/utils/test_dispatcher.py` & `cg-60.4.7/tests/utils/test_dispatcher.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.6/tests/utils/test_files.py` & `cg-60.4.7/tests/utils/test_files.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.6/tests/utils/test_time.py` & `cg-60.4.7/tests/utils/test_time.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.6/tests/utils/test_utils.py` & `cg-60.4.7/tests/utils/test_utils.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.6/PKG-INFO` & `cg-60.4.7/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cg
-Version: 60.4.6
+Version: 60.4.7
 Summary: Clinical Genomics command center
 Home-page: https://github.com/Clinical-Genomics/cg
 Author: Clinical Genomics
 Author-email: support@clinicalgenomics.se
 Requires-Python: >=3.9,<3.13
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
```

