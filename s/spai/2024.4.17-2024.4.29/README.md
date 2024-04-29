# Comparing `tmp/spai-2024.4.17.tar.gz` & `tmp/spai-2024.4.29.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "spai-2024.4.17.tar", max compression
+gzip compressed data, was "spai-2024.4.29.tar", max compression
```

## Comparing `spai-2024.4.17.tar` & `spai-2024.4.29.tar`

### file list

```diff
@@ -1,132 +1,133 @@
--rw-r--r--   0        0        0       57 2023-06-09 06:48:31.112024 spai-2024.4.17/README.md
--rw-r--r--   0        0        0      525 2024-04-17 12:41:17.311631 spai-2024.4.17/pyproject.toml
--rw-r--r--   0        0        0       27 2024-04-17 12:41:17.311631 spai-2024.4.17/spai/__init__.py
--rw-r--r--   0        0        0        1 2024-04-12 10:11:48.513337 spai-2024.4.17/spai/analytics/__init__.py
--rw-r--r--   0        0        0     5030 2024-04-16 13:43:54.585423 spai-2024.4.17/spai/analytics/forest_monitoring.py
--rw-r--r--   0        0        0      110 2024-04-16 13:43:54.585423 spai-2024.4.17/spai/analytics/utils.py
--rw-r--r--   0        0        0    13235 2024-04-16 13:43:54.589423 spai-2024.4.17/spai/analytics/water_quality.py
--rw-r--r--   0        0        0       96 2024-02-13 11:22:06.401893 spai-2024.4.17/spai/auth/__init__.py
--rw-r--r--   0        0        0     1210 2024-02-13 11:22:06.401893 spai-2024.4.17/spai/auth/auth.py
--rw-r--r--   0        0        0       99 2024-02-13 11:22:06.401893 spai-2024.4.17/spai/auth/is_logged.py
--rw-r--r--   0        0        0      161 2024-02-13 11:22:06.401893 spai-2024.4.17/spai/auth/logout.py
--rw-r--r--   0        0        0     7202 2024-04-15 14:42:23.329718 spai-2024.4.17/spai/cli.py
--rw-r--r--   0        0        0        0 2024-02-13 11:22:06.401893 spai-2024.4.17/spai/commands/__init__.py
--rw-r--r--   0        0        0     1017 2024-02-13 11:22:06.405893 spai-2024.4.17/spai/commands/auth.py
--rw-r--r--   0        0        0     1160 2024-03-13 09:12:15.507871 spai-2024.4.17/spai/commands/list.py
--rw-r--r--   0        0        0       86 2024-03-13 09:12:15.507871 spai-2024.4.17/spai/config/__init__.py
--rw-r--r--   0        0        0     3777 2024-04-17 08:20:38.264305 spai-2024.4.17/spai/config/validate.py
--rw-r--r--   0        0        0     1324 2024-03-13 09:12:15.507871 spai-2024.4.17/spai/config/vars.py
--rw-r--r--   0        0        0        0 2023-05-19 06:35:36.838003 spai-2024.4.17/spai/data/__init__.py
--rw-r--r--   0        0        0       49 2024-02-13 11:22:06.405893 spai-2024.4.17/spai/data/indices/__init__.py
--rw-r--r--   0        0        0       54 2024-02-13 11:22:06.405893 spai-2024.4.17/spai/data/indices/fwi/__init__.py
--rw-r--r--   0        0        0     3234 2024-02-13 11:22:06.405893 spai-2024.4.17/spai/data/indices/fwi/fwi_nasa.py
--rw-r--r--   0        0        0      608 2024-04-12 10:11:48.513337 spai-2024.4.17/spai/data/satellite/__init__.py
--rw-r--r--   0        0        0     3941 2024-02-13 11:22:06.405893 spai-2024.4.17/spai/data/satellite/download.py
--rw-r--r--   0        0        0     6332 2024-04-12 10:11:48.513337 spai-2024.4.17/spai/data/satellite/download_stac.py
--rw-r--r--   0        0        0      647 2023-10-30 11:07:40.852696 spai-2024.4.17/spai/data/satellite/explore.py
--rw-r--r--   0        0        0      725 2024-02-13 11:22:06.405893 spai-2024.4.17/spai/data/satellite/sentinelhub/SHCloudMaskDownloader.py
--rw-r--r--   0        0        0      758 2024-03-13 09:12:15.507871 spai-2024.4.17/spai/data/satellite/sentinelhub/SHDEM30Downloader 2.py
--rw-r--r--   0        0        0      758 2024-03-13 09:12:15.507871 spai-2024.4.17/spai/data/satellite/sentinelhub/SHDEM30Downloader 3.py
--rw-r--r--   0        0        0      758 2024-02-13 11:22:06.405893 spai-2024.4.17/spai/data/satellite/sentinelhub/SHDEM30Downloader.py
--rw-r--r--   0        0        0     3587 2024-02-13 11:22:06.405893 spai-2024.4.17/spai/data/satellite/sentinelhub/SHDownloader.py
--rw-r--r--   0        0        0     2584 2024-02-13 11:22:06.405893 spai-2024.4.17/spai/data/satellite/sentinelhub/SHExplorer.py
--rw-r--r--   0        0        0      854 2023-05-25 06:56:10.755647 spai-2024.4.17/spai/data/satellite/sentinelhub/SHS1Downloader.py
--rw-r--r--   0        0        0     1264 2023-10-30 11:07:40.856696 spai-2024.4.17/spai/data/satellite/sentinelhub/SHS2Downloader.py
--rw-r--r--   0        0        0      275 2023-05-25 06:56:56.219839 spai-2024.4.17/spai/data/satellite/sentinelhub/SHS2L1CDownloader.py
--rw-r--r--   0        0        0      276 2023-05-25 05:49:51.650010 spai-2024.4.17/spai/data/satellite/sentinelhub/SHS2L2ADownloader.py
--rw-r--r--   0        0        0      282 2024-02-13 11:22:06.405893 spai-2024.4.17/spai/data/satellite/sentinelhub/__init__.py
--rw-r--r--   0        0        0     2222 2024-04-12 10:11:48.513337 spai-2024.4.17/spai/data/satellite/stac/STACDownloader.py
--rw-r--r--   0        0        0      208 2024-04-12 10:11:48.513337 spai-2024.4.17/spai/data/satellite/stac/__init__.py
--rw-r--r--   0        0        0      461 2024-04-12 10:11:48.513337 spai-2024.4.17/spai/data/satellite/stac/aws/AWSDEM30Downloader.py
--rw-r--r--   0        0        0      461 2024-04-12 10:11:48.513337 spai-2024.4.17/spai/data/satellite/stac/aws/AWSDEM90Downloader.py
--rw-r--r--   0        0        0      876 2024-04-12 10:11:48.513337 spai-2024.4.17/spai/data/satellite/stac/aws/AWSDEMDownloader.py
--rw-r--r--   0        0        0      392 2024-04-12 10:11:48.513337 spai-2024.4.17/spai/data/satellite/stac/aws/AWSDownloader.py
--rw-r--r--   0        0        0     1951 2024-04-12 10:11:48.513337 spai-2024.4.17/spai/data/satellite/stac/aws/AWSS2L2ADownloader.py
--rw-r--r--   0        0        0      233 2024-04-12 10:11:48.513337 spai-2024.4.17/spai/data/satellite/stac/aws/__init__.py
--rw-r--r--   0        0        0      456 2024-04-12 10:11:48.513337 spai-2024.4.17/spai/data/satellite/stac/decorators.py
--rw-r--r--   0        0        0      716 2024-04-12 10:11:48.513337 spai-2024.4.17/spai/data/satellite/stac/pc/PCDownloader.py
--rw-r--r--   0        0        0      802 2024-04-12 10:11:48.517337 spai-2024.4.17/spai/data/satellite/stac/pc/PCS1GRDDownloader.py
--rw-r--r--   0        0        0      120 2024-04-11 11:16:27.098890 spai-2024.4.17/spai/data/satellite/stac/pc/__init__.py
--rw-r--r--   0        0        0     8905 2024-04-12 10:11:48.517337 spai-2024.4.17/spai/data/satellite/utils.py
--rw-r--r--   0        0        0       84 2024-02-13 11:22:06.405893 spai-2024.4.17/spai/data/vector/__init__.py
--rw-r--r--   0        0        0     5533 2024-02-13 11:22:06.405893 spai-2024.4.17/spai/data/vector/openstreetmap.py
--rw-r--r--   0        0        0       71 2024-02-13 11:22:06.405893 spai-2024.4.17/spai/errors/__init__.py
--rw-r--r--   0        0        0      308 2024-02-13 11:22:06.405893 spai-2024.4.17/spai/errors/auth.py
--rw-r--r--   0        0        0      156 2024-02-13 11:22:06.405893 spai-2024.4.17/spai/errors/mails.py
--rw-r--r--   0        0        0       29 2023-05-25 13:36:54.194947 spai-2024.4.17/spai/image/__init__.py
--rw-r--r--   0        0        0     1350 2023-10-30 11:07:40.856696 spai-2024.4.17/spai/image/utils.py
--rw-r--r--   0        0        0       95 2023-05-25 13:32:15.318266 spai-2024.4.17/spai/image/xyz/__init__.py
--rw-r--r--   0        0        0     2026 2023-05-25 13:32:39.966326 spai-2024.4.17/spai/image/xyz/cache.py
--rw-r--r--   0        0        0      575 2023-05-25 13:32:27.546296 spai-2024.4.17/spai/image/xyz/errors.py
--rw-r--r--   0        0        0     6924 2023-05-25 13:31:09.006104 spai-2024.4.17/spai/image/xyz/get_image_tile.py
--rw-r--r--   0        0        0     1828 2023-05-25 13:32:00.366229 spai-2024.4.17/spai/image/xyz/image_utils.py
--rw-r--r--   0        0        0       28 2024-02-13 11:22:06.405893 spai-2024.4.17/spai/mails/__init__.py
--rw-r--r--   0        0        0     1334 2024-02-13 11:22:06.405893 spai-2024.4.17/spai/mails/mimetypes.py
--rw-r--r--   0        0        0     2932 2024-02-13 11:22:06.405893 spai-2024.4.17/spai/mails/send.py
--rw-r--r--   0        0        0     4444 2024-04-17 12:22:14.977615 spai-2024.4.17/spai/models/Config.py
--rw-r--r--   0        0        0      984 2024-03-13 09:12:15.507871 spai-2024.4.17/spai/models/StorageConfig.py
--rw-r--r--   0        0        0       27 2024-02-13 11:22:06.405893 spai-2024.4.17/spai/models/__init__.py
--rw-r--r--   0        0        0      391 2024-02-13 11:22:06.405893 spai-2024.4.17/spai/processing/__init__.py
--rw-r--r--   0        0        0      669 2024-03-28 15:02:41.834449 spai-2024.4.17/spai/processing/autocategorize1D.py
--rw-r--r--   0        0        0      477 2024-02-13 11:22:06.405893 spai-2024.4.17/spai/processing/colorize_raster.py
--rw-r--r--   0        0        0      932 2024-02-13 11:22:06.405893 spai-2024.4.17/spai/processing/convert_array_to_vector.py
--rw-r--r--   0        0        0      291 2024-02-13 11:22:06.405893 spai-2024.4.17/spai/processing/mask_raster.py
--rw-r--r--   0        0        0      682 2024-02-13 11:22:06.405893 spai-2024.4.17/spai/processing/normalised_difference.py
--rw-r--r--   0        0        0     1239 2024-02-13 11:22:06.405893 spai-2024.4.17/spai/processing/px_count.py
--rw-r--r--   0        0        0      107 2024-02-13 11:22:06.405893 spai-2024.4.17/spai/processing/rasterio_mask.py
--rw-r--r--   0        0        0      266 2024-02-13 11:22:06.405893 spai-2024.4.17/spai/processing/read_raster.py
--rw-r--r--   0        0        0     1109 2024-04-16 13:43:54.589423 spai-2024.4.17/spai/processing/save_table.py
--rw-r--r--   0        0        0      496 2024-03-28 15:02:41.834449 spai-2024.4.17/spai/processing/utils.py
--rw-r--r--   0        0        0      475 2024-02-13 11:22:06.405893 spai-2024.4.17/spai/project/__init__.py
--rw-r--r--   0        0        0      466 2024-02-13 11:22:06.405893 spai-2024.4.17/spai/project/bck/GetLogs.py
--rw-r--r--   0        0        0     1018 2024-03-13 09:12:15.507871 spai-2024.4.17/spai/project/bck/InstallReqs 2.py
--rw-r--r--   0        0        0     1018 2024-03-13 09:12:15.507871 spai-2024.4.17/spai/project/bck/InstallReqs 3.py
--rw-r--r--   0        0        0      482 2024-02-13 11:22:06.405893 spai-2024.4.17/spai/project/bck/RunService.py
--rw-r--r--   0        0        0      492 2024-02-13 11:22:06.405893 spai-2024.4.17/spai/project/bck/ScheduleService.py
--rw-r--r--   0        0        0      510 2024-02-13 11:22:06.405893 spai-2024.4.17/spai/project/bck/StopService.py
--rw-r--r--   0        0        0     1578 2024-02-13 11:22:06.405893 spai-2024.4.17/spai/project/bck/main.py
--rw-r--r--   0        0        0      337 2024-02-13 11:22:06.405893 spai-2024.4.17/spai/project/delete_project.py
--rw-r--r--   0        0        0     2030 2024-04-17 08:22:35.960893 spai-2024.4.17/spai/project/deploy_folder.py
--rw-r--r--   0        0        0      407 2024-04-17 08:22:35.960893 spai-2024.4.17/spai/project/deploy_template.py
--rw-r--r--   0        0        0     1203 2024-02-13 11:22:06.405893 spai-2024.4.17/spai/project/download_template.py
--rw-r--r--   0        0        0      455 2024-02-13 11:22:06.405893 spai-2024.4.17/spai/project/get_logs.py
--rw-r--r--   0        0        0      242 2024-02-13 11:22:06.405893 spai-2024.4.17/spai/project/get_project_by_name.py
--rw-r--r--   0        0        0      172 2024-02-13 11:22:06.409893 spai-2024.4.17/spai/project/get_projects.py
--rw-r--r--   0        0        0      344 2024-02-13 11:22:06.409893 spai-2024.4.17/spai/project/get_service_by_name_type_project.py
--rw-r--r--   0        0        0     1616 2024-03-13 09:12:15.507871 spai-2024.4.17/spai/project/get_services.py
--rw-r--r--   0        0        0      525 2024-02-21 09:43:40.417670 spai-2024.4.17/spai/project/init_project.py
--rw-r--r--   0        0        0      726 2024-04-15 09:44:33.796059 spai-2024.4.17/spai/project/install_requirements.py
--rw-r--r--   0        0        0     5617 2024-02-27 12:31:33.913016 spai-2024.4.17/spai/project/project-template/README.md
--rw-r--r--   0        0        0      867 2024-03-13 09:12:15.507871 spai-2024.4.17/spai/project/project-template/apis/analytics/main.py
--rw-r--r--   0        0        0       36 2024-03-13 09:12:15.507871 spai-2024.4.17/spai/project/project-template/apis/analytics/requirements.txt
--rw-r--r--   0        0        0     1800 2024-03-13 09:12:15.507871 spai-2024.4.17/spai/project/project-template/apis/xyz/main.py
--rw-r--r--   0        0        0       88 2024-03-13 09:12:15.507871 spai-2024.4.17/spai/project/project-template/apis/xyz/requirements.txt
--rw-r--r--   0        0        0   748531 2024-03-13 09:12:15.511871 spai-2024.4.17/spai/project/project-template/notebooks/analytics/main.ipynb
--rw-r--r--   0        0        0       39 2024-03-13 09:12:15.511871 spai-2024.4.17/spai/project/project-template/notebooks/analytics/requirements.txt
--rw-r--r--   0        0        0     1602 2024-04-12 10:11:48.517337 spai-2024.4.17/spai/project/project-template/scripts/analytics/main.py
--rw-r--r--   0        0        0       30 2024-03-13 09:12:15.511871 spai-2024.4.17/spai/project/project-template/scripts/analytics/requirements.txt
--rw-r--r--   0        0        0     1076 2024-04-12 10:11:48.517337 spai-2024.4.17/spai/project/project-template/scripts/downloader/main.py
--rw-r--r--   0        0        0       85 2024-04-12 10:11:48.517337 spai-2024.4.17/spai/project/project-template/scripts/downloader/requirements.txt
--rw-r--r--   0        0        0      618 2024-03-13 09:12:15.511871 spai-2024.4.17/spai/project/project-template/spai.config.yaml
--rw-r--r--   0        0        0     1523 2024-04-12 10:11:48.517337 spai-2024.4.17/spai/project/project-template/uis/map/main.py
--rw-r--r--   0        0        0       23 2024-02-27 12:31:33.593015 spai-2024.4.17/spai/project/project-template/uis/map/requirements.txt
--rw-r--r--   0        0        0     5209 2024-04-17 09:38:49.162295 spai-2024.4.17/spai/project/run_local.py
--rw-r--r--   0        0        0      813 2024-03-13 09:12:15.511871 spai-2024.4.17/spai/project/stop_service.py
--rw-r--r--   0        0        0       38 2024-02-13 11:22:06.413893 spai-2024.4.17/spai/reports/__init__.py
--rw-r--r--   0        0        0     1328 2024-02-13 11:22:06.413893 spai-2024.4.17/spai/reports/generate.py
--rw-r--r--   0        0        0     4780 2024-04-17 08:20:38.264305 spai-2024.4.17/spai/repos/APIRepo.py
--rw-r--r--   0        0        0      997 2024-02-13 11:22:06.413893 spai-2024.4.17/spai/repos/AuthRepo.py
--rw-r--r--   0        0        0      188 2024-02-13 11:22:06.413893 spai-2024.4.17/spai/repos/MailsRepo.py
--rw-r--r--   0        0        0      200 2024-02-13 11:22:06.413893 spai-2024.4.17/spai/repos/ReportsRepo.py
--rw-r--r--   0        0        0       60 2024-02-13 11:22:06.413893 spai-2024.4.17/spai/repos/__init__.py
--rw-r--r--   0        0        0     2426 2024-04-17 08:20:38.264305 spai-2024.4.17/spai/storage/BaseStorage.py
--rw-r--r--   0        0        0     3716 2024-03-13 09:12:15.515871 spai-2024.4.17/spai/storage/CloudStorage.py
--rw-r--r--   0        0        0     4527 2024-04-11 11:16:27.098890 spai-2024.4.17/spai/storage/LocalStorage.py
--rw-r--r--   0        0        0     8449 2024-04-12 10:11:48.517337 spai-2024.4.17/spai/storage/S3Storage.py
--rw-r--r--   0        0        0     1407 2024-03-13 09:12:15.515871 spai-2024.4.17/spai/storage/Storage.py
--rw-r--r--   0        0        0     6077 2024-03-13 09:12:15.515871 spai-2024.4.17/spai/storage/_S3Storage.py
--rw-r--r--   0        0        0      120 2024-03-13 09:12:15.515871 spai-2024.4.17/spai/storage/__init__.py
--rw-r--r--   0        0        0      409 2024-03-13 09:12:15.515871 spai-2024.4.17/spai/storage/create_s3.py
--rw-r--r--   0        0        0     1559 2024-04-11 11:16:27.102890 spai-2024.4.17/spai/storage/decorators.py
--rw-r--r--   0        0        0      583 2024-03-13 09:12:15.515871 spai-2024.4.17/spai/storage/minio.py
--rw-r--r--   0        0        0      939 1970-01-01 00:00:00.000000 spai-2024.4.17/PKG-INFO
+-rw-r--r--   0        0        0       57 2024-04-29 10:40:31.981993 spai-2024.4.29/README.md
+-rw-r--r--   0        0        0      525 2024-04-29 11:06:53.893979 spai-2024.4.29/pyproject.toml
+-rw-r--r--   0        0        0       27 2024-04-29 11:06:53.897979 spai-2024.4.29/spai/__init__.py
+-rw-r--r--   0        0        0        1 2024-04-29 10:40:32.077990 spai-2024.4.29/spai/analytics/__init__.py
+-rw-r--r--   0        0        0     5030 2024-04-29 10:40:32.077990 spai-2024.4.29/spai/analytics/forest_monitoring.py
+-rw-r--r--   0        0        0      110 2024-04-29 10:40:32.077990 spai-2024.4.29/spai/analytics/utils.py
+-rw-r--r--   0        0        0    13235 2024-04-29 10:40:32.077990 spai-2024.4.29/spai/analytics/water_quality.py
+-rw-r--r--   0        0        0      151 2024-04-29 11:02:59.461707 spai-2024.4.29/spai/auth/__init__.py
+-rw-r--r--   0        0        0     1210 2024-04-29 10:40:32.077990 spai-2024.4.29/spai/auth/auth.py
+-rw-r--r--   0        0        0       99 2024-04-29 10:40:32.077990 spai-2024.4.29/spai/auth/is_logged.py
+-rw-r--r--   0        0        0      161 2024-04-29 10:40:32.077990 spai-2024.4.29/spai/auth/logout.py
+-rw-r--r--   0        0        0      423 2024-04-29 11:02:59.461707 spai-2024.4.29/spai/auth/retrieve_credentials.py
+-rw-r--r--   0        0        0     7202 2024-04-29 10:40:32.077990 spai-2024.4.29/spai/cli.py
+-rw-r--r--   0        0        0        0 2024-04-29 10:40:32.077990 spai-2024.4.29/spai/commands/__init__.py
+-rw-r--r--   0        0        0     1531 2024-04-29 11:02:59.461707 spai-2024.4.29/spai/commands/auth.py
+-rw-r--r--   0        0        0     1160 2024-04-29 10:40:32.077990 spai-2024.4.29/spai/commands/list.py
+-rw-r--r--   0        0        0       86 2024-04-29 10:40:32.077990 spai-2024.4.29/spai/config/__init__.py
+-rw-r--r--   0        0        0     3777 2024-04-29 10:40:32.077990 spai-2024.4.29/spai/config/validate.py
+-rw-r--r--   0        0        0     1324 2024-04-29 10:40:32.077990 spai-2024.4.29/spai/config/vars.py
+-rw-r--r--   0        0        0        0 2024-04-29 10:40:32.077990 spai-2024.4.29/spai/data/__init__.py
+-rw-r--r--   0        0        0       49 2024-04-29 10:40:32.077990 spai-2024.4.29/spai/data/indices/__init__.py
+-rw-r--r--   0        0        0       54 2024-04-29 10:40:32.077990 spai-2024.4.29/spai/data/indices/fwi/__init__.py
+-rw-r--r--   0        0        0     3234 2024-04-29 10:40:32.077990 spai-2024.4.29/spai/data/indices/fwi/fwi_nasa.py
+-rw-r--r--   0        0        0      608 2024-04-29 10:40:32.077990 spai-2024.4.29/spai/data/satellite/__init__.py
+-rw-r--r--   0        0        0     3941 2024-04-29 10:40:32.077990 spai-2024.4.29/spai/data/satellite/download.py
+-rw-r--r--   0        0        0     6332 2024-04-29 10:40:32.077990 spai-2024.4.29/spai/data/satellite/download_stac.py
+-rw-r--r--   0        0        0      647 2024-04-29 10:40:32.077990 spai-2024.4.29/spai/data/satellite/explore.py
+-rw-r--r--   0        0        0      725 2024-04-29 10:40:32.077990 spai-2024.4.29/spai/data/satellite/sentinelhub/SHCloudMaskDownloader.py
+-rw-r--r--   0        0        0      758 2024-04-29 10:40:32.077990 spai-2024.4.29/spai/data/satellite/sentinelhub/SHDEM30Downloader 2.py
+-rw-r--r--   0        0        0      758 2024-04-29 10:40:32.077990 spai-2024.4.29/spai/data/satellite/sentinelhub/SHDEM30Downloader 3.py
+-rw-r--r--   0        0        0      758 2024-04-29 10:40:32.077990 spai-2024.4.29/spai/data/satellite/sentinelhub/SHDEM30Downloader.py
+-rw-r--r--   0        0        0     3587 2024-04-29 10:40:32.077990 spai-2024.4.29/spai/data/satellite/sentinelhub/SHDownloader.py
+-rw-r--r--   0        0        0     2584 2024-04-29 10:40:32.077990 spai-2024.4.29/spai/data/satellite/sentinelhub/SHExplorer.py
+-rw-r--r--   0        0        0      854 2024-04-29 10:40:32.077990 spai-2024.4.29/spai/data/satellite/sentinelhub/SHS1Downloader.py
+-rw-r--r--   0        0        0     1264 2024-04-29 10:40:32.077990 spai-2024.4.29/spai/data/satellite/sentinelhub/SHS2Downloader.py
+-rw-r--r--   0        0        0      275 2024-04-29 10:40:32.077990 spai-2024.4.29/spai/data/satellite/sentinelhub/SHS2L1CDownloader.py
+-rw-r--r--   0        0        0      276 2024-04-29 10:40:32.077990 spai-2024.4.29/spai/data/satellite/sentinelhub/SHS2L2ADownloader.py
+-rw-r--r--   0        0        0      282 2024-04-29 10:40:32.077990 spai-2024.4.29/spai/data/satellite/sentinelhub/__init__.py
+-rw-r--r--   0        0        0     2222 2024-04-29 10:40:32.077990 spai-2024.4.29/spai/data/satellite/stac/STACDownloader.py
+-rw-r--r--   0        0        0      208 2024-04-29 10:40:32.077990 spai-2024.4.29/spai/data/satellite/stac/__init__.py
+-rw-r--r--   0        0        0      461 2024-04-29 10:40:32.077990 spai-2024.4.29/spai/data/satellite/stac/aws/AWSDEM30Downloader.py
+-rw-r--r--   0        0        0      461 2024-04-29 10:40:32.077990 spai-2024.4.29/spai/data/satellite/stac/aws/AWSDEM90Downloader.py
+-rw-r--r--   0        0        0      876 2024-04-29 10:40:32.077990 spai-2024.4.29/spai/data/satellite/stac/aws/AWSDEMDownloader.py
+-rw-r--r--   0        0        0      392 2024-04-29 10:40:32.077990 spai-2024.4.29/spai/data/satellite/stac/aws/AWSDownloader.py
+-rw-r--r--   0        0        0     1951 2024-04-29 10:40:32.077990 spai-2024.4.29/spai/data/satellite/stac/aws/AWSS2L2ADownloader.py
+-rw-r--r--   0        0        0      233 2024-04-29 10:40:32.077990 spai-2024.4.29/spai/data/satellite/stac/aws/__init__.py
+-rw-r--r--   0        0        0      456 2024-04-29 10:40:32.077990 spai-2024.4.29/spai/data/satellite/stac/decorators.py
+-rw-r--r--   0        0        0      716 2024-04-29 10:40:32.077990 spai-2024.4.29/spai/data/satellite/stac/pc/PCDownloader.py
+-rw-r--r--   0        0        0      802 2024-04-29 10:40:32.077990 spai-2024.4.29/spai/data/satellite/stac/pc/PCS1GRDDownloader.py
+-rw-r--r--   0        0        0      120 2024-04-29 10:40:32.077990 spai-2024.4.29/spai/data/satellite/stac/pc/__init__.py
+-rw-r--r--   0        0        0     8905 2024-04-29 10:40:32.077990 spai-2024.4.29/spai/data/satellite/utils.py
+-rw-r--r--   0        0        0       84 2024-04-29 10:40:32.077990 spai-2024.4.29/spai/data/vector/__init__.py
+-rw-r--r--   0        0        0     5533 2024-04-29 10:40:32.077990 spai-2024.4.29/spai/data/vector/openstreetmap.py
+-rw-r--r--   0        0        0       71 2024-04-29 10:40:32.077990 spai-2024.4.29/spai/errors/__init__.py
+-rw-r--r--   0        0        0      308 2024-04-29 10:40:32.077990 spai-2024.4.29/spai/errors/auth.py
+-rw-r--r--   0        0        0      156 2024-04-29 10:40:32.077990 spai-2024.4.29/spai/errors/mails.py
+-rw-r--r--   0        0        0       29 2024-04-29 10:40:32.077990 spai-2024.4.29/spai/image/__init__.py
+-rw-r--r--   0        0        0     1350 2024-04-29 10:40:32.077990 spai-2024.4.29/spai/image/utils.py
+-rw-r--r--   0        0        0       95 2024-04-29 10:40:32.077990 spai-2024.4.29/spai/image/xyz/__init__.py
+-rw-r--r--   0        0        0     2026 2024-04-29 10:40:32.077990 spai-2024.4.29/spai/image/xyz/cache.py
+-rw-r--r--   0        0        0      575 2024-04-29 10:40:32.077990 spai-2024.4.29/spai/image/xyz/errors.py
+-rw-r--r--   0        0        0     6924 2024-04-29 10:40:32.077990 spai-2024.4.29/spai/image/xyz/get_image_tile.py
+-rw-r--r--   0        0        0     1828 2024-04-29 10:40:32.077990 spai-2024.4.29/spai/image/xyz/image_utils.py
+-rw-r--r--   0        0        0       28 2024-04-29 10:40:32.077990 spai-2024.4.29/spai/mails/__init__.py
+-rw-r--r--   0        0        0     1334 2024-04-29 10:40:32.077990 spai-2024.4.29/spai/mails/mimetypes.py
+-rw-r--r--   0        0        0     2932 2024-04-29 10:40:32.077990 spai-2024.4.29/spai/mails/send.py
+-rw-r--r--   0        0        0     4444 2024-04-29 10:40:32.081990 spai-2024.4.29/spai/models/Config.py
+-rw-r--r--   0        0        0      984 2024-04-29 10:40:32.081990 spai-2024.4.29/spai/models/StorageConfig.py
+-rw-r--r--   0        0        0       27 2024-04-29 10:40:32.081990 spai-2024.4.29/spai/models/__init__.py
+-rw-r--r--   0        0        0      391 2024-04-29 10:40:32.081990 spai-2024.4.29/spai/processing/__init__.py
+-rw-r--r--   0        0        0      669 2024-04-29 10:40:32.081990 spai-2024.4.29/spai/processing/autocategorize1D.py
+-rw-r--r--   0        0        0      477 2024-04-29 10:40:32.081990 spai-2024.4.29/spai/processing/colorize_raster.py
+-rw-r--r--   0        0        0      932 2024-04-29 10:40:32.081990 spai-2024.4.29/spai/processing/convert_array_to_vector.py
+-rw-r--r--   0        0        0      291 2024-04-29 10:40:32.081990 spai-2024.4.29/spai/processing/mask_raster.py
+-rw-r--r--   0        0        0      682 2024-04-29 10:40:32.081990 spai-2024.4.29/spai/processing/normalised_difference.py
+-rw-r--r--   0        0        0     1239 2024-04-29 10:40:32.081990 spai-2024.4.29/spai/processing/px_count.py
+-rw-r--r--   0        0        0      107 2024-04-29 10:40:32.081990 spai-2024.4.29/spai/processing/rasterio_mask.py
+-rw-r--r--   0        0        0      266 2024-04-29 10:40:32.081990 spai-2024.4.29/spai/processing/read_raster.py
+-rw-r--r--   0        0        0     1109 2024-04-29 10:40:32.081990 spai-2024.4.29/spai/processing/save_table.py
+-rw-r--r--   0        0        0      496 2024-04-29 10:40:32.081990 spai-2024.4.29/spai/processing/utils.py
+-rw-r--r--   0        0        0      475 2024-04-29 10:40:32.081990 spai-2024.4.29/spai/project/__init__.py
+-rw-r--r--   0        0        0      466 2024-04-29 10:40:32.081990 spai-2024.4.29/spai/project/bck/GetLogs.py
+-rw-r--r--   0        0        0     1018 2024-04-29 10:40:32.081990 spai-2024.4.29/spai/project/bck/InstallReqs 2.py
+-rw-r--r--   0        0        0     1018 2024-04-29 10:40:32.081990 spai-2024.4.29/spai/project/bck/InstallReqs 3.py
+-rw-r--r--   0        0        0      482 2024-04-29 10:40:32.081990 spai-2024.4.29/spai/project/bck/RunService.py
+-rw-r--r--   0        0        0      492 2024-04-29 10:40:32.081990 spai-2024.4.29/spai/project/bck/ScheduleService.py
+-rw-r--r--   0        0        0      510 2024-04-29 10:40:32.081990 spai-2024.4.29/spai/project/bck/StopService.py
+-rw-r--r--   0        0        0     1578 2024-04-29 10:40:32.081990 spai-2024.4.29/spai/project/bck/main.py
+-rw-r--r--   0        0        0      337 2024-04-29 10:40:32.081990 spai-2024.4.29/spai/project/delete_project.py
+-rw-r--r--   0        0        0     2030 2024-04-29 10:40:32.081990 spai-2024.4.29/spai/project/deploy_folder.py
+-rw-r--r--   0        0        0      407 2024-04-29 10:40:32.081990 spai-2024.4.29/spai/project/deploy_template.py
+-rw-r--r--   0        0        0     1203 2024-04-29 10:40:32.081990 spai-2024.4.29/spai/project/download_template.py
+-rw-r--r--   0        0        0      455 2024-04-29 10:40:32.081990 spai-2024.4.29/spai/project/get_logs.py
+-rw-r--r--   0        0        0      242 2024-04-29 10:40:32.081990 spai-2024.4.29/spai/project/get_project_by_name.py
+-rw-r--r--   0        0        0      172 2024-04-29 10:40:32.081990 spai-2024.4.29/spai/project/get_projects.py
+-rw-r--r--   0        0        0      344 2024-04-29 10:40:32.081990 spai-2024.4.29/spai/project/get_service_by_name_type_project.py
+-rw-r--r--   0        0        0     1616 2024-04-29 10:40:32.081990 spai-2024.4.29/spai/project/get_services.py
+-rw-r--r--   0        0        0      525 2024-04-29 10:40:32.081990 spai-2024.4.29/spai/project/init_project.py
+-rw-r--r--   0        0        0      726 2024-04-29 10:40:32.081990 spai-2024.4.29/spai/project/install_requirements.py
+-rw-r--r--   0        0        0     5617 2024-04-29 10:40:32.081990 spai-2024.4.29/spai/project/project-template/README.md
+-rw-r--r--   0        0        0      867 2024-04-29 10:40:32.081990 spai-2024.4.29/spai/project/project-template/apis/analytics/main.py
+-rw-r--r--   0        0        0       36 2024-04-29 10:40:32.081990 spai-2024.4.29/spai/project/project-template/apis/analytics/requirements.txt
+-rw-r--r--   0        0        0     1800 2024-04-29 10:40:32.081990 spai-2024.4.29/spai/project/project-template/apis/xyz/main.py
+-rw-r--r--   0        0        0       88 2024-04-29 10:40:32.081990 spai-2024.4.29/spai/project/project-template/apis/xyz/requirements.txt
+-rw-r--r--   0        0        0   748531 2024-04-29 10:40:32.081990 spai-2024.4.29/spai/project/project-template/notebooks/analytics/main.ipynb
+-rw-r--r--   0        0        0       39 2024-04-29 10:40:32.081990 spai-2024.4.29/spai/project/project-template/notebooks/analytics/requirements.txt
+-rw-r--r--   0        0        0     1602 2024-04-29 10:40:32.081990 spai-2024.4.29/spai/project/project-template/scripts/analytics/main.py
+-rw-r--r--   0        0        0       30 2024-04-29 10:40:32.081990 spai-2024.4.29/spai/project/project-template/scripts/analytics/requirements.txt
+-rw-r--r--   0        0        0     1076 2024-04-29 10:40:32.081990 spai-2024.4.29/spai/project/project-template/scripts/downloader/main.py
+-rw-r--r--   0        0        0       85 2024-04-29 10:40:32.085990 spai-2024.4.29/spai/project/project-template/scripts/downloader/requirements.txt
+-rw-r--r--   0        0        0      618 2024-04-29 10:40:32.085990 spai-2024.4.29/spai/project/project-template/spai.config.yaml
+-rw-r--r--   0        0        0     1523 2024-04-29 10:40:32.085990 spai-2024.4.29/spai/project/project-template/uis/map/main.py
+-rw-r--r--   0        0        0       23 2024-04-29 10:40:32.085990 spai-2024.4.29/spai/project/project-template/uis/map/requirements.txt
+-rw-r--r--   0        0        0     5209 2024-04-29 10:40:32.085990 spai-2024.4.29/spai/project/run_local.py
+-rw-r--r--   0        0        0      813 2024-04-29 10:40:32.085990 spai-2024.4.29/spai/project/stop_service.py
+-rw-r--r--   0        0        0       38 2024-04-29 10:40:32.085990 spai-2024.4.29/spai/reports/__init__.py
+-rw-r--r--   0        0        0     1328 2024-04-29 10:40:32.085990 spai-2024.4.29/spai/reports/generate.py
+-rw-r--r--   0        0        0     4998 2024-04-29 11:02:59.461707 spai-2024.4.29/spai/repos/APIRepo.py
+-rw-r--r--   0        0        0      997 2024-04-29 10:40:32.085990 spai-2024.4.29/spai/repos/AuthRepo.py
+-rw-r--r--   0        0        0      188 2024-04-29 10:40:32.085990 spai-2024.4.29/spai/repos/MailsRepo.py
+-rw-r--r--   0        0        0      200 2024-04-29 10:40:32.085990 spai-2024.4.29/spai/repos/ReportsRepo.py
+-rw-r--r--   0        0        0       60 2024-04-29 10:40:32.085990 spai-2024.4.29/spai/repos/__init__.py
+-rw-r--r--   0        0        0     2426 2024-04-29 10:40:32.085990 spai-2024.4.29/spai/storage/BaseStorage.py
+-rw-r--r--   0        0        0     3716 2024-04-29 10:40:32.085990 spai-2024.4.29/spai/storage/CloudStorage.py
+-rw-r--r--   0        0        0     4527 2024-04-29 10:40:32.085990 spai-2024.4.29/spai/storage/LocalStorage.py
+-rw-r--r--   0        0        0     8449 2024-04-29 10:40:32.085990 spai-2024.4.29/spai/storage/S3Storage.py
+-rw-r--r--   0        0        0     1407 2024-04-29 10:40:32.085990 spai-2024.4.29/spai/storage/Storage.py
+-rw-r--r--   0        0        0     6077 2024-04-29 10:40:32.085990 spai-2024.4.29/spai/storage/_S3Storage.py
+-rw-r--r--   0        0        0      120 2024-04-29 10:40:32.085990 spai-2024.4.29/spai/storage/__init__.py
+-rw-r--r--   0        0        0      409 2024-04-29 10:40:32.085990 spai-2024.4.29/spai/storage/create_s3.py
+-rw-r--r--   0        0        0     1559 2024-04-29 10:40:32.085990 spai-2024.4.29/spai/storage/decorators.py
+-rw-r--r--   0        0        0      583 2024-04-29 10:40:32.085990 spai-2024.4.29/spai/storage/minio.py
+-rw-r--r--   0        0        0      888 1970-01-01 00:00:00.000000 spai-2024.4.29/PKG-INFO
```

### Comparing `spai-2024.4.17/pyproject.toml` & `spai-2024.4.29/pyproject.toml`

 * *Files 24% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "spai"
-version = "2024.04.17"
+version = "2024.04.29"
 description = ""
 authors = ["Juan Sensio <it@earthpulse.es>"]
 readme = "README.md"
 packages = [{include = "spai"}]
 
 [tool.poetry.scripts]
 spai = "spai.cli:app"
```

