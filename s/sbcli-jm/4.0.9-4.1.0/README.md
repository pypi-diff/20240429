# Comparing `tmp/sbcli_jm-4.0.9.zip` & `tmp/sbcli_jm-4.1.0.zip`

## zipinfo {}

```diff
@@ -1,146 +1,146 @@
-Zip file size: 180151 bytes, number of entries: 144
-drwxr-xr-x  2.0 unx        0 b- stor 24-Apr-25 09:24 sbcli_jm-4.0.9/
-drwxr-xr-x  2.0 unx        0 b- stor 24-Apr-25 09:24 sbcli_jm-4.0.9/simplyblock_cli/
-drwxr-xr-x  2.0 unx        0 b- stor 24-Apr-25 09:24 sbcli_jm-4.0.9/sbcli_jm.egg-info/
-drwxr-xr-x  2.0 unx        0 b- stor 24-Apr-25 09:24 sbcli_jm-4.0.9/simplyblock_core/
-drwxr-xr-x  2.0 unx        0 b- stor 24-Apr-25 09:24 sbcli_jm-4.0.9/simplyblock_web/
--rw-r--r--  2.0 unx     2251 b- defN 24-Apr-25 09:24 sbcli_jm-4.0.9/setup.py
--rw-r--r--  2.0 unx      740 b- defN 24-Apr-25 09:24 sbcli_jm-4.0.9/README.md
--rw-r--r--  2.0 unx      150 b- defN 24-Apr-25 09:24 sbcli_jm-4.0.9/env_var
--rw-r--r--  2.0 unx       84 b- defN 24-Apr-25 09:24 sbcli_jm-4.0.9/pyproject.toml
--rw-r--r--  2.0 unx       38 b- defN 24-Apr-25 09:24 sbcli_jm-4.0.9/setup.cfg
--rw-r--r--  2.0 unx     1138 b- defN 24-Apr-25 09:24 sbcli_jm-4.0.9/PKG-INFO
--rw-r--r--  2.0 unx    77093 b- defN 24-Apr-25 09:24 sbcli_jm-4.0.9/simplyblock_cli/cli.py
--rw-r--r--  2.0 unx      357 b- defN 24-Apr-25 09:24 sbcli_jm-4.0.9/simplyblock_cli/main.py
--rw-r--r--  2.0 unx        1 b- defN 24-Apr-25 09:24 sbcli_jm-4.0.9/sbcli_jm.egg-info/dependency_links.txt
--rw-r--r--  2.0 unx     5067 b- defN 24-Apr-25 09:24 sbcli_jm-4.0.9/sbcli_jm.egg-info/SOURCES.txt
--rw-r--r--  2.0 unx       49 b- defN 24-Apr-25 09:24 sbcli_jm-4.0.9/sbcli_jm.egg-info/top_level.txt
--rw-r--r--  2.0 unx     1138 b- defN 24-Apr-25 09:24 sbcli_jm-4.0.9/sbcli_jm.egg-info/PKG-INFO
--rw-r--r--  2.0 unx       66 b- defN 24-Apr-25 09:24 sbcli_jm-4.0.9/sbcli_jm.egg-info/requires.txt
--rw-r--r--  2.0 unx       54 b- defN 24-Apr-25 09:24 sbcli_jm-4.0.9/sbcli_jm.egg-info/entry_points.txt
-drwxr-xr-x  2.0 unx        0 b- stor 24-Apr-25 09:24 sbcli_jm-4.0.9/simplyblock_core/services/
-drwxr-xr-x  2.0 unx        0 b- stor 24-Apr-25 09:24 sbcli_jm-4.0.9/simplyblock_core/scripts/
-drwxr-xr-x  2.0 unx        0 b- stor 24-Apr-25 09:24 sbcli_jm-4.0.9/simplyblock_core/controllers/
-drwxr-xr-x  2.0 unx        0 b- stor 24-Apr-25 09:24 sbcli_jm-4.0.9/simplyblock_core/models/
--rw-r--r--  2.0 unx    66775 b- defN 24-Apr-25 09:24 sbcli_jm-4.0.9/simplyblock_core/storage_node_ops.py
--rw-r--r--  2.0 unx     1443 b- defN 24-Apr-25 09:24 sbcli_jm-4.0.9/simplyblock_core/constants.py
--rw-r--r--  2.0 unx     3153 b- defN 24-Apr-25 09:24 sbcli_jm-4.0.9/simplyblock_core/mgmt_node_ops.py
--rw-r--r--  2.0 unx     3444 b- defN 24-Apr-25 09:24 sbcli_jm-4.0.9/simplyblock_core/cnode_client.py
--rw-r--r--  2.0 unx      279 b- defN 24-Apr-25 09:24 sbcli_jm-4.0.9/simplyblock_core/shell_utils.py
--rw-r--r--  2.0 unx      938 b- defN 24-Apr-25 09:24 sbcli_jm-4.0.9/simplyblock_core/pci_utils.py
--rw-r--r--  2.0 unx        0 b- defN 24-Apr-25 09:24 sbcli_jm-4.0.9/simplyblock_core/__init__.py
--rw-r--r--  2.0 unx     3416 b- defN 24-Apr-25 09:24 sbcli_jm-4.0.9/simplyblock_core/snode_client.py
--rw-r--r--  2.0 unx     8189 b- defN 24-Apr-25 09:24 sbcli_jm-4.0.9/simplyblock_core/kv_store.py
--rw-r--r--  2.0 unx     7640 b- defN 24-Apr-25 09:24 sbcli_jm-4.0.9/simplyblock_core/utils.py
--rw-r--r--  2.0 unx    23335 b- defN 24-Apr-25 09:24 sbcli_jm-4.0.9/simplyblock_core/cluster_ops.py
--rw-r--r--  2.0 unx     5112 b- defN 24-Apr-25 09:24 sbcli_jm-4.0.9/simplyblock_core/compute_node_ops.py
--rw-r--r--  2.0 unx    21979 b- defN 24-Apr-25 09:24 sbcli_jm-4.0.9/simplyblock_core/rpc_client.py
--rw-r--r--  2.0 unx     7401 b- defN 24-Apr-25 09:24 sbcli_jm-4.0.9/simplyblock_core/distr_controller.py
--rw-r--r--  2.0 unx     2189 b- defN 24-Apr-25 09:24 sbcli_jm-4.0.9/simplyblock_core/services/lvol_monitor.py
--rw-r--r--  2.0 unx     3203 b- defN 24-Apr-25 09:24 sbcli_jm-4.0.9/simplyblock_core/services/caching_node_monitor.py
--rw-r--r--  2.0 unx     5443 b- defN 24-Apr-25 09:24 sbcli_jm-4.0.9/simplyblock_core/services/capacity_collector.py
--rw-r--r--  2.0 unx     5462 b- defN 24-Apr-25 09:24 sbcli_jm-4.0.9/simplyblock_core/services/health_check_service.py
--rw-r--r--  2.0 unx      229 b- defN 24-Apr-25 09:24 sbcli_jm-4.0.9/simplyblock_core/services/service_template.service
--rw-r--r--  2.0 unx     5262 b- defN 24-Apr-25 09:24 sbcli_jm-4.0.9/simplyblock_core/services/lvol_stat_collector.py
--rw-r--r--  2.0 unx      173 b- defN 24-Apr-25 09:24 sbcli_jm-4.0.9/simplyblock_core/services/remove_service.sh
--rw-r--r--  2.0 unx     2410 b- defN 24-Apr-25 09:24 sbcli_jm-4.0.9/simplyblock_core/services/log_agg_service.py
--rw-r--r--  2.0 unx     5123 b- defN 24-Apr-25 09:24 sbcli_jm-4.0.9/simplyblock_core/services/distr_event_collector.py
--rw-r--r--  2.0 unx     7438 b- defN 24-Apr-25 09:24 sbcli_jm-4.0.9/simplyblock_core/services/capacity_and_stats_collector.py
--rw-r--r--  2.0 unx     2423 b- defN 24-Apr-25 09:24 sbcli_jm-4.0.9/simplyblock_core/services/port_stat_collector.py
--rw-r--r--  2.0 unx     2490 b- defN 24-Apr-25 09:24 sbcli_jm-4.0.9/simplyblock_core/services/device_monitor.py
--rw-r--r--  2.0 unx     4118 b- defN 24-Apr-25 09:24 sbcli_jm-4.0.9/simplyblock_core/services/__init__.py
--rw-r--r--  2.0 unx      837 b- defN 24-Apr-25 09:24 sbcli_jm-4.0.9/simplyblock_core/services/install_service.sh
--rw-r--r--  2.0 unx     3003 b- defN 24-Apr-25 09:24 sbcli_jm-4.0.9/simplyblock_core/services/mgmt_node_monitor.py
--rw-r--r--  2.0 unx     2671 b- defN 24-Apr-25 09:24 sbcli_jm-4.0.9/simplyblock_core/services/cap_monitor.py
--rw-r--r--  2.0 unx     6577 b- defN 24-Apr-25 09:24 sbcli_jm-4.0.9/simplyblock_core/services/storage_node_monitor.py
-drwxr-xr-x  2.0 unx        0 b- stor 24-Apr-25 09:24 sbcli_jm-4.0.9/simplyblock_core/scripts/alerting/
-drwxr-xr-x  2.0 unx        0 b- stor 24-Apr-25 09:24 sbcli_jm-4.0.9/simplyblock_core/scripts/dashboards/
--rw-r--r--  2.0 unx      694 b- defN 24-Apr-25 09:24 sbcli_jm-4.0.9/simplyblock_core/scripts/deploy_stack.sh
--rw-r--r--  2.0 unx      152 b- defN 24-Apr-25 09:24 sbcli_jm-4.0.9/simplyblock_core/scripts/set_db_config.sh
--rw-r--r--  2.0 unx     1163 b- defN 24-Apr-25 09:24 sbcli_jm-4.0.9/simplyblock_core/scripts/haproxy.cfg
--rw-r--r--  2.0 unx     8081 b- defN 24-Apr-25 09:24 sbcli_jm-4.0.9/simplyblock_core/scripts/docker-compose-swarm.yml
--rw-r--r--  2.0 unx       54 b- defN 24-Apr-25 09:24 sbcli_jm-4.0.9/simplyblock_core/scripts/db_config_single.sh
--rw-r--r--  2.0 unx     5305 b- defN 24-Apr-25 09:24 sbcli_jm-4.0.9/simplyblock_core/scripts/stack_deploy_wait.sh
--rw-r--r--  2.0 unx      453 b- defN 24-Apr-25 09:24 sbcli_jm-4.0.9/simplyblock_core/scripts/config_docker.sh
--rw-r--r--  2.0 unx     1694 b- defN 24-Apr-25 09:24 sbcli_jm-4.0.9/simplyblock_core/scripts/__init__.py
--rw-r--r--  2.0 unx      311 b- defN 24-Apr-25 09:24 sbcli_jm-4.0.9/simplyblock_core/scripts/clean_local_storage_deploy.sh
--rw-r--r--  2.0 unx      118 b- defN 24-Apr-25 09:24 sbcli_jm-4.0.9/simplyblock_core/scripts/db_config_double.sh
--rw-r--r--  2.0 unx      360 b- defN 24-Apr-25 09:24 sbcli_jm-4.0.9/simplyblock_core/scripts/datasource.yml
--rw-r--r--  2.0 unx       43 b- defN 24-Apr-25 09:24 sbcli_jm-4.0.9/simplyblock_core/scripts/run_ssh.sh
--rw-r--r--  2.0 unx     1438 b- defN 24-Apr-25 09:24 sbcli_jm-4.0.9/simplyblock_core/scripts/install_deps.sh
--rw-r--r--  2.0 unx      187 b- defN 24-Apr-25 09:24 sbcli_jm-4.0.9/simplyblock_core/scripts/prometheus.yml
--rwxr-xr-x  2.0 unx      595 b- defN 24-Apr-25 09:24 sbcli_jm-4.0.9/simplyblock_core/scripts/apply_dashboard.sh
--rw-r--r--  2.0 unx     5860 b- defN 24-Apr-25 09:24 sbcli_jm-4.0.9/simplyblock_core/scripts/alerting/alert_rules.yaml
--rw-r--r--  2.0 unx     1853 b- defN 24-Apr-25 09:24 sbcli_jm-4.0.9/simplyblock_core/scripts/alerting/alert_resources.yaml
--rw-r--r--  2.0 unx    98143 b- defN 24-Apr-25 09:24 sbcli_jm-4.0.9/simplyblock_core/scripts/dashboards/devices.json
--rw-r--r--  2.0 unx    98086 b- defN 24-Apr-25 09:24 sbcli_jm-4.0.9/simplyblock_core/scripts/dashboards/nodes.json
--rw-r--r--  2.0 unx    98031 b- defN 24-Apr-25 09:24 sbcli_jm-4.0.9/simplyblock_core/scripts/dashboards/lvols.json
--rw-r--r--  2.0 unx    98198 b- defN 24-Apr-25 09:24 sbcli_jm-4.0.9/simplyblock_core/scripts/dashboards/cluster.json
--rw-r--r--  2.0 unx    12785 b- defN 24-Apr-25 09:24 sbcli_jm-4.0.9/simplyblock_core/controllers/device_controller.py
--rw-r--r--  2.0 unx     1120 b- defN 24-Apr-25 09:24 sbcli_jm-4.0.9/simplyblock_core/controllers/mgmt_events.py
--rw-r--r--  2.0 unx     1961 b- defN 24-Apr-25 09:24 sbcli_jm-4.0.9/simplyblock_core/controllers/events_controller.py
--rw-r--r--  2.0 unx     1521 b- defN 24-Apr-25 09:24 sbcli_jm-4.0.9/simplyblock_core/controllers/storage_events.py
--rw-r--r--  2.0 unx     1630 b- defN 24-Apr-25 09:24 sbcli_jm-4.0.9/simplyblock_core/controllers/lvol_events.py
--rw-r--r--  2.0 unx    10557 b- defN 24-Apr-25 09:24 sbcli_jm-4.0.9/simplyblock_core/controllers/snapshot_controller.py
--rw-r--r--  2.0 unx     1568 b- defN 24-Apr-25 09:24 sbcli_jm-4.0.9/simplyblock_core/controllers/device_events.py
--rw-r--r--  2.0 unx    10375 b- defN 24-Apr-25 09:24 sbcli_jm-4.0.9/simplyblock_core/controllers/pool_controller.py
--rw-r--r--  2.0 unx        0 b- defN 24-Apr-25 09:24 sbcli_jm-4.0.9/simplyblock_core/controllers/__init__.py
--rw-r--r--  2.0 unx     1900 b- defN 24-Apr-25 09:24 sbcli_jm-4.0.9/simplyblock_core/controllers/cluster_events.py
--rw-r--r--  2.0 unx    22802 b- defN 24-Apr-25 09:24 sbcli_jm-4.0.9/simplyblock_core/controllers/caching_node_controller.py
--rw-r--r--  2.0 unx     1122 b- defN 24-Apr-25 09:24 sbcli_jm-4.0.9/simplyblock_core/controllers/snapshot_events.py
--rw-r--r--  2.0 unx    47314 b- defN 24-Apr-25 09:24 sbcli_jm-4.0.9/simplyblock_core/controllers/lvol_controller.py
--rw-r--r--  2.0 unx    11294 b- defN 24-Apr-25 09:24 sbcli_jm-4.0.9/simplyblock_core/controllers/health_controller.py
--rw-r--r--  2.0 unx      695 b- defN 24-Apr-25 09:24 sbcli_jm-4.0.9/simplyblock_core/controllers/pool_events.py
--rw-r--r--  2.0 unx     1500 b- defN 24-Apr-25 09:24 sbcli_jm-4.0.9/simplyblock_core/models/events.py
--rw-r--r--  2.0 unx      806 b- defN 24-Apr-25 09:24 sbcli_jm-4.0.9/simplyblock_core/models/iface.py
--rw-r--r--  2.0 unx     4846 b- defN 24-Apr-25 09:24 sbcli_jm-4.0.9/simplyblock_core/models/base_model.py
--rw-r--r--  2.0 unx     2579 b- defN 24-Apr-25 09:24 sbcli_jm-4.0.9/simplyblock_core/models/lvol_model.py
--rw-r--r--  2.0 unx      917 b- defN 24-Apr-25 09:24 sbcli_jm-4.0.9/simplyblock_core/models/compute_node.py
--rw-r--r--  2.0 unx      736 b- defN 24-Apr-25 09:24 sbcli_jm-4.0.9/simplyblock_core/models/snapshot.py
--rw-r--r--  2.0 unx     1602 b- defN 24-Apr-25 09:24 sbcli_jm-4.0.9/simplyblock_core/models/pool.py
--rw-r--r--  2.0 unx     1228 b- defN 24-Apr-25 09:24 sbcli_jm-4.0.9/simplyblock_core/models/global_settings.py
--rw-r--r--  2.0 unx     1020 b- defN 24-Apr-25 09:24 sbcli_jm-4.0.9/simplyblock_core/models/port_stat.py
--rw-r--r--  2.0 unx     3471 b- defN 24-Apr-25 09:24 sbcli_jm-4.0.9/simplyblock_core/models/storage_node.py
--rw-r--r--  2.0 unx        0 b- defN 24-Apr-25 09:24 sbcli_jm-4.0.9/simplyblock_core/models/__init__.py
--rw-r--r--  2.0 unx     4242 b- defN 24-Apr-25 09:24 sbcli_jm-4.0.9/simplyblock_core/models/stats.py
--rw-r--r--  2.0 unx     2565 b- defN 24-Apr-25 09:24 sbcli_jm-4.0.9/simplyblock_core/models/cluster.py
--rw-r--r--  2.0 unx     1466 b- defN 24-Apr-25 09:24 sbcli_jm-4.0.9/simplyblock_core/models/mgmt_node.py
--rw-r--r--  2.0 unx     3766 b- defN 24-Apr-25 09:24 sbcli_jm-4.0.9/simplyblock_core/models/caching_node.py
--rw-r--r--  2.0 unx     2132 b- defN 24-Apr-25 09:24 sbcli_jm-4.0.9/simplyblock_core/models/nvme_device.py
-drwxr-xr-x  2.0 unx        0 b- stor 24-Apr-25 09:24 sbcli_jm-4.0.9/simplyblock_web/static/
-drwxr-xr-x  2.0 unx        0 b- stor 24-Apr-25 09:24 sbcli_jm-4.0.9/simplyblock_web/templates/
-drwxr-xr-x  2.0 unx        0 b- stor 24-Apr-25 09:24 sbcli_jm-4.0.9/simplyblock_web/blueprints/
--rw-r--r--  2.0 unx      725 b- defN 24-Apr-25 09:24 sbcli_jm-4.0.9/simplyblock_web/caching_node_app_k8s.py
--rw-r--r--  2.0 unx     5098 b- defN 24-Apr-25 09:24 sbcli_jm-4.0.9/simplyblock_web/node_utils.py
--rw-r--r--  2.0 unx      703 b- defN 24-Apr-25 09:24 sbcli_jm-4.0.9/simplyblock_web/snode_app.py
--rw-r--r--  2.0 unx     1263 b- defN 24-Apr-25 09:24 sbcli_jm-4.0.9/simplyblock_web/app.py
--rw-r--r--  2.0 unx     1638 b- defN 24-Apr-25 09:24 sbcli_jm-4.0.9/simplyblock_web/auth_middleware.py
--rw-r--r--  2.0 unx        0 b- defN 24-Apr-25 09:24 sbcli_jm-4.0.9/simplyblock_web/__init__.py
--rw-r--r--  2.0 unx      717 b- defN 24-Apr-25 09:24 sbcli_jm-4.0.9/simplyblock_web/caching_node_app.py
--rw-r--r--  2.0 unx     2513 b- defN 24-Apr-25 09:24 sbcli_jm-4.0.9/simplyblock_web/utils.py
--rw-r--r--  2.0 unx     1434 b- defN 24-Apr-25 09:24 sbcli_jm-4.0.9/simplyblock_web/node_webapp.py
--rw-r--r--  2.0 unx      507 b- defN 24-Apr-25 09:24 sbcli_jm-4.0.9/simplyblock_web/static/deploy_cnode.yaml
--rw-r--r--  2.0 unx      322 b- defN 24-Apr-25 09:24 sbcli_jm-4.0.9/simplyblock_web/static/tst.py
--rw-r--r--  2.0 unx      434 b- defN 24-Apr-25 09:24 sbcli_jm-4.0.9/simplyblock_web/static/is_up.py
--rw-r--r--  2.0 unx      827 b- defN 24-Apr-25 09:24 sbcli_jm-4.0.9/simplyblock_web/static/delete.py
--rw-r--r--  2.0 unx     1302 b- defN 24-Apr-25 09:24 sbcli_jm-4.0.9/simplyblock_web/static/deploy.py
--rw-r--r--  2.0 unx     1466 b- defN 24-Apr-25 09:24 sbcli_jm-4.0.9/simplyblock_web/static/deploy_spdk.yaml
--rw-r--r--  2.0 unx      463 b- defN 24-Apr-25 09:24 sbcli_jm-4.0.9/simplyblock_web/static/rpac.yaml
--rw-r--r--  2.0 unx      417 b- defN 24-Apr-25 09:24 sbcli_jm-4.0.9/simplyblock_web/static/list_deps.py
--rw-r--r--  2.0 unx     2876 b- defN 24-Apr-25 09:24 sbcli_jm-4.0.9/simplyblock_web/templates/deploy_spdk.yaml.j2
--rw-r--r--  2.0 unx     5547 b- defN 24-Apr-25 09:24 sbcli_jm-4.0.9/simplyblock_web/blueprints/node_api_caching_docker.py
--rw-r--r--  2.0 unx     4795 b- defN 24-Apr-25 09:24 sbcli_jm-4.0.9/simplyblock_web/blueprints/node_api_caching_ks.py
--rw-r--r--  2.0 unx     5317 b- defN 24-Apr-25 09:24 sbcli_jm-4.0.9/simplyblock_web/blueprints/web_api_caching_node.py
--rw-r--r--  2.0 unx    10052 b- defN 24-Apr-25 09:24 sbcli_jm-4.0.9/simplyblock_web/blueprints/snode_ops.py
--rw-r--r--  2.0 unx     8547 b- defN 24-Apr-25 09:24 sbcli_jm-4.0.9/simplyblock_web/blueprints/web_api_lvol.py
--rw-r--r--  2.0 unx    11244 b- defN 24-Apr-25 09:24 sbcli_jm-4.0.9/simplyblock_web/blueprints/csi.py
--rw-r--r--  2.0 unx    12198 b- defN 24-Apr-25 09:24 sbcli_jm-4.0.9/simplyblock_web/blueprints/caching_node_ops.py
--rw-r--r--  2.0 unx      975 b- defN 24-Apr-25 09:24 sbcli_jm-4.0.9/simplyblock_web/blueprints/web_api_mgmt_node.py
--rw-r--r--  2.0 unx     6326 b- defN 24-Apr-25 09:24 sbcli_jm-4.0.9/simplyblock_web/blueprints/web_api_storage_node.py
--rw-r--r--  2.0 unx        0 b- defN 24-Apr-25 09:24 sbcli_jm-4.0.9/simplyblock_web/blueprints/__init__.py
--rw-r--r--  2.0 unx     7846 b- defN 24-Apr-25 09:24 sbcli_jm-4.0.9/simplyblock_web/blueprints/caching_node_ops_k8s.py
--rw-r--r--  2.0 unx     2940 b- defN 24-Apr-25 09:24 sbcli_jm-4.0.9/simplyblock_web/blueprints/web_api_device.py
--rw-r--r--  2.0 unx     5274 b- defN 24-Apr-25 09:24 sbcli_jm-4.0.9/simplyblock_web/blueprints/web_api_cluster.py
--rw-r--r--  2.0 unx     3103 b- defN 24-Apr-25 09:24 sbcli_jm-4.0.9/simplyblock_web/blueprints/node_api_basic.py
--rw-r--r--  2.0 unx     6206 b- defN 24-Apr-25 09:24 sbcli_jm-4.0.9/simplyblock_web/blueprints/web_api_pool.py
-144 files, 993795 bytes uncompressed, 154317 bytes compressed:  84.5%
+Zip file size: 180073 bytes, number of entries: 144
+drwxr-xr-x  2.0 unx        0 b- stor 24-Apr-29 09:15 sbcli_jm-4.1.0/
+drwxr-xr-x  2.0 unx        0 b- stor 24-Apr-29 09:15 sbcli_jm-4.1.0/simplyblock_cli/
+drwxr-xr-x  2.0 unx        0 b- stor 24-Apr-29 09:15 sbcli_jm-4.1.0/sbcli_jm.egg-info/
+drwxr-xr-x  2.0 unx        0 b- stor 24-Apr-29 09:15 sbcli_jm-4.1.0/simplyblock_core/
+drwxr-xr-x  2.0 unx        0 b- stor 24-Apr-29 09:15 sbcli_jm-4.1.0/simplyblock_web/
+-rw-r--r--  2.0 unx     2251 b- defN 24-Apr-29 09:15 sbcli_jm-4.1.0/setup.py
+-rw-r--r--  2.0 unx      740 b- defN 24-Apr-29 09:15 sbcli_jm-4.1.0/README.md
+-rw-r--r--  2.0 unx      150 b- defN 24-Apr-29 09:15 sbcli_jm-4.1.0/env_var
+-rw-r--r--  2.0 unx       84 b- defN 24-Apr-29 09:15 sbcli_jm-4.1.0/pyproject.toml
+-rw-r--r--  2.0 unx       38 b- defN 24-Apr-29 09:15 sbcli_jm-4.1.0/setup.cfg
+-rw-r--r--  2.0 unx     1138 b- defN 24-Apr-29 09:15 sbcli_jm-4.1.0/PKG-INFO
+-rw-r--r--  2.0 unx    76859 b- defN 24-Apr-29 09:15 sbcli_jm-4.1.0/simplyblock_cli/cli.py
+-rw-r--r--  2.0 unx      357 b- defN 24-Apr-29 09:15 sbcli_jm-4.1.0/simplyblock_cli/main.py
+-rw-r--r--  2.0 unx        1 b- defN 24-Apr-29 09:15 sbcli_jm-4.1.0/sbcli_jm.egg-info/dependency_links.txt
+-rw-r--r--  2.0 unx     5067 b- defN 24-Apr-29 09:15 sbcli_jm-4.1.0/sbcli_jm.egg-info/SOURCES.txt
+-rw-r--r--  2.0 unx       49 b- defN 24-Apr-29 09:15 sbcli_jm-4.1.0/sbcli_jm.egg-info/top_level.txt
+-rw-r--r--  2.0 unx     1138 b- defN 24-Apr-29 09:15 sbcli_jm-4.1.0/sbcli_jm.egg-info/PKG-INFO
+-rw-r--r--  2.0 unx       66 b- defN 24-Apr-29 09:15 sbcli_jm-4.1.0/sbcli_jm.egg-info/requires.txt
+-rw-r--r--  2.0 unx       54 b- defN 24-Apr-29 09:15 sbcli_jm-4.1.0/sbcli_jm.egg-info/entry_points.txt
+drwxr-xr-x  2.0 unx        0 b- stor 24-Apr-29 09:15 sbcli_jm-4.1.0/simplyblock_core/services/
+drwxr-xr-x  2.0 unx        0 b- stor 24-Apr-29 09:15 sbcli_jm-4.1.0/simplyblock_core/scripts/
+drwxr-xr-x  2.0 unx        0 b- stor 24-Apr-29 09:15 sbcli_jm-4.1.0/simplyblock_core/controllers/
+drwxr-xr-x  2.0 unx        0 b- stor 24-Apr-29 09:15 sbcli_jm-4.1.0/simplyblock_core/models/
+-rw-r--r--  2.0 unx    66762 b- defN 24-Apr-29 09:15 sbcli_jm-4.1.0/simplyblock_core/storage_node_ops.py
+-rw-r--r--  2.0 unx     1443 b- defN 24-Apr-29 09:15 sbcli_jm-4.1.0/simplyblock_core/constants.py
+-rw-r--r--  2.0 unx     3153 b- defN 24-Apr-29 09:15 sbcli_jm-4.1.0/simplyblock_core/mgmt_node_ops.py
+-rw-r--r--  2.0 unx     3444 b- defN 24-Apr-29 09:15 sbcli_jm-4.1.0/simplyblock_core/cnode_client.py
+-rw-r--r--  2.0 unx      279 b- defN 24-Apr-29 09:15 sbcli_jm-4.1.0/simplyblock_core/shell_utils.py
+-rw-r--r--  2.0 unx      938 b- defN 24-Apr-29 09:15 sbcli_jm-4.1.0/simplyblock_core/pci_utils.py
+-rw-r--r--  2.0 unx        0 b- defN 24-Apr-29 09:15 sbcli_jm-4.1.0/simplyblock_core/__init__.py
+-rw-r--r--  2.0 unx     3416 b- defN 24-Apr-29 09:15 sbcli_jm-4.1.0/simplyblock_core/snode_client.py
+-rw-r--r--  2.0 unx     8189 b- defN 24-Apr-29 09:15 sbcli_jm-4.1.0/simplyblock_core/kv_store.py
+-rw-r--r--  2.0 unx     7640 b- defN 24-Apr-29 09:15 sbcli_jm-4.1.0/simplyblock_core/utils.py
+-rw-r--r--  2.0 unx    23335 b- defN 24-Apr-29 09:15 sbcli_jm-4.1.0/simplyblock_core/cluster_ops.py
+-rw-r--r--  2.0 unx     5112 b- defN 24-Apr-29 09:15 sbcli_jm-4.1.0/simplyblock_core/compute_node_ops.py
+-rw-r--r--  2.0 unx    21979 b- defN 24-Apr-29 09:15 sbcli_jm-4.1.0/simplyblock_core/rpc_client.py
+-rw-r--r--  2.0 unx     7401 b- defN 24-Apr-29 09:15 sbcli_jm-4.1.0/simplyblock_core/distr_controller.py
+-rw-r--r--  2.0 unx     2189 b- defN 24-Apr-29 09:15 sbcli_jm-4.1.0/simplyblock_core/services/lvol_monitor.py
+-rw-r--r--  2.0 unx     3203 b- defN 24-Apr-29 09:15 sbcli_jm-4.1.0/simplyblock_core/services/caching_node_monitor.py
+-rw-r--r--  2.0 unx     5443 b- defN 24-Apr-29 09:15 sbcli_jm-4.1.0/simplyblock_core/services/capacity_collector.py
+-rw-r--r--  2.0 unx     5462 b- defN 24-Apr-29 09:15 sbcli_jm-4.1.0/simplyblock_core/services/health_check_service.py
+-rw-r--r--  2.0 unx      229 b- defN 24-Apr-29 09:15 sbcli_jm-4.1.0/simplyblock_core/services/service_template.service
+-rw-r--r--  2.0 unx     5262 b- defN 24-Apr-29 09:15 sbcli_jm-4.1.0/simplyblock_core/services/lvol_stat_collector.py
+-rw-r--r--  2.0 unx      173 b- defN 24-Apr-29 09:15 sbcli_jm-4.1.0/simplyblock_core/services/remove_service.sh
+-rw-r--r--  2.0 unx     2410 b- defN 24-Apr-29 09:15 sbcli_jm-4.1.0/simplyblock_core/services/log_agg_service.py
+-rw-r--r--  2.0 unx     5123 b- defN 24-Apr-29 09:15 sbcli_jm-4.1.0/simplyblock_core/services/distr_event_collector.py
+-rw-r--r--  2.0 unx     7438 b- defN 24-Apr-29 09:15 sbcli_jm-4.1.0/simplyblock_core/services/capacity_and_stats_collector.py
+-rw-r--r--  2.0 unx     2423 b- defN 24-Apr-29 09:15 sbcli_jm-4.1.0/simplyblock_core/services/port_stat_collector.py
+-rw-r--r--  2.0 unx     2490 b- defN 24-Apr-29 09:15 sbcli_jm-4.1.0/simplyblock_core/services/device_monitor.py
+-rw-r--r--  2.0 unx     4118 b- defN 24-Apr-29 09:15 sbcli_jm-4.1.0/simplyblock_core/services/__init__.py
+-rw-r--r--  2.0 unx      837 b- defN 24-Apr-29 09:15 sbcli_jm-4.1.0/simplyblock_core/services/install_service.sh
+-rw-r--r--  2.0 unx     3003 b- defN 24-Apr-29 09:15 sbcli_jm-4.1.0/simplyblock_core/services/mgmt_node_monitor.py
+-rw-r--r--  2.0 unx     2671 b- defN 24-Apr-29 09:15 sbcli_jm-4.1.0/simplyblock_core/services/cap_monitor.py
+-rw-r--r--  2.0 unx     6577 b- defN 24-Apr-29 09:15 sbcli_jm-4.1.0/simplyblock_core/services/storage_node_monitor.py
+drwxr-xr-x  2.0 unx        0 b- stor 24-Apr-29 09:15 sbcli_jm-4.1.0/simplyblock_core/scripts/alerting/
+drwxr-xr-x  2.0 unx        0 b- stor 24-Apr-29 09:15 sbcli_jm-4.1.0/simplyblock_core/scripts/dashboards/
+-rw-r--r--  2.0 unx      694 b- defN 24-Apr-29 09:15 sbcli_jm-4.1.0/simplyblock_core/scripts/deploy_stack.sh
+-rw-r--r--  2.0 unx      152 b- defN 24-Apr-29 09:15 sbcli_jm-4.1.0/simplyblock_core/scripts/set_db_config.sh
+-rw-r--r--  2.0 unx     1163 b- defN 24-Apr-29 09:15 sbcli_jm-4.1.0/simplyblock_core/scripts/haproxy.cfg
+-rw-r--r--  2.0 unx     8081 b- defN 24-Apr-29 09:15 sbcli_jm-4.1.0/simplyblock_core/scripts/docker-compose-swarm.yml
+-rw-r--r--  2.0 unx       54 b- defN 24-Apr-29 09:15 sbcli_jm-4.1.0/simplyblock_core/scripts/db_config_single.sh
+-rw-r--r--  2.0 unx     5305 b- defN 24-Apr-29 09:15 sbcli_jm-4.1.0/simplyblock_core/scripts/stack_deploy_wait.sh
+-rw-r--r--  2.0 unx      453 b- defN 24-Apr-29 09:15 sbcli_jm-4.1.0/simplyblock_core/scripts/config_docker.sh
+-rw-r--r--  2.0 unx     1694 b- defN 24-Apr-29 09:15 sbcli_jm-4.1.0/simplyblock_core/scripts/__init__.py
+-rw-r--r--  2.0 unx      311 b- defN 24-Apr-29 09:15 sbcli_jm-4.1.0/simplyblock_core/scripts/clean_local_storage_deploy.sh
+-rw-r--r--  2.0 unx      118 b- defN 24-Apr-29 09:15 sbcli_jm-4.1.0/simplyblock_core/scripts/db_config_double.sh
+-rw-r--r--  2.0 unx      360 b- defN 24-Apr-29 09:15 sbcli_jm-4.1.0/simplyblock_core/scripts/datasource.yml
+-rw-r--r--  2.0 unx       43 b- defN 24-Apr-29 09:15 sbcli_jm-4.1.0/simplyblock_core/scripts/run_ssh.sh
+-rw-r--r--  2.0 unx     1438 b- defN 24-Apr-29 09:15 sbcli_jm-4.1.0/simplyblock_core/scripts/install_deps.sh
+-rw-r--r--  2.0 unx      187 b- defN 24-Apr-29 09:15 sbcli_jm-4.1.0/simplyblock_core/scripts/prometheus.yml
+-rwxr-xr-x  2.0 unx      595 b- defN 24-Apr-29 09:15 sbcli_jm-4.1.0/simplyblock_core/scripts/apply_dashboard.sh
+-rw-r--r--  2.0 unx     5860 b- defN 24-Apr-29 09:15 sbcli_jm-4.1.0/simplyblock_core/scripts/alerting/alert_rules.yaml
+-rw-r--r--  2.0 unx     1853 b- defN 24-Apr-29 09:15 sbcli_jm-4.1.0/simplyblock_core/scripts/alerting/alert_resources.yaml
+-rw-r--r--  2.0 unx    98143 b- defN 24-Apr-29 09:15 sbcli_jm-4.1.0/simplyblock_core/scripts/dashboards/devices.json
+-rw-r--r--  2.0 unx    98086 b- defN 24-Apr-29 09:15 sbcli_jm-4.1.0/simplyblock_core/scripts/dashboards/nodes.json
+-rw-r--r--  2.0 unx    98031 b- defN 24-Apr-29 09:15 sbcli_jm-4.1.0/simplyblock_core/scripts/dashboards/lvols.json
+-rw-r--r--  2.0 unx    98198 b- defN 24-Apr-29 09:15 sbcli_jm-4.1.0/simplyblock_core/scripts/dashboards/cluster.json
+-rw-r--r--  2.0 unx    12785 b- defN 24-Apr-29 09:15 sbcli_jm-4.1.0/simplyblock_core/controllers/device_controller.py
+-rw-r--r--  2.0 unx     1120 b- defN 24-Apr-29 09:15 sbcli_jm-4.1.0/simplyblock_core/controllers/mgmt_events.py
+-rw-r--r--  2.0 unx     1961 b- defN 24-Apr-29 09:15 sbcli_jm-4.1.0/simplyblock_core/controllers/events_controller.py
+-rw-r--r--  2.0 unx     1521 b- defN 24-Apr-29 09:15 sbcli_jm-4.1.0/simplyblock_core/controllers/storage_events.py
+-rw-r--r--  2.0 unx     1630 b- defN 24-Apr-29 09:15 sbcli_jm-4.1.0/simplyblock_core/controllers/lvol_events.py
+-rw-r--r--  2.0 unx    10557 b- defN 24-Apr-29 09:15 sbcli_jm-4.1.0/simplyblock_core/controllers/snapshot_controller.py
+-rw-r--r--  2.0 unx     1568 b- defN 24-Apr-29 09:15 sbcli_jm-4.1.0/simplyblock_core/controllers/device_events.py
+-rw-r--r--  2.0 unx    10375 b- defN 24-Apr-29 09:15 sbcli_jm-4.1.0/simplyblock_core/controllers/pool_controller.py
+-rw-r--r--  2.0 unx        0 b- defN 24-Apr-29 09:15 sbcli_jm-4.1.0/simplyblock_core/controllers/__init__.py
+-rw-r--r--  2.0 unx     1900 b- defN 24-Apr-29 09:15 sbcli_jm-4.1.0/simplyblock_core/controllers/cluster_events.py
+-rw-r--r--  2.0 unx    22802 b- defN 24-Apr-29 09:15 sbcli_jm-4.1.0/simplyblock_core/controllers/caching_node_controller.py
+-rw-r--r--  2.0 unx     1122 b- defN 24-Apr-29 09:15 sbcli_jm-4.1.0/simplyblock_core/controllers/snapshot_events.py
+-rw-r--r--  2.0 unx    47342 b- defN 24-Apr-29 09:15 sbcli_jm-4.1.0/simplyblock_core/controllers/lvol_controller.py
+-rw-r--r--  2.0 unx    11294 b- defN 24-Apr-29 09:15 sbcli_jm-4.1.0/simplyblock_core/controllers/health_controller.py
+-rw-r--r--  2.0 unx      695 b- defN 24-Apr-29 09:15 sbcli_jm-4.1.0/simplyblock_core/controllers/pool_events.py
+-rw-r--r--  2.0 unx     1500 b- defN 24-Apr-29 09:15 sbcli_jm-4.1.0/simplyblock_core/models/events.py
+-rw-r--r--  2.0 unx      806 b- defN 24-Apr-29 09:15 sbcli_jm-4.1.0/simplyblock_core/models/iface.py
+-rw-r--r--  2.0 unx     4846 b- defN 24-Apr-29 09:15 sbcli_jm-4.1.0/simplyblock_core/models/base_model.py
+-rw-r--r--  2.0 unx     2579 b- defN 24-Apr-29 09:15 sbcli_jm-4.1.0/simplyblock_core/models/lvol_model.py
+-rw-r--r--  2.0 unx      917 b- defN 24-Apr-29 09:15 sbcli_jm-4.1.0/simplyblock_core/models/compute_node.py
+-rw-r--r--  2.0 unx      736 b- defN 24-Apr-29 09:15 sbcli_jm-4.1.0/simplyblock_core/models/snapshot.py
+-rw-r--r--  2.0 unx     1602 b- defN 24-Apr-29 09:15 sbcli_jm-4.1.0/simplyblock_core/models/pool.py
+-rw-r--r--  2.0 unx     1228 b- defN 24-Apr-29 09:15 sbcli_jm-4.1.0/simplyblock_core/models/global_settings.py
+-rw-r--r--  2.0 unx     1020 b- defN 24-Apr-29 09:15 sbcli_jm-4.1.0/simplyblock_core/models/port_stat.py
+-rw-r--r--  2.0 unx     3531 b- defN 24-Apr-29 09:15 sbcli_jm-4.1.0/simplyblock_core/models/storage_node.py
+-rw-r--r--  2.0 unx        0 b- defN 24-Apr-29 09:15 sbcli_jm-4.1.0/simplyblock_core/models/__init__.py
+-rw-r--r--  2.0 unx     4242 b- defN 24-Apr-29 09:15 sbcli_jm-4.1.0/simplyblock_core/models/stats.py
+-rw-r--r--  2.0 unx     2565 b- defN 24-Apr-29 09:15 sbcli_jm-4.1.0/simplyblock_core/models/cluster.py
+-rw-r--r--  2.0 unx     1466 b- defN 24-Apr-29 09:15 sbcli_jm-4.1.0/simplyblock_core/models/mgmt_node.py
+-rw-r--r--  2.0 unx     3766 b- defN 24-Apr-29 09:15 sbcli_jm-4.1.0/simplyblock_core/models/caching_node.py
+-rw-r--r--  2.0 unx     2979 b- defN 24-Apr-29 09:15 sbcli_jm-4.1.0/simplyblock_core/models/nvme_device.py
+drwxr-xr-x  2.0 unx        0 b- stor 24-Apr-29 09:15 sbcli_jm-4.1.0/simplyblock_web/static/
+drwxr-xr-x  2.0 unx        0 b- stor 24-Apr-29 09:15 sbcli_jm-4.1.0/simplyblock_web/templates/
+drwxr-xr-x  2.0 unx        0 b- stor 24-Apr-29 09:15 sbcli_jm-4.1.0/simplyblock_web/blueprints/
+-rw-r--r--  2.0 unx      725 b- defN 24-Apr-29 09:15 sbcli_jm-4.1.0/simplyblock_web/caching_node_app_k8s.py
+-rw-r--r--  2.0 unx     5098 b- defN 24-Apr-29 09:15 sbcli_jm-4.1.0/simplyblock_web/node_utils.py
+-rw-r--r--  2.0 unx      703 b- defN 24-Apr-29 09:15 sbcli_jm-4.1.0/simplyblock_web/snode_app.py
+-rw-r--r--  2.0 unx     1263 b- defN 24-Apr-29 09:15 sbcli_jm-4.1.0/simplyblock_web/app.py
+-rw-r--r--  2.0 unx     1638 b- defN 24-Apr-29 09:15 sbcli_jm-4.1.0/simplyblock_web/auth_middleware.py
+-rw-r--r--  2.0 unx        0 b- defN 24-Apr-29 09:15 sbcli_jm-4.1.0/simplyblock_web/__init__.py
+-rw-r--r--  2.0 unx      717 b- defN 24-Apr-29 09:15 sbcli_jm-4.1.0/simplyblock_web/caching_node_app.py
+-rw-r--r--  2.0 unx     2513 b- defN 24-Apr-29 09:15 sbcli_jm-4.1.0/simplyblock_web/utils.py
+-rw-r--r--  2.0 unx     1434 b- defN 24-Apr-29 09:15 sbcli_jm-4.1.0/simplyblock_web/node_webapp.py
+-rw-r--r--  2.0 unx      507 b- defN 24-Apr-29 09:15 sbcli_jm-4.1.0/simplyblock_web/static/deploy_cnode.yaml
+-rw-r--r--  2.0 unx      322 b- defN 24-Apr-29 09:15 sbcli_jm-4.1.0/simplyblock_web/static/tst.py
+-rw-r--r--  2.0 unx      434 b- defN 24-Apr-29 09:15 sbcli_jm-4.1.0/simplyblock_web/static/is_up.py
+-rw-r--r--  2.0 unx      827 b- defN 24-Apr-29 09:15 sbcli_jm-4.1.0/simplyblock_web/static/delete.py
+-rw-r--r--  2.0 unx     1302 b- defN 24-Apr-29 09:15 sbcli_jm-4.1.0/simplyblock_web/static/deploy.py
+-rw-r--r--  2.0 unx     1466 b- defN 24-Apr-29 09:15 sbcli_jm-4.1.0/simplyblock_web/static/deploy_spdk.yaml
+-rw-r--r--  2.0 unx      463 b- defN 24-Apr-29 09:15 sbcli_jm-4.1.0/simplyblock_web/static/rpac.yaml
+-rw-r--r--  2.0 unx      417 b- defN 24-Apr-29 09:15 sbcli_jm-4.1.0/simplyblock_web/static/list_deps.py
+-rw-r--r--  2.0 unx     2876 b- defN 24-Apr-29 09:15 sbcli_jm-4.1.0/simplyblock_web/templates/deploy_spdk.yaml.j2
+-rw-r--r--  2.0 unx     5547 b- defN 24-Apr-29 09:15 sbcli_jm-4.1.0/simplyblock_web/blueprints/node_api_caching_docker.py
+-rw-r--r--  2.0 unx     4795 b- defN 24-Apr-29 09:15 sbcli_jm-4.1.0/simplyblock_web/blueprints/node_api_caching_ks.py
+-rw-r--r--  2.0 unx     5317 b- defN 24-Apr-29 09:15 sbcli_jm-4.1.0/simplyblock_web/blueprints/web_api_caching_node.py
+-rw-r--r--  2.0 unx    10049 b- defN 24-Apr-29 09:15 sbcli_jm-4.1.0/simplyblock_web/blueprints/snode_ops.py
+-rw-r--r--  2.0 unx     8547 b- defN 24-Apr-29 09:15 sbcli_jm-4.1.0/simplyblock_web/blueprints/web_api_lvol.py
+-rw-r--r--  2.0 unx    11244 b- defN 24-Apr-29 09:15 sbcli_jm-4.1.0/simplyblock_web/blueprints/csi.py
+-rw-r--r--  2.0 unx    12198 b- defN 24-Apr-29 09:15 sbcli_jm-4.1.0/simplyblock_web/blueprints/caching_node_ops.py
+-rw-r--r--  2.0 unx      975 b- defN 24-Apr-29 09:15 sbcli_jm-4.1.0/simplyblock_web/blueprints/web_api_mgmt_node.py
+-rw-r--r--  2.0 unx     6326 b- defN 24-Apr-29 09:15 sbcli_jm-4.1.0/simplyblock_web/blueprints/web_api_storage_node.py
+-rw-r--r--  2.0 unx        0 b- defN 24-Apr-29 09:15 sbcli_jm-4.1.0/simplyblock_web/blueprints/__init__.py
+-rw-r--r--  2.0 unx     7846 b- defN 24-Apr-29 09:15 sbcli_jm-4.1.0/simplyblock_web/blueprints/caching_node_ops_k8s.py
+-rw-r--r--  2.0 unx     2940 b- defN 24-Apr-29 09:15 sbcli_jm-4.1.0/simplyblock_web/blueprints/web_api_device.py
+-rw-r--r--  2.0 unx     5274 b- defN 24-Apr-29 09:15 sbcli_jm-4.1.0/simplyblock_web/blueprints/web_api_cluster.py
+-rw-r--r--  2.0 unx     3103 b- defN 24-Apr-29 09:15 sbcli_jm-4.1.0/simplyblock_web/blueprints/node_api_basic.py
+-rw-r--r--  2.0 unx     6206 b- defN 24-Apr-29 09:15 sbcli_jm-4.1.0/simplyblock_web/blueprints/web_api_pool.py
+144 files, 994480 bytes uncompressed, 154239 bytes compressed:  84.5%
```

