# Comparing `tmp/byotrack-0.5.3.tar.gz` & `tmp/byotrack-0.5.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "byotrack-0.5.3.tar", last modified: Fri Apr 12 13:12:26 2024, max compression
+gzip compressed data, was "byotrack-0.5.4.tar", last modified: Mon Apr 29 17:06:57 2024, max compression
```

## Comparing `byotrack-0.5.3.tar` & `byotrack-0.5.4.tar`

### file list

```diff
@@ -1,67 +1,67 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 13:12:26.623401 byotrack-0.5.3/
--rw-r--r--   0 runner    (1001) docker     (127)     1068 2024-04-12 13:12:20.000000 byotrack-0.5.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     7305 2024-04-12 13:12:26.623401 byotrack-0.5.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     6097 2024-04-12 13:12:20.000000 byotrack-0.5.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 13:12:26.615402 byotrack-0.5.3/byotrack/
--rw-r--r--   0 runner    (1001) docker     (127)     2867 2024-04-12 13:12:20.000000 byotrack-0.5.3/byotrack/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 13:12:26.619402 byotrack-0.5.3/byotrack/api/
--rw-r--r--   0 runner    (1001) docker     (127)       27 2024-04-12 13:12:20.000000 byotrack-0.5.3/byotrack/api/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 13:12:26.619402 byotrack-0.5.3/byotrack/api/detector/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-12 13:12:20.000000 byotrack-0.5.3/byotrack/api/detector/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    13360 2024-04-12 13:12:20.000000 byotrack-0.5.3/byotrack/api/detector/detections.py
--rw-r--r--   0 runner    (1001) docker     (127)     3243 2024-04-12 13:12:20.000000 byotrack-0.5.3/byotrack/api/detector/detector.py
--rw-r--r--   0 runner    (1001) docker     (127)     1041 2024-04-12 13:12:20.000000 byotrack-0.5.3/byotrack/api/linker.py
--rw-r--r--   0 runner    (1001) docker     (127)     2506 2024-04-12 13:12:20.000000 byotrack-0.5.3/byotrack/api/parameters.py
--rw-r--r--   0 runner    (1001) docker     (127)      972 2024-04-12 13:12:20.000000 byotrack-0.5.3/byotrack/api/refiner.py
--rw-r--r--   0 runner    (1001) docker     (127)     1784 2024-04-12 13:12:20.000000 byotrack-0.5.3/byotrack/api/tracker.py
--rw-r--r--   0 runner    (1001) docker     (127)     5535 2024-04-12 13:12:20.000000 byotrack-0.5.3/byotrack/api/tracks.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 13:12:26.619402 byotrack-0.5.3/byotrack/fiji/
--rw-r--r--   0 runner    (1001) docker     (127)      109 2024-04-12 13:12:20.000000 byotrack-0.5.3/byotrack/fiji/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3304 2024-04-12 13:12:20.000000 byotrack-0.5.3/byotrack/fiji/io.py
--rw-r--r--   0 runner    (1001) docker     (127)     1380 2024-04-12 13:12:20.000000 byotrack-0.5.3/byotrack/fiji/run.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 13:12:26.619402 byotrack-0.5.3/byotrack/icy/
--rw-r--r--   0 runner    (1001) docker     (127)      117 2024-04-12 13:12:20.000000 byotrack-0.5.3/byotrack/icy/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7498 2024-04-12 13:12:20.000000 byotrack-0.5.3/byotrack/icy/io.py
--rw-r--r--   0 runner    (1001) docker     (127)     1847 2024-04-12 13:12:20.000000 byotrack-0.5.3/byotrack/icy/run.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 13:12:26.619402 byotrack-0.5.3/byotrack/implementation/
--rw-r--r--   0 runner    (1001) docker     (127)       73 2024-04-12 13:12:20.000000 byotrack-0.5.3/byotrack/implementation/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 13:12:26.619402 byotrack-0.5.3/byotrack/implementation/detector/
--rw-r--r--   0 runner    (1001) docker     (127)       31 2024-04-12 13:12:20.000000 byotrack-0.5.3/byotrack/implementation/detector/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3971 2024-04-12 13:12:20.000000 byotrack-0.5.3/byotrack/implementation/detector/stardist.py
--rw-r--r--   0 runner    (1001) docker     (127)     9017 2024-04-12 13:12:20.000000 byotrack-0.5.3/byotrack/implementation/detector/wavelet.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 13:12:26.619402 byotrack-0.5.3/byotrack/implementation/linker/
--rw-r--r--   0 runner    (1001) docker     (127)       29 2024-04-12 13:12:20.000000 byotrack-0.5.3/byotrack/implementation/linker/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 13:12:26.619402 byotrack-0.5.3/byotrack/implementation/linker/icy_emht/
--rw-r--r--   0 runner    (1001) docker     (127)       60 2024-04-12 13:12:20.000000 byotrack-0.5.3/byotrack/implementation/linker/icy_emht/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6198 2024-04-12 13:12:20.000000 byotrack-0.5.3/byotrack/implementation/linker/icy_emht/emht_protocol.xml
--rw-r--r--   0 runner    (1001) docker     (127)     4772 2024-04-12 13:12:20.000000 byotrack-0.5.3/byotrack/implementation/linker/icy_emht/emht_protocol_with_full_specs.xml
--rw-r--r--   0 runner    (1001) docker     (127)    13152 2024-04-12 13:12:20.000000 byotrack-0.5.3/byotrack/implementation/linker/icy_emht/icy_emht.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 13:12:26.623401 byotrack-0.5.3/byotrack/implementation/linker/trackmate/
--rw-r--r--   0 runner    (1001) docker     (127)       60 2024-04-12 13:12:20.000000 byotrack-0.5.3/byotrack/implementation/linker/trackmate/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3024 2024-04-12 13:12:20.000000 byotrack-0.5.3/byotrack/implementation/linker/trackmate/_trackmate.py
--rw-r--r--   0 runner    (1001) docker     (127)     7952 2024-04-12 13:12:20.000000 byotrack-0.5.3/byotrack/implementation/linker/trackmate/trackmate.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 13:12:26.623401 byotrack-0.5.3/byotrack/implementation/refiner/
--rw-r--r--   0 runner    (1001) docker     (127)       31 2024-04-12 13:12:20.000000 byotrack-0.5.3/byotrack/implementation/refiner/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3131 2024-04-12 13:12:20.000000 byotrack-0.5.3/byotrack/implementation/refiner/cleaner.py
--rw-r--r--   0 runner    (1001) docker     (127)     2093 2024-04-12 13:12:20.000000 byotrack-0.5.3/byotrack/implementation/refiner/interpolater.py
--rw-r--r--   0 runner    (1001) docker     (127)     8048 2024-04-12 13:12:20.000000 byotrack-0.5.3/byotrack/implementation/refiner/propagation.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 13:12:26.623401 byotrack-0.5.3/byotrack/implementation/refiner/stitching/
--rw-r--r--   0 runner    (1001) docker     (127)       71 2024-04-12 13:12:20.000000 byotrack-0.5.3/byotrack/implementation/refiner/stitching/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6628 2024-04-12 13:12:20.000000 byotrack-0.5.3/byotrack/implementation/refiner/stitching/dist_stitcher.py
--rw-r--r--   0 runner    (1001) docker     (127)     4193 2024-04-12 13:12:20.000000 byotrack-0.5.3/byotrack/implementation/refiner/stitching/emc2.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-12 13:12:20.000000 byotrack-0.5.3/byotrack/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 13:12:26.623401 byotrack-0.5.3/byotrack/video/
--rw-r--r--   0 runner    (1001) docker     (127)      253 2024-04-12 13:12:20.000000 byotrack-0.5.3/byotrack/video/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8032 2024-04-12 13:12:20.000000 byotrack-0.5.3/byotrack/video/reader.py
--rw-r--r--   0 runner    (1001) docker     (127)     3796 2024-04-12 13:12:20.000000 byotrack-0.5.3/byotrack/video/transforms.py
--rw-r--r--   0 runner    (1001) docker     (127)     8314 2024-04-12 13:12:20.000000 byotrack-0.5.3/byotrack/video/video.py
--rw-r--r--   0 runner    (1001) docker     (127)    11897 2024-04-12 13:12:20.000000 byotrack-0.5.3/byotrack/visualize.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 13:12:26.623401 byotrack-0.5.3/byotrack.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     7305 2024-04-12 13:12:26.000000 byotrack-0.5.3/byotrack.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1713 2024-04-12 13:12:26.000000 byotrack-0.5.3/byotrack.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-12 13:12:26.000000 byotrack-0.5.3/byotrack.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      116 2024-04-12 13:12:26.000000 byotrack-0.5.3/byotrack.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        9 2024-04-12 13:12:26.000000 byotrack-0.5.3/byotrack.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      139 2024-04-12 13:12:21.000000 byotrack-0.5.3/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)     1172 2024-04-12 13:12:26.623401 byotrack-0.5.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)       54 2024-04-12 13:12:21.000000 byotrack-0.5.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 17:06:57.501359 byotrack-0.5.4/
+-rw-r--r--   0 runner    (1001) docker     (127)     1068 2024-04-29 17:06:49.000000 byotrack-0.5.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     7345 2024-04-29 17:06:57.501359 byotrack-0.5.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     6097 2024-04-29 17:06:49.000000 byotrack-0.5.4/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 17:06:57.493359 byotrack-0.5.4/byotrack/
+-rw-r--r--   0 runner    (1001) docker     (127)     2867 2024-04-29 17:06:49.000000 byotrack-0.5.4/byotrack/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 17:06:57.493359 byotrack-0.5.4/byotrack/api/
+-rw-r--r--   0 runner    (1001) docker     (127)       27 2024-04-29 17:06:49.000000 byotrack-0.5.4/byotrack/api/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 17:06:57.493359 byotrack-0.5.4/byotrack/api/detector/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-29 17:06:49.000000 byotrack-0.5.4/byotrack/api/detector/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13360 2024-04-29 17:06:49.000000 byotrack-0.5.4/byotrack/api/detector/detections.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3243 2024-04-29 17:06:49.000000 byotrack-0.5.4/byotrack/api/detector/detector.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1041 2024-04-29 17:06:49.000000 byotrack-0.5.4/byotrack/api/linker.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2506 2024-04-29 17:06:49.000000 byotrack-0.5.4/byotrack/api/parameters.py
+-rw-r--r--   0 runner    (1001) docker     (127)      972 2024-04-29 17:06:49.000000 byotrack-0.5.4/byotrack/api/refiner.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1784 2024-04-29 17:06:49.000000 byotrack-0.5.4/byotrack/api/tracker.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5535 2024-04-29 17:06:49.000000 byotrack-0.5.4/byotrack/api/tracks.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 17:06:57.493359 byotrack-0.5.4/byotrack/fiji/
+-rw-r--r--   0 runner    (1001) docker     (127)      109 2024-04-29 17:06:49.000000 byotrack-0.5.4/byotrack/fiji/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3304 2024-04-29 17:06:49.000000 byotrack-0.5.4/byotrack/fiji/io.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1380 2024-04-29 17:06:49.000000 byotrack-0.5.4/byotrack/fiji/run.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 17:06:57.497359 byotrack-0.5.4/byotrack/icy/
+-rw-r--r--   0 runner    (1001) docker     (127)      117 2024-04-29 17:06:49.000000 byotrack-0.5.4/byotrack/icy/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7498 2024-04-29 17:06:49.000000 byotrack-0.5.4/byotrack/icy/io.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1847 2024-04-29 17:06:49.000000 byotrack-0.5.4/byotrack/icy/run.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 17:06:57.497359 byotrack-0.5.4/byotrack/implementation/
+-rw-r--r--   0 runner    (1001) docker     (127)       73 2024-04-29 17:06:49.000000 byotrack-0.5.4/byotrack/implementation/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 17:06:57.497359 byotrack-0.5.4/byotrack/implementation/detector/
+-rw-r--r--   0 runner    (1001) docker     (127)       31 2024-04-29 17:06:49.000000 byotrack-0.5.4/byotrack/implementation/detector/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3971 2024-04-29 17:06:49.000000 byotrack-0.5.4/byotrack/implementation/detector/stardist.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9017 2024-04-29 17:06:49.000000 byotrack-0.5.4/byotrack/implementation/detector/wavelet.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 17:06:57.497359 byotrack-0.5.4/byotrack/implementation/linker/
+-rw-r--r--   0 runner    (1001) docker     (127)       29 2024-04-29 17:06:49.000000 byotrack-0.5.4/byotrack/implementation/linker/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 17:06:57.497359 byotrack-0.5.4/byotrack/implementation/linker/icy_emht/
+-rw-r--r--   0 runner    (1001) docker     (127)       60 2024-04-29 17:06:49.000000 byotrack-0.5.4/byotrack/implementation/linker/icy_emht/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6198 2024-04-29 17:06:49.000000 byotrack-0.5.4/byotrack/implementation/linker/icy_emht/emht_protocol.xml
+-rw-r--r--   0 runner    (1001) docker     (127)     4772 2024-04-29 17:06:49.000000 byotrack-0.5.4/byotrack/implementation/linker/icy_emht/emht_protocol_with_full_specs.xml
+-rw-r--r--   0 runner    (1001) docker     (127)    13152 2024-04-29 17:06:49.000000 byotrack-0.5.4/byotrack/implementation/linker/icy_emht/icy_emht.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 17:06:57.497359 byotrack-0.5.4/byotrack/implementation/linker/trackmate/
+-rw-r--r--   0 runner    (1001) docker     (127)       60 2024-04-29 17:06:49.000000 byotrack-0.5.4/byotrack/implementation/linker/trackmate/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3024 2024-04-29 17:06:49.000000 byotrack-0.5.4/byotrack/implementation/linker/trackmate/_trackmate.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7952 2024-04-29 17:06:49.000000 byotrack-0.5.4/byotrack/implementation/linker/trackmate/trackmate.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 17:06:57.497359 byotrack-0.5.4/byotrack/implementation/refiner/
+-rw-r--r--   0 runner    (1001) docker     (127)       31 2024-04-29 17:06:49.000000 byotrack-0.5.4/byotrack/implementation/refiner/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3131 2024-04-29 17:06:49.000000 byotrack-0.5.4/byotrack/implementation/refiner/cleaner.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2093 2024-04-29 17:06:49.000000 byotrack-0.5.4/byotrack/implementation/refiner/interpolater.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8048 2024-04-29 17:06:49.000000 byotrack-0.5.4/byotrack/implementation/refiner/propagation.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 17:06:57.497359 byotrack-0.5.4/byotrack/implementation/refiner/stitching/
+-rw-r--r--   0 runner    (1001) docker     (127)       71 2024-04-29 17:06:49.000000 byotrack-0.5.4/byotrack/implementation/refiner/stitching/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6612 2024-04-29 17:06:49.000000 byotrack-0.5.4/byotrack/implementation/refiner/stitching/dist_stitcher.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4193 2024-04-29 17:06:49.000000 byotrack-0.5.4/byotrack/implementation/refiner/stitching/emc2.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-29 17:06:49.000000 byotrack-0.5.4/byotrack/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 17:06:57.501359 byotrack-0.5.4/byotrack/video/
+-rw-r--r--   0 runner    (1001) docker     (127)      253 2024-04-29 17:06:49.000000 byotrack-0.5.4/byotrack/video/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8032 2024-04-29 17:06:49.000000 byotrack-0.5.4/byotrack/video/reader.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3934 2024-04-29 17:06:49.000000 byotrack-0.5.4/byotrack/video/transforms.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8314 2024-04-29 17:06:49.000000 byotrack-0.5.4/byotrack/video/video.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11897 2024-04-29 17:06:49.000000 byotrack-0.5.4/byotrack/visualize.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 17:06:57.501359 byotrack-0.5.4/byotrack.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     7345 2024-04-29 17:06:57.000000 byotrack-0.5.4/byotrack.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1713 2024-04-29 17:06:57.000000 byotrack-0.5.4/byotrack.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-29 17:06:57.000000 byotrack-0.5.4/byotrack.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      116 2024-04-29 17:06:57.000000 byotrack-0.5.4/byotrack.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        9 2024-04-29 17:06:57.000000 byotrack-0.5.4/byotrack.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      139 2024-04-29 17:06:49.000000 byotrack-0.5.4/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)     1200 2024-04-29 17:06:57.501359 byotrack-0.5.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)       54 2024-04-29 17:06:49.000000 byotrack-0.5.4/setup.py
```

### Comparing `byotrack-0.5.3/LICENSE` & `byotrack-0.5.4/LICENSE`

 * *Files identical despite different names*

### Comparing `byotrack-0.5.3/PKG-INFO` & `byotrack-0.5.4/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,26 +1,27 @@
 Metadata-Version: 2.1
 Name: byotrack