### Comparing `spai-2024.4.17/spai/analytics/forest_monitoring.py` & `spai-2024.4.29/spai/analytics/forest_monitoring.py`

 * *Files identical despite different names*

### Comparing `spai-2024.4.17/spai/analytics/water_quality.py` & `spai-2024.4.29/spai/analytics/water_quality.py`

 * *Files identical despite different names*

### Comparing `spai-2024.4.17/spai/auth/auth.py` & `spai-2024.4.29/spai/auth/auth.py`

 * *Files identical despite different names*

### Comparing `spai-2024.4.17/spai/cli.py` & `spai-2024.4.29/spai/cli.py`

 * *Files identical despite different names*

### Comparing `spai-2024.4.17/spai/commands/list.py` & `spai-2024.4.29/spai/commands/list.py`

 * *Files identical despite different names*

### Comparing `spai-2024.4.17/spai/config/validate.py` & `spai-2024.4.29/spai/config/validate.py`

 * *Files identical despite different names*

### Comparing `spai-2024.4.17/spai/config/vars.py` & `spai-2024.4.29/spai/config/vars.py`

 * *Files identical despite different names*

### Comparing `spai-2024.4.17/spai/data/indices/fwi/fwi_nasa.py` & `spai-2024.4.29/spai/data/indices/fwi/fwi_nasa.py`

 * *Files identical despite different names*