## zipnote {}

```diff
@@ -1,433 +1,433 @@
-Filename: sbcli_jm-4.0.9/
+Filename: sbcli_jm-4.1.0/
 Comment: 
 
-Filename: sbcli_jm-4.0.9/simplyblock_cli/
+Filename: sbcli_jm-4.1.0/simplyblock_cli/
 Comment: 
 
-Filename: sbcli_jm-4.0.9/sbcli_jm.egg-info/
+Filename: sbcli_jm-4.1.0/sbcli_jm.egg-info/
 Comment: 
 
-Filename: sbcli_jm-4.0.9/simplyblock_core/
+Filename: sbcli_jm-4.1.0/simplyblock_core/
 Comment: 
 
-Filename: sbcli_jm-4.0.9/simplyblock_web/
+Filename: sbcli_jm-4.1.0/simplyblock_web/
 Comment: 
 
-Filename: sbcli_jm-4.0.9/setup.py
+Filename: sbcli_jm-4.1.0/setup.py
 Comment: 
 
-Filename: sbcli_jm-4.0.9/README.md
+Filename: sbcli_jm-4.1.0/README.md
 Comment: 
 
-Filename: sbcli_jm-4.0.9/env_var
+Filename: sbcli_jm-4.1.0/env_var
 Comment: 
 
-Filename: sbcli_jm-4.0.9/pyproject.toml
+Filename: sbcli_jm-4.1.0/pyproject.toml
 Comment: 
 
-Filename: sbcli_jm-4.0.9/setup.cfg
+Filename: sbcli_jm-4.1.0/setup.cfg
 Comment: 
 
-Filename: sbcli_jm-4.0.9/PKG-INFO
+Filename: sbcli_jm-4.1.0/PKG-INFO
 Comment: 
 
-Filename: sbcli_jm-4.0.9/simplyblock_cli/cli.py
+Filename: sbcli_jm-4.1.0/simplyblock_cli/cli.py
 Comment: 
 
-Filename: sbcli_jm-4.0.9/simplyblock_cli/main.py
+Filename: sbcli_jm-4.1.0/simplyblock_cli/main.py
 Comment: 
 
-Filename: sbcli_jm-4.0.9/sbcli_jm.egg-info/dependency_links.txt
+Filename: sbcli_jm-4.1.0/sbcli_jm.egg-info/dependency_links.txt
 Comment: 
 
-Filename: sbcli_jm-4.0.9/sbcli_jm.egg-info/SOURCES.txt
+Filename: sbcli_jm-4.1.0/sbcli_jm.egg-info/SOURCES.txt
 Comment: 
 
-Filename: sbcli_jm-4.0.9/sbcli_jm.egg-info/top_level.txt
+Filename: sbcli_jm-4.1.0/sbcli_jm.egg-info/top_level.txt
 Comment: 
 
-Filename: sbcli_jm-4.0.9/sbcli_jm.egg-info/PKG-INFO
+Filename: sbcli_jm-4.1.0/sbcli_jm.egg-info/PKG-INFO
 Comment: 
 
-Filename: sbcli_jm-4.0.9/sbcli_jm.egg-info/requires.txt
+Filename: sbcli_jm-4.1.0/sbcli_jm.egg-info/requires.txt
 Comment: 
 
-Filename: sbcli_jm-4.0.9/sbcli_jm.egg-info/entry_points.txt
+Filename: sbcli_jm-4.1.0/sbcli_jm.egg-info/entry_points.txt
 Comment: 
 
-Filename: sbcli_jm-4.0.9/simplyblock_core/services/
+Filename: sbcli_jm-4.1.0/simplyblock_core/services/
 Comment: 
 
-Filename: sbcli_jm-4.0.9/simplyblock_core/scripts/
+Filename: sbcli_jm-4.1.0/simplyblock_core/scripts/
 Comment: 
 
-Filename: sbcli_jm-4.0.9/simplyblock_core/controllers/
+Filename: sbcli_jm-4.1.0/simplyblock_core/controllers/
 Comment: 
 
-Filename: sbcli_jm-4.0.9/simplyblock_core/models/
+Filename: sbcli_jm-4.1.0/simplyblock_core/models/
 Comment: 
 
-Filename: sbcli_jm-4.0.9/simplyblock_core/storage_node_ops.py
+Filename: sbcli_jm-4.1.0/simplyblock_core/storage_node_ops.py
 Comment: 
 
-Filename: sbcli_jm-4.0.9/simplyblock_core/constants.py
+Filename: sbcli_jm-4.1.0/simplyblock_core/constants.py
 Comment: 
 
-Filename: sbcli_jm-4.0.9/simplyblock_core/mgmt_node_ops.py
+Filename: sbcli_jm-4.1.0/simplyblock_core/mgmt_node_ops.py
 Comment: 
 
-Filename: sbcli_jm-4.0.9/simplyblock_core/cnode_client.py
+Filename: sbcli_jm-4.1.0/simplyblock_core/cnode_client.py
 Comment: 
 
-Filename: sbcli_jm-4.0.9/simplyblock_core/shell_utils.py
+Filename: sbcli_jm-4.1.0/simplyblock_core/shell_utils.py
 Comment: 
 
-Filename: sbcli_jm-4.0.9/simplyblock_core/pci_utils.py
+Filename: sbcli_jm-4.1.0/simplyblock_core/pci_utils.py
 Comment: 
 
-Filename: sbcli_jm-4.0.9/simplyblock_core/__init__.py
+Filename: sbcli_jm-4.1.0/simplyblock_core/__init__.py
 Comment: 
 
-Filename: sbcli_jm-4.0.9/simplyblock_core/snode_client.py
+Filename: sbcli_jm-4.1.0/simplyblock_core/snode_client.py
 Comment: 
 
-Filename: sbcli_jm-4.0.9/simplyblock_core/kv_store.py
+Filename: sbcli_jm-4.1.0/simplyblock_core/kv_store.py
 Comment: 
 
-Filename: sbcli_jm-4.0.9/simplyblock_core/utils.py
+Filename: sbcli_jm-4.1.0/simplyblock_core/utils.py
 Comment: 
 
-Filename: sbcli_jm-4.0.9/simplyblock_core/cluster_ops.py
+Filename: sbcli_jm-4.1.0/simplyblock_core/cluster_ops.py
 Comment: 
 
-Filename: sbcli_jm-4.0.9/simplyblock_core/compute_node_ops.py
+Filename: sbcli_jm-4.1.0/simplyblock_core/compute_node_ops.py
 Comment: 
 
-Filename: sbcli_jm-4.0.9/simplyblock_core/rpc_client.py
+Filename: sbcli_jm-4.1.0/simplyblock_core/rpc_client.py
 Comment: 
 
-Filename: sbcli_jm-4.0.9/simplyblock_core/distr_controller.py
+Filename: sbcli_jm-4.1.0/simplyblock_core/distr_controller.py
 Comment: 
 
-Filename: sbcli_jm-4.0.9/simplyblock_core/services/lvol_monitor.py
+Filename: sbcli_jm-4.1.0/simplyblock_core/services/lvol_monitor.py
 Comment: 
 
-Filename: sbcli_jm-4.0.9/simplyblock_core/services/caching_node_monitor.py
+Filename: sbcli_jm-4.1.0/simplyblock_core/services/caching_node_monitor.py
 Comment: 
 
-Filename: sbcli_jm-4.0.9/simplyblock_core/services/capacity_collector.py
+Filename: sbcli_jm-4.1.0/simplyblock_core/services/capacity_collector.py
 Comment: 
 
-Filename: sbcli_jm-4.0.9/simplyblock_core/services/health_check_service.py
+Filename: sbcli_jm-4.1.0/simplyblock_core/services/health_check_service.py
 Comment: 
 
-Filename: sbcli_jm-4.0.9/simplyblock_core/services/service_template.service
+Filename: sbcli_jm-4.1.0/simplyblock_core/services/service_template.service
 Comment: 
 
-Filename: sbcli_jm-4.0.9/simplyblock_core/services/lvol_stat_collector.py
+Filename: sbcli_jm-4.1.0/simplyblock_core/services/lvol_stat_collector.py
 Comment: 
 
-Filename: sbcli_jm-4.0.9/simplyblock_core/services/remove_service.sh
+Filename: sbcli_jm-4.1.0/simplyblock_core/services/remove_service.sh
 Comment: 
 
-Filename: sbcli_jm-4.0.9/simplyblock_core/services/log_agg_service.py
+Filename: sbcli_jm-4.1.0/simplyblock_core/services/log_agg_service.py
 Comment: 
 
-Filename: sbcli_jm-4.0.9/simplyblock_core/services/distr_event_collector.py
+Filename: sbcli_jm-4.1.0/simplyblock_core/services/distr_event_collector.py
 Comment: 
 
-Filename: sbcli_jm-4.0.9/simplyblock_core/services/capacity_and_stats_collector.py
+Filename: sbcli_jm-4.1.0/simplyblock_core/services/capacity_and_stats_collector.py
 Comment: 
 
-Filename: sbcli_jm-4.0.9/simplyblock_core/services/port_stat_collector.py
+Filename: sbcli_jm-4.1.0/simplyblock_core/services/port_stat_collector.py
 Comment: 
 
-Filename: sbcli_jm-4.0.9/simplyblock_core/services/device_monitor.py
+Filename: sbcli_jm-4.1.0/simplyblock_core/services/device_monitor.py
 Comment: 
 
-Filename: sbcli_jm-4.0.9/simplyblock_core/services/__init__.py
+Filename: sbcli_jm-4.1.0/simplyblock_core/services/__init__.py
 Comment: 
 
-Filename: sbcli_jm-4.0.9/simplyblock_core/services/install_service.sh
+Filename: sbcli_jm-4.1.0/simplyblock_core/services/install_service.sh
 Comment: 
 
-Filename: sbcli_jm-4.0.9/simplyblock_core/services/mgmt_node_monitor.py
+Filename: sbcli_jm-4.1.0/simplyblock_core/services/mgmt_node_monitor.py
 Comment: 
 
-Filename: sbcli_jm-4.0.9/simplyblock_core/services/cap_monitor.py
+Filename: sbcli_jm-4.1.0/simplyblock_core/services/cap_monitor.py
 Comment: 
 
-Filename: sbcli_jm-4.0.9/simplyblock_core/services/storage_node_monitor.py
+Filename: sbcli_jm-4.1.0/simplyblock_core/services/storage_node_monitor.py
 Comment: 
 
-Filename: sbcli_jm-4.0.9/simplyblock_core/scripts/alerting/
+Filename: sbcli_jm-4.1.0/simplyblock_core/scripts/alerting/
 Comment: 
 
-Filename: sbcli_jm-4.0.9/simplyblock_core/scripts/dashboards/
+Filename: sbcli_jm-4.1.0/simplyblock_core/scripts/dashboards/
 Comment: 
 
-Filename: sbcli_jm-4.0.9/simplyblock_core/scripts/deploy_stack.sh
+Filename: sbcli_jm-4.1.0/simplyblock_core/scripts/deploy_stack.sh
 Comment: 
 
-Filename: sbcli_jm-4.0.9/simplyblock_core/scripts/set_db_config.sh
+Filename: sbcli_jm-4.1.0/simplyblock_core/scripts/set_db_config.sh
 Comment: 
 
-Filename: sbcli_jm-4.0.9/simplyblock_core/scripts/haproxy.cfg
+Filename: sbcli_jm-4.1.0/simplyblock_core/scripts/haproxy.cfg
 Comment: 
 
-Filename: sbcli_jm-4.0.9/simplyblock_core/scripts/docker-compose-swarm.yml
+Filename: sbcli_jm-4.1.0/simplyblock_core/scripts/docker-compose-swarm.yml
 Comment: 
 
-Filename: sbcli_jm-4.0.9/simplyblock_core/scripts/db_config_single.sh
+Filename: sbcli_jm-4.1.0/simplyblock_core/scripts/db_config_single.sh
 Comment: 
 
-Filename: sbcli_jm-4.0.9/simplyblock_core/scripts/stack_deploy_wait.sh
+Filename: sbcli_jm-4.1.0/simplyblock_core/scripts/stack_deploy_wait.sh
 Comment: 
 
-Filename: sbcli_jm-4.0.9/simplyblock_core/scripts/config_docker.sh
+Filename: sbcli_jm-4.1.0/simplyblock_core/scripts/config_docker.sh
 Comment: 
 
-Filename: sbcli_jm-4.0.9/simplyblock_core/scripts/__init__.py
+Filename: sbcli_jm-4.1.0/simplyblock_core/scripts/__init__.py
 Comment: 
 
-Filename: sbcli_jm-4.0.9/simplyblock_core/scripts/clean_local_storage_deploy.sh
+Filename: sbcli_jm-4.1.0/simplyblock_core/scripts/clean_local_storage_deploy.sh
 Comment: 
 
-Filename: sbcli_jm-4.0.9/simplyblock_core/scripts/db_config_double.sh
+Filename: sbcli_jm-4.1.0/simplyblock_core/scripts/db_config_double.sh
 Comment: 
 
-Filename: sbcli_jm-4.0.9/simplyblock_core/scripts/datasource.yml
+Filename: sbcli_jm-4.1.0/simplyblock_core/scripts/datasource.yml
 Comment: 
 
-Filename: sbcli_jm-4.0.9/simplyblock_core/scripts/run_ssh.sh
+Filename: sbcli_jm-4.1.0/simplyblock_core/scripts/run_ssh.sh
 Comment: 
 
-Filename: sbcli_jm-4.0.9/simplyblock_core/scripts/install_deps.sh
+Filename: sbcli_jm-4.1.0/simplyblock_core/scripts/install_deps.sh
 Comment: 
 
-Filename: sbcli_jm-4.0.9/simplyblock_core/scripts/prometheus.yml
+Filename: sbcli_jm-4.1.0/simplyblock_core/scripts/prometheus.yml
 Comment: 
 
-Filename: sbcli_jm-4.0.9/simplyblock_core/scripts/apply_dashboard.sh
+Filename: sbcli_jm-4.1.0/simplyblock_core/scripts/apply_dashboard.sh
 Comment: 
 
-Filename: sbcli_jm-4.0.9/simplyblock_core/scripts/alerting/alert_rules.yaml
+Filename: sbcli_jm-4.1.0/simplyblock_core/scripts/alerting/alert_rules.yaml
 Comment: 
 
-Filename: sbcli_jm-4.0.9/simplyblock_core/scripts/alerting/alert_resources.yaml
+Filename: sbcli_jm-4.1.0/simplyblock_core/scripts/alerting/alert_resources.yaml
 Comment: 
 
-Filename: sbcli_jm-4.0.9/simplyblock_core/scripts/dashboards/devices.json
+Filename: sbcli_jm-4.1.0/simplyblock_core/scripts/dashboards/devices.json
 Comment: 
 
-Filename: sbcli_jm-4.0.9/simplyblock_core/scripts/dashboards/nodes.json
+Filename: sbcli_jm-4.1.0/simplyblock_core/scripts/dashboards/nodes.json
 Comment: 
 
-Filename: sbcli_jm-4.0.9/simplyblock_core/scripts/dashboards/lvols.json
+Filename: sbcli_jm-4.1.0/simplyblock_core/scripts/dashboards/lvols.json
 Comment: 
 
-Filename: sbcli_jm-4.0.9/simplyblock_core/scripts/dashboards/cluster.json
+Filename: sbcli_jm-4.1.0/simplyblock_core/scripts/dashboards/cluster.json
 Comment: 
 
-Filename: sbcli_jm-4.0.9/simplyblock_core/controllers/device_controller.py
+Filename: sbcli_jm-4.1.0/simplyblock_core/controllers/device_controller.py
 Comment: 
 
-Filename: sbcli_jm-4.0.9/simplyblock_core/controllers/mgmt_events.py
+Filename: sbcli_jm-4.1.0/simplyblock_core/controllers/mgmt_events.py
 Comment: 
 
-Filename: sbcli_jm-4.0.9/simplyblock_core/controllers/events_controller.py
+Filename: sbcli_jm-4.1.0/simplyblock_core/controllers/events_controller.py
 Comment: 
 
-Filename: sbcli_jm-4.0.9/simplyblock_core/controllers/storage_events.py
+Filename: sbcli_jm-4.1.0/simplyblock_core/controllers/storage_events.py
 Comment: 
 
-Filename: sbcli_jm-4.0.9/simplyblock_core/controllers/lvol_events.py
+Filename: sbcli_jm-4.1.0/simplyblock_core/controllers/lvol_events.py
 Comment: 
 
-Filename: sbcli_jm-4.0.9/simplyblock_core/controllers/snapshot_controller.py
+Filename: sbcli_jm-4.1.0/simplyblock_core/controllers/snapshot_controller.py
 Comment: 
 
-Filename: sbcli_jm-4.0.9/simplyblock_core/controllers/device_events.py
+Filename: sbcli_jm-4.1.0/simplyblock_core/controllers/device_events.py
 Comment: 
 
-Filename: sbcli_jm-4.0.9/simplyblock_core/controllers/pool_controller.py
+Filename: sbcli_jm-4.1.0/simplyblock_core/controllers/pool_controller.py
 Comment: 
 
-Filename: sbcli_jm-4.0.9/simplyblock_core/controllers/__init__.py
+Filename: sbcli_jm-4.1.0/simplyblock_core/controllers/__init__.py
 Comment: 
 
-Filename: sbcli_jm-4.0.9/simplyblock_core/controllers/cluster_events.py
+Filename: sbcli_jm-4.1.0/simplyblock_core/controllers/cluster_events.py
 Comment: 
 
-Filename: sbcli_jm-4.0.9/simplyblock_core/controllers/caching_node_controller.py
+Filename: sbcli_jm-4.1.0/simplyblock_core/controllers/caching_node_controller.py
 Comment: 
 
-Filename: sbcli_jm-4.0.9/simplyblock_core/controllers/snapshot_events.py
+Filename: sbcli_jm-4.1.0/simplyblock_core/controllers/snapshot_events.py
 Comment: 
 
-Filename: sbcli_jm-4.0.9/simplyblock_core/controllers/lvol_controller.py
+Filename: sbcli_jm-4.1.0/simplyblock_core/controllers/lvol_controller.py
 Comment: 
 
-Filename: sbcli_jm-4.0.9/simplyblock_core/controllers/health_controller.py
+Filename: sbcli_jm-4.1.0/simplyblock_core/controllers/health_controller.py
 Comment: 
 
-Filename: sbcli_jm-4.0.9/simplyblock_core/controllers/pool_events.py
+Filename: sbcli_jm-4.1.0/simplyblock_core/controllers/pool_events.py
 Comment: 
 
-Filename: sbcli_jm-4.0.9/simplyblock_core/models/events.py
+Filename: sbcli_jm-4.1.0/simplyblock_core/models/events.py
 Comment: 
 
-Filename: sbcli_jm-4.0.9/simplyblock_core/models/iface.py
+Filename: sbcli_jm-4.1.0/simplyblock_core/models/iface.py
 Comment: 
 
-Filename: sbcli_jm-4.0.9/simplyblock_core/models/base_model.py
+Filename: sbcli_jm-4.1.0/simplyblock_core/models/base_model.py
 Comment: 
 
-Filename: sbcli_jm-4.0.9/simplyblock_core/models/lvol_model.py
+Filename: sbcli_jm-4.1.0/simplyblock_core/models/lvol_model.py
 Comment: 
 
-Filename: sbcli_jm-4.0.9/simplyblock_core/models/compute_node.py
+Filename: sbcli_jm-4.1.0/simplyblock_core/models/compute_node.py
 Comment: 
 
-Filename: sbcli_jm-4.0.9/simplyblock_core/models/snapshot.py
+Filename: sbcli_jm-4.1.0/simplyblock_core/models/snapshot.py
 Comment: 
 
-Filename: sbcli_jm-4.0.9/simplyblock_core/models/pool.py
+Filename: sbcli_jm-4.1.0/simplyblock_core/models/pool.py
 Comment: 
 
-Filename: sbcli_jm-4.0.9/simplyblock_core/models/global_settings.py
+Filename: sbcli_jm-4.1.0/simplyblock_core/models/global_settings.py
 Comment: 
 
-Filename: sbcli_jm-4.0.9/simplyblock_core/models/port_stat.py
+Filename: sbcli_jm-4.1.0/simplyblock_core/models/port_stat.py
 Comment: 
 
-Filename: sbcli_jm-4.0.9/simplyblock_core/models/storage_node.py
+Filename: sbcli_jm-4.1.0/simplyblock_core/models/storage_node.py
 Comment: 
 
-Filename: sbcli_jm-4.0.9/simplyblock_core/models/__init__.py
+Filename: sbcli_jm-4.1.0/simplyblock_core/models/__init__.py
 Comment: 
 
-Filename: sbcli_jm-4.0.9/simplyblock_core/models/stats.py
+Filename: sbcli_jm-4.1.0/simplyblock_core/models/stats.py
 Comment: 
 
-Filename: sbcli_jm-4.0.9/simplyblock_core/models/cluster.py
+Filename: sbcli_jm-4.1.0/simplyblock_core/models/cluster.py
 Comment: 
 
-Filename: sbcli_jm-4.0.9/simplyblock_core/models/mgmt_node.py
+Filename: sbcli_jm-4.1.0/simplyblock_core/models/mgmt_node.py
 Comment: 
 
-Filename: sbcli_jm-4.0.9/simplyblock_core/models/caching_node.py
+Filename: sbcli_jm-4.1.0/simplyblock_core/models/caching_node.py
 Comment: 
 
-Filename: sbcli_jm-4.0.9/simplyblock_core/models/nvme_device.py
+Filename: sbcli_jm-4.1.0/simplyblock_core/models/nvme_device.py
 Comment: 
 
-Filename: sbcli_jm-4.0.9/simplyblock_web/static/
+Filename: sbcli_jm-4.1.0/simplyblock_web/static/
 Comment: 
 
-Filename: sbcli_jm-4.0.9/simplyblock_web/templates/
+Filename: sbcli_jm-4.1.0/simplyblock_web/templates/
 Comment: 
 
-Filename: sbcli_jm-4.0.9/simplyblock_web/blueprints/
+Filename: sbcli_jm-4.1.0/simplyblock_web/blueprints/
 Comment: 
 
-Filename: sbcli_jm-4.0.9/simplyblock_web/caching_node_app_k8s.py
+Filename: sbcli_jm-4.1.0/simplyblock_web/caching_node_app_k8s.py
 Comment: 
 
-Filename: sbcli_jm-4.0.9/simplyblock_web/node_utils.py
+Filename: sbcli_jm-4.1.0/simplyblock_web/node_utils.py
 Comment: 
 
-Filename: sbcli_jm-4.0.9/simplyblock_web/snode_app.py
+Filename: sbcli_jm-4.1.0/simplyblock_web/snode_app.py
 Comment: 
 
-Filename: sbcli_jm-4.0.9/simplyblock_web/app.py
+Filename: sbcli_jm-4.1.0/simplyblock_web/app.py
 Comment: 
 
-Filename: sbcli_jm-4.0.9/simplyblock_web/auth_middleware.py
+Filename: sbcli_jm-4.1.0/simplyblock_web/auth_middleware.py
 Comment: 
 
-Filename: sbcli_jm-4.0.9/simplyblock_web/__init__.py
+Filename: sbcli_jm-4.1.0/simplyblock_web/__init__.py
 Comment: 
 
-Filename: sbcli_jm-4.0.9/simplyblock_web/caching_node_app.py
+Filename: sbcli_jm-4.1.0/simplyblock_web/caching_node_app.py
 Comment: 
 
-Filename: sbcli_jm-4.0.9/simplyblock_web/utils.py
+Filename: sbcli_jm-4.1.0/simplyblock_web/utils.py
 Comment: 
 
-Filename: sbcli_jm-4.0.9/simplyblock_web/node_webapp.py
+Filename: sbcli_jm-4.1.0/simplyblock_web/node_webapp.py
 Comment: 
 
-Filename: sbcli_jm-4.0.9/simplyblock_web/static/deploy_cnode.yaml
+Filename: sbcli_jm-4.1.0/simplyblock_web/static/deploy_cnode.yaml
 Comment: 
 
-Filename: sbcli_jm-4.0.9/simplyblock_web/static/tst.py
+Filename: sbcli_jm-4.1.0/simplyblock_web/static/tst.py
 Comment: 
 
-Filename: sbcli_jm-4.0.9/simplyblock_web/static/is_up.py
+Filename: sbcli_jm-4.1.0/simplyblock_web/static/is_up.py
 Comment: 
 
-Filename: sbcli_jm-4.0.9/simplyblock_web/static/delete.py
+Filename: sbcli_jm-4.1.0/simplyblock_web/static/delete.py
 Comment: 
 
-Filename: sbcli_jm-4.0.9/simplyblock_web/static/deploy.py
+Filename: sbcli_jm-4.1.0/simplyblock_web/static/deploy.py
 Comment: 
 
-Filename: sbcli_jm-4.0.9/simplyblock_web/static/deploy_spdk.yaml
+Filename: sbcli_jm-4.1.0/simplyblock_web/static/deploy_spdk.yaml
 Comment: 
 
-Filename: sbcli_jm-4.0.9/simplyblock_web/static/rpac.yaml
+Filename: sbcli_jm-4.1.0/simplyblock_web/static/rpac.yaml
 Comment: 
 
-Filename: sbcli_jm-4.0.9/simplyblock_web/static/list_deps.py
+Filename: sbcli_jm-4.1.0/simplyblock_web/static/list_deps.py
 Comment: 
 
-Filename: sbcli_jm-4.0.9/simplyblock_web/templates/deploy_spdk.yaml.j2
+Filename: sbcli_jm-4.1.0/simplyblock_web/templates/deploy_spdk.yaml.j2
 Comment: 
 
-Filename: sbcli_jm-4.0.9/simplyblock_web/blueprints/node_api_caching_docker.py
+Filename: sbcli_jm-4.1.0/simplyblock_web/blueprints/node_api_caching_docker.py
 Comment: 
 
-Filename: sbcli_jm-4.0.9/simplyblock_web/blueprints/node_api_caching_ks.py
+Filename: sbcli_jm-4.1.0/simplyblock_web/blueprints/node_api_caching_ks.py
 Comment: 
 
-Filename: sbcli_jm-4.0.9/simplyblock_web/blueprints/web_api_caching_node.py
+Filename: sbcli_jm-4.1.0/simplyblock_web/blueprints/web_api_caching_node.py
 Comment: 
 
-Filename: sbcli_jm-4.0.9/simplyblock_web/blueprints/snode_ops.py
+Filename: sbcli_jm-4.1.0/simplyblock_web/blueprints/snode_ops.py
 Comment: 
 
-Filename: sbcli_jm-4.0.9/simplyblock_web/blueprints/web_api_lvol.py
+Filename: sbcli_jm-4.1.0/simplyblock_web/blueprints/web_api_lvol.py
 Comment: 
 
-Filename: sbcli_jm-4.0.9/simplyblock_web/blueprints/csi.py
+Filename: sbcli_jm-4.1.0/simplyblock_web/blueprints/csi.py
 Comment: 
 
-Filename: sbcli_jm-4.0.9/simplyblock_web/blueprints/caching_node_ops.py
+Filename: sbcli_jm-4.1.0/simplyblock_web/blueprints/caching_node_ops.py
 Comment: 
 
-Filename: sbcli_jm-4.0.9/simplyblock_web/blueprints/web_api_mgmt_node.py
+Filename: sbcli_jm-4.1.0/simplyblock_web/blueprints/web_api_mgmt_node.py
 Comment: 
 
-Filename: sbcli_jm-4.0.9/simplyblock_web/blueprints/web_api_storage_node.py
+Filename: sbcli_jm-4.1.0/simplyblock_web/blueprints/web_api_storage_node.py
 Comment: 
 
-Filename: sbcli_jm-4.0.9/simplyblock_web/blueprints/__init__.py
+Filename: sbcli_jm-4.1.0/simplyblock_web/blueprints/__init__.py
 Comment: 
 
-Filename: sbcli_jm-4.0.9/simplyblock_web/blueprints/caching_node_ops_k8s.py
+Filename: sbcli_jm-4.1.0/simplyblock_web/blueprints/caching_node_ops_k8s.py
 Comment: 
 
-Filename: sbcli_jm-4.0.9/simplyblock_web/blueprints/web_api_device.py
+Filename: sbcli_jm-4.1.0/simplyblock_web/blueprints/web_api_device.py
 Comment: 
 
-Filename: sbcli_jm-4.0.9/simplyblock_web/blueprints/web_api_cluster.py
+Filename: sbcli_jm-4.1.0/simplyblock_web/blueprints/web_api_cluster.py
 Comment: 
 
-Filename: sbcli_jm-4.0.9/simplyblock_web/blueprints/node_api_basic.py
+Filename: sbcli_jm-4.1.0/simplyblock_web/blueprints/node_api_basic.py
 Comment: 
 
-Filename: sbcli_jm-4.0.9/simplyblock_web/blueprints/web_api_pool.py
+Filename: sbcli_jm-4.1.0/simplyblock_web/blueprints/web_api_pool.py
 Comment: 
 
 Zip file comment:
```

