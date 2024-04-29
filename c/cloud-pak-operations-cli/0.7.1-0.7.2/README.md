# Comparing `tmp/cloud-pak-operations-cli-0.7.1.tar.gz` & `tmp/cloud_pak_operations_cli-0.7.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cloud-pak-operations-cli-0.7.1.tar", last modified: Wed Mar 20 13:56:31 2024, max compression
+gzip compressed data, was "cloud_pak_operations_cli-0.7.2.tar", last modified: Mon Apr 29 08:16:33 2024, max compression
```

## Comparing `cloud-pak-operations-cli-0.7.1.tar` & `cloud_pak_operations_cli-0.7.2.tar`

### file list

```diff
@@ -1,203 +1,205 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-20 13:56:31.437304 cloud-pak-operations-cli-0.7.1/
--rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-03-20 13:56:26.000000 cloud-pak-operations-cli-0.7.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       29 2024-03-20 13:56:26.000000 cloud-pak-operations-cli-0.7.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     2497 2024-03-20 13:56:31.437304 cloud-pak-operations-cli-0.7.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1346 2024-03-20 13:56:26.000000 cloud-pak-operations-cli-0.7.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-20 13:56:31.437304 cloud-pak-operations-cli-0.7.1/cloud_pak_operations_cli.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2497 2024-03-20 13:56:31.000000 cloud-pak-operations-cli-0.7.1/cloud_pak_operations_cli.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     6356 2024-03-20 13:56:31.000000 cloud-pak-operations-cli-0.7.1/cloud_pak_operations_cli.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-20 13:56:31.000000 cloud-pak-operations-cli-0.7.1/cloud_pak_operations_cli.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      132 2024-03-20 13:56:31.000000 cloud-pak-operations-cli-0.7.1/cloud_pak_operations_cli.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      208 2024-03-20 13:56:31.000000 cloud-pak-operations-cli-0.7.1/cloud_pak_operations_cli.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        4 2024-03-20 13:56:31.000000 cloud-pak-operations-cli-0.7.1/cloud_pak_operations_cli.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-20 13:56:31.413303 cloud-pak-operations-cli-0.7.1/cpo/
--rw-r--r--   0 runner    (1001) docker     (127)      945 2024-03-20 13:56:26.000000 cloud-pak-operations-cli-0.7.1/cpo/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-20 13:56:31.413303 cloud-pak-operations-cli-0.7.1/cpo/commands/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-20 13:56:26.000000 cloud-pak-operations-cli-0.7.1/cpo/commands/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-20 13:56:31.413303 cloud-pak-operations-cli-0.7.1/cpo/commands/adm/
--rw-r--r--   0 runner    (1001) docker     (127)      632 2024-03-20 13:56:26.000000 cloud-pak-operations-cli-0.7.1/cpo/commands/adm/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-20 13:56:31.413303 cloud-pak-operations-cli-0.7.1/cpo/commands/adm/config/
--rw-r--r--   0 runner    (1001) docker     (127)      627 2024-03-20 13:56:26.000000 cloud-pak-operations-cli-0.7.1/cpo/commands/adm/config/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      981 2024-03-20 13:56:26.000000 cloud-pak-operations-cli-0.7.1/cpo/commands/adm/config/set.py
--rw-r--r--   0 runner    (1001) docker     (127)      879 2024-03-20 13:56:26.000000 cloud-pak-operations-cli-0.7.1/cpo/commands/adm/download_dependencies.py
--rw-r--r--   0 runner    (1001) docker     (127)     1123 2024-03-20 13:56:26.000000 cloud-pak-operations-cli-0.7.1/cpo/commands/adm/get-shell-completion-script-location.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-20 13:56:31.417303 cloud-pak-operations-cli-0.7.1/cpo/commands/adm/ibm_internal_plugin/
--rw-r--r--   0 runner    (1001) docker     (127)      647 2024-03-20 13:56:26.000000 cloud-pak-operations-cli-0.7.1/cpo/commands/adm/ibm_internal_plugin/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3726 2024-03-20 13:56:26.000000 cloud-pak-operations-cli-0.7.1/cpo/commands/adm/ibm_internal_plugin/install.py
--rw-r--r--   0 runner    (1001) docker     (127)     1838 2024-03-20 13:56:26.000000 cloud-pak-operations-cli-0.7.1/cpo/commands/adm/ibm_internal_plugin/ls.py
--rw-r--r--   0 runner    (1001) docker     (127)     2906 2024-03-20 13:56:26.000000 cloud-pak-operations-cli-0.7.1/cpo/commands/adm/ibm_internal_plugin/upgrade_plugins.py
--rw-r--r--   0 runner    (1001) docker     (127)     1389 2024-03-20 13:56:26.000000 cloud-pak-operations-cli-0.7.1/cpo/commands/adm/store_credentials.py
--rw-r--r--   0 runner    (1001) docker     (127)     1577 2024-03-20 13:56:26.000000 cloud-pak-operations-cli-0.7.1/cpo/commands/adm/update_dev.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-20 13:56:31.417303 cloud-pak-operations-cli-0.7.1/cpo/commands/cluster/
--rw-r--r--   0 runner    (1001) docker     (127)      632 2024-03-20 13:56:26.000000 cloud-pak-operations-cli-0.7.1/cpo/commands/cluster/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1845 2024-03-20 13:56:26.000000 cloud-pak-operations-cli-0.7.1/cpo/commands/cluster/add.py
--rw-r--r--   0 runner    (1001) docker     (127)     1374 2024-03-20 13:56:26.000000 cloud-pak-operations-cli-0.7.1/cpo/commands/cluster/current.py
--rw-r--r--   0 runner    (1001) docker     (127)     1626 2024-03-20 13:56:26.000000 cloud-pak-operations-cli-0.7.1/cpo/commands/cluster/delete_terminated_pods.py
--rw-r--r--   0 runner    (1001) docker     (127)     1843 2024-03-20 13:56:26.000000 cloud-pak-operations-cli-0.7.1/cpo/commands/cluster/edit.py
--rw-r--r--   0 runner    (1001) docker     (127)     1775 2024-03-20 13:56:26.000000 cloud-pak-operations-cli-0.7.1/cpo/commands/cluster/get_cluster_access_token.py
--rw-r--r--   0 runner    (1001) docker     (127)     2030 2024-03-20 13:56:26.000000 cloud-pak-operations-cli-0.7.1/cpo/commands/cluster/install_nfs_storage_class.py
--rw-r--r--   0 runner    (1001) docker     (127)     1929 2024-03-20 13:56:26.000000 cloud-pak-operations-cli-0.7.1/cpo/commands/cluster/install_odf_storage_classes.py
--rw-r--r--   0 runner    (1001) docker     (127)     1286 2024-03-20 13:56:26.000000 cloud-pak-operations-cli-0.7.1/cpo/commands/cluster/login.py
--rw-r--r--   0 runner    (1001) docker     (127)      883 2024-03-20 13:56:26.000000 cloud-pak-operations-cli-0.7.1/cpo/commands/cluster/ls.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-20 13:56:31.417303 cloud-pak-operations-cli-0.7.1/cpo/commands/cluster/pull_secret/
--rw-r--r--   0 runner    (1001) docker     (127)      643 2024-03-20 13:56:26.000000 cloud-pak-operations-cli-0.7.1/cpo/commands/cluster/pull_secret/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1535 2024-03-20 13:56:26.000000 cloud-pak-operations-cli-0.7.1/cpo/commands/cluster/pull_secret/ls.py
--rw-r--r--   0 runner    (1001) docker     (127)     1513 2024-03-20 13:56:26.000000 cloud-pak-operations-cli-0.7.1/cpo/commands/cluster/pull_secret/rm.py
--rw-r--r--   0 runner    (1001) docker     (127)     1832 2024-03-20 13:56:26.000000 cloud-pak-operations-cli-0.7.1/cpo/commands/cluster/pull_secret/set.py
--rw-r--r--   0 runner    (1001) docker     (127)      885 2024-03-20 13:56:26.000000 cloud-pak-operations-cli-0.7.1/cpo/commands/cluster/reset_current_cluster.py
--rw-r--r--   0 runner    (1001) docker     (127)      939 2024-03-20 13:56:26.000000 cloud-pak-operations-cli-0.7.1/cpo/commands/cluster/rm.py
--rw-r--r--   0 runner    (1001) docker     (127)     1124 2024-03-20 13:56:26.000000 cloud-pak-operations-cli-0.7.1/cpo/commands/cluster/use.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-20 13:56:31.417303 cloud-pak-operations-cli-0.7.1/cpo/commands/ibmcloud/
--rw-r--r--   0 runner    (1001) docker     (127)      632 2024-03-20 13:56:26.000000 cloud-pak-operations-cli-0.7.1/cpo/commands/ibmcloud/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      809 2024-03-20 13:56:26.000000 cloud-pak-operations-cli-0.7.1/cpo/commands/ibmcloud/login.py
--rw-r--r--   0 runner    (1001) docker     (127)     1211 2024-03-20 13:56:26.000000 cloud-pak-operations-cli-0.7.1/cpo/commands/ibmcloud/logout.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-20 13:56:31.417303 cloud-pak-operations-cli-0.7.1/cpo/commands/ibmcloud/oc/
--rw-r--r--   0 runner    (1001) docker     (127)      636 2024-03-20 13:56:26.000000 cloud-pak-operations-cli-0.7.1/cpo/commands/ibmcloud/oc/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-20 13:56:31.421304 cloud-pak-operations-cli-0.7.1/cpo/commands/ibmcloud/oc/cluster/
--rw-r--r--   0 runner    (1001) docker     (127)      646 2024-03-20 13:56:26.000000 cloud-pak-operations-cli-0.7.1/cpo/commands/ibmcloud/oc/cluster/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1552 2024-03-20 13:56:26.000000 cloud-pak-operations-cli-0.7.1/cpo/commands/ibmcloud/oc/cluster/add.py
--rw-r--r--   0 runner    (1001) docker     (127)     1370 2024-03-20 13:56:26.000000 cloud-pak-operations-cli-0.7.1/cpo/commands/ibmcloud/oc/cluster/login.py
--rw-r--r--   0 runner    (1001) docker     (127)      943 2024-03-20 13:56:26.000000 cloud-pak-operations-cli-0.7.1/cpo/commands/ibmcloud/oc/cluster/ls.py
--rw-r--r--   0 runner    (1001) docker     (127)     1195 2024-03-20 13:56:26.000000 cloud-pak-operations-cli-0.7.1/cpo/commands/ibmcloud/oc/cluster/rm.py
--rw-r--r--   0 runner    (1001) docker     (127)     1202 2024-03-20 13:56:26.000000 cloud-pak-operations-cli-0.7.1/cpo/commands/ibmcloud/oc/cluster/status.py
--rw-r--r--   0 runner    (1001) docker     (127)      920 2024-03-20 13:56:26.000000 cloud-pak-operations-cli-0.7.1/cpo/commands/ibmcloud/regenerate_api_key.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-20 13:56:31.421304 cloud-pak-operations-cli-0.7.1/cpo/config/
--rw-r--r--   0 runner    (1001) docker     (127)      706 2024-03-20 13:56:26.000000 cloud-pak-operations-cli-0.7.1/cpo/config/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3818 2024-03-20 13:56:26.000000 cloud-pak-operations-cli-0.7.1/cpo/config/binaries_manager.py
--rw-r--r--   0 runner    (1001) docker     (127)    17434 2024-03-20 13:56:26.000000 cloud-pak-operations-cli-0.7.1/cpo/config/cluster_credentials_manager.py
--rw-r--r--   0 runner    (1001) docker     (127)     8215 2024-03-20 13:56:26.000000 cloud-pak-operations-cli-0.7.1/cpo/config/configuration_manager.py
--rw-r--r--   0 runner    (1001) docker     (127)     1796 2024-03-20 13:56:26.000000 cloud-pak-operations-cli-0.7.1/cpo/cpo.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-20 13:56:31.409303 cloud-pak-operations-cli-0.7.1/cpo/deps/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-20 13:56:31.421304 cloud-pak-operations-cli-0.7.1/cpo/deps/autocomplete/
--rw-r--r--   0 runner    (1001) docker     (127)      651 2024-03-20 13:56:26.000000 cloud-pak-operations-cli-0.7.1/cpo/deps/autocomplete/cpo-autocomplete-bash.sh
--rw-r--r--   0 runner    (1001) docker     (127)      946 2024-03-20 13:56:26.000000 cloud-pak-operations-cli-0.7.1/cpo/deps/autocomplete/cpo-autocomplete-zsh.sh
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-20 13:56:31.421304 cloud-pak-operations-cli-0.7.1/cpo/deps/playbooks/
--rw-r--r--   0 runner    (1001) docker     (127)     1563 2024-03-20 13:56:26.000000 cloud-pak-operations-cli-0.7.1/cpo/deps/playbooks/delete_terminated_pods_playbook.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     9526 2024-03-20 13:56:26.000000 cloud-pak-operations-cli-0.7.1/cpo/deps/playbooks/deploy_odf_playbook.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-20 13:56:31.421304 cloud-pak-operations-cli-0.7.1/cpo/lib/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-20 13:56:26.000000 cloud-pak-operations-cli-0.7.1/cpo/lib/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-20 13:56:31.421304 cloud-pak-operations-cli-0.7.1/cpo/lib/ansible/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-20 13:56:26.000000 cloud-pak-operations-cli-0.7.1/cpo/lib/ansible/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-20 13:56:31.421304 cloud-pak-operations-cli-0.7.1/cpo/lib/ansible/modules/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-20 13:56:26.000000 cloud-pak-operations-cli-0.7.1/cpo/lib/ansible/modules/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5754 2024-03-20 13:56:26.000000 cloud-pak-operations-cli-0.7.1/cpo/lib/ansible/modules/abstract_module.py
--rw-r--r--   0 runner    (1001) docker     (127)      748 2024-03-20 13:56:26.000000 cloud-pak-operations-cli-0.7.1/cpo/lib/ansible/modules/custom_resource_event_result.py
--rw-r--r--   0 runner    (1001) docker     (127)     4441 2024-03-20 13:56:26.000000 cloud-pak-operations-cli-0.7.1/cpo/lib/ansible/modules/wait_for_custom_resource.py
--rw-r--r--   0 runner    (1001) docker     (127)     4658 2024-03-20 13:56:26.000000 cloud-pak-operations-cli-0.7.1/cpo/lib/ansible/modules/wait_for_custom_resource_definitions.py
--rw-r--r--   0 runner    (1001) docker     (127)     4608 2024-03-20 13:56:26.000000 cloud-pak-operations-cli-0.7.1/cpo/lib/ansible/modules/wait_for_namespaced_custom_resource.py
--rw-r--r--   0 runner    (1001) docker     (127)     3728 2024-03-20 13:56:26.000000 cloud-pak-operations-cli-0.7.1/cpo/lib/ansible/openshift_playbook_runner.py
--rw-r--r--   0 runner    (1001) docker     (127)     5074 2024-03-20 13:56:26.000000 cloud-pak-operations-cli-0.7.1/cpo/lib/ansible/playbook_runner.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-20 13:56:31.425304 cloud-pak-operations-cli-0.7.1/cpo/lib/click/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-20 13:56:26.000000 cloud-pak-operations-cli-0.7.1/cpo/lib/click/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1221 2024-03-20 13:56:26.000000 cloud-pak-operations-cli-0.7.1/cpo/lib/click/cpd_service_spec_param_type.py
--rw-r--r--   0 runner    (1001) docker     (127)    13173 2024-03-20 13:56:26.000000 cloud-pak-operations-cli-0.7.1/cpo/lib/click/lazy_loading_multi_command.py
--rw-r--r--   0 runner    (1001) docker     (127)     1761 2024-03-20 13:56:26.000000 cloud-pak-operations-cli-0.7.1/cpo/lib/click/package_directory_details.py
--rw-r--r--   0 runner    (1001) docker     (127)     8633 2024-03-20 13:56:26.000000 cloud-pak-operations-cli-0.7.1/cpo/lib/click/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-20 13:56:31.425304 cloud-pak-operations-cli-0.7.1/cpo/lib/cluster/
--rw-r--r--   0 runner    (1001) docker     (127)     1224 2024-03-20 13:56:26.000000 cloud-pak-operations-cli-0.7.1/cpo/lib/cluster/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1180 2024-03-20 13:56:26.000000 cloud-pak-operations-cli-0.7.1/cpo/lib/cluster/cluster.py
--rw-r--r--   0 runner    (1001) docker     (127)      931 2024-03-20 13:56:26.000000 cloud-pak-operations-cli-0.7.1/cpo/lib/cluster/cluster_factory.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-20 13:56:31.425304 cloud-pak-operations-cli-0.7.1/cpo/lib/dependency_manager/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-20 13:56:26.000000 cloud-pak-operations-cli-0.7.1/cpo/lib/dependency_manager/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    10042 2024-03-20 13:56:26.000000 cloud-pak-operations-cli-0.7.1/cpo/lib/dependency_manager/dependency_manager.py
--rw-r--r--   0 runner    (1001) docker     (127)     3033 2024-03-20 13:56:26.000000 cloud-pak-operations-cli-0.7.1/cpo/lib/dependency_manager/dependency_manager_binary_plugin.py
--rw-r--r--   0 runner    (1001) docker     (127)     5981 2024-03-20 13:56:26.000000 cloud-pak-operations-cli-0.7.1/cpo/lib/dependency_manager/dependency_manager_plugin.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-20 13:56:31.425304 cloud-pak-operations-cli-0.7.1/cpo/lib/dependency_manager/plugins/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-20 13:56:26.000000 cloud-pak-operations-cli-0.7.1/cpo/lib/dependency_manager/plugins/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5323 2024-03-20 13:56:26.000000 cloud-pak-operations-cli-0.7.1/cpo/lib/dependency_manager/plugins/ibm_cloud_cli_plugin.py
--rw-r--r--   0 runner    (1001) docker     (127)     3891 2024-03-20 13:56:26.000000 cloud-pak-operations-cli-0.7.1/cpo/lib/dependency_manager/plugins/ibm_cloud_pak_cli_plugin.py
--rw-r--r--   0 runner    (1001) docker     (127)     4645 2024-03-20 13:56:26.000000 cloud-pak-operations-cli-0.7.1/cpo/lib/dependency_manager/plugins/ibm_cloud_terraform_provider_plugin.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-20 13:56:31.425304 cloud-pak-operations-cli-0.7.1/cpo/lib/dependency_manager/plugins/openshift/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-20 13:56:26.000000 cloud-pak-operations-cli-0.7.1/cpo/lib/dependency_manager/plugins/openshift/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1408 2024-03-20 13:56:26.000000 cloud-pak-operations-cli-0.7.1/cpo/lib/dependency_manager/plugins/openshift/openshift_cli_plugin.py
--rw-r--r--   0 runner    (1001) docker     (127)     2446 2024-03-20 13:56:26.000000 cloud-pak-operations-cli-0.7.1/cpo/lib/dependency_manager/plugins/openshift/openshift_install_plugin.py
--rw-r--r--   0 runner    (1001) docker     (127)     5395 2024-03-20 13:56:26.000000 cloud-pak-operations-cli-0.7.1/cpo/lib/dependency_manager/plugins/openshift/openshift_plugin.py
--rw-r--r--   0 runner    (1001) docker     (127)     4824 2024-03-20 13:56:26.000000 cloud-pak-operations-cli-0.7.1/cpo/lib/dependency_manager/plugins/terraform_plugin.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-20 13:56:31.425304 cloud-pak-operations-cli-0.7.1/cpo/lib/ibm_internal_plugin/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-20 13:56:26.000000 cloud-pak-operations-cli-0.7.1/cpo/lib/ibm_internal_plugin/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4111 2024-03-20 13:56:26.000000 cloud-pak-operations-cli-0.7.1/cpo/lib/ibm_internal_plugin/ibm_internal_plugin_manager.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-20 13:56:31.425304 cloud-pak-operations-cli-0.7.1/cpo/lib/ibmcloud/
--rw-r--r--   0 runner    (1001) docker     (127)      845 2024-03-20 13:56:26.000000 cloud-pak-operations-cli-0.7.1/cpo/lib/ibmcloud/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-20 13:56:31.429304 cloud-pak-operations-cli-0.7.1/cpo/lib/ibmcloud/data/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-20 13:56:26.000000 cloud-pak-operations-cli-0.7.1/cpo/lib/ibmcloud/data/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1703 2024-03-20 13:56:26.000000 cloud-pak-operations-cli-0.7.1/cpo/lib/ibmcloud/data/cluster_status.py
--rw-r--r--   0 runner    (1001) docker     (127)      921 2024-03-20 13:56:26.000000 cloud-pak-operations-cli-0.7.1/cpo/lib/ibmcloud/data/ingress_status.py
--rw-r--r--   0 runner    (1001) docker     (127)    19829 2024-03-20 13:56:26.000000 cloud-pak-operations-cli-0.7.1/cpo/lib/ibmcloud/ibm_cloud_api_manager.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-20 13:56:31.429304 cloud-pak-operations-cli-0.7.1/cpo/lib/ibmcloud/oc/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-20 13:56:26.000000 cloud-pak-operations-cli-0.7.1/cpo/lib/ibmcloud/oc/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-20 13:56:31.429304 cloud-pak-operations-cli-0.7.1/cpo/lib/ibmcloud/oc/cluster/
--rw-r--r--   0 runner    (1001) docker     (127)      778 2024-03-20 13:56:26.000000 cloud-pak-operations-cli-0.7.1/cpo/lib/ibmcloud/oc/cluster/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      972 2024-03-20 13:56:26.000000 cloud-pak-operations-cli-0.7.1/cpo/lib/ibmcloud/oc/cluster/ls.py
--rw-r--r--   0 runner    (1001) docker     (127)     1926 2024-03-20 13:56:26.000000 cloud-pak-operations-cli-0.7.1/cpo/lib/ibmcloud/oc/cluster/roks_cluster.py
--rw-r--r--   0 runner    (1001) docker     (127)     1124 2024-03-20 13:56:26.000000 cloud-pak-operations-cli-0.7.1/cpo/lib/ibmcloud/oc/cluster/roks_cluster_factory.py
--rw-r--r--   0 runner    (1001) docker     (127)     3480 2024-03-20 13:56:26.000000 cloud-pak-operations-cli-0.7.1/cpo/lib/jmespath.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-20 13:56:31.429304 cloud-pak-operations-cli-0.7.1/cpo/lib/openshift/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-20 13:56:26.000000 cloud-pak-operations-cli-0.7.1/cpo/lib/openshift/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-20 13:56:31.429304 cloud-pak-operations-cli-0.7.1/cpo/lib/openshift/cluster/
--rw-r--r--   0 runner    (1001) docker     (127)      778 2024-03-20 13:56:26.000000 cloud-pak-operations-cli-0.7.1/cpo/lib/openshift/cluster/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1199 2024-03-20 13:56:26.000000 cloud-pak-operations-cli-0.7.1/cpo/lib/openshift/cluster/generic_cluster.py
--rw-r--r--   0 runner    (1001) docker     (127)     1105 2024-03-20 13:56:26.000000 cloud-pak-operations-cli-0.7.1/cpo/lib/openshift/cluster/generic_cluster_factory.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-20 13:56:31.429304 cloud-pak-operations-cli-0.7.1/cpo/lib/openshift/credentials/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-20 13:56:26.000000 cloud-pak-operations-cli-0.7.1/cpo/lib/openshift/credentials/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2048 2024-03-20 13:56:26.000000 cloud-pak-operations-cli-0.7.1/cpo/lib/openshift/credentials/cluster_based_user_credentials.py
--rw-r--r--   0 runner    (1001) docker     (127)     2367 2024-03-20 13:56:26.000000 cloud-pak-operations-cli-0.7.1/cpo/lib/openshift/credentials/credentials.py
--rw-r--r--   0 runner    (1001) docker     (127)     1354 2024-03-20 13:56:26.000000 cloud-pak-operations-cli-0.7.1/cpo/lib/openshift/credentials/token_credentials.py
--rw-r--r--   0 runner    (1001) docker     (127)     4209 2024-03-20 13:56:26.000000 cloud-pak-operations-cli-0.7.1/cpo/lib/openshift/credentials/user_credentials.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-20 13:56:31.429304 cloud-pak-operations-cli-0.7.1/cpo/lib/openshift/data/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-20 13:56:26.000000 cloud-pak-operations-cli-0.7.1/cpo/lib/openshift/data/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6591 2024-03-20 13:56:26.000000 cloud-pak-operations-cli-0.7.1/cpo/lib/openshift/data/global_pull_secret_data.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-20 13:56:31.429304 cloud-pak-operations-cli-0.7.1/cpo/lib/openshift/nfs/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-20 13:56:26.000000 cloud-pak-operations-cli-0.7.1/cpo/lib/openshift/nfs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    13709 2024-03-20 13:56:26.000000 cloud-pak-operations-cli-0.7.1/cpo/lib/openshift/nfs/nfs_subdir_external_provisioner.py
--rw-r--r--   0 runner    (1001) docker     (127)     9279 2024-03-20 13:56:26.000000 cloud-pak-operations-cli-0.7.1/cpo/lib/openshift/oc.py
--rw-r--r--   0 runner    (1001) docker     (127)    46470 2024-03-20 13:56:26.000000 cloud-pak-operations-cli-0.7.1/cpo/lib/openshift/openshift_api_manager.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-20 13:56:31.429304 cloud-pak-operations-cli-0.7.1/cpo/lib/openshift/openshift_install/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-20 13:56:26.000000 cloud-pak-operations-cli-0.7.1/cpo/lib/openshift/openshift_install/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8373 2024-03-20 13:56:26.000000 cloud-pak-operations-cli-0.7.1/cpo/lib/openshift/openshift_install/openshift_installation_manager.py
--rw-r--r--   0 runner    (1001) docker     (127)      751 2024-03-20 13:56:26.000000 cloud-pak-operations-cli-0.7.1/cpo/lib/openshift/openshift_install/openshift_installation_manager_plugin.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-20 13:56:31.429304 cloud-pak-operations-cli-0.7.1/cpo/lib/openshift/openshift_install/types/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-20 13:56:26.000000 cloud-pak-operations-cli-0.7.1/cpo/lib/openshift/openshift_install/types/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      664 2024-03-20 13:56:26.000000 cloud-pak-operations-cli-0.7.1/cpo/lib/openshift/openshift_install/types/architecture.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-20 13:56:31.433304 cloud-pak-operations-cli-0.7.1/cpo/lib/openshift/types/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-20 13:56:26.000000 cloud-pak-operations-cli-0.7.1/cpo/lib/openshift/types/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      725 2024-03-20 13:56:26.000000 cloud-pak-operations-cli-0.7.1/cpo/lib/openshift/types/auths_dict.py
--rw-r--r--   0 runner    (1001) docker     (127)     1456 2024-03-20 13:56:26.000000 cloud-pak-operations-cli-0.7.1/cpo/lib/openshift/types/catalog_source.py
--rw-r--r--   0 runner    (1001) docker     (127)      688 2024-03-20 13:56:26.000000 cloud-pak-operations-cli-0.7.1/cpo/lib/openshift/types/credentials.py
--rw-r--r--   0 runner    (1001) docker     (127)     1226 2024-03-20 13:56:26.000000 cloud-pak-operations-cli-0.7.1/cpo/lib/openshift/types/custom_resource.py
--rw-r--r--   0 runner    (1001) docker     (127)      748 2024-03-20 13:56:26.000000 cloud-pak-operations-cli-0.7.1/cpo/lib/openshift/types/custom_resource_event_result.py
--rw-r--r--   0 runner    (1001) docker     (127)     1794 2024-03-20 13:56:26.000000 cloud-pak-operations-cli-0.7.1/cpo/lib/openshift/types/get_pod_entry.py
--rw-r--r--   0 runner    (1001) docker     (127)      715 2024-03-20 13:56:26.000000 cloud-pak-operations-cli-0.7.1/cpo/lib/openshift/types/kind_metadata.py
--rw-r--r--   0 runner    (1001) docker     (127)     1030 2024-03-20 13:56:26.000000 cloud-pak-operations-cli-0.7.1/cpo/lib/openshift/types/object_meta.py
--rw-r--r--   0 runner    (1001) docker     (127)     1073 2024-03-20 13:56:26.000000 cloud-pak-operations-cli-0.7.1/cpo/lib/openshift/types/operator_group.py
--rw-r--r--   0 runner    (1001) docker     (127)     1195 2024-03-20 13:56:26.000000 cloud-pak-operations-cli-0.7.1/cpo/lib/openshift/types/role.py
--rw-r--r--   0 runner    (1001) docker     (127)     1391 2024-03-20 13:56:26.000000 cloud-pak-operations-cli-0.7.1/cpo/lib/openshift/types/role_binding.py
--rw-r--r--   0 runner    (1001) docker     (127)      763 2024-03-20 13:56:26.000000 cloud-pak-operations-cli-0.7.1/cpo/lib/openshift/types/role_rule.py
--rw-r--r--   0 runner    (1001) docker     (127)      937 2024-03-20 13:56:26.000000 cloud-pak-operations-cli-0.7.1/cpo/lib/openshift/types/service_account.py
--rw-r--r--   0 runner    (1001) docker     (127)     1281 2024-03-20 13:56:26.000000 cloud-pak-operations-cli-0.7.1/cpo/lib/openshift/types/subscription.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-20 13:56:31.433304 cloud-pak-operations-cli-0.7.1/cpo/lib/openshift/utils/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-20 13:56:26.000000 cloud-pak-operations-cli-0.7.1/cpo/lib/openshift/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2313 2024-03-20 13:56:26.000000 cloud-pak-operations-cli-0.7.1/cpo/lib/openshift/utils/click.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-20 13:56:31.433304 cloud-pak-operations-cli-0.7.1/cpo/lib/plugin_manager/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-20 13:56:26.000000 cloud-pak-operations-cli-0.7.1/cpo/lib/plugin_manager/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2865 2024-03-20 13:56:26.000000 cloud-pak-operations-cli-0.7.1/cpo/lib/plugin_manager/package_data.py
--rw-r--r--   0 runner    (1001) docker     (127)     5700 2024-03-20 13:56:26.000000 cloud-pak-operations-cli-0.7.1/cpo/lib/plugin_manager/plugin_manager.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-20 13:56:31.433304 cloud-pak-operations-cli-0.7.1/cpo/scripts/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-20 13:56:26.000000 cloud-pak-operations-cli-0.7.1/cpo/scripts/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1336 2024-03-20 13:56:26.000000 cloud-pak-operations-cli-0.7.1/cpo/scripts/get_current_cluster_alias.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-20 13:56:31.437304 cloud-pak-operations-cli-0.7.1/cpo/utils/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-20 13:56:26.000000 cloud-pak-operations-cli-0.7.1/cpo/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7923 2024-03-20 13:56:26.000000 cloud-pak-operations-cli-0.7.1/cpo/utils/compression.py
--rw-r--r--   0 runner    (1001) docker     (127)     1029 2024-03-20 13:56:26.000000 cloud-pak-operations-cli-0.7.1/cpo/utils/debugger.py
--rw-r--r--   0 runner    (1001) docker     (127)     4773 2024-03-20 13:56:26.000000 cloud-pak-operations-cli-0.7.1/cpo/utils/download.py
--rw-r--r--   0 runner    (1001) docker     (127)     3513 2024-03-20 13:56:26.000000 cloud-pak-operations-cli-0.7.1/cpo/utils/error.py
--rw-r--r--   0 runner    (1001) docker     (127)      994 2024-03-20 13:56:26.000000 cloud-pak-operations-cli-0.7.1/cpo/utils/file.py
--rw-r--r--   0 runner    (1001) docker     (127)      819 2024-03-20 13:56:26.000000 cloud-pak-operations-cli-0.7.1/cpo/utils/http_method.py
--rw-r--r--   0 runner    (1001) docker     (127)     2558 2024-03-20 13:56:26.000000 cloud-pak-operations-cli-0.7.1/cpo/utils/importlib.py
--rw-r--r--   0 runner    (1001) docker     (127)     6686 2024-03-20 13:56:26.000000 cloud-pak-operations-cli-0.7.1/cpo/utils/logging.py
--rw-r--r--   0 runner    (1001) docker     (127)     4301 2024-03-20 13:56:26.000000 cloud-pak-operations-cli-0.7.1/cpo/utils/network.py
--rw-r--r--   0 runner    (1001) docker     (127)     1524 2024-03-20 13:56:26.000000 cloud-pak-operations-cli-0.7.1/cpo/utils/operating_system.py
--rw-r--r--   0 runner    (1001) docker     (127)     6438 2024-03-20 13:56:26.000000 cloud-pak-operations-cli-0.7.1/cpo/utils/process.py
--rw-r--r--   0 runner    (1001) docker     (127)     6519 2024-03-20 13:56:26.000000 cloud-pak-operations-cli-0.7.1/cpo/utils/ssh.py
--rw-r--r--   0 runner    (1001) docker     (127)     1396 2024-03-20 13:56:26.000000 cloud-pak-operations-cli-0.7.1/cpo/utils/wait.py
--rw-r--r--   0 runner    (1001) docker     (127)     1340 2024-03-20 13:56:26.000000 cloud-pak-operations-cli-0.7.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-20 13:56:31.437304 cloud-pak-operations-cli-0.7.1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 08:16:33.981149 cloud_pak_operations_cli-0.7.2/
+-rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-04-29 08:16:19.000000 cloud_pak_operations_cli-0.7.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       29 2024-04-29 08:16:19.000000 cloud_pak_operations_cli-0.7.2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     2497 2024-04-29 08:16:33.981149 cloud_pak_operations_cli-0.7.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1346 2024-04-29 08:16:19.000000 cloud_pak_operations_cli-0.7.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 08:16:33.981149 cloud_pak_operations_cli-0.7.2/cloud_pak_operations_cli.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2497 2024-04-29 08:16:33.000000 cloud_pak_operations_cli-0.7.2/cloud_pak_operations_cli.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     6458 2024-04-29 08:16:33.000000 cloud_pak_operations_cli-0.7.2/cloud_pak_operations_cli.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-29 08:16:33.000000 cloud_pak_operations_cli-0.7.2/cloud_pak_operations_cli.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      132 2024-04-29 08:16:33.000000 cloud_pak_operations_cli-0.7.2/cloud_pak_operations_cli.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      208 2024-04-29 08:16:33.000000 cloud_pak_operations_cli-0.7.2/cloud_pak_operations_cli.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        4 2024-04-29 08:16:33.000000 cloud_pak_operations_cli-0.7.2/cloud_pak_operations_cli.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 08:16:33.953149 cloud_pak_operations_cli-0.7.2/cpo/
+-rw-r--r--   0 runner    (1001) docker     (127)      945 2024-04-29 08:16:19.000000 cloud_pak_operations_cli-0.7.2/cpo/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 08:16:33.953149 cloud_pak_operations_cli-0.7.2/cpo/commands/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-29 08:16:19.000000 cloud_pak_operations_cli-0.7.2/cpo/commands/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 08:16:33.953149 cloud_pak_operations_cli-0.7.2/cpo/commands/adm/
+-rw-r--r--   0 runner    (1001) docker     (127)      635 2024-04-29 08:16:19.000000 cloud_pak_operations_cli-0.7.2/cpo/commands/adm/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      879 2024-04-29 08:16:19.000000 cloud_pak_operations_cli-0.7.2/cpo/commands/adm/download_dependencies.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1123 2024-04-29 08:16:19.000000 cloud_pak_operations_cli-0.7.2/cpo/commands/adm/get-shell-completion-script-location.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 08:16:33.953149 cloud_pak_operations_cli-0.7.2/cpo/commands/adm/ibm_internal_plugin/
+-rw-r--r--   0 runner    (1001) docker     (127)      653 2024-04-29 08:16:19.000000 cloud_pak_operations_cli-0.7.2/cpo/commands/adm/ibm_internal_plugin/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3726 2024-04-29 08:16:19.000000 cloud_pak_operations_cli-0.7.2/cpo/commands/adm/ibm_internal_plugin/install.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1838 2024-04-29 08:16:19.000000 cloud_pak_operations_cli-0.7.2/cpo/commands/adm/ibm_internal_plugin/ls.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2813 2024-04-29 08:16:19.000000 cloud_pak_operations_cli-0.7.2/cpo/commands/adm/ibm_internal_plugin/upgrade_plugins.py
+-rw-r--r--   0 runner    (1001) docker     (127)      996 2024-04-29 08:16:19.000000 cloud_pak_operations_cli-0.7.2/cpo/commands/adm/set_config_option.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1388 2024-04-29 08:16:19.000000 cloud_pak_operations_cli-0.7.2/cpo/commands/adm/store_credentials.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1573 2024-04-29 08:16:19.000000 cloud_pak_operations_cli-0.7.2/cpo/commands/adm/update_dev.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 08:16:33.957149 cloud_pak_operations_cli-0.7.2/cpo/commands/cluster/
+-rw-r--r--   0 runner    (1001) docker     (127)      632 2024-04-29 08:16:19.000000 cloud_pak_operations_cli-0.7.2/cpo/commands/cluster/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1829 2024-04-29 08:16:19.000000 cloud_pak_operations_cli-0.7.2/cpo/commands/cluster/add.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1342 2024-04-29 08:16:19.000000 cloud_pak_operations_cli-0.7.2/cpo/commands/cluster/current.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1802 2024-04-29 08:16:19.000000 cloud_pak_operations_cli-0.7.2/cpo/commands/cluster/edit.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1743 2024-04-29 08:16:19.000000 cloud_pak_operations_cli-0.7.2/cpo/commands/cluster/get_cluster_access_token.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1286 2024-04-29 08:16:19.000000 cloud_pak_operations_cli-0.7.2/cpo/commands/cluster/login.py
+-rw-r--r--   0 runner    (1001) docker     (127)      883 2024-04-29 08:16:19.000000 cloud_pak_operations_cli-0.7.2/cpo/commands/cluster/ls.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 08:16:33.957149 cloud_pak_operations_cli-0.7.2/cpo/commands/cluster/pods/
+-rw-r--r--   0 runner    (1001) docker     (127)      622 2024-04-29 08:16:19.000000 cloud_pak_operations_cli-0.7.2/cpo/commands/cluster/pods/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1579 2024-04-29 08:16:19.000000 cloud_pak_operations_cli-0.7.2/cpo/commands/cluster/pods/delete_terminated_pods.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 08:16:33.957149 cloud_pak_operations_cli-0.7.2/cpo/commands/cluster/pull_secret/
+-rw-r--r--   0 runner    (1001) docker     (127)      646 2024-04-29 08:16:19.000000 cloud_pak_operations_cli-0.7.2/cpo/commands/cluster/pull_secret/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1488 2024-04-29 08:16:19.000000 cloud_pak_operations_cli-0.7.2/cpo/commands/cluster/pull_secret/ls.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1466 2024-04-29 08:16:19.000000 cloud_pak_operations_cli-0.7.2/cpo/commands/cluster/pull_secret/rm.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1785 2024-04-29 08:16:19.000000 cloud_pak_operations_cli-0.7.2/cpo/commands/cluster/pull_secret/set.py
+-rw-r--r--   0 runner    (1001) docker     (127)      885 2024-04-29 08:16:19.000000 cloud_pak_operations_cli-0.7.2/cpo/commands/cluster/reset_current_cluster.py
+-rw-r--r--   0 runner    (1001) docker     (127)      939 2024-04-29 08:16:19.000000 cloud_pak_operations_cli-0.7.2/cpo/commands/cluster/rm.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 08:16:33.957149 cloud_pak_operations_cli-0.7.2/cpo/commands/cluster/storage/
+-rw-r--r--   0 runner    (1001) docker     (127)      654 2024-04-29 08:16:19.000000 cloud_pak_operations_cli-0.7.2/cpo/commands/cluster/storage/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2002 2024-04-29 08:16:19.000000 cloud_pak_operations_cli-0.7.2/cpo/commands/cluster/storage/install_kubernetes_nfs_subdir_external_provisioner.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1860 2024-04-29 08:16:19.000000 cloud_pak_operations_cli-0.7.2/cpo/commands/cluster/storage/install_openshift_data_foundation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1124 2024-04-29 08:16:19.000000 cloud_pak_operations_cli-0.7.2/cpo/commands/cluster/use.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 08:16:33.957149 cloud_pak_operations_cli-0.7.2/cpo/commands/ibmcloud/
+-rw-r--r--   0 runner    (1001) docker     (127)      643 2024-04-29 08:16:19.000000 cloud_pak_operations_cli-0.7.2/cpo/commands/ibmcloud/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      809 2024-04-29 08:16:19.000000 cloud_pak_operations_cli-0.7.2/cpo/commands/ibmcloud/login.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1211 2024-04-29 08:16:19.000000 cloud_pak_operations_cli-0.7.2/cpo/commands/ibmcloud/logout.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 08:16:33.957149 cloud_pak_operations_cli-0.7.2/cpo/commands/ibmcloud/oc/
+-rw-r--r--   0 runner    (1001) docker     (127)      654 2024-04-29 08:16:19.000000 cloud_pak_operations_cli-0.7.2/cpo/commands/ibmcloud/oc/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 08:16:33.961149 cloud_pak_operations_cli-0.7.2/cpo/commands/ibmcloud/oc/cluster/
+-rw-r--r--   0 runner    (1001) docker     (127)      663 2024-04-29 08:16:19.000000 cloud_pak_operations_cli-0.7.2/cpo/commands/ibmcloud/oc/cluster/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1520 2024-04-29 08:16:19.000000 cloud_pak_operations_cli-0.7.2/cpo/commands/ibmcloud/oc/cluster/add.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1370 2024-04-29 08:16:19.000000 cloud_pak_operations_cli-0.7.2/cpo/commands/ibmcloud/oc/cluster/login.py
+-rw-r--r--   0 runner    (1001) docker     (127)      943 2024-04-29 08:16:19.000000 cloud_pak_operations_cli-0.7.2/cpo/commands/ibmcloud/oc/cluster/ls.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1195 2024-04-29 08:16:19.000000 cloud_pak_operations_cli-0.7.2/cpo/commands/ibmcloud/oc/cluster/rm.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1202 2024-04-29 08:16:19.000000 cloud_pak_operations_cli-0.7.2/cpo/commands/ibmcloud/oc/cluster/status.py
+-rw-r--r--   0 runner    (1001) docker     (127)      897 2024-04-29 08:16:19.000000 cloud_pak_operations_cli-0.7.2/cpo/commands/ibmcloud/regenerate_api_key.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 08:16:33.961149 cloud_pak_operations_cli-0.7.2/cpo/config/
+-rw-r--r--   0 runner    (1001) docker     (127)      706 2024-04-29 08:16:19.000000 cloud_pak_operations_cli-0.7.2/cpo/config/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3742 2024-04-29 08:16:19.000000 cloud_pak_operations_cli-0.7.2/cpo/config/binaries_manager.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17370 2024-04-29 08:16:19.000000 cloud_pak_operations_cli-0.7.2/cpo/config/cluster_credentials_manager.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8184 2024-04-29 08:16:19.000000 cloud_pak_operations_cli-0.7.2/cpo/config/configuration_manager.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1796 2024-04-29 08:16:19.000000 cloud_pak_operations_cli-0.7.2/cpo/cpo.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 08:16:33.945149 cloud_pak_operations_cli-0.7.2/cpo/deps/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 08:16:33.961149 cloud_pak_operations_cli-0.7.2/cpo/deps/autocomplete/
+-rw-r--r--   0 runner    (1001) docker     (127)      651 2024-04-29 08:16:19.000000 cloud_pak_operations_cli-0.7.2/cpo/deps/autocomplete/cpo-autocomplete-bash.sh
+-rw-r--r--   0 runner    (1001) docker     (127)      946 2024-04-29 08:16:19.000000 cloud_pak_operations_cli-0.7.2/cpo/deps/autocomplete/cpo-autocomplete-zsh.sh
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 08:16:33.961149 cloud_pak_operations_cli-0.7.2/cpo/deps/playbooks/
+-rw-r--r--   0 runner    (1001) docker     (127)     1563 2024-04-29 08:16:19.000000 cloud_pak_operations_cli-0.7.2/cpo/deps/playbooks/delete_terminated_pods_playbook.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     9526 2024-04-29 08:16:19.000000 cloud_pak_operations_cli-0.7.2/cpo/deps/playbooks/deploy_odf_playbook.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 08:16:33.961149 cloud_pak_operations_cli-0.7.2/cpo/lib/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-29 08:16:19.000000 cloud_pak_operations_cli-0.7.2/cpo/lib/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 08:16:33.961149 cloud_pak_operations_cli-0.7.2/cpo/lib/ansible/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-29 08:16:19.000000 cloud_pak_operations_cli-0.7.2/cpo/lib/ansible/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 08:16:33.965149 cloud_pak_operations_cli-0.7.2/cpo/lib/ansible/modules/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-29 08:16:19.000000 cloud_pak_operations_cli-0.7.2/cpo/lib/ansible/modules/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5726 2024-04-29 08:16:19.000000 cloud_pak_operations_cli-0.7.2/cpo/lib/ansible/modules/abstract_module.py
+-rw-r--r--   0 runner    (1001) docker     (127)      723 2024-04-29 08:16:19.000000 cloud_pak_operations_cli-0.7.2/cpo/lib/ansible/modules/custom_resource_event_result.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4419 2024-04-29 08:16:19.000000 cloud_pak_operations_cli-0.7.2/cpo/lib/ansible/modules/wait_for_custom_resource.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4646 2024-04-29 08:16:19.000000 cloud_pak_operations_cli-0.7.2/cpo/lib/ansible/modules/wait_for_custom_resource_definitions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4676 2024-04-29 08:16:19.000000 cloud_pak_operations_cli-0.7.2/cpo/lib/ansible/modules/wait_for_namespaced_custom_resource.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3715 2024-04-29 08:16:19.000000 cloud_pak_operations_cli-0.7.2/cpo/lib/ansible/openshift_playbook_runner.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5074 2024-04-29 08:16:19.000000 cloud_pak_operations_cli-0.7.2/cpo/lib/ansible/playbook_runner.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 08:16:33.965149 cloud_pak_operations_cli-0.7.2/cpo/lib/click/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-29 08:16:19.000000 cloud_pak_operations_cli-0.7.2/cpo/lib/click/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1211 2024-04-29 08:16:19.000000 cloud_pak_operations_cli-0.7.2/cpo/lib/click/cpd_service_spec_param_type.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13693 2024-04-29 08:16:19.000000 cloud_pak_operations_cli-0.7.2/cpo/lib/click/lazy_loading_multi_command.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1761 2024-04-29 08:16:19.000000 cloud_pak_operations_cli-0.7.2/cpo/lib/click/package_directory_details.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8614 2024-04-29 08:16:19.000000 cloud_pak_operations_cli-0.7.2/cpo/lib/click/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 08:16:33.965149 cloud_pak_operations_cli-0.7.2/cpo/lib/cluster/
+-rw-r--r--   0 runner    (1001) docker     (127)     1224 2024-04-29 08:16:19.000000 cloud_pak_operations_cli-0.7.2/cpo/lib/cluster/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1180 2024-04-29 08:16:19.000000 cloud_pak_operations_cli-0.7.2/cpo/lib/cluster/cluster.py
+-rw-r--r--   0 runner    (1001) docker     (127)      931 2024-04-29 08:16:19.000000 cloud_pak_operations_cli-0.7.2/cpo/lib/cluster/cluster_factory.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 08:16:33.965149 cloud_pak_operations_cli-0.7.2/cpo/lib/dependency_manager/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-29 08:16:19.000000 cloud_pak_operations_cli-0.7.2/cpo/lib/dependency_manager/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10023 2024-04-29 08:16:19.000000 cloud_pak_operations_cli-0.7.2/cpo/lib/dependency_manager/dependency_manager.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3033 2024-04-29 08:16:19.000000 cloud_pak_operations_cli-0.7.2/cpo/lib/dependency_manager/dependency_manager_binary_plugin.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5944 2024-04-29 08:16:19.000000 cloud_pak_operations_cli-0.7.2/cpo/lib/dependency_manager/dependency_manager_plugin.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 08:16:33.965149 cloud_pak_operations_cli-0.7.2/cpo/lib/dependency_manager/plugins/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-29 08:16:19.000000 cloud_pak_operations_cli-0.7.2/cpo/lib/dependency_manager/plugins/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5291 2024-04-29 08:16:19.000000 cloud_pak_operations_cli-0.7.2/cpo/lib/dependency_manager/plugins/ibm_cloud_cli_plugin.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3859 2024-04-29 08:16:19.000000 cloud_pak_operations_cli-0.7.2/cpo/lib/dependency_manager/plugins/ibm_cloud_pak_cli_plugin.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4645 2024-04-29 08:16:19.000000 cloud_pak_operations_cli-0.7.2/cpo/lib/dependency_manager/plugins/ibm_cloud_terraform_provider_plugin.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 08:16:33.965149 cloud_pak_operations_cli-0.7.2/cpo/lib/dependency_manager/plugins/openshift/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-29 08:16:19.000000 cloud_pak_operations_cli-0.7.2/cpo/lib/dependency_manager/plugins/openshift/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1382 2024-04-29 08:16:19.000000 cloud_pak_operations_cli-0.7.2/cpo/lib/dependency_manager/plugins/openshift/openshift_cli_plugin.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2420 2024-04-29 08:16:19.000000 cloud_pak_operations_cli-0.7.2/cpo/lib/dependency_manager/plugins/openshift/openshift_install_plugin.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5395 2024-04-29 08:16:19.000000 cloud_pak_operations_cli-0.7.2/cpo/lib/dependency_manager/plugins/openshift/openshift_plugin.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4792 2024-04-29 08:16:19.000000 cloud_pak_operations_cli-0.7.2/cpo/lib/dependency_manager/plugins/terraform_plugin.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 08:16:33.969149 cloud_pak_operations_cli-0.7.2/cpo/lib/ibm_internal_plugin/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-29 08:16:19.000000 cloud_pak_operations_cli-0.7.2/cpo/lib/ibm_internal_plugin/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4111 2024-04-29 08:16:19.000000 cloud_pak_operations_cli-0.7.2/cpo/lib/ibm_internal_plugin/ibm_internal_plugin_manager.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 08:16:33.969149 cloud_pak_operations_cli-0.7.2/cpo/lib/ibmcloud/
+-rw-r--r--   0 runner    (1001) docker     (127)      845 2024-04-29 08:16:19.000000 cloud_pak_operations_cli-0.7.2/cpo/lib/ibmcloud/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 08:16:33.969149 cloud_pak_operations_cli-0.7.2/cpo/lib/ibmcloud/data/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-29 08:16:19.000000 cloud_pak_operations_cli-0.7.2/cpo/lib/ibmcloud/data/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1703 2024-04-29 08:16:19.000000 cloud_pak_operations_cli-0.7.2/cpo/lib/ibmcloud/data/cluster_status.py
+-rw-r--r--   0 runner    (1001) docker     (127)      921 2024-04-29 08:16:19.000000 cloud_pak_operations_cli-0.7.2/cpo/lib/ibmcloud/data/ingress_status.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19809 2024-04-29 08:16:19.000000 cloud_pak_operations_cli-0.7.2/cpo/lib/ibmcloud/ibm_cloud_api_manager.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 08:16:33.969149 cloud_pak_operations_cli-0.7.2/cpo/lib/ibmcloud/oc/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-29 08:16:19.000000 cloud_pak_operations_cli-0.7.2/cpo/lib/ibmcloud/oc/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 08:16:33.969149 cloud_pak_operations_cli-0.7.2/cpo/lib/ibmcloud/oc/cluster/
+-rw-r--r--   0 runner    (1001) docker     (127)      778 2024-04-29 08:16:19.000000 cloud_pak_operations_cli-0.7.2/cpo/lib/ibmcloud/oc/cluster/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      972 2024-04-29 08:16:19.000000 cloud_pak_operations_cli-0.7.2/cpo/lib/ibmcloud/oc/cluster/ls.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1926 2024-04-29 08:16:19.000000 cloud_pak_operations_cli-0.7.2/cpo/lib/ibmcloud/oc/cluster/roks_cluster.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1124 2024-04-29 08:16:19.000000 cloud_pak_operations_cli-0.7.2/cpo/lib/ibmcloud/oc/cluster/roks_cluster_factory.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3480 2024-04-29 08:16:19.000000 cloud_pak_operations_cli-0.7.2/cpo/lib/jmespath.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 08:16:33.969149 cloud_pak_operations_cli-0.7.2/cpo/lib/openshift/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-29 08:16:19.000000 cloud_pak_operations_cli-0.7.2/cpo/lib/openshift/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 08:16:33.969149 cloud_pak_operations_cli-0.7.2/cpo/lib/openshift/cluster/
+-rw-r--r--   0 runner    (1001) docker     (127)      778 2024-04-29 08:16:19.000000 cloud_pak_operations_cli-0.7.2/cpo/lib/openshift/cluster/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1199 2024-04-29 08:16:19.000000 cloud_pak_operations_cli-0.7.2/cpo/lib/openshift/cluster/generic_cluster.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1105 2024-04-29 08:16:19.000000 cloud_pak_operations_cli-0.7.2/cpo/lib/openshift/cluster/generic_cluster_factory.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 08:16:33.973149 cloud_pak_operations_cli-0.7.2/cpo/lib/openshift/credentials/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-29 08:16:19.000000 cloud_pak_operations_cli-0.7.2/cpo/lib/openshift/credentials/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2056 2024-04-29 08:16:19.000000 cloud_pak_operations_cli-0.7.2/cpo/lib/openshift/credentials/cluster_based_user_credentials.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2367 2024-04-29 08:16:19.000000 cloud_pak_operations_cli-0.7.2/cpo/lib/openshift/credentials/credentials.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1354 2024-04-29 08:16:19.000000 cloud_pak_operations_cli-0.7.2/cpo/lib/openshift/credentials/token_credentials.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4192 2024-04-29 08:16:19.000000 cloud_pak_operations_cli-0.7.2/cpo/lib/openshift/credentials/user_credentials.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 08:16:33.973149 cloud_pak_operations_cli-0.7.2/cpo/lib/openshift/data/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-29 08:16:19.000000 cloud_pak_operations_cli-0.7.2/cpo/lib/openshift/data/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6578 2024-04-29 08:16:19.000000 cloud_pak_operations_cli-0.7.2/cpo/lib/openshift/data/global_pull_secret_data.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 08:16:33.973149 cloud_pak_operations_cli-0.7.2/cpo/lib/openshift/nfs/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-29 08:16:19.000000 cloud_pak_operations_cli-0.7.2/cpo/lib/openshift/nfs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13709 2024-04-29 08:16:19.000000 cloud_pak_operations_cli-0.7.2/cpo/lib/openshift/nfs/nfs_subdir_external_provisioner.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9279 2024-04-29 08:16:19.000000 cloud_pak_operations_cli-0.7.2/cpo/lib/openshift/oc.py
+-rw-r--r--   0 runner    (1001) docker     (127)    46436 2024-04-29 08:16:19.000000 cloud_pak_operations_cli-0.7.2/cpo/lib/openshift/openshift_api_manager.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 08:16:33.973149 cloud_pak_operations_cli-0.7.2/cpo/lib/openshift/openshift_install/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-29 08:16:19.000000 cloud_pak_operations_cli-0.7.2/cpo/lib/openshift/openshift_install/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8373 2024-04-29 08:16:19.000000 cloud_pak_operations_cli-0.7.2/cpo/lib/openshift/openshift_install/openshift_installation_manager.py
+-rw-r--r--   0 runner    (1001) docker     (127)      751 2024-04-29 08:16:19.000000 cloud_pak_operations_cli-0.7.2/cpo/lib/openshift/openshift_install/openshift_installation_manager_plugin.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 08:16:33.973149 cloud_pak_operations_cli-0.7.2/cpo/lib/openshift/openshift_install/types/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-29 08:16:19.000000 cloud_pak_operations_cli-0.7.2/cpo/lib/openshift/openshift_install/types/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      664 2024-04-29 08:16:19.000000 cloud_pak_operations_cli-0.7.2/cpo/lib/openshift/openshift_install/types/architecture.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 08:16:33.977149 cloud_pak_operations_cli-0.7.2/cpo/lib/openshift/types/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-29 08:16:19.000000 cloud_pak_operations_cli-0.7.2/cpo/lib/openshift/types/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      725 2024-04-29 08:16:19.000000 cloud_pak_operations_cli-0.7.2/cpo/lib/openshift/types/auths_dict.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1456 2024-04-29 08:16:19.000000 cloud_pak_operations_cli-0.7.2/cpo/lib/openshift/types/catalog_source.py
+-rw-r--r--   0 runner    (1001) docker     (127)      688 2024-04-29 08:16:19.000000 cloud_pak_operations_cli-0.7.2/cpo/lib/openshift/types/credentials.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1226 2024-04-29 08:16:19.000000 cloud_pak_operations_cli-0.7.2/cpo/lib/openshift/types/custom_resource.py
+-rw-r--r--   0 runner    (1001) docker     (127)      723 2024-04-29 08:16:19.000000 cloud_pak_operations_cli-0.7.2/cpo/lib/openshift/types/custom_resource_event_result.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1794 2024-04-29 08:16:19.000000 cloud_pak_operations_cli-0.7.2/cpo/lib/openshift/types/get_pod_entry.py
+-rw-r--r--   0 runner    (1001) docker     (127)      715 2024-04-29 08:16:19.000000 cloud_pak_operations_cli-0.7.2/cpo/lib/openshift/types/kind_metadata.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1017 2024-04-29 08:16:19.000000 cloud_pak_operations_cli-0.7.2/cpo/lib/openshift/types/object_meta.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1073 2024-04-29 08:16:19.000000 cloud_pak_operations_cli-0.7.2/cpo/lib/openshift/types/operator_group.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1195 2024-04-29 08:16:19.000000 cloud_pak_operations_cli-0.7.2/cpo/lib/openshift/types/role.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1391 2024-04-29 08:16:19.000000 cloud_pak_operations_cli-0.7.2/cpo/lib/openshift/types/role_binding.py
+-rw-r--r--   0 runner    (1001) docker     (127)      763 2024-04-29 08:16:19.000000 cloud_pak_operations_cli-0.7.2/cpo/lib/openshift/types/role_rule.py
+-rw-r--r--   0 runner    (1001) docker     (127)      937 2024-04-29 08:16:19.000000 cloud_pak_operations_cli-0.7.2/cpo/lib/openshift/types/service_account.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1281 2024-04-29 08:16:19.000000 cloud_pak_operations_cli-0.7.2/cpo/lib/openshift/types/subscription.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 08:16:33.977149 cloud_pak_operations_cli-0.7.2/cpo/lib/openshift/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-29 08:16:19.000000 cloud_pak_operations_cli-0.7.2/cpo/lib/openshift/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2313 2024-04-29 08:16:19.000000 cloud_pak_operations_cli-0.7.2/cpo/lib/openshift/utils/click.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 08:16:33.977149 cloud_pak_operations_cli-0.7.2/cpo/lib/plugin_manager/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-29 08:16:19.000000 cloud_pak_operations_cli-0.7.2/cpo/lib/plugin_manager/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2831 2024-04-29 08:16:19.000000 cloud_pak_operations_cli-0.7.2/cpo/lib/plugin_manager/package_data.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5669 2024-04-29 08:16:19.000000 cloud_pak_operations_cli-0.7.2/cpo/lib/plugin_manager/plugin_manager.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 08:16:33.977149 cloud_pak_operations_cli-0.7.2/cpo/scripts/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-29 08:16:19.000000 cloud_pak_operations_cli-0.7.2/cpo/scripts/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1336 2024-04-29 08:16:19.000000 cloud_pak_operations_cli-0.7.2/cpo/scripts/get_current_cluster_alias.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 08:16:33.981149 cloud_pak_operations_cli-0.7.2/cpo/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-29 08:16:19.000000 cloud_pak_operations_cli-0.7.2/cpo/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7923 2024-04-29 08:16:19.000000 cloud_pak_operations_cli-0.7.2/cpo/utils/compression.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1029 2024-04-29 08:16:19.000000 cloud_pak_operations_cli-0.7.2/cpo/utils/debugger.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4773 2024-04-29 08:16:19.000000 cloud_pak_operations_cli-0.7.2/cpo/utils/download.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3472 2024-04-29 08:16:19.000000 cloud_pak_operations_cli-0.7.2/cpo/utils/error.py
+-rw-r--r--   0 runner    (1001) docker     (127)      960 2024-04-29 08:16:19.000000 cloud_pak_operations_cli-0.7.2/cpo/utils/file.py
+-rw-r--r--   0 runner    (1001) docker     (127)      819 2024-04-29 08:16:19.000000 cloud_pak_operations_cli-0.7.2/cpo/utils/http_method.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2558 2024-04-29 08:16:19.000000 cloud_pak_operations_cli-0.7.2/cpo/utils/importlib.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6673 2024-04-29 08:16:19.000000 cloud_pak_operations_cli-0.7.2/cpo/utils/logging.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4301 2024-04-29 08:16:19.000000 cloud_pak_operations_cli-0.7.2/cpo/utils/network.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1524 2024-04-29 08:16:19.000000 cloud_pak_operations_cli-0.7.2/cpo/utils/operating_system.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6422 2024-04-29 08:16:19.000000 cloud_pak_operations_cli-0.7.2/cpo/utils/process.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6485 2024-04-29 08:16:19.000000 cloud_pak_operations_cli-0.7.2/cpo/utils/ssh.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1396 2024-04-29 08:16:19.000000 cloud_pak_operations_cli-0.7.2/cpo/utils/wait.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1340 2024-04-29 08:16:19.000000 cloud_pak_operations_cli-0.7.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-29 08:16:33.981149 cloud_pak_operations_cli-0.7.2/setup.cfg
```

### Comparing `cloud-pak-operations-cli-0.7.1/LICENSE` & `cloud_pak_operations_cli-0.7.2/LICENSE`

 * *Files identical despite different names*

### Comparing `cloud-pak-operations-cli-0.7.1/PKG-INFO` & `cloud_pak_operations_cli-0.7.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cloud-pak-operations-cli
-Version: 0.7.1
+Version: 0.7.2
 Summary: IBM Cloud Pak Operations CLI
 Author-email: IBM Corporation <db2datagate@ibm.com>
 Project-URL: repository, https://github.com/IBM/cloud-pak-operations-cli
 Classifier: Development Status :: 4 - Beta
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: MacOS
 Classifier: Operating System :: Microsoft :: Windows
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: cloud-pak-operations-cli Version: 0.7.1 Summary:
+Metadata-Version: 2.1 Name: cloud-pak-operations-cli Version: 0.7.2 Summary:
 IBM Cloud Pak Operations CLI Author-email: IBM Corporation
 ibm.com> Project-URL: repository, https://github.com/IBM/cloud-pak-operations-
 cli Classifier: Development Status :: 4 - Beta Classifier: License :: OSI
 Approved :: Apache Software License Classifier: Operating System :: MacOS
 Classifier: Operating System :: Microsoft :: Windows Classifier: Operating
 System :: POSIX :: Linux Classifier: Programming Language :: Python :: 3.10
 Requires-Python: >=3.10 Description-Content-Type: text/markdown License-File:
```

### Comparing `cloud-pak-operations-cli-0.7.1/README.md` & `cloud_pak_operations_cli-0.7.2/README.md`

 * *Files identical despite different names*

### Comparing `cloud-pak-operations-cli-0.7.1/cloud_pak_operations_cli.egg-info/PKG-INFO` & `cloud_pak_operations_cli-0.7.2/cloud_pak_operations_cli.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cloud-pak-operations-cli
-Version: 0.7.1
+Version: 0.7.2
 Summary: IBM Cloud Pak Operations CLI
 Author-email: IBM Corporation <db2datagate@ibm.com>
 Project-URL: repository, https://github.com/IBM/cloud-pak-operations-cli
 Classifier: Development Status :: 4 - Beta
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: MacOS
 Classifier: Operating System :: Microsoft :: Windows
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: cloud-pak-operations-cli Version: 0.7.1 Summary:
+Metadata-Version: 2.1 Name: cloud-pak-operations-cli Version: 0.7.2 Summary:
 IBM Cloud Pak Operations CLI Author-email: IBM Corporation
 ibm.com> Project-URL: repository, https://github.com/IBM/cloud-pak-operations-
 cli Classifier: Development Status :: 4 - Beta Classifier: License :: OSI
 Approved :: Apache Software License Classifier: Operating System :: MacOS
 Classifier: Operating System :: Microsoft :: Windows Classifier: Operating
 System :: POSIX :: Linux Classifier: Programming Language :: Python :: 3.10
 Requires-Python: >=3.10 Description-Content-Type: text/markdown License-File:
```

### Comparing `cloud-pak-operations-cli-0.7.1/cloud_pak_operations_cli.egg-info/SOURCES.txt` & `cloud_pak_operations_cli-0.7.2/cloud_pak_operations_cli.egg-info/SOURCES.txt`

 * *Files 3% similar despite different names*

```diff
@@ -10,39 +10,40 @@
 cloud_pak_operations_cli.egg-info/top_level.txt
 cpo/__init__.py
 cpo/cpo.py
 cpo/commands/__init__.py
 cpo/commands/adm/__init__.py
 cpo/commands/adm/download_dependencies.py
 cpo/commands/adm/get-shell-completion-script-location.py
+cpo/commands/adm/set_config_option.py
 cpo/commands/adm/store_credentials.py
 cpo/commands/adm/update_dev.py
-cpo/commands/adm/config/__init__.py
-cpo/commands/adm/config/set.py
 cpo/commands/adm/ibm_internal_plugin/__init__.py
 cpo/commands/adm/ibm_internal_plugin/install.py
 cpo/commands/adm/ibm_internal_plugin/ls.py
 cpo/commands/adm/ibm_internal_plugin/upgrade_plugins.py
 cpo/commands/cluster/__init__.py
 cpo/commands/cluster/add.py
 cpo/commands/cluster/current.py
-cpo/commands/cluster/delete_terminated_pods.py
 cpo/commands/cluster/edit.py
 cpo/commands/cluster/get_cluster_access_token.py
-cpo/commands/cluster/install_nfs_storage_class.py
-cpo/commands/cluster/install_odf_storage_classes.py
 cpo/commands/cluster/login.py
 cpo/commands/cluster/ls.py
 cpo/commands/cluster/reset_current_cluster.py
 cpo/commands/cluster/rm.py
 cpo/commands/cluster/use.py
+cpo/commands/cluster/pods/__init__.py
+cpo/commands/cluster/pods/delete_terminated_pods.py
 cpo/commands/cluster/pull_secret/__init__.py
 cpo/commands/cluster/pull_secret/ls.py
 cpo/commands/cluster/pull_secret/rm.py
 cpo/commands/cluster/pull_secret/set.py
+cpo/commands/cluster/storage/__init__.py
+cpo/commands/cluster/storage/install_kubernetes_nfs_subdir_external_provisioner.py
+cpo/commands/cluster/storage/install_openshift_data_foundation.py
 cpo/commands/ibmcloud/__init__.py
 cpo/commands/ibmcloud/login.py
 cpo/commands/ibmcloud/logout.py
 cpo/commands/ibmcloud/regenerate_api_key.py
 cpo/commands/ibmcloud/oc/__init__.py
 cpo/commands/ibmcloud/oc/cluster/__init__.py
 cpo/commands/ibmcloud/oc/cluster/add.py
```

### Comparing `cloud-pak-operations-cli-0.7.1/cpo/__init__.py` & `cloud_pak_operations_cli-0.7.2/cpo/__init__.py`

 * *Files identical despite different names*

### Comparing `cloud-pak-operations-cli-0.7.1/cpo/commands/adm/__init__.py` & `cloud_pak_operations_cli-0.7.2/cpo/commands/adm/__init__.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,15 +1,15 @@
-#  Copyright 2021, 2022 IBM Corporation
+#  Copyright 2021, 2024 IBM Corporation
 #
 #  Licensed under the Apache License, Version 2.0 (the "License");
 #  you may not use this file except in compliance with the License.
 #  You may obtain a copy of the License at
 #
 #  http://www.apache.org/licenses/LICENSE-2.0
 #
 #  Unless required by applicable law or agreed to in writing, software
 #  distributed under the License is distributed on an "AS IS" BASIS,
 #  WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 #  See the License for the specific language governing permissions and
 #  limitations under the License.
 
-__doc__ = "CLI administration commands"
+__doc__ = "Commands to administer the CLI"
```

### Comparing `cloud-pak-operations-cli-0.7.1/cpo/commands/adm/config/__init__.py` & `cloud_pak_operations_cli-0.7.2/cpo/commands/adm/ibm_internal_plugin/__init__.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,15 +1,15 @@
-#  Copyright 2021 IBM Corporation
+#  Copyright 2022, 2024 IBM Corporation
 #
 #  Licensed under the Apache License, Version 2.0 (the "License");
 #  you may not use this file except in compliance with the License.
 #  You may obtain a copy of the License at
 #
 #  http://www.apache.org/licenses/LICENSE-2.0
 #
 #  Unless required by applicable law or agreed to in writing, software
 #  distributed under the License is distributed on an "AS IS" BASIS,
 #  WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 #  See the License for the specific language governing permissions and
 #  limitations under the License.
 
-__doc__ = "Modify the CLI configuration"
+__doc__ = "Commands to administer IBM-internal CLI plug-ins"
```

### Comparing `cloud-pak-operations-cli-0.7.1/cpo/commands/adm/config/set.py` & `cloud_pak_operations_cli-0.7.2/cpo/commands/adm/set_config_option.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-#  Copyright 2021 IBM Corporation
+#  Copyright 2024 IBM Corporation
 #
 #  Licensed under the Apache License, Version 2.0 (the "License");
 #  you may not use this file except in compliance with the License.
 #  You may obtain a copy of the License at
 #
 #  http://www.apache.org/licenses/LICENSE-2.0
 #
@@ -18,11 +18,11 @@
 
 from cpo.utils.logging import loglevel_command
 
 
 @loglevel_command()
 @click.option("--key", help="Key name which should be set", required=True)
 @click.option("--value", help="Value to which key should be set", required=True)
-def set(key: str, value: str):
-    """Set configuration value"""
+def set_config_option(key: str, value: str):
+    """Set configuration option"""
 
     cpo.config.configuration_manager.set_bool_config_value(key, value)
```

### Comparing `cloud-pak-operations-cli-0.7.1/cpo/commands/adm/download_dependencies.py` & `cloud_pak_operations_cli-0.7.2/cpo/commands/adm/download_dependencies.py`

 * *Files identical despite different names*

### Comparing `cloud-pak-operations-cli-0.7.1/cpo/commands/adm/get-shell-completion-script-location.py` & `cloud_pak_operations_cli-0.7.2/cpo/commands/adm/get-shell-completion-script-location.py`

 * *Files identical despite different names*

### Comparing `cloud-pak-operations-cli-0.7.1/cpo/commands/adm/ibm_internal_plugin/__init__.py` & `cloud_pak_operations_cli-0.7.2/cpo/commands/cluster/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,15 +1,15 @@
-#  Copyright 2022 IBM Corporation
+#  Copyright 2021, 2024 IBM Corporation
 #
 #  Licensed under the Apache License, Version 2.0 (the "License");
 #  you may not use this file except in compliance with the License.
 #  You may obtain a copy of the License at
 #
 #  http://www.apache.org/licenses/LICENSE-2.0
 #
 #  Unless required by applicable law or agreed to in writing, software
 #  distributed under the License is distributed on an "AS IS" BASIS,
 #  WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 #  See the License for the specific language governing permissions and
 #  limitations under the License.
 
-__doc__ = "IBM-internal CLI plug-in administration commands"
+__doc__ = "Commands to manage clusters"
```

### Comparing `cloud-pak-operations-cli-0.7.1/cpo/commands/adm/ibm_internal_plugin/install.py` & `cloud_pak_operations_cli-0.7.2/cpo/commands/adm/ibm_internal_plugin/install.py`

 * *Files identical despite different names*

### Comparing `cloud-pak-operations-cli-0.7.1/cpo/commands/adm/ibm_internal_plugin/ls.py` & `cloud_pak_operations_cli-0.7.2/cpo/commands/adm/ibm_internal_plugin/ls.py`

 * *Files identical despite different names*

### Comparing `cloud-pak-operations-cli-0.7.1/cpo/commands/adm/ibm_internal_plugin/upgrade_plugins.py` & `cloud_pak_operations_cli-0.7.2/cpo/commands/adm/ibm_internal_plugin/upgrade_plugins.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-#  Copyright 2023 IBM Corporation
+#  Copyright 2023, 2024 IBM Corporation
 #
 #  Licensed under the Apache License, Version 2.0 (the "License");
 #  you may not use this file except in compliance with the License.
 #  You may obtain a copy of the License at
 #
 #  http://www.apache.org/licenses/LICENSE-2.0
 #
@@ -43,19 +43,17 @@
     required=True,
 )
 @click.option(
     "--repository-url",
     default="https://na.artifactory.swg-devops.com/artifactory/api/pypi/hyc-ibm-sap-cp4d-team-pypi-local/simple",
 )
 @click.option("--user", help="Install to user site-packages directory", is_flag=True)