### Comparing `spai-2024.4.17/spai/data/satellite/__init__.py` & `spai-2024.4.29/spai/data/satellite/__init__.py`

 * *Files identical despite different names*

### Comparing `spai-2024.4.17/spai/data/satellite/download.py` & `spai-2024.4.29/spai/data/satellite/download.py`

 * *Files identical despite different names*

### Comparing `spai-2024.4.17/spai/data/satellite/download_stac.py` & `spai-2024.4.29/spai/data/satellite/download_stac.py`

 * *Files identical despite different names*

### Comparing `spai-2024.4.17/spai/data/satellite/explore.py` & `spai-2024.4.29/spai/data/satellite/explore.py`

 * *Files identical despite different names*

### Comparing `spai-2024.4.17/spai/data/satellite/sentinelhub/SHCloudMaskDownloader.py` & `spai-2024.4.29/spai/data/satellite/sentinelhub/SHCloudMaskDownloader.py`

 * *Files identical despite different names*

### Comparing `spai-2024.4.17/spai/data/satellite/sentinelhub/SHDEM30Downloader 2.py` & `spai-2024.4.29/spai/data/satellite/sentinelhub/SHDEM30Downloader 2.py`

 * *Files identical despite different names*

### Comparing `spai-2024.4.17/spai/data/satellite/sentinelhub/SHDEM30Downloader 3.py` & `spai-2024.4.29/spai/data/satellite/sentinelhub/SHDEM30Downloader 3.py`

 * *Files identical despite different names*