## Comparing `sbcli_jm-4.0.9/setup.py` & `sbcli_jm-4.1.0/setup.py`

 * *Files identical despite different names*

## Comparing `sbcli_jm-4.0.9/README.md` & `sbcli_jm-4.1.0/README.md`

 * *Files identical despite different names*

## Comparing `sbcli_jm-4.0.9/PKG-INFO` & `sbcli_jm-4.1.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sbcli-jm
-Version: 4.0.9
+Version: 4.1.0
 Summary: CLI for managing SimplyBlock cluster
 Home-page: https://www.simplyblock.io/
 Author: Hamdy
 Author-email: hamdy@simplyblock.io
 Description-Content-Type: text/markdown
 Requires-Dist: foundationdb
 Requires-Dist: requests
```

## Comparing `sbcli_jm-4.0.9/simplyblock_cli/cli.py` & `sbcli_jm-4.1.0/simplyblock_cli/cli.py`

 * *Files 0% similar despite different names*

```diff
@@ -40,16 +40,14 @@
         sub_command.add_argument("cluster_id", help='UUID of the cluster to which the node will belong')
         sub_command.add_argument("node_ip", help='IP of storage node to add')
         sub_command.add_argument("ifname", help='Management interface name')
         sub_command.add_argument("--data-nics", help='Data interface names', nargs='+', dest='data_nics')
         sub_command.add_argument("--cpu-mask", help='SPDK app CPU mask, default is all cores found',
                                  dest='spdk_cpu_mask')
         sub_command.add_argument("--memory", help='SPDK huge memory allocation, default is 4G', dest='spdk_mem')
