# Comparing `tmp/netbox_docker_plugin-1.6.1.tar.gz` & `tmp/netbox_docker_plugin-1.6.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "netbox_docker_plugin-1.6.1.tar", last modified: Mon Apr 22 12:19:59 2024, max compression
+gzip compressed data, was "netbox_docker_plugin-1.6.2.tar", last modified: Mon Apr 29 13:08:57 2024, max compression
```

## Comparing `netbox_docker_plugin-1.6.1.tar` & `netbox_docker_plugin-1.6.2.tar`

### file list

```diff
@@ -1,132 +1,132 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 12:19:59.630593 netbox_docker_plugin-1.6.1/
--rw-r--r--   0 runner    (1001) docker     (127)     1494 2024-04-22 12:19:56.000000 netbox_docker_plugin-1.6.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       56 2024-04-22 12:19:56.000000 netbox_docker_plugin-1.6.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     5117 2024-04-22 12:19:59.630593 netbox_docker_plugin-1.6.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     4633 2024-04-22 12:19:56.000000 netbox_docker_plugin-1.6.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 12:19:59.610593 netbox_docker_plugin-1.6.1/netbox_docker_plugin/
--rw-r--r--   0 runner    (1001) docker     (127)      608 2024-04-22 12:19:56.000000 netbox_docker_plugin-1.6.1/netbox_docker_plugin/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 12:19:59.614593 netbox_docker_plugin-1.6.1/netbox_docker_plugin/api/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-22 12:19:56.000000 netbox_docker_plugin-1.6.1/netbox_docker_plugin/api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    15301 2024-04-22 12:19:56.000000 netbox_docker_plugin-1.6.1/netbox_docker_plugin/api/serializers.py
--rw-r--r--   0 runner    (1001) docker     (127)      474 2024-04-22 12:19:56.000000 netbox_docker_plugin-1.6.1/netbox_docker_plugin/api/urls.py
--rw-r--r--   0 runner    (1001) docker     (127)     3344 2024-04-22 12:19:56.000000 netbox_docker_plugin-1.6.1/netbox_docker_plugin/api/views.py
--rw-r--r--   0 runner    (1001) docker     (127)     7310 2024-04-22 12:19:56.000000 netbox_docker_plugin-1.6.1/netbox_docker_plugin/filtersets.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 12:19:59.614593 netbox_docker_plugin-1.6.1/netbox_docker_plugin/forms/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-22 12:19:56.000000 netbox_docker_plugin-1.6.1/netbox_docker_plugin/forms/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1158 2024-04-22 12:19:56.000000 netbox_docker_plugin-1.6.1/netbox_docker_plugin/forms/bind.py
--rw-r--r--   0 runner    (1001) docker     (127)     4199 2024-04-22 12:19:56.000000 netbox_docker_plugin-1.6.1/netbox_docker_plugin/forms/container.py
--rw-r--r--   0 runner    (1001) docker     (127)      736 2024-04-22 12:19:56.000000 netbox_docker_plugin-1.6.1/netbox_docker_plugin/forms/env.py
--rw-r--r--   0 runner    (1001) docker     (127)     1958 2024-04-22 12:19:56.000000 netbox_docker_plugin-1.6.1/netbox_docker_plugin/forms/host.py
--rw-r--r--   0 runner    (1001) docker     (127)     2743 2024-04-22 12:19:56.000000 netbox_docker_plugin-1.6.1/netbox_docker_plugin/forms/image.py
--rw-r--r--   0 runner    (1001) docker     (127)      728 2024-04-22 12:19:56.000000 netbox_docker_plugin-1.6.1/netbox_docker_plugin/forms/label.py
--rw-r--r--   0 runner    (1001) docker     (127)     1411 2024-04-22 12:19:56.000000 netbox_docker_plugin-1.6.1/netbox_docker_plugin/forms/mount.py
--rw-r--r--   0 runner    (1001) docker     (127)     2837 2024-04-22 12:19:56.000000 netbox_docker_plugin-1.6.1/netbox_docker_plugin/forms/network.py
--rw-r--r--   0 runner    (1001) docker     (127)     1428 2024-04-22 12:19:56.000000 netbox_docker_plugin-1.6.1/netbox_docker_plugin/forms/network_setting.py
--rw-r--r--   0 runner    (1001) docker     (127)      815 2024-04-22 12:19:56.000000 netbox_docker_plugin-1.6.1/netbox_docker_plugin/forms/port.py
--rw-r--r--   0 runner    (1001) docker     (127)     1318 2024-04-22 12:19:56.000000 netbox_docker_plugin-1.6.1/netbox_docker_plugin/forms/registry.py
--rw-r--r--   0 runner    (1001) docker     (127)     1701 2024-04-22 12:19:56.000000 netbox_docker_plugin-1.6.1/netbox_docker_plugin/forms/volume.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 12:19:59.618593 netbox_docker_plugin-1.6.1/netbox_docker_plugin/migrations/
--rw-r--r--   0 runner    (1001) docker     (127)     1087 2024-04-22 12:19:56.000000 netbox_docker_plugin-1.6.1/netbox_docker_plugin/migrations/0001_initial.py
--rw-r--r--   0 runner    (1001) docker     (127)     1629 2024-04-22 12:19:56.000000 netbox_docker_plugin-1.6.1/netbox_docker_plugin/migrations/0002_image.py
--rw-r--r--   0 runner    (1001) docker     (127)      669 2024-04-22 12:19:56.000000 netbox_docker_plugin-1.6.1/netbox_docker_plugin/migrations/0003_image_size.py
--rw-r--r--   0 runner    (1001) docker     (127)     1292 2024-04-22 12:19:56.000000 netbox_docker_plugin-1.6.1/netbox_docker_plugin/migrations/0004_volume.py
--rw-r--r--   0 runner    (1001) docker     (127)     1337 2024-04-22 12:19:56.000000 netbox_docker_plugin-1.6.1/netbox_docker_plugin/migrations/0005_network.py
--rw-r--r--   0 runner    (1001) docker     (127)     9267 2024-04-22 12:19:56.000000 netbox_docker_plugin-1.6.1/netbox_docker_plugin/migrations/0006_container_port_mount_label_env_and_more.py
--rw-r--r--   0 runner    (1001) docker     (127)     1904 2024-04-22 12:19:56.000000 netbox_docker_plugin-1.6.1/netbox_docker_plugin/migrations/0007_remove_container_netbox_docker_plugin_container_unique_name_host__and_more.py
--rw-r--r--   0 runner    (1001) docker     (127)     1468 2024-04-22 12:19:56.000000 netbox_docker_plugin-1.6.1/netbox_docker_plugin/migrations/0008_alter_network_unique_together_network_networkid_and_more.py
--rw-r--r--   0 runner    (1001) docker     (127)     2092 2024-04-22 12:19:56.000000 netbox_docker_plugin-1.6.1/netbox_docker_plugin/migrations/0009_remove_container_network_networksettings_and_more.py
--rw-r--r--   0 runner    (1001) docker     (127)     1088 2024-04-22 12:19:56.000000 netbox_docker_plugin-1.6.1/netbox_docker_plugin/migrations/0010_container_containerid_and_more.py
--rw-r--r--   0 runner    (1001) docker     (127)      664 2024-04-22 12:19:56.000000 netbox_docker_plugin-1.6.1/netbox_docker_plugin/migrations/0011_host_token.py
--rw-r--r--   0 runner    (1001) docker     (127)      541 2024-04-22 12:19:56.000000 netbox_docker_plugin-1.6.1/netbox_docker_plugin/migrations/0012_host_state.py
--rw-r--r--   0 runner    (1001) docker     (127)      605 2024-04-22 12:19:56.000000 netbox_docker_plugin-1.6.1/netbox_docker_plugin/migrations/0013_host_netbox_url.py
--rw-r--r--   0 runner    (1001) docker     (127)      441 2024-04-22 12:19:56.000000 netbox_docker_plugin-1.6.1/netbox_docker_plugin/migrations/0014_container_operation.py
--rw-r--r--   0 runner    (1001) docker     (127)      674 2024-04-22 12:19:56.000000 netbox_docker_plugin-1.6.1/netbox_docker_plugin/migrations/0015_remove_mount_netbox_docker_plugin_mount_unique_volume_and_more.py
--rw-r--r--   0 runner    (1001) docker     (127)      716 2024-04-22 12:19:56.000000 netbox_docker_plugin-1.6.1/netbox_docker_plugin/migrations/0016_alter_env_value.py
--rw-r--r--   0 runner    (1001) docker     (127)      437 2024-04-22 12:19:56.000000 netbox_docker_plugin-1.6.1/netbox_docker_plugin/migrations/0017_network_state.py
--rw-r--r--   0 runner    (1001) docker     (127)      925 2024-04-22 12:19:56.000000 netbox_docker_plugin-1.6.1/netbox_docker_plugin/migrations/0018_alter_mount_volume_alter_networksetting_network.py
--rw-r--r--   0 runner    (1001) docker     (127)      695 2024-04-22 12:19:56.000000 netbox_docker_plugin-1.6.1/netbox_docker_plugin/migrations/0019_host_agent_version_host_docker_api_version.py
--rw-r--r--   0 runner    (1001) docker     (127)      771 2024-04-22 12:19:56.000000 netbox_docker_plugin-1.6.1/netbox_docker_plugin/migrations/0020_container_hostname.py
--rw-r--r--   0 runner    (1001) docker     (127)     3042 2024-04-22 12:19:56.000000 netbox_docker_plugin-1.6.1/netbox_docker_plugin/migrations/0021_registry_and_more.py
--rw-r--r--   0 runner    (1001) docker     (127)     2410 2024-04-22 12:19:56.000000 netbox_docker_plugin-1.6.1/netbox_docker_plugin/migrations/0022_bind_bind_netbox_docker_plugin_bind_unique_bind.py
--rw-r--r--   0 runner    (1001) docker     (127)      842 2024-04-22 12:19:56.000000 netbox_docker_plugin-1.6.1/netbox_docker_plugin/migrations/0023_delete_hosts.py
--rw-r--r--   0 runner    (1001) docker     (127)     1351 2024-04-22 12:19:56.000000 netbox_docker_plugin-1.6.1/netbox_docker_plugin/migrations/0024_registry_host_alter_registry_name_and_more.py
--rw-r--r--   0 runner    (1001) docker     (127)      747 2024-04-22 12:19:56.000000 netbox_docker_plugin-1.6.1/netbox_docker_plugin/migrations/0025_alter_image_version.py
--rw-r--r--   0 runner    (1001) docker     (127)      742 2024-04-22 12:19:56.000000 netbox_docker_plugin-1.6.1/netbox_docker_plugin/migrations/0026_image_digest.py
--rw-r--r--   0 runner    (1001) docker     (127)      438 2024-04-22 12:19:56.000000 netbox_docker_plugin-1.6.1/netbox_docker_plugin/migrations/0027_container_restart_policy.py
--rw-r--r--   0 runner    (1001) docker     (127)      858 2024-04-22 12:19:56.000000 netbox_docker_plugin-1.6.1/netbox_docker_plugin/migrations/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 12:19:59.622593 netbox_docker_plugin-1.6.1/netbox_docker_plugin/models/
--rw-r--r--   0 runner    (1001) docker     (127)      194 2024-04-22 12:19:56.000000 netbox_docker_plugin-1.6.1/netbox_docker_plugin/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    10657 2024-04-22 12:19:56.000000 netbox_docker_plugin-1.6.1/netbox_docker_plugin/models/container.py
--rw-r--r--   0 runner    (1001) docker     (127)     2045 2024-04-22 12:19:56.000000 netbox_docker_plugin-1.6.1/netbox_docker_plugin/models/host.py
--rw-r--r--   0 runner    (1001) docker     (127)     2323 2024-04-22 12:19:56.000000 netbox_docker_plugin-1.6.1/netbox_docker_plugin/models/image.py
--rw-r--r--   0 runner    (1001) docker     (127)     2369 2024-04-22 12:19:56.000000 netbox_docker_plugin-1.6.1/netbox_docker_plugin/models/network.py
--rw-r--r--   0 runner    (1001) docker     (127)     1776 2024-04-22 12:19:56.000000 netbox_docker_plugin-1.6.1/netbox_docker_plugin/models/registry.py
--rw-r--r--   0 runner    (1001) docker     (127)     1307 2024-04-22 12:19:56.000000 netbox_docker_plugin-1.6.1/netbox_docker_plugin/models/volume.py
--rw-r--r--   0 runner    (1001) docker     (127)     3732 2024-04-22 12:19:56.000000 netbox_docker_plugin-1.6.1/netbox_docker_plugin/navigation.py
--rw-r--r--   0 runner    (1001) docker     (127)    10276 2024-04-22 12:19:56.000000 netbox_docker_plugin-1.6.1/netbox_docker_plugin/tables.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 12:19:59.610593 netbox_docker_plugin-1.6.1/netbox_docker_plugin/templates/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 12:19:59.622593 netbox_docker_plugin-1.6.1/netbox_docker_plugin/templates/netbox_docker_plugin/
--rw-r--r--   0 runner    (1001) docker     (127)     7124 2024-04-22 12:19:56.000000 netbox_docker_plugin-1.6.1/netbox_docker_plugin/templates/netbox_docker_plugin/container.html
--rw-r--r--   0 runner    (1001) docker     (127)     5086 2024-04-22 12:19:56.000000 netbox_docker_plugin-1.6.1/netbox_docker_plugin/templates/netbox_docker_plugin/host.html
--rw-r--r--   0 runner    (1001) docker     (127)     1808 2024-04-22 12:19:56.000000 netbox_docker_plugin-1.6.1/netbox_docker_plugin/templates/netbox_docker_plugin/image.html
--rw-r--r--   0 runner    (1001) docker     (127)     1445 2024-04-22 12:19:56.000000 netbox_docker_plugin-1.6.1/netbox_docker_plugin/templates/netbox_docker_plugin/network.html
--rw-r--r--   0 runner    (1001) docker     (127)     2075 2024-04-22 12:19:56.000000 netbox_docker_plugin-1.6.1/netbox_docker_plugin/templates/netbox_docker_plugin/registry.html
--rw-r--r--   0 runner    (1001) docker     (127)     1182 2024-04-22 12:19:56.000000 netbox_docker_plugin-1.6.1/netbox_docker_plugin/templates/netbox_docker_plugin/volume.html
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 12:19:59.622593 netbox_docker_plugin-1.6.1/netbox_docker_plugin/templatetags/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-22 12:19:56.000000 netbox_docker_plugin-1.6.1/netbox_docker_plugin/templatetags/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      300 2024-04-22 12:19:56.000000 netbox_docker_plugin-1.6.1/netbox_docker_plugin/templatetags/host.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 12:19:59.622593 netbox_docker_plugin-1.6.1/netbox_docker_plugin/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-22 12:19:56.000000 netbox_docker_plugin-1.6.1/netbox_docker_plugin/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      824 2024-04-22 12:19:56.000000 netbox_docker_plugin-1.6.1/netbox_docker_plugin/tests/base.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 12:19:59.622593 netbox_docker_plugin-1.6.1/netbox_docker_plugin/tests/container/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-22 12:19:56.000000 netbox_docker_plugin-1.6.1/netbox_docker_plugin/tests/container/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5074 2024-04-22 12:19:56.000000 netbox_docker_plugin-1.6.1/netbox_docker_plugin/tests/container/test_container_api.py
--rw-r--r--   0 runner    (1001) docker     (127)    11074 2024-04-22 12:19:56.000000 netbox_docker_plugin-1.6.1/netbox_docker_plugin/tests/container/test_container_operation_view.py
--rw-r--r--   0 runner    (1001) docker     (127)     4868 2024-04-22 12:19:56.000000 netbox_docker_plugin-1.6.1/netbox_docker_plugin/tests/container/test_container_validation.py
--rw-r--r--   0 runner    (1001) docker     (127)     2401 2024-04-22 12:19:56.000000 netbox_docker_plugin-1.6.1/netbox_docker_plugin/tests/container/test_container_views.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 12:19:59.626592 netbox_docker_plugin-1.6.1/netbox_docker_plugin/tests/host/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-22 12:19:56.000000 netbox_docker_plugin-1.6.1/netbox_docker_plugin/tests/host/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4443 2024-04-22 12:19:56.000000 netbox_docker_plugin-1.6.1/netbox_docker_plugin/tests/host/test_host_api.py
--rw-r--r--   0 runner    (1001) docker     (127)     2889 2024-04-22 12:19:56.000000 netbox_docker_plugin-1.6.1/netbox_docker_plugin/tests/host/test_host_views.py
--rw-r--r--   0 runner    (1001) docker     (127)      822 2024-04-22 12:19:56.000000 netbox_docker_plugin-1.6.1/netbox_docker_plugin/tests/host/test_replace_password.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 12:19:59.626592 netbox_docker_plugin-1.6.1/netbox_docker_plugin/tests/image/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-22 12:19:56.000000 netbox_docker_plugin-1.6.1/netbox_docker_plugin/tests/image/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2228 2024-04-22 12:19:56.000000 netbox_docker_plugin-1.6.1/netbox_docker_plugin/tests/image/test_image_api.py
--rw-r--r--   0 runner    (1001) docker     (127)     1779 2024-04-22 12:19:56.000000 netbox_docker_plugin-1.6.1/netbox_docker_plugin/tests/image/test_image_views.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 12:19:59.626592 netbox_docker_plugin-1.6.1/netbox_docker_plugin/tests/network/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-22 12:19:56.000000 netbox_docker_plugin-1.6.1/netbox_docker_plugin/tests/network/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1658 2024-04-22 12:19:56.000000 netbox_docker_plugin-1.6.1/netbox_docker_plugin/tests/network/test_network_api.py
--rw-r--r--   0 runner    (1001) docker     (127)     1658 2024-04-22 12:19:56.000000 netbox_docker_plugin-1.6.1/netbox_docker_plugin/tests/network/test_network_views.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 12:19:59.626592 netbox_docker_plugin-1.6.1/netbox_docker_plugin/tests/registry/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-22 12:19:56.000000 netbox_docker_plugin-1.6.1/netbox_docker_plugin/tests/registry/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1885 2024-04-22 12:19:56.000000 netbox_docker_plugin-1.6.1/netbox_docker_plugin/tests/registry/test_registry_api.py
--rw-r--r--   0 runner    (1001) docker     (127)     1436 2024-04-22 12:19:56.000000 netbox_docker_plugin-1.6.1/netbox_docker_plugin/tests/registry/test_registry_views.py
--rw-r--r--   0 runner    (1001) docker     (127)      824 2024-04-22 12:19:56.000000 netbox_docker_plugin-1.6.1/netbox_docker_plugin/tests/test_init.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 12:19:59.626592 netbox_docker_plugin-1.6.1/netbox_docker_plugin/tests/volume/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-22 12:19:56.000000 netbox_docker_plugin-1.6.1/netbox_docker_plugin/tests/volume/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4575 2024-04-22 12:19:56.000000 netbox_docker_plugin-1.6.1/netbox_docker_plugin/tests/volume/test_volume_api.py
--rw-r--r--   0 runner    (1001) docker     (127)     1482 2024-04-22 12:19:56.000000 netbox_docker_plugin-1.6.1/netbox_docker_plugin/tests/volume/test_volume_views.py
--rw-r--r--   0 runner    (1001) docker     (127)    10937 2024-04-22 12:19:56.000000 netbox_docker_plugin-1.6.1/netbox_docker_plugin/urls.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 12:19:59.626592 netbox_docker_plugin-1.6.1/netbox_docker_plugin/utilities/
--rw-r--r--   0 runner    (1001) docker     (127)     7955 2024-04-22 12:19:56.000000 netbox_docker_plugin-1.6.1/netbox_docker_plugin/utilities/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 12:19:59.630593 netbox_docker_plugin-1.6.1/netbox_docker_plugin/views/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-22 12:19:56.000000 netbox_docker_plugin-1.6.1/netbox_docker_plugin/views/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      698 2024-04-22 12:19:56.000000 netbox_docker_plugin-1.6.1/netbox_docker_plugin/views/bind.py
--rw-r--r--   0 runner    (1001) docker     (127)     2495 2024-04-22 12:19:56.000000 netbox_docker_plugin-1.6.1/netbox_docker_plugin/views/container.py
--rw-r--r--   0 runner    (1001) docker     (127)      607 2024-04-22 12:19:56.000000 netbox_docker_plugin-1.6.1/netbox_docker_plugin/views/env.py
--rw-r--r--   0 runner    (1001) docker     (127)     3392 2024-04-22 12:19:56.000000 netbox_docker_plugin-1.6.1/netbox_docker_plugin/views/host.py
--rw-r--r--   0 runner    (1001) docker     (127)     1541 2024-04-22 12:19:56.000000 netbox_docker_plugin-1.6.1/netbox_docker_plugin/views/image.py
--rw-r--r--   0 runner    (1001) docker     (127)      637 2024-04-22 12:19:56.000000 netbox_docker_plugin-1.6.1/netbox_docker_plugin/views/label.py
--rw-r--r--   0 runner    (1001) docker     (127)      725 2024-04-22 12:19:56.000000 netbox_docker_plugin-1.6.1/netbox_docker_plugin/views/mount.py
--rw-r--r--   0 runner    (1001) docker     (127)     1635 2024-04-22 12:19:56.000000 netbox_docker_plugin-1.6.1/netbox_docker_plugin/views/network.py
--rw-r--r--   0 runner    (1001) docker     (127)      880 2024-04-22 12:19:56.000000 netbox_docker_plugin-1.6.1/netbox_docker_plugin/views/network_setting.py
--rw-r--r--   0 runner    (1001) docker     (127)      622 2024-04-22 12:19:56.000000 netbox_docker_plugin-1.6.1/netbox_docker_plugin/views/port.py
--rw-r--r--   0 runner    (1001) docker     (127)     1502 2024-04-22 12:19:56.000000 netbox_docker_plugin-1.6.1/netbox_docker_plugin/views/registry.py
--rw-r--r--   0 runner    (1001) docker     (127)     1325 2024-04-22 12:19:56.000000 netbox_docker_plugin-1.6.1/netbox_docker_plugin/views/volume.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 12:19:59.630593 netbox_docker_plugin-1.6.1/netbox_docker_plugin.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     5117 2024-04-22 12:19:59.000000 netbox_docker_plugin-1.6.1/netbox_docker_plugin.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     5392 2024-04-22 12:19:59.000000 netbox_docker_plugin-1.6.1/netbox_docker_plugin.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-22 12:19:59.000000 netbox_docker_plugin-1.6.1/netbox_docker_plugin.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       21 2024-04-22 12:19:59.000000 netbox_docker_plugin-1.6.1/netbox_docker_plugin.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      695 2024-04-22 12:19:56.000000 netbox_docker_plugin-1.6.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-22 12:19:59.630593 netbox_docker_plugin-1.6.1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 13:08:57.218918 netbox_docker_plugin-1.6.2/
+-rw-r--r--   0 runner    (1001) docker     (127)     1494 2024-04-29 13:08:53.000000 netbox_docker_plugin-1.6.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       56 2024-04-29 13:08:53.000000 netbox_docker_plugin-1.6.2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     5117 2024-04-29 13:08:57.218918 netbox_docker_plugin-1.6.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     4633 2024-04-29 13:08:53.000000 netbox_docker_plugin-1.6.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 13:08:57.202918 netbox_docker_plugin-1.6.2/netbox_docker_plugin/
+-rw-r--r--   0 runner    (1001) docker     (127)      608 2024-04-29 13:08:53.000000 netbox_docker_plugin-1.6.2/netbox_docker_plugin/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 13:08:57.202918 netbox_docker_plugin-1.6.2/netbox_docker_plugin/api/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-29 13:08:53.000000 netbox_docker_plugin-1.6.2/netbox_docker_plugin/api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15347 2024-04-29 13:08:53.000000 netbox_docker_plugin-1.6.2/netbox_docker_plugin/api/serializers.py
+-rw-r--r--   0 runner    (1001) docker     (127)      474 2024-04-29 13:08:53.000000 netbox_docker_plugin-1.6.2/netbox_docker_plugin/api/urls.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3344 2024-04-29 13:08:53.000000 netbox_docker_plugin-1.6.2/netbox_docker_plugin/api/views.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7310 2024-04-29 13:08:53.000000 netbox_docker_plugin-1.6.2/netbox_docker_plugin/filtersets.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 13:08:57.206918 netbox_docker_plugin-1.6.2/netbox_docker_plugin/forms/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-29 13:08:53.000000 netbox_docker_plugin-1.6.2/netbox_docker_plugin/forms/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1158 2024-04-29 13:08:53.000000 netbox_docker_plugin-1.6.2/netbox_docker_plugin/forms/bind.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4199 2024-04-29 13:08:53.000000 netbox_docker_plugin-1.6.2/netbox_docker_plugin/forms/container.py
+-rw-r--r--   0 runner    (1001) docker     (127)      736 2024-04-29 13:08:53.000000 netbox_docker_plugin-1.6.2/netbox_docker_plugin/forms/env.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1958 2024-04-29 13:08:53.000000 netbox_docker_plugin-1.6.2/netbox_docker_plugin/forms/host.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2743 2024-04-29 13:08:53.000000 netbox_docker_plugin-1.6.2/netbox_docker_plugin/forms/image.py
+-rw-r--r--   0 runner    (1001) docker     (127)      728 2024-04-29 13:08:53.000000 netbox_docker_plugin-1.6.2/netbox_docker_plugin/forms/label.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1411 2024-04-29 13:08:53.000000 netbox_docker_plugin-1.6.2/netbox_docker_plugin/forms/mount.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2837 2024-04-29 13:08:53.000000 netbox_docker_plugin-1.6.2/netbox_docker_plugin/forms/network.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1428 2024-04-29 13:08:53.000000 netbox_docker_plugin-1.6.2/netbox_docker_plugin/forms/network_setting.py
+-rw-r--r--   0 runner    (1001) docker     (127)      815 2024-04-29 13:08:53.000000 netbox_docker_plugin-1.6.2/netbox_docker_plugin/forms/port.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1318 2024-04-29 13:08:53.000000 netbox_docker_plugin-1.6.2/netbox_docker_plugin/forms/registry.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1701 2024-04-29 13:08:53.000000 netbox_docker_plugin-1.6.2/netbox_docker_plugin/forms/volume.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 13:08:57.210918 netbox_docker_plugin-1.6.2/netbox_docker_plugin/migrations/
+-rw-r--r--   0 runner    (1001) docker     (127)     1087 2024-04-29 13:08:53.000000 netbox_docker_plugin-1.6.2/netbox_docker_plugin/migrations/0001_initial.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1629 2024-04-29 13:08:53.000000 netbox_docker_plugin-1.6.2/netbox_docker_plugin/migrations/0002_image.py
+-rw-r--r--   0 runner    (1001) docker     (127)      669 2024-04-29 13:08:53.000000 netbox_docker_plugin-1.6.2/netbox_docker_plugin/migrations/0003_image_size.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1292 2024-04-29 13:08:53.000000 netbox_docker_plugin-1.6.2/netbox_docker_plugin/migrations/0004_volume.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1337 2024-04-29 13:08:53.000000 netbox_docker_plugin-1.6.2/netbox_docker_plugin/migrations/0005_network.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9267 2024-04-29 13:08:53.000000 netbox_docker_plugin-1.6.2/netbox_docker_plugin/migrations/0006_container_port_mount_label_env_and_more.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1904 2024-04-29 13:08:53.000000 netbox_docker_plugin-1.6.2/netbox_docker_plugin/migrations/0007_remove_container_netbox_docker_plugin_container_unique_name_host__and_more.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1468 2024-04-29 13:08:53.000000 netbox_docker_plugin-1.6.2/netbox_docker_plugin/migrations/0008_alter_network_unique_together_network_networkid_and_more.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2092 2024-04-29 13:08:53.000000 netbox_docker_plugin-1.6.2/netbox_docker_plugin/migrations/0009_remove_container_network_networksettings_and_more.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1088 2024-04-29 13:08:53.000000 netbox_docker_plugin-1.6.2/netbox_docker_plugin/migrations/0010_container_containerid_and_more.py
+-rw-r--r--   0 runner    (1001) docker     (127)      664 2024-04-29 13:08:53.000000 netbox_docker_plugin-1.6.2/netbox_docker_plugin/migrations/0011_host_token.py
+-rw-r--r--   0 runner    (1001) docker     (127)      541 2024-04-29 13:08:53.000000 netbox_docker_plugin-1.6.2/netbox_docker_plugin/migrations/0012_host_state.py
+-rw-r--r--   0 runner    (1001) docker     (127)      605 2024-04-29 13:08:53.000000 netbox_docker_plugin-1.6.2/netbox_docker_plugin/migrations/0013_host_netbox_url.py
+-rw-r--r--   0 runner    (1001) docker     (127)      441 2024-04-29 13:08:53.000000 netbox_docker_plugin-1.6.2/netbox_docker_plugin/migrations/0014_container_operation.py
+-rw-r--r--   0 runner    (1001) docker     (127)      674 2024-04-29 13:08:53.000000 netbox_docker_plugin-1.6.2/netbox_docker_plugin/migrations/0015_remove_mount_netbox_docker_plugin_mount_unique_volume_and_more.py
+-rw-r--r--   0 runner    (1001) docker     (127)      716 2024-04-29 13:08:53.000000 netbox_docker_plugin-1.6.2/netbox_docker_plugin/migrations/0016_alter_env_value.py
+-rw-r--r--   0 runner    (1001) docker     (127)      437 2024-04-29 13:08:53.000000 netbox_docker_plugin-1.6.2/netbox_docker_plugin/migrations/0017_network_state.py
+-rw-r--r--   0 runner    (1001) docker     (127)      925 2024-04-29 13:08:53.000000 netbox_docker_plugin-1.6.2/netbox_docker_plugin/migrations/0018_alter_mount_volume_alter_networksetting_network.py
+-rw-r--r--   0 runner    (1001) docker     (127)      695 2024-04-29 13:08:53.000000 netbox_docker_plugin-1.6.2/netbox_docker_plugin/migrations/0019_host_agent_version_host_docker_api_version.py
+-rw-r--r--   0 runner    (1001) docker     (127)      771 2024-04-29 13:08:53.000000 netbox_docker_plugin-1.6.2/netbox_docker_plugin/migrations/0020_container_hostname.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3042 2024-04-29 13:08:53.000000 netbox_docker_plugin-1.6.2/netbox_docker_plugin/migrations/0021_registry_and_more.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2410 2024-04-29 13:08:53.000000 netbox_docker_plugin-1.6.2/netbox_docker_plugin/migrations/0022_bind_bind_netbox_docker_plugin_bind_unique_bind.py
+-rw-r--r--   0 runner    (1001) docker     (127)      842 2024-04-29 13:08:53.000000 netbox_docker_plugin-1.6.2/netbox_docker_plugin/migrations/0023_delete_hosts.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1351 2024-04-29 13:08:53.000000 netbox_docker_plugin-1.6.2/netbox_docker_plugin/migrations/0024_registry_host_alter_registry_name_and_more.py
+-rw-r--r--   0 runner    (1001) docker     (127)      747 2024-04-29 13:08:53.000000 netbox_docker_plugin-1.6.2/netbox_docker_plugin/migrations/0025_alter_image_version.py
+-rw-r--r--   0 runner    (1001) docker     (127)      742 2024-04-29 13:08:53.000000 netbox_docker_plugin-1.6.2/netbox_docker_plugin/migrations/0026_image_digest.py
+-rw-r--r--   0 runner    (1001) docker     (127)      438 2024-04-29 13:08:53.000000 netbox_docker_plugin-1.6.2/netbox_docker_plugin/migrations/0027_container_restart_policy.py
+-rw-r--r--   0 runner    (1001) docker     (127)      858 2024-04-29 13:08:53.000000 netbox_docker_plugin-1.6.2/netbox_docker_plugin/migrations/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 13:08:57.210918 netbox_docker_plugin-1.6.2/netbox_docker_plugin/models/
+-rw-r--r--   0 runner    (1001) docker     (127)      194 2024-04-29 13:08:53.000000 netbox_docker_plugin-1.6.2/netbox_docker_plugin/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10657 2024-04-29 13:08:53.000000 netbox_docker_plugin-1.6.2/netbox_docker_plugin/models/container.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2045 2024-04-29 13:08:53.000000 netbox_docker_plugin-1.6.2/netbox_docker_plugin/models/host.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2323 2024-04-29 13:08:53.000000 netbox_docker_plugin-1.6.2/netbox_docker_plugin/models/image.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2369 2024-04-29 13:08:53.000000 netbox_docker_plugin-1.6.2/netbox_docker_plugin/models/network.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1776 2024-04-29 13:08:53.000000 netbox_docker_plugin-1.6.2/netbox_docker_plugin/models/registry.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1307 2024-04-29 13:08:53.000000 netbox_docker_plugin-1.6.2/netbox_docker_plugin/models/volume.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3732 2024-04-29 13:08:53.000000 netbox_docker_plugin-1.6.2/netbox_docker_plugin/navigation.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10276 2024-04-29 13:08:53.000000 netbox_docker_plugin-1.6.2/netbox_docker_plugin/tables.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 13:08:57.198918 netbox_docker_plugin-1.6.2/netbox_docker_plugin/templates/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 13:08:57.210918 netbox_docker_plugin-1.6.2/netbox_docker_plugin/templates/netbox_docker_plugin/
+-rw-r--r--   0 runner    (1001) docker     (127)     7124 2024-04-29 13:08:53.000000 netbox_docker_plugin-1.6.2/netbox_docker_plugin/templates/netbox_docker_plugin/container.html
+-rw-r--r--   0 runner    (1001) docker     (127)     5086 2024-04-29 13:08:53.000000 netbox_docker_plugin-1.6.2/netbox_docker_plugin/templates/netbox_docker_plugin/host.html
+-rw-r--r--   0 runner    (1001) docker     (127)     1808 2024-04-29 13:08:53.000000 netbox_docker_plugin-1.6.2/netbox_docker_plugin/templates/netbox_docker_plugin/image.html
+-rw-r--r--   0 runner    (1001) docker     (127)     1445 2024-04-29 13:08:53.000000 netbox_docker_plugin-1.6.2/netbox_docker_plugin/templates/netbox_docker_plugin/network.html
+-rw-r--r--   0 runner    (1001) docker     (127)     2075 2024-04-29 13:08:53.000000 netbox_docker_plugin-1.6.2/netbox_docker_plugin/templates/netbox_docker_plugin/registry.html
+-rw-r--r--   0 runner    (1001) docker     (127)     1182 2024-04-29 13:08:53.000000 netbox_docker_plugin-1.6.2/netbox_docker_plugin/templates/netbox_docker_plugin/volume.html
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 13:08:57.210918 netbox_docker_plugin-1.6.2/netbox_docker_plugin/templatetags/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-29 13:08:53.000000 netbox_docker_plugin-1.6.2/netbox_docker_plugin/templatetags/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      300 2024-04-29 13:08:53.000000 netbox_docker_plugin-1.6.2/netbox_docker_plugin/templatetags/host.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 13:08:57.214918 netbox_docker_plugin-1.6.2/netbox_docker_plugin/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-29 13:08:53.000000 netbox_docker_plugin-1.6.2/netbox_docker_plugin/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      824 2024-04-29 13:08:53.000000 netbox_docker_plugin-1.6.2/netbox_docker_plugin/tests/base.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 13:08:57.214918 netbox_docker_plugin-1.6.2/netbox_docker_plugin/tests/container/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-29 13:08:53.000000 netbox_docker_plugin-1.6.2/netbox_docker_plugin/tests/container/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5093 2024-04-29 13:08:53.000000 netbox_docker_plugin-1.6.2/netbox_docker_plugin/tests/container/test_container_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11074 2024-04-29 13:08:53.000000 netbox_docker_plugin-1.6.2/netbox_docker_plugin/tests/container/test_container_operation_view.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4868 2024-04-29 13:08:53.000000 netbox_docker_plugin-1.6.2/netbox_docker_plugin/tests/container/test_container_validation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2401 2024-04-29 13:08:53.000000 netbox_docker_plugin-1.6.2/netbox_docker_plugin/tests/container/test_container_views.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 13:08:57.214918 netbox_docker_plugin-1.6.2/netbox_docker_plugin/tests/host/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-29 13:08:53.000000 netbox_docker_plugin-1.6.2/netbox_docker_plugin/tests/host/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4443 2024-04-29 13:08:53.000000 netbox_docker_plugin-1.6.2/netbox_docker_plugin/tests/host/test_host_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2889 2024-04-29 13:08:53.000000 netbox_docker_plugin-1.6.2/netbox_docker_plugin/tests/host/test_host_views.py
+-rw-r--r--   0 runner    (1001) docker     (127)      822 2024-04-29 13:08:53.000000 netbox_docker_plugin-1.6.2/netbox_docker_plugin/tests/host/test_replace_password.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 13:08:57.214918 netbox_docker_plugin-1.6.2/netbox_docker_plugin/tests/image/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-29 13:08:53.000000 netbox_docker_plugin-1.6.2/netbox_docker_plugin/tests/image/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2228 2024-04-29 13:08:53.000000 netbox_docker_plugin-1.6.2/netbox_docker_plugin/tests/image/test_image_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1779 2024-04-29 13:08:53.000000 netbox_docker_plugin-1.6.2/netbox_docker_plugin/tests/image/test_image_views.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 13:08:57.214918 netbox_docker_plugin-1.6.2/netbox_docker_plugin/tests/network/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-29 13:08:53.000000 netbox_docker_plugin-1.6.2/netbox_docker_plugin/tests/network/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1658 2024-04-29 13:08:53.000000 netbox_docker_plugin-1.6.2/netbox_docker_plugin/tests/network/test_network_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1658 2024-04-29 13:08:53.000000 netbox_docker_plugin-1.6.2/netbox_docker_plugin/tests/network/test_network_views.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 13:08:57.214918 netbox_docker_plugin-1.6.2/netbox_docker_plugin/tests/registry/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-29 13:08:53.000000 netbox_docker_plugin-1.6.2/netbox_docker_plugin/tests/registry/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1885 2024-04-29 13:08:53.000000 netbox_docker_plugin-1.6.2/netbox_docker_plugin/tests/registry/test_registry_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1436 2024-04-29 13:08:53.000000 netbox_docker_plugin-1.6.2/netbox_docker_plugin/tests/registry/test_registry_views.py
+-rw-r--r--   0 runner    (1001) docker     (127)      824 2024-04-29 13:08:53.000000 netbox_docker_plugin-1.6.2/netbox_docker_plugin/tests/test_init.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 13:08:57.218918 netbox_docker_plugin-1.6.2/netbox_docker_plugin/tests/volume/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-29 13:08:53.000000 netbox_docker_plugin-1.6.2/netbox_docker_plugin/tests/volume/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4575 2024-04-29 13:08:53.000000 netbox_docker_plugin-1.6.2/netbox_docker_plugin/tests/volume/test_volume_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1482 2024-04-29 13:08:53.000000 netbox_docker_plugin-1.6.2/netbox_docker_plugin/tests/volume/test_volume_views.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10937 2024-04-29 13:08:53.000000 netbox_docker_plugin-1.6.2/netbox_docker_plugin/urls.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 13:08:57.218918 netbox_docker_plugin-1.6.2/netbox_docker_plugin/utilities/
+-rw-r--r--   0 runner    (1001) docker     (127)     7955 2024-04-29 13:08:53.000000 netbox_docker_plugin-1.6.2/netbox_docker_plugin/utilities/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 13:08:57.218918 netbox_docker_plugin-1.6.2/netbox_docker_plugin/views/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-29 13:08:53.000000 netbox_docker_plugin-1.6.2/netbox_docker_plugin/views/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      698 2024-04-29 13:08:53.000000 netbox_docker_plugin-1.6.2/netbox_docker_plugin/views/bind.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2566 2024-04-29 13:08:53.000000 netbox_docker_plugin-1.6.2/netbox_docker_plugin/views/container.py
+-rw-r--r--   0 runner    (1001) docker     (127)      607 2024-04-29 13:08:53.000000 netbox_docker_plugin-1.6.2/netbox_docker_plugin/views/env.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3458 2024-04-29 13:08:53.000000 netbox_docker_plugin-1.6.2/netbox_docker_plugin/views/host.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1608 2024-04-29 13:08:53.000000 netbox_docker_plugin-1.6.2/netbox_docker_plugin/views/image.py
+-rw-r--r--   0 runner    (1001) docker     (127)      637 2024-04-29 13:08:53.000000 netbox_docker_plugin-1.6.2/netbox_docker_plugin/views/label.py
+-rw-r--r--   0 runner    (1001) docker     (127)      725 2024-04-29 13:08:53.000000 netbox_docker_plugin-1.6.2/netbox_docker_plugin/views/mount.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1704 2024-04-29 13:08:53.000000 netbox_docker_plugin-1.6.2/netbox_docker_plugin/views/network.py
+-rw-r--r--   0 runner    (1001) docker     (127)      880 2024-04-29 13:08:53.000000 netbox_docker_plugin-1.6.2/netbox_docker_plugin/views/network_setting.py
+-rw-r--r--   0 runner    (1001) docker     (127)      622 2024-04-29 13:08:53.000000 netbox_docker_plugin-1.6.2/netbox_docker_plugin/views/port.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1502 2024-04-29 13:08:53.000000 netbox_docker_plugin-1.6.2/netbox_docker_plugin/views/registry.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1393 2024-04-29 13:08:53.000000 netbox_docker_plugin-1.6.2/netbox_docker_plugin/views/volume.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 13:08:57.218918 netbox_docker_plugin-1.6.2/netbox_docker_plugin.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     5117 2024-04-29 13:08:57.000000 netbox_docker_plugin-1.6.2/netbox_docker_plugin.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     5392 2024-04-29 13:08:57.000000 netbox_docker_plugin-1.6.2/netbox_docker_plugin.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-29 13:08:57.000000 netbox_docker_plugin-1.6.2/netbox_docker_plugin.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       21 2024-04-29 13:08:57.000000 netbox_docker_plugin-1.6.2/netbox_docker_plugin.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      695 2024-04-29 13:08:53.000000 netbox_docker_plugin-1.6.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-29 13:08:57.218918 netbox_docker_plugin-1.6.2/setup.cfg
```

### Comparing `netbox_docker_plugin-1.6.1/LICENSE` & `netbox_docker_plugin-1.6.2/LICENSE`

 * *Files identical despite different names*

### Comparing `netbox_docker_plugin-1.6.1/PKG-INFO` & `netbox_docker_plugin-1.6.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: netbox-docker-plugin
-Version: 1.6.1
+Version: 1.6.2
 Summary: Manage Docker with Netbox & style.
 Author-email: Vincent Simonin <vincent@saashup.com>
 Project-URL: Homepage, https://github.com/SaaShup/netbox-docker-plugin
 Project-URL: Bug Tracker, https://github.com/SaaShup/netbox-docker-plugin/issues
 Keywords: netbox,netbox-plugin,docker
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.8
```

### Comparing `netbox_docker_plugin-1.6.1/README.md` & `netbox_docker_plugin-1.6.2/README.md`

 * *Files identical despite different names*

### Comparing `netbox_docker_plugin-1.6.1/netbox_docker_plugin/__init__.py` & `netbox_docker_plugin-1.6.2/netbox_docker_plugin/__init__.py`

 * *Files 18% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 
 class NetBoxDockerConfig(PluginConfig):
     """Plugin Config Class"""
 
     name = "netbox_docker_plugin"
     verbose_name = " NetBox Docker Plugin"
     description = "Manage Docker"
-    version = "1.6.1"
+    version = "1.6.2"
     base_url = "docker"
     author= "Vincent Simonin"
     author_email= "vincent@saashup.com"
 
     def ready(self):
         post_migrate.connect(create_webhook)
```