### Comparing `spai-2024.4.17/spai/data/satellite/sentinelhub/SHDEM30Downloader.py` & `spai-2024.4.29/spai/data/satellite/sentinelhub/SHDEM30Downloader.py`

 * *Files identical despite different names*

### Comparing `spai-2024.4.17/spai/data/satellite/sentinelhub/SHDownloader.py` & `spai-2024.4.29/spai/data/satellite/sentinelhub/SHDownloader.py`

 * *Files identical despite different names*

### Comparing `spai-2024.4.17/spai/data/satellite/sentinelhub/SHExplorer.py` & `spai-2024.4.29/spai/data/satellite/sentinelhub/SHExplorer.py`

 * *Files identical despite different names*

### Comparing `spai-2024.4.17/spai/data/satellite/sentinelhub/SHS1Downloader.py` & `spai-2024.4.29/spai/data/satellite/sentinelhub/SHS1Downloader.py`

 * *Files identical despite different names*

### Comparing `spai-2024.4.17/spai/data/satellite/sentinelhub/SHS2Downloader.py` & `spai-2024.4.29/spai/data/satellite/sentinelhub/SHS2Downloader.py`

 * *Files identical despite different names*

### Comparing `spai-2024.4.17/spai/data/satellite/stac/STACDownloader.py` & `spai-2024.4.29/spai/data/satellite/stac/STACDownloader.py`

 * *Files identical despite different names*