-        sub_command.add_argument("--dev-split", help='Split nvme devices by this factor, can be 2 or more',
-                                 dest='dev_split', type=int, default=1)
         sub_command.add_argument("--spdk-image", help='SPDK image uri', dest='spdk_image')
         sub_command.add_argument("--spdk-debug", help='Enable spdk debug logs', dest='spdk_debug', required=False, action='store_true')
 
         sub_command.add_argument("--iobuf_small_pool_count", help='bdev_set_options param', dest='small_pool_count',  type=int, default=0)
         sub_command.add_argument("--iobuf_large_pool_count", help='bdev_set_options param', dest='large_pool_count',  type=int, default=0)
         sub_command.add_argument("--iobuf_small_bufsize", help='bdev_set_options param', dest='small_bufsize',  type=int, default=0)
         sub_command.add_argument("--iobuf_large_bufsize", help='bdev_set_options param', dest='large_bufsize',  type=int, default=0)
@@ -784,15 +782,14 @@
                 ret = self.storage_node_add(args)
 
             elif sub_command == "add-node":
                 cluster_id = args.cluster_id
                 node_ip = args.node_ip
                 ifname = args.ifname
                 data_nics = args.data_nics
-                dev_split = args.dev_split
                 spdk_image = args.spdk_image
                 spdk_debug = args.spdk_debug
 
                 small_pool_count = args.small_pool_count
                 large_pool_count = args.large_pool_count
                 small_bufsize = args.small_bufsize
                 large_bufsize = args.large_bufsize