### Comparing `netbox_docker_plugin-1.6.1/netbox_docker_plugin/api/serializers.py` & `netbox_docker_plugin-1.6.2/netbox_docker_plugin/api/serializers.py`

 * *Files 0% similar despite different names*

```diff
@@ -134,14 +134,15 @@
     class Meta:
         """Nested Container Serializer Meta class"""
 
         model = Container
         fields = (
             "id",
             "url",
+            "display",
             "name",
             "ContainerID",
             "state",
             "status",
             "restart_policy",
             "operation",
             "hostname",
@@ -385,14 +386,15 @@
     class Meta:
         """Container Serializer Meta class"""
 
         model = Container
         fields = (
             "id",
             "url",
+            "display",
             "host",
             "image",
             "name",
             "state",
             "operation",
             "status",
             "ContainerID",
```

### Comparing `netbox_docker_plugin-1.6.1/netbox_docker_plugin/api/views.py` & `netbox_docker_plugin-1.6.2/netbox_docker_plugin/api/views.py`

 * *Files identical despite different names*

### Comparing `netbox_docker_plugin-1.6.1/netbox_docker_plugin/filtersets.py` & `netbox_docker_plugin-1.6.2/netbox_docker_plugin/filtersets.py`

 * *Files identical despite different names*

### Comparing `netbox_docker_plugin-1.6.1/netbox_docker_plugin/forms/bind.py` & `netbox_docker_plugin-1.6.2/netbox_docker_plugin/forms/bind.py`

 * *Files identical despite different names*