### Comparing `spai-2024.4.17/spai/data/satellite/stac/aws/AWSDEMDownloader.py` & `spai-2024.4.29/spai/data/satellite/stac/aws/AWSDEMDownloader.py`

 * *Files identical despite different names*

### Comparing `spai-2024.4.17/spai/data/satellite/stac/aws/AWSS2L2ADownloader.py` & `spai-2024.4.29/spai/data/satellite/stac/aws/AWSS2L2ADownloader.py`

 * *Files identical despite different names*

### Comparing `spai-2024.4.17/spai/data/satellite/stac/pc/PCDownloader.py` & `spai-2024.4.29/spai/data/satellite/stac/pc/PCDownloader.py`

 * *Files identical despite different names*

### Comparing `spai-2024.4.17/spai/data/satellite/stac/pc/PCS1GRDDownloader.py` & `spai-2024.4.29/spai/data/satellite/stac/pc/PCS1GRDDownloader.py`

 * *Files identical despite different names*

### Comparing `spai-2024.4.17/spai/data/satellite/utils.py` & `spai-2024.4.29/spai/data/satellite/utils.py`

 * *Files identical despite different names*

### Comparing `spai-2024.4.17/spai/data/vector/openstreetmap.py` & `spai-2024.4.29/spai/data/vector/openstreetmap.py`

 * *Files identical despite different names*