@@ -807,15 +804,15 @@
                 spdk_mem = None
                 if args.spdk_mem:
                     spdk_mem = self.parse_size(args.spdk_mem)
                     if spdk_mem < 1 * 1024 * 1024:
                         return f"SPDK memory:{args.spdk_mem} must be larger than 1G"
 
                 out = storage_ops.add_node(
-                    cluster_id, node_ip, ifname, data_nics, spdk_cpu_mask, spdk_mem, dev_split, spdk_image, spdk_debug,
+                    cluster_id, node_ip, ifname, data_nics, spdk_cpu_mask, spdk_mem, spdk_image, spdk_debug,
                     small_pool_count, large_pool_count, small_bufsize, large_bufsize)
                 return out
 
             elif sub_command == "list":
                 ret = storage_ops.list_storage_nodes(self.db_store, args.json)
 
             elif sub_command == "remove":
```

## Comparing `sbcli_jm-4.0.9/sbcli_jm.egg-info/SOURCES.txt` & `sbcli_jm-4.1.0/sbcli_jm.egg-info/SOURCES.txt`

 * *Files identical despite different names*

## Comparing `sbcli_jm-4.0.9/sbcli_jm.egg-info/PKG-INFO` & `sbcli_jm-4.1.0/sbcli_jm.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sbcli-jm
-Version: 4.0.9
+Version: 4.1.0
 Summary: CLI for managing SimplyBlock cluster
 Home-page: https://www.simplyblock.io/
 Author: Hamdy
 Author-email: hamdy@simplyblock.io
 Description-Content-Type: text/markdown
 Requires-Dist: foundationdb
 Requires-Dist: requests