### Comparing `netbox_docker_plugin-1.6.1/netbox_docker_plugin/forms/container.py` & `netbox_docker_plugin-1.6.2/netbox_docker_plugin/forms/container.py`

 * *Files identical despite different names*

### Comparing `netbox_docker_plugin-1.6.1/netbox_docker_plugin/forms/env.py` & `netbox_docker_plugin-1.6.2/netbox_docker_plugin/forms/env.py`

 * *Files identical despite different names*

### Comparing `netbox_docker_plugin-1.6.1/netbox_docker_plugin/forms/host.py` & `netbox_docker_plugin-1.6.2/netbox_docker_plugin/forms/host.py`

 * *Files identical despite different names*

### Comparing `netbox_docker_plugin-1.6.1/netbox_docker_plugin/forms/image.py` & `netbox_docker_plugin-1.6.2/netbox_docker_plugin/forms/image.py`

 * *Files identical despite different names*

### Comparing `netbox_docker_plugin-1.6.1/netbox_docker_plugin/forms/label.py` & `netbox_docker_plugin-1.6.2/netbox_docker_plugin/forms/label.py`

 * *Files identical despite different names*

### Comparing `netbox_docker_plugin-1.6.1/netbox_docker_plugin/forms/mount.py` & `netbox_docker_plugin-1.6.2/netbox_docker_plugin/forms/mount.py`

 * *Files identical despite different names*

