# Comparing `tmp/pulumi_civo-2.4.0a1714108777.tar.gz` & `tmp/pulumi_civo-2.4.0a1714363963.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pulumi_civo-2.4.0a1714108777.tar", last modified: Fri Apr 26 05:23:51 2024, max compression
+gzip compressed data, was "pulumi_civo-2.4.0a1714363963.tar", last modified: Mon Apr 29 04:15:24 2024, max compression
```

## Comparing `pulumi_civo-2.4.0a1714108777.tar` & `pulumi_civo-2.4.0a1714363963.tar`

### file list

```diff
@@ -1,58 +1,58 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 05:23:51.673763 pulumi_civo-2.4.0a1714108777/
--rw-r--r--   0 runner    (1001) docker     (127)     2509 2024-04-26 05:23:51.673763 pulumi_civo-2.4.0a1714108777/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2065 2024-04-26 05:23:45.000000 pulumi_civo-2.4.0a1714108777/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 05:23:51.669763 pulumi_civo-2.4.0a1714108777/pulumi_civo/
--rw-r--r--   0 runner    (1001) docker     (127)     4334 2024-04-26 05:23:45.000000 pulumi_civo-2.4.0a1714108777/pulumi_civo/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    41211 2024-04-26 05:23:45.000000 pulumi_civo-2.4.0a1714108777/pulumi_civo/_inputs.py
--rw-r--r--   0 runner    (1001) docker     (127)     9248 2024-04-26 05:23:45.000000 pulumi_civo-2.4.0a1714108777/pulumi_civo/_utilities.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 05:23:51.669763 pulumi_civo-2.4.0a1714108777/pulumi_civo/config/
--rw-r--r--   0 runner    (1001) docker     (127)      285 2024-04-26 05:23:45.000000 pulumi_civo-2.4.0a1714108777/pulumi_civo/config/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      743 2024-04-26 05:23:45.000000 pulumi_civo-2.4.0a1714108777/pulumi_civo/config/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1135 2024-04-26 05:23:45.000000 pulumi_civo-2.4.0a1714108777/pulumi_civo/config/vars.py
--rw-r--r--   0 runner    (1001) docker     (127)    23846 2024-04-26 05:23:45.000000 pulumi_civo-2.4.0a1714108777/pulumi_civo/database.py
--rw-r--r--   0 runner    (1001) docker     (127)     7049 2024-04-26 05:23:45.000000 pulumi_civo-2.4.0a1714108777/pulumi_civo/dns_domain_name.py
--rw-r--r--   0 runner    (1001) docker     (127)    19775 2024-04-26 05:23:45.000000 pulumi_civo-2.4.0a1714108777/pulumi_civo/dns_domain_record.py
--rw-r--r--   0 runner    (1001) docker     (127)    18933 2024-04-26 05:23:45.000000 pulumi_civo-2.4.0a1714108777/pulumi_civo/firewall.py
--rw-r--r--   0 runner    (1001) docker     (127)    24234 2024-04-26 05:23:45.000000 pulumi_civo-2.4.0a1714108777/pulumi_civo/firewall_rule.py
--rw-r--r--   0 runner    (1001) docker     (127)     9625 2024-04-26 05:23:45.000000 pulumi_civo-2.4.0a1714108777/pulumi_civo/get_database.py
--rw-r--r--   0 runner    (1001) docker     (127)     4725 2024-04-26 05:23:45.000000 pulumi_civo-2.4.0a1714108777/pulumi_civo/get_database_version.py
--rw-r--r--   0 runner    (1001) docker     (127)     5485 2024-04-26 05:23:45.000000 pulumi_civo-2.4.0a1714108777/pulumi_civo/get_disk_image.py
--rw-r--r--   0 runner    (1001) docker     (127)     3568 2024-04-26 05:23:45.000000 pulumi_civo-2.4.0a1714108777/pulumi_civo/get_dns_domain_name.py
--rw-r--r--   0 runner    (1001) docker     (127)     7627 2024-04-26 05:23:45.000000 pulumi_civo-2.4.0a1714108777/pulumi_civo/get_dns_domain_record.py
--rw-r--r--   0 runner    (1001) docker     (127)     4813 2024-04-26 05:23:45.000000 pulumi_civo-2.4.0a1714108777/pulumi_civo/get_firewall.py
--rw-r--r--   0 runner    (1001) docker     (127)    13408 2024-04-26 05:23:45.000000 pulumi_civo-2.4.0a1714108777/pulumi_civo/get_instance.py
--rw-r--r--   0 runner    (1001) docker     (127)     6266 2024-04-26 05:23:45.000000 pulumi_civo-2.4.0a1714108777/pulumi_civo/get_instances.py
--rw-r--r--   0 runner    (1001) docker     (127)    12629 2024-04-26 05:23:45.000000 pulumi_civo-2.4.0a1714108777/pulumi_civo/get_kubernetes_cluster.py
--rw-r--r--   0 runner    (1001) docker     (127)     5511 2024-04-26 05:23:45.000000 pulumi_civo-2.4.0a1714108777/pulumi_civo/get_kubernetes_version.py
--rw-r--r--   0 runner    (1001) docker     (127)    11395 2024-04-26 05:23:45.000000 pulumi_civo-2.4.0a1714108777/pulumi_civo/get_load_balancer.py
--rw-r--r--   0 runner    (1001) docker     (127)     5164 2024-04-26 05:23:45.000000 pulumi_civo-2.4.0a1714108777/pulumi_civo/get_network.py
--rw-r--r--   0 runner    (1001) docker     (127)     6452 2024-04-26 05:23:45.000000 pulumi_civo-2.4.0a1714108777/pulumi_civo/get_object_store.py
--rw-r--r--   0 runner    (1001) docker     (127)     6960 2024-04-26 05:23:45.000000 pulumi_civo-2.4.0a1714108777/pulumi_civo/get_object_store_credential.py
--rw-r--r--   0 runner    (1001) docker     (127)     4384 2024-04-26 05:23:45.000000 pulumi_civo-2.4.0a1714108777/pulumi_civo/get_region.py
--rw-r--r--   0 runner    (1001) docker     (127)     4680 2024-04-26 05:23:45.000000 pulumi_civo-2.4.0a1714108777/pulumi_civo/get_reserved_ip.py
--rw-r--r--   0 runner    (1001) docker     (127)     4290 2024-04-26 05:23:45.000000 pulumi_civo-2.4.0a1714108777/pulumi_civo/get_size.py
--rw-r--r--   0 runner    (1001) docker     (127)     3523 2024-04-26 05:23:45.000000 pulumi_civo-2.4.0a1714108777/pulumi_civo/get_ssh_key.py
--rw-r--r--   0 runner    (1001) docker     (127)     5624 2024-04-26 05:23:45.000000 pulumi_civo-2.4.0a1714108777/pulumi_civo/get_volume.py
--rw-r--r--   0 runner    (1001) docker     (127)    47548 2024-04-26 05:23:45.000000 pulumi_civo-2.4.0a1714108777/pulumi_civo/instance.py
--rw-r--r--   0 runner    (1001) docker     (127)    10269 2024-04-26 05:23:45.000000 pulumi_civo-2.4.0a1714108777/pulumi_civo/instance_reserved_ip_assignment.py
--rw-r--r--   0 runner    (1001) docker     (127)    44029 2024-04-26 05:23:45.000000 pulumi_civo-2.4.0a1714108777/pulumi_civo/kubernetes_cluster.py
--rw-r--r--   0 runner    (1001) docker     (127)    20650 2024-04-26 05:23:45.000000 pulumi_civo-2.4.0a1714108777/pulumi_civo/kubernetes_node_pool.py
--rw-r--r--   0 runner    (1001) docker     (127)     9516 2024-04-26 05:23:45.000000 pulumi_civo-2.4.0a1714108777/pulumi_civo/network.py
--rw-r--r--   0 runner    (1001) docker     (127)    15632 2024-04-26 05:23:45.000000 pulumi_civo-2.4.0a1714108777/pulumi_civo/object_store.py
--rw-r--r--   0 runner    (1001) docker     (127)    15459 2024-04-26 05:23:45.000000 pulumi_civo-2.4.0a1714108777/pulumi_civo/object_store_credential.py
--rw-r--r--   0 runner    (1001) docker     (127)    55857 2024-04-26 05:23:45.000000 pulumi_civo-2.4.0a1714108777/pulumi_civo/outputs.py
--rw-r--r--   0 runner    (1001) docker     (127)     7299 2024-04-26 05:23:45.000000 pulumi_civo-2.4.0a1714108777/pulumi_civo/provider.py
--rw-r--r--   0 runner    (1001) docker     (127)       41 2024-04-26 05:23:45.000000 pulumi_civo-2.4.0a1714108777/pulumi_civo/pulumi-plugin.json
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-26 05:23:45.000000 pulumi_civo-2.4.0a1714108777/pulumi_civo/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)     8431 2024-04-26 05:23:45.000000 pulumi_civo-2.4.0a1714108777/pulumi_civo/reserved_ip.py
--rw-r--r--   0 runner    (1001) docker     (127)     9505 2024-04-26 05:23:45.000000 pulumi_civo-2.4.0a1714108777/pulumi_civo/ssh_key.py
--rw-r--r--   0 runner    (1001) docker     (127)    14175 2024-04-26 05:23:45.000000 pulumi_civo-2.4.0a1714108777/pulumi_civo/volume.py
--rw-r--r--   0 runner    (1001) docker     (127)     9414 2024-04-26 05:23:45.000000 pulumi_civo-2.4.0a1714108777/pulumi_civo/volume_attachment.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 05:23:51.669763 pulumi_civo-2.4.0a1714108777/pulumi_civo.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2509 2024-04-26 05:23:51.000000 pulumi_civo-2.4.0a1714108777/pulumi_civo.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1533 2024-04-26 05:23:51.000000 pulumi_civo-2.4.0a1714108777/pulumi_civo.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-26 05:23:51.000000 pulumi_civo-2.4.0a1714108777/pulumi_civo.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       49 2024-04-26 05:23:51.000000 pulumi_civo-2.4.0a1714108777/pulumi_civo.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       12 2024-04-26 05:23:51.000000 pulumi_civo-2.4.0a1714108777/pulumi_civo.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      669 2024-04-26 05:23:45.000000 pulumi_civo-2.4.0a1714108777/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-26 05:23:51.673763 pulumi_civo-2.4.0a1714108777/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 04:15:24.146010 pulumi_civo-2.4.0a1714363963/
+-rw-r--r--   0 runner    (1001) docker     (127)     2509 2024-04-29 04:15:24.146010 pulumi_civo-2.4.0a1714363963/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2065 2024-04-29 04:15:17.000000 pulumi_civo-2.4.0a1714363963/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 04:15:24.142010 pulumi_civo-2.4.0a1714363963/pulumi_civo/
+-rw-r--r--   0 runner    (1001) docker     (127)     4334 2024-04-29 04:15:17.000000 pulumi_civo-2.4.0a1714363963/pulumi_civo/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    41211 2024-04-29 04:15:17.000000 pulumi_civo-2.4.0a1714363963/pulumi_civo/_inputs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9248 2024-04-29 04:15:17.000000 pulumi_civo-2.4.0a1714363963/pulumi_civo/_utilities.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 04:15:24.142010 pulumi_civo-2.4.0a1714363963/pulumi_civo/config/
+-rw-r--r--   0 runner    (1001) docker     (127)      285 2024-04-29 04:15:17.000000 pulumi_civo-2.4.0a1714363963/pulumi_civo/config/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      743 2024-04-29 04:15:17.000000 pulumi_civo-2.4.0a1714363963/pulumi_civo/config/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1135 2024-04-29 04:15:17.000000 pulumi_civo-2.4.0a1714363963/pulumi_civo/config/vars.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23846 2024-04-29 04:15:17.000000 pulumi_civo-2.4.0a1714363963/pulumi_civo/database.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7049 2024-04-29 04:15:17.000000 pulumi_civo-2.4.0a1714363963/pulumi_civo/dns_domain_name.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19775 2024-04-29 04:15:17.000000 pulumi_civo-2.4.0a1714363963/pulumi_civo/dns_domain_record.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18933 2024-04-29 04:15:17.000000 pulumi_civo-2.4.0a1714363963/pulumi_civo/firewall.py
+-rw-r--r--   0 runner    (1001) docker     (127)    24234 2024-04-29 04:15:17.000000 pulumi_civo-2.4.0a1714363963/pulumi_civo/firewall_rule.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9625 2024-04-29 04:15:17.000000 pulumi_civo-2.4.0a1714363963/pulumi_civo/get_database.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4725 2024-04-29 04:15:17.000000 pulumi_civo-2.4.0a1714363963/pulumi_civo/get_database_version.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5485 2024-04-29 04:15:17.000000 pulumi_civo-2.4.0a1714363963/pulumi_civo/get_disk_image.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3568 2024-04-29 04:15:17.000000 pulumi_civo-2.4.0a1714363963/pulumi_civo/get_dns_domain_name.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7627 2024-04-29 04:15:17.000000 pulumi_civo-2.4.0a1714363963/pulumi_civo/get_dns_domain_record.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4813 2024-04-29 04:15:17.000000 pulumi_civo-2.4.0a1714363963/pulumi_civo/get_firewall.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13408 2024-04-29 04:15:17.000000 pulumi_civo-2.4.0a1714363963/pulumi_civo/get_instance.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6266 2024-04-29 04:15:17.000000 pulumi_civo-2.4.0a1714363963/pulumi_civo/get_instances.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12629 2024-04-29 04:15:17.000000 pulumi_civo-2.4.0a1714363963/pulumi_civo/get_kubernetes_cluster.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5511 2024-04-29 04:15:17.000000 pulumi_civo-2.4.0a1714363963/pulumi_civo/get_kubernetes_version.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11395 2024-04-29 04:15:17.000000 pulumi_civo-2.4.0a1714363963/pulumi_civo/get_load_balancer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5164 2024-04-29 04:15:17.000000 pulumi_civo-2.4.0a1714363963/pulumi_civo/get_network.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6452 2024-04-29 04:15:17.000000 pulumi_civo-2.4.0a1714363963/pulumi_civo/get_object_store.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6960 2024-04-29 04:15:17.000000 pulumi_civo-2.4.0a1714363963/pulumi_civo/get_object_store_credential.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4384 2024-04-29 04:15:17.000000 pulumi_civo-2.4.0a1714363963/pulumi_civo/get_region.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4680 2024-04-29 04:15:17.000000 pulumi_civo-2.4.0a1714363963/pulumi_civo/get_reserved_ip.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4290 2024-04-29 04:15:17.000000 pulumi_civo-2.4.0a1714363963/pulumi_civo/get_size.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3523 2024-04-29 04:15:17.000000 pulumi_civo-2.4.0a1714363963/pulumi_civo/get_ssh_key.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5624 2024-04-29 04:15:17.000000 pulumi_civo-2.4.0a1714363963/pulumi_civo/get_volume.py
+-rw-r--r--   0 runner    (1001) docker     (127)    47548 2024-04-29 04:15:17.000000 pulumi_civo-2.4.0a1714363963/pulumi_civo/instance.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10269 2024-04-29 04:15:17.000000 pulumi_civo-2.4.0a1714363963/pulumi_civo/instance_reserved_ip_assignment.py
+-rw-r--r--   0 runner    (1001) docker     (127)    44029 2024-04-29 04:15:17.000000 pulumi_civo-2.4.0a1714363963/pulumi_civo/kubernetes_cluster.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20650 2024-04-29 04:15:17.000000 pulumi_civo-2.4.0a1714363963/pulumi_civo/kubernetes_node_pool.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9516 2024-04-29 04:15:17.000000 pulumi_civo-2.4.0a1714363963/pulumi_civo/network.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15632 2024-04-29 04:15:17.000000 pulumi_civo-2.4.0a1714363963/pulumi_civo/object_store.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15459 2024-04-29 04:15:17.000000 pulumi_civo-2.4.0a1714363963/pulumi_civo/object_store_credential.py
+-rw-r--r--   0 runner    (1001) docker     (127)    55857 2024-04-29 04:15:17.000000 pulumi_civo-2.4.0a1714363963/pulumi_civo/outputs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7299 2024-04-29 04:15:17.000000 pulumi_civo-2.4.0a1714363963/pulumi_civo/provider.py
+-rw-r--r--   0 runner    (1001) docker     (127)       41 2024-04-29 04:15:17.000000 pulumi_civo-2.4.0a1714363963/pulumi_civo/pulumi-plugin.json
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-29 04:15:17.000000 pulumi_civo-2.4.0a1714363963/pulumi_civo/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)     8431 2024-04-29 04:15:17.000000 pulumi_civo-2.4.0a1714363963/pulumi_civo/reserved_ip.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9505 2024-04-29 04:15:17.000000 pulumi_civo-2.4.0a1714363963/pulumi_civo/ssh_key.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14175 2024-04-29 04:15:17.000000 pulumi_civo-2.4.0a1714363963/pulumi_civo/volume.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9414 2024-04-29 04:15:17.000000 pulumi_civo-2.4.0a1714363963/pulumi_civo/volume_attachment.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 04:15:24.142010 pulumi_civo-2.4.0a1714363963/pulumi_civo.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2509 2024-04-29 04:15:24.000000 pulumi_civo-2.4.0a1714363963/pulumi_civo.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1533 2024-04-29 04:15:24.000000 pulumi_civo-2.4.0a1714363963/pulumi_civo.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-29 04:15:24.000000 pulumi_civo-2.4.0a1714363963/pulumi_civo.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       49 2024-04-29 04:15:24.000000 pulumi_civo-2.4.0a1714363963/pulumi_civo.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       12 2024-04-29 04:15:24.000000 pulumi_civo-2.4.0a1714363963/pulumi_civo.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      669 2024-04-29 04:15:17.000000 pulumi_civo-2.4.0a1714363963/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-29 04:15:24.146010 pulumi_civo-2.4.0a1714363963/setup.cfg
```

### Comparing `pulumi_civo-2.4.0a1714108777/PKG-INFO` & `pulumi_civo-2.4.0a1714363963/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pulumi_civo
-Version: 2.4.0a1714108777
+Version: 2.4.0a1714363963
 Summary: A Pulumi package for creating and managing Civo cloud resources.
 License: Apache-2.0
 Project-URL: Homepage, https://pulumi.io
 Project-URL: Repository, https://github.com/pulumi/pulumi-civo
 Keywords: pulumi,civo
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
```

### Comparing `pulumi_civo-2.4.0a1714108777/README.md` & `pulumi_civo-2.4.0a1714363963/README.md`

 * *Files identical despite different names*

### Comparing `pulumi_civo-2.4.0a1714108777/pulumi_civo/__init__.py` & `pulumi_civo-2.4.0a1714363963/pulumi_civo/__init__.py`

 * *Files identical despite different names*

### Comparing `pulumi_civo-2.4.0a1714108777/pulumi_civo/_inputs.py` & `pulumi_civo-2.4.0a1714363963/pulumi_civo/_inputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_civo-2.4.0a1714108777/pulumi_civo/_utilities.py` & `pulumi_civo-2.4.0a1714363963/pulumi_civo/_utilities.py`

 * *Files identical despite different names*

### Comparing `pulumi_civo-2.4.0a1714108777/pulumi_civo/config/__init__.pyi` & `pulumi_civo-2.4.0a1714363963/pulumi_civo/config/__init__.pyi`

 * *Files identical despite different names*

### Comparing `pulumi_civo-2.4.0a1714108777/pulumi_civo/config/vars.py` & `pulumi_civo-2.4.0a1714363963/pulumi_civo/config/vars.py`

 * *Files identical despite different names*

### Comparing `pulumi_civo-2.4.0a1714108777/pulumi_civo/database.py` & `pulumi_civo-2.4.0a1714363963/pulumi_civo/database.py`

 * *Files identical despite different names*

### Comparing `pulumi_civo-2.4.0a1714108777/pulumi_civo/dns_domain_name.py` & `pulumi_civo-2.4.0a1714363963/pulumi_civo/dns_domain_name.py`

 * *Files identical despite different names*

### Comparing `pulumi_civo-2.4.0a1714108777/pulumi_civo/dns_domain_record.py` & `pulumi_civo-2.4.0a1714363963/pulumi_civo/dns_domain_record.py`

 * *Files identical despite different names*

### Comparing `pulumi_civo-2.4.0a1714108777/pulumi_civo/firewall.py` & `pulumi_civo-2.4.0a1714363963/pulumi_civo/firewall.py`

 * *Files identical despite different names*

### Comparing `pulumi_civo-2.4.0a1714108777/pulumi_civo/firewall_rule.py` & `pulumi_civo-2.4.0a1714363963/pulumi_civo/firewall_rule.py`

 * *Files identical despite different names*

### Comparing `pulumi_civo-2.4.0a1714108777/pulumi_civo/get_database.py` & `pulumi_civo-2.4.0a1714363963/pulumi_civo/get_database.py`

 * *Files identical despite different names*

### Comparing `pulumi_civo-2.4.0a1714108777/pulumi_civo/get_database_version.py` & `pulumi_civo-2.4.0a1714363963/pulumi_civo/get_database_version.py`

 * *Files identical despite different names*

### Comparing `pulumi_civo-2.4.0a1714108777/pulumi_civo/get_disk_image.py` & `pulumi_civo-2.4.0a1714363963/pulumi_civo/get_disk_image.py`

 * *Files identical despite different names*

### Comparing `pulumi_civo-2.4.0a1714108777/pulumi_civo/get_dns_domain_name.py` & `pulumi_civo-2.4.0a1714363963/pulumi_civo/get_dns_domain_name.py`

 * *Files identical despite different names*

### Comparing `pulumi_civo-2.4.0a1714108777/pulumi_civo/get_dns_domain_record.py` & `pulumi_civo-2.4.0a1714363963/pulumi_civo/get_dns_domain_record.py`

 * *Files identical despite different names*

### Comparing `pulumi_civo-2.4.0a1714108777/pulumi_civo/get_firewall.py` & `pulumi_civo-2.4.0a1714363963/pulumi_civo/get_firewall.py`

 * *Files identical despite different names*

### Comparing `pulumi_civo-2.4.0a1714108777/pulumi_civo/get_instance.py` & `pulumi_civo-2.4.0a1714363963/pulumi_civo/get_instance.py`

 * *Files identical despite different names*

### Comparing `pulumi_civo-2.4.0a1714108777/pulumi_civo/get_instances.py` & `pulumi_civo-2.4.0a1714363963/pulumi_civo/get_instances.py`

 * *Files identical despite different names*

### Comparing `pulumi_civo-2.4.0a1714108777/pulumi_civo/get_kubernetes_cluster.py` & `pulumi_civo-2.4.0a1714363963/pulumi_civo/get_kubernetes_cluster.py`

 * *Files identical despite different names*

### Comparing `pulumi_civo-2.4.0a1714108777/pulumi_civo/get_kubernetes_version.py` & `pulumi_civo-2.4.0a1714363963/pulumi_civo/get_kubernetes_version.py`

 * *Files identical despite different names*

### Comparing `pulumi_civo-2.4.0a1714108777/pulumi_civo/get_load_balancer.py` & `pulumi_civo-2.4.0a1714363963/pulumi_civo/get_load_balancer.py`

 * *Files identical despite different names*

### Comparing `pulumi_civo-2.4.0a1714108777/pulumi_civo/get_network.py` & `pulumi_civo-2.4.0a1714363963/pulumi_civo/get_network.py`

 * *Files identical despite different names*

### Comparing `pulumi_civo-2.4.0a1714108777/pulumi_civo/get_object_store.py` & `pulumi_civo-2.4.0a1714363963/pulumi_civo/get_object_store.py`

 * *Files identical despite different names*

### Comparing `pulumi_civo-2.4.0a1714108777/pulumi_civo/get_object_store_credential.py` & `pulumi_civo-2.4.0a1714363963/pulumi_civo/get_object_store_credential.py`

 * *Files identical despite different names*

### Comparing `pulumi_civo-2.4.0a1714108777/pulumi_civo/get_region.py` & `pulumi_civo-2.4.0a1714363963/pulumi_civo/get_region.py`

 * *Files identical despite different names*

### Comparing `pulumi_civo-2.4.0a1714108777/pulumi_civo/get_reserved_ip.py` & `pulumi_civo-2.4.0a1714363963/pulumi_civo/get_reserved_ip.py`

 * *Files identical despite different names*

### Comparing `pulumi_civo-2.4.0a1714108777/pulumi_civo/get_size.py` & `pulumi_civo-2.4.0a1714363963/pulumi_civo/get_size.py`

 * *Files identical despite different names*

### Comparing `pulumi_civo-2.4.0a1714108777/pulumi_civo/get_ssh_key.py` & `pulumi_civo-2.4.0a1714363963/pulumi_civo/get_ssh_key.py`

 * *Files identical despite different names*

### Comparing `pulumi_civo-2.4.0a1714108777/pulumi_civo/get_volume.py` & `pulumi_civo-2.4.0a1714363963/pulumi_civo/get_volume.py`

 * *Files identical despite different names*

### Comparing `pulumi_civo-2.4.0a1714108777/pulumi_civo/instance.py` & `pulumi_civo-2.4.0a1714363963/pulumi_civo/instance.py`

 * *Files identical despite different names*

### Comparing `pulumi_civo-2.4.0a1714108777/pulumi_civo/instance_reserved_ip_assignment.py` & `pulumi_civo-2.4.0a1714363963/pulumi_civo/instance_reserved_ip_assignment.py`

 * *Files identical despite different names*

### Comparing `pulumi_civo-2.4.0a1714108777/pulumi_civo/kubernetes_cluster.py` & `pulumi_civo-2.4.0a1714363963/pulumi_civo/kubernetes_cluster.py`

 * *Files identical despite different names*

### Comparing `pulumi_civo-2.4.0a1714108777/pulumi_civo/kubernetes_node_pool.py` & `pulumi_civo-2.4.0a1714363963/pulumi_civo/kubernetes_node_pool.py`

 * *Files identical despite different names*

### Comparing `pulumi_civo-2.4.0a1714108777/pulumi_civo/network.py` & `pulumi_civo-2.4.0a1714363963/pulumi_civo/network.py`

 * *Files identical despite different names*

### Comparing `pulumi_civo-2.4.0a1714108777/pulumi_civo/object_store.py` & `pulumi_civo-2.4.0a1714363963/pulumi_civo/object_store.py`

 * *Files identical despite different names*

### Comparing `pulumi_civo-2.4.0a1714108777/pulumi_civo/object_store_credential.py` & `pulumi_civo-2.4.0a1714363963/pulumi_civo/object_store_credential.py`

 * *Files identical despite different names*

### Comparing `pulumi_civo-2.4.0a1714108777/pulumi_civo/outputs.py` & `pulumi_civo-2.4.0a1714363963/pulumi_civo/outputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_civo-2.4.0a1714108777/pulumi_civo/provider.py` & `pulumi_civo-2.4.0a1714363963/pulumi_civo/provider.py`

 * *Files identical despite different names*

### Comparing `pulumi_civo-2.4.0a1714108777/pulumi_civo/reserved_ip.py` & `pulumi_civo-2.4.0a1714363963/pulumi_civo/reserved_ip.py`

 * *Files identical despite different names*

### Comparing `pulumi_civo-2.4.0a1714108777/pulumi_civo/ssh_key.py` & `pulumi_civo-2.4.0a1714363963/pulumi_civo/ssh_key.py`

 * *Files identical despite different names*

### Comparing `pulumi_civo-2.4.0a1714108777/pulumi_civo/volume.py` & `pulumi_civo-2.4.0a1714363963/pulumi_civo/volume.py`

 * *Files identical despite different names*

### Comparing `pulumi_civo-2.4.0a1714108777/pulumi_civo/volume_attachment.py` & `pulumi_civo-2.4.0a1714363963/pulumi_civo/volume_attachment.py`

 * *Files identical despite different names*

### Comparing `pulumi_civo-2.4.0a1714108777/pulumi_civo.egg-info/PKG-INFO` & `pulumi_civo-2.4.0a1714363963/pulumi_civo.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pulumi_civo
-Version: 2.4.0a1714108777
+Version: 2.4.0a1714363963
 Summary: A Pulumi package for creating and managing Civo cloud resources.
 License: Apache-2.0
 Project-URL: Homepage, https://pulumi.io
 Project-URL: Repository, https://github.com/pulumi/pulumi-civo
 Keywords: pulumi,civo
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
```

### Comparing `pulumi_civo-2.4.0a1714108777/pulumi_civo.egg-info/SOURCES.txt` & `pulumi_civo-2.4.0a1714363963/pulumi_civo.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pulumi_civo-2.4.0a1714108777/pyproject.toml` & `pulumi_civo-2.4.0a1714363963/pyproject.toml`

 * *Files 17% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [project]
   name = "pulumi_civo"
   description = "A Pulumi package for creating and managing Civo cloud resources."
   dependencies = ["parver>=0.2.1", "pulumi>=3.0.0,<4.0.0", "semver>=2.8.1"]
   keywords = ["pulumi", "civo"]
   readme = "README.md"
   requires-python = ">=3.8"
-  version = "2.4.0a1714108777"
+  version = "2.4.0a1714363963"
   [project.license]
     text = "Apache-2.0"
   [project.urls]
     Homepage = "https://pulumi.io"
     Repository = "https://github.com/pulumi/pulumi-civo"
 
 [build-system]
```