```

## Comparing `sbcli_jm-4.0.9/simplyblock_core/storage_node_ops.py` & `sbcli_jm-4.1.0/simplyblock_core/storage_node_ops.py`

 * *Files 1% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 from simplyblock_core import constants, scripts, distr_controller
 from simplyblock_core import utils
 from simplyblock_core.controllers import lvol_controller, storage_events, snapshot_controller, device_events, \
     device_controller
 from simplyblock_core.kv_store import DBController
 from simplyblock_core import shell_utils
 from simplyblock_core.models.iface import IFace
-from simplyblock_core.models.nvme_device import NVMeDevice
+from simplyblock_core.models.nvme_device import NVMeDevice, JMDevice
 from simplyblock_core.models.storage_node import StorageNode
 from simplyblock_core.pci_utils import get_nvme_devices, bind_spdk_driver
 from simplyblock_core.rpc_client import RPCClient
 from simplyblock_core.snode_client import SNodeClient
 
 logger = log.getLogger()
 
@@ -80,18 +80,20 @@
     exit(1)
 
 
 def addNvmeDevices(cluster, rpc_client, devs, snode):
     sequential_number = 0
     devices = []
     ret = rpc_client.bdev_nvme_controller_list()
-    if ret:
-        ctr_map = {i["ctrlrs"][0]['trid']['traddr']: i["name"] for i in ret}
-    else:
-        ctr_map = {}
+    ctr_map = {}
+    try:
+        if ret:
+            ctr_map = {i["ctrlrs"][0]['trid']['traddr']: i["name"] for i in ret}
+    except:
+        pass
 
     for index, pcie in enumerate(devs):
 
         if pcie in ctr_map:
             nvme_controller = ctr_map[pcie]
         else:
             nvme_controller = "nvme_%s" % index
@@ -128,20 +130,15 @@
                 'serial_number': nvme_driver_data['ctrlr_data']['serial_number'],
                 'nvme_bdev': nvme_bdev,
                 'nvme_controller': nvme_controller,
                 'node_id': snode.get_id(),
                 'cluster_id': snode.cluster_id,
                 'jm_bdev': jm_bdev,
                 'nvme_main_bdev': nvme_main_bdev,
-
-                # 'nvmf_nqn': subsystem_nqn,
-                # 'nvmf_ip': IP,
-                # 'nvmf_port': 4420,
-
-                'status': 'online'
+                'status': NVMeDevice.STATUS_ONLINE
         }))
         sequential_number += device_partitions_count
     return devices
 
 
 def _get_nvme_list(cluster):
     out, err, _ = shell_utils.run_command("sudo nvme list -v -o json")
@@ -322,33 +319,45 @@
         nvme.io_error = False
         old_status = nvme.status
         nvme.status = NVMeDevice.STATUS_ONLINE
         device_events.device_status_change(nvme, nvme.status, old_status)
         snode.write_to_db(db_controller.kv_store)
 
     if jm_nvme_bdevs:
-        ret = rpc_client.bdev_raid_create(f"raid_jm_{snode.get_id()}", jm_nvme_bdevs)
+        raid_bdev = f"raid_jm_{snode.get_id()}"
+        ret = rpc_client.bdev_raid_create(raid_bdev, jm_nvme_bdevs)
         if not ret:
             logger.error(f"Failed to create raid_jm_{snode.get_id()}")
             return False
         alceml_name = f"alceml_jm_{snode.get_id()}"
         pba_init_mode = 3
         if after_restart:
             pba_init_mode = 2
-        ret = rpc_client.bdev_alceml_create(alceml_name, f"raid_jm_{snode.get_id()}", str(uuid.uuid4()), pba_init_mode=pba_init_mode)
+        ret = rpc_client.bdev_alceml_create(alceml_name, raid_bdev, str(uuid.uuid4()), pba_init_mode=pba_init_mode)
         if not ret:
             logger.error(f"Failed to create alceml bdev: {alceml_name}")
             return False
 
         jm_bdev = f"jm_{snode.get_id()}"
         ret = rpc_client.bdev_jm_create(jm_bdev, alceml_name)
         if not ret:
             logger.error(f"Failed to create {jm_bdev}")
             return False
         snode.jm_bdev = jm_bdev
+        snode.jm_device = JMDevice({
+                'uuid': str(uuid.uuid4()),
+                'device_name': jm_bdev,
+                'size': 0,
+                'status': JMDevice.STATUS_ONLINE,
+
+                'jm_nvme_bdev_list': jm_nvme_bdevs,
+                'raid_bdev': raid_bdev,
+                'alceml_bdev': alceml_name,
+                'jm_bdev': jm_bdev
+            })
 
     snode.write_to_db(db_controller.kv_store)
     return True
 
 
 def _connect_to_remote_devs(this_node):
     db_controller = DBController()
@@ -375,15 +384,15 @@
                 continue
             dev.remote_bdev = f"{name}n1"
             remote_devices.append(dev)
     return remote_devices
 
 
 def add_node(cluster_id, node_ip, iface_name, data_nics_list, spdk_cpu_mask,
-             spdk_mem, dev_split=1, spdk_image=None, spdk_debug=False,
+             spdk_mem, spdk_image=None, spdk_debug=False,
              small_pool_count=0, large_pool_count=0, small_bufsize=0, large_bufsize=0):
     db_controller = DBController()
     kv_store = db_controller.kv_store
 
     cluster = db_controller.get_cluster_by_id(cluster_id)
     if not cluster:
         logger.error("Cluster not found: %s", cluster_id)
@@ -556,29 +565,15 @@
     node_info, _ = snode_api.info()
     # adding devices
     nvme_devs = addNvmeDevices(cluster, rpc_client, node_info['spdk_pcie_list'], snode)
     if not nvme_devs:
         logger.error("No NVMe devices was found!")
         return False
 
-    if dev_split > 1:
-        # split devices
-        new_devices = []
-        for dev in nvme_devs:
-            ret = rpc_client.bdev_split(dev.nvme_bdev, dev_split)
-            for pt in ret:
-                dev_dict = dev.get_clean_dict()
-                dev_dict['uuid'] = str(uuid.uuid4())
-                dev_dict['device_name'] = pt
-                dev_dict['nvme_bdev'] = pt
-                dev_dict['size'] = int(dev.size / dev_split)
-                new_devices.append(NVMeDevice(dev_dict))
-        snode.nvme_devices = new_devices
-    else:
-        snode.nvme_devices = nvme_devs
+    snode.nvme_devices = nvme_devs
 
     # Set device cluster order
     dev_order = get_next_cluster_device_order(db_controller)
     for index, nvme in enumerate(snode.nvme_devices):
         nvme.cluster_device_order = dev_order
         dev_order += 1
         device_events.device_create(nvme)
@@ -1135,27 +1130,33 @@
     data = []
     for device in snode.nvme_devices:
         logger.debug(device)
         logger.debug("*" * 20)
         data.append({
             "UUID": device.uuid,
             "Name": device.device_name,
-            "Hostname": snode.hostname,
             "Size": utils.humanbytes(device.size),
-            # "Sequential Number": device.sequential_number,
-            # "Partitions Count": device.partitions_count,
-            # "Model ID": device.model_id,
             "Serial Number": device.serial_number,
             "PCIe": device.pcie_address,
             "Status": device.status,
             "IO Err": device.io_error,
-            "Health": device.health_check,
-
+            "Health": device.health_check
         })
 
+    if snode.jm_device:
+        data.append({
+            "UUID": snode.jm_device.uuid,
+            "Name": snode.jm_device.device_name,
+            "Size": utils.humanbytes(snode.jm_device.size),
+            "Serial Number": "JM_DEVICE",
+            "PCIe": "JM_DEVICE",
+            "Status": snode.jm_device.status,
+            "IO Err": snode.jm_device.io_error,
+            "Health": snode.jm_device.health_check
+        })
     if sort and sort in ['node-seq', 'dev-seq', 'serial']:
         if sort == 'serial':
             sort_key = "Serial Number"
         elif sort == 'dev-seq':
             sort_key = "Sequential Number"
         elif sort == 'node-seq':
             # TODO: check this key
```