### Comparing `netbox_docker_plugin-1.6.1/netbox_docker_plugin/forms/network.py` & `netbox_docker_plugin-1.6.2/netbox_docker_plugin/forms/network.py`

 * *Files identical despite different names*

### Comparing `netbox_docker_plugin-1.6.1/netbox_docker_plugin/forms/network_setting.py` & `netbox_docker_plugin-1.6.2/netbox_docker_plugin/forms/network_setting.py`

 * *Files identical despite different names*

### Comparing `netbox_docker_plugin-1.6.1/netbox_docker_plugin/forms/port.py` & `netbox_docker_plugin-1.6.2/netbox_docker_plugin/forms/port.py`

 * *Files identical despite different names*

### Comparing `netbox_docker_plugin-1.6.1/netbox_docker_plugin/forms/registry.py` & `netbox_docker_plugin-1.6.2/netbox_docker_plugin/forms/registry.py`

 * *Files identical despite different names*

### Comparing `netbox_docker_plugin-1.6.1/netbox_docker_plugin/forms/volume.py` & `netbox_docker_plugin-1.6.2/netbox_docker_plugin/forms/volume.py`

 * *Files identical despite different names*

### Comparing `netbox_docker_plugin-1.6.1/netbox_docker_plugin/migrations/0001_initial.py` & `netbox_docker_plugin-1.6.2/netbox_docker_plugin/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `netbox_docker_plugin-1.6.1/netbox_docker_plugin/migrations/0002_image.py` & `netbox_docker_plugin-1.6.2/netbox_docker_plugin/migrations/0002_image.py`

 * *Files identical despite different names*