### Comparing `spai-2024.4.17/spai/image/utils.py` & `spai-2024.4.29/spai/image/utils.py`

 * *Files identical despite different names*

### Comparing `spai-2024.4.17/spai/image/xyz/cache.py` & `spai-2024.4.29/spai/image/xyz/cache.py`

 * *Files identical despite different names*

### Comparing `spai-2024.4.17/spai/image/xyz/errors.py` & `spai-2024.4.29/spai/image/xyz/errors.py`

 * *Files identical despite different names*

### Comparing `spai-2024.4.17/spai/image/xyz/get_image_tile.py` & `spai-2024.4.29/spai/image/xyz/get_image_tile.py`

 * *Files identical despite different names*

### Comparing `spai-2024.4.17/spai/image/xyz/image_utils.py` & `spai-2024.4.29/spai/image/xyz/image_utils.py`

 * *Files identical despite different names*

### Comparing `spai-2024.4.17/spai/mails/mimetypes.py` & `spai-2024.4.29/spai/mails/mimetypes.py`

 * *Files identical despite different names*

### Comparing `spai-2024.4.17/spai/mails/send.py` & `spai-2024.4.29/spai/mails/send.py`

 * *Files identical despite different names*

### Comparing `spai-2024.4.17/spai/models/Config.py` & `spai-2024.4.29/spai/models/Config.py`

 * *Files identical despite different names*