## Comparing `sbcli_jm-4.0.9/simplyblock_core/constants.py` & `sbcli_jm-4.1.0/simplyblock_core/constants.py`

 * *Files identical despite different names*

## Comparing `sbcli_jm-4.0.9/simplyblock_core/mgmt_node_ops.py` & `sbcli_jm-4.1.0/simplyblock_core/mgmt_node_ops.py`

 * *Files identical despite different names*

## Comparing `sbcli_jm-4.0.9/simplyblock_core/cnode_client.py` & `sbcli_jm-4.1.0/simplyblock_core/cnode_client.py`

 * *Files identical despite different names*

## Comparing `sbcli_jm-4.0.9/simplyblock_core/pci_utils.py` & `sbcli_jm-4.1.0/simplyblock_core/pci_utils.py`

 * *Files identical despite different names*

## Comparing `sbcli_jm-4.0.9/simplyblock_core/snode_client.py` & `sbcli_jm-4.1.0/simplyblock_core/snode_client.py`

 * *Files identical despite different names*

## Comparing `sbcli_jm-4.0.9/simplyblock_core/kv_store.py` & `sbcli_jm-4.1.0/simplyblock_core/kv_store.py`

 * *Files identical despite different names*

## Comparing `sbcli_jm-4.0.9/simplyblock_core/utils.py` & `sbcli_jm-4.1.0/simplyblock_core/utils.py`

 * *Files identical despite different names*

## Comparing `sbcli_jm-4.0.9/simplyblock_core/cluster_ops.py` & `sbcli_jm-4.1.0/simplyblock_core/cluster_ops.py`

 * *Files identical despite different names*

## Comparing `sbcli_jm-4.0.9/simplyblock_core/compute_node_ops.py` & `sbcli_jm-4.1.0/simplyblock_core/compute_node_ops.py`

 * *Files identical despite different names*

## Comparing `sbcli_jm-4.0.9/simplyblock_core/rpc_client.py` & `sbcli_jm-4.1.0/simplyblock_core/rpc_client.py`

 * *Files identical despite different names*

## Comparing `sbcli_jm-4.0.9/simplyblock_core/distr_controller.py` & `sbcli_jm-4.1.0/simplyblock_core/distr_controller.py`

 * *Files identical despite different names*

## Comparing `sbcli_jm-4.0.9/simplyblock_core/services/lvol_monitor.py` & `sbcli_jm-4.1.0/simplyblock_core/services/lvol_monitor.py`

 * *Files identical despite different names*

## Comparing `sbcli_jm-4.0.9/simplyblock_core/services/caching_node_monitor.py` & `sbcli_jm-4.1.0/simplyblock_core/services/caching_node_monitor.py`

 * *Files identical despite different names*

## Comparing `sbcli_jm-4.0.9/simplyblock_core/services/capacity_collector.py` & `sbcli_jm-4.1.0/simplyblock_core/services/capacity_collector.py`

 * *Files identical despite different names*

## Comparing `sbcli_jm-4.0.9/simplyblock_core/services/health_check_service.py` & `sbcli_jm-4.1.0/simplyblock_core/services/health_check_service.py`

 * *Files identical despite different names*

## Comparing `sbcli_jm-4.0.9/simplyblock_core/services/lvol_stat_collector.py` & `sbcli_jm-4.1.0/simplyblock_core/services/lvol_stat_collector.py`

 * *Files identical despite different names*

## Comparing `sbcli_jm-4.0.9/simplyblock_core/services/log_agg_service.py` & `sbcli_jm-4.1.0/simplyblock_core/services/log_agg_service.py`

 * *Files identical despite different names*

## Comparing `sbcli_jm-4.0.9/simplyblock_core/services/distr_event_collector.py` & `sbcli_jm-4.1.0/simplyblock_core/services/distr_event_collector.py`

 * *Files identical despite different names*

## Comparing `sbcli_jm-4.0.9/simplyblock_core/services/capacity_and_stats_collector.py` & `sbcli_jm-4.1.0/simplyblock_core/services/capacity_and_stats_collector.py`

 * *Files identical despite different names*

## Comparing `sbcli_jm-4.0.9/simplyblock_core/services/port_stat_collector.py` & `sbcli_jm-4.1.0/simplyblock_core/services/port_stat_collector.py`

 * *Files identical despite different names*

## Comparing `sbcli_jm-4.0.9/simplyblock_core/services/device_monitor.py` & `sbcli_jm-4.1.0/simplyblock_core/services/device_monitor.py`

 * *Files identical despite different names*

## Comparing `sbcli_jm-4.0.9/simplyblock_core/services/__init__.py` & `sbcli_jm-4.1.0/simplyblock_core/services/__init__.py`

 * *Files identical despite different names*

## Comparing `sbcli_jm-4.0.9/simplyblock_core/services/install_service.sh` & `sbcli_jm-4.1.0/simplyblock_core/services/install_service.sh`

 * *Files identical despite different names*

## Comparing `sbcli_jm-4.0.9/simplyblock_core/services/mgmt_node_monitor.py` & `sbcli_jm-4.1.0/simplyblock_core/services/mgmt_node_monitor.py`

 * *Files identical despite different names*

## Comparing `sbcli_jm-4.0.9/simplyblock_core/services/cap_monitor.py` & `sbcli_jm-4.1.0/simplyblock_core/services/cap_monitor.py`

 * *Files identical despite different names*

## Comparing `sbcli_jm-4.0.9/simplyblock_core/services/storage_node_monitor.py` & `sbcli_jm-4.1.0/simplyblock_core/services/storage_node_monitor.py`

 * *Files identical despite different names*

## Comparing `sbcli_jm-4.0.9/simplyblock_core/scripts/deploy_stack.sh` & `sbcli_jm-4.1.0/simplyblock_core/scripts/deploy_stack.sh`

 * *Files identical despite different names*

## Comparing `sbcli_jm-4.0.9/simplyblock_core/scripts/haproxy.cfg` & `sbcli_jm-4.1.0/simplyblock_core/scripts/haproxy.cfg`

 * *Files identical despite different names*

## Comparing `sbcli_jm-4.0.9/simplyblock_core/scripts/docker-compose-swarm.yml` & `sbcli_jm-4.1.0/simplyblock_core/scripts/docker-compose-swarm.yml`

 * *Files identical despite different names*

## Comparing `sbcli_jm-4.0.9/simplyblock_core/scripts/stack_deploy_wait.sh` & `sbcli_jm-4.1.0/simplyblock_core/scripts/stack_deploy_wait.sh`

 * *Files identical despite different names*

## Comparing `sbcli_jm-4.0.9/simplyblock_core/scripts/__init__.py` & `sbcli_jm-4.1.0/simplyblock_core/scripts/__init__.py`

 * *Files identical despite different names*

## Comparing `sbcli_jm-4.0.9/simplyblock_core/scripts/install_deps.sh` & `sbcli_jm-4.1.0/simplyblock_core/scripts/install_deps.sh`

 * *Files identical despite different names*

## Comparing `sbcli_jm-4.0.9/simplyblock_core/scripts/apply_dashboard.sh` & `sbcli_jm-4.1.0/simplyblock_core/scripts/apply_dashboard.sh`

 * *Files identical despite different names*

## Comparing `sbcli_jm-4.0.9/simplyblock_core/scripts/alerting/alert_rules.yaml` & `sbcli_jm-4.1.0/simplyblock_core/scripts/alerting/alert_rules.yaml`

 * *Files identical despite different names*

## Comparing `sbcli_jm-4.0.9/simplyblock_core/scripts/alerting/alert_resources.yaml` & `sbcli_jm-4.1.0/simplyblock_core/scripts/alerting/alert_resources.yaml`

 * *Files identical despite different names*

## Comparing `sbcli_jm-4.0.9/simplyblock_core/scripts/dashboards/devices.json` & `sbcli_jm-4.1.0/simplyblock_core/scripts/dashboards/devices.json`

 * *Files identical despite different names*

## Comparing `sbcli_jm-4.0.9/simplyblock_core/scripts/dashboards/nodes.json` & `sbcli_jm-4.1.0/simplyblock_core/scripts/dashboards/nodes.json`

 * *Files identical despite different names*

## Comparing `sbcli_jm-4.0.9/simplyblock_core/scripts/dashboards/lvols.json` & `sbcli_jm-4.1.0/simplyblock_core/scripts/dashboards/lvols.json`

 * *Files identical despite different names*

## Comparing `sbcli_jm-4.0.9/simplyblock_core/scripts/dashboards/cluster.json` & `sbcli_jm-4.1.0/simplyblock_core/scripts/dashboards/cluster.json`

 * *Files identical despite different names*

## Comparing `sbcli_jm-4.0.9/simplyblock_core/controllers/device_controller.py` & `sbcli_jm-4.1.0/simplyblock_core/controllers/device_controller.py`

 * *Files identical despite different names*

## Comparing `sbcli_jm-4.0.9/simplyblock_core/controllers/mgmt_events.py` & `sbcli_jm-4.1.0/simplyblock_core/controllers/mgmt_events.py`

 * *Files identical despite different names*

## Comparing `sbcli_jm-4.0.9/simplyblock_core/controllers/events_controller.py` & `sbcli_jm-4.1.0/simplyblock_core/controllers/events_controller.py`

 * *Files identical despite different names*

## Comparing `sbcli_jm-4.0.9/simplyblock_core/controllers/storage_events.py` & `sbcli_jm-4.1.0/simplyblock_core/controllers/storage_events.py`

 * *Files identical despite different names*

## Comparing `sbcli_jm-4.0.9/simplyblock_core/controllers/lvol_events.py` & `sbcli_jm-4.1.0/simplyblock_core/controllers/lvol_events.py`

 * *Files identical despite different names*

## Comparing `sbcli_jm-4.0.9/simplyblock_core/controllers/snapshot_controller.py` & `sbcli_jm-4.1.0/simplyblock_core/controllers/snapshot_controller.py`

 * *Files identical despite different names*

## Comparing `sbcli_jm-4.0.9/simplyblock_core/controllers/device_events.py` & `sbcli_jm-4.1.0/simplyblock_core/controllers/device_events.py`

 * *Files identical despite different names*