### Comparing `netbox_docker_plugin-1.6.1/netbox_docker_plugin/migrations/0003_image_size.py` & `netbox_docker_plugin-1.6.2/netbox_docker_plugin/migrations/0003_image_size.py`

 * *Files identical despite different names*

### Comparing `netbox_docker_plugin-1.6.1/netbox_docker_plugin/migrations/0004_volume.py` & `netbox_docker_plugin-1.6.2/netbox_docker_plugin/migrations/0004_volume.py`

 * *Files identical despite different names*

### Comparing `netbox_docker_plugin-1.6.1/netbox_docker_plugin/migrations/0005_network.py` & `netbox_docker_plugin-1.6.2/netbox_docker_plugin/migrations/0005_network.py`

 * *Files identical despite different names*

### Comparing `netbox_docker_plugin-1.6.1/netbox_docker_plugin/migrations/0006_container_port_mount_label_env_and_more.py` & `netbox_docker_plugin-1.6.2/netbox_docker_plugin/migrations/0006_container_port_mount_label_env_and_more.py`

 * *Files identical despite different names*

### Comparing `netbox_docker_plugin-1.6.1/netbox_docker_plugin/migrations/0007_remove_container_netbox_docker_plugin_container_unique_name_host__and_more.py` & `netbox_docker_plugin-1.6.2/netbox_docker_plugin/migrations/0007_remove_container_netbox_docker_plugin_container_unique_name_host__and_more.py`

 * *Files identical despite different names*