-@click.argument("distribution-package-names", nargs=-1)
 def upgrade_plugins(
     artifactory_username: str,
     artifactory_password: str,
-    distribution_package_names: list[str],
     repository_url: str,
     user: bool,
 ):
     """Upgrade IBM-internal CLI plug-ins"""
 
     ibm_internal_plugin_installer = IBMInternalPluginInstaller(
         artifactory_username, artifactory_password, repository_url
```

### Comparing `cloud-pak-operations-cli-0.7.1/cpo/commands/adm/store_credentials.py` & `cloud_pak_operations_cli-0.7.2/cpo/commands/adm/store_credentials.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,23 +1,21 @@
-#  Copyright 2021, 2022 IBM Corporation
+#  Copyright 2021, 2024 IBM Corporation
 #
 #  Licensed under the Apache License, Version 2.0 (the "License");
 #  you may not use this file except in compliance with the License.
 #  You may obtain a copy of the License at
 #
 #  http://www.apache.org/licenses/LICENSE-2.0
 #
 #  Unless required by applicable law or agreed to in writing, software
 #  distributed under the License is distributed on an "AS IS" BASIS,
 #  WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 #  See the License for the specific language governing permissions and
 #  limitations under the License.
 
-from typing import Optional
-
 import click
 
 import cpo.config
 
 from cpo.utils.logging import loglevel_command
 
 
@@ -25,16 +23,19 @@
 @click.option("--artifactory-password", help="Artifactory password")
 @click.option("--artifactory-username", help="Artifactory username")
 @click.option(
     "--ibm-cloud-pak-for-data-entitlement-key",
     help="IBM Cloud Pak for Data entitlement key (see https://myibm.ibm.com/products-services/containerlibrary)",
 )
 def store_credentials(
-    artifactory_password: Optional[str],
-    artifactory_username: Optional[str],
-    ibm_cloud_pak_for_data_entitlement_key: Optional[str],
+    artifactory_password: str | None,
+    artifactory_username: str | None,
+    ibm_cloud_pak_for_data_entitlement_key: str | None,
 ):
-    """Store credentials in a configuration file"""
+    """Store credentials
+
+    Credentials are stored in ~/.cpo/credentials.json.
+    """
 
     credentials_to_be_stored = locals().copy()
 
     cpo.config.configuration_manager.store_credentials(credentials_to_be_stored)
```

### Comparing `cloud-pak-operations-cli-0.7.1/cpo/commands/adm/update_dev.py` & `cloud_pak_operations_cli-0.7.2/cpo/commands/adm/update_dev.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-#  Copyright 2021, 2022 IBM Corporation
+#  Copyright 2021, 2024 IBM Corporation
 #
 #  Licensed under the Apache License, Version 2.0 (the "License");
 #  you may not use this file except in compliance with the License.
 #  You may obtain a copy of the License at
 #
 #  http://www.apache.org/licenses/LICENSE-2.0
 #
@@ -20,19 +20,19 @@
 from cpo import distribution_package_name
 from cpo.utils.error import CloudPakOperationsCLIException
 from cpo.utils.logging import loglevel_command
 
 
 @loglevel_command()
 def update_dev():
-    """Update the CLI to the latest development version"""
+    """Update the CLI to the latest development code"""
 
     if metadata.version(distribution_package_name) != "0.0.1":
         raise CloudPakOperationsCLIException(
-            f"Current version is not a development version (use 'pip3 install --upgrade {distribution_package_name}' "
+            f"Current version is not a development version (use 'pip install --upgrade {distribution_package_name}' "
             f"to upgrade a release version)"
         )
 
     search_result = regex.search("https://(.*)", metadata.metadata(distribution_package_name)["Download-URL"])
 
     if search_result is not None:
         git_hub_url_without_scheme = search_result.group(1)
```

### Comparing `cloud-pak-operations-cli-0.7.1/cpo/commands/cluster/__init__.py` & `cloud_pak_operations_cli-0.7.2/cpo/commands/cluster/pods/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,15 +1,15 @@
-#  Copyright 2021, 2023 IBM Corporation
+#  Copyright 2024 IBM Corporation
 #
 #  Licensed under the Apache License, Version 2.0 (the "License");
 #  you may not use this file except in compliance with the License.
 #  You may obtain a copy of the License at
 #
 #  http://www.apache.org/licenses/LICENSE-2.0
 #
 #  Unless required by applicable law or agreed to in writing, software
 #  distributed under the License is distributed on an "AS IS" BASIS,
 #  WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 #  See the License for the specific language governing permissions and
 #  limitations under the License.
 
-__doc__ = "Cluster management commands"
+__doc__ = "Commands to manage pods"
```

### Comparing `cloud-pak-operations-cli-0.7.1/cpo/commands/cluster/add.py` & `cloud_pak_operations_cli-0.7.2/cpo/commands/cluster/add.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,22 +1,22 @@
-#  Copyright 2022, 2023 IBM Corporation
+#  Copyright 2022, 2024 IBM Corporation
 #
 #  Licensed under the Apache License, Version 2.0 (the "License");
 #  you may not use this file except in compliance with the License.
 #  You may obtain a copy of the License at
 #
 #  http://www.apache.org/licenses/LICENSE-2.0
 #
 #  Unless required by applicable law or agreed to in writing, software
 #  distributed under the License is distributed on an "AS IS" BASIS,
 #  WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 #  See the License for the specific language governing permissions and
 #  limitations under the License.
 
-from typing import Any, Optional
+from typing import Any
 
 import click
 
 import cpo.config.cluster_credentials_manager
 import cpo.lib.openshift.cluster
 
 from cpo.utils.logging import loglevel_command
@@ -29,15 +29,15 @@
 @click.option("--password", help="OpenShift password", required=True)
 @click.option(
     "--insecure-skip-tls-verify",
     default=None,
     help="Skips checking the server's certificate for validity",
     is_flag=True,
 )
-def add(server: str, alias: Optional[str], username: str, password: str, insecure_skip_tls_verify: Optional[bool]):
+def add(server: str, alias: str | None, username: str, password: str, insecure_skip_tls_verify: bool | None):
     """Register an existing Red Hat OpenShift cluster"""
 
     data: dict[str, Any] = {
         "username": username,
         "password": password,
     }
```

### Comparing `cloud-pak-operations-cli-0.7.1/cpo/commands/cluster/current.py` & `cloud_pak_operations_cli-0.7.2/cpo/commands/cluster/current.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,35 +1,33 @@
-#  Copyright 2021, 2023 IBM Corporation
+#  Copyright 2021, 2024 IBM Corporation
 #
 #  Licensed under the Apache License, Version 2.0 (the "License");
 #  you may not use this file except in compliance with the License.
 #  You may obtain a copy of the License at
 #
 #  http://www.apache.org/licenses/LICENSE-2.0
 #
 #  Unless required by applicable law or agreed to in writing, software
 #  distributed under the License is distributed on an "AS IS" BASIS,
 #  WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 #  See the License for the specific language governing permissions and
 #  limitations under the License.
 
-from typing import Optional
-
 import click
 
 import cpo.config.cluster_credentials_manager
 
 from cpo.utils.logging import loglevel_command
 
 
 @loglevel_command()
 @click.option(
     "--print-alias", help="Print the alias used to reference a cluster instead of its server URL", is_flag=True
 )
-def current(print_alias: Optional[bool]):
+def current(print_alias: bool | None):
     """Get the current registered OpenShift cluster"""
 
     current_cluster = cpo.config.cluster_credentials_manager.cluster_credentials_manager.get_current_cluster()
 
     if current_cluster is not None:
         if not print_alias:
             click.echo(current_cluster.get_server())
```

### Comparing `cloud-pak-operations-cli-0.7.1/cpo/commands/cluster/delete_terminated_pods.py` & `cloud_pak_operations_cli-0.7.2/cpo/commands/cluster/storage/install_openshift_data_foundation.py`

 * *Files 18% similar despite different names*

```diff
@@ -8,41 +8,47 @@
 #
 #  Unless required by applicable law or agreed to in writing, software
 #  distributed under the License is distributed on an "AS IS" BASIS,
 #  WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 #  See the License for the specific language governing permissions and
 #  limitations under the License.
 
-from typing import Optional
-
 import click
 
 import cpo.config.cluster_credentials_manager
 import cpo.lib.click.utils
 import cpo.utils.network
 
 from cpo.lib.ansible.openshift_playbook_runner import OpenShiftPlaybookRunner
+from cpo.lib.openshift.openshift_api_manager import OpenShiftAPIManager
 from cpo.lib.openshift.utils.click import openshift_server_options
 from cpo.utils.logging import loglevel_command
 
 
 @loglevel_command(
     context_settings=cpo.lib.click.utils.create_default_map_from_dict(
         cpo.config.cluster_credentials_manager.cluster_credentials_manager.get_current_credentials()
     )
 )
 @openshift_server_options
 @click.pass_context
-def delete_terminated_pods(
+def install_odf_storage_classes(
     ctx: click.Context,
-    server: Optional[str],
-    username: Optional[str],
-    password: Optional[str],
-    token: Optional[str],
-    insecure_skip_tls_verify: Optional[bool],
-    use_cluster: Optional[str],
+    server: str | None,
+    username: str | None,
+    password: str | None,
+    token: str | None,
+    insecure_skip_tls_verify: bool | None,
+    use_cluster: str | None,
 ):
-    """Delete terminated pods"""
+    """Install Red Hat OpenShift Data Foundation (ODF)"""
 
     credentials = cpo.lib.click.utils.get_cluster_credentials(ctx, locals().copy())
+    version = OpenShiftAPIManager(credentials).get_version()
 
-    OpenShiftPlaybookRunner("delete_terminated_pods_playbook.yaml", credentials).run_playbook()
+    OpenShiftPlaybookRunner(
+        "deploy_odf_playbook.yaml",
+        credentials,
+        variables={
+            "openshift_server_version": f"{version.major}.{version.minor}",
+        },
+    ).run_playbook()
```

### Comparing `cloud-pak-operations-cli-0.7.1/cpo/commands/cluster/edit.py` & `cloud_pak_operations_cli-0.7.2/cpo/commands/cluster/edit.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,23 +1,21 @@
-#  Copyright 2021, 2023 IBM Corporation
+#  Copyright 2021, 2024 IBM Corporation
 #
 #  Licensed under the Apache License, Version 2.0 (the "License");
 #  you may not use this file except in compliance with the License.
 #  You may obtain a copy of the License at
 #
 #  http://www.apache.org/licenses/LICENSE-2.0
 #
 #  Unless required by applicable law or agreed to in writing, software
 #  distributed under the License is distributed on an "AS IS" BASIS,
 #  WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 #  See the License for the specific language governing permissions and
 #  limitations under the License.
 
-from typing import Optional
-
 import click
 
 import cpo.config.cluster_credentials_manager
 
 from cpo.utils.logging import loglevel_command
 
 
@@ -30,18 +28,18 @@
     "--insecure-skip-tls-verify/--no-insecure-skip-tls-verify",
     default=None,
     help="Disables or enables checking the server's certificate for validity",
     is_flag=True,
 )
 def edit(
     alias_or_server: str,
-    alias: Optional[str],
-    username: Optional[str],
-    password: Optional[str],
-    insecure_skip_tls_verify: Optional[bool],
+    alias: str | None,
+    username: str | None,
+    password: str | None,
+    insecure_skip_tls_verify: bool | None,
 ):
     """Edit metadata of a registered OpenShift cluster"""
 
     metadata_to_be_edited = locals().copy()
     metadata_to_be_edited.pop("alias_or_server")
 
     if all(value is None for value in metadata_to_be_edited.values()):
```

### Comparing `cloud-pak-operations-cli-0.7.1/cpo/commands/cluster/get_cluster_access_token.py` & `cloud_pak_operations_cli-0.7.2/cpo/commands/cluster/get_cluster_access_token.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,23 +1,21 @@
-#  Copyright 2021 IBM Corporation
+#  Copyright 2021, 2024 IBM Corporation
 #
 #  Licensed under the Apache License, Version 2.0 (the "License");
 #  you may not use this file except in compliance with the License.
 #  You may obtain a copy of the License at
 #
 #  http://www.apache.org/licenses/LICENSE-2.0
 #
 #  Unless required by applicable law or agreed to in writing, software
 #  distributed under the License is distributed on an "AS IS" BASIS,
 #  WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 #  See the License for the specific language governing permissions and
 #  limitations under the License.
 
-from typing import Optional
-
 import click
 
 import cpo.config.cluster_credentials_manager
 import cpo.lib.click.utils
 import cpo.utils.network
 
 from cpo.utils.logging import loglevel_command
@@ -29,17 +27,17 @@
 @click.option("--password", help="OpenShift cluster password")
 @click.option(
     "--print-login-command", help="Print oc login command instead of just the OAuth access token", is_flag=True
 )
 @click.pass_context
 def get_cluster_access_token(
     ctx: click.Context,
-    server: Optional[str],
-    username: Optional[str],
-    password: Optional[str],
+    server: str | None,
+    username: str | None,
+    password: str | None,
     print_login_command: bool,
 ):
     """Obtain an OAuth access token for an OpenShift cluster"""
 
     cpo.utils.network.disable_insecure_request_warning()
 
     credentials = cpo.lib.click.utils.get_cluster_credentials(ctx, locals().copy())
```

### Comparing `cloud-pak-operations-cli-0.7.1/cpo/commands/cluster/install_nfs_storage_class.py` & `cloud_pak_operations_cli-0.7.2/cpo/commands/cluster/storage/install_kubernetes_nfs_subdir_external_provisioner.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,23 +1,21 @@
-#  Copyright 2021, 2023 IBM Corporation
+#  Copyright 2024 IBM Corporation
 #
 #  Licensed under the Apache License, Version 2.0 (the "License");
 #  you may not use this file except in compliance with the License.
 #  You may obtain a copy of the License at
 #
 #  http://www.apache.org/licenses/LICENSE-2.0
 #
 #  Unless required by applicable law or agreed to in writing, software
 #  distributed under the License is distributed on an "AS IS" BASIS,
 #  WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 #  See the License for the specific language governing permissions and
 #  limitations under the License.
 
-from typing import Optional
-
 import click
 
 import cpo.config.cluster_credentials_manager
 import cpo.lib.click.utils
 import cpo.utils.network
 
 from cpo.lib.openshift.nfs.nfs_subdir_external_provisioner import NFSSubdirExternalProvisioner
@@ -38,22 +36,22 @@
     default="default",
     help="Project used to install the Kubernetes NFS Subdir External Provisioner",
     show_default=True,
 )
 @click.pass_context
 def install_nfs_storage_class(
     ctx: click.Context,
-    server: Optional[str],
-    username: Optional[str],
-    password: Optional[str],
-    token: Optional[str],
-    insecure_skip_tls_verify: Optional[bool],
-    use_cluster: Optional[str],
+    server: str | None,
+    username: str | None,
+    password: str | None,
+    token: str | None,
+    insecure_skip_tls_verify: bool | None,
+    use_cluster: str | None,
     nfs_path: str,
     nfs_server: str,
     project: str,
 ):
-    """Install NFS storage class"""
+    """Install Kubernetes NFS Subdir External Provisioner"""
 
     NFSSubdirExternalProvisioner(
         cpo.lib.click.utils.get_cluster_credentials(ctx, locals().copy()), project, nfs_server, nfs_path
     ).install_nfs_subdir_external_provisioner()
```

### Comparing `cloud-pak-operations-cli-0.7.1/cpo/commands/cluster/install_odf_storage_classes.py` & `cloud_pak_operations_cli-0.7.2/cpo/commands/cluster/pull_secret/rm.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,56 +1,43 @@
-#  Copyright 2022, 2024 IBM Corporation
+#  Copyright 2021, 2024 IBM Corporation
 #
 #  Licensed under the Apache License, Version 2.0 (the "License");
 #  you may not use this file except in compliance with the License.
 #  You may obtain a copy of the License at
 #
 #  http://www.apache.org/licenses/LICENSE-2.0
 #
 #  Unless required by applicable law or agreed to in writing, software
 #  distributed under the License is distributed on an "AS IS" BASIS,
 #  WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 #  See the License for the specific language governing permissions and
 #  limitations under the License.
 
-from typing import Optional
-
 import click
 
 import cpo.config.cluster_credentials_manager
 import cpo.lib.click.utils
-import cpo.utils.network
 
-from cpo.lib.ansible.openshift_playbook_runner import OpenShiftPlaybookRunner
 from cpo.lib.openshift.openshift_api_manager import OpenShiftAPIManager
 from cpo.lib.openshift.utils.click import openshift_server_options
 from cpo.utils.logging import loglevel_command
 
 
-@loglevel_command(
-    context_settings=cpo.lib.click.utils.create_default_map_from_dict(
-        cpo.config.cluster_credentials_manager.cluster_credentials_manager.get_current_credentials()
-    )
-)
+@loglevel_command()
 @openshift_server_options
+@click.option("--registry-location", help="Container registry location", required=True)
 @click.pass_context
