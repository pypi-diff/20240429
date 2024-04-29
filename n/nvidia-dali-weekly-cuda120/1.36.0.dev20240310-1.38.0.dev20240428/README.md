# Comparing `tmp/nvidia-dali-weekly-cuda120-1.36.0.dev20240310.tar.gz` & `tmp/nvidia_dali_weekly_cuda120-1.38.0.dev20240428.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nvidia-dali-weekly-cuda120-1.36.0.dev20240310.tar", last modified: Mon Mar 11 10:25:56 2024, max compression
+gzip compressed data, was "nvidia_dali_weekly_cuda120-1.38.0.dev20240428.tar", last modified: Mon Apr  5 07:00:00 1993, max compression
```

## Comparing `nvidia-dali-weekly-cuda120-1.36.0.dev20240310.tar` & `nvidia_dali_weekly_cuda120-1.38.0.dev20240428.tar`

### file list

```diff
@@ -1,13 +1,2 @@
-drwxr-xr-x   0 svc-compute-packagin (25503) sw-cuda-installer  (2174)        0 2024-03-11 10:25:56.100171 nvidia-dali-weekly-cuda120-1.36.0.dev20240310/
--rw-r--r--   0 svc-compute-packagin (25503) sw-cuda-installer  (2174)      473 2024-03-11 10:25:56.000000 nvidia-dali-weekly-cuda120-1.36.0.dev20240310/ERROR.txt
--rw-rw-r--   0 svc-compute-packagin (25503) sw-cuda-installer  (2174)    11336 2024-02-03 04:02:37.000000 nvidia-dali-weekly-cuda120-1.36.0.dev20240310/LICENSE.md
--rw-r--r--   0 svc-compute-packagin (25503) sw-cuda-installer  (2174)       26 2024-03-11 10:25:56.000000 nvidia-dali-weekly-cuda120-1.36.0.dev20240310/PACKAGE_NAME
--rw-r--r--   0 svc-compute-packagin (25503) sw-cuda-installer  (2174)     1709 2024-03-11 10:25:56.100171 nvidia-dali-weekly-cuda120-1.36.0.dev20240310/PKG-INFO
--rw-r--r--   0 svc-compute-packagin (25503) sw-cuda-installer  (2174)      298 2024-03-11 10:25:56.000000 nvidia-dali-weekly-cuda120-1.36.0.dev20240310/README.rst
-drwxr-xr-x   0 svc-compute-packagin (25503) sw-cuda-installer  (2174)        0 2024-03-11 10:25:56.100171 nvidia-dali-weekly-cuda120-1.36.0.dev20240310/nvidia_dali_weekly_cuda120.egg-info/
--rw-r--r--   0 svc-compute-packagin (25503) sw-cuda-installer  (2174)     1709 2024-03-11 10:25:56.000000 nvidia-dali-weekly-cuda120-1.36.0.dev20240310/nvidia_dali_weekly_cuda120.egg-info/PKG-INFO
--rw-r--r--   0 svc-compute-packagin (25503) sw-cuda-installer  (2174)      253 2024-03-11 10:25:56.000000 nvidia-dali-weekly-cuda120-1.36.0.dev20240310/nvidia_dali_weekly_cuda120.egg-info/SOURCES.txt
--rw-r--r--   0 svc-compute-packagin (25503) sw-cuda-installer  (2174)        1 2024-03-11 10:25:56.000000 nvidia-dali-weekly-cuda120-1.36.0.dev20240310/nvidia_dali_weekly_cuda120.egg-info/dependency_links.txt
--rw-r--r--   0 svc-compute-packagin (25503) sw-cuda-installer  (2174)       22 2024-03-11 10:25:56.000000 nvidia-dali-weekly-cuda120-1.36.0.dev20240310/nvidia_dali_weekly_cuda120.egg-info/top_level.txt
--rw-r--r--   0 svc-compute-packagin (25503) sw-cuda-installer  (2174)       38 2024-03-11 10:25:56.100171 nvidia-dali-weekly-cuda120-1.36.0.dev20240310/setup.cfg
--rw-rw-r--   0 svc-compute-packagin (25503) sw-cuda-installer  (2174)     4864 2024-02-03 04:02:37.000000 nvidia-dali-weekly-cuda120-1.36.0.dev20240310/setup.py
+-rw-r--r--   0        0        0      217 1993-04-05 07:00:00.000000 pyproject.toml
+-rw-r--r--   0        0        0     2395 1993-04-05 07:00:00.000000 PKG-INFO
```