### Comparing `netbox_docker_plugin-1.6.1/netbox_docker_plugin/migrations/0008_alter_network_unique_together_network_networkid_and_more.py` & `netbox_docker_plugin-1.6.2/netbox_docker_plugin/migrations/0008_alter_network_unique_together_network_networkid_and_more.py`

 * *Files identical despite different names*

### Comparing `netbox_docker_plugin-1.6.1/netbox_docker_plugin/migrations/0009_remove_container_network_networksettings_and_more.py` & `netbox_docker_plugin-1.6.2/netbox_docker_plugin/migrations/0009_remove_container_network_networksettings_and_more.py`

 * *Files identical despite different names*

### Comparing `netbox_docker_plugin-1.6.1/netbox_docker_plugin/migrations/0010_container_containerid_and_more.py` & `netbox_docker_plugin-1.6.2/netbox_docker_plugin/migrations/0010_container_containerid_and_more.py`

 * *Files identical despite different names*

### Comparing `netbox_docker_plugin-1.6.1/netbox_docker_plugin/migrations/0011_host_token.py` & `netbox_docker_plugin-1.6.2/netbox_docker_plugin/migrations/0011_host_token.py`

 * *Files identical despite different names*

### Comparing `netbox_docker_plugin-1.6.1/netbox_docker_plugin/migrations/0012_host_state.py` & `netbox_docker_plugin-1.6.2/netbox_docker_plugin/migrations/0012_host_state.py`

 * *Files identical despite different names*

### Comparing `netbox_docker_plugin-1.6.1/netbox_docker_plugin/migrations/0013_host_netbox_url.py` & `netbox_docker_plugin-1.6.2/netbox_docker_plugin/migrations/0013_host_netbox_url.py`

 * *Files identical despite different names*

### Comparing `netbox_docker_plugin-1.6.1/netbox_docker_plugin/migrations/0015_remove_mount_netbox_docker_plugin_mount_unique_volume_and_more.py` & `netbox_docker_plugin-1.6.2/netbox_docker_plugin/migrations/0015_remove_mount_netbox_docker_plugin_mount_unique_volume_and_more.py`

 * *Files identical despite different names*

### Comparing `netbox_docker_plugin-1.6.1/netbox_docker_plugin/migrations/0016_alter_env_value.py` & `netbox_docker_plugin-1.6.2/netbox_docker_plugin/migrations/0016_alter_env_value.py`

 * *Files identical despite different names*

### Comparing `netbox_docker_plugin-1.6.1/netbox_docker_plugin/migrations/0018_alter_mount_volume_alter_networksetting_network.py` & `netbox_docker_plugin-1.6.2/netbox_docker_plugin/migrations/0018_alter_mount_volume_alter_networksetting_network.py`

 * *Files identical despite different names*