-Version: 0.5.3
+Version: 0.5.4
 Summary: Biological particle tracking with Python
 Home-page: https://github.com/raphaelreme/byotrack
 Author: Raphael Reme
 Author-email: raphaelreme-dev@protonmail.com
 License: MIT
 Keywords: Tracking,biologie,machine learning,statistics,optimization
-Classifier: Development Status :: 2 - Pre-Alpha
+Classifier: Development Status :: 4 - Beta
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Requires-Python: <3.12,>=3.7
+Classifier: Programming Language :: Python :: 3.12
+Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: numba
 Requires-Dist: numpy
 Requires-Dist: opencv-python
 Requires-Dist: pillow
 Requires-Dist: pylapy[scipy]
```

### Comparing `byotrack-0.5.3/README.md` & `byotrack-0.5.4/README.md`

 * *Files identical despite different names*

### Comparing `byotrack-0.5.3/byotrack/__init__.py` & `byotrack-0.5.4/byotrack/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -77,8 +77,8 @@
 from byotrack.api.linker import Linker
 from byotrack.api.refiner import Refiner
 from byotrack.api.tracker import MultiStepTracker, Tracker
 from byotrack.api.tracks import Track
 from byotrack.video import Video, VideoTransformConfig
 
 
-__version__ = "0.5.3"
+__version__ = "0.5.4"
```

### Comparing `byotrack-0.5.3/byotrack/api/detector/detections.py` & `byotrack-0.5.4/byotrack/api/detector/detections.py`

 * *Files identical despite different names*

### Comparing `byotrack-0.5.3/byotrack/api/detector/detector.py` & `byotrack-0.5.4/byotrack/api/detector/detector.py`

 * *Files identical despite different names*

### Comparing `byotrack-0.5.3/byotrack/api/linker.py` & `byotrack-0.5.4/byotrack/api/linker.py`

 * *Files identical despite different names*

### Comparing `byotrack-0.5.3/byotrack/api/parameters.py` & `byotrack-0.5.4/byotrack/api/parameters.py`

 * *Files identical despite different names*

### Comparing `byotrack-0.5.3/byotrack/api/refiner.py` & `byotrack-0.5.4/byotrack/api/refiner.py`

 * *Files identical despite different names*

### Comparing `byotrack-0.5.3/byotrack/api/tracker.py` & `byotrack-0.5.4/byotrack/api/tracker.py`

 * *Files identical despite different names*

### Comparing `byotrack-0.5.3/byotrack/api/tracks.py` & `byotrack-0.5.4/byotrack/api/tracks.py`

 * *Files identical despite different names*

### Comparing `byotrack-0.5.3/byotrack/fiji/io.py` & `byotrack-0.5.4/byotrack/fiji/io.py`

 * *Files identical despite different names*

### Comparing `byotrack-0.5.3/byotrack/fiji/run.py` & `byotrack-0.5.4/byotrack/fiji/run.py`

 * *Files identical despite different names*

### Comparing `byotrack-0.5.3/byotrack/icy/io.py` & `byotrack-0.5.4/byotrack/icy/io.py`

 * *Files identical despite different names*

### Comparing `byotrack-0.5.3/byotrack/icy/run.py` & `byotrack-0.5.4/byotrack/icy/run.py`

 * *Files identical despite different names*

### Comparing `byotrack-0.5.3/byotrack/implementation/detector/stardist.py` & `byotrack-0.5.4/byotrack/implementation/detector/stardist.py`

 * *Files identical despite different names*

### Comparing `byotrack-0.5.3/byotrack/implementation/detector/wavelet.py` & `byotrack-0.5.4/byotrack/implementation/detector/wavelet.py`

 * *Files identical despite different names*

### Comparing `byotrack-0.5.3/byotrack/implementation/linker/icy_emht/emht_protocol.xml` & `byotrack-0.5.4/byotrack/implementation/linker/icy_emht/emht_protocol.xml`

 * *Files identical despite different names*

### Comparing `byotrack-0.5.3/byotrack/implementation/linker/icy_emht/emht_protocol_with_full_specs.xml` & `byotrack-0.5.4/byotrack/implementation/linker/icy_emht/emht_protocol_with_full_specs.xml`

 * *Files identical despite different names*

### Comparing `byotrack-0.5.3/byotrack/implementation/linker/icy_emht/icy_emht.py` & `byotrack-0.5.4/byotrack/implementation/linker/icy_emht/icy_emht.py`

 * *Files identical despite different names*

### Comparing `byotrack-0.5.3/byotrack/implementation/linker/trackmate/_trackmate.py` & `byotrack-0.5.4/byotrack/implementation/linker/trackmate/_trackmate.py`

 * *Files identical despite different names*

### Comparing `byotrack-0.5.3/byotrack/implementation/linker/trackmate/trackmate.py` & `byotrack-0.5.4/byotrack/implementation/linker/trackmate/trackmate.py`

 * *Files identical despite different names*

### Comparing `byotrack-0.5.3/byotrack/implementation/refiner/cleaner.py` & `byotrack-0.5.4/byotrack/implementation/refiner/cleaner.py`

 * *Files identical despite different names*

### Comparing `byotrack-0.5.3/byotrack/implementation/refiner/interpolater.py` & `byotrack-0.5.4/byotrack/implementation/refiner/interpolater.py`

 * *Files identical despite different names*

### Comparing `byotrack-0.5.3/byotrack/implementation/refiner/propagation.py` & `byotrack-0.5.4/byotrack/implementation/refiner/propagation.py`

 * *Files identical despite different names*

### Comparing `byotrack-0.5.3/byotrack/implementation/refiner/stitching/dist_stitcher.py` & `byotrack-0.5.4/byotrack/implementation/refiner/stitching/dist_stitcher.py`

 * *Files 0% similar despite different names*

```diff
@@ -98,16 +98,16 @@
 
         Returns:
             torch.Tensor: Boolean tensor that indicates True when the dist computation should be skipped
         """
         starts = torch.tensor([track.start for track in tracks])
         ends = torch.tensor([track.start + len(track) for track in tracks])
 
-        first_pos = torch.concatenate([track.points[:1] for track in tracks])
-        last_pos = torch.concatenate([track.points[-1:] for track in tracks])
+        first_pos = torch.cat([track.points[:1] for track in tracks])
+        last_pos = torch.cat([track.points[-1:] for track in tracks])
 
         skip = starts[:, None] >= starts[None, :]  # Ensure full asymmetry
         skip |= ends[:, None] > starts[None, :] + max_overlap
 
         if max_gap > 0:
             skip |= ends[:, None] + max_gap < starts[None, :]
```

### Comparing `byotrack-0.5.3/byotrack/implementation/refiner/stitching/emc2.py` & `byotrack-0.5.4/byotrack/implementation/refiner/stitching/emc2.py`

 * *Files identical despite different names*

### Comparing `byotrack-0.5.3/byotrack/video/reader.py` & `byotrack-0.5.4/byotrack/video/reader.py`

 * *Files identical despite different names*

### Comparing `byotrack-0.5.3/byotrack/video/transforms.py` & `byotrack-0.5.4/byotrack/video/transforms.py`

 * *Files 5% similar despite different names*

```diff
@@ -101,22 +101,24 @@
             frames (np.ndarray): Several frames of the same video to compute the stats
                 Shape: (N, H, W, C)
 
         """
         frames = frames[: self.max_frames_for_stats]
         self.mini = np.quantile(frames, self.q_min, axis=(0, 1, 2))
         self.maxi = np.quantile(frames, self.q_max, axis=(0, 1, 2))