### Comparing `spai-2024.4.17/spai/models/StorageConfig.py` & `spai-2024.4.29/spai/models/StorageConfig.py`

 * *Files identical despite different names*

### Comparing `spai-2024.4.17/spai/processing/autocategorize1D.py` & `spai-2024.4.29/spai/processing/autocategorize1D.py`

 * *Files identical despite different names*

### Comparing `spai-2024.4.17/spai/processing/convert_array_to_vector.py` & `spai-2024.4.29/spai/processing/convert_array_to_vector.py`

 * *Files identical despite different names*

### Comparing `spai-2024.4.17/spai/processing/normalised_difference.py` & `spai-2024.4.29/spai/processing/normalised_difference.py`

 * *Files identical despite different names*

### Comparing `spai-2024.4.17/spai/processing/px_count.py` & `spai-2024.4.29/spai/processing/px_count.py`

 * *Files identical despite different names*

### Comparing `spai-2024.4.17/spai/processing/save_table.py` & `spai-2024.4.29/spai/processing/save_table.py`

 * *Files identical despite different names*

### Comparing `spai-2024.4.17/spai/project/bck/InstallReqs 2.py` & `spai-2024.4.29/spai/project/bck/InstallReqs 2.py`

 * *Files identical despite different names*

### Comparing `spai-2024.4.17/spai/project/bck/InstallReqs 3.py` & `spai-2024.4.29/spai/project/bck/InstallReqs 3.py`

 * *Files identical despite different names*