### Comparing `netbox_docker_plugin-1.6.1/netbox_docker_plugin/migrations/0019_host_agent_version_host_docker_api_version.py` & `netbox_docker_plugin-1.6.2/netbox_docker_plugin/migrations/0019_host_agent_version_host_docker_api_version.py`

 * *Files identical despite different names*

### Comparing `netbox_docker_plugin-1.6.1/netbox_docker_plugin/migrations/0020_container_hostname.py` & `netbox_docker_plugin-1.6.2/netbox_docker_plugin/migrations/0020_container_hostname.py`

 * *Files identical despite different names*

### Comparing `netbox_docker_plugin-1.6.1/netbox_docker_plugin/migrations/0021_registry_and_more.py` & `netbox_docker_plugin-1.6.2/netbox_docker_plugin/migrations/0021_registry_and_more.py`

 * *Files identical despite different names*

### Comparing `netbox_docker_plugin-1.6.1/netbox_docker_plugin/migrations/0022_bind_bind_netbox_docker_plugin_bind_unique_bind.py` & `netbox_docker_plugin-1.6.2/netbox_docker_plugin/migrations/0022_bind_bind_netbox_docker_plugin_bind_unique_bind.py`

 * *Files identical despite different names*

### Comparing `netbox_docker_plugin-1.6.1/netbox_docker_plugin/migrations/0023_delete_hosts.py` & `netbox_docker_plugin-1.6.2/netbox_docker_plugin/migrations/0023_delete_hosts.py`

 * *Files identical despite different names*

### Comparing `netbox_docker_plugin-1.6.1/netbox_docker_plugin/migrations/0024_registry_host_alter_registry_name_and_more.py` & `netbox_docker_plugin-1.6.2/netbox_docker_plugin/migrations/0024_registry_host_alter_registry_name_and_more.py`

 * *Files identical despite different names*

### Comparing `netbox_docker_plugin-1.6.1/netbox_docker_plugin/migrations/0025_alter_image_version.py` & `netbox_docker_plugin-1.6.2/netbox_docker_plugin/migrations/0025_alter_image_version.py`

 * *Files identical despite different names*

### Comparing `netbox_docker_plugin-1.6.1/netbox_docker_plugin/migrations/0026_image_digest.py` & `netbox_docker_plugin-1.6.2/netbox_docker_plugin/migrations/0026_image_digest.py`

 * *Files identical despite different names*

### Comparing `netbox_docker_plugin-1.6.1/netbox_docker_plugin/migrations/__init__.py` & `netbox_docker_plugin-1.6.2/netbox_docker_plugin/migrations/__init__.py`

 * *Files identical despite different names*

### Comparing `netbox_docker_plugin-1.6.1/netbox_docker_plugin/models/container.py` & `netbox_docker_plugin-1.6.2/netbox_docker_plugin/models/container.py`

 * *Files identical despite different names*

### Comparing `netbox_docker_plugin-1.6.1/netbox_docker_plugin/models/host.py` & `netbox_docker_plugin-1.6.2/netbox_docker_plugin/models/host.py`

 * *Files identical despite different names*

### Comparing `netbox_docker_plugin-1.6.1/netbox_docker_plugin/models/image.py` & `netbox_docker_plugin-1.6.2/netbox_docker_plugin/models/image.py`

 * *Files identical despite different names*

### Comparing `netbox_docker_plugin-1.6.1/netbox_docker_plugin/models/network.py` & `netbox_docker_plugin-1.6.2/netbox_docker_plugin/models/network.py`

 * *Files identical despite different names*

### Comparing `netbox_docker_plugin-1.6.1/netbox_docker_plugin/models/registry.py` & `netbox_docker_plugin-1.6.2/netbox_docker_plugin/models/registry.py`

 * *Files identical despite different names*

### Comparing `netbox_docker_plugin-1.6.1/netbox_docker_plugin/models/volume.py` & `netbox_docker_plugin-1.6.2/netbox_docker_plugin/models/volume.py`

 * *Files identical despite different names*

### Comparing `netbox_docker_plugin-1.6.1/netbox_docker_plugin/navigation.py` & `netbox_docker_plugin-1.6.2/netbox_docker_plugin/navigation.py`

 * *Files identical despite different names*

### Comparing `netbox_docker_plugin-1.6.1/netbox_docker_plugin/tables.py` & `netbox_docker_plugin-1.6.2/netbox_docker_plugin/tables.py`

 * *Files identical despite different names*

### Comparing `netbox_docker_plugin-1.6.1/netbox_docker_plugin/templates/netbox_docker_plugin/container.html` & `netbox_docker_plugin-1.6.2/netbox_docker_plugin/templates/netbox_docker_plugin/container.html`

 * *Files identical despite different names*

### Comparing `netbox_docker_plugin-1.6.1/netbox_docker_plugin/templates/netbox_docker_plugin/host.html` & `netbox_docker_plugin-1.6.2/netbox_docker_plugin/templates/netbox_docker_plugin/host.html`

 * *Files identical despite different names*

### Comparing `netbox_docker_plugin-1.6.1/netbox_docker_plugin/templates/netbox_docker_plugin/image.html` & `netbox_docker_plugin-1.6.2/netbox_docker_plugin/templates/netbox_docker_plugin/image.html`

 * *Files identical despite different names*

### Comparing `netbox_docker_plugin-1.6.1/netbox_docker_plugin/templates/netbox_docker_plugin/network.html` & `netbox_docker_plugin-1.6.2/netbox_docker_plugin/templates/netbox_docker_plugin/network.html`

 * *Files identical despite different names*

### Comparing `netbox_docker_plugin-1.6.1/netbox_docker_plugin/templates/netbox_docker_plugin/registry.html` & `netbox_docker_plugin-1.6.2/netbox_docker_plugin/templates/netbox_docker_plugin/registry.html`

 * *Files identical despite different names*

### Comparing `netbox_docker_plugin-1.6.1/netbox_docker_plugin/templates/netbox_docker_plugin/volume.html` & `netbox_docker_plugin-1.6.2/netbox_docker_plugin/templates/netbox_docker_plugin/volume.html`

 * *Files identical despite different names*

### Comparing `netbox_docker_plugin-1.6.1/netbox_docker_plugin/tests/base.py` & `netbox_docker_plugin-1.6.2/netbox_docker_plugin/tests/base.py`

 * *Files identical despite different names*

### Comparing `netbox_docker_plugin-1.6.1/netbox_docker_plugin/tests/container/test_container_api.py` & `netbox_docker_plugin-1.6.2/netbox_docker_plugin/tests/container/test_container_api.py`

 * *Files 1% similar despite different names*

```diff
@@ -19,14 +19,15 @@
     APIViewTestCases.DeleteObjectViewTestCase,
 ):
     """Container Test Case Class"""
 
     model = Container
     brief_fields = [
         "ContainerID",
+        "display",
         "hostname",
         "id",
         "name",
         "operation",
         "restart_policy",
         "state",
         "status",
```

### Comparing `netbox_docker_plugin-1.6.1/netbox_docker_plugin/tests/container/test_container_operation_view.py` & `netbox_docker_plugin-1.6.2/netbox_docker_plugin/tests/container/test_container_operation_view.py`

 * *Files identical despite different names*

### Comparing `netbox_docker_plugin-1.6.1/netbox_docker_plugin/tests/container/test_container_validation.py` & `netbox_docker_plugin-1.6.2/netbox_docker_plugin/tests/container/test_container_validation.py`

 * *Files identical despite different names*

### Comparing `netbox_docker_plugin-1.6.1/netbox_docker_plugin/tests/container/test_container_views.py` & `netbox_docker_plugin-1.6.2/netbox_docker_plugin/tests/container/test_container_views.py`

 * *Files identical despite different names*

### Comparing `netbox_docker_plugin-1.6.1/netbox_docker_plugin/tests/host/test_host_api.py` & `netbox_docker_plugin-1.6.2/netbox_docker_plugin/tests/host/test_host_api.py`

 * *Files identical despite different names*

### Comparing `netbox_docker_plugin-1.6.1/netbox_docker_plugin/tests/host/test_host_views.py` & `netbox_docker_plugin-1.6.2/netbox_docker_plugin/tests/host/test_host_views.py`

 * *Files identical despite different names*

### Comparing `netbox_docker_plugin-1.6.1/netbox_docker_plugin/tests/host/test_replace_password.py` & `netbox_docker_plugin-1.6.2/netbox_docker_plugin/tests/host/test_replace_password.py`

 * *Files identical despite different names*

### Comparing `netbox_docker_plugin-1.6.1/netbox_docker_plugin/tests/image/test_image_api.py` & `netbox_docker_plugin-1.6.2/netbox_docker_plugin/tests/image/test_image_api.py`

 * *Files identical despite different names*