+
         if self.smooth_clip > 0:
-            self.max = 1 + self.smooth_clip * np.log((frames.max() / self.maxi - 1) / self.smooth_clip + 1)
+            ratio = frames.max(axis=(0, 1, 2)) / (self.maxi + (self.maxi == 0))
+            self.max = 1 + 0.5 * np.log(np.maximum(1, 1 + (ratio - 1) / 0.5))
 
     def __call__(self, frame: np.ndarray) -> np.ndarray:
         if self.smooth_clip <= 0:  # No smooth clip
             frame = np.clip(frame, self.mini, self.maxi)
             frame -= self.mini
-            frame /= self.maxi - self.mini
+            frame /= self.maxi - self.mini + (self.maxi == self.mini)  # Divide by one if mini == maxi
             return frame
 
-        frame = (frame - self.mini) / (self.maxi - self.mini)
+        frame = (frame - self.mini) / (self.maxi - self.mini + (self.maxi == self.mini))
         # Log cliping high values
         frame[frame > 1] = 1 + self.smooth_clip * np.log((frame[frame > 1] - 1) / self.smooth_clip + 1)
         np.clip(frame, 0, self.max, frame)
         return frame / self.max
```

### Comparing `byotrack-0.5.3/byotrack/video/video.py` & `byotrack-0.5.4/byotrack/video/video.py`

 * *Files identical despite different names*

### Comparing `byotrack-0.5.3/byotrack/visualize.py` & `byotrack-0.5.4/byotrack/visualize.py`

 * *Files identical despite different names*

### Comparing `byotrack-0.5.3/byotrack.egg-info/PKG-INFO` & `byotrack-0.5.4/byotrack.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,26 +1,27 @@
 Metadata-Version: 2.1
 Name: byotrack