-def install_odf_storage_classes(
+def rm(
     ctx: click.Context,
-    server: Optional[str],
-    username: Optional[str],
-    password: Optional[str],
-    token: Optional[str],
-    insecure_skip_tls_verify: Optional[bool],
-    use_cluster: Optional[str],
+    server: str | None,
+    username: str | None,
+    password: str | None,
+    token: str | None,
+    insecure_skip_tls_verify: bool | None,
+    use_cluster: str | None,
+    registry_location: str,
 ):
-    """Install Red Hat OpenShift Data Foundation (ODF) storage classes"""
+    """Remove registry credentials from the global pull secret"""
 
-    credentials = cpo.lib.click.utils.get_cluster_credentials(ctx, locals().copy())
-    version = OpenShiftAPIManager(credentials).get_version()
-
-    OpenShiftPlaybookRunner(
-        "deploy_odf_playbook.yaml",
-        credentials,
-        variables={
-            "openshift_server_version": f"{version.major}.{version.minor}",
-        },
-    ).run_playbook()
+    OpenShiftAPIManager(cpo.lib.click.utils.get_cluster_credentials(ctx, locals().copy())).delete_credentials(
+        registry_location
+    )
```

### Comparing `cloud-pak-operations-cli-0.7.1/cpo/commands/cluster/login.py` & `cloud_pak_operations_cli-0.7.2/cpo/commands/cluster/login.py`

 * *Files identical despite different names*

### Comparing `cloud-pak-operations-cli-0.7.1/cpo/commands/cluster/ls.py` & `cloud_pak_operations_cli-0.7.2/cpo/commands/cluster/ls.py`

 * *Files identical despite different names*

### Comparing `cloud-pak-operations-cli-0.7.1/cpo/commands/cluster/pull_secret/__init__.py` & `cloud_pak_operations_cli-0.7.2/cpo/commands/cluster/pull_secret/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,15 @@
-#  Copyright 2021 IBM Corporation
+#  Copyright 2021, 2024 IBM Corporation
 #
 #  Licensed under the Apache License, Version 2.0 (the "License");
 #  you may not use this file except in compliance with the License.
 #  You may obtain a copy of the License at
 #
 #  http://www.apache.org/licenses/LICENSE-2.0
 #
 #  Unless required by applicable law or agreed to in writing, software
 #  distributed under the License is distributed on an "AS IS" BASIS,
 #  WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 #  See the License for the specific language governing permissions and
 #  limitations under the License.
 
-__doc__ = "Commands for managing the global pull secret"
+__doc__ = "Commands to manage the global pull secret"
```

### Comparing `cloud-pak-operations-cli-0.7.1/cpo/commands/cluster/pull_secret/ls.py` & `cloud_pak_operations_cli-0.7.2/cpo/commands/cluster/pull_secret/ls.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,23 +1,21 @@
-#  Copyright 2021, 2023 IBM Corporation
+#  Copyright 2021, 2024 IBM Corporation
 #
 #  Licensed under the Apache License, Version 2.0 (the "License");
 #  you may not use this file except in compliance with the License.
 #  You may obtain a copy of the License at
 #
 #  http://www.apache.org/licenses/LICENSE-2.0
 #
 #  Unless required by applicable law or agreed to in writing, software
 #  distributed under the License is distributed on an "AS IS" BASIS,
 #  WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 #  See the License for the specific language governing permissions and
 #  limitations under the License.
 
-from typing import Optional
-
 import click
 
 import cpo.config.cluster_credentials_manager
 import cpo.lib.click.utils
 
 from cpo.lib.openshift.openshift_api_manager import OpenShiftAPIManager
 from cpo.lib.openshift.utils.click import openshift_server_options
@@ -26,20 +24,20 @@
 
 @loglevel_command(default_log_level="WARNING")
 @openshift_server_options
 @click.option("--json", help="Prints the command output in JSON format", is_flag=True)
 @click.pass_context
 def ls(
     ctx: click.Context,
-    server: Optional[str],
-    username: Optional[str],
-    password: Optional[str],
-    token: Optional[str],
-    insecure_skip_tls_verify: Optional[bool],
-    use_cluster: Optional[str],
+    server: str | None,
+    username: str | None,
+    password: str | None,
+    token: str | None,
+    insecure_skip_tls_verify: bool | None,
+    use_cluster: str | None,
     json: bool,
 ):
     """List registry credentials stored in the global pull secret"""
 
     OpenShiftAPIManager(
         cpo.lib.click.utils.get_cluster_credentials(ctx, locals().copy())
     ).get_global_pull_secret_data().format(json)
```

### Comparing `cloud-pak-operations-cli-0.7.1/cpo/commands/cluster/pull_secret/rm.py` & `cloud_pak_operations_cli-0.7.2/cpo/commands/cluster/pull_secret/set.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,45 +1,47 @@
-#  Copyright 2021, 2023 IBM Corporation
+#  Copyright 2021, 2024 IBM Corporation
 #
 #  Licensed under the Apache License, Version 2.0 (the "License");
 #  you may not use this file except in compliance with the License.
 #  You may obtain a copy of the License at
 #
 #  http://www.apache.org/licenses/LICENSE-2.0
 #
 #  Unless required by applicable law or agreed to in writing, software
 #  distributed under the License is distributed on an "AS IS" BASIS,
 #  WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 #  See the License for the specific language governing permissions and
 #  limitations under the License.
 
-from typing import Optional
-
 import click
 
 import cpo.config.cluster_credentials_manager
 import cpo.lib.click.utils
 
 from cpo.lib.openshift.openshift_api_manager import OpenShiftAPIManager
 from cpo.lib.openshift.utils.click import openshift_server_options
 from cpo.utils.logging import loglevel_command
 
 
 @loglevel_command()
 @openshift_server_options
 @click.option("--registry-location", help="Container registry location", required=True)
+@click.option("--registry-location-username", help="Container registry username", required=True)
+@click.option("--registry-location-password", help="Container registry password", required=True)
 @click.pass_context
-def rm(
+def set(
     ctx: click.Context,
-    server: Optional[str],
-    username: Optional[str],
-    password: Optional[str],
-    token: Optional[str],
-    insecure_skip_tls_verify: Optional[bool],
-    use_cluster: Optional[str],
+    server: str | None,
+    username: str | None,
+    password: str | None,
+    token: str | None,
+    insecure_skip_tls_verify: bool | None,
+    use_cluster: str | None,
     registry_location: str,
+    registry_location_username: str,
+    registry_location_password: str,
 ):
-    """Remove registry credentials from the global pull secret"""
+    """Store registry credentials in the global pull secret"""
 
-    OpenShiftAPIManager(cpo.lib.click.utils.get_cluster_credentials(ctx, locals().copy())).delete_credentials(
-        registry_location
+    OpenShiftAPIManager(cpo.lib.click.utils.get_cluster_credentials(ctx, locals().copy())).set_credentials(
+        registry_location, registry_location_username, registry_location_password
     )
```

### Comparing `cloud-pak-operations-cli-0.7.1/cpo/commands/cluster/reset_current_cluster.py` & `cloud_pak_operations_cli-0.7.2/cpo/commands/cluster/reset_current_cluster.py`

 * *Files identical despite different names*

### Comparing `cloud-pak-operations-cli-0.7.1/cpo/commands/cluster/rm.py` & `cloud_pak_operations_cli-0.7.2/cpo/commands/cluster/rm.py`

 * *Files identical despite different names*

### Comparing `cloud-pak-operations-cli-0.7.1/cpo/commands/cluster/use.py` & `cloud_pak_operations_cli-0.7.2/cpo/commands/cluster/use.py`

 * *Files identical despite different names*

### Comparing `cloud-pak-operations-cli-0.7.1/cpo/commands/ibmcloud/__init__.py` & `cloud_pak_operations_cli-0.7.2/cpo/commands/ibmcloud/__init__.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,15 +1,15 @@
-#  Copyright 2021, 2022 IBM Corporation
+#  Copyright 2021, 2024 IBM Corporation
 #
 #  Licensed under the Apache License, Version 2.0 (the "License");
 #  you may not use this file except in compliance with the License.
 #  You may obtain a copy of the License at
 #
 #  http://www.apache.org/licenses/LICENSE-2.0
 #
 #  Unless required by applicable law or agreed to in writing, software
 #  distributed under the License is distributed on an "AS IS" BASIS,
 #  WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 #  See the License for the specific language governing permissions and
 #  limitations under the License.
 
-__doc__ = "IBM Cloud-specific commands"
+__doc__ = "Commands to manage IBM Cloud resources"
```

### Comparing `cloud-pak-operations-cli-0.7.1/cpo/commands/ibmcloud/login.py` & `cloud_pak_operations_cli-0.7.2/cpo/commands/ibmcloud/login.py`

 * *Files identical despite different names*

### Comparing `cloud-pak-operations-cli-0.7.1/cpo/commands/ibmcloud/logout.py` & `cloud_pak_operations_cli-0.7.2/cpo/commands/ibmcloud/logout.py`

 * *Files identical despite different names*

### Comparing `cloud-pak-operations-cli-0.7.1/cpo/commands/ibmcloud/oc/__init__.py` & `cloud_pak_operations_cli-0.7.2/cpo/commands/cluster/storage/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,15 +1,15 @@
-#  Copyright 2021 IBM Corporation
+#  Copyright 2024 IBM Corporation
 #
 #  Licensed under the Apache License, Version 2.0 (the "License");
 #  you may not use this file except in compliance with the License.
 #  You may obtain a copy of the License at
 #
 #  http://www.apache.org/licenses/LICENSE-2.0
 #
 #  Unless required by applicable law or agreed to in writing, software
 #  distributed under the License is distributed on an "AS IS" BASIS,
 #  WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 #  See the License for the specific language governing permissions and
 #  limitations under the License.
 
-__doc__ = "Manage Red Hat OpenShift on IBM Cloud"
+__doc__ = "Commands to install storage-related OpenShift resources"
```

### Comparing `cloud-pak-operations-cli-0.7.1/cpo/commands/ibmcloud/oc/cluster/__init__.py` & `cloud_pak_operations_cli-0.7.2/cpo/utils/http_method.py`

 * *Files 16% similar despite different names*

```diff
@@ -8,8 +8,21 @@
 #
 #  Unless required by applicable law or agreed to in writing, software
 #  distributed under the License is distributed on an "AS IS" BASIS,
 #  WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 #  See the License for the specific language governing permissions and
 #  limitations under the License.
 
-__doc__ = "Manage a Red Hat OpenShift on IBM Cloud cluster"
+from enum import Enum, auto
+
+
+class HTTPMethod(Enum):
+    DELETE = auto()
+    GET = auto()
+    HEAD = auto()
+    OPTIONS = auto()
+    PATCH = auto()
+    POST = auto()
+    PUT = auto()
+
+    def __str__(self):
+        return self.name
```

### Comparing `cloud-pak-operations-cli-0.7.1/cpo/commands/ibmcloud/oc/cluster/add.py` & `cloud_pak_operations_cli-0.7.2/cpo/commands/ibmcloud/oc/cluster/add.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,38 +1,36 @@
-#  Copyright 2021, 2022 IBM Corporation
+#  Copyright 2021, 2024 IBM Corporation
 #
 #  Licensed under the Apache License, Version 2.0 (the "License");
 #  you may not use this file except in compliance with the License.
 #  You may obtain a copy of the License at
 #
 #  http://www.apache.org/licenses/LICENSE-2.0
 #
 #  Unless required by applicable law or agreed to in writing, software
 #  distributed under the License is distributed on an "AS IS" BASIS,
 #  WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 #  See the License for the specific language governing permissions and
 #  limitations under the License.
 
-from typing import Optional
-
 import click
 
 import cpo.config.cluster_credentials_manager
 import cpo.lib.ibmcloud.oc.cluster
 
 from cpo.lib.ibmcloud.ibm_cloud_api_manager import IBMCloudAPIManager
 from cpo.utils.logging import loglevel_command
 
 
 @loglevel_command()
 @click.option("--alias", help="Alias used to reference a cluster instead of its server URL")
 @click.option(
     "--cluster-name", help="Name of the Red Hat OpenShift on IBM Cloud cluster to be registered", required=True
 )
-def add(alias: Optional[str], cluster_name: str):
+def add(alias: str | None, cluster_name: str):
     """Register an existing Red Hat OpenShift on IBM Cloud cluster"""
 
     server = IBMCloudAPIManager().get_cluster_status(cluster_name).get_server_url()
 
     cpo.config.cluster_credentials_manager.cluster_credentials_manager.add_cluster(
         alias if (alias is not None) else "",
         server,
```

### Comparing `cloud-pak-operations-cli-0.7.1/cpo/commands/ibmcloud/oc/cluster/login.py` & `cloud_pak_operations_cli-0.7.2/cpo/commands/ibmcloud/oc/cluster/login.py`

 * *Files identical despite different names*

### Comparing `cloud-pak-operations-cli-0.7.1/cpo/commands/ibmcloud/oc/cluster/ls.py` & `cloud_pak_operations_cli-0.7.2/cpo/commands/ibmcloud/oc/cluster/ls.py`

 * *Files identical despite different names*

### Comparing `cloud-pak-operations-cli-0.7.1/cpo/commands/ibmcloud/oc/cluster/rm.py` & `cloud_pak_operations_cli-0.7.2/cpo/commands/ibmcloud/oc/cluster/rm.py`

 * *Files identical despite different names*

### Comparing `cloud-pak-operations-cli-0.7.1/cpo/commands/ibmcloud/oc/cluster/status.py` & `cloud_pak_operations_cli-0.7.2/cpo/commands/ibmcloud/oc/cluster/status.py`

 * *Files identical despite different names*

### Comparing `cloud-pak-operations-cli-0.7.1/cpo/commands/ibmcloud/regenerate_api_key.py` & `cloud_pak_operations_cli-0.7.2/cpo/lib/ansible/modules/custom_resource_event_result.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,24 +1,21 @@
-#  Copyright 2022 IBM Corporation
+#  Copyright 2022, 2024 IBM Corporation
 #
 #  Licensed under the Apache License, Version 2.0 (the "License");
 #  you may not use this file except in compliance with the License.
 #  You may obtain a copy of the License at
 #
 #  http://www.apache.org/licenses/LICENSE-2.0
 #
 #  Unless required by applicable law or agreed to in writing, software
 #  distributed under the License is distributed on an "AS IS" BASIS,
 #  WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 #  See the License for the specific language governing permissions and
 #  limitations under the License.
 
-from cpo.lib.ibmcloud.ibm_cloud_api_manager import IBMCloudAPIManager
-from cpo.utils.logging import loglevel_command
+from dataclasses import dataclass
 
 
-@loglevel_command()
-def regenerate_api_key():
-    """Deletes the current IBM Cloud API key and generates a new one"""
-
-    ibm_cloud_api_manager = IBMCloudAPIManager()
-    ibm_cloud_api_manager.regenerate_api_key()
+@dataclass
+class CustomResourceEventResult:
+    succeeded: bool
+    message: str | None = None
```

### Comparing `cloud-pak-operations-cli-0.7.1/cpo/config/__init__.py` & `cloud_pak_operations_cli-0.7.2/cpo/config/__init__.py`

 * *Files identical despite different names*

### Comparing `cloud-pak-operations-cli-0.7.1/cpo/config/binaries_manager.py` & `cloud_pak_operations_cli-0.7.2/cpo/config/binaries_manager.py`

 * *Files 10% similar despite different names*

```diff
@@ -11,40 +11,38 @@
 #  WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 #  See the License for the specific language governing permissions and
 #  limitations under the License.
 
 import json
 import pathlib
 
-from typing import Optional
-
 import semver
 
 from cpo.config import configuration_manager
 from cpo.lib.dependency_manager.dependency_manager_plugin import DependencyVersion
 
 BinariesFileContents = dict[str, str]
 
 
 class BinariesManager:
     """Manages downloaded binaries"""
 
     def __init__(self):
-        self._binaries_file_contents: Optional[dict[str, str]] = None
+        self._binaries_file_contents: dict[str, str] | None = None
 
-    def get_binaries_file_contents(self) -> Optional[BinariesFileContents]:
+    def get_binaries_file_contents(self) -> BinariesFileContents | None:
         """Returns the contents of the binaries file
 
         Returns
         -------
-        Optional[BinariesFileContents]
+        BinariesFileContents | None
             contents of the binaries file or None if it does not exist
         """
 
-        binaries_file_contents: Optional[BinariesFileContents] = None
+        binaries_file_contents: BinariesFileContents | None = None
         binaries_file_path = self.get_binaries_file_path()
 
         if binaries_file_path.exists():
             with open(binaries_file_path) as binaries_file:
                 binaries_file_contents = json.load(binaries_file)
 
         return binaries_file_contents
@@ -54,15 +52,15 @@
 
         Returns
         -------
         BinariesFileContents
             contents of the binaries file or a default value if it does not exist
         """
 
-        binaries_file_contents: Optional[BinariesFileContents] = self.get_binaries_file_contents()
+        binaries_file_contents = self.get_binaries_file_contents()
 
         if binaries_file_contents is None:
             binaries_file_contents = {}
 
         return binaries_file_contents
 
     def get_binaries_file_path(self) -> pathlib.Path:
@@ -72,15 +70,15 @@
         -------
         str
             path of the binaries file
         """
 
         return configuration_manager.get_cli_data_directory_path() / "binaries.json"
 
-    def get_latest_downloaded_binary_version(self, binary_alias: str) -> Optional[DependencyVersion]:
+    def get_latest_downloaded_binary_version(self, binary_alias: str) -> DependencyVersion | None:
         binaries = self._get_binary_versions()
 
         return DependencyVersion(semver.Version.parse(binaries[binary_alias])) if binary_alias in binaries else None
 
     def set_latest_downloaded_binary_version(self, binary_alias: str, version: semver.Version):
         binary_versions = self._get_binary_versions()
```

### Comparing `cloud-pak-operations-cli-0.7.1/cpo/config/cluster_credentials_manager.py` & `cloud_pak_operations_cli-0.7.2/cpo/config/cluster_credentials_manager.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-#  Copyright 2021, 2023 IBM Corporation
+#  Copyright 2021, 2024 IBM Corporation
 #
 #  Licensed under the Apache License, Version 2.0 (the "License");
 #  you may not use this file except in compliance with the License.
 #  You may obtain a copy of the License at
 #
 #  http://www.apache.org/licenses/LICENSE-2.0
 #
@@ -11,15 +11,15 @@
 #  WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 #  See the License for the specific language governing permissions and
 #  limitations under the License.
 
 import json
 import pathlib
 
-from typing import Any, Optional, TypedDict
+from typing import Any, TypedDict
 
 from filelock import FileLock
 from tabulate import tabulate
 
 import cpo.lib.cluster
 
 from cpo.config import configuration_manager
@@ -36,15 +36,15 @@
     current_cluster: str
 
 
 class ClusterCredentialsManager:
     """Manages registered OpenShift clusters"""
 
     def __init__(self):
-        self._current_credentials: Optional[ContextData] = None
+        self._current_credentials: ContextData | None = None
 
     @file_lock
     def add_cluster(self, alias: str, server: str, type: str, cluster_data: ClusterData):
         """Registers an existing OpenShift cluster
 
         Parameters
         ----------
@@ -135,57 +135,57 @@
 
         clusters_file_contents["clusters"][cluster.get_server()] = cluster_data
         self._save_clusters_file(clusters_file_contents)
 
         return cluster
 
     @file_lock
-    def get_cluster(self, alias_or_server) -> Optional[AbstractCluster]:
+    def get_cluster(self, alias_or_server) -> AbstractCluster | None:
         """Returns metadata of the registered OpenShift cluster with the given
         alias or server URL
 
         Parameters
         ----------
         alias_or_server
             alias or server URL of the registered OpenShift cluster for which
             metadata shall be returned
 
         Returns
         -------
-        Optional[AbstractCluster]
+        AbstractCluster | None
             metadata of the registered OpenShift cluster with the given alias or
             server URL or None if no cluster was found
         """
 
         return self.get_cluster_from_clusters_file_contents(
             self.get_clusters_file_contents_with_default(), alias_or_server
         )
 
     def get_cluster_from_clusters_file_contents(
         self, clusters_file_contents: ClustersFileContents, alias_or_server
-    ) -> Optional[AbstractCluster]:
+    ) -> AbstractCluster | None:
         """Returns metadata of the registered OpenShift cluster with the given
         alias or server URL
 
         Parameters
         ----------
         clusters_file_contents
             contents of the clusters file or a default value if it does not exist
         alias_or_server
             alias or server URL of the registered OpenShift cluster for which
             metadata shall be returned
 
         Returns
         -------
-        Optional[AbstractCluster]
+        AbstractCluster | None
             metadata of the registered OpenShift cluster with the given alias or
             server URL or None if no cluster was found
         """
 
-        result: Optional[AbstractCluster] = None
+        result: AbstractCluster | None = None
 
         for server, cluster_data in clusters_file_contents["clusters"].items():
             if (server == alias_or_server) or (
                 ("alias" in cluster_data) and (cluster_data["alias"] == alias_or_server)
             ):
                 cluster_factory = cpo.lib.cluster.cluster_factories[cluster_data["type"]]
                 result = cluster_factory.create_cluster(server, cluster_data)
@@ -242,24 +242,24 @@
             cluster_list.append(cluster_list_element)
 
         result = tabulate(cluster_list, headers=["", "server", "alias", "type"])
 
         return result
 
     @file_lock
-    def get_clusters_file_contents(self) -> Optional[ClustersFileContents]:
+    def get_clusters_file_contents(self) -> ClustersFileContents | None:
         """Returns the contents of the clusters file
 
         Returns
         -------
-        Optional[ClustersFileContents]
+        ClustersFileContents | None
             contents of the clusters file or None if it does not exist
         """
 
-        clusters_file_contents: Optional[ClustersFileContents] = None
+        clusters_file_contents: ClustersFileContents | None = None
         clusters_file_path = self.get_clusters_file_path()
 
         if clusters_file_path.exists():
             with open(clusters_file_path) as clusters_file:
                 clusters_file_contents = json.load(clusters_file)
 
         return clusters_file_contents
@@ -270,18 +270,18 @@
 
         Returns
         -------
         ClustersFileContents
             contents of the clusters file or a default value if it does not exist
         """
 
-        clusters_file_contents: Optional[ClustersFileContents] = self.get_clusters_file_contents()
+        clusters_file_contents = self.get_clusters_file_contents()
 
         if clusters_file_contents is None:
-            clusters_file_contents = {"clusters": {}, "current_cluster": ""}
+            clusters_file_contents = ClustersFileContents(clusters={}, current_cluster="")
         elif "clusters" not in clusters_file_contents:
             # TODO: check JSON schema
             raise CloudPakOperationsCLIException("Corrupt configuration file")
 
         return clusters_file_contents
 
     def get_clusters_file_path(self) -> pathlib.Path:
@@ -292,25 +292,25 @@
         str
             path of the clusters file
         """
 
         return configuration_manager.get_cli_data_directory_path() / "clusters.json"
 
     @file_lock
-    def get_current_cluster(self) -> Optional[AbstractCluster]:
+    def get_current_cluster(self) -> AbstractCluster | None:
         """Returns metadata of the current registered OpenShift cluster
 
         Returns
         -------
-        Optional[AbstractCluster]
+        AbstractCluster | None
             metadata of the current registered OpenShift cluster or None if no
             current cluster is set
         """
 
-        cluster: Optional[AbstractCluster] = None
+        cluster: AbstractCluster | None = None
         clusters_file_contents = self.get_clusters_file_contents_with_default()
         server_of_current_cluster = clusters_file_contents["current_cluster"]
 
         if server_of_current_cluster != "":
             cluster = self.get_cluster_from_clusters_file_contents(clusters_file_contents, server_of_current_cluster)
 
             if cluster is None:
```

### Comparing `cloud-pak-operations-cli-0.7.1/cpo/config/configuration_manager.py` & `cloud_pak_operations_cli-0.7.2/cpo/config/configuration_manager.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-#  Copyright 2021, 2023 IBM Corporation
+#  Copyright 2021, 2024 IBM Corporation
 #
 #  Licensed under the Apache License, Version 2.0 (the "License");
 #  you may not use this file except in compliance with the License.
 #  You may obtain a copy of the License at
 #
 #  http://www.apache.org/licenses/LICENSE-2.0
 #
@@ -11,15 +11,15 @@
 #  WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 #  See the License for the specific language governing permissions and
 #  limitations under the License.
 
 import json
 import pathlib
 
-from typing import Any, Optional
+from typing import Any
 
 import cpo
 
 from cpo.utils.error import CloudPakOperationsCLIException
 
 
 class ConfigurationManager:
@@ -135,49 +135,49 @@
         -------
         pathlib.Path
             path of the root package
         """
 
         return pathlib.Path(cpo.__file__).parent
 
-    def get_value_from_credentials_file(self, key: str) -> Optional[str]:
+    def get_value_from_credentials_file(self, key: str) -> str | None:
         """Returns the value corresponding to the given key stored in the
         credentials file
 
         Parameters
         ----------
         key
             key for which the corresponding value shall be returned
 
         Returns
         -------
-            Optional[str]
+            str | None
                 value corresponding to the given key or None if the key does not exist
         """
 
         credentials_file_contents = self.read_credentials_file_contents()
-        result: Optional[str] = None
+        result: str | None = None
 
         if (credentials_file_contents is not None) and (key in credentials_file_contents):
             result = credentials_file_contents[key]
 
         return result
 
-    def read_credentials_file_contents(self) -> Optional[Any]:
+    def read_credentials_file_contents(self) -> Any | None:
         """Returns the contents of the credentials file
 
         Returns
         -------
-            Optional[str]
+            str | None
                 contents of the credentials file or none of the credentials file does
                 not exist or is empty
         """
 
         credentials_file_path = self.get_credentials_file_path()
-        result: Optional[str] = None
+        result: str | None = None
 
         if credentials_file_path.exists() and (credentials_file_path.stat().st_size != 0):
             with open(credentials_file_path) as json_file:
                 result = json.load(json_file)
 
         return result
 
@@ -225,15 +225,15 @@
             dictionary containing key-value pairs to be stored (key-value pairs
             whose value is None are ignored)
         """
 
         if all(value is None for value in credentials_to_be_stored.values()):
             return
 
-        credentials: Optional[dict[Any, Any]] = None
+        credentials: dict[Any, Any] | None = None
         credentials_file_path = self.get_credentials_file_path()
 
         if credentials_file_path.exists():
             with open(credentials_file_path) as credentials_file:
                 credentials = json.load(credentials_file)
 
                 if credentials is None:
```

### Comparing `cloud-pak-operations-cli-0.7.1/cpo/cpo.py` & `cloud_pak_operations_cli-0.7.2/cpo/cpo.py`

 * *Files identical despite different names*

### Comparing `cloud-pak-operations-cli-0.7.1/cpo/deps/autocomplete/cpo-autocomplete-bash.sh` & `cloud_pak_operations_cli-0.7.2/cpo/deps/autocomplete/cpo-autocomplete-bash.sh`

 * *Files identical despite different names*

### Comparing `cloud-pak-operations-cli-0.7.1/cpo/deps/autocomplete/cpo-autocomplete-zsh.sh` & `cloud_pak_operations_cli-0.7.2/cpo/deps/autocomplete/cpo-autocomplete-zsh.sh`

 * *Files identical despite different names*

### Comparing `cloud-pak-operations-cli-0.7.1/cpo/deps/playbooks/delete_terminated_pods_playbook.yaml` & `cloud_pak_operations_cli-0.7.2/cpo/deps/playbooks/delete_terminated_pods_playbook.yaml`

 * *Files identical despite different names*

### Comparing `cloud-pak-operations-cli-0.7.1/cpo/deps/playbooks/deploy_odf_playbook.yaml` & `cloud_pak_operations_cli-0.7.2/cpo/deps/playbooks/deploy_odf_playbook.yaml`

 * *Files identical despite different names*

### Comparing `cloud-pak-operations-cli-0.7.1/cpo/lib/ansible/modules/abstract_module.py` & `cloud_pak_operations_cli-0.7.2/cpo/lib/ansible/modules/abstract_module.py`

 * *Files 4% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 #  WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 #  See the License for the specific language governing permissions and
 #  limitations under the License.
 
 import logging
 
 from abc import ABC, abstractmethod
-from typing import Callable, Optional
+from typing import Callable
 
 import urllib3.exceptions
 
 from ansible.module_utils.basic import AnsibleModule
 from kubernetes import client, config, watch
 from q import q
 
@@ -83,23 +83,23 @@
         if level >= logging.WARN:
             self.get_module().warn(msg)
 
     def _wait_for_custom_resource(
         self,
         kind_metadata: KindMetadata,
         log_callback: Callable[[int, str], None],
-        success_callback: Callable[..., Optional[CustomResourceEventResult]],
+        success_callback: Callable[..., CustomResourceEventResult | None],
         **kwargs,
     ) -> CustomResourceEventResult:
         custom_objects_api = client.CustomObjectsApi()
-        custom_resource_event_result: Optional[CustomResourceEventResult] = None
+        custom_resource_event_result: CustomResourceEventResult | None = None
 
         while custom_resource_event_result is None:
             try:
-                resource_version: Optional[str] = None
+                resource_version: str | None = None
                 w = watch.Watch()
 
                 for event in w.stream(
                     custom_objects_api.list_cluster_custom_object,
                     kind_metadata.group,
                     kind_metadata.version,
                     kind_metadata.plural,
@@ -119,23 +119,23 @@
         return custom_resource_event_result
 
     def _wait_for_namespaced_custom_resource(
         self,
         project: str,
         kind_metadata: KindMetadata,
         log_callback: Callable[[int, str], None],
-        success_callback: Callable[..., Optional[CustomResourceEventResult]],
+        success_callback: Callable[..., CustomResourceEventResult | None],
         **kwargs,
     ) -> CustomResourceEventResult:
         custom_objects_api = client.CustomObjectsApi()
-        custom_resource_event_result: Optional[CustomResourceEventResult] = None
+        custom_resource_event_result: CustomResourceEventResult | None = None
 
         while custom_resource_event_result is None:
             try:
-                resource_version: Optional[str] = None
+                resource_version: str | None = None
                 w = watch.Watch()
 
                 for event in w.stream(
                     custom_objects_api.list_namespaced_custom_object,
                     kind_metadata.group,
                     kind_metadata.version,
                     project,
```

### Comparing `cloud-pak-operations-cli-0.7.1/cpo/lib/ansible/modules/custom_resource_event_result.py` & `cloud_pak_operations_cli-0.7.2/cpo/lib/openshift/types/custom_resource_event_result.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,22 +1,21 @@
-#  Copyright 2022 IBM Corporation
+#  Copyright 2022, 2024 IBM Corporation
 #
 #  Licensed under the Apache License, Version 2.0 (the "License");
 #  you may not use this file except in compliance with the License.
 #  You may obtain a copy of the License at
 #
 #  http://www.apache.org/licenses/LICENSE-2.0
 #
 #  Unless required by applicable law or agreed to in writing, software
 #  distributed under the License is distributed on an "AS IS" BASIS,
 #  WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 #  See the License for the specific language governing permissions and
 #  limitations under the License.
 
 from dataclasses import dataclass
-from typing import Optional
 
 
 @dataclass
 class CustomResourceEventResult:
     succeeded: bool
-    message: Optional[str] = None
+    message: str | None = None
```

### Comparing `cloud-pak-operations-cli-0.7.1/cpo/lib/ansible/modules/wait_for_custom_resource.py` & `cloud_pak_operations_cli-0.7.2/cpo/lib/ansible/modules/wait_for_custom_resource.py`

 * *Files 18% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 #  WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 #  See the License for the specific language governing permissions and
 #  limitations under the License.
 
 import logging
 
 from dataclasses import dataclass
-from typing import Any, Optional
+from typing import Any
 
 from ansible.module_utils.basic import AnsibleModule
 
 import cpo.lib.jmespath
 
 from cpo.lib.ansible.modules.abstract_module import AbstractModule
 from cpo.lib.ansible.modules.custom_resource_event_result import CustomResourceEventResult
@@ -65,29 +65,29 @@
             },
         }
 
         self._module = AnsibleModule(argument_spec=argument_spec, supports_check_mode=True)
         super().__init__(self._module.params["kubeconfig"])  # type: ignore
 
         self._custom_resource_name: str = self._module.params["custom_resource_name"]  # type: ignore
-        self._jmespath_expression: Optional[str] = self._module.params["jmespath_expression"]  # type: ignore
+        self._jmespath_expression: str | None = self._module.params["jmespath_expression"]  # type: ignore
         self._kind_metadata = KindMetadata(
             self._module.params["group"],  # type: ignore
             self._module.params["kind"],  # type: ignore
             self._module.params["plural"],  # type: ignore
             self._module.params["version"],  # type: ignore
         )
 
     # override
     def get_module(self) -> AnsibleModule:
         return self._module
 
     # override
     def run(self):
-        result: Optional[dict]
+        result: dict | None
 
         try:
             self._wait_for_custom_resource(
                 self._kind_metadata,
                 self._log,
                 self._success_callback,
                 # passed to _add_event_indicates_custom_resource_definitions_are_created
@@ -100,16 +100,16 @@
 
             result = {"changed": False, "failed": True}
 
         self._module.exit_json(**result)
 
     def _success_callback(
         self, event: Any, kind_metadata: KindMetadata, custom_resource_event_data: CustomResourceEventData
-    ) -> Optional[CustomResourceEventResult]:
-        custom_resource_event_result: Optional[CustomResourceEventResult] = None
+    ) -> CustomResourceEventResult | None:
+        custom_resource_event_result: CustomResourceEventResult | None = None
 
         if (event["type"] == "ADDED") or (event["type"] == "MODIFIED"):
             resource_name = cpo.lib.jmespath.get_jmespath_string("object.metadata.name", event)
 
             try:
                 if resource_name == custom_resource_event_data.custom_resource_name:
                     if (self._jmespath_expression is None) or cpo.lib.jmespath.get_jmespath_bool(
```

### Comparing `cloud-pak-operations-cli-0.7.1/cpo/lib/ansible/modules/wait_for_custom_resource_definitions.py` & `cloud_pak_operations_cli-0.7.2/cpo/lib/ansible/modules/wait_for_custom_resource_definitions.py`

 * *Files 2% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 #  WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 #  See the License for the specific language governing permissions and
 #  limitations under the License.
 
 import logging
 
 from dataclasses import dataclass, field
-from typing import Any, Optional
+from typing import Any
 
 from ansible.module_utils.basic import AnsibleModule
 
 import cpo.lib.jmespath
 
 from cpo.lib.ansible.modules.abstract_module import AbstractModule
 from cpo.lib.ansible.modules.custom_resource_event_result import CustomResourceEventResult
@@ -55,15 +55,15 @@
 
     # override
     def get_module(self) -> AnsibleModule:
         return self._module
 
     # override
     def run(self):
-        result: Optional[dict]
+        result: dict | None = None
 
         try:
             self._wait_for_custom_resource(
                 KindMetadata(
                     "apiextensions.k8s.io",
                     "CustomResourceDefinition",
                     "customresourcedefinitions",
@@ -86,15 +86,15 @@
         self._module.exit_json(**result)
 
     def _add_event_indicates_custom_resource_definitions_are_created(
         self,
         event: Any,
         kind_metadata: KindMetadata,
         custom_resource_definitions_event_data: CustomResourceDefinitionsEventData,
-    ) -> Optional[CustomResourceEventResult]:
+    ) -> CustomResourceEventResult | None:
         """Callback for checking whether the given set of expected custom
         resource definitions was created
 
         Parameters
         ----------
         event
             OpenShift watch event
@@ -108,15 +108,15 @@
         Returns
         -------
         bool
             true, if the given set of expected custom resource definitions was
             created
         """
 
-        custom_resource_event_result: Optional[CustomResourceEventResult] = None
+        custom_resource_event_result: CustomResourceEventResult | None = None
 
         if event["type"] == "ADDED":
             encountered_crd_kind = cpo.lib.jmespath.get_jmespath_string("object.spec.names.kind", event)
 
             if encountered_crd_kind in custom_resource_definitions_event_data.expected_crd_kinds:
                 self._log(logging.DEBUG, f"Detected creation of custom resource definition '{encountered_crd_kind}'")
                 custom_resource_definitions_event_data.encountered_crd_kinds.add(encountered_crd_kind)
```

### Comparing `cloud-pak-operations-cli-0.7.1/cpo/lib/ansible/modules/wait_for_namespaced_custom_resource.py` & `cloud_pak_operations_cli-0.7.2/cpo/lib/ansible/modules/wait_for_namespaced_custom_resource.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,23 +1,25 @@
-#  Copyright 2022, 2023 IBM Corporation
+#  Copyright 2022, 2024 IBM Corporation
 #
 #  Licensed under the Apache License, Version 2.0 (the "License");
 #  you may not use this file except in compliance with the License.
 #  You may obtain a copy of the License at
 #
 #  http://www.apache.org/licenses/LICENSE-2.0
 #
 #  Unless required by applicable law or agreed to in writing, software
 #  distributed under the License is distributed on an "AS IS" BASIS,
 #  WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 #  See the License for the specific language governing permissions and
 #  limitations under the License.
 
+import logging
+
 from dataclasses import dataclass
-from typing import Any, Optional
+from typing import Any
 
 from ansible.module_utils.basic import AnsibleModule
 
 import cpo.lib.jmespath
 
 from cpo.lib.ansible.modules.abstract_module import AbstractModule
 from cpo.lib.ansible.modules.custom_resource_event_result import CustomResourceEventResult
@@ -67,15 +69,15 @@
             },
         }
 
         self._module = AnsibleModule(argument_spec=argument_spec, supports_check_mode=True)
         super().__init__(self._module.params["kubeconfig"])  # type: ignore
 
         self._custom_resource_name: str = self._module.params["custom_resource_name"]  # type: ignore
-        self._jmespath_expression: Optional[str] = self._module.params["jmespath_expression"]  # type: ignore
+        self._jmespath_expression: str | None = self._module.params["jmespath_expression"]  # type: ignore
         self._kind_metadata = KindMetadata(
             self._module.params["group"],  # type: ignore
             self._module.params["kind"],  # type: ignore
             self._module.params["plural"],  # type: ignore
             self._module.params["version"],  # type: ignore
         )
 
@@ -83,36 +85,38 @@
 
     # override
     def get_module(self) -> AnsibleModule:
         return self._module
 
     # override
     def run(self):
-        result: Optional[dict]
+        result: dict | None = None
 
         try:
             self._wait_for_namespaced_custom_resource(
                 self._project,
                 self._kind_metadata,
                 self._log,
                 self._success_callback,
                 # passed to _add_event_indicates_custom_resource_definitions_are_created
                 custom_resource_event_data=CustomResourceEventData(custom_resource_name=self._custom_resource_name),
             )
 
             result = {"changed": False}
-        except Exception:
+        except Exception as exception:
+            self._log(logging.ERROR, str(exception))
+
             result = {"changed": False, "failed": True}
 
         self._module.exit_json(**result)
 
     def _success_callback(
         self, event: Any, kind_metadata: KindMetadata, custom_resource_event_data: CustomResourceEventData
-    ) -> Optional[CustomResourceEventResult]:
-        custom_resource_event_result: Optional[CustomResourceEventResult] = None
+    ) -> CustomResourceEventResult | None:
+        custom_resource_event_result: CustomResourceEventResult | None = None
 
         if (event["type"] == "ADDED") or (event["type"] == "MODIFIED"):
             resource_name = cpo.lib.jmespath.get_jmespath_string("object.metadata.name", event)
 
             try:
                 if resource_name == custom_resource_event_data.custom_resource_name:
                     if (self._jmespath_expression is None) or cpo.lib.jmespath.get_jmespath_bool(
```

### Comparing `cloud-pak-operations-cli-0.7.1/cpo/lib/ansible/openshift_playbook_runner.py` & `cloud_pak_operations_cli-0.7.2/cpo/lib/ansible/openshift_playbook_runner.py`

 * *Files 2% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 #  distributed under the License is distributed on an "AS IS" BASIS,
 #  WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 #  See the License for the specific language governing permissions and
 #  limitations under the License.
 
 import logging
 
-from typing import Any, Optional
+from typing import Any
 
 import jmespath
 
 import cpo.lib.jmespath
 
 from cpo.config import configuration_manager
 from cpo.lib.ansible.playbook_runner import PlaybookRunner
@@ -40,15 +40,15 @@
         private_data_dir=configuration_manager.get_deps_directory_path() / "playbooks",
         variables: dict[str, Any] = {},
     ):
         super().__init__(playbook_name, private_data_dir=private_data_dir, variables=variables)
 
         self._openshift_api_manager = OpenShiftAPIManager(credentials)
         self._token_expired = False
-        self.kube_config: Optional[dict[str, Any]] = None
+        self.kube_config: dict[str, Any] | None = None
 
     # override
     def run_playbook(self):
         """Runs a playbook
 
         If the OpenShift-based playbook fails due to an expired OAuth access
         token, it is refreshed an the playbook is rerun.
```

### Comparing `cloud-pak-operations-cli-0.7.1/cpo/lib/ansible/playbook_runner.py` & `cloud_pak_operations_cli-0.7.2/cpo/lib/ansible/playbook_runner.py`

 * *Files identical despite different names*

### Comparing `cloud-pak-operations-cli-0.7.1/cpo/lib/click/cpd_service_spec_param_type.py` & `cloud_pak_operations_cli-0.7.2/cpo/lib/click/cpd_service_spec_param_type.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,34 +1,34 @@
-#  Copyright 2021 IBM Corporation
+#  Copyright 2021, 2024 IBM Corporation
 #
 #  Licensed under the Apache License, Version 2.0 (the "License");
 #  you may not use this file except in compliance with the License.
 #  You may obtain a copy of the License at
 #
 #  http://www.apache.org/licenses/LICENSE-2.0
 #
 #  Unless required by applicable law or agreed to in writing, software
 #  distributed under the License is distributed on an "AS IS" BASIS,
 #  WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 #  See the License for the specific language governing permissions and
 #  limitations under the License.
 
-from typing import Any, Optional
+from typing import Any
 
 import click
 
 
 class CloudPakForDataServiceSpecParamType(click.ParamType):
     """Click parameter type accepting a boolean, integer, or string
     argument"""
 
     name = "VALUE"
 
     # override
-    def convert(self, value: Any, param: Optional[click.Parameter], ctx: Optional[click.Context]) -> Any:
+    def convert(self, value: Any, param: click.Parameter | None, ctx: click.Context | None) -> Any:
         try:
             return click.BOOL.convert(value, param, ctx)
         except click.BadParameter:
             pass
 
         try:
             return click.INT.convert(value, param, ctx)
```

### Comparing `cloud-pak-operations-cli-0.7.1/cpo/lib/click/lazy_loading_multi_command.py` & `cloud_pak_operations_cli-0.7.2/cpo/lib/click/lazy_loading_multi_command.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-#  Copyright 2021, 2023 IBM Corporation
+#  Copyright 2021, 2024 IBM Corporation
 #
 #  Licensed under the Apache License, Version 2.0 (the "License");
 #  you may not use this file except in compliance with the License.
 #  You may obtain a copy of the License at
 #
 #  http://www.apache.org/licenses/LICENSE-2.0
 #
@@ -14,17 +14,18 @@
 
 import importlib
 import importlib.metadata
 import importlib.util
 import logging
 import pathlib
 
-from dataclasses import dataclass, field
+from dataclasses import dataclass
+from functools import total_ordering
 from types import ModuleType
-from typing import Optional, cast
+from typing import cast
 
 import click
 
 from sortedcontainers import SortedSet
 
 import cpo
 import cpo.utils.debugger
@@ -35,23 +36,34 @@
 from cpo.lib.plugin_manager.plugin_manager import plugin_manager
 from cpo.utils.error import CloudPakOperationsCLIException
 
 logger = logging.getLogger(__name__)
 
 
 @dataclass
+@total_ordering
 class CommandDetails:
     command: click.Command
+    command_name: str
     distribution_package_name: str
 
+    def __lt__(self, other: "CommandDetails") -> bool:
+        result: bool | None = None
+
+        if isinstance(self.command, click.Group) and not isinstance(other.command, click.Group):
+            result = True
+        elif not isinstance(self.command, click.Group) and isinstance(other.command, click.Group):
+            result = False
+        else:
+            result = self.command_name < other.command_name
+
+        return result
 
-@dataclass
-class CommandData:
-    command_names: SortedSet = field(default_factory=SortedSet)
-    commands: dict[str, CommandDetails] = field(default_factory=dict)
+
+CommandData = dict[str, CommandDetails]
 
 
 class LazyLoadingMultiCommand(click.Group):
     """Provides Click commands found within modules of the package passed to
     the constructor
 
     For each found subpackage of the package passed to the constructor, a
@@ -75,47 +87,47 @@
                 return 1
 
     def __init__(self, distribution_package_name: str, package: ModuleType, **kwargs):
         super().__init__(**kwargs)
 
         assert package.__file__ is not None
 
-        self._command_data: Optional[CommandData] = None
+        self._command_data: CommandData | None = None
         self._package_directories = SortedSet(
             [PackageDirectoryDetails(distribution_package_name, pathlib.Path(package.__file__).parent)]
         )
 
     def add_package_directory_path(self, distribution_package_name: str, package: ModuleType):
         assert package.__file__ is not None
 
         self._package_directories.add(
             PackageDirectoryDetails(distribution_package_name, pathlib.Path(package.__file__).parent)
         )
 
     # override
-    def get_command(self, ctx: click.Context, cmd_name: str) -> Optional[click.Command]:
+    def get_command(self, ctx: click.Context, cmd_name: str) -> click.Command | None:
         self._initialize_command_data_if_required()
 
-        command: Optional[click.Command] = None
+        command: click.Command | None = None
 
         if self._command_data is not None:
-            command = self._command_data.commands[cmd_name].command if cmd_name in self._command_data.commands else None
+            command = self._command_data[cmd_name].command if cmd_name in self._command_data else None
 
         return command
 
     # override
     def list_commands(self, ctx: click.Context) -> list[str]:
         self._initialize_command_data_if_required()
 
-        return self._command_data.command_names if self._command_data is not None else []
+        return list(self._command_data.keys()) if self._command_data is not None else []
 
     def _append_distribution_package_name_to_help_text(
-        self, help_text: Optional[str], distribution_package_name: str
-    ) -> Optional[str]:
-        suffix = f"[{distribution_package_name}]"
+        self, help_text: str | None, distribution_package_name: str
+    ) -> str | None:
+        suffix = f"(plug-in: {distribution_package_name})"
 
         return suffix if (help_text is None) or (help_text == "") else f"{help_text} {suffix}"
 
     def _import_module_from_file_location(self, package_element_descriptor: PackageElementDescriptor) -> ModuleType:
         """Imports the module corresponding to the given package element
         descriptor from a file location
 
@@ -158,20 +170,18 @@
             module = self._import_module_from_file_location(package_element_descriptor)
             command_dict = self._search_for_commands(package_element_descriptor, module)
 
             if len(command_dict) == 0:
                 continue
 
             for command_name in command_dict:
-                if command_name in command_data.command_names:
+                if command_name in command_data:
                     self._raise_registration_error(command_name, command_data, package_element_descriptor)
 
-                command_data.command_names.add(command_name)
-
-            command_data.commands.update(command_dict)
+            command_data.update(command_dict)
 
     def _import_subpackages(self, command_data: CommandData, subpackages: list[PackageElementDescriptor]):
         """Imports the given subpackages and updates the given command data
         object
 
         Parameters
         ----------
@@ -182,42 +192,47 @@
         """
 
         for package_element_descriptor in subpackages:
             logger.debug(f"Importing package {package_element_descriptor.name}")
 
             command_name = package_element_descriptor.name.replace("_", "-")
 
-            if command_name in command_data.command_names:
-                command_details = command_data.commands[command_name]
+            if command_name in command_data:
+                command_details = command_data[command_name]
 
                 if not isinstance(command_details.command, LazyLoadingMultiCommand):
                     self._raise_registration_error(command_name, command_data, package_element_descriptor)
 
                 command_group = cast(LazyLoadingMultiCommand, command_details.command)
                 command_group.add_package_directory_path(
                     package_element_descriptor.distribution_package_name,
                     self._import_module_from_file_location(package_element_descriptor),
                 )
             else:
                 package = self._import_module_from_file_location(package_element_descriptor)
 
-                command_data.command_names.add(command_name)
-                command_data.commands.update(
+                command_data.update(
                     {
                         command_name: CommandDetails(
                             LazyLoadingMultiCommand(
                                 package_element_descriptor.distribution_package_name,
                                 package,
-                                help=package.__doc__
-                                if package_element_descriptor.distribution_package_name == cpo.distribution_package_name
-                                else self._append_distribution_package_name_to_help_text(
-                                    package.__doc__, package_element_descriptor.distribution_package_name
+                                help=(
+                                    f"[{package.__doc__}]"
+                                    if package_element_descriptor.distribution_package_name
+                                    == cpo.distribution_package_name
+                                    else "[{help_text}]".format(
+                                        help_text=self._append_distribution_package_name_to_help_text(
+                                            package.__doc__, package_element_descriptor.distribution_package_name
+                                        )
+                                    )
                                 ),
                                 name=None,
                             ),
+                            command_name,
                             package_element_descriptor.distribution_package_name,
                         )
                     }
                 )
 
     def _initialize_command_data_if_required(self):
         """Creates a data structure based on modules and subpackges of the
@@ -256,15 +271,15 @@
 
                 if command_hierarchy_path in plugin_manager.package_data_dict:
                     plugin_package_data = plugin_manager.package_data_dict[command_hierarchy_path]
 
                     self._import_modules(command_data, plugin_package_data.modules)
                     self._import_subpackages(command_data, plugin_package_data.subpackages)
 
-        self._command_data = command_data
+        self._command_data = dict(sorted(command_data.items(), key=lambda item: item[1]))
 
     def _is_builtin_package(self, package_directory_path: pathlib.Path) -> bool:
         return package_directory_path.is_relative_to(commands_package_path)
 
     def _raise_registration_error(
         self, command_name: str, command_data: CommandData, package_element_descriptor: PackageElementDescriptor
     ):
@@ -281,30 +296,28 @@
             object describing a module or a subpackage within a package whereas the
             module or subpackage corresponds to the Click command (group) with the
             given name
         """
 
         command_type_1 = "Command group" if str(package_element_descriptor.path).endswith("__init__.py") else "Command"
         command_type_2 = (
-            "command group"
-            if isinstance(command_data.commands[command_name].command, click.MultiCommand)
-            else "command"
+            "command group" if isinstance(command_data[command_name].command, click.MultiCommand) else "command"
         )
 
         command_hierarchy_path = (
             f", command hierarchy path: '{package_element_descriptor.command_hierarchy_path}'"
             if package_element_descriptor.command_hierarchy_path is not None
             else ""
         )
 
         raise CloudPakOperationsCLIException(
             f"{command_type_1} '{command_name}' (distribution package: '"
             f"{package_element_descriptor.distribution_package_name}'{command_hierarchy_path}) cannot be registered as "
             f"a {command_type_2} with the same name was already provided by distribution package '"
-            f"{command_data.commands[command_name].distribution_package_name}'"
+            f"{command_data[command_name].distribution_package_name}'"
         )
 
     def _search_for_commands(
         self, package_element_descriptor: PackageElementDescriptor, module: ModuleType
     ) -> dict[str, CommandDetails]:
         """Searches the given module for Click commands
 
@@ -330,10 +343,12 @@
                 if package_element_descriptor.distribution_package_name != cpo.distribution_package_name:
                     attribute.help = self._append_distribution_package_name_to_help_text(
                         attribute.help, package_element_descriptor.distribution_package_name
                     )
 
                 command_name = attribute_name.replace("_", "-")
 
-                commands[command_name] = CommandDetails(attribute, package_element_descriptor.distribution_package_name)
+                commands[command_name] = CommandDetails(
+                    attribute, command_name, package_element_descriptor.distribution_package_name
+                )
 
         return commands
```

### Comparing `cloud-pak-operations-cli-0.7.1/cpo/lib/click/package_directory_details.py` & `cloud_pak_operations_cli-0.7.2/cpo/lib/click/package_directory_details.py`

 * *Files identical despite different names*

### Comparing `cloud-pak-operations-cli-0.7.1/cpo/lib/click/utils.py` & `cloud_pak_operations_cli-0.7.2/cpo/lib/click/utils.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-#  Copyright 2021, 2023 IBM Corporation
+#  Copyright 2021, 2024 IBM Corporation
 #
 #  Licensed under the Apache License, Version 2.0 (the "License");
 #  you may not use this file except in compliance with the License.
 #  You may obtain a copy of the License at
 #
 #  http://www.apache.org/licenses/LICENSE-2.0
 #
@@ -11,15 +11,15 @@
 #  WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 #  See the License for the specific language governing permissions and
 #  limitations under the License.
 
 import json
 import pathlib
 
-from typing import Any, Optional
+from typing import Any
 
 import click
 import semver
 
 import cpo.lib.openshift.oc
 
 from cpo.config.cluster_credentials_manager import cluster_credentials_manager
@@ -73,19 +73,19 @@
 
     Returns
     -------
     AbstractCredentials
         cluster credentials
     """
 
-    insecure_skip_tls_verify: Optional[bool] = (
+    insecure_skip_tls_verify: bool | None = (
         options["insecure_skip_tls_verify"] if "insecure_skip_tls_verify" in options else None
     )
 
-    result: Optional[AbstractCredentials] = None
+    result: AbstractCredentials | None = None
 
     if (
         ("server" in options)
         and (options["server"] is not None)
         and ("username" in options)
         and (options["username"] is not None)
         and ("password" in options)
@@ -126,15 +126,15 @@
             ctx,
         )
 
     return result
 
 
 def get_oc_login_command_for_remote_host(ctx: click.Context, options: dict[str, Any]) -> str:
-    result: Optional[str] = None
+    result: str | None = None
 
     if (
         ("server" in options)
         and (options["server"] is not None)
         and ("username" in options)
         and (options["username"] is not None)
         and ("password" in options)
```

### Comparing `cloud-pak-operations-cli-0.7.1/cpo/lib/cluster/__init__.py` & `cloud_pak_operations_cli-0.7.2/cpo/lib/cluster/__init__.py`

 * *Files identical despite different names*

### Comparing `cloud-pak-operations-cli-0.7.1/cpo/lib/cluster/cluster.py` & `cloud_pak_operations_cli-0.7.2/cpo/lib/cluster/cluster.py`

 * *Files identical despite different names*

### Comparing `cloud-pak-operations-cli-0.7.1/cpo/lib/cluster/cluster_factory.py` & `cloud_pak_operations_cli-0.7.2/cpo/lib/cluster/cluster_factory.py`

 * *Files identical despite different names*

### Comparing `cloud-pak-operations-cli-0.7.1/cpo/lib/dependency_manager/dependency_manager.py` & `cloud_pak_operations_cli-0.7.2/cpo/lib/dependency_manager/dependency_manager.py`

 * *Files 2% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 #  WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 #  See the License for the specific language governing permissions and
 #  limitations under the License.
 
 import os
 import pathlib
 
-from typing import Optional, TypeVar
+from typing import TypeVar
 
 import semver
 
 import cpo.utils.operating_system
 import cpo.utils.process
 
 from cpo.config.binaries_manager import binaries_manager
@@ -140,15 +140,15 @@
         Returns
         -------
         ProcessResult
             object storing the return code and captured process output (if
             requested)
         """
 
-        dependency_version: Optional[DependencyVersion] = None
+        dependency_version: DependencyVersion | None = None
 
         if isinstance(version, semver.Version):
             dependency_version = DependencyVersion(version)
         elif isinstance(version, str):
             dependency_version = AbstractDependencyManagerPlugIn.parse_as_semantic_version(version)
 
         plugin = self.get_plugin_for_plugin_class(cls)
@@ -200,15 +200,15 @@
         cls
             dependency manager plug-in type
         version
             version of the dependency
 
         Returns
         -------
-        Optional[pathlib.Path]
+        pathlib.Path | None
             path of the binary provided by the dependency corresponding to the
             dependency manager plug-in of the given type or None if the dependency
             does not provide a binary
         """
 
         plugin = self.get_plugin_for_plugin_class(cls)
 
@@ -263,8 +263,8 @@
             dependency_version = plugin.get_latest_dependency_version()
 
         plugin.download_dependency_version(dependency_version)
         binaries_manager.set_latest_downloaded_binary_version(plugin.get_dependency_alias(), dependency_version.version)
 
         return dependency_version
 
-    _instance: Optional["DependencyManager"] = None
+    _instance: "DependencyManager | None" = None
```

### Comparing `cloud-pak-operations-cli-0.7.1/cpo/lib/dependency_manager/dependency_manager_binary_plugin.py` & `cloud_pak_operations_cli-0.7.2/cpo/lib/dependency_manager/dependency_manager_binary_plugin.py`

 * *Files identical despite different names*

### Comparing `cloud-pak-operations-cli-0.7.1/cpo/lib/dependency_manager/dependency_manager_plugin.py` & `cloud_pak_operations_cli-0.7.2/cpo/lib/dependency_manager/dependency_manager_plugin.py`

 * *Files 2% similar despite different names*

```diff
@@ -13,15 +13,14 @@
 #  limitations under the License.
 
 import json
 import re as regex
 
 from abc import ABC, abstractmethod
 from dataclasses import dataclass
-from typing import Optional
 
 import requests
 import semver
 
 from cpo.utils.error import CloudPakOperationsCLIException
 from cpo.utils.operating_system import OperatingSystem
 
@@ -132,15 +131,15 @@
 
         pass
 
     @abstractmethod
     def is_operating_system_supported(self, operating_system: OperatingSystem) -> bool:
         pass
 
-    def _get_latest_dependency_version_on_github(self, owner: str, repo: str) -> Optional[DependencyVersion]:
+    def _get_latest_dependency_version_on_github(self, owner: str, repo: str) -> DependencyVersion | None:
         """Returns the latest version of the dependency on GitHub
 
         This method parses the "name" key of the JSON document returned by the
         GitHub Releases API, which has the following structure:
 
         [
             {
@@ -182,21 +181,21 @@
         owner
             GitHub repository owner
         repo
             GitHub repository name
 
         Returns
         -------
-        Optional[DependencyVersion]
+        DependencyVersion | None
             latest version of the dependency or None if no release was found
         """
 
         response = requests.get(f"https://api.github.com/repos/{owner}/{repo}/releases")
         response.raise_for_status()
 
         response_json = json.loads(response.content)
-        result: Optional[DependencyVersion] = None
+        result: DependencyVersion | None = None
 
         if len(response_json) != 0:
             result = AbstractDependencyManagerPlugIn.parse_as_semantic_version(response_json[0]["name"])
 
         return result
```

### Comparing `cloud-pak-operations-cli-0.7.1/cpo/lib/dependency_manager/plugins/ibm_cloud_cli_plugin.py` & `cloud_pak_operations_cli-0.7.2/cpo/lib/dependency_manager/plugins/ibm_cloud_cli_plugin.py`

 * *Files 2% similar despite different names*

```diff
@@ -12,16 +12,14 @@
 #  See the License for the specific language governing permissions and
 #  limitations under the License.
 
 import os
 import pathlib
 import urllib.parse
 
-from typing import Optional
-
 import semver
 
 import cpo.config
 import cpo.utils.compression
 import cpo.utils.download
 import cpo.utils.file
 import cpo.utils.operating_system
@@ -79,15 +77,15 @@
         except CloudPakOperationsCLIException as exception:
             if exception.stderr is not None:
                 raise IBMCloudException(exception.stderr)
             else:
                 raise
 
     # override
-    def get_binary_name(self) -> Optional[str]:
+    def get_binary_name(self) -> str | None:
         return "ibmcloud"
 
     # override
     def get_dependency_alias(self) -> str:
         return "ibmcloud"
 
     # override
```

### Comparing `cloud-pak-operations-cli-0.7.1/cpo/lib/dependency_manager/plugins/ibm_cloud_pak_cli_plugin.py` & `cloud_pak_operations_cli-0.7.2/cpo/lib/dependency_manager/plugins/ibm_cloud_pak_cli_plugin.py`

 * *Files 3% similar despite different names*

```diff
@@ -11,16 +11,14 @@
 #  WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 #  See the License for the specific language governing permissions and
 #  limitations under the License.
 
 import pathlib
 import urllib.parse
 
-from typing import Optional
-
 import semver
 
 import cpo.config
 import cpo.utils.compression
 import cpo.utils.download
 import cpo.utils.operating_system
 
@@ -45,15 +43,15 @@
         file_name = f"cloudctl-{file_name_infix}-amd64.tar.gz"
         url = f"https://github.com/IBM/cloud-pak-cli/releases/download/v{str(dependency_version)}/{file_name}"
         archive_path = cpo.utils.download.download_file(urllib.parse.urlsplit(url))
 
         self._extract_archive(archive_path, dependency_version.version, operating_system)
 
     # override
-    def get_binary_name(self) -> Optional[str]:
+    def get_binary_name(self) -> str | None:
         return "cloudctl"
 
     # override
     def get_dependency_alias(self) -> str:
         return "cloudctl"
 
     # override
```

### Comparing `cloud-pak-operations-cli-0.7.1/cpo/lib/dependency_manager/plugins/ibm_cloud_terraform_provider_plugin.py` & `cloud_pak_operations_cli-0.7.2/cpo/lib/dependency_manager/plugins/ibm_cloud_terraform_provider_plugin.py`

 * *Files identical despite different names*

### Comparing `cloud-pak-operations-cli-0.7.1/cpo/lib/dependency_manager/plugins/openshift/openshift_cli_plugin.py` & `cloud_pak_operations_cli-0.7.2/cpo/lib/dependency_manager/plugins/openshift/openshift_cli_plugin.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,30 +1,28 @@
-#  Copyright 2023 IBM Corporation
+#  Copyright 2023, 2024 IBM Corporation
 #
 #  Licensed under the Apache License, Version 2.0 (the "License");
 #  you may not use this file except in compliance with the License.
 #  You may obtain a copy of the License at
 #
 #  http://www.apache.org/licenses/LICENSE-2.0
 #
 #  Unless required by applicable law or agreed to in writing, software
 #  distributed under the License is distributed on an "AS IS" BASIS,
 #  WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 #  See the License for the specific language governing permissions and
 #  limitations under the License.
 
-from typing import Optional
-
 from cpo.lib.dependency_manager.plugins.openshift.openshift_plugin import AbstractOpenShiftPlugIn
 from cpo.utils.operating_system import OperatingSystem
 
 
 class OpenShiftCLIPlugIn(AbstractOpenShiftPlugIn):
     # override
-    def get_binary_name(self) -> Optional[str]:
+    def get_binary_name(self) -> str | None:
         return "oc"
 
     # override
     def get_dependency_alias(self) -> str:
         return "oc"
 
     # override
```

### Comparing `cloud-pak-operations-cli-0.7.1/cpo/lib/dependency_manager/plugins/openshift/openshift_install_plugin.py` & `cloud_pak_operations_cli-0.7.2/cpo/lib/dependency_manager/plugins/openshift/openshift_install_plugin.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-#  Copyright 2023 IBM Corporation
+#  Copyright 2023, 2024 IBM Corporation
 #
 #  Licensed under the Apache License, Version 2.0 (the "License");
 #  you may not use this file except in compliance with the License.
 #  You may obtain a copy of the License at
 #
 #  http://www.apache.org/licenses/LICENSE-2.0
 #
@@ -12,29 +12,27 @@
 #  See the License for the specific language governing permissions and
 #  limitations under the License.
 
 import io
 import re as regex
 import urllib.parse
 
-from typing import Optional
-
 import semver
 
 import cpo.utils.download
 import cpo.utils.operating_system
 
 from cpo.lib.dependency_manager.plugins.openshift.openshift_plugin import AbstractOpenShiftPlugIn
 from cpo.utils.error import CloudPakOperationsCLIException
 from cpo.utils.operating_system import OperatingSystem
 
 
 class OpenShiftInstallPlugIn(AbstractOpenShiftPlugIn):
     # override
-    def get_binary_name(self) -> Optional[str]:
+    def get_binary_name(self) -> str | None:
         return "openshift-install"
 
     # override
     def get_dependency_alias(self) -> str:
         return "openshift-install"
 
     # override
```

### Comparing `cloud-pak-operations-cli-0.7.1/cpo/lib/dependency_manager/plugins/openshift/openshift_plugin.py` & `cloud_pak_operations_cli-0.7.2/cpo/lib/dependency_manager/plugins/openshift/openshift_plugin.py`

 * *Files identical despite different names*

### Comparing `cloud-pak-operations-cli-0.7.1/cpo/lib/dependency_manager/plugins/terraform_plugin.py` & `cloud_pak_operations_cli-0.7.2/cpo/lib/dependency_manager/plugins/terraform_plugin.py`

 * *Files 2% similar despite different names*

```diff
@@ -13,16 +13,14 @@
 #  limitations under the License.
 
 import os
 import pathlib
 import stat
 import urllib.parse
 
-from typing import Optional
-
 import semver
 
 import cpo.config
 import cpo.utils.compression
 import cpo.utils.download
 import cpo.utils.operating_system
 
@@ -53,15 +51,15 @@
         file_name = f"terraform_{str(dependency_version)}_{file_name_suffix}"
         url = f"https://releases.hashicorp.com/terraform/{str(dependency_version)}/{file_name}"
         archive_path = cpo.utils.download.download_file(urllib.parse.urlsplit(url))
 
         self._extract_archive(archive_path, dependency_version.version, operating_system)
 
     # override
-    def get_binary_name(self) -> Optional[str]:
+    def get_binary_name(self) -> str | None:
         return "terraform"
 
     # override
     def get_dependency_alias(self) -> str:
         return "terraform"
 
     # override
```

### Comparing `cloud-pak-operations-cli-0.7.1/cpo/lib/ibm_internal_plugin/ibm_internal_plugin_manager.py` & `cloud_pak_operations_cli-0.7.2/cpo/lib/ibm_internal_plugin/ibm_internal_plugin_manager.py`

 * *Files identical despite different names*

### Comparing `cloud-pak-operations-cli-0.7.1/cpo/lib/ibmcloud/__init__.py` & `cloud_pak_operations_cli-0.7.2/cpo/lib/ibmcloud/__init__.py`

 * *Files identical despite different names*

### Comparing `cloud-pak-operations-cli-0.7.1/cpo/lib/ibmcloud/data/cluster_status.py` & `cloud_pak_operations_cli-0.7.2/cpo/lib/ibmcloud/data/cluster_status.py`

 * *Files identical despite different names*

### Comparing `cloud-pak-operations-cli-0.7.1/cpo/lib/ibmcloud/data/ingress_status.py` & `cloud_pak_operations_cli-0.7.2/cpo/lib/ibmcloud/data/ingress_status.py`

 * *Files identical despite different names*

### Comparing `cloud-pak-operations-cli-0.7.1/cpo/lib/ibmcloud/ibm_cloud_api_manager.py` & `cloud_pak_operations_cli-0.7.2/cpo/lib/ibmcloud/ibm_cloud_api_manager.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-#  Copyright 2022, 2023 IBM Corporation
+#  Copyright 2022, 2024 IBM Corporation
 #
 #  Licensed under the Apache License, Version 2.0 (the "License");
 #  you may not use this file except in compliance with the License.
 #  You may obtain a copy of the License at
 #
 #  http://www.apache.org/licenses/LICENSE-2.0
 #
@@ -15,15 +15,15 @@
 import json
 import logging
 import os
 import re as regex
 import subprocess
 
 from dataclasses import dataclass
-from typing import Any, Final, Optional
+from typing import Any, Final
 
 import cpo.utils.process
 
 from cpo.config import configuration_manager
 from cpo.config.cluster_credentials_manager import cluster_credentials_manager
 from cpo.lib.dependency_manager.dependency_manager import DependencyManager
 from cpo.lib.dependency_manager.plugins.ibm_cloud_cli_plugin import IBMCloudCLIPlugIn
@@ -384,15 +384,15 @@
         """Log in to IBM Cloud interactively"""
 
         login_command_return_code = self._execute_ibmcloud_command_interactively(["login", "--no-region", "--sso"])
 
         if login_command_return_code != 0:
             raise CloudPakOperationsCLIException("Interactive login to IBM Cloud failed.")
 
-    def log_in_using_api_key(self, api_key: Optional[str] = None):
+    def log_in_using_api_key(self, api_key: str | None = None):
         """Log in to IBM Cloud using the given IBM Cloud API key
 
         Parameters
         ----------
         api_key
             IBM Cloud API key
         """
@@ -505,36 +505,36 @@
         return self._execute_ibmcloud_command(
             args,
             capture_output=capture_output,
             check=False,
             print_captured_output=print_captured_output,
         )
 
-    def _read_ibmcloud_config_file_contents(self) -> Optional[Any]:
+    def _read_ibmcloud_config_file_contents(self) -> Any | None:
         """Returns the contents of the credentials file
 
         Returns
         -------
-            Optional[str]
+            str | None
                 contents of the credentials file or None if the credentials file does
                 not exist or is empty
         """
 
         ibmcloud_config_file_path = configuration_manager.get_ibmcloud_data_directory_path() / "config.json"
-        result: Optional[str] = None
+        result: str | None = None
 
         if ibmcloud_config_file_path.exists() and (ibmcloud_config_file_path.stat().st_size != 0):
             with open(ibmcloud_config_file_path) as json_file:
                 result = json.load(json_file)
 
         return result
 
-    _IBMCLOUD_CLI_ERROR_OAUTH_TOKEN_EXPIRED_ERROR_MESSAGE: Final[
-        str
-    ] = "FAILED\nClassic: Login token is expired. Please update tokens using 'ibmcloud login' and try again.*"
+    _IBMCLOUD_CLI_ERROR_OAUTH_TOKEN_EXPIRED_ERROR_MESSAGE: Final[str] = (
+        "FAILED\nClassic: Login token is expired. Please update tokens using 'ibmcloud login' and try again.*"
+    )
 
 
 class PlugInManager:
     """Manages IBM Cloud CLI plug-ins"""
 
     def __init__(self, ibm_cloud_api_manager: IBMCloudAPIManager):
         self._ibm_cloud_api_manager = ibm_cloud_api_manager
```

### Comparing `cloud-pak-operations-cli-0.7.1/cpo/lib/ibmcloud/oc/cluster/__init__.py` & `cloud_pak_operations_cli-0.7.2/cpo/lib/ibmcloud/oc/cluster/__init__.py`

 * *Files identical despite different names*

### Comparing `cloud-pak-operations-cli-0.7.1/cpo/lib/ibmcloud/oc/cluster/ls.py` & `cloud_pak_operations_cli-0.7.2/cpo/lib/ibmcloud/oc/cluster/ls.py`

 * *Files identical despite different names*

### Comparing `cloud-pak-operations-cli-0.7.1/cpo/lib/ibmcloud/oc/cluster/roks_cluster.py` & `cloud_pak_operations_cli-0.7.2/cpo/lib/ibmcloud/oc/cluster/roks_cluster.py`

 * *Files identical despite different names*

### Comparing `cloud-pak-operations-cli-0.7.1/cpo/lib/ibmcloud/oc/cluster/roks_cluster_factory.py` & `cloud_pak_operations_cli-0.7.2/cpo/lib/ibmcloud/oc/cluster/roks_cluster_factory.py`

 * *Files identical despite different names*

### Comparing `cloud-pak-operations-cli-0.7.1/cpo/lib/jmespath.py` & `cloud_pak_operations_cli-0.7.2/cpo/lib/jmespath.py`

 * *Files identical despite different names*

### Comparing `cloud-pak-operations-cli-0.7.1/cpo/lib/openshift/cluster/__init__.py` & `cloud_pak_operations_cli-0.7.2/cpo/lib/openshift/cluster/__init__.py`

 * *Files identical despite different names*

### Comparing `cloud-pak-operations-cli-0.7.1/cpo/lib/openshift/cluster/generic_cluster.py` & `cloud_pak_operations_cli-0.7.2/cpo/lib/openshift/cluster/generic_cluster.py`

 * *Files identical despite different names*

### Comparing `cloud-pak-operations-cli-0.7.1/cpo/lib/openshift/cluster/generic_cluster_factory.py` & `cloud_pak_operations_cli-0.7.2/cpo/lib/openshift/cluster/generic_cluster_factory.py`

 * *Files identical despite different names*

### Comparing `cloud-pak-operations-cli-0.7.1/cpo/lib/openshift/credentials/cluster_based_user_credentials.py` & `cloud_pak_operations_cli-0.7.2/cpo/lib/openshift/credentials/cluster_based_user_credentials.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,37 +1,37 @@
-#  Copyright 2021, 2023 IBM Corporation
+#  Copyright 2021, 2024 IBM Corporation
 #
 #  Licensed under the Apache License, Version 2.0 (the "License");
 #  you may not use this file except in compliance with the License.
 #  You may obtain a copy of the License at
 #
 #  http://www.apache.org/licenses/LICENSE-2.0
 #
 #  Unless required by applicable law or agreed to in writing, software
 #  distributed under the License is distributed on an "AS IS" BASIS,
 #  WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 #  See the License for the specific language governing permissions and
 #  limitations under the License.
 
-from typing import Optional
-
 from cpo.config.cluster_credentials_manager import cluster_credentials_manager
 from cpo.lib.cluster.cluster import AbstractCluster
 from cpo.lib.openshift.credentials.user_credentials import UserCredentials
 
 
 class ClusterBasedUserCredentials(UserCredentials):
-    def __init__(self, cluster: AbstractCluster, insecure_skip_tls_verify: Optional[bool] = None):
+    def __init__(self, cluster: AbstractCluster, insecure_skip_tls_verify: bool | None = None):
         super().__init__(
             cluster.get_server(),
             cluster.get_username(),
             cluster.get_password(),
-            insecure_skip_tls_verify
-            if insecure_skip_tls_verify is not None
-            else self._get_insecure_skip_tls_verify_from_cluster_data(cluster),
+            (
+                insecure_skip_tls_verify
+                if insecure_skip_tls_verify is not None
+                else self._get_insecure_skip_tls_verify_from_cluster_data(cluster)
+            ),
         )
 
         self._cluster = cluster
 
     # override
     def get_access_token(self, force_refresh_if_possible: bool = False) -> str:
         if "token" not in self._cluster.get_cluster_data() or force_refresh_if_possible:
```

### Comparing `cloud-pak-operations-cli-0.7.1/cpo/lib/openshift/credentials/credentials.py` & `cloud_pak_operations_cli-0.7.2/cpo/lib/openshift/credentials/credentials.py`

 * *Files identical despite different names*

### Comparing `cloud-pak-operations-cli-0.7.1/cpo/lib/openshift/credentials/token_credentials.py` & `cloud_pak_operations_cli-0.7.2/cpo/lib/openshift/credentials/token_credentials.py`

 * *Files identical despite different names*

### Comparing `cloud-pak-operations-cli-0.7.1/cpo/lib/openshift/credentials/user_credentials.py` & `cloud_pak_operations_cli-0.7.2/cpo/lib/openshift/credentials/user_credentials.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-#  Copyright 2021, 2022 IBM Corporation
+#  Copyright 2021, 2024 IBM Corporation
 #
 #  Licensed under the Apache License, Version 2.0 (the "License");
 #  you may not use this file except in compliance with the License.
 #  You may obtain a copy of the License at
 #
 #  http://www.apache.org/licenses/LICENSE-2.0
 #
@@ -11,34 +11,34 @@
 #  WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 #  See the License for the specific language governing permissions and
 #  limitations under the License.
 
 import json
 import urllib.parse
 
-from typing import Final, Optional
+from typing import Final
 
 import requests
 
 from requests.models import Response
 
 from cpo.lib.openshift.credentials.credentials import AbstractCredentials
 from cpo.utils.error import CloudPakOperationsCLIException
 from cpo.utils.network import ScopedInsecureRequestWarningDisabler
 
 
 class UserCredentials(AbstractCredentials):
-    OPENSHIFT_OAUTH_AUTHORIZATION_ENDPOINT: Final[
-        str
-    ] = "{authorization_endpoint}?client_id=openshift-challenging-client&response_type=token"
+    OPENSHIFT_OAUTH_AUTHORIZATION_ENDPOINT: Final[str] = (
+        "{authorization_endpoint}?client_id=openshift-challenging-client&response_type=token"
+    )
 
     def __init__(self, server: str, username: str, password: str, insecure_skip_tls_verify: bool):
         super().__init__(server, insecure_skip_tls_verify)
         self._password = password
-        self._token: Optional[str] = None
+        self._token: str | None = None
         self._username = username
 
     # override
     def get_access_token(self, force_refresh_if_possible: bool = False) -> str:
         if self._token is None or force_refresh_if_possible:
             self.refresh_access_token()
 
@@ -53,15 +53,15 @@
     # override
     def persist_access_token(self, token: str):
         self._token = token
 
     # override
     def refresh_access_token(self):
         authorization_endpoint = self._get_authorization_endpoint()
-        response: Optional[Response] = None
+        response: Response | None = None
 
         with ScopedInsecureRequestWarningDisabler(self._insecure_skip_tls_verify):
             response = requests.get(
                 UserCredentials.OPENSHIFT_OAUTH_AUTHORIZATION_ENDPOINT.format(
                     authorization_endpoint=authorization_endpoint
                 ),
                 allow_redirects=False,
@@ -90,15 +90,15 @@
 
         Returns
         -------
         str
             OAuth authorization endpoint returned by the OAuth server
         """
 
-        response: Optional[Response] = None
+        response: Response | None = None
 
         with ScopedInsecureRequestWarningDisabler(self._insecure_skip_tls_verify):
             response = requests.get(
                 f"{self._server}/.well-known/oauth-authorization-server",
                 verify=not self._insecure_skip_tls_verify,
             )
```

### Comparing `cloud-pak-operations-cli-0.7.1/cpo/lib/openshift/data/global_pull_secret_data.py` & `cloud_pak_operations_cli-0.7.2/cpo/lib/openshift/data/global_pull_secret_data.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-#  Copyright 2021, 2023 IBM Corporation
+#  Copyright 2021, 2024 IBM Corporation
 #
 #  Licensed under the Apache License, Version 2.0 (the "License");
 #  you may not use this file except in compliance with the License.
 #  You may obtain a copy of the License at
 #
 #  http://www.apache.org/licenses/LICENSE-2.0
 #
@@ -12,15 +12,15 @@
 #  See the License for the specific language governing permissions and
 #  limitations under the License.
 
 import base64
 import json
 import re as regex
 
-from typing import Any, Optional
+from typing import Any
 
 import click
 import jmespath
 
 from tabulate import tabulate
 
 from cpo.lib.openshift.types.auths_dict import AuthDict, AuthsDict
@@ -114,15 +114,15 @@
                 auth_list_element: list[str] = [image_registry, search_result.group(1), image_registry_password]
 
                 auth_list.append(auth_list_element)
 
             auth_list.sort(key=lambda auth_list_element: auth_list_element[0])
             click.echo(tabulate(auth_list, headers=["registry location", "username", "password"]))
 
-    def get_credentials(self, registry_location: str) -> Optional[Credentials]:
+    def get_credentials(self, registry_location: str) -> Credentials | None:
         """Returns credentials for the given registry location
 
         Parameters
         ----------
         registry_location
             registry location for which credentials shall be returned
```

### Comparing `cloud-pak-operations-cli-0.7.1/cpo/lib/openshift/nfs/nfs_subdir_external_provisioner.py` & `cloud_pak_operations_cli-0.7.2/cpo/lib/openshift/nfs/nfs_subdir_external_provisioner.py`

 * *Files identical despite different names*

### Comparing `cloud-pak-operations-cli-0.7.1/cpo/lib/openshift/oc.py` & `cloud_pak_operations_cli-0.7.2/cpo/lib/openshift/oc.py`

 * *Files identical despite different names*

### Comparing `cloud-pak-operations-cli-0.7.1/cpo/lib/openshift/openshift_api_manager.py` & `cloud_pak_operations_cli-0.7.2/cpo/lib/openshift/openshift_api_manager.py`

 * *Files 2% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 #  distributed under the License is distributed on an "AS IS" BASIS,
 #  WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 #  See the License for the specific language governing permissions and
 #  limitations under the License.
 
 import logging
 
-from typing import Any, Callable, Optional
+from typing import Any, Callable
 
 import semver
 import urllib3.exceptions
 
 from kubernetes import client, config, watch
 
 import cpo.lib.jmespath
@@ -558,29 +558,29 @@
             catalog sources
         """
 
         return self.execute_kubernetes_client(self._get_catalog_sources, project=project)
 
     def get_namespaced_custom_resource_if_exists(
         self, project: str, name: str, kind_metadata: KindMetadata
-    ) -> Optional[Any]:
+    ) -> Any | None:
         """Returns custom resource
 
         Parameters
         ----------
         project
             project to be searched for custom resource
         name
             name of the custom resource to be returned
         kind_metadata
             kind metadata of the custom resource
 
         Returns
         -------
-        Optional[Any]
+        Any | None
             custom resource or None if it does not exist
         """
 
         return self.execute_kubernetes_client(
             self._get_namespaced_custom_resource_if_exists, kind_metadata=kind_metadata, name=name, project=project
         )
 
@@ -885,15 +885,15 @@
         )
 
     def wait_for_namespaced_custom_resource(
         self,
         project: str,
         kind_metadata: KindMetadata,
         log_callback: Callable[[str], None],
-        success_callback: Callable[..., Optional[CustomResourceEventResult]],
+        success_callback: Callable[..., CustomResourceEventResult | None],
         **kwargs,
     ) -> CustomResourceEventResult:
         """Waits for a specific custom resource of the given kind to be created in
         the given project
 
         The passed callback is used for checking wheter a created custom resource
         of the given kind is the sought-after custom resource.
@@ -1189,15 +1189,15 @@
         assert isinstance(version_info.major, str)
         assert isinstance(version_info.minor, str)
 
         return semver.Version(int(version_info.major), int(version_info.minor))
 
     def _get_namespaced_custom_resource_if_exists(self, project: str, name: str, kind_metadata: KindMetadata) -> Any:
         custom_objects_api = client.CustomObjectsApi()
-        custom_resource: Optional[Any] = None
+        custom_resource: Any | None = None
 
         try:
             custom_resource = custom_objects_api.get_namespaced_custom_object(
                 kind_metadata.group, kind_metadata.version, project, kind_metadata.plural, name
             )
         except client.ApiException as exception:
             if exception.status != 404:
@@ -1356,15 +1356,15 @@
         **kwargs,
     ):
         custom_objects_api = client.CustomObjectsApi()
         succeeded = False
 
         while not succeeded:
             try:
-                resource_version: Optional[str] = None
+                resource_version: str | None = None
                 w = watch.Watch()
 
                 for event in w.stream(
                     custom_objects_api.list_cluster_custom_object,
                     kind_metadata.group,
                     kind_metadata.version,
                     kind_metadata.plural,
@@ -1382,23 +1382,23 @@
                 self._handle_protocol_error(exception, log_callback)
 
     def _wait_for_namespaced_custom_resource(
         self,
         project: str,
         kind_metadata: KindMetadata,
         log_callback: Callable[[str], None],
-        success_callback: Callable[..., Optional[CustomResourceEventResult]],
+        success_callback: Callable[..., CustomResourceEventResult | None],
         **kwargs,
     ) -> CustomResourceEventResult:
         custom_objects_api = client.CustomObjectsApi()
-        custom_resource_event_result: Optional[CustomResourceEventResult] = None
+        custom_resource_event_result: CustomResourceEventResult | None = None
 
         while custom_resource_event_result is None:
             try:
-                resource_version: Optional[str] = None
+                resource_version: str | None = None
                 w = watch.Watch()
 
                 for event in w.stream(
                     custom_objects_api.list_namespaced_custom_object,
                     kind_metadata.group,
                     kind_metadata.version,
                     project,
```

### Comparing `cloud-pak-operations-cli-0.7.1/cpo/lib/openshift/openshift_install/openshift_installation_manager.py` & `cloud_pak_operations_cli-0.7.2/cpo/lib/openshift/openshift_install/openshift_installation_manager.py`

 * *Files identical despite different names*

### Comparing `cloud-pak-operations-cli-0.7.1/cpo/lib/openshift/openshift_install/openshift_installation_manager_plugin.py` & `cloud_pak_operations_cli-0.7.2/cpo/lib/openshift/openshift_install/openshift_installation_manager_plugin.py`

 * *Files identical despite different names*

### Comparing `cloud-pak-operations-cli-0.7.1/cpo/lib/openshift/openshift_install/types/architecture.py` & `cloud_pak_operations_cli-0.7.2/cpo/lib/openshift/openshift_install/types/architecture.py`

 * *Files identical despite different names*

### Comparing `cloud-pak-operations-cli-0.7.1/cpo/lib/openshift/types/auths_dict.py` & `cloud_pak_operations_cli-0.7.2/cpo/lib/openshift/types/auths_dict.py`

 * *Files identical despite different names*

### Comparing `cloud-pak-operations-cli-0.7.1/cpo/lib/openshift/types/catalog_source.py` & `cloud_pak_operations_cli-0.7.2/cpo/lib/openshift/types/catalog_source.py`

 * *Files identical despite different names*

### Comparing `cloud-pak-operations-cli-0.7.1/cpo/lib/openshift/types/credentials.py` & `cloud_pak_operations_cli-0.7.2/cpo/lib/openshift/types/credentials.py`

 * *Files identical despite different names*

### Comparing `cloud-pak-operations-cli-0.7.1/cpo/lib/openshift/types/custom_resource.py` & `cloud_pak_operations_cli-0.7.2/cpo/lib/openshift/types/custom_resource.py`

 * *Files identical despite different names*

### Comparing `cloud-pak-operations-cli-0.7.1/cpo/lib/openshift/types/custom_resource_event_result.py` & `cloud_pak_operations_cli-0.7.2/cpo/lib/openshift/types/kind_metadata.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,22 +1,23 @@
-#  Copyright 2022 IBM Corporation
+#  Copyright 2021 IBM Corporation
 #
 #  Licensed under the Apache License, Version 2.0 (the "License");
 #  you may not use this file except in compliance with the License.
 #  You may obtain a copy of the License at
 #
 #  http://www.apache.org/licenses/LICENSE-2.0
 #
 #  Unless required by applicable law or agreed to in writing, software
 #  distributed under the License is distributed on an "AS IS" BASIS,
 #  WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 #  See the License for the specific language governing permissions and
 #  limitations under the License.
 
 from dataclasses import dataclass
-from typing import Optional
 
 
 @dataclass
-class CustomResourceEventResult:
-    succeeded: bool
-    message: Optional[str] = None
+class KindMetadata:
+    group: str
+    kind: str
+    plural: str
+    version: str
```

### Comparing `cloud-pak-operations-cli-0.7.1/cpo/lib/openshift/types/get_pod_entry.py` & `cloud_pak_operations_cli-0.7.2/cpo/lib/openshift/types/get_pod_entry.py`

 * *Files identical despite different names*

### Comparing `cloud-pak-operations-cli-0.7.1/cpo/lib/openshift/types/kind_metadata.py` & `cloud_pak_operations_cli-0.7.2/cpo/lib/openshift/types/service_account.py`

 * *Files 18% similar despite different names*

```diff
@@ -8,16 +8,22 @@
 #
 #  Unless required by applicable law or agreed to in writing, software
 #  distributed under the License is distributed on an "AS IS" BASIS,
 #  WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 #  See the License for the specific language governing permissions and
 #  limitations under the License.
 
-from dataclasses import dataclass
+from typing import TypedDict
 
+from cpo.lib.openshift.types.object_meta import ObjectMeta
 
-@dataclass
-class KindMetadata:
-    group: str
+
+class ServiceAccount(TypedDict):
+    """
+    Notes
+    -----
+    https://docs.openshift.com/container-platform/latest/rest_api/security_apis/serviceaccount-core-v1.html#serviceaccount-core-v1
+    """
+
+    apiVersion: str
     kind: str
-    plural: str
-    version: str
+    metadata: ObjectMeta
```

### Comparing `cloud-pak-operations-cli-0.7.1/cpo/lib/openshift/types/object_meta.py` & `cloud_pak_operations_cli-0.7.2/cpo/lib/openshift/types/object_meta.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,26 +1,26 @@
-#  Copyright 2021, 2023 IBM Corporation
+#  Copyright 2021, 2024 IBM Corporation
 #
 #  Licensed under the Apache License, Version 2.0 (the "License");
 #  you may not use this file except in compliance with the License.
 #  You may obtain a copy of the License at
 #
 #  http://www.apache.org/licenses/LICENSE-2.0
 #
 #  Unless required by applicable law or agreed to in writing, software
 #  distributed under the License is distributed on an "AS IS" BASIS,
 #  WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 #  See the License for the specific language governing permissions and
 #  limitations under the License.
 
-from typing import Optional, TypedDict
+from typing import TypedDict
 
 
 class ObjectMetaOptional(TypedDict, total=False):
-    creationTimestamp: Optional[str]
+    creationTimestamp: str | None
     labels: dict[str, str]
     namespace: str
 
 
 class ObjectMetaRequired(TypedDict):
     name: str
```

### Comparing `cloud-pak-operations-cli-0.7.1/cpo/lib/openshift/types/operator_group.py` & `cloud_pak_operations_cli-0.7.2/cpo/lib/openshift/types/operator_group.py`

 * *Files identical despite different names*

### Comparing `cloud-pak-operations-cli-0.7.1/cpo/lib/openshift/types/role.py` & `cloud_pak_operations_cli-0.7.2/cpo/lib/openshift/types/role.py`

 * *Files identical despite different names*

### Comparing `cloud-pak-operations-cli-0.7.1/cpo/lib/openshift/types/role_binding.py` & `cloud_pak_operations_cli-0.7.2/cpo/lib/openshift/types/role_binding.py`

 * *Files identical despite different names*

### Comparing `cloud-pak-operations-cli-0.7.1/cpo/lib/openshift/types/role_rule.py` & `cloud_pak_operations_cli-0.7.2/cpo/lib/openshift/types/role_rule.py`

 * *Files identical despite different names*

### Comparing `cloud-pak-operations-cli-0.7.1/cpo/lib/openshift/types/service_account.py` & `cloud_pak_operations_cli-0.7.2/cpo/utils/debugger.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,29 +1,35 @@
-#  Copyright 2021 IBM Corporation
+#  Copyright 2021, 2023 IBM Corporation
 #
 #  Licensed under the Apache License, Version 2.0 (the "License");
 #  you may not use this file except in compliance with the License.
 #  You may obtain a copy of the License at
 #
 #  http://www.apache.org/licenses/LICENSE-2.0
 #
 #  Unless required by applicable law or agreed to in writing, software
 #  distributed under the License is distributed on an "AS IS" BASIS,
 #  WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 #  See the License for the specific language governing permissions and
 #  limitations under the License.
 
-from typing import TypedDict
+import inspect
+import os
 
-from cpo.lib.openshift.types.object_meta import ObjectMeta
 
+def is_debugpy_running() -> bool:
+    """Returns whether debugpy is running
 
-class ServiceAccount(TypedDict):
-    """
-    Notes
-    -----
-    https://docs.openshift.com/container-platform/latest/rest_api/security_apis/serviceaccount-core-v1.html#serviceaccount-core-v1
+    Visual Studio Code uses debugpy (https://github.com/microsoft/debugpy)
+    as the default Python debugger.
+
+    Returns
+    -------
+    bool
+        True, if debugpy is running
     """
 
-    apiVersion: str
-    kind: str
-    metadata: ObjectMeta
+    for frame in inspect.stack():
+        if frame.filename.endswith(f"debugpy{os.sep}__main__.py"):
+            return True
+
+    return False
```

### Comparing `cloud-pak-operations-cli-0.7.1/cpo/lib/openshift/types/subscription.py` & `cloud_pak_operations_cli-0.7.2/cpo/lib/openshift/types/subscription.py`

 * *Files identical despite different names*

### Comparing `cloud-pak-operations-cli-0.7.1/cpo/lib/openshift/utils/click.py` & `cloud_pak_operations_cli-0.7.2/cpo/lib/openshift/utils/click.py`

 * *Files identical despite different names*

### Comparing `cloud-pak-operations-cli-0.7.1/cpo/lib/plugin_manager/package_data.py` & `cloud_pak_operations_cli-0.7.2/cpo/lib/plugin_manager/package_data.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-#  Copyright 2021, 2023 IBM Corporation
+#  Copyright 2021, 2024 IBM Corporation
 #
 #  Licensed under the Apache License, Version 2.0 (the "License");
 #  you may not use this file except in compliance with the License.
 #  You may obtain a copy of the License at
 #
 #  http://www.apache.org/licenses/LICENSE-2.0
 #
@@ -11,32 +11,31 @@
 #  WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 #  See the License for the specific language governing permissions and
 #  limitations under the License.
 
 import pathlib
 
 from dataclasses import dataclass
-from typing import Optional
 
 
 @dataclass
 class PackageElementDescriptor:
-    command_hierarchy_path: Optional[str]
+    command_hierarchy_path: str | None
     distribution_package_name: str
     name: str
     path: pathlib.Path
 
 
 class PackageData:
     """Stores descriptors for modules and subpackages within a
     package"""
 
     @staticmethod
     def get_package_data(
-        distribution_package_name: str, command_hierarchy_path: Optional[str], package_path: pathlib.Path
+        distribution_package_name: str, command_hierarchy_path: str | None, package_path: pathlib.Path
     ) -> "PackageData":
         """Creates an object describing modules and subpackages within the
         package with the given path
 
         Parameters
         ----------
         distribution_package_name
```

### Comparing `cloud-pak-operations-cli-0.7.1/cpo/lib/plugin_manager/plugin_manager.py` & `cloud_pak_operations_cli-0.7.2/cpo/lib/plugin_manager/plugin_manager.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-#  Copyright 2021, 2023 IBM Corporation
+#  Copyright 2021, 2024 IBM Corporation
 #
 #  Licensed under the Apache License, Version 2.0 (the "License");
 #  you may not use this file except in compliance with the License.
 #  You may obtain a copy of the License at
 #
 #  http://www.apache.org/licenses/LICENSE-2.0
 #
@@ -13,15 +13,14 @@
 #  limitations under the License.
 
 import logging
 import pathlib
 
 from importlib.metadata import entry_points
 from types import ModuleType
-from typing import Optional
 
 from cpo.lib.plugin_manager.package_data import PackageData
 from cpo.utils.error import CloudPakOperationsCLIException
 
 logger = logging.getLogger(__name__)
 
 
@@ -62,15 +61,15 @@
 
     Notes
     -----
     https://packaging.python.org/guides/creating-and-discovering-plugins/#using-package-metadata
     """
 
     def __init__(self):
-        self._package_data_dict: Optional[dict[str, PackageData]] = None
+        self._package_data_dict: dict[str, PackageData] | None = None
 
     def reload(self):
         """Reloads CLI plug-ins"""
 
         self._package_data_dict = None
 
         self._load_plugins_if_required()
```

### Comparing `cloud-pak-operations-cli-0.7.1/cpo/scripts/get_current_cluster_alias.py` & `cloud_pak_operations_cli-0.7.2/cpo/scripts/get_current_cluster_alias.py`

 * *Files identical despite different names*

### Comparing `cloud-pak-operations-cli-0.7.1/cpo/utils/compression.py` & `cloud_pak_operations_cli-0.7.2/cpo/utils/compression.py`

 * *Files identical despite different names*

### Comparing `cloud-pak-operations-cli-0.7.1/cpo/utils/download.py` & `cloud_pak_operations_cli-0.7.2/cpo/utils/download.py`

 * *Files identical despite different names*

### Comparing `cloud-pak-operations-cli-0.7.1/cpo/utils/error.py` & `cloud_pak_operations_cli-0.7.2/cpo/utils/error.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-#  Copyright 2022 IBM Corporation
+#  Copyright 2022, 2024 IBM Corporation
 #
 #  Licensed under the Apache License, Version 2.0 (the "License");
 #  you may not use this file except in compliance with the License.
 #  You may obtain a copy of the License at
 #
 #  http://www.apache.org/licenses/LICENSE-2.0
 #
@@ -10,21 +10,19 @@
 #  distributed under the License is distributed on an "AS IS" BASIS,
 #  WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 #  See the License for the specific language governing permissions and
 #  limitations under the License.
 
 import re as regex
 
-from typing import Optional
-
 import colorama
 
 
 class CloudPakOperationsCLIException(Exception):
-    def __init__(self, error_message: str, stderr: Optional[str] = None, stdout: Optional[str] = None):
+    def __init__(self, error_message: str, stderr: str | None = None, stdout: str | None = None):
         super().__init__(error_message)
         self._error_message = error_message[7:] if error_message.startswith("Error: ") else error_message
         self._stderr = stderr
         self._stdout = stdout
 
     def __str__(self):
         output = self._get_highlighted_str(self._error_message)
@@ -44,19 +42,19 @@
         return output
 
     @property
     def error_message(self) -> str:
         return self._error_message
 
     @property
-    def stderr(self) -> Optional[str]:
+    def stderr(self) -> str | None:
         return self._stderr
 
     @property
-    def stdout(self) -> Optional[str]:
+    def stdout(self) -> str | None:
         return self._stdout
 
     def _get_highlighted_str(self, str: str) -> str:
         return f"{colorama.Style.BRIGHT}{str}{colorama.Style.RESET_ALL}"
 
 
 class IBMCloudException(CloudPakOperationsCLIException):
@@ -84,15 +82,15 @@
         if search_result is not None:
             output = search_result.group(1)
         else:
             output = error_message
 
         return output
 
-    def __init__(self, error_message, stderr: Optional[str] = None, stdout: Optional[str] = None):
+    def __init__(self, error_message, stderr: str | None = None, stdout: str | None = None):
         super().__init__(error_message, stderr, stdout)
 
 
 class JmespathPathExpressionNotFoundException(CloudPakOperationsCLIException):
     def __init__(self, expresion):
         super().__init__(f"Jmespath expression not found ({expresion})")
```

### Comparing `cloud-pak-operations-cli-0.7.1/cpo/utils/file.py` & `cloud_pak_operations_cli-0.7.2/cpo/utils/file.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-#  Copyright 2021, 2022 IBM Corporation
+#  Copyright 2021, 2024 IBM Corporation
 #
 #  Licensed under the Apache License, Version 2.0 (the "License");
 #  you may not use this file except in compliance with the License.
 #  You may obtain a copy of the License at
 #
 #  http://www.apache.org/licenses/LICENSE-2.0
 #
@@ -12,24 +12,23 @@
 #  See the License for the specific language governing permissions and
 #  limitations under the License.
 
 import os
 import pathlib
 
 from enum import Enum
-from typing import Optional
 
 
 class FileType(Enum):
     Directory = 1
     RegularFile = 2
 
 
-def get_relative_path(path: os.PathLike, subpath: pathlib.Path) -> Optional[pathlib.Path]:
-    relative_path: Optional[pathlib.Path] = None
+def get_relative_path(path: os.PathLike, subpath: pathlib.Path) -> pathlib.Path | None:
+    relative_path: pathlib.Path | None = None
 
     try:
         relative_path = subpath.relative_to(path)
     except ValueError:
         pass
 
     return relative_path
```

### Comparing `cloud-pak-operations-cli-0.7.1/cpo/utils/importlib.py` & `cloud_pak_operations_cli-0.7.2/cpo/utils/importlib.py`

 * *Files identical despite different names*

### Comparing `cloud-pak-operations-cli-0.7.1/cpo/utils/logging.py` & `cloud_pak_operations_cli-0.7.2/cpo/utils/logging.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-#  Copyright 2021, 2023 IBM Corporation
+#  Copyright 2021, 2024 IBM Corporation
 #
 #  Licensed under the Apache License, Version 2.0 (the "License");
 #  you may not use this file except in compliance with the License.
 #  You may obtain a copy of the License at
 #
 #  http://www.apache.org/licenses/LICENSE-2.0
 #
@@ -11,15 +11,15 @@
 #  WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 #  See the License for the specific language governing permissions and
 #  limitations under the License.
 
 import logging
 import time
 
-from typing import Any, Callable, Optional
+from typing import Any, Callable
 
 import click
 
 from halo import Halo
 
 
 class ClickLoggingFormatter(logging.Formatter):
@@ -70,15 +70,15 @@
 
 
 class ClickLoggingHandler(logging.Handler):
     """Click-based log handler"""
 
     def __init__(self):
         super().__init__()
-        self._spinner: Optional[Halo] = None
+        self._spinner: Halo | None = None
 
     def emit(self, record: logging.LogRecord):
         """Prints the given log record using click.echo()
 
         Parameters
         ----------
         record
```

### Comparing `cloud-pak-operations-cli-0.7.1/cpo/utils/network.py` & `cloud_pak_operations_cli-0.7.2/cpo/utils/network.py`

 * *Files identical despite different names*

### Comparing `cloud-pak-operations-cli-0.7.1/cpo/utils/operating_system.py` & `cloud_pak_operations_cli-0.7.2/cpo/utils/operating_system.py`

 * *Files identical despite different names*

### Comparing `cloud-pak-operations-cli-0.7.1/cpo/utils/process.py` & `cloud_pak_operations_cli-0.7.2/cpo/utils/process.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-#  Copyright 2021, 2023 IBM Corporation
+#  Copyright 2021, 2024 IBM Corporation
 #
 #  Licensed under the Apache License, Version 2.0 (the "License");
 #  you may not use this file except in compliance with the License.
 #  You may obtain a copy of the License at
 #
 #  http://www.apache.org/licenses/LICENSE-2.0
 #
@@ -13,15 +13,15 @@
 #  limitations under the License.
 
 import asyncio
 import logging
 import os
 import pathlib
 
-from typing import Callable, Optional
+from typing import Callable
 
 import click
 
 from cpo.utils.error import CloudPakOperationsCLIException
 
 
 class ProcessResult:
@@ -84,15 +84,15 @@
         requested)
     """
 
     command = [str(program)] + args
 
     logging.debug(f"Executing command: {' '.join(command)}")
 
-    return_code: Optional[int] = None
+    return_code: int | None = None
     stderr_buffer: list[str] = []
     stdout_buffer: list[str] = []
 
     if capture_output:
         return_code = asyncio.run(
             _create_subprocess_and_capture_output(
                 program,
@@ -220,14 +220,14 @@
 def _process_stdout_output(line: str, buffer: list[str], print_captured_output: bool):
     if print_captured_output:
         click.echo(line, nl=False)
 
     buffer.append(line.rstrip())
 
 
-async def _read_stream(stream: Optional[asyncio.StreamReader], callback: Callable[[str], None]):
+async def _read_stream(stream: asyncio.StreamReader | None, callback: Callable[[str], None]):
     if stream is not None:
         while True:
             if len(line := await stream.readline()) != 0:
                 callback(line.decode())
             else:
                 break
```

### Comparing `cloud-pak-operations-cli-0.7.1/cpo/utils/ssh.py` & `cloud_pak_operations_cli-0.7.2/cpo/utils/ssh.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-#  Copyright 2021, 2023 IBM Corporation
+#  Copyright 2021, 2024 IBM Corporation
 #
 #  Licensed under the Apache License, Version 2.0 (the "License");
 #  you may not use this file except in compliance with the License.
 #  You may obtain a copy of the License at
 #
 #  http://www.apache.org/licenses/LICENSE-2.0
 #
@@ -12,15 +12,14 @@
 #  See the License for the specific language governing permissions and
 #  limitations under the License.
 
 import logging
 import pathlib
 
 from abc import ABC, abstractmethod
-from typing import Optional
 
 import asyncssh
 import click
 import colorama
 
 from cpo.utils.error import CloudPakOperationsCLIException
 
@@ -46,15 +45,15 @@
 
         Parameters
         ----------
         hostname
             name of the remote host to which an SSH connection shall be established
         """
 
-        self._connection: Optional[asyncssh.SSHClientConnection] = None
+        self._connection: asyncssh.SSHClientConnection | None = None
         self._hostname = hostname
 
     async def __aenter__(self):
         return self
 
     async def __aexit__(self, exc_type, exc_value, traceback):
         await self.disconnect()
@@ -149,15 +148,15 @@
           interleaved although it should be:
 
           - https://github.com/ronf/asyncssh/issues/58
           - https://github.com/ronf/asyncssh/issues/231
         """
 
         def __init__(self):
-            self._channel: Optional[asyncssh.SSHClientChannel] = None
+            self._channel: asyncssh.SSHClientChannel | None = None
             self._received_data = ""
 
         # override
         def check_exit_status(self):
             """Checks the exit status of a command executed on a remote host and
             raises an asyncssh.ProcessError exception if it is not 0"""
```

### Comparing `cloud-pak-operations-cli-0.7.1/cpo/utils/wait.py` & `cloud_pak_operations_cli-0.7.2/cpo/utils/wait.py`

 * *Files identical despite different names*

### Comparing `cloud-pak-operations-cli-0.7.1/pyproject.toml` & `cloud_pak_operations_cli-0.7.2/pyproject.toml`

 * *Files identical despite different names*