### Comparing `netbox_docker_plugin-1.6.1/netbox_docker_plugin/tests/image/test_image_views.py` & `netbox_docker_plugin-1.6.2/netbox_docker_plugin/tests/image/test_image_views.py`

 * *Files identical despite different names*

### Comparing `netbox_docker_plugin-1.6.1/netbox_docker_plugin/tests/network/test_network_api.py` & `netbox_docker_plugin-1.6.2/netbox_docker_plugin/tests/network/test_network_api.py`

 * *Files identical despite different names*

### Comparing `netbox_docker_plugin-1.6.1/netbox_docker_plugin/tests/network/test_network_views.py` & `netbox_docker_plugin-1.6.2/netbox_docker_plugin/tests/network/test_network_views.py`

 * *Files identical despite different names*

### Comparing `netbox_docker_plugin-1.6.1/netbox_docker_plugin/tests/registry/test_registry_api.py` & `netbox_docker_plugin-1.6.2/netbox_docker_plugin/tests/registry/test_registry_api.py`

 * *Files identical despite different names*

### Comparing `netbox_docker_plugin-1.6.1/netbox_docker_plugin/tests/registry/test_registry_views.py` & `netbox_docker_plugin-1.6.2/netbox_docker_plugin/tests/registry/test_registry_views.py`

 * *Files identical despite different names*

### Comparing `netbox_docker_plugin-1.6.1/netbox_docker_plugin/tests/test_init.py` & `netbox_docker_plugin-1.6.2/netbox_docker_plugin/tests/test_init.py`

 * *Files identical despite different names*

### Comparing `netbox_docker_plugin-1.6.1/netbox_docker_plugin/tests/volume/test_volume_api.py` & `netbox_docker_plugin-1.6.2/netbox_docker_plugin/tests/volume/test_volume_api.py`

 * *Files identical despite different names*

### Comparing `netbox_docker_plugin-1.6.1/netbox_docker_plugin/tests/volume/test_volume_views.py` & `netbox_docker_plugin-1.6.2/netbox_docker_plugin/tests/volume/test_volume_views.py`

 * *Files identical despite different names*

### Comparing `netbox_docker_plugin-1.6.1/netbox_docker_plugin/urls.py` & `netbox_docker_plugin-1.6.2/netbox_docker_plugin/urls.py`

 * *Files identical despite different names*

### Comparing `netbox_docker_plugin-1.6.1/netbox_docker_plugin/utilities/__init__.py` & `netbox_docker_plugin-1.6.2/netbox_docker_plugin/utilities/__init__.py`

 * *Files identical despite different names*

### Comparing `netbox_docker_plugin-1.6.1/netbox_docker_plugin/views/bind.py` & `netbox_docker_plugin-1.6.2/netbox_docker_plugin/views/bind.py`

 * *Files identical despite different names*

### Comparing `netbox_docker_plugin-1.6.1/netbox_docker_plugin/views/container.py` & `netbox_docker_plugin-1.6.2/netbox_docker_plugin/views/container.py`

 * *Files 2% similar despite different names*

```diff
@@ -77,14 +77,15 @@
     filterset = filtersets.ContainerFilterSet
     table = tables.ContainerTable
 
 
 class ContainerDeleteView(generic.ObjectDeleteView):
     """Container delete view definition"""
 
+    default_return_url = "plugins:netbox_docker_plugin:container_list"
     queryset = Container.objects.all()
 
 
 class ContainerOperationView(generic.ObjectEditView):
     """Container operation view definition"""
 
     def get_object(self, **kwargs):
```

### Comparing `netbox_docker_plugin-1.6.1/netbox_docker_plugin/views/env.py` & `netbox_docker_plugin-1.6.2/netbox_docker_plugin/views/env.py`

 * *Files identical despite different names*

### Comparing `netbox_docker_plugin-1.6.1/netbox_docker_plugin/views/host.py` & `netbox_docker_plugin-1.6.2/netbox_docker_plugin/views/host.py`

 * *Files 18% similar despite different names*

```diff
@@ -105,14 +105,15 @@
 
         return super().save_object(object_form, request)
 
 
 class HostDeleteView(generic.ObjectDeleteView):
     """Host delete view definition"""
 
+    default_return_url = "plugins:netbox_docker_plugin:host_list"
     queryset = Host.objects.all()
 
 
 class HostBulkDeleteView(generic.BulkDeleteView):
     """Host bulk delete view definition"""
 
     queryset = Host.objects.all()
```

### Comparing `netbox_docker_plugin-1.6.1/netbox_docker_plugin/views/image.py` & `netbox_docker_plugin-1.6.2/netbox_docker_plugin/views/image.py`

 * *Files 3% similar despite different names*

```diff
@@ -47,14 +47,15 @@
     queryset = Image.objects.all()
     model_form = image.ImageImportForm
 
 
 class ImageDeleteView(generic.ObjectDeleteView):
     """Image delete view definition"""
 
+    default_return_url = "plugins:netbox_docker_plugin:image_list"
     queryset = Image.objects.all()
 
 
 class ImageBulkDeleteView(generic.BulkDeleteView):
     """Image bulk delete view definition"""
 
     queryset = Image.objects.all()
```

### Comparing `netbox_docker_plugin-1.6.1/netbox_docker_plugin/views/label.py` & `netbox_docker_plugin-1.6.2/netbox_docker_plugin/views/label.py`

 * *Files identical despite different names*

### Comparing `netbox_docker_plugin-1.6.1/netbox_docker_plugin/views/mount.py` & `netbox_docker_plugin-1.6.2/netbox_docker_plugin/views/mount.py`

 * *Files identical despite different names*

### Comparing `netbox_docker_plugin-1.6.1/netbox_docker_plugin/views/network.py` & `netbox_docker_plugin-1.6.2/netbox_docker_plugin/views/network.py`

 * *Files 6% similar despite different names*

```diff
@@ -46,14 +46,15 @@
     queryset = Network.objects.all()
     model_form = network.NetworkImportForm
 
 
 class NetworkDeleteView(generic.ObjectDeleteView):
     """Network delete view definition"""
 
+    default_return_url = "plugins:netbox_docker_plugin:network_list"
     queryset = Network.objects.all()
 
 
 class NetworkBulkDeleteView(generic.BulkDeleteView):
     """Network bulk delete view definition"""
 
     queryset = Network.objects.all()
```

### Comparing `netbox_docker_plugin-1.6.1/netbox_docker_plugin/views/network_setting.py` & `netbox_docker_plugin-1.6.2/netbox_docker_plugin/views/network_setting.py`

 * *Files identical despite different names*

### Comparing `netbox_docker_plugin-1.6.1/netbox_docker_plugin/views/port.py` & `netbox_docker_plugin-1.6.2/netbox_docker_plugin/views/port.py`

 * *Files identical despite different names*

### Comparing `netbox_docker_plugin-1.6.1/netbox_docker_plugin/views/registry.py` & `netbox_docker_plugin-1.6.2/netbox_docker_plugin/views/registry.py`

 * *Files identical despite different names*

### Comparing `netbox_docker_plugin-1.6.1/netbox_docker_plugin/views/volume.py` & `netbox_docker_plugin-1.6.2/netbox_docker_plugin/views/volume.py`

 * *Files 10% similar despite different names*

```diff
@@ -46,8 +46,9 @@
     filterset = filtersets.VolumeFilterSet
     table = tables.VolumeTable
 
 
 class VolumeDeleteView(generic.ObjectDeleteView):
     """Volume delete view definition"""
 
+    default_return_url = "plugins:netbox_docker_plugin:volume_list"
     queryset = Volume.objects.all()
```

### Comparing `netbox_docker_plugin-1.6.1/netbox_docker_plugin.egg-info/PKG-INFO` & `netbox_docker_plugin-1.6.2/netbox_docker_plugin.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: netbox-docker-plugin
-Version: 1.6.1
+Version: 1.6.2
 Summary: Manage Docker with Netbox & style.
 Author-email: Vincent Simonin <vincent@saashup.com>
 Project-URL: Homepage, https://github.com/SaaShup/netbox-docker-plugin
 Project-URL: Bug Tracker, https://github.com/SaaShup/netbox-docker-plugin/issues
 Keywords: netbox,netbox-plugin,docker
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.8
```

### Comparing `netbox_docker_plugin-1.6.1/netbox_docker_plugin.egg-info/SOURCES.txt` & `netbox_docker_plugin-1.6.2/netbox_docker_plugin.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `netbox_docker_plugin-1.6.1/pyproject.toml` & `netbox_docker_plugin-1.6.2/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=68.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "netbox-docker-plugin"
-version = "1.6.1"
+version = "1.6.2"
 authors = [
   { name="Vincent Simonin", email="vincent@saashup.com" },
 ]
 description = "Manage Docker with Netbox & style."
 readme = "README.md"
 requires-python = ">=3.8"
 classifiers = [
```