-Version: 0.5.3
+Version: 0.5.4
 Summary: Biological particle tracking with Python
 Home-page: https://github.com/raphaelreme/byotrack
 Author: Raphael Reme
 Author-email: raphaelreme-dev@protonmail.com
 License: MIT
 Keywords: Tracking,biologie,machine learning,statistics,optimization
-Classifier: Development Status :: 2 - Pre-Alpha
+Classifier: Development Status :: 4 - Beta
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Requires-Python: <3.12,>=3.7
+Classifier: Programming Language :: Python :: 3.12
+Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: numba
 Requires-Dist: numpy
 Requires-Dist: opencv-python
 Requires-Dist: pillow
 Requires-Dist: pylapy[scipy]
```

### Comparing `byotrack-0.5.3/byotrack.egg-info/SOURCES.txt` & `byotrack-0.5.4/byotrack.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `byotrack-0.5.3/setup.cfg` & `byotrack-0.5.4/setup.cfg`

 * *Files 10% similar despite different names*

```diff
@@ -7,27 +7,28 @@
 keywords = Tracking, biologie, machine learning, statistics, optimization
 license = MIT
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/raphaelreme/byotrack
 project_urls = 
 classifiers = 
-	Development Status :: 2 - Pre-Alpha
+	Development Status :: 4 - Beta
 	License :: OSI Approved :: MIT License
 	Natural Language :: English
 	Operating System :: OS Independent
 	Programming Language :: Python :: 3.7
 	Programming Language :: Python :: 3.8
 	Programming Language :: Python :: 3.9
 	Programming Language :: Python :: 3.10
 	Programming Language :: Python :: 3.11
+	Programming Language :: Python :: 3.12
 
 [options]
 packages = find:
-python_requires = >=3.7, <3.12
+python_requires = >=3.7
 install_requires = 
 	numba
 	numpy
 	opencv-python
 	pillow
 	pylapy[scipy]
 	torch
```