## Comparing `sbcli_jm-4.0.9/simplyblock_core/controllers/pool_controller.py` & `sbcli_jm-4.1.0/simplyblock_core/controllers/pool_controller.py`

 * *Files identical despite different names*

## Comparing `sbcli_jm-4.0.9/simplyblock_core/controllers/cluster_events.py` & `sbcli_jm-4.1.0/simplyblock_core/controllers/cluster_events.py`

 * *Files identical despite different names*

## Comparing `sbcli_jm-4.0.9/simplyblock_core/controllers/caching_node_controller.py` & `sbcli_jm-4.1.0/simplyblock_core/controllers/caching_node_controller.py`

 * *Files identical despite different names*

## Comparing `sbcli_jm-4.0.9/simplyblock_core/controllers/snapshot_events.py` & `sbcli_jm-4.1.0/simplyblock_core/controllers/snapshot_events.py`

 * *Files identical despite different names*

## Comparing `sbcli_jm-4.0.9/simplyblock_core/controllers/lvol_controller.py` & `sbcli_jm-4.1.0/simplyblock_core/controllers/lvol_controller.py`

 * *Files 1% similar despite different names*

```diff
@@ -162,15 +162,15 @@
                 return False, f"Invalid LVol max_w_mbytes: {max_w_mbytes} " \
                               f"Pool Max W MBytes has reached {total} of {pool.max_w_mbytes_per_sec}"
 
     return True, ""
 
 
 def get_jm_names(snode):
-    return [f"jm_{snode.get_id()}"]
+    return [snode.jm_device.jm_bdev] if snode.jm_device else []
 
 
 # Deprecated
 def add_lvol(name, size, host_id_or_name, pool_id_or_name, use_comp, use_crypto,
              distr_vuid, distr_ndcs, distr_npcs,
              max_rw_iops, max_rw_mbytes, max_r_mbytes, max_w_mbytes,
              distr_bs=None, distr_chunk_bs=None):
```

## Comparing `sbcli_jm-4.0.9/simplyblock_core/controllers/health_controller.py` & `sbcli_jm-4.1.0/simplyblock_core/controllers/health_controller.py`

 * *Files identical despite different names*

## Comparing `sbcli_jm-4.0.9/simplyblock_core/controllers/pool_events.py` & `sbcli_jm-4.1.0/simplyblock_core/controllers/pool_events.py`

 * *Files identical despite different names*

## Comparing `sbcli_jm-4.0.9/simplyblock_core/models/events.py` & `sbcli_jm-4.1.0/simplyblock_core/models/events.py`

 * *Files identical despite different names*

## Comparing `sbcli_jm-4.0.9/simplyblock_core/models/iface.py` & `sbcli_jm-4.1.0/simplyblock_core/models/iface.py`

 * *Files identical despite different names*

## Comparing `sbcli_jm-4.0.9/simplyblock_core/models/base_model.py` & `sbcli_jm-4.1.0/simplyblock_core/models/base_model.py`

 * *Files identical despite different names*

## Comparing `sbcli_jm-4.0.9/simplyblock_core/models/lvol_model.py` & `sbcli_jm-4.1.0/simplyblock_core/models/lvol_model.py`

 * *Files identical despite different names*

## Comparing `sbcli_jm-4.0.9/simplyblock_core/models/compute_node.py` & `sbcli_jm-4.1.0/simplyblock_core/models/compute_node.py`

 * *Files identical despite different names*

## Comparing `sbcli_jm-4.0.9/simplyblock_core/models/snapshot.py` & `sbcli_jm-4.1.0/simplyblock_core/models/snapshot.py`

 * *Files identical despite different names*

## Comparing `sbcli_jm-4.0.9/simplyblock_core/models/pool.py` & `sbcli_jm-4.1.0/simplyblock_core/models/pool.py`

 * *Files identical despite different names*

## Comparing `sbcli_jm-4.0.9/simplyblock_core/models/global_settings.py` & `sbcli_jm-4.1.0/simplyblock_core/models/global_settings.py`

 * *Files identical despite different names*

## Comparing `sbcli_jm-4.0.9/simplyblock_core/models/port_stat.py` & `sbcli_jm-4.1.0/simplyblock_core/models/port_stat.py`

 * *Files identical despite different names*

## Comparing `sbcli_jm-4.0.9/simplyblock_core/models/storage_node.py` & `sbcli_jm-4.1.0/simplyblock_core/models/storage_node.py`

 * *Files 2% similar despite different names*

```diff
@@ -74,14 +74,15 @@
         "spdk_image": {"type": str, "default": ""},
         "spdk_debug": {"type": bool, "default": False},
 
         "ec2_metadata": {"type": dict, "default": {}},
         "ec2_instance_id": {"type": str, "default": ""},
         "ec2_public_ip": {"type": str, "default": ""},
 
+        "jm_device": {"type": NVMeDevice, "default": None},
         "jm_bdev": {"type": str, "default": ""},
 
     }
 
     def __init__(self, data=None):
         super(StorageNode, self).__init__()
         self.set_attrs(self.attributes, data)
```

## Comparing `sbcli_jm-4.0.9/simplyblock_core/models/stats.py` & `sbcli_jm-4.1.0/simplyblock_core/models/stats.py`

 * *Files identical despite different names*

## Comparing `sbcli_jm-4.0.9/simplyblock_core/models/cluster.py` & `sbcli_jm-4.1.0/simplyblock_core/models/cluster.py`

 * *Files identical despite different names*

## Comparing `sbcli_jm-4.0.9/simplyblock_core/models/mgmt_node.py` & `sbcli_jm-4.1.0/simplyblock_core/models/mgmt_node.py`

 * *Files identical despite different names*

## Comparing `sbcli_jm-4.0.9/simplyblock_core/models/caching_node.py` & `sbcli_jm-4.1.0/simplyblock_core/models/caching_node.py`

 * *Files identical despite different names*

## Comparing `sbcli_jm-4.0.9/simplyblock_core/models/nvme_device.py` & `sbcli_jm-4.1.0/simplyblock_core/models/nvme_device.py`

 * *Files 10% similar despite different names*

```diff
@@ -52,9 +52,39 @@
         super(NVMeDevice, self).__init__()
         self.set_attrs(self.attributes, data)
         self.object_type = "object"
 
     def get_id(self):
         return self.uuid
 
-    def get_capacity_percentage(self):
-        return ((self.size - self.capacity) / self.size) * 100
+
+class JMDevice(BaseModel):
+
+    STATUS_ONLINE = 'online'
+    STATUS_UNAVAILABLE = 'unavailable'
+    STATUS_REMOVED = 'removed'
+    STATUS_FAILED = 'failed'
+    STATUS_READONLY = 'read_only'
+
+    attributes = {
+        "uuid": {"type": str, 'default': ""},
+        "device_name": {"type": str, 'default': ""},
+        "status": {"type": str, 'default': ""},
+        "size": {"type": int, 'default': -1},
+
+        "jm_nvme_bdev_list": {"type": List[str], 'default': []},
+        "raid_bdev": {"type": str, 'default': ""},
+        "alceml_bdev": {"type": str, 'default': ""},
+        "jm_bdev": {"type": str, 'default': ""},
+
+        "health_check": {"type": bool, "default": True},
+        "io_error": {"type": bool, 'default': False},
+    }
+
+    def __init__(self, data=None):
+        super(JMDevice, self).__init__()
+        self.set_attrs(self.attributes, data)
+        self.object_type = "object"
+
+    def get_id(self):
+        return self.uuid
+
```

## Comparing `sbcli_jm-4.0.9/simplyblock_web/caching_node_app_k8s.py` & `sbcli_jm-4.1.0/simplyblock_web/caching_node_app_k8s.py`

 * *Files identical despite different names*

## Comparing `sbcli_jm-4.0.9/simplyblock_web/node_utils.py` & `sbcli_jm-4.1.0/simplyblock_web/node_utils.py`

 * *Files identical despite different names*

## Comparing `sbcli_jm-4.0.9/simplyblock_web/snode_app.py` & `sbcli_jm-4.1.0/simplyblock_web/snode_app.py`

 * *Files identical despite different names*

## Comparing `sbcli_jm-4.0.9/simplyblock_web/app.py` & `sbcli_jm-4.1.0/simplyblock_web/app.py`

 * *Files identical despite different names*

## Comparing `sbcli_jm-4.0.9/simplyblock_web/auth_middleware.py` & `sbcli_jm-4.1.0/simplyblock_web/auth_middleware.py`

 * *Files identical despite different names*

## Comparing `sbcli_jm-4.0.9/simplyblock_web/caching_node_app.py` & `sbcli_jm-4.1.0/simplyblock_web/caching_node_app.py`

 * *Files identical despite different names*

## Comparing `sbcli_jm-4.0.9/simplyblock_web/utils.py` & `sbcli_jm-4.1.0/simplyblock_web/utils.py`

 * *Files identical despite different names*

## Comparing `sbcli_jm-4.0.9/simplyblock_web/node_webapp.py` & `sbcli_jm-4.1.0/simplyblock_web/node_webapp.py`

 * *Files identical despite different names*

## Comparing `sbcli_jm-4.0.9/simplyblock_web/static/delete.py` & `sbcli_jm-4.1.0/simplyblock_web/static/delete.py`

 * *Files identical despite different names*

## Comparing `sbcli_jm-4.0.9/simplyblock_web/static/deploy.py` & `sbcli_jm-4.1.0/simplyblock_web/static/deploy.py`

 * *Files identical despite different names*

## Comparing `sbcli_jm-4.0.9/simplyblock_web/static/deploy_spdk.yaml` & `sbcli_jm-4.1.0/simplyblock_web/static/deploy_spdk.yaml`

 * *Files identical despite different names*

## Comparing `sbcli_jm-4.0.9/simplyblock_web/templates/deploy_spdk.yaml.j2` & `sbcli_jm-4.1.0/simplyblock_web/templates/deploy_spdk.yaml.j2`

 * *Files identical despite different names*

## Comparing `sbcli_jm-4.0.9/simplyblock_web/blueprints/node_api_caching_docker.py` & `sbcli_jm-4.1.0/simplyblock_web/blueprints/node_api_caching_docker.py`

 * *Files identical despite different names*

## Comparing `sbcli_jm-4.0.9/simplyblock_web/blueprints/node_api_caching_ks.py` & `sbcli_jm-4.1.0/simplyblock_web/blueprints/node_api_caching_ks.py`

 * *Files identical despite different names*

## Comparing `sbcli_jm-4.0.9/simplyblock_web/blueprints/web_api_caching_node.py` & `sbcli_jm-4.1.0/simplyblock_web/blueprints/web_api_caching_node.py`

 * *Files identical despite different names*

## Comparing `sbcli_jm-4.0.9/simplyblock_web/blueprints/snode_ops.py` & `sbcli_jm-4.1.0/simplyblock_web/blueprints/snode_ops.py`

 * *Files 1% similar despite different names*

```diff
@@ -297,17 +297,17 @@
         data = request.get_json()
         nbd_device = data['nbd_device']
         jm_percent = data['jm_percent']
     except:
         pass
 
     cmd_list = [
-        f"parted -sf {nbd_device} mklabel gpt",
-        f"parted -sf {nbd_device} mkpart journal \"0%\" \"{jm_percent}%\"",
-        f"parted -sf {nbd_device} mkpart main \"{jm_percent}%\" \"100%\"",
+        f"parted -f {nbd_device} mklabel gpt",
+        f"parted -f {nbd_device} mkpart journal \"0%\" \"{jm_percent}%\"",
+        f"parted -f {nbd_device} mkpart main \"{jm_percent}%\" \"100%\"",
         f"sgdisk -t 1:6527994e-2c5a-4eec-9613-8f5944074e8b {nbd_device}",
         f"sgdisk -t 2:6527994e-2c5a-4eec-9613-8f5944074e8b {nbd_device}"
     ]
 
     for cmd in cmd_list:
         logger.debug(cmd)
         out, err, ret_code = shell_utils.run_command(cmd)
```

## Comparing `sbcli_jm-4.0.9/simplyblock_web/blueprints/web_api_lvol.py` & `sbcli_jm-4.1.0/simplyblock_web/blueprints/web_api_lvol.py`

 * *Files identical despite different names*

## Comparing `sbcli_jm-4.0.9/simplyblock_web/blueprints/csi.py` & `sbcli_jm-4.1.0/simplyblock_web/blueprints/csi.py`

 * *Files identical despite different names*

## Comparing `sbcli_jm-4.0.9/simplyblock_web/blueprints/caching_node_ops.py` & `sbcli_jm-4.1.0/simplyblock_web/blueprints/caching_node_ops.py`

 * *Files identical despite different names*

## Comparing `sbcli_jm-4.0.9/simplyblock_web/blueprints/web_api_mgmt_node.py` & `sbcli_jm-4.1.0/simplyblock_web/blueprints/web_api_mgmt_node.py`

 * *Files identical despite different names*

## Comparing `sbcli_jm-4.0.9/simplyblock_web/blueprints/web_api_storage_node.py` & `sbcli_jm-4.1.0/simplyblock_web/blueprints/web_api_storage_node.py`

 * *Files identical despite different names*

## Comparing `sbcli_jm-4.0.9/simplyblock_web/blueprints/caching_node_ops_k8s.py` & `sbcli_jm-4.1.0/simplyblock_web/blueprints/caching_node_ops_k8s.py`

 * *Files identical despite different names*

## Comparing `sbcli_jm-4.0.9/simplyblock_web/blueprints/web_api_device.py` & `sbcli_jm-4.1.0/simplyblock_web/blueprints/web_api_device.py`

 * *Files identical despite different names*

## Comparing `sbcli_jm-4.0.9/simplyblock_web/blueprints/web_api_cluster.py` & `sbcli_jm-4.1.0/simplyblock_web/blueprints/web_api_cluster.py`

 * *Files identical despite different names*

## Comparing `sbcli_jm-4.0.9/simplyblock_web/blueprints/node_api_basic.py` & `sbcli_jm-4.1.0/simplyblock_web/blueprints/node_api_basic.py`

 * *Files identical despite different names*

## Comparing `sbcli_jm-4.0.9/simplyblock_web/blueprints/web_api_pool.py` & `sbcli_jm-4.1.0/simplyblock_web/blueprints/web_api_pool.py`

 * *Files identical despite different names*