### Comparing `spai-2024.4.17/spai/project/bck/main.py` & `spai-2024.4.29/spai/project/bck/main.py`

 * *Files identical despite different names*

### Comparing `spai-2024.4.17/spai/project/deploy_folder.py` & `spai-2024.4.29/spai/project/deploy_folder.py`

 * *Files identical despite different names*

### Comparing `spai-2024.4.17/spai/project/download_template.py` & `spai-2024.4.29/spai/project/download_template.py`

 * *Files identical despite different names*

### Comparing `spai-2024.4.17/spai/project/get_services.py` & `spai-2024.4.29/spai/project/get_services.py`

 * *Files identical despite different names*

### Comparing `spai-2024.4.17/spai/project/init_project.py` & `spai-2024.4.29/spai/project/init_project.py`

 * *Files identical despite different names*

### Comparing `spai-2024.4.17/spai/project/install_requirements.py` & `spai-2024.4.29/spai/project/install_requirements.py`

 * *Files identical despite different names*

### Comparing `spai-2024.4.17/spai/project/project-template/README.md` & `spai-2024.4.29/spai/project/project-template/README.md`

 * *Files identical despite different names*

### Comparing `spai-2024.4.17/spai/project/project-template/apis/analytics/main.py` & `spai-2024.4.29/spai/project/project-template/apis/analytics/main.py`

 * *Files identical despite different names*

### Comparing `spai-2024.4.17/spai/project/project-template/apis/xyz/main.py` & `spai-2024.4.29/spai/project/project-template/apis/xyz/main.py`

 * *Files identical despite different names*

### Comparing `spai-2024.4.17/spai/project/project-template/notebooks/analytics/main.ipynb` & `spai-2024.4.29/spai/project/project-template/notebooks/analytics/main.ipynb`

 * *Files identical despite different names*

### Comparing `spai-2024.4.17/spai/project/project-template/scripts/analytics/main.py` & `spai-2024.4.29/spai/project/project-template/scripts/analytics/main.py`

 * *Files identical despite different names*

### Comparing `spai-2024.4.17/spai/project/project-template/scripts/downloader/main.py` & `spai-2024.4.29/spai/project/project-template/scripts/downloader/main.py`

 * *Files identical despite different names*

### Comparing `spai-2024.4.17/spai/project/project-template/spai.config.yaml` & `spai-2024.4.29/spai/project/project-template/spai.config.yaml`

 * *Files identical despite different names*

### Comparing `spai-2024.4.17/spai/project/project-template/uis/map/main.py` & `spai-2024.4.29/spai/project/project-template/uis/map/main.py`

 * *Files identical despite different names*

### Comparing `spai-2024.4.17/spai/project/run_local.py` & `spai-2024.4.29/spai/project/run_local.py`

 * *Files identical despite different names*

### Comparing `spai-2024.4.17/spai/project/stop_service.py` & `spai-2024.4.29/spai/project/stop_service.py`

 * *Files identical despite different names*

### Comparing `spai-2024.4.17/spai/reports/generate.py` & `spai-2024.4.29/spai/reports/generate.py`

 * *Files identical despite different names*

### Comparing `spai-2024.4.17/spai/repos/APIRepo.py` & `spai-2024.4.29/spai/repos/APIRepo.py`

 * *Files 8% similar despite different names*

```diff
@@ -34,23 +34,28 @@
     def logout_url(self):
         response = requests.get(self.url + "auth/logout")
         return response.json()["logout_url"]
 
     def get_headers(self, user):
         return {"Authorization": "Bearer " + user["id_token"]}
 
+    def retrieve_user(self, user):
+        response = requests.get(self.url + "auth/me", headers=self.get_headers(user))
+        return self.format_response(response)
+
     def retrieve_projects(self, user):
         return requests.get(
             self.url + "projects", headers=self.get_headers(user)
         ).json()
 
     def retrieve_project(self, user, project):
-        return requests.get(
+        response = requests.get(
             self.url + f"projects/{project}", headers=self.get_headers(user)
         )
+        return self.format_response(response)
 
     def retrieve_project_by_name(self, user, project_name):
         response = requests.get(
             self.url + f"projects?name={project_name}", headers=self.get_headers(user)
         )
         return self.format_response(response)
```

### Comparing `spai-2024.4.17/spai/repos/AuthRepo.py` & `spai-2024.4.29/spai/repos/AuthRepo.py`

 * *Files identical despite different names*

### Comparing `spai-2024.4.17/spai/storage/BaseStorage.py` & `spai-2024.4.29/spai/storage/BaseStorage.py`

 * *Files identical despite different names*

### Comparing `spai-2024.4.17/spai/storage/CloudStorage.py` & `spai-2024.4.29/spai/storage/CloudStorage.py`

 * *Files identical despite different names*

### Comparing `spai-2024.4.17/spai/storage/LocalStorage.py` & `spai-2024.4.29/spai/storage/LocalStorage.py`

 * *Files identical despite different names*

### Comparing `spai-2024.4.17/spai/storage/S3Storage.py` & `spai-2024.4.29/spai/storage/S3Storage.py`

 * *Files identical despite different names*

### Comparing `spai-2024.4.17/spai/storage/Storage.py` & `spai-2024.4.29/spai/storage/Storage.py`

 * *Files identical despite different names*

### Comparing `spai-2024.4.17/spai/storage/_S3Storage.py` & `spai-2024.4.29/spai/storage/_S3Storage.py`

 * *Files identical despite different names*

### Comparing `spai-2024.4.17/spai/storage/decorators.py` & `spai-2024.4.29/spai/storage/decorators.py`

 * *Files identical despite different names*

### Comparing `spai-2024.4.17/spai/storage/minio.py` & `spai-2024.4.29/spai/storage/minio.py`

 * *Files identical despite different names*

### Comparing `spai-2024.4.17/PKG-INFO` & `spai-2024.4.29/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,20 +1,19 @@
 Metadata-Version: 2.1
 Name: spai
-Version: 2024.4.17
+Version: 2024.4.29
 Summary: 
 Author: Juan Sensio
 Author-email: it@earthpulse.es
 Requires-Python: >=3.8,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Classifier: Programming Language :: Python :: 3.12
 Requires-Dist: PyJWT (>=2.7.0,<3.0.0)
 Requires-Dist: PyYAML (>=6.0.0,<7.0.0)
 Requires-Dist: minio (>=7.1.15,<8.0.0)
 Requires-Dist: pandas (>=2.0.2,<3.0.0)
 Requires-Dist: pillow (>=10.2.0,<11.0.0)
 Requires-Dist: pydantic (>=2.0.3,<3.0.0)
 Requires-Dist: requests (>=2.31.0,<3.0.0)
```

