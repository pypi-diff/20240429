# Comparing `tmp/pylxd-2.3.2a0.tar.gz` & `tmp/pylxd-2.3.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pylxd-2.3.2a0.tar", last modified: Mon Jan 15 22:03:10 2024, max compression
+gzip compressed data, was "pylxd-2.3.3.tar", last modified: Mon Apr 29 15:37:33 2024, max compression
```

## Comparing `pylxd-2.3.2a0.tar` & `pylxd-2.3.3.tar`

### file list

```diff
@@ -1,69 +1,69 @@
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2024-01-15 22:03:10.143161 pylxd-2.3.2a0/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1422 2023-05-05 08:25:21.000000 pylxd-2.3.2a0/CONTRIBUTORS.rst
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    10142 2021-09-29 19:03:03.000000 pylxd-2.3.2a0/LICENSE
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       60 2021-09-29 19:03:03.000000 pylxd-2.3.2a0/MANIFEST.in
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2175 2024-01-15 22:03:10.143161 pylxd-2.3.2a0/PKG-INFO
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1525 2023-10-18 17:36:47.000000 pylxd-2.3.2a0/README.rst
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2024-01-15 22:03:10.135161 pylxd-2.3.2a0/integration/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        0 2021-09-29 19:03:03.000000 pylxd-2.3.2a0/integration/__init__.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     5370 2023-06-01 18:56:49.000000 pylxd-2.3.2a0/integration/busybox.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1469 2023-07-13 13:52:25.000000 pylxd-2.3.2a0/integration/test_client.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1492 2023-06-01 18:56:49.000000 pylxd-2.3.2a0/integration/test_cluster_members.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     9853 2023-06-01 18:56:49.000000 pylxd-2.3.2a0/integration/test_containers.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2994 2023-07-13 12:08:43.000000 pylxd-2.3.2a0/integration/test_images.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     3981 2023-06-01 18:56:49.000000 pylxd-2.3.2a0/integration/test_networks.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2842 2024-01-11 18:53:51.000000 pylxd-2.3.2a0/integration/test_profiles.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     3379 2022-04-08 22:48:50.000000 pylxd-2.3.2a0/integration/test_projects.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     6082 2023-07-13 16:12:42.000000 pylxd-2.3.2a0/integration/test_storage.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     5769 2023-06-01 18:56:49.000000 pylxd-2.3.2a0/integration/testing.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2024-01-15 22:03:10.135161 pylxd-2.3.2a0/migration/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        0 2021-09-29 19:03:03.000000 pylxd-2.3.2a0/migration/__init__.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     5370 2023-06-01 18:56:49.000000 pylxd-2.3.2a0/migration/busybox.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2839 2023-06-01 18:56:49.000000 pylxd-2.3.2a0/migration/test_containers.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     5329 2023-06-01 18:56:49.000000 pylxd-2.3.2a0/migration/testing.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2024-01-15 22:03:10.135161 pylxd-2.3.2a0/pylxd/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      696 2023-09-25 15:31:32.000000 pylxd-2.3.2a0/pylxd/__init__.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    19090 2023-08-08 15:38:43.000000 pylxd-2.3.2a0/pylxd/client.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1809 2023-06-01 18:56:49.000000 pylxd-2.3.2a0/pylxd/exceptions.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2456 2023-05-05 08:25:21.000000 pylxd-2.3.2a0/pylxd/managers.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2024-01-15 22:03:10.139161 pylxd-2.3.2a0/pylxd/models/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      911 2022-10-31 15:18:30.000000 pylxd-2.3.2a0/pylxd/models/__init__.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    12781 2023-08-09 14:03:27.000000 pylxd-2.3.2a0/pylxd/models/_model.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     3653 2022-06-06 22:07:26.000000 pylxd-2.3.2a0/pylxd/models/certificate.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     4058 2022-10-24 16:03:37.000000 pylxd-2.3.2a0/pylxd/models/cluster.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      802 2021-09-29 19:03:03.000000 pylxd-2.3.2a0/pylxd/models/container.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     8443 2023-10-15 22:02:57.000000 pylxd-2.3.2a0/pylxd/models/image.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    34058 2023-08-09 14:03:27.000000 pylxd-2.3.2a0/pylxd/models/instance.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     6223 2023-06-01 18:56:49.000000 pylxd-2.3.2a0/pylxd/models/network.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     3440 2021-09-29 19:03:03.000000 pylxd-2.3.2a0/pylxd/models/operation.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2381 2024-01-11 18:53:51.000000 pylxd-2.3.2a0/pylxd/models/profile.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2367 2022-09-26 21:41:17.000000 pylxd-2.3.2a0/pylxd/models/project.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    23890 2023-10-18 17:36:47.000000 pylxd-2.3.2a0/pylxd/models/storage_pool.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2024-01-15 22:03:10.139161 pylxd-2.3.2a0/pylxd/models/tests/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        0 2021-09-29 19:03:03.000000 pylxd-2.3.2a0/pylxd/models/tests/__init__.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     5113 2022-06-06 22:07:26.000000 pylxd-2.3.2a0/pylxd/models/tests/test_certificate.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1858 2022-10-24 16:03:37.000000 pylxd-2.3.2a0/pylxd/models/tests/test_cluster.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1376 2022-10-20 21:45:44.000000 pylxd-2.3.2a0/pylxd/models/tests/test_cluster_certificate.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1204 2021-09-29 19:03:03.000000 pylxd-2.3.2a0/pylxd/models/tests/test_cluster_member.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    13387 2021-09-29 19:03:03.000000 pylxd-2.3.2a0/pylxd/models/tests/test_image.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    30217 2023-05-05 08:25:21.000000 pylxd-2.3.2a0/pylxd/models/tests/test_instance.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    11372 2021-09-29 19:03:03.000000 pylxd-2.3.2a0/pylxd/models/tests/test_model.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    14808 2023-01-11 16:17:27.000000 pylxd-2.3.2a0/pylxd/models/tests/test_network.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     4428 2021-09-29 19:03:03.000000 pylxd-2.3.2a0/pylxd/models/tests/test_operation.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     5198 2021-09-29 19:03:03.000000 pylxd-2.3.2a0/pylxd/models/tests/test_profile.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     4864 2021-09-29 19:03:03.000000 pylxd-2.3.2a0/pylxd/models/tests/test_project.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    11204 2022-10-20 15:23:34.000000 pylxd-2.3.2a0/pylxd/models/tests/test_storage.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      792 2021-09-29 19:03:03.000000 pylxd-2.3.2a0/pylxd/models/virtual_machine.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2024-01-15 22:03:10.143161 pylxd-2.3.2a0/pylxd/tests/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        0 2021-09-29 19:03:03.000000 pylxd-2.3.2a0/pylxd/tests/__init__.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    36958 2022-10-31 15:18:30.000000 pylxd-2.3.2a0/pylxd/tests/mock_lxd.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    24040 2023-05-05 08:25:21.000000 pylxd-2.3.2a0/pylxd/tests/test_client.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1326 2022-10-20 15:23:34.000000 pylxd-2.3.2a0/pylxd/tests/testing.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2024-01-15 22:03:10.135161 pylxd-2.3.2a0/pylxd.egg-info/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2175 2024-01-15 22:03:10.000000 pylxd-2.3.2a0/pylxd.egg-info/PKG-INFO
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1584 2024-01-15 22:03:10.000000 pylxd-2.3.2a0/pylxd.egg-info/SOURCES.txt
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        1 2024-01-15 22:03:10.000000 pylxd-2.3.2a0/pylxd.egg-info/dependency_links.txt
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      323 2024-01-15 22:03:10.000000 pylxd-2.3.2a0/pylxd.egg-info/requires.txt
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       28 2024-01-15 22:03:10.000000 pylxd-2.3.2a0/pylxd.egg-info/top_level.txt
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2364 2024-01-15 22:03:10.143161 pylxd-2.3.2a0/setup.cfg
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      584 2023-10-17 18:41:38.000000 pylxd-2.3.2a0/setup.py
+drwxrwxr-x   0 sdeziel   (1000) sdeziel   (1000)        0 2024-04-29 15:37:33.527112 pylxd-2.3.3/
+-rw-rw-r--   0 sdeziel   (1000) sdeziel   (1000)     1422 2023-05-05 08:25:21.000000 pylxd-2.3.3/CONTRIBUTORS.rst
+-rw-rw-r--   0 sdeziel   (1000) sdeziel   (1000)    10142 2021-09-29 19:03:03.000000 pylxd-2.3.3/LICENSE
+-rw-rw-r--   0 sdeziel   (1000) sdeziel   (1000)       60 2021-09-29 19:03:03.000000 pylxd-2.3.3/MANIFEST.in
+-rw-r--r--   0 sdeziel   (1000) sdeziel   (1000)     2940 2024-04-29 15:37:33.527112 pylxd-2.3.3/PKG-INFO
+-rw-rw-r--   0 sdeziel   (1000) sdeziel   (1000)     1525 2023-10-18 17:36:47.000000 pylxd-2.3.3/README.rst
+drwxrwxr-x   0 sdeziel   (1000) sdeziel   (1000)        0 2024-04-29 15:37:33.511112 pylxd-2.3.3/integration/
+-rw-rw-r--   0 sdeziel   (1000) sdeziel   (1000)        0 2021-09-29 19:03:03.000000 pylxd-2.3.3/integration/__init__.py
+-rw-rw-r--   0 sdeziel   (1000) sdeziel   (1000)     5370 2023-06-01 18:56:49.000000 pylxd-2.3.3/integration/busybox.py
+-rw-rw-r--   0 sdeziel   (1000) sdeziel   (1000)     1469 2023-07-13 13:52:25.000000 pylxd-2.3.3/integration/test_client.py
+-rw-rw-r--   0 sdeziel   (1000) sdeziel   (1000)     1492 2023-06-01 18:56:49.000000 pylxd-2.3.3/integration/test_cluster_members.py
+-rw-rw-r--   0 sdeziel   (1000) sdeziel   (1000)     9853 2024-02-27 18:44:48.000000 pylxd-2.3.3/integration/test_containers.py
+-rw-rw-r--   0 sdeziel   (1000) sdeziel   (1000)     2994 2023-07-13 12:08:43.000000 pylxd-2.3.3/integration/test_images.py
+-rw-rw-r--   0 sdeziel   (1000) sdeziel   (1000)     3981 2023-06-01 18:56:49.000000 pylxd-2.3.3/integration/test_networks.py
+-rw-rw-r--   0 sdeziel   (1000) sdeziel   (1000)     2842 2024-01-11 18:53:51.000000 pylxd-2.3.3/integration/test_profiles.py
+-rw-rw-r--   0 sdeziel   (1000) sdeziel   (1000)     3379 2022-04-08 22:48:50.000000 pylxd-2.3.3/integration/test_projects.py
+-rw-rw-r--   0 sdeziel   (1000) sdeziel   (1000)     6082 2023-07-13 16:12:42.000000 pylxd-2.3.3/integration/test_storage.py
+-rw-rw-r--   0 sdeziel   (1000) sdeziel   (1000)     5769 2023-06-01 18:56:49.000000 pylxd-2.3.3/integration/testing.py
+drwxrwxr-x   0 sdeziel   (1000) sdeziel   (1000)        0 2024-04-29 15:37:33.511112 pylxd-2.3.3/migration/
+-rw-rw-r--   0 sdeziel   (1000) sdeziel   (1000)        0 2021-09-29 19:03:03.000000 pylxd-2.3.3/migration/__init__.py
+-rw-rw-r--   0 sdeziel   (1000) sdeziel   (1000)     5370 2023-06-01 18:56:49.000000 pylxd-2.3.3/migration/busybox.py
+-rw-rw-r--   0 sdeziel   (1000) sdeziel   (1000)     2839 2023-06-01 18:56:49.000000 pylxd-2.3.3/migration/test_containers.py
+-rw-rw-r--   0 sdeziel   (1000) sdeziel   (1000)     5329 2023-06-01 18:56:49.000000 pylxd-2.3.3/migration/testing.py
+drwxrwxr-x   0 sdeziel   (1000) sdeziel   (1000)        0 2024-04-29 15:37:33.515112 pylxd-2.3.3/pylxd/
+-rw-rw-r--   0 sdeziel   (1000) sdeziel   (1000)      696 2023-09-25 15:31:32.000000 pylxd-2.3.3/pylxd/__init__.py
+-rw-rw-r--   0 sdeziel   (1000) sdeziel   (1000)    19090 2023-08-08 15:38:43.000000 pylxd-2.3.3/pylxd/client.py
+-rw-rw-r--   0 sdeziel   (1000) sdeziel   (1000)     2135 2024-04-22 20:24:10.000000 pylxd-2.3.3/pylxd/exceptions.py
+-rw-rw-r--   0 sdeziel   (1000) sdeziel   (1000)     2456 2023-05-05 08:25:21.000000 pylxd-2.3.3/pylxd/managers.py
+drwxrwxr-x   0 sdeziel   (1000) sdeziel   (1000)        0 2024-04-29 15:37:33.519112 pylxd-2.3.3/pylxd/models/
+-rw-rw-r--   0 sdeziel   (1000) sdeziel   (1000)      911 2022-10-31 15:18:30.000000 pylxd-2.3.3/pylxd/models/__init__.py
+-rw-rw-r--   0 sdeziel   (1000) sdeziel   (1000)    12772 2024-01-17 21:29:41.000000 pylxd-2.3.3/pylxd/models/_model.py
+-rw-rw-r--   0 sdeziel   (1000) sdeziel   (1000)     3653 2022-06-06 22:07:26.000000 pylxd-2.3.3/pylxd/models/certificate.py
+-rw-rw-r--   0 sdeziel   (1000) sdeziel   (1000)     4058 2022-10-24 16:03:37.000000 pylxd-2.3.3/pylxd/models/cluster.py
+-rw-rw-r--   0 sdeziel   (1000) sdeziel   (1000)      802 2021-09-29 19:03:03.000000 pylxd-2.3.3/pylxd/models/container.py
+-rw-rw-r--   0 sdeziel   (1000) sdeziel   (1000)     8971 2024-04-26 16:18:04.000000 pylxd-2.3.3/pylxd/models/image.py
+-rw-rw-r--   0 sdeziel   (1000) sdeziel   (1000)    34058 2023-08-09 14:03:27.000000 pylxd-2.3.3/pylxd/models/instance.py
+-rw-rw-r--   0 sdeziel   (1000) sdeziel   (1000)     6223 2023-06-01 18:56:49.000000 pylxd-2.3.3/pylxd/models/network.py
+-rw-rw-r--   0 sdeziel   (1000) sdeziel   (1000)     3431 2024-01-17 21:29:41.000000 pylxd-2.3.3/pylxd/models/operation.py
+-rw-rw-r--   0 sdeziel   (1000) sdeziel   (1000)     2381 2024-01-11 18:53:51.000000 pylxd-2.3.3/pylxd/models/profile.py
+-rw-rw-r--   0 sdeziel   (1000) sdeziel   (1000)     2367 2022-09-26 21:41:17.000000 pylxd-2.3.3/pylxd/models/project.py
+-rw-rw-r--   0 sdeziel   (1000) sdeziel   (1000)    23890 2023-10-18 17:36:47.000000 pylxd-2.3.3/pylxd/models/storage_pool.py
+drwxrwxr-x   0 sdeziel   (1000) sdeziel   (1000)        0 2024-04-29 15:37:33.523112 pylxd-2.3.3/pylxd/models/tests/
+-rw-rw-r--   0 sdeziel   (1000) sdeziel   (1000)        0 2021-09-29 19:03:03.000000 pylxd-2.3.3/pylxd/models/tests/__init__.py
+-rw-rw-r--   0 sdeziel   (1000) sdeziel   (1000)     5113 2022-06-06 22:07:26.000000 pylxd-2.3.3/pylxd/models/tests/test_certificate.py
+-rw-rw-r--   0 sdeziel   (1000) sdeziel   (1000)     1858 2022-10-24 16:03:37.000000 pylxd-2.3.3/pylxd/models/tests/test_cluster.py
+-rw-rw-r--   0 sdeziel   (1000) sdeziel   (1000)     1376 2022-10-20 21:45:44.000000 pylxd-2.3.3/pylxd/models/tests/test_cluster_certificate.py
+-rw-rw-r--   0 sdeziel   (1000) sdeziel   (1000)     1204 2021-09-29 19:03:03.000000 pylxd-2.3.3/pylxd/models/tests/test_cluster_member.py
+-rw-rw-r--   0 sdeziel   (1000) sdeziel   (1000)    13387 2021-09-29 19:03:03.000000 pylxd-2.3.3/pylxd/models/tests/test_image.py
+-rw-rw-r--   0 sdeziel   (1000) sdeziel   (1000)    30217 2023-05-05 08:25:21.000000 pylxd-2.3.3/pylxd/models/tests/test_instance.py
+-rw-rw-r--   0 sdeziel   (1000) sdeziel   (1000)    11372 2021-09-29 19:03:03.000000 pylxd-2.3.3/pylxd/models/tests/test_model.py
+-rw-rw-r--   0 sdeziel   (1000) sdeziel   (1000)    14808 2023-01-11 16:17:27.000000 pylxd-2.3.3/pylxd/models/tests/test_network.py
+-rw-rw-r--   0 sdeziel   (1000) sdeziel   (1000)     5198 2024-04-22 20:24:10.000000 pylxd-2.3.3/pylxd/models/tests/test_operation.py
+-rw-rw-r--   0 sdeziel   (1000) sdeziel   (1000)     5198 2021-09-29 19:03:03.000000 pylxd-2.3.3/pylxd/models/tests/test_profile.py
+-rw-rw-r--   0 sdeziel   (1000) sdeziel   (1000)     4864 2021-09-29 19:03:03.000000 pylxd-2.3.3/pylxd/models/tests/test_project.py
+-rw-rw-r--   0 sdeziel   (1000) sdeziel   (1000)    11204 2022-10-20 15:23:34.000000 pylxd-2.3.3/pylxd/models/tests/test_storage.py
+-rw-rw-r--   0 sdeziel   (1000) sdeziel   (1000)      792 2021-09-29 19:03:03.000000 pylxd-2.3.3/pylxd/models/virtual_machine.py
+drwxrwxr-x   0 sdeziel   (1000) sdeziel   (1000)        0 2024-04-29 15:37:33.523112 pylxd-2.3.3/pylxd/tests/
+-rw-rw-r--   0 sdeziel   (1000) sdeziel   (1000)        0 2021-09-29 19:03:03.000000 pylxd-2.3.3/pylxd/tests/__init__.py
+-rw-rw-r--   0 sdeziel   (1000) sdeziel   (1000)    36958 2022-10-31 15:18:30.000000 pylxd-2.3.3/pylxd/tests/mock_lxd.py
+-rw-rw-r--   0 sdeziel   (1000) sdeziel   (1000)    24040 2023-05-05 08:25:21.000000 pylxd-2.3.3/pylxd/tests/test_client.py
+-rw-rw-r--   0 sdeziel   (1000) sdeziel   (1000)     1326 2022-10-20 15:23:34.000000 pylxd-2.3.3/pylxd/tests/testing.py
+drwxrwxr-x   0 sdeziel   (1000) sdeziel   (1000)        0 2024-04-29 15:37:33.523112 pylxd-2.3.3/pylxd.egg-info/
+-rw-r--r--   0 sdeziel   (1000) sdeziel   (1000)     2940 2024-04-29 15:37:33.000000 pylxd-2.3.3/pylxd.egg-info/PKG-INFO
+-rw-rw-r--   0 sdeziel   (1000) sdeziel   (1000)     1584 2024-04-29 15:37:33.000000 pylxd-2.3.3/pylxd.egg-info/SOURCES.txt
+-rw-rw-r--   0 sdeziel   (1000) sdeziel   (1000)        1 2024-04-29 15:37:33.000000 pylxd-2.3.3/pylxd.egg-info/dependency_links.txt
+-rw-rw-r--   0 sdeziel   (1000) sdeziel   (1000)      323 2024-04-29 15:37:33.000000 pylxd-2.3.3/pylxd.egg-info/requires.txt
+-rw-rw-r--   0 sdeziel   (1000) sdeziel   (1000)       28 2024-04-29 15:37:33.000000 pylxd-2.3.3/pylxd.egg-info/top_level.txt
+-rw-rw-r--   0 sdeziel   (1000) sdeziel   (1000)     2406 2024-04-29 15:37:33.527112 pylxd-2.3.3/setup.cfg
+-rw-rw-r--   0 sdeziel   (1000) sdeziel   (1000)      584 2023-10-17 18:41:38.000000 pylxd-2.3.3/setup.py
```

### Comparing `pylxd-2.3.2a0/CONTRIBUTORS.rst` & `pylxd-2.3.3/CONTRIBUTORS.rst`

 * *Files identical despite different names*

### Comparing `pylxd-2.3.2a0/LICENSE` & `pylxd-2.3.3/LICENSE`

 * *Files identical despite different names*

### Comparing `pylxd-2.3.2a0/README.rst` & `pylxd-2.3.3/README.rst`

 * *Files identical despite different names*

### Comparing `pylxd-2.3.2a0/integration/busybox.py` & `pylxd-2.3.3/integration/busybox.py`

 * *Files identical despite different names*

### Comparing `pylxd-2.3.2a0/integration/test_client.py` & `pylxd-2.3.3/integration/test_client.py`

 * *Files identical despite different names*

### Comparing `pylxd-2.3.2a0/integration/test_cluster_members.py` & `pylxd-2.3.3/integration/test_cluster_members.py`

 * *Files identical despite different names*

### Comparing `pylxd-2.3.2a0/integration/test_containers.py` & `pylxd-2.3.3/integration/test_containers.py`

 * *Files identical despite different names*

### Comparing `pylxd-2.3.2a0/integration/test_images.py` & `pylxd-2.3.3/integration/test_images.py`

 * *Files identical despite different names*

### Comparing `pylxd-2.3.2a0/integration/test_networks.py` & `pylxd-2.3.3/integration/test_networks.py`

 * *Files identical despite different names*

### Comparing `pylxd-2.3.2a0/integration/test_profiles.py` & `pylxd-2.3.3/integration/test_profiles.py`

 * *Files identical despite different names*

### Comparing `pylxd-2.3.2a0/integration/test_projects.py` & `pylxd-2.3.3/integration/test_projects.py`

 * *Files identical despite different names*

### Comparing `pylxd-2.3.2a0/integration/test_storage.py` & `pylxd-2.3.3/integration/test_storage.py`

 * *Files identical despite different names*

### Comparing `pylxd-2.3.2a0/integration/testing.py` & `pylxd-2.3.3/integration/testing.py`

 * *Files identical despite different names*

### Comparing `pylxd-2.3.2a0/migration/busybox.py` & `pylxd-2.3.3/migration/busybox.py`

 * *Files identical despite different names*

### Comparing `pylxd-2.3.2a0/migration/test_containers.py` & `pylxd-2.3.3/migration/test_containers.py`

 * *Files identical despite different names*

### Comparing `pylxd-2.3.2a0/migration/testing.py` & `pylxd-2.3.3/migration/testing.py`

 * *Files identical despite different names*

### Comparing `pylxd-2.3.2a0/pylxd/__init__.py` & `pylxd-2.3.3/pylxd/__init__.py`

 * *Files identical despite different names*

### Comparing `pylxd-2.3.2a0/pylxd/client.py` & `pylxd-2.3.3/pylxd/client.py`

 * *Files identical despite different names*

### Comparing `pylxd-2.3.2a0/pylxd/exceptions.py` & `pylxd-2.3.3/pylxd/exceptions.py`

 * *Files 20% similar despite different names*

```diff
@@ -13,15 +13,21 @@
     def __init__(self, response):
         super().__init__()
         self.response = response
 
     def __str__(self):
         if self.response.status_code == 200:  # Operation failure
             try:
-                return self.response.json()["metadata"]["err"]
+                json_response = self.response.json()
+                metadata = json_response.get("metadata")
+                if metadata and isinstance(metadata, dict) and "err" in metadata:
+                    return json_response["metadata"]["err"]
+                if "error" in json_response:
+                    return json_response["error"]
+                return str(json_response)
             except (ValueError, KeyError):
                 pass
 
         try:
             data = self.response.json()
             return data["error"]
         except (ValueError, KeyError):
```

### Comparing `pylxd-2.3.2a0/pylxd/managers.py` & `pylxd-2.3.3/pylxd/managers.py`

 * *Files identical despite different names*

### Comparing `pylxd-2.3.2a0/pylxd/models/__init__.py` & `pylxd-2.3.3/pylxd/models/__init__.py`

 * *Files identical despite different names*

### Comparing `pylxd-2.3.2a0/pylxd/models/_model.py` & `pylxd-2.3.3/pylxd/models/_model.py`

 * *Files 1% similar despite different names*

```diff
@@ -140,16 +140,16 @@
                 item = f"{self.__class__.__name__}.{key}"
                 if env != "always" and item in _seen_attribute_warnings:
                     continue
                 _seen_attribute_warnings.add(item)
                 if env == "none":
                     continue
                 warnings.warn(
-                    'Attempted to set unknown attribute "{}" '
-                    'on instance of "{}"'.format(key, self.__class__.__name__)
+                    f'Attempted to set unknown attribute "{key}" '
+                    f'on instance of "{self.__class__.__name__}"'
                 )
         self.__dirty__.clear()
 
     def __getattribute__(self, name):
         try:
             return super().__getattribute__(name)
         except AttributeError:
```

### Comparing `pylxd-2.3.2a0/pylxd/models/certificate.py` & `pylxd-2.3.3/pylxd/models/certificate.py`

 * *Files identical despite different names*

### Comparing `pylxd-2.3.2a0/pylxd/models/cluster.py` & `pylxd-2.3.3/pylxd/models/cluster.py`

 * *Files identical despite different names*

### Comparing `pylxd-2.3.2a0/pylxd/models/container.py` & `pylxd-2.3.3/pylxd/models/container.py`

 * *Files identical despite different names*

### Comparing `pylxd-2.3.2a0/pylxd/models/image.py` & `pylxd-2.3.3/pylxd/models/image.py`

 * *Files 4% similar despite different names*

```diff
@@ -94,15 +94,17 @@
         images = []
         for url in response.json()["metadata"]:
             fingerprint = url.split("/")[-1]
             images.append(cls(client, fingerprint=fingerprint))
         return images
 
     @classmethod
-    def create(cls, client, image_data, metadata=None, public=False, wait=True):
+    def create(
+        cls, client, image_data, metadata=None, public=False, wait=True, vm=False
+    ):
         """Create an image.
 
         If metadata is provided, a multipart form data request is formed to
         push metadata and image together in a single request. The metadata must
         be a tar achive.
 
         `wait` parameter is now ignored, as the image fingerprint cannot be
@@ -119,18 +121,31 @@
         if public:
             headers["X-LXD-Public"] = "1"
 
         if metadata is not None:
             # Image uploaded as chunked/stream (metadata, rootfs)
             # multipart message.
             # Order of parts is important metadata should be passed first
-            files = collections.OrderedDict(
-                metadata=("metadata", metadata, "application/octet-stream"),
-                rootfs=("rootfs", image_data, "application/octet-stream"),
-            )
+            files: collections.OrderedDict
+            if not vm:
+                files = collections.OrderedDict(
+                    metadata=("metadata", metadata, "application/octet-stream"),
+                    rootfs=("rootfs", image_data, "application/octet-stream"),
+                )
+            else:
+                files = collections.OrderedDict(
+                    {
+                        "metadata": ("metadata", metadata, "application/octet-stream"),
+                        "rootfs.img": (
+                            "rootfs.img",
+                            image_data,
+                            "application/octet-stream",
+                        ),
+                    }
+                )
             data = MultipartEncoder(files)
             headers.update({"Content-Type": data.content_type})
         else:
             data = image_data
 
         response = client.api.images.post(data=data, headers=headers)
         operation = client.operations.wait_for_operation(response.json()["operation"])
```

### Comparing `pylxd-2.3.2a0/pylxd/models/instance.py` & `pylxd-2.3.3/pylxd/models/instance.py`

 * *Files identical despite different names*

### Comparing `pylxd-2.3.2a0/pylxd/models/network.py` & `pylxd-2.3.3/pylxd/models/network.py`

 * *Files identical despite different names*

### Comparing `pylxd-2.3.2a0/pylxd/models/operation.py` & `pylxd-2.3.3/pylxd/models/operation.py`

 * *Files 1% similar despite different names*

```diff
@@ -80,16 +80,16 @@
                 env = os.environ.get("PYLXD_WARNINGS", "").lower()
                 if env != "always" and key in _seen_attribute_warnings:
                     continue
                 _seen_attribute_warnings.add(key)
                 if env == "none":
                     continue
                 warnings.warn(
-                    'Attempted to set unknown attribute "{}" '
-                    'on instance of "{}"'.format(key, self.__class__.__name__)
+                    f'Attempted to set unknown attribute "{key}" '
+                    f'on instance of "{self.__class__.__name__}"'
                 )
                 pass
 
     def wait(self):
         """Wait for the operation to complete and return."""
         response = self._client.api.operations[self.id].wait.get()
```

### Comparing `pylxd-2.3.2a0/pylxd/models/profile.py` & `pylxd-2.3.3/pylxd/models/profile.py`

 * *Files identical despite different names*

### Comparing `pylxd-2.3.2a0/pylxd/models/project.py` & `pylxd-2.3.3/pylxd/models/project.py`

 * *Files identical despite different names*

### Comparing `pylxd-2.3.2a0/pylxd/models/storage_pool.py` & `pylxd-2.3.3/pylxd/models/storage_pool.py`

 * *Files identical despite different names*

### Comparing `pylxd-2.3.2a0/pylxd/models/tests/test_certificate.py` & `pylxd-2.3.3/pylxd/models/tests/test_certificate.py`

 * *Files identical despite different names*

### Comparing `pylxd-2.3.2a0/pylxd/models/tests/test_cluster.py` & `pylxd-2.3.3/pylxd/models/tests/test_cluster.py`

 * *Files identical despite different names*

### Comparing `pylxd-2.3.2a0/pylxd/models/tests/test_cluster_certificate.py` & `pylxd-2.3.3/pylxd/models/tests/test_cluster_certificate.py`

 * *Files identical despite different names*

### Comparing `pylxd-2.3.2a0/pylxd/models/tests/test_cluster_member.py` & `pylxd-2.3.3/pylxd/models/tests/test_cluster_member.py`

 * *Files identical despite different names*

### Comparing `pylxd-2.3.2a0/pylxd/models/tests/test_image.py` & `pylxd-2.3.3/pylxd/models/tests/test_image.py`

 * *Files identical despite different names*

### Comparing `pylxd-2.3.2a0/pylxd/models/tests/test_instance.py` & `pylxd-2.3.3/pylxd/models/tests/test_instance.py`

 * *Files identical despite different names*

### Comparing `pylxd-2.3.2a0/pylxd/models/tests/test_model.py` & `pylxd-2.3.3/pylxd/models/tests/test_model.py`

 * *Files identical despite different names*

### Comparing `pylxd-2.3.2a0/pylxd/models/tests/test_network.py` & `pylxd-2.3.3/pylxd/models/tests/test_network.py`

 * *Files identical despite different names*

### Comparing `pylxd-2.3.2a0/pylxd/models/tests/test_operation.py` & `pylxd-2.3.3/pylxd/models/tests/test_operation.py`

 * *Files 14% similar despite different names*

```diff
@@ -96,14 +96,37 @@
 
         name = "/1.0/operations/operation-abc"
 
         an_operation = models.Operation.get(self.client, name)
 
         self.assertRaises(exceptions.LXDAPIException, an_operation.wait)
 
+    def test_wait_with_error_async_without_metadata(self):
+        """If the operation errors, wait raises an exception."""
+
+        def error(request, context):
+            context.status_code = 200
+            return {"type": "async", "error": "Could not proceed", "metadata": None}
+
+        self.add_rule(
+            {
+                "json": error,
+                "method": "GET",
+                "url": r"^http://pylxd.test/1.0/operations/operation-abc/wait$",
+            }
+        )
+
+        name = "/1.0/operations/operation-abc"
+
+        an_operation = models.Operation.get(self.client, name)
+
+        with self.assertRaises(exceptions.LXDAPIException) as wait_cm:
+            an_operation.wait()
+        assert str(wait_cm.exception) == "Could not proceed"
+
     def test_unknown_attribute(self):
         self.add_rule(
             {
                 "text": json.dumps(
                     {
                         "type": "sync",
                         "metadata": {
```

### Comparing `pylxd-2.3.2a0/pylxd/models/tests/test_profile.py` & `pylxd-2.3.3/pylxd/models/tests/test_profile.py`

 * *Files identical despite different names*

### Comparing `pylxd-2.3.2a0/pylxd/models/tests/test_project.py` & `pylxd-2.3.3/pylxd/models/tests/test_project.py`

 * *Files identical despite different names*

### Comparing `pylxd-2.3.2a0/pylxd/models/tests/test_storage.py` & `pylxd-2.3.3/pylxd/models/tests/test_storage.py`

 * *Files identical despite different names*

### Comparing `pylxd-2.3.2a0/pylxd/models/virtual_machine.py` & `pylxd-2.3.3/pylxd/models/virtual_machine.py`

 * *Files identical despite different names*

### Comparing `pylxd-2.3.2a0/pylxd/tests/mock_lxd.py` & `pylxd-2.3.3/pylxd/tests/mock_lxd.py`

 * *Files identical despite different names*

### Comparing `pylxd-2.3.2a0/pylxd/tests/test_client.py` & `pylxd-2.3.3/pylxd/tests/test_client.py`

 * *Files identical despite different names*

### Comparing `pylxd-2.3.2a0/pylxd/tests/testing.py` & `pylxd-2.3.3/pylxd/tests/testing.py`

 * *Files identical despite different names*

### Comparing `pylxd-2.3.2a0/pylxd.egg-info/SOURCES.txt` & `pylxd-2.3.3/pylxd.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pylxd-2.3.2a0/setup.cfg` & `pylxd-2.3.3/setup.cfg`

 * *Files 4% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 [metadata]
 name = pylxd
-version = 2.3.2a
+version = 2.3.3
 description = python library for LXD
 long_description = file: README.rst
+long_description_content_type = text/x-rst
 author = Paul Hummer and others (see CONTRIBUTORS.rst)
 author_email = lxd@lists.canonical.com
 home_page = https://ubuntu.com/lxd
 classifier = 
 	Intended Audience :: Information Technology
 	Intended Audience :: System Administrators
 	License :: OSI Approved :: Apache Software License
```

### Comparing `pylxd-2.3.2a0/setup.py` & `pylxd-2.3.3/setup.py`

 * *Files identical despite different names*

