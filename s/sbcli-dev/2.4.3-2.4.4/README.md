# Comparing `tmp/sbcli_dev-2.4.3.zip` & `tmp/sbcli_dev-2.4.4.zip`

## zipinfo {}

```diff
@@ -1,148 +1,148 @@
-Zip file size: 212993 bytes, number of entries: 146
-drwxr-xr-x  2.0 unx        0 b- stor 24-Apr-26 21:50 sbcli_dev-2.4.3/
-drwxr-xr-x  2.0 unx        0 b- stor 24-Apr-26 21:50 sbcli_dev-2.4.3/simplyblock_cli/
-drwxr-xr-x  2.0 unx        0 b- stor 24-Apr-26 21:50 sbcli_dev-2.4.3/sbcli_dev.egg-info/
-drwxr-xr-x  2.0 unx        0 b- stor 24-Apr-26 21:50 sbcli_dev-2.4.3/simplyblock_core/
-drwxr-xr-x  2.0 unx        0 b- stor 24-Apr-26 21:50 sbcli_dev-2.4.3/simplyblock_web/
--rw-r--r--  2.0 unx     2269 b- defN 24-Apr-26 21:49 sbcli_dev-2.4.3/setup.py
--rw-r--r--  2.0 unx     1068 b- defN 24-Apr-26 21:49 sbcli_dev-2.4.3/README.md
--rw-r--r--  2.0 unx      148 b- defN 24-Apr-26 21:49 sbcli_dev-2.4.3/env_var
--rw-r--r--  2.0 unx       84 b- defN 24-Apr-26 21:49 sbcli_dev-2.4.3/pyproject.toml
--rw-r--r--  2.0 unx       38 b- defN 24-Apr-26 21:50 sbcli_dev-2.4.3/setup.cfg
--rw-r--r--  2.0 unx     1489 b- defN 24-Apr-26 21:50 sbcli_dev-2.4.3/PKG-INFO
--rw-r--r--  2.0 unx    77199 b- defN 24-Apr-26 21:49 sbcli_dev-2.4.3/simplyblock_cli/cli.py
--rw-r--r--  2.0 unx      357 b- defN 24-Apr-26 21:49 sbcli_dev-2.4.3/simplyblock_cli/main.py
--rw-r--r--  2.0 unx        1 b- defN 24-Apr-26 21:50 sbcli_dev-2.4.3/sbcli_dev.egg-info/dependency_links.txt
--rw-r--r--  2.0 unx     5188 b- defN 24-Apr-26 21:50 sbcli_dev-2.4.3/sbcli_dev.egg-info/SOURCES.txt
--rw-r--r--  2.0 unx       49 b- defN 24-Apr-26 21:50 sbcli_dev-2.4.3/sbcli_dev.egg-info/top_level.txt
--rw-r--r--  2.0 unx     1489 b- defN 24-Apr-26 21:50 sbcli_dev-2.4.3/sbcli_dev.egg-info/PKG-INFO
--rw-r--r--  2.0 unx       73 b- defN 24-Apr-26 21:50 sbcli_dev-2.4.3/sbcli_dev.egg-info/requires.txt
--rw-r--r--  2.0 unx       55 b- defN 24-Apr-26 21:50 sbcli_dev-2.4.3/sbcli_dev.egg-info/entry_points.txt
-drwxr-xr-x  2.0 unx        0 b- stor 24-Apr-26 21:50 sbcli_dev-2.4.3/simplyblock_core/services/
-drwxr-xr-x  2.0 unx        0 b- stor 24-Apr-26 21:50 sbcli_dev-2.4.3/simplyblock_core/scripts/
-drwxr-xr-x  2.0 unx        0 b- stor 24-Apr-26 21:50 sbcli_dev-2.4.3/simplyblock_core/controllers/
-drwxr-xr-x  2.0 unx        0 b- stor 24-Apr-26 21:50 sbcli_dev-2.4.3/simplyblock_core/models/
--rw-r--r--  2.0 unx    65987 b- defN 24-Apr-26 21:49 sbcli_dev-2.4.3/simplyblock_core/storage_node_ops.py
--rw-r--r--  2.0 unx     1440 b- defN 24-Apr-26 21:49 sbcli_dev-2.4.3/simplyblock_core/constants.py
--rw-r--r--  2.0 unx     3153 b- defN 24-Apr-26 21:49 sbcli_dev-2.4.3/simplyblock_core/mgmt_node_ops.py
--rw-r--r--  2.0 unx     3444 b- defN 24-Apr-26 21:49 sbcli_dev-2.4.3/simplyblock_core/cnode_client.py
--rw-r--r--  2.0 unx      279 b- defN 24-Apr-26 21:49 sbcli_dev-2.4.3/simplyblock_core/shell_utils.py
--rw-r--r--  2.0 unx      938 b- defN 24-Apr-26 21:49 sbcli_dev-2.4.3/simplyblock_core/pci_utils.py
--rw-r--r--  2.0 unx        0 b- defN 24-Apr-26 21:49 sbcli_dev-2.4.3/simplyblock_core/__init__.py
--rw-r--r--  2.0 unx     3193 b- defN 24-Apr-26 21:49 sbcli_dev-2.4.3/simplyblock_core/snode_client.py
--rw-r--r--  2.0 unx     8189 b- defN 24-Apr-26 21:49 sbcli_dev-2.4.3/simplyblock_core/kv_store.py
--rw-r--r--  2.0 unx     7640 b- defN 24-Apr-26 21:49 sbcli_dev-2.4.3/simplyblock_core/utils.py
--rw-r--r--  2.0 unx    23335 b- defN 24-Apr-26 21:49 sbcli_dev-2.4.3/simplyblock_core/cluster_ops.py
--rw-r--r--  2.0 unx     5112 b- defN 24-Apr-26 21:49 sbcli_dev-2.4.3/simplyblock_core/compute_node_ops.py
--rw-r--r--  2.0 unx    21493 b- defN 24-Apr-26 21:49 sbcli_dev-2.4.3/simplyblock_core/rpc_client.py
--rw-r--r--  2.0 unx     7479 b- defN 24-Apr-26 21:49 sbcli_dev-2.4.3/simplyblock_core/distr_controller.py
--rw-r--r--  2.0 unx     2189 b- defN 24-Apr-26 21:49 sbcli_dev-2.4.3/simplyblock_core/services/lvol_monitor.py
--rw-r--r--  2.0 unx     3203 b- defN 24-Apr-26 21:49 sbcli_dev-2.4.3/simplyblock_core/services/caching_node_monitor.py
--rw-r--r--  2.0 unx     5462 b- defN 24-Apr-26 21:49 sbcli_dev-2.4.3/simplyblock_core/services/health_check_service.py
--rw-r--r--  2.0 unx      229 b- defN 24-Apr-26 21:49 sbcli_dev-2.4.3/simplyblock_core/services/service_template.service
--rw-r--r--  2.0 unx     5268 b- defN 24-Apr-26 21:49 sbcli_dev-2.4.3/simplyblock_core/services/lvol_stat_collector.py
--rw-r--r--  2.0 unx      173 b- defN 24-Apr-26 21:49 sbcli_dev-2.4.3/simplyblock_core/services/remove_service.sh
--rw-r--r--  2.0 unx     2410 b- defN 24-Apr-26 21:49 sbcli_dev-2.4.3/simplyblock_core/services/log_agg_service.py
--rw-r--r--  2.0 unx     5140 b- defN 24-Apr-26 21:49 sbcli_dev-2.4.3/simplyblock_core/services/distr_event_collector.py
--rw-r--r--  2.0 unx     7439 b- defN 24-Apr-26 21:49 sbcli_dev-2.4.3/simplyblock_core/services/capacity_and_stats_collector.py
--rw-r--r--  2.0 unx     2423 b- defN 24-Apr-26 21:49 sbcli_dev-2.4.3/simplyblock_core/services/port_stat_collector.py
--rw-r--r--  2.0 unx     2499 b- defN 24-Apr-26 21:49 sbcli_dev-2.4.3/simplyblock_core/services/device_monitor.py
--rw-r--r--  2.0 unx     4118 b- defN 24-Apr-26 21:49 sbcli_dev-2.4.3/simplyblock_core/services/__init__.py
--rw-r--r--  2.0 unx      837 b- defN 24-Apr-26 21:49 sbcli_dev-2.4.3/simplyblock_core/services/install_service.sh
--rw-r--r--  2.0 unx     3003 b- defN 24-Apr-26 21:49 sbcli_dev-2.4.3/simplyblock_core/services/mgmt_node_monitor.py
--rw-r--r--  2.0 unx     2671 b- defN 24-Apr-26 21:49 sbcli_dev-2.4.3/simplyblock_core/services/cap_monitor.py
--rw-r--r--  2.0 unx     6577 b- defN 24-Apr-26 21:49 sbcli_dev-2.4.3/simplyblock_core/services/storage_node_monitor.py
-drwxr-xr-x  2.0 unx        0 b- stor 24-Apr-26 21:50 sbcli_dev-2.4.3/simplyblock_core/scripts/alerting/
-drwxr-xr-x  2.0 unx        0 b- stor 24-Apr-26 21:50 sbcli_dev-2.4.3/simplyblock_core/scripts/dashboards/
--rw-r--r--  2.0 unx      871 b- defN 24-Apr-26 21:49 sbcli_dev-2.4.3/simplyblock_core/scripts/deploy_stack.sh
--rw-r--r--  2.0 unx      152 b- defN 24-Apr-26 21:49 sbcli_dev-2.4.3/simplyblock_core/scripts/set_db_config.sh
--rw-r--r--  2.0 unx     1163 b- defN 24-Apr-26 21:49 sbcli_dev-2.4.3/simplyblock_core/scripts/haproxy.cfg
--rw-r--r--  2.0 unx     4977 b- defN 24-Apr-26 21:49 sbcli_dev-2.4.3/simplyblock_core/scripts/docker-compose-swarm.yml
--rw-r--r--  2.0 unx       54 b- defN 24-Apr-26 21:49 sbcli_dev-2.4.3/simplyblock_core/scripts/db_config_single.sh
--rw-r--r--  2.0 unx     5305 b- defN 24-Apr-26 21:49 sbcli_dev-2.4.3/simplyblock_core/scripts/stack_deploy_wait.sh
--rw-r--r--  2.0 unx     4142 b- defN 24-Apr-26 21:49 sbcli_dev-2.4.3/simplyblock_core/scripts/docker-compose-swarm-monitoring.yml
--rw-r--r--  2.0 unx      453 b- defN 24-Apr-26 21:49 sbcli_dev-2.4.3/simplyblock_core/scripts/config_docker.sh
--rw-r--r--  2.0 unx     1694 b- defN 24-Apr-26 21:49 sbcli_dev-2.4.3/simplyblock_core/scripts/__init__.py
--rw-r--r--  2.0 unx      311 b- defN 24-Apr-26 21:49 sbcli_dev-2.4.3/simplyblock_core/scripts/clean_local_storage_deploy.sh
--rw-r--r--  2.0 unx      118 b- defN 24-Apr-26 21:49 sbcli_dev-2.4.3/simplyblock_core/scripts/db_config_double.sh
--rw-r--r--  2.0 unx      360 b- defN 24-Apr-26 21:49 sbcli_dev-2.4.3/simplyblock_core/scripts/datasource.yml
--rw-r--r--  2.0 unx       43 b- defN 24-Apr-26 21:49 sbcli_dev-2.4.3/simplyblock_core/scripts/run_ssh.sh
--rw-r--r--  2.0 unx     1420 b- defN 24-Apr-26 21:49 sbcli_dev-2.4.3/simplyblock_core/scripts/install_deps.sh
--rw-r--r--  2.0 unx      311 b- defN 24-Apr-26 21:49 sbcli_dev-2.4.3/simplyblock_core/scripts/prometheus.yml
--rwxr-xr-x  2.0 unx      657 b- defN 24-Apr-26 21:49 sbcli_dev-2.4.3/simplyblock_core/scripts/apply_dashboard.sh
--rw-r--r--  2.0 unx    25433 b- defN 24-Apr-26 21:49 sbcli_dev-2.4.3/simplyblock_core/scripts/alerting/alert_rules.yaml
--rw-r--r--  2.0 unx     1856 b- defN 24-Apr-26 21:49 sbcli_dev-2.4.3/simplyblock_core/scripts/alerting/alert_resources.yaml
--rw-r--r--  2.0 unx   106705 b- defN 24-Apr-26 21:49 sbcli_dev-2.4.3/simplyblock_core/scripts/dashboards/devices.json
--rw-r--r--  2.0 unx   799409 b- defN 24-Apr-26 21:49 sbcli_dev-2.4.3/simplyblock_core/scripts/dashboards/node-exporter.json
--rw-r--r--  2.0 unx    99758 b- defN 24-Apr-26 21:49 sbcli_dev-2.4.3/simplyblock_core/scripts/dashboards/nodes.json
--rw-r--r--  2.0 unx    99707 b- defN 24-Apr-26 21:49 sbcli_dev-2.4.3/simplyblock_core/scripts/dashboards/lvols.json
--rw-r--r--  2.0 unx    99862 b- defN 24-Apr-26 21:49 sbcli_dev-2.4.3/simplyblock_core/scripts/dashboards/cluster.json
--rw-r--r--  2.0 unx    99707 b- defN 24-Apr-26 21:49 sbcli_dev-2.4.3/simplyblock_core/scripts/dashboards/pools.json
--rw-r--r--  2.0 unx    13877 b- defN 24-Apr-26 21:49 sbcli_dev-2.4.3/simplyblock_core/controllers/device_controller.py
--rw-r--r--  2.0 unx     1120 b- defN 24-Apr-26 21:49 sbcli_dev-2.4.3/simplyblock_core/controllers/mgmt_events.py
--rw-r--r--  2.0 unx     3191 b- defN 24-Apr-26 21:49 sbcli_dev-2.4.3/simplyblock_core/controllers/events_controller.py
--rw-r--r--  2.0 unx     1521 b- defN 24-Apr-26 21:49 sbcli_dev-2.4.3/simplyblock_core/controllers/storage_events.py
--rw-r--r--  2.0 unx     1630 b- defN 24-Apr-26 21:49 sbcli_dev-2.4.3/simplyblock_core/controllers/lvol_events.py
--rw-r--r--  2.0 unx    10557 b- defN 24-Apr-26 21:49 sbcli_dev-2.4.3/simplyblock_core/controllers/snapshot_controller.py
--rw-r--r--  2.0 unx     1568 b- defN 24-Apr-26 21:49 sbcli_dev-2.4.3/simplyblock_core/controllers/device_events.py
--rw-r--r--  2.0 unx    10375 b- defN 24-Apr-26 21:49 sbcli_dev-2.4.3/simplyblock_core/controllers/pool_controller.py
--rw-r--r--  2.0 unx        0 b- defN 24-Apr-26 21:49 sbcli_dev-2.4.3/simplyblock_core/controllers/__init__.py
--rw-r--r--  2.0 unx     1900 b- defN 24-Apr-26 21:49 sbcli_dev-2.4.3/simplyblock_core/controllers/cluster_events.py
--rw-r--r--  2.0 unx    22847 b- defN 24-Apr-26 21:49 sbcli_dev-2.4.3/simplyblock_core/controllers/caching_node_controller.py
--rw-r--r--  2.0 unx     1122 b- defN 24-Apr-26 21:49 sbcli_dev-2.4.3/simplyblock_core/controllers/snapshot_events.py
--rw-r--r--  2.0 unx    47339 b- defN 24-Apr-26 21:49 sbcli_dev-2.4.3/simplyblock_core/controllers/lvol_controller.py
--rw-r--r--  2.0 unx    11294 b- defN 24-Apr-26 21:49 sbcli_dev-2.4.3/simplyblock_core/controllers/health_controller.py
--rw-r--r--  2.0 unx      695 b- defN 24-Apr-26 21:49 sbcli_dev-2.4.3/simplyblock_core/controllers/pool_events.py
--rw-r--r--  2.0 unx     1500 b- defN 24-Apr-26 21:49 sbcli_dev-2.4.3/simplyblock_core/models/events.py
--rw-r--r--  2.0 unx      806 b- defN 24-Apr-26 21:49 sbcli_dev-2.4.3/simplyblock_core/models/iface.py
--rw-r--r--  2.0 unx     4846 b- defN 24-Apr-26 21:49 sbcli_dev-2.4.3/simplyblock_core/models/base_model.py
--rw-r--r--  2.0 unx     2579 b- defN 24-Apr-26 21:49 sbcli_dev-2.4.3/simplyblock_core/models/lvol_model.py
--rw-r--r--  2.0 unx      917 b- defN 24-Apr-26 21:49 sbcli_dev-2.4.3/simplyblock_core/models/compute_node.py
--rw-r--r--  2.0 unx      736 b- defN 24-Apr-26 21:49 sbcli_dev-2.4.3/simplyblock_core/models/snapshot.py
--rw-r--r--  2.0 unx     1602 b- defN 24-Apr-26 21:49 sbcli_dev-2.4.3/simplyblock_core/models/pool.py
--rw-r--r--  2.0 unx     1228 b- defN 24-Apr-26 21:49 sbcli_dev-2.4.3/simplyblock_core/models/global_settings.py
--rw-r--r--  2.0 unx     1020 b- defN 24-Apr-26 21:49 sbcli_dev-2.4.3/simplyblock_core/models/port_stat.py
--rw-r--r--  2.0 unx     3696 b- defN 24-Apr-26 21:49 sbcli_dev-2.4.3/simplyblock_core/models/storage_node.py
--rw-r--r--  2.0 unx        0 b- defN 24-Apr-26 21:49 sbcli_dev-2.4.3/simplyblock_core/models/__init__.py
--rw-r--r--  2.0 unx     4242 b- defN 24-Apr-26 21:49 sbcli_dev-2.4.3/simplyblock_core/models/stats.py
--rw-r--r--  2.0 unx     2565 b- defN 24-Apr-26 21:49 sbcli_dev-2.4.3/simplyblock_core/models/cluster.py
--rw-r--r--  2.0 unx     1466 b- defN 24-Apr-26 21:49 sbcli_dev-2.4.3/simplyblock_core/models/mgmt_node.py
--rw-r--r--  2.0 unx     3766 b- defN 24-Apr-26 21:49 sbcli_dev-2.4.3/simplyblock_core/models/caching_node.py
--rw-r--r--  2.0 unx     2071 b- defN 24-Apr-26 21:49 sbcli_dev-2.4.3/simplyblock_core/models/nvme_device.py
-drwxr-xr-x  2.0 unx        0 b- stor 24-Apr-26 21:50 sbcli_dev-2.4.3/simplyblock_web/static/
-drwxr-xr-x  2.0 unx        0 b- stor 24-Apr-26 21:50 sbcli_dev-2.4.3/simplyblock_web/templates/
-drwxr-xr-x  2.0 unx        0 b- stor 24-Apr-26 21:50 sbcli_dev-2.4.3/simplyblock_web/blueprints/
--rw-r--r--  2.0 unx      725 b- defN 24-Apr-26 21:49 sbcli_dev-2.4.3/simplyblock_web/caching_node_app_k8s.py
--rw-r--r--  2.0 unx     5098 b- defN 24-Apr-26 21:49 sbcli_dev-2.4.3/simplyblock_web/node_utils.py
--rw-r--r--  2.0 unx      703 b- defN 24-Apr-26 21:49 sbcli_dev-2.4.3/simplyblock_web/snode_app.py
--rw-r--r--  2.0 unx     1263 b- defN 24-Apr-26 21:49 sbcli_dev-2.4.3/simplyblock_web/app.py
--rw-r--r--  2.0 unx     1638 b- defN 24-Apr-26 21:49 sbcli_dev-2.4.3/simplyblock_web/auth_middleware.py
--rw-r--r--  2.0 unx        0 b- defN 24-Apr-26 21:49 sbcli_dev-2.4.3/simplyblock_web/__init__.py
--rw-r--r--  2.0 unx      717 b- defN 24-Apr-26 21:49 sbcli_dev-2.4.3/simplyblock_web/caching_node_app.py
--rw-r--r--  2.0 unx     2513 b- defN 24-Apr-26 21:49 sbcli_dev-2.4.3/simplyblock_web/utils.py
--rw-r--r--  2.0 unx     1434 b- defN 24-Apr-26 21:49 sbcli_dev-2.4.3/simplyblock_web/node_webapp.py
--rw-r--r--  2.0 unx      507 b- defN 24-Apr-26 21:49 sbcli_dev-2.4.3/simplyblock_web/static/deploy_cnode.yaml
--rw-r--r--  2.0 unx      322 b- defN 24-Apr-26 21:49 sbcli_dev-2.4.3/simplyblock_web/static/tst.py
--rw-r--r--  2.0 unx      434 b- defN 24-Apr-26 21:49 sbcli_dev-2.4.3/simplyblock_web/static/is_up.py
--rw-r--r--  2.0 unx      827 b- defN 24-Apr-26 21:49 sbcli_dev-2.4.3/simplyblock_web/static/delete.py
--rw-r--r--  2.0 unx     1302 b- defN 24-Apr-26 21:49 sbcli_dev-2.4.3/simplyblock_web/static/deploy.py
--rw-r--r--  2.0 unx     1466 b- defN 24-Apr-26 21:49 sbcli_dev-2.4.3/simplyblock_web/static/deploy_spdk.yaml
--rw-r--r--  2.0 unx      463 b- defN 24-Apr-26 21:49 sbcli_dev-2.4.3/simplyblock_web/static/rpac.yaml
--rw-r--r--  2.0 unx      417 b- defN 24-Apr-26 21:49 sbcli_dev-2.4.3/simplyblock_web/static/list_deps.py
--rw-r--r--  2.0 unx     2876 b- defN 24-Apr-26 21:49 sbcli_dev-2.4.3/simplyblock_web/templates/deploy_spdk.yaml.j2
--rw-r--r--  2.0 unx     5547 b- defN 24-Apr-26 21:49 sbcli_dev-2.4.3/simplyblock_web/blueprints/node_api_caching_docker.py
--rw-r--r--  2.0 unx     4795 b- defN 24-Apr-26 21:49 sbcli_dev-2.4.3/simplyblock_web/blueprints/node_api_caching_ks.py
--rw-r--r--  2.0 unx     5317 b- defN 24-Apr-26 21:49 sbcli_dev-2.4.3/simplyblock_web/blueprints/web_api_caching_node.py
--rw-r--r--  2.0 unx     9573 b- defN 24-Apr-26 21:49 sbcli_dev-2.4.3/simplyblock_web/blueprints/snode_ops.py
--rw-r--r--  2.0 unx     8547 b- defN 24-Apr-26 21:49 sbcli_dev-2.4.3/simplyblock_web/blueprints/web_api_lvol.py
--rw-r--r--  2.0 unx    11244 b- defN 24-Apr-26 21:49 sbcli_dev-2.4.3/simplyblock_web/blueprints/csi.py
--rw-r--r--  2.0 unx    12198 b- defN 24-Apr-26 21:49 sbcli_dev-2.4.3/simplyblock_web/blueprints/caching_node_ops.py
--rw-r--r--  2.0 unx      975 b- defN 24-Apr-26 21:49 sbcli_dev-2.4.3/simplyblock_web/blueprints/web_api_mgmt_node.py
--rw-r--r--  2.0 unx     6326 b- defN 24-Apr-26 21:49 sbcli_dev-2.4.3/simplyblock_web/blueprints/web_api_storage_node.py
--rw-r--r--  2.0 unx        0 b- defN 24-Apr-26 21:49 sbcli_dev-2.4.3/simplyblock_web/blueprints/__init__.py
--rw-r--r--  2.0 unx     7846 b- defN 24-Apr-26 21:49 sbcli_dev-2.4.3/simplyblock_web/blueprints/caching_node_ops_k8s.py
--rw-r--r--  2.0 unx     2940 b- defN 24-Apr-26 21:49 sbcli_dev-2.4.3/simplyblock_web/blueprints/web_api_device.py
--rw-r--r--  2.0 unx     5274 b- defN 24-Apr-26 21:49 sbcli_dev-2.4.3/simplyblock_web/blueprints/web_api_cluster.py
--rw-r--r--  2.0 unx     3103 b- defN 24-Apr-26 21:49 sbcli_dev-2.4.3/simplyblock_web/blueprints/node_api_basic.py
--rw-r--r--  2.0 unx     6206 b- defN 24-Apr-26 21:49 sbcli_dev-2.4.3/simplyblock_web/blueprints/web_api_pool.py
-146 files, 1923970 bytes uncompressed, 186415 bytes compressed:  90.3%
+Zip file size: 213368 bytes, number of entries: 146
+drwxr-xr-x  2.0 unx        0 b- stor 24-Apr-29 15:05 sbcli_dev-2.4.4/
+drwxr-xr-x  2.0 unx        0 b- stor 24-Apr-29 15:05 sbcli_dev-2.4.4/simplyblock_cli/
+drwxr-xr-x  2.0 unx        0 b- stor 24-Apr-29 15:05 sbcli_dev-2.4.4/sbcli_dev.egg-info/
+drwxr-xr-x  2.0 unx        0 b- stor 24-Apr-29 15:05 sbcli_dev-2.4.4/simplyblock_core/
+drwxr-xr-x  2.0 unx        0 b- stor 24-Apr-29 15:05 sbcli_dev-2.4.4/simplyblock_web/
+-rw-r--r--  2.0 unx     2269 b- defN 24-Apr-29 15:05 sbcli_dev-2.4.4/setup.py
+-rw-r--r--  2.0 unx     1068 b- defN 24-Apr-29 15:05 sbcli_dev-2.4.4/README.md
+-rw-r--r--  2.0 unx      148 b- defN 24-Apr-29 15:05 sbcli_dev-2.4.4/env_var
+-rw-r--r--  2.0 unx       84 b- defN 24-Apr-29 15:05 sbcli_dev-2.4.4/pyproject.toml
+-rw-r--r--  2.0 unx       38 b- defN 24-Apr-29 15:05 sbcli_dev-2.4.4/setup.cfg
+-rw-r--r--  2.0 unx     1489 b- defN 24-Apr-29 15:05 sbcli_dev-2.4.4/PKG-INFO
+-rw-r--r--  2.0 unx    77737 b- defN 24-Apr-29 15:05 sbcli_dev-2.4.4/simplyblock_cli/cli.py
+-rw-r--r--  2.0 unx      357 b- defN 24-Apr-29 15:05 sbcli_dev-2.4.4/simplyblock_cli/main.py
+-rw-r--r--  2.0 unx        1 b- defN 24-Apr-29 15:05 sbcli_dev-2.4.4/sbcli_dev.egg-info/dependency_links.txt
+-rw-r--r--  2.0 unx     5188 b- defN 24-Apr-29 15:05 sbcli_dev-2.4.4/sbcli_dev.egg-info/SOURCES.txt
+-rw-r--r--  2.0 unx       49 b- defN 24-Apr-29 15:05 sbcli_dev-2.4.4/sbcli_dev.egg-info/top_level.txt
+-rw-r--r--  2.0 unx     1489 b- defN 24-Apr-29 15:05 sbcli_dev-2.4.4/sbcli_dev.egg-info/PKG-INFO
+-rw-r--r--  2.0 unx       73 b- defN 24-Apr-29 15:05 sbcli_dev-2.4.4/sbcli_dev.egg-info/requires.txt
+-rw-r--r--  2.0 unx       55 b- defN 24-Apr-29 15:05 sbcli_dev-2.4.4/sbcli_dev.egg-info/entry_points.txt
+drwxr-xr-x  2.0 unx        0 b- stor 24-Apr-29 15:05 sbcli_dev-2.4.4/simplyblock_core/services/
+drwxr-xr-x  2.0 unx        0 b- stor 24-Apr-29 15:05 sbcli_dev-2.4.4/simplyblock_core/scripts/
+drwxr-xr-x  2.0 unx        0 b- stor 24-Apr-29 15:05 sbcli_dev-2.4.4/simplyblock_core/controllers/
+drwxr-xr-x  2.0 unx        0 b- stor 24-Apr-29 15:05 sbcli_dev-2.4.4/simplyblock_core/models/
+-rw-r--r--  2.0 unx    65987 b- defN 24-Apr-29 15:05 sbcli_dev-2.4.4/simplyblock_core/storage_node_ops.py
+-rw-r--r--  2.0 unx     1494 b- defN 24-Apr-29 15:05 sbcli_dev-2.4.4/simplyblock_core/constants.py
+-rw-r--r--  2.0 unx     3153 b- defN 24-Apr-29 15:05 sbcli_dev-2.4.4/simplyblock_core/mgmt_node_ops.py
+-rw-r--r--  2.0 unx     3444 b- defN 24-Apr-29 15:05 sbcli_dev-2.4.4/simplyblock_core/cnode_client.py
+-rw-r--r--  2.0 unx      279 b- defN 24-Apr-29 15:05 sbcli_dev-2.4.4/simplyblock_core/shell_utils.py
+-rw-r--r--  2.0 unx      938 b- defN 24-Apr-29 15:05 sbcli_dev-2.4.4/simplyblock_core/pci_utils.py
+-rw-r--r--  2.0 unx        0 b- defN 24-Apr-29 15:05 sbcli_dev-2.4.4/simplyblock_core/__init__.py
+-rw-r--r--  2.0 unx     3193 b- defN 24-Apr-29 15:05 sbcli_dev-2.4.4/simplyblock_core/snode_client.py
+-rw-r--r--  2.0 unx     8189 b- defN 24-Apr-29 15:05 sbcli_dev-2.4.4/simplyblock_core/kv_store.py
+-rw-r--r--  2.0 unx     7640 b- defN 24-Apr-29 15:05 sbcli_dev-2.4.4/simplyblock_core/utils.py
+-rw-r--r--  2.0 unx    23423 b- defN 24-Apr-29 15:05 sbcli_dev-2.4.4/simplyblock_core/cluster_ops.py
+-rw-r--r--  2.0 unx     5112 b- defN 24-Apr-29 15:05 sbcli_dev-2.4.4/simplyblock_core/compute_node_ops.py
+-rw-r--r--  2.0 unx    21493 b- defN 24-Apr-29 15:05 sbcli_dev-2.4.4/simplyblock_core/rpc_client.py
+-rw-r--r--  2.0 unx     7479 b- defN 24-Apr-29 15:05 sbcli_dev-2.4.4/simplyblock_core/distr_controller.py
+-rw-r--r--  2.0 unx     2189 b- defN 24-Apr-29 15:05 sbcli_dev-2.4.4/simplyblock_core/services/lvol_monitor.py
+-rw-r--r--  2.0 unx     3203 b- defN 24-Apr-29 15:05 sbcli_dev-2.4.4/simplyblock_core/services/caching_node_monitor.py
+-rw-r--r--  2.0 unx     5462 b- defN 24-Apr-29 15:05 sbcli_dev-2.4.4/simplyblock_core/services/health_check_service.py
+-rw-r--r--  2.0 unx      229 b- defN 24-Apr-29 15:05 sbcli_dev-2.4.4/simplyblock_core/services/service_template.service
+-rw-r--r--  2.0 unx     5268 b- defN 24-Apr-29 15:05 sbcli_dev-2.4.4/simplyblock_core/services/lvol_stat_collector.py
+-rw-r--r--  2.0 unx      173 b- defN 24-Apr-29 15:05 sbcli_dev-2.4.4/simplyblock_core/services/remove_service.sh
+-rw-r--r--  2.0 unx     2410 b- defN 24-Apr-29 15:05 sbcli_dev-2.4.4/simplyblock_core/services/log_agg_service.py
+-rw-r--r--  2.0 unx     5140 b- defN 24-Apr-29 15:05 sbcli_dev-2.4.4/simplyblock_core/services/distr_event_collector.py
+-rw-r--r--  2.0 unx     7439 b- defN 24-Apr-29 15:05 sbcli_dev-2.4.4/simplyblock_core/services/capacity_and_stats_collector.py
+-rw-r--r--  2.0 unx     2423 b- defN 24-Apr-29 15:05 sbcli_dev-2.4.4/simplyblock_core/services/port_stat_collector.py
+-rw-r--r--  2.0 unx     2499 b- defN 24-Apr-29 15:05 sbcli_dev-2.4.4/simplyblock_core/services/device_monitor.py
+-rw-r--r--  2.0 unx     4118 b- defN 24-Apr-29 15:05 sbcli_dev-2.4.4/simplyblock_core/services/__init__.py
+-rw-r--r--  2.0 unx      837 b- defN 24-Apr-29 15:05 sbcli_dev-2.4.4/simplyblock_core/services/install_service.sh
+-rw-r--r--  2.0 unx     3003 b- defN 24-Apr-29 15:05 sbcli_dev-2.4.4/simplyblock_core/services/mgmt_node_monitor.py
+-rw-r--r--  2.0 unx     2671 b- defN 24-Apr-29 15:05 sbcli_dev-2.4.4/simplyblock_core/services/cap_monitor.py
+-rw-r--r--  2.0 unx     6577 b- defN 24-Apr-29 15:05 sbcli_dev-2.4.4/simplyblock_core/services/storage_node_monitor.py
+drwxr-xr-x  2.0 unx        0 b- stor 24-Apr-29 15:05 sbcli_dev-2.4.4/simplyblock_core/scripts/alerting/
+drwxr-xr-x  2.0 unx        0 b- stor 24-Apr-29 15:05 sbcli_dev-2.4.4/simplyblock_core/scripts/dashboards/
+-rw-r--r--  2.0 unx      930 b- defN 24-Apr-29 15:05 sbcli_dev-2.4.4/simplyblock_core/scripts/deploy_stack.sh
+-rw-r--r--  2.0 unx      152 b- defN 24-Apr-29 15:05 sbcli_dev-2.4.4/simplyblock_core/scripts/set_db_config.sh
+-rw-r--r--  2.0 unx     1163 b- defN 24-Apr-29 15:05 sbcli_dev-2.4.4/simplyblock_core/scripts/haproxy.cfg
+-rw-r--r--  2.0 unx     4977 b- defN 24-Apr-29 15:05 sbcli_dev-2.4.4/simplyblock_core/scripts/docker-compose-swarm.yml
+-rw-r--r--  2.0 unx       54 b- defN 24-Apr-29 15:05 sbcli_dev-2.4.4/simplyblock_core/scripts/db_config_single.sh
+-rw-r--r--  2.0 unx     5305 b- defN 24-Apr-29 15:05 sbcli_dev-2.4.4/simplyblock_core/scripts/stack_deploy_wait.sh
+-rw-r--r--  2.0 unx     4470 b- defN 24-Apr-29 15:05 sbcli_dev-2.4.4/simplyblock_core/scripts/docker-compose-swarm-monitoring.yml
+-rw-r--r--  2.0 unx      453 b- defN 24-Apr-29 15:05 sbcli_dev-2.4.4/simplyblock_core/scripts/config_docker.sh
+-rw-r--r--  2.0 unx     1782 b- defN 24-Apr-29 15:05 sbcli_dev-2.4.4/simplyblock_core/scripts/__init__.py
+-rw-r--r--  2.0 unx      311 b- defN 24-Apr-29 15:05 sbcli_dev-2.4.4/simplyblock_core/scripts/clean_local_storage_deploy.sh
+-rw-r--r--  2.0 unx      118 b- defN 24-Apr-29 15:05 sbcli_dev-2.4.4/simplyblock_core/scripts/db_config_double.sh
+-rw-r--r--  2.0 unx      360 b- defN 24-Apr-29 15:05 sbcli_dev-2.4.4/simplyblock_core/scripts/datasource.yml
+-rw-r--r--  2.0 unx       43 b- defN 24-Apr-29 15:05 sbcli_dev-2.4.4/simplyblock_core/scripts/run_ssh.sh
+-rw-r--r--  2.0 unx     1420 b- defN 24-Apr-29 15:05 sbcli_dev-2.4.4/simplyblock_core/scripts/install_deps.sh
+-rw-r--r--  2.0 unx      311 b- defN 24-Apr-29 15:05 sbcli_dev-2.4.4/simplyblock_core/scripts/prometheus.yml
+-rwxr-xr-x  2.0 unx      657 b- defN 24-Apr-29 15:05 sbcli_dev-2.4.4/simplyblock_core/scripts/apply_dashboard.sh
+-rw-r--r--  2.0 unx    25433 b- defN 24-Apr-29 15:05 sbcli_dev-2.4.4/simplyblock_core/scripts/alerting/alert_rules.yaml
+-rw-r--r--  2.0 unx     1856 b- defN 24-Apr-29 15:05 sbcli_dev-2.4.4/simplyblock_core/scripts/alerting/alert_resources.yaml
+-rw-r--r--  2.0 unx   106705 b- defN 24-Apr-29 15:05 sbcli_dev-2.4.4/simplyblock_core/scripts/dashboards/devices.json
+-rw-r--r--  2.0 unx   799409 b- defN 24-Apr-29 15:05 sbcli_dev-2.4.4/simplyblock_core/scripts/dashboards/node-exporter.json
+-rw-r--r--  2.0 unx    99758 b- defN 24-Apr-29 15:05 sbcli_dev-2.4.4/simplyblock_core/scripts/dashboards/nodes.json
+-rw-r--r--  2.0 unx    99707 b- defN 24-Apr-29 15:05 sbcli_dev-2.4.4/simplyblock_core/scripts/dashboards/lvols.json
+-rw-r--r--  2.0 unx    99862 b- defN 24-Apr-29 15:05 sbcli_dev-2.4.4/simplyblock_core/scripts/dashboards/cluster.json
+-rw-r--r--  2.0 unx    99707 b- defN 24-Apr-29 15:05 sbcli_dev-2.4.4/simplyblock_core/scripts/dashboards/pools.json
+-rw-r--r--  2.0 unx    13877 b- defN 24-Apr-29 15:05 sbcli_dev-2.4.4/simplyblock_core/controllers/device_controller.py
+-rw-r--r--  2.0 unx     1120 b- defN 24-Apr-29 15:05 sbcli_dev-2.4.4/simplyblock_core/controllers/mgmt_events.py
+-rw-r--r--  2.0 unx     3191 b- defN 24-Apr-29 15:05 sbcli_dev-2.4.4/simplyblock_core/controllers/events_controller.py
+-rw-r--r--  2.0 unx     1521 b- defN 24-Apr-29 15:05 sbcli_dev-2.4.4/simplyblock_core/controllers/storage_events.py
+-rw-r--r--  2.0 unx     1630 b- defN 24-Apr-29 15:05 sbcli_dev-2.4.4/simplyblock_core/controllers/lvol_events.py
+-rw-r--r--  2.0 unx    10557 b- defN 24-Apr-29 15:05 sbcli_dev-2.4.4/simplyblock_core/controllers/snapshot_controller.py
+-rw-r--r--  2.0 unx     1568 b- defN 24-Apr-29 15:05 sbcli_dev-2.4.4/simplyblock_core/controllers/device_events.py
+-rw-r--r--  2.0 unx    10375 b- defN 24-Apr-29 15:05 sbcli_dev-2.4.4/simplyblock_core/controllers/pool_controller.py
+-rw-r--r--  2.0 unx        0 b- defN 24-Apr-29 15:05 sbcli_dev-2.4.4/simplyblock_core/controllers/__init__.py
+-rw-r--r--  2.0 unx     1900 b- defN 24-Apr-29 15:05 sbcli_dev-2.4.4/simplyblock_core/controllers/cluster_events.py
+-rw-r--r--  2.0 unx    22847 b- defN 24-Apr-29 15:05 sbcli_dev-2.4.4/simplyblock_core/controllers/caching_node_controller.py
+-rw-r--r--  2.0 unx     1122 b- defN 24-Apr-29 15:05 sbcli_dev-2.4.4/simplyblock_core/controllers/snapshot_events.py
+-rw-r--r--  2.0 unx    47339 b- defN 24-Apr-29 15:05 sbcli_dev-2.4.4/simplyblock_core/controllers/lvol_controller.py
+-rw-r--r--  2.0 unx    11294 b- defN 24-Apr-29 15:05 sbcli_dev-2.4.4/simplyblock_core/controllers/health_controller.py
+-rw-r--r--  2.0 unx      695 b- defN 24-Apr-29 15:05 sbcli_dev-2.4.4/simplyblock_core/controllers/pool_events.py
+-rw-r--r--  2.0 unx     1500 b- defN 24-Apr-29 15:05 sbcli_dev-2.4.4/simplyblock_core/models/events.py
+-rw-r--r--  2.0 unx      806 b- defN 24-Apr-29 15:05 sbcli_dev-2.4.4/simplyblock_core/models/iface.py
+-rw-r--r--  2.0 unx     4846 b- defN 24-Apr-29 15:05 sbcli_dev-2.4.4/simplyblock_core/models/base_model.py
+-rw-r--r--  2.0 unx     2579 b- defN 24-Apr-29 15:05 sbcli_dev-2.4.4/simplyblock_core/models/lvol_model.py
+-rw-r--r--  2.0 unx      917 b- defN 24-Apr-29 15:05 sbcli_dev-2.4.4/simplyblock_core/models/compute_node.py
+-rw-r--r--  2.0 unx      736 b- defN 24-Apr-29 15:05 sbcli_dev-2.4.4/simplyblock_core/models/snapshot.py
+-rw-r--r--  2.0 unx     1602 b- defN 24-Apr-29 15:05 sbcli_dev-2.4.4/simplyblock_core/models/pool.py
+-rw-r--r--  2.0 unx     1228 b- defN 24-Apr-29 15:05 sbcli_dev-2.4.4/simplyblock_core/models/global_settings.py
+-rw-r--r--  2.0 unx     1020 b- defN 24-Apr-29 15:05 sbcli_dev-2.4.4/simplyblock_core/models/port_stat.py
+-rw-r--r--  2.0 unx     3696 b- defN 24-Apr-29 15:05 sbcli_dev-2.4.4/simplyblock_core/models/storage_node.py
+-rw-r--r--  2.0 unx        0 b- defN 24-Apr-29 15:05 sbcli_dev-2.4.4/simplyblock_core/models/__init__.py
+-rw-r--r--  2.0 unx     4242 b- defN 24-Apr-29 15:05 sbcli_dev-2.4.4/simplyblock_core/models/stats.py
+-rw-r--r--  2.0 unx     2565 b- defN 24-Apr-29 15:05 sbcli_dev-2.4.4/simplyblock_core/models/cluster.py
+-rw-r--r--  2.0 unx     1466 b- defN 24-Apr-29 15:05 sbcli_dev-2.4.4/simplyblock_core/models/mgmt_node.py
+-rw-r--r--  2.0 unx     3766 b- defN 24-Apr-29 15:05 sbcli_dev-2.4.4/simplyblock_core/models/caching_node.py
+-rw-r--r--  2.0 unx     2071 b- defN 24-Apr-29 15:05 sbcli_dev-2.4.4/simplyblock_core/models/nvme_device.py
+drwxr-xr-x  2.0 unx        0 b- stor 24-Apr-29 15:05 sbcli_dev-2.4.4/simplyblock_web/static/
+drwxr-xr-x  2.0 unx        0 b- stor 24-Apr-29 15:05 sbcli_dev-2.4.4/simplyblock_web/templates/
+drwxr-xr-x  2.0 unx        0 b- stor 24-Apr-29 15:05 sbcli_dev-2.4.4/simplyblock_web/blueprints/
+-rw-r--r--  2.0 unx      725 b- defN 24-Apr-29 15:05 sbcli_dev-2.4.4/simplyblock_web/caching_node_app_k8s.py
+-rw-r--r--  2.0 unx     5098 b- defN 24-Apr-29 15:05 sbcli_dev-2.4.4/simplyblock_web/node_utils.py
+-rw-r--r--  2.0 unx      703 b- defN 24-Apr-29 15:05 sbcli_dev-2.4.4/simplyblock_web/snode_app.py
+-rw-r--r--  2.0 unx     1263 b- defN 24-Apr-29 15:05 sbcli_dev-2.4.4/simplyblock_web/app.py
+-rw-r--r--  2.0 unx     1638 b- defN 24-Apr-29 15:05 sbcli_dev-2.4.4/simplyblock_web/auth_middleware.py
+-rw-r--r--  2.0 unx        0 b- defN 24-Apr-29 15:05 sbcli_dev-2.4.4/simplyblock_web/__init__.py
+-rw-r--r--  2.0 unx      717 b- defN 24-Apr-29 15:05 sbcli_dev-2.4.4/simplyblock_web/caching_node_app.py
+-rw-r--r--  2.0 unx     2513 b- defN 24-Apr-29 15:05 sbcli_dev-2.4.4/simplyblock_web/utils.py
+-rw-r--r--  2.0 unx     1434 b- defN 24-Apr-29 15:05 sbcli_dev-2.4.4/simplyblock_web/node_webapp.py
+-rw-r--r--  2.0 unx      507 b- defN 24-Apr-29 15:05 sbcli_dev-2.4.4/simplyblock_web/static/deploy_cnode.yaml
+-rw-r--r--  2.0 unx      322 b- defN 24-Apr-29 15:05 sbcli_dev-2.4.4/simplyblock_web/static/tst.py
+-rw-r--r--  2.0 unx      434 b- defN 24-Apr-29 15:05 sbcli_dev-2.4.4/simplyblock_web/static/is_up.py
+-rw-r--r--  2.0 unx      827 b- defN 24-Apr-29 15:05 sbcli_dev-2.4.4/simplyblock_web/static/delete.py
+-rw-r--r--  2.0 unx     1302 b- defN 24-Apr-29 15:05 sbcli_dev-2.4.4/simplyblock_web/static/deploy.py
+-rw-r--r--  2.0 unx     1466 b- defN 24-Apr-29 15:05 sbcli_dev-2.4.4/simplyblock_web/static/deploy_spdk.yaml
+-rw-r--r--  2.0 unx      463 b- defN 24-Apr-29 15:05 sbcli_dev-2.4.4/simplyblock_web/static/rpac.yaml
+-rw-r--r--  2.0 unx      417 b- defN 24-Apr-29 15:05 sbcli_dev-2.4.4/simplyblock_web/static/list_deps.py
+-rw-r--r--  2.0 unx     2876 b- defN 24-Apr-29 15:05 sbcli_dev-2.4.4/simplyblock_web/templates/deploy_spdk.yaml.j2
+-rw-r--r--  2.0 unx     5547 b- defN 24-Apr-29 15:05 sbcli_dev-2.4.4/simplyblock_web/blueprints/node_api_caching_docker.py
+-rw-r--r--  2.0 unx     4795 b- defN 24-Apr-29 15:05 sbcli_dev-2.4.4/simplyblock_web/blueprints/node_api_caching_ks.py
+-rw-r--r--  2.0 unx     5317 b- defN 24-Apr-29 15:05 sbcli_dev-2.4.4/simplyblock_web/blueprints/web_api_caching_node.py
+-rw-r--r--  2.0 unx     9573 b- defN 24-Apr-29 15:05 sbcli_dev-2.4.4/simplyblock_web/blueprints/snode_ops.py
+-rw-r--r--  2.0 unx     8547 b- defN 24-Apr-29 15:05 sbcli_dev-2.4.4/simplyblock_web/blueprints/web_api_lvol.py
+-rw-r--r--  2.0 unx    11244 b- defN 24-Apr-29 15:05 sbcli_dev-2.4.4/simplyblock_web/blueprints/csi.py
+-rw-r--r--  2.0 unx    12198 b- defN 24-Apr-29 15:05 sbcli_dev-2.4.4/simplyblock_web/blueprints/caching_node_ops.py
+-rw-r--r--  2.0 unx      975 b- defN 24-Apr-29 15:05 sbcli_dev-2.4.4/simplyblock_web/blueprints/web_api_mgmt_node.py
+-rw-r--r--  2.0 unx     6326 b- defN 24-Apr-29 15:05 sbcli_dev-2.4.4/simplyblock_web/blueprints/web_api_storage_node.py
+-rw-r--r--  2.0 unx        0 b- defN 24-Apr-29 15:05 sbcli_dev-2.4.4/simplyblock_web/blueprints/__init__.py
+-rw-r--r--  2.0 unx     7846 b- defN 24-Apr-29 15:05 sbcli_dev-2.4.4/simplyblock_web/blueprints/caching_node_ops_k8s.py
+-rw-r--r--  2.0 unx     2940 b- defN 24-Apr-29 15:05 sbcli_dev-2.4.4/simplyblock_web/blueprints/web_api_device.py
+-rw-r--r--  2.0 unx     5274 b- defN 24-Apr-29 15:05 sbcli_dev-2.4.4/simplyblock_web/blueprints/web_api_cluster.py
+-rw-r--r--  2.0 unx     3103 b- defN 24-Apr-29 15:05 sbcli_dev-2.4.4/simplyblock_web/blueprints/node_api_basic.py
+-rw-r--r--  2.0 unx     6206 b- defN 24-Apr-29 15:05 sbcli_dev-2.4.4/simplyblock_web/blueprints/web_api_pool.py
+146 files, 1925125 bytes uncompressed, 186790 bytes compressed:  90.3%
```

## zipnote {}

```diff
@@ -1,439 +1,439 @@
-Filename: sbcli_dev-2.4.3/
+Filename: sbcli_dev-2.4.4/
 Comment: 
 
-Filename: sbcli_dev-2.4.3/simplyblock_cli/
+Filename: sbcli_dev-2.4.4/simplyblock_cli/
 Comment: 
 
-Filename: sbcli_dev-2.4.3/sbcli_dev.egg-info/
+Filename: sbcli_dev-2.4.4/sbcli_dev.egg-info/
 Comment: 
 
-Filename: sbcli_dev-2.4.3/simplyblock_core/
+Filename: sbcli_dev-2.4.4/simplyblock_core/
 Comment: 
 
-Filename: sbcli_dev-2.4.3/simplyblock_web/
+Filename: sbcli_dev-2.4.4/simplyblock_web/
 Comment: 
 
-Filename: sbcli_dev-2.4.3/setup.py
+Filename: sbcli_dev-2.4.4/setup.py
 Comment: 
 
-Filename: sbcli_dev-2.4.3/README.md
+Filename: sbcli_dev-2.4.4/README.md
 Comment: 
 
-Filename: sbcli_dev-2.4.3/env_var
+Filename: sbcli_dev-2.4.4/env_var
 Comment: 
 
-Filename: sbcli_dev-2.4.3/pyproject.toml
+Filename: sbcli_dev-2.4.4/pyproject.toml
 Comment: 
 
-Filename: sbcli_dev-2.4.3/setup.cfg
+Filename: sbcli_dev-2.4.4/setup.cfg
 Comment: 
 
-Filename: sbcli_dev-2.4.3/PKG-INFO
+Filename: sbcli_dev-2.4.4/PKG-INFO
 Comment: 
 
-Filename: sbcli_dev-2.4.3/simplyblock_cli/cli.py
+Filename: sbcli_dev-2.4.4/simplyblock_cli/cli.py
 Comment: 
 
-Filename: sbcli_dev-2.4.3/simplyblock_cli/main.py
+Filename: sbcli_dev-2.4.4/simplyblock_cli/main.py
 Comment: 
 
-Filename: sbcli_dev-2.4.3/sbcli_dev.egg-info/dependency_links.txt
+Filename: sbcli_dev-2.4.4/sbcli_dev.egg-info/dependency_links.txt
 Comment: 
 
-Filename: sbcli_dev-2.4.3/sbcli_dev.egg-info/SOURCES.txt
+Filename: sbcli_dev-2.4.4/sbcli_dev.egg-info/SOURCES.txt
 Comment: 
 
-Filename: sbcli_dev-2.4.3/sbcli_dev.egg-info/top_level.txt
+Filename: sbcli_dev-2.4.4/sbcli_dev.egg-info/top_level.txt
 Comment: 
 
-Filename: sbcli_dev-2.4.3/sbcli_dev.egg-info/PKG-INFO
+Filename: sbcli_dev-2.4.4/sbcli_dev.egg-info/PKG-INFO
 Comment: 
 
-Filename: sbcli_dev-2.4.3/sbcli_dev.egg-info/requires.txt
+Filename: sbcli_dev-2.4.4/sbcli_dev.egg-info/requires.txt
 Comment: 
 
-Filename: sbcli_dev-2.4.3/sbcli_dev.egg-info/entry_points.txt
+Filename: sbcli_dev-2.4.4/sbcli_dev.egg-info/entry_points.txt
 Comment: 
 
-Filename: sbcli_dev-2.4.3/simplyblock_core/services/
+Filename: sbcli_dev-2.4.4/simplyblock_core/services/
 Comment: 
 
-Filename: sbcli_dev-2.4.3/simplyblock_core/scripts/
+Filename: sbcli_dev-2.4.4/simplyblock_core/scripts/
 Comment: 
 
-Filename: sbcli_dev-2.4.3/simplyblock_core/controllers/
+Filename: sbcli_dev-2.4.4/simplyblock_core/controllers/
 Comment: 
 
-Filename: sbcli_dev-2.4.3/simplyblock_core/models/
+Filename: sbcli_dev-2.4.4/simplyblock_core/models/
 Comment: 
 
-Filename: sbcli_dev-2.4.3/simplyblock_core/storage_node_ops.py
+Filename: sbcli_dev-2.4.4/simplyblock_core/storage_node_ops.py
 Comment: 
 
-Filename: sbcli_dev-2.4.3/simplyblock_core/constants.py
+Filename: sbcli_dev-2.4.4/simplyblock_core/constants.py
 Comment: 
 
-Filename: sbcli_dev-2.4.3/simplyblock_core/mgmt_node_ops.py
+Filename: sbcli_dev-2.4.4/simplyblock_core/mgmt_node_ops.py
 Comment: 
 
-Filename: sbcli_dev-2.4.3/simplyblock_core/cnode_client.py
+Filename: sbcli_dev-2.4.4/simplyblock_core/cnode_client.py
 Comment: 
 
-Filename: sbcli_dev-2.4.3/simplyblock_core/shell_utils.py
+Filename: sbcli_dev-2.4.4/simplyblock_core/shell_utils.py
 Comment: 
 
-Filename: sbcli_dev-2.4.3/simplyblock_core/pci_utils.py
+Filename: sbcli_dev-2.4.4/simplyblock_core/pci_utils.py
 Comment: 
 
-Filename: sbcli_dev-2.4.3/simplyblock_core/__init__.py
+Filename: sbcli_dev-2.4.4/simplyblock_core/__init__.py
 Comment: 
 
-Filename: sbcli_dev-2.4.3/simplyblock_core/snode_client.py
+Filename: sbcli_dev-2.4.4/simplyblock_core/snode_client.py
 Comment: 
 
-Filename: sbcli_dev-2.4.3/simplyblock_core/kv_store.py
+Filename: sbcli_dev-2.4.4/simplyblock_core/kv_store.py
 Comment: 
 
-Filename: sbcli_dev-2.4.3/simplyblock_core/utils.py
+Filename: sbcli_dev-2.4.4/simplyblock_core/utils.py
 Comment: 
 
-Filename: sbcli_dev-2.4.3/simplyblock_core/cluster_ops.py
+Filename: sbcli_dev-2.4.4/simplyblock_core/cluster_ops.py
 Comment: 
 
-Filename: sbcli_dev-2.4.3/simplyblock_core/compute_node_ops.py
+Filename: sbcli_dev-2.4.4/simplyblock_core/compute_node_ops.py
 Comment: 
 
-Filename: sbcli_dev-2.4.3/simplyblock_core/rpc_client.py
+Filename: sbcli_dev-2.4.4/simplyblock_core/rpc_client.py
 Comment: 
 
-Filename: sbcli_dev-2.4.3/simplyblock_core/distr_controller.py
+Filename: sbcli_dev-2.4.4/simplyblock_core/distr_controller.py
 Comment: 
 
-Filename: sbcli_dev-2.4.3/simplyblock_core/services/lvol_monitor.py
+Filename: sbcli_dev-2.4.4/simplyblock_core/services/lvol_monitor.py
 Comment: 
 
-Filename: sbcli_dev-2.4.3/simplyblock_core/services/caching_node_monitor.py
+Filename: sbcli_dev-2.4.4/simplyblock_core/services/caching_node_monitor.py
 Comment: 
 
-Filename: sbcli_dev-2.4.3/simplyblock_core/services/health_check_service.py
+Filename: sbcli_dev-2.4.4/simplyblock_core/services/health_check_service.py
 Comment: 
 
-Filename: sbcli_dev-2.4.3/simplyblock_core/services/service_template.service
+Filename: sbcli_dev-2.4.4/simplyblock_core/services/service_template.service
 Comment: 
 
-Filename: sbcli_dev-2.4.3/simplyblock_core/services/lvol_stat_collector.py
+Filename: sbcli_dev-2.4.4/simplyblock_core/services/lvol_stat_collector.py
 Comment: 
 
-Filename: sbcli_dev-2.4.3/simplyblock_core/services/remove_service.sh
+Filename: sbcli_dev-2.4.4/simplyblock_core/services/remove_service.sh
 Comment: 
 
-Filename: sbcli_dev-2.4.3/simplyblock_core/services/log_agg_service.py
+Filename: sbcli_dev-2.4.4/simplyblock_core/services/log_agg_service.py
 Comment: 
 
-Filename: sbcli_dev-2.4.3/simplyblock_core/services/distr_event_collector.py
+Filename: sbcli_dev-2.4.4/simplyblock_core/services/distr_event_collector.py
 Comment: 
 
-Filename: sbcli_dev-2.4.3/simplyblock_core/services/capacity_and_stats_collector.py
+Filename: sbcli_dev-2.4.4/simplyblock_core/services/capacity_and_stats_collector.py
 Comment: 
 
-Filename: sbcli_dev-2.4.3/simplyblock_core/services/port_stat_collector.py
+Filename: sbcli_dev-2.4.4/simplyblock_core/services/port_stat_collector.py
 Comment: 
 
-Filename: sbcli_dev-2.4.3/simplyblock_core/services/device_monitor.py
+Filename: sbcli_dev-2.4.4/simplyblock_core/services/device_monitor.py
 Comment: 
 
-Filename: sbcli_dev-2.4.3/simplyblock_core/services/__init__.py
+Filename: sbcli_dev-2.4.4/simplyblock_core/services/__init__.py
 Comment: 
 
-Filename: sbcli_dev-2.4.3/simplyblock_core/services/install_service.sh
+Filename: sbcli_dev-2.4.4/simplyblock_core/services/install_service.sh
 Comment: 
 
-Filename: sbcli_dev-2.4.3/simplyblock_core/services/mgmt_node_monitor.py
+Filename: sbcli_dev-2.4.4/simplyblock_core/services/mgmt_node_monitor.py
 Comment: 
 
-Filename: sbcli_dev-2.4.3/simplyblock_core/services/cap_monitor.py
+Filename: sbcli_dev-2.4.4/simplyblock_core/services/cap_monitor.py
 Comment: 
 
-Filename: sbcli_dev-2.4.3/simplyblock_core/services/storage_node_monitor.py
+Filename: sbcli_dev-2.4.4/simplyblock_core/services/storage_node_monitor.py
 Comment: 
 
-Filename: sbcli_dev-2.4.3/simplyblock_core/scripts/alerting/
+Filename: sbcli_dev-2.4.4/simplyblock_core/scripts/alerting/
 Comment: 
 
-Filename: sbcli_dev-2.4.3/simplyblock_core/scripts/dashboards/
+Filename: sbcli_dev-2.4.4/simplyblock_core/scripts/dashboards/
 Comment: 
 
-Filename: sbcli_dev-2.4.3/simplyblock_core/scripts/deploy_stack.sh
+Filename: sbcli_dev-2.4.4/simplyblock_core/scripts/deploy_stack.sh
 Comment: 
 
-Filename: sbcli_dev-2.4.3/simplyblock_core/scripts/set_db_config.sh
+Filename: sbcli_dev-2.4.4/simplyblock_core/scripts/set_db_config.sh
 Comment: 
 
-Filename: sbcli_dev-2.4.3/simplyblock_core/scripts/haproxy.cfg
+Filename: sbcli_dev-2.4.4/simplyblock_core/scripts/haproxy.cfg
 Comment: 
 
-Filename: sbcli_dev-2.4.3/simplyblock_core/scripts/docker-compose-swarm.yml
+Filename: sbcli_dev-2.4.4/simplyblock_core/scripts/docker-compose-swarm.yml
 Comment: 
 
-Filename: sbcli_dev-2.4.3/simplyblock_core/scripts/db_config_single.sh
+Filename: sbcli_dev-2.4.4/simplyblock_core/scripts/db_config_single.sh
 Comment: 
 
-Filename: sbcli_dev-2.4.3/simplyblock_core/scripts/stack_deploy_wait.sh
+Filename: sbcli_dev-2.4.4/simplyblock_core/scripts/stack_deploy_wait.sh
 Comment: 
 
-Filename: sbcli_dev-2.4.3/simplyblock_core/scripts/docker-compose-swarm-monitoring.yml
+Filename: sbcli_dev-2.4.4/simplyblock_core/scripts/docker-compose-swarm-monitoring.yml
 Comment: 
 
-Filename: sbcli_dev-2.4.3/simplyblock_core/scripts/config_docker.sh
+Filename: sbcli_dev-2.4.4/simplyblock_core/scripts/config_docker.sh
 Comment: 
 
-Filename: sbcli_dev-2.4.3/simplyblock_core/scripts/__init__.py
+Filename: sbcli_dev-2.4.4/simplyblock_core/scripts/__init__.py
 Comment: 
 
-Filename: sbcli_dev-2.4.3/simplyblock_core/scripts/clean_local_storage_deploy.sh
+Filename: sbcli_dev-2.4.4/simplyblock_core/scripts/clean_local_storage_deploy.sh
 Comment: 
 
-Filename: sbcli_dev-2.4.3/simplyblock_core/scripts/db_config_double.sh
+Filename: sbcli_dev-2.4.4/simplyblock_core/scripts/db_config_double.sh
 Comment: 
 
-Filename: sbcli_dev-2.4.3/simplyblock_core/scripts/datasource.yml
+Filename: sbcli_dev-2.4.4/simplyblock_core/scripts/datasource.yml
 Comment: 
 
-Filename: sbcli_dev-2.4.3/simplyblock_core/scripts/run_ssh.sh
+Filename: sbcli_dev-2.4.4/simplyblock_core/scripts/run_ssh.sh
 Comment: 
 
-Filename: sbcli_dev-2.4.3/simplyblock_core/scripts/install_deps.sh
+Filename: sbcli_dev-2.4.4/simplyblock_core/scripts/install_deps.sh
 Comment: 
 
-Filename: sbcli_dev-2.4.3/simplyblock_core/scripts/prometheus.yml
+Filename: sbcli_dev-2.4.4/simplyblock_core/scripts/prometheus.yml
 Comment: 
 
-Filename: sbcli_dev-2.4.3/simplyblock_core/scripts/apply_dashboard.sh
+Filename: sbcli_dev-2.4.4/simplyblock_core/scripts/apply_dashboard.sh
 Comment: 
 
-Filename: sbcli_dev-2.4.3/simplyblock_core/scripts/alerting/alert_rules.yaml
+Filename: sbcli_dev-2.4.4/simplyblock_core/scripts/alerting/alert_rules.yaml
 Comment: 
 
-Filename: sbcli_dev-2.4.3/simplyblock_core/scripts/alerting/alert_resources.yaml
+Filename: sbcli_dev-2.4.4/simplyblock_core/scripts/alerting/alert_resources.yaml
 Comment: 
 
-Filename: sbcli_dev-2.4.3/simplyblock_core/scripts/dashboards/devices.json
+Filename: sbcli_dev-2.4.4/simplyblock_core/scripts/dashboards/devices.json
 Comment: 
 
-Filename: sbcli_dev-2.4.3/simplyblock_core/scripts/dashboards/node-exporter.json
+Filename: sbcli_dev-2.4.4/simplyblock_core/scripts/dashboards/node-exporter.json
 Comment: 
 
-Filename: sbcli_dev-2.4.3/simplyblock_core/scripts/dashboards/nodes.json
+Filename: sbcli_dev-2.4.4/simplyblock_core/scripts/dashboards/nodes.json
 Comment: 
 
-Filename: sbcli_dev-2.4.3/simplyblock_core/scripts/dashboards/lvols.json
+Filename: sbcli_dev-2.4.4/simplyblock_core/scripts/dashboards/lvols.json
 Comment: 
 
-Filename: sbcli_dev-2.4.3/simplyblock_core/scripts/dashboards/cluster.json
+Filename: sbcli_dev-2.4.4/simplyblock_core/scripts/dashboards/cluster.json
 Comment: 
 
-Filename: sbcli_dev-2.4.3/simplyblock_core/scripts/dashboards/pools.json
+Filename: sbcli_dev-2.4.4/simplyblock_core/scripts/dashboards/pools.json
 Comment: 
 
-Filename: sbcli_dev-2.4.3/simplyblock_core/controllers/device_controller.py
+Filename: sbcli_dev-2.4.4/simplyblock_core/controllers/device_controller.py
 Comment: 
 
-Filename: sbcli_dev-2.4.3/simplyblock_core/controllers/mgmt_events.py
+Filename: sbcli_dev-2.4.4/simplyblock_core/controllers/mgmt_events.py
 Comment: 
 
-Filename: sbcli_dev-2.4.3/simplyblock_core/controllers/events_controller.py
+Filename: sbcli_dev-2.4.4/simplyblock_core/controllers/events_controller.py
 Comment: 
 
-Filename: sbcli_dev-2.4.3/simplyblock_core/controllers/storage_events.py
+Filename: sbcli_dev-2.4.4/simplyblock_core/controllers/storage_events.py
 Comment: 
 
-Filename: sbcli_dev-2.4.3/simplyblock_core/controllers/lvol_events.py
+Filename: sbcli_dev-2.4.4/simplyblock_core/controllers/lvol_events.py
 Comment: 
 
-Filename: sbcli_dev-2.4.3/simplyblock_core/controllers/snapshot_controller.py
+Filename: sbcli_dev-2.4.4/simplyblock_core/controllers/snapshot_controller.py
 Comment: 
 
-Filename: sbcli_dev-2.4.3/simplyblock_core/controllers/device_events.py
+Filename: sbcli_dev-2.4.4/simplyblock_core/controllers/device_events.py
 Comment: 
 
-Filename: sbcli_dev-2.4.3/simplyblock_core/controllers/pool_controller.py
+Filename: sbcli_dev-2.4.4/simplyblock_core/controllers/pool_controller.py
 Comment: 
 
-Filename: sbcli_dev-2.4.3/simplyblock_core/controllers/__init__.py
+Filename: sbcli_dev-2.4.4/simplyblock_core/controllers/__init__.py
 Comment: 
 
-Filename: sbcli_dev-2.4.3/simplyblock_core/controllers/cluster_events.py
+Filename: sbcli_dev-2.4.4/simplyblock_core/controllers/cluster_events.py
 Comment: 
 
-Filename: sbcli_dev-2.4.3/simplyblock_core/controllers/caching_node_controller.py
+Filename: sbcli_dev-2.4.4/simplyblock_core/controllers/caching_node_controller.py
 Comment: 
 
-Filename: sbcli_dev-2.4.3/simplyblock_core/controllers/snapshot_events.py
+Filename: sbcli_dev-2.4.4/simplyblock_core/controllers/snapshot_events.py
 Comment: 
 
-Filename: sbcli_dev-2.4.3/simplyblock_core/controllers/lvol_controller.py
+Filename: sbcli_dev-2.4.4/simplyblock_core/controllers/lvol_controller.py
 Comment: 
 
-Filename: sbcli_dev-2.4.3/simplyblock_core/controllers/health_controller.py
+Filename: sbcli_dev-2.4.4/simplyblock_core/controllers/health_controller.py
 Comment: 
 
-Filename: sbcli_dev-2.4.3/simplyblock_core/controllers/pool_events.py
+Filename: sbcli_dev-2.4.4/simplyblock_core/controllers/pool_events.py
 Comment: 
 
-Filename: sbcli_dev-2.4.3/simplyblock_core/models/events.py
+Filename: sbcli_dev-2.4.4/simplyblock_core/models/events.py
 Comment: 
 
-Filename: sbcli_dev-2.4.3/simplyblock_core/models/iface.py
+Filename: sbcli_dev-2.4.4/simplyblock_core/models/iface.py
 Comment: 
 
-Filename: sbcli_dev-2.4.3/simplyblock_core/models/base_model.py
+Filename: sbcli_dev-2.4.4/simplyblock_core/models/base_model.py
 Comment: 
 
-Filename: sbcli_dev-2.4.3/simplyblock_core/models/lvol_model.py
+Filename: sbcli_dev-2.4.4/simplyblock_core/models/lvol_model.py
 Comment: 
 
-Filename: sbcli_dev-2.4.3/simplyblock_core/models/compute_node.py
+Filename: sbcli_dev-2.4.4/simplyblock_core/models/compute_node.py
 Comment: 
 
-Filename: sbcli_dev-2.4.3/simplyblock_core/models/snapshot.py
+Filename: sbcli_dev-2.4.4/simplyblock_core/models/snapshot.py
 Comment: 
 
-Filename: sbcli_dev-2.4.3/simplyblock_core/models/pool.py
+Filename: sbcli_dev-2.4.4/simplyblock_core/models/pool.py
 Comment: 
 
-Filename: sbcli_dev-2.4.3/simplyblock_core/models/global_settings.py
+Filename: sbcli_dev-2.4.4/simplyblock_core/models/global_settings.py
 Comment: 
 
-Filename: sbcli_dev-2.4.3/simplyblock_core/models/port_stat.py
+Filename: sbcli_dev-2.4.4/simplyblock_core/models/port_stat.py
 Comment: 
 
-Filename: sbcli_dev-2.4.3/simplyblock_core/models/storage_node.py
+Filename: sbcli_dev-2.4.4/simplyblock_core/models/storage_node.py
 Comment: 
 
-Filename: sbcli_dev-2.4.3/simplyblock_core/models/__init__.py
+Filename: sbcli_dev-2.4.4/simplyblock_core/models/__init__.py
 Comment: 
 
-Filename: sbcli_dev-2.4.3/simplyblock_core/models/stats.py
+Filename: sbcli_dev-2.4.4/simplyblock_core/models/stats.py
 Comment: 
 
-Filename: sbcli_dev-2.4.3/simplyblock_core/models/cluster.py
+Filename: sbcli_dev-2.4.4/simplyblock_core/models/cluster.py
 Comment: 
 
-Filename: sbcli_dev-2.4.3/simplyblock_core/models/mgmt_node.py
+Filename: sbcli_dev-2.4.4/simplyblock_core/models/mgmt_node.py
 Comment: 
 
-Filename: sbcli_dev-2.4.3/simplyblock_core/models/caching_node.py
+Filename: sbcli_dev-2.4.4/simplyblock_core/models/caching_node.py
 Comment: 
 
-Filename: sbcli_dev-2.4.3/simplyblock_core/models/nvme_device.py
+Filename: sbcli_dev-2.4.4/simplyblock_core/models/nvme_device.py
 Comment: 
 
-Filename: sbcli_dev-2.4.3/simplyblock_web/static/
+Filename: sbcli_dev-2.4.4/simplyblock_web/static/
 Comment: 
 
-Filename: sbcli_dev-2.4.3/simplyblock_web/templates/
+Filename: sbcli_dev-2.4.4/simplyblock_web/templates/
 Comment: 
 
-Filename: sbcli_dev-2.4.3/simplyblock_web/blueprints/
+Filename: sbcli_dev-2.4.4/simplyblock_web/blueprints/
 Comment: 
 
-Filename: sbcli_dev-2.4.3/simplyblock_web/caching_node_app_k8s.py
+Filename: sbcli_dev-2.4.4/simplyblock_web/caching_node_app_k8s.py
 Comment: 
 
-Filename: sbcli_dev-2.4.3/simplyblock_web/node_utils.py
+Filename: sbcli_dev-2.4.4/simplyblock_web/node_utils.py
 Comment: 
 
-Filename: sbcli_dev-2.4.3/simplyblock_web/snode_app.py
+Filename: sbcli_dev-2.4.4/simplyblock_web/snode_app.py
 Comment: 
 
-Filename: sbcli_dev-2.4.3/simplyblock_web/app.py
+Filename: sbcli_dev-2.4.4/simplyblock_web/app.py
 Comment: 
 
-Filename: sbcli_dev-2.4.3/simplyblock_web/auth_middleware.py
+Filename: sbcli_dev-2.4.4/simplyblock_web/auth_middleware.py
 Comment: 
 
-Filename: sbcli_dev-2.4.3/simplyblock_web/__init__.py
+Filename: sbcli_dev-2.4.4/simplyblock_web/__init__.py
 Comment: 
 
-Filename: sbcli_dev-2.4.3/simplyblock_web/caching_node_app.py
+Filename: sbcli_dev-2.4.4/simplyblock_web/caching_node_app.py
 Comment: 
 
-Filename: sbcli_dev-2.4.3/simplyblock_web/utils.py
+Filename: sbcli_dev-2.4.4/simplyblock_web/utils.py
 Comment: 
 
-Filename: sbcli_dev-2.4.3/simplyblock_web/node_webapp.py
+Filename: sbcli_dev-2.4.4/simplyblock_web/node_webapp.py
 Comment: 
 
-Filename: sbcli_dev-2.4.3/simplyblock_web/static/deploy_cnode.yaml
+Filename: sbcli_dev-2.4.4/simplyblock_web/static/deploy_cnode.yaml
 Comment: 
 
-Filename: sbcli_dev-2.4.3/simplyblock_web/static/tst.py
+Filename: sbcli_dev-2.4.4/simplyblock_web/static/tst.py
 Comment: 
 
-Filename: sbcli_dev-2.4.3/simplyblock_web/static/is_up.py
+Filename: sbcli_dev-2.4.4/simplyblock_web/static/is_up.py
 Comment: 
 
-Filename: sbcli_dev-2.4.3/simplyblock_web/static/delete.py
+Filename: sbcli_dev-2.4.4/simplyblock_web/static/delete.py
 Comment: 
 
-Filename: sbcli_dev-2.4.3/simplyblock_web/static/deploy.py
+Filename: sbcli_dev-2.4.4/simplyblock_web/static/deploy.py
 Comment: 
 
-Filename: sbcli_dev-2.4.3/simplyblock_web/static/deploy_spdk.yaml
+Filename: sbcli_dev-2.4.4/simplyblock_web/static/deploy_spdk.yaml
 Comment: 
 
-Filename: sbcli_dev-2.4.3/simplyblock_web/static/rpac.yaml
+Filename: sbcli_dev-2.4.4/simplyblock_web/static/rpac.yaml
 Comment: 
 
-Filename: sbcli_dev-2.4.3/simplyblock_web/static/list_deps.py
+Filename: sbcli_dev-2.4.4/simplyblock_web/static/list_deps.py
 Comment: 
 
-Filename: sbcli_dev-2.4.3/simplyblock_web/templates/deploy_spdk.yaml.j2
+Filename: sbcli_dev-2.4.4/simplyblock_web/templates/deploy_spdk.yaml.j2
 Comment: 
 
-Filename: sbcli_dev-2.4.3/simplyblock_web/blueprints/node_api_caching_docker.py
+Filename: sbcli_dev-2.4.4/simplyblock_web/blueprints/node_api_caching_docker.py
 Comment: 
 
-Filename: sbcli_dev-2.4.3/simplyblock_web/blueprints/node_api_caching_ks.py
+Filename: sbcli_dev-2.4.4/simplyblock_web/blueprints/node_api_caching_ks.py
 Comment: 
 
-Filename: sbcli_dev-2.4.3/simplyblock_web/blueprints/web_api_caching_node.py
+Filename: sbcli_dev-2.4.4/simplyblock_web/blueprints/web_api_caching_node.py
 Comment: 
 
-Filename: sbcli_dev-2.4.3/simplyblock_web/blueprints/snode_ops.py
+Filename: sbcli_dev-2.4.4/simplyblock_web/blueprints/snode_ops.py
 Comment: 
 
-Filename: sbcli_dev-2.4.3/simplyblock_web/blueprints/web_api_lvol.py
+Filename: sbcli_dev-2.4.4/simplyblock_web/blueprints/web_api_lvol.py
 Comment: 
 
-Filename: sbcli_dev-2.4.3/simplyblock_web/blueprints/csi.py
+Filename: sbcli_dev-2.4.4/simplyblock_web/blueprints/csi.py
 Comment: 
 
-Filename: sbcli_dev-2.4.3/simplyblock_web/blueprints/caching_node_ops.py
+Filename: sbcli_dev-2.4.4/simplyblock_web/blueprints/caching_node_ops.py
 Comment: 
 
-Filename: sbcli_dev-2.4.3/simplyblock_web/blueprints/web_api_mgmt_node.py
+Filename: sbcli_dev-2.4.4/simplyblock_web/blueprints/web_api_mgmt_node.py
 Comment: 
 
-Filename: sbcli_dev-2.4.3/simplyblock_web/blueprints/web_api_storage_node.py
+Filename: sbcli_dev-2.4.4/simplyblock_web/blueprints/web_api_storage_node.py
 Comment: 
 
-Filename: sbcli_dev-2.4.3/simplyblock_web/blueprints/__init__.py
+Filename: sbcli_dev-2.4.4/simplyblock_web/blueprints/__init__.py
 Comment: 
 
-Filename: sbcli_dev-2.4.3/simplyblock_web/blueprints/caching_node_ops_k8s.py
+Filename: sbcli_dev-2.4.4/simplyblock_web/blueprints/caching_node_ops_k8s.py
 Comment: 
 
-Filename: sbcli_dev-2.4.3/simplyblock_web/blueprints/web_api_device.py
+Filename: sbcli_dev-2.4.4/simplyblock_web/blueprints/web_api_device.py
 Comment: 
 
-Filename: sbcli_dev-2.4.3/simplyblock_web/blueprints/web_api_cluster.py
+Filename: sbcli_dev-2.4.4/simplyblock_web/blueprints/web_api_cluster.py
 Comment: 
 
-Filename: sbcli_dev-2.4.3/simplyblock_web/blueprints/node_api_basic.py
+Filename: sbcli_dev-2.4.4/simplyblock_web/blueprints/node_api_basic.py
 Comment: 
 
-Filename: sbcli_dev-2.4.3/simplyblock_web/blueprints/web_api_pool.py
+Filename: sbcli_dev-2.4.4/simplyblock_web/blueprints/web_api_pool.py
 Comment: 
 
 Zip file comment:
```

## Comparing `sbcli_dev-2.4.3/setup.py` & `sbcli_dev-2.4.4/setup.py`

 * *Files identical despite different names*

## Comparing `sbcli_dev-2.4.3/README.md` & `sbcli_dev-2.4.4/README.md`

 * *Files identical despite different names*

## Comparing `sbcli_dev-2.4.3/PKG-INFO` & `sbcli_dev-2.4.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sbcli-dev
-Version: 2.4.3
+Version: 2.4.4
 Summary: CLI for managing SimplyBlock cluster
 Home-page: https://www.simplyblock.io/
 Author: Hamdy
 Author-email: hamdy@simplyblock.io
 Description-Content-Type: text/markdown
 Requires-Dist: foundationdb
 Requires-Dist: requests
```

## Comparing `sbcli_dev-2.4.3/simplyblock_cli/cli.py` & `sbcli_dev-2.4.4/simplyblock_cli/cli.py`

 * *Files 1% similar despite different names*

```diff
@@ -306,14 +306,18 @@
         sub_command.add_argument("--cap-crit", help='Capacity critical level in percent, default=90',
                                  type=int, required=False, dest="cap_crit")
         sub_command.add_argument("--prov-cap-warn", help='Capacity warning level in percent, default=180',
                                  type=int, required=False, dest="prov_cap_warn")
         sub_command.add_argument("--prov-cap-crit", help='Capacity critical level in percent, default=190',
                                  type=int, required=False, dest="prov_cap_crit")
         sub_command.add_argument("--ifname", help='Management interface name, default: eth0')
+        sub_command.add_argument("--log-del-interval", help='graylog deletion interval, default: 24h',
+                                 dest='log_del_interval', default='24h')
+        sub_command.add_argument("--metrics-retention-period", help='retention period for prometheus metrics, default: 7d',
+                                 dest='metrics_retention_period', default='7d')
 
         # show cluster list
         sub_command = self.add_sub_command(subparser, 'list', 'Show clusters list')
 
         # # join cluster
         # sub_command = self.add_sub_command(subparser, 'join', 'join cluster')
         # sub_command.add_argument("cluster_ip", help='the cluster IP address')
@@ -1341,20 +1345,22 @@
         CLI_PASS = args.CLI_PASS
         model_ids = args.model_ids
         cap_warn = args.cap_warn
         cap_crit = args.cap_crit
         prov_cap_warn = args.prov_cap_warn
         prov_cap_crit = args.prov_cap_crit
         ifname = args.ifname
+        log_del_interval = args.log_del_interval
+        metrics_retention_period = args.metrics_retention_period
 
         # TODO: Validate the inputs
         return cluster_ops.create_cluster(
             blk_size, page_size_in_blocks, ha_type, tls,
             auth_hosts_only, CLI_PASS, model_ids, cap_warn, cap_crit, prov_cap_warn, prov_cap_crit,
-            ifname)
+            ifname, log_del_interval, metrics_retention_period)
 
     def cluster_join(self, args):
         cluster_id = args.cluster_id
         cluster_ip = args.cluster_ip
         role = args.role
         ifname = args.ifname
         data_nics = args.data_nics
```

## Comparing `sbcli_dev-2.4.3/sbcli_dev.egg-info/SOURCES.txt` & `sbcli_dev-2.4.4/sbcli_dev.egg-info/SOURCES.txt`

 * *Files identical despite different names*

## Comparing `sbcli_dev-2.4.3/sbcli_dev.egg-info/PKG-INFO` & `sbcli_dev-2.4.4/sbcli_dev.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sbcli-dev
-Version: 2.4.3
+Version: 2.4.4
 Summary: CLI for managing SimplyBlock cluster
 Home-page: https://www.simplyblock.io/
 Author: Hamdy
 Author-email: hamdy@simplyblock.io
 Description-Content-Type: text/markdown
 Requires-Dist: foundationdb
 Requires-Dist: requests
```

## Comparing `sbcli_dev-2.4.3/simplyblock_core/storage_node_ops.py` & `sbcli_dev-2.4.4/simplyblock_core/storage_node_ops.py`

 * *Files identical despite different names*

## Comparing `sbcli_dev-2.4.3/simplyblock_core/constants.py` & `sbcli_dev-2.4.4/simplyblock_core/constants.py`

 * *Files 10% similar despite different names*

```diff
@@ -45,13 +45,14 @@
 }
 
 # To use 75% of hugepages to calculate ssd size to use for the ocf bdev
 CACHING_NODE_MEMORY_FACTOR = 0.75
 
 HEALTH_CHECK_INTERVAL_SEC = 60
 
+GRAYLOG_CHECK_INTERVAL_SEC = 60
 
-SIMPLY_BLOCK_DOCKER_IMAGE = "simplyblock/simplyblock:dev"
+SIMPLY_BLOCK_DOCKER_IMAGE = "simplyblock/simplyblock:cleanup_logs_monitor_data"
 SIMPLY_BLOCK_SPDK_CORE_IMAGE = "simplyblock/spdk-core:latest"
 SIMPLY_BLOCK_SPDK_ULTRA_IMAGE = "simplyblock/spdk:main-latest"
 
 GELF_PORT = 12201
```

## Comparing `sbcli_dev-2.4.3/simplyblock_core/mgmt_node_ops.py` & `sbcli_dev-2.4.4/simplyblock_core/mgmt_node_ops.py`

 * *Files identical despite different names*

## Comparing `sbcli_dev-2.4.3/simplyblock_core/cnode_client.py` & `sbcli_dev-2.4.4/simplyblock_core/cnode_client.py`

 * *Files identical despite different names*

## Comparing `sbcli_dev-2.4.3/simplyblock_core/pci_utils.py` & `sbcli_dev-2.4.4/simplyblock_core/pci_utils.py`

 * *Files identical despite different names*

## Comparing `sbcli_dev-2.4.3/simplyblock_core/snode_client.py` & `sbcli_dev-2.4.4/simplyblock_core/snode_client.py`

 * *Files identical despite different names*

## Comparing `sbcli_dev-2.4.3/simplyblock_core/kv_store.py` & `sbcli_dev-2.4.4/simplyblock_core/kv_store.py`

 * *Files identical despite different names*

## Comparing `sbcli_dev-2.4.3/simplyblock_core/utils.py` & `sbcli_dev-2.4.4/simplyblock_core/utils.py`

 * *Files identical despite different names*

## Comparing `sbcli_dev-2.4.3/simplyblock_core/cluster_ops.py` & `sbcli_dev-2.4.4/simplyblock_core/cluster_ops.py`

 * *Files 1% similar despite different names*

```diff
@@ -43,15 +43,15 @@
     session.auth = ("admin", password)
     response = session.request("POST", url, headers=headers, data=payload)
     logger.debug(response.text)
     return response.status_code == 201
 
 def create_cluster(blk_size, page_size_in_blocks, ha_type, tls,
                    auth_hosts_only, cli_pass, model_ids,
-                   cap_warn, cap_crit, prov_cap_warn, prov_cap_crit, ifname):
+                   cap_warn, cap_crit, prov_cap_warn, prov_cap_crit, ifname, log_del_interval, metrics_retention_period):
     logger.info("Installing dependencies...")
     ret = scripts.install_deps()
     logger.info("Installing dependencies > Done")
 
     if not ifname:
         ifname = "eth0"
 
@@ -103,15 +103,15 @@
         c.cap_crit = cap_crit
     if prov_cap_warn and prov_cap_warn > 0:
         c.prov_cap_warn = prov_cap_warn
     if prov_cap_crit and prov_cap_crit > 0:
         c.prov_cap_crit = prov_cap_crit
 
     logger.info("Deploying swarm stack ...")
-    ret = scripts.deploy_stack(cli_pass, DEV_IP, constants.SIMPLY_BLOCK_DOCKER_IMAGE, c.secret, c.uuid)
+    ret = scripts.deploy_stack(cli_pass, DEV_IP, constants.SIMPLY_BLOCK_DOCKER_IMAGE, c.secret, c.uuid, log_del_interval, metrics_retention_period)
     logger.info("Deploying swarm stack > Done")
 
     logger.info("Configuring DB...")
     out = scripts.set_db_config_single()
     logger.info("Configuring DB > Done")
 
     _add_graylog_input(DEV_IP, c.secret)
```

## Comparing `sbcli_dev-2.4.3/simplyblock_core/compute_node_ops.py` & `sbcli_dev-2.4.4/simplyblock_core/compute_node_ops.py`

 * *Files identical despite different names*

## Comparing `sbcli_dev-2.4.3/simplyblock_core/rpc_client.py` & `sbcli_dev-2.4.4/simplyblock_core/rpc_client.py`

 * *Files identical despite different names*

## Comparing `sbcli_dev-2.4.3/simplyblock_core/distr_controller.py` & `sbcli_dev-2.4.4/simplyblock_core/distr_controller.py`

 * *Files identical despite different names*

## Comparing `sbcli_dev-2.4.3/simplyblock_core/services/lvol_monitor.py` & `sbcli_dev-2.4.4/simplyblock_core/services/lvol_monitor.py`

 * *Files identical despite different names*

## Comparing `sbcli_dev-2.4.3/simplyblock_core/services/caching_node_monitor.py` & `sbcli_dev-2.4.4/simplyblock_core/services/caching_node_monitor.py`

 * *Files identical despite different names*

## Comparing `sbcli_dev-2.4.3/simplyblock_core/services/health_check_service.py` & `sbcli_dev-2.4.4/simplyblock_core/services/health_check_service.py`

 * *Files identical despite different names*

## Comparing `sbcli_dev-2.4.3/simplyblock_core/services/lvol_stat_collector.py` & `sbcli_dev-2.4.4/simplyblock_core/services/lvol_stat_collector.py`

 * *Files identical despite different names*

## Comparing `sbcli_dev-2.4.3/simplyblock_core/services/log_agg_service.py` & `sbcli_dev-2.4.4/simplyblock_core/services/log_agg_service.py`

 * *Files identical despite different names*

## Comparing `sbcli_dev-2.4.3/simplyblock_core/services/distr_event_collector.py` & `sbcli_dev-2.4.4/simplyblock_core/services/distr_event_collector.py`

 * *Files identical despite different names*

## Comparing `sbcli_dev-2.4.3/simplyblock_core/services/capacity_and_stats_collector.py` & `sbcli_dev-2.4.4/simplyblock_core/services/capacity_and_stats_collector.py`

 * *Files identical despite different names*

## Comparing `sbcli_dev-2.4.3/simplyblock_core/services/port_stat_collector.py` & `sbcli_dev-2.4.4/simplyblock_core/services/port_stat_collector.py`

 * *Files identical despite different names*

## Comparing `sbcli_dev-2.4.3/simplyblock_core/services/device_monitor.py` & `sbcli_dev-2.4.4/simplyblock_core/services/device_monitor.py`

 * *Files identical despite different names*

## Comparing `sbcli_dev-2.4.3/simplyblock_core/services/__init__.py` & `sbcli_dev-2.4.4/simplyblock_core/services/__init__.py`

 * *Files identical despite different names*

## Comparing `sbcli_dev-2.4.3/simplyblock_core/services/install_service.sh` & `sbcli_dev-2.4.4/simplyblock_core/services/install_service.sh`

 * *Files identical despite different names*

## Comparing `sbcli_dev-2.4.3/simplyblock_core/services/mgmt_node_monitor.py` & `sbcli_dev-2.4.4/simplyblock_core/services/mgmt_node_monitor.py`

 * *Files identical despite different names*

## Comparing `sbcli_dev-2.4.3/simplyblock_core/services/cap_monitor.py` & `sbcli_dev-2.4.4/simplyblock_core/services/cap_monitor.py`

 * *Files identical despite different names*

## Comparing `sbcli_dev-2.4.3/simplyblock_core/services/storage_node_monitor.py` & `sbcli_dev-2.4.4/simplyblock_core/services/storage_node_monitor.py`

 * *Files identical despite different names*

## Comparing `sbcli_dev-2.4.3/simplyblock_core/scripts/deploy_stack.sh` & `sbcli_dev-2.4.4/simplyblock_core/scripts/deploy_stack.sh`

 * *Files 9% similar despite different names*

```diff
@@ -5,14 +5,16 @@
 export SIMPLYBLOCK_DOCKER_IMAGE=$3
 
 export GRAYLOG_ROOT_PASSWORD_SHA2=$4
 export GRAYLOG_PASSWORD_SECRET="is6SP2EdWg0NdmVGv6CEp5hRHNL7BKVMFem4t9pouMqDQnHwXMSomas1qcbKSt5yISr8eBHv4Y7Dbswhyz84Ut0TW6kqsiPs"
 
 export CLUSTER_SECRET=$5
 export CLUSTER_ID=$6
+export LOG_DELETION_INTERVAL=$7
+export RETENTION_PERIOD=$8
 export DIR="$(dirname "$(realpath "$0")")"
 
 if [ -s "/etc/foundationdb/fdb.cluster" ]
 then
    FDB_CLUSTER_FILE_CONTENTS=$(tail /etc/foundationdb/fdb.cluster -n 1)
    export FDB_CLUSTER_FILE_CONTENTS=$FDB_CLUSTER_FILE_CONTENTS
 fi
```

## Comparing `sbcli_dev-2.4.3/simplyblock_core/scripts/haproxy.cfg` & `sbcli_dev-2.4.4/simplyblock_core/scripts/haproxy.cfg`

 * *Files identical despite different names*

## Comparing `sbcli_dev-2.4.3/simplyblock_core/scripts/docker-compose-swarm.yml` & `sbcli_dev-2.4.4/simplyblock_core/scripts/docker-compose-swarm.yml`

 * *Files identical despite different names*

## Comparing `sbcli_dev-2.4.3/simplyblock_core/scripts/stack_deploy_wait.sh` & `sbcli_dev-2.4.4/simplyblock_core/scripts/stack_deploy_wait.sh`

 * *Files identical despite different names*

## Comparing `sbcli_dev-2.4.3/simplyblock_core/scripts/docker-compose-swarm-monitoring.yml` & `sbcli_dev-2.4.4/simplyblock_core/scripts/docker-compose-swarm-monitoring.yml`

 * *Files 13% similar despite different names*

```diff
@@ -76,14 +76,15 @@
     user: root
     volumes:
       - ./prometheus.yml:/etc/prometheus/prometheus.yml
       - prometheus_data:/prometheus
     command:
       - "--config.file=/etc/prometheus/prometheus.yml"
       - "--storage.tsdb.path=/prometheus"
+      - "--storage.tsdb.retention.time=${RETENTION_PERIOD}"
     restart: "always"
     deploy:
       placement:
         constraints: [node.role == manager]
 
   node-exporter:
     image: prom/node-exporter:v1.7.0
@@ -124,14 +125,23 @@
         published: 3000
         protocol: tcp
         mode: host
     deploy:
       placement:
         constraints: [node.role == manager]
 
+  CleanupGraylog:
+    image: $SIMPLYBLOCK_DOCKER_IMAGE
+    environment:
+      LOG_DELETION_INTERVAL: "${LOG_DELETION_INTERVAL}"
+    command: "python simplyblock_core/workers/cleanup_graylog.py"
+    deploy:
+      placement:
+        constraints: [node.role == manager]
+
   ### monitoring ###
 
 volumes:
   mongodb_data:
   os_data:
   graylog_data:
   graylog_journal:
```

## Comparing `sbcli_dev-2.4.3/simplyblock_core/scripts/__init__.py` & `sbcli_dev-2.4.4/simplyblock_core/scripts/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -26,18 +26,18 @@
     return __run_script(['bash', '-x', os.path.join(DIR_PATH, 'install_deps.sh')])
 
 
 def configure_docker(docker_ip):
     return __run_script(['bash', '-x', os.path.join(DIR_PATH, 'config_docker.sh'), docker_ip])
 
 
-def deploy_stack(cli_pass, dev_ip, image_name, graylog_password, cluster_id):
+def deploy_stack(cli_pass, dev_ip, image_name, graylog_password, cluster_id, log_del_interval, metrics_retention_period):
     pass_hash = hashlib.sha256(graylog_password.encode('utf-8')).hexdigest()
     return __run_script(
-        ['sudo', 'bash', '-x', os.path.join(DIR_PATH, 'deploy_stack.sh'), cli_pass, dev_ip, image_name, pass_hash, graylog_password, cluster_id])
+        ['sudo', 'bash', '-x', os.path.join(DIR_PATH, 'deploy_stack.sh'), cli_pass, dev_ip, image_name, pass_hash, graylog_password, cluster_id, log_del_interval, metrics_retention_period])
 
 def apply_dashboard(grafanaPassword):
     return __run_script(
         ['sudo', 'bash', '-x', os.path.join(DIR_PATH, 'apply_dashboard.sh'), grafanaPassword])
 
 
 def deploy_cleaner():
```

## Comparing `sbcli_dev-2.4.3/simplyblock_core/scripts/install_deps.sh` & `sbcli_dev-2.4.4/simplyblock_core/scripts/install_deps.sh`

 * *Files identical despite different names*

## Comparing `sbcli_dev-2.4.3/simplyblock_core/scripts/apply_dashboard.sh` & `sbcli_dev-2.4.4/simplyblock_core/scripts/apply_dashboard.sh`

 * *Files identical despite different names*

## Comparing `sbcli_dev-2.4.3/simplyblock_core/scripts/alerting/alert_rules.yaml` & `sbcli_dev-2.4.4/simplyblock_core/scripts/alerting/alert_rules.yaml`

 * *Files identical despite different names*

## Comparing `sbcli_dev-2.4.3/simplyblock_core/scripts/alerting/alert_resources.yaml` & `sbcli_dev-2.4.4/simplyblock_core/scripts/alerting/alert_resources.yaml`

 * *Files identical despite different names*

## Comparing `sbcli_dev-2.4.3/simplyblock_core/scripts/dashboards/devices.json` & `sbcli_dev-2.4.4/simplyblock_core/scripts/dashboards/devices.json`

 * *Files identical despite different names*

## Comparing `sbcli_dev-2.4.3/simplyblock_core/scripts/dashboards/node-exporter.json` & `sbcli_dev-2.4.4/simplyblock_core/scripts/dashboards/node-exporter.json`

 * *Files identical despite different names*

## Comparing `sbcli_dev-2.4.3/simplyblock_core/scripts/dashboards/nodes.json` & `sbcli_dev-2.4.4/simplyblock_core/scripts/dashboards/nodes.json`

 * *Files identical despite different names*

## Comparing `sbcli_dev-2.4.3/simplyblock_core/scripts/dashboards/lvols.json` & `sbcli_dev-2.4.4/simplyblock_core/scripts/dashboards/lvols.json`

 * *Files identical despite different names*

## Comparing `sbcli_dev-2.4.3/simplyblock_core/scripts/dashboards/cluster.json` & `sbcli_dev-2.4.4/simplyblock_core/scripts/dashboards/cluster.json`

 * *Files identical despite different names*

## Comparing `sbcli_dev-2.4.3/simplyblock_core/scripts/dashboards/pools.json` & `sbcli_dev-2.4.4/simplyblock_core/scripts/dashboards/pools.json`

 * *Files identical despite different names*

## Comparing `sbcli_dev-2.4.3/simplyblock_core/controllers/device_controller.py` & `sbcli_dev-2.4.4/simplyblock_core/controllers/device_controller.py`

 * *Files identical despite different names*

## Comparing `sbcli_dev-2.4.3/simplyblock_core/controllers/mgmt_events.py` & `sbcli_dev-2.4.4/simplyblock_core/controllers/mgmt_events.py`

 * *Files identical despite different names*

## Comparing `sbcli_dev-2.4.3/simplyblock_core/controllers/events_controller.py` & `sbcli_dev-2.4.4/simplyblock_core/controllers/events_controller.py`

 * *Files identical despite different names*

## Comparing `sbcli_dev-2.4.3/simplyblock_core/controllers/storage_events.py` & `sbcli_dev-2.4.4/simplyblock_core/controllers/storage_events.py`

 * *Files identical despite different names*

## Comparing `sbcli_dev-2.4.3/simplyblock_core/controllers/lvol_events.py` & `sbcli_dev-2.4.4/simplyblock_core/controllers/lvol_events.py`

 * *Files identical despite different names*

## Comparing `sbcli_dev-2.4.3/simplyblock_core/controllers/snapshot_controller.py` & `sbcli_dev-2.4.4/simplyblock_core/controllers/snapshot_controller.py`

 * *Files identical despite different names*

## Comparing `sbcli_dev-2.4.3/simplyblock_core/controllers/device_events.py` & `sbcli_dev-2.4.4/simplyblock_core/controllers/device_events.py`

 * *Files identical despite different names*

## Comparing `sbcli_dev-2.4.3/simplyblock_core/controllers/pool_controller.py` & `sbcli_dev-2.4.4/simplyblock_core/controllers/pool_controller.py`

 * *Files identical despite different names*

## Comparing `sbcli_dev-2.4.3/simplyblock_core/controllers/cluster_events.py` & `sbcli_dev-2.4.4/simplyblock_core/controllers/cluster_events.py`

 * *Files identical despite different names*

## Comparing `sbcli_dev-2.4.3/simplyblock_core/controllers/caching_node_controller.py` & `sbcli_dev-2.4.4/simplyblock_core/controllers/caching_node_controller.py`

 * *Files identical despite different names*

## Comparing `sbcli_dev-2.4.3/simplyblock_core/controllers/snapshot_events.py` & `sbcli_dev-2.4.4/simplyblock_core/controllers/snapshot_events.py`

 * *Files identical despite different names*

## Comparing `sbcli_dev-2.4.3/simplyblock_core/controllers/lvol_controller.py` & `sbcli_dev-2.4.4/simplyblock_core/controllers/lvol_controller.py`

 * *Files identical despite different names*

## Comparing `sbcli_dev-2.4.3/simplyblock_core/controllers/health_controller.py` & `sbcli_dev-2.4.4/simplyblock_core/controllers/health_controller.py`

 * *Files identical despite different names*

## Comparing `sbcli_dev-2.4.3/simplyblock_core/controllers/pool_events.py` & `sbcli_dev-2.4.4/simplyblock_core/controllers/pool_events.py`

 * *Files identical despite different names*

## Comparing `sbcli_dev-2.4.3/simplyblock_core/models/events.py` & `sbcli_dev-2.4.4/simplyblock_core/models/events.py`

 * *Files identical despite different names*

## Comparing `sbcli_dev-2.4.3/simplyblock_core/models/iface.py` & `sbcli_dev-2.4.4/simplyblock_core/models/iface.py`

 * *Files identical despite different names*

## Comparing `sbcli_dev-2.4.3/simplyblock_core/models/base_model.py` & `sbcli_dev-2.4.4/simplyblock_core/models/base_model.py`

 * *Files identical despite different names*

## Comparing `sbcli_dev-2.4.3/simplyblock_core/models/lvol_model.py` & `sbcli_dev-2.4.4/simplyblock_core/models/lvol_model.py`

 * *Files identical despite different names*

## Comparing `sbcli_dev-2.4.3/simplyblock_core/models/compute_node.py` & `sbcli_dev-2.4.4/simplyblock_core/models/compute_node.py`

 * *Files identical despite different names*

## Comparing `sbcli_dev-2.4.3/simplyblock_core/models/snapshot.py` & `sbcli_dev-2.4.4/simplyblock_core/models/snapshot.py`

 * *Files identical despite different names*

## Comparing `sbcli_dev-2.4.3/simplyblock_core/models/pool.py` & `sbcli_dev-2.4.4/simplyblock_core/models/pool.py`

 * *Files identical despite different names*

## Comparing `sbcli_dev-2.4.3/simplyblock_core/models/global_settings.py` & `sbcli_dev-2.4.4/simplyblock_core/models/global_settings.py`

 * *Files identical despite different names*

## Comparing `sbcli_dev-2.4.3/simplyblock_core/models/port_stat.py` & `sbcli_dev-2.4.4/simplyblock_core/models/port_stat.py`

 * *Files identical despite different names*

## Comparing `sbcli_dev-2.4.3/simplyblock_core/models/storage_node.py` & `sbcli_dev-2.4.4/simplyblock_core/models/storage_node.py`

 * *Files identical despite different names*

## Comparing `sbcli_dev-2.4.3/simplyblock_core/models/stats.py` & `sbcli_dev-2.4.4/simplyblock_core/models/stats.py`

 * *Files identical despite different names*

## Comparing `sbcli_dev-2.4.3/simplyblock_core/models/cluster.py` & `sbcli_dev-2.4.4/simplyblock_core/models/cluster.py`

 * *Files identical despite different names*

## Comparing `sbcli_dev-2.4.3/simplyblock_core/models/mgmt_node.py` & `sbcli_dev-2.4.4/simplyblock_core/models/mgmt_node.py`

 * *Files identical despite different names*

## Comparing `sbcli_dev-2.4.3/simplyblock_core/models/caching_node.py` & `sbcli_dev-2.4.4/simplyblock_core/models/caching_node.py`

 * *Files identical despite different names*

## Comparing `sbcli_dev-2.4.3/simplyblock_core/models/nvme_device.py` & `sbcli_dev-2.4.4/simplyblock_core/models/nvme_device.py`

 * *Files identical despite different names*

## Comparing `sbcli_dev-2.4.3/simplyblock_web/caching_node_app_k8s.py` & `sbcli_dev-2.4.4/simplyblock_web/caching_node_app_k8s.py`

 * *Files identical despite different names*

## Comparing `sbcli_dev-2.4.3/simplyblock_web/node_utils.py` & `sbcli_dev-2.4.4/simplyblock_web/node_utils.py`

 * *Files identical despite different names*

## Comparing `sbcli_dev-2.4.3/simplyblock_web/snode_app.py` & `sbcli_dev-2.4.4/simplyblock_web/snode_app.py`

 * *Files identical despite different names*

## Comparing `sbcli_dev-2.4.3/simplyblock_web/app.py` & `sbcli_dev-2.4.4/simplyblock_web/app.py`

 * *Files identical despite different names*

## Comparing `sbcli_dev-2.4.3/simplyblock_web/auth_middleware.py` & `sbcli_dev-2.4.4/simplyblock_web/auth_middleware.py`

 * *Files identical despite different names*

## Comparing `sbcli_dev-2.4.3/simplyblock_web/caching_node_app.py` & `sbcli_dev-2.4.4/simplyblock_web/caching_node_app.py`

 * *Files identical despite different names*

## Comparing `sbcli_dev-2.4.3/simplyblock_web/utils.py` & `sbcli_dev-2.4.4/simplyblock_web/utils.py`

 * *Files identical despite different names*

## Comparing `sbcli_dev-2.4.3/simplyblock_web/node_webapp.py` & `sbcli_dev-2.4.4/simplyblock_web/node_webapp.py`

 * *Files identical despite different names*

## Comparing `sbcli_dev-2.4.3/simplyblock_web/static/delete.py` & `sbcli_dev-2.4.4/simplyblock_web/static/delete.py`

 * *Files identical despite different names*

## Comparing `sbcli_dev-2.4.3/simplyblock_web/static/deploy.py` & `sbcli_dev-2.4.4/simplyblock_web/static/deploy.py`

 * *Files identical despite different names*

## Comparing `sbcli_dev-2.4.3/simplyblock_web/static/deploy_spdk.yaml` & `sbcli_dev-2.4.4/simplyblock_web/static/deploy_spdk.yaml`

 * *Files identical despite different names*

## Comparing `sbcli_dev-2.4.3/simplyblock_web/templates/deploy_spdk.yaml.j2` & `sbcli_dev-2.4.4/simplyblock_web/templates/deploy_spdk.yaml.j2`

 * *Files identical despite different names*

## Comparing `sbcli_dev-2.4.3/simplyblock_web/blueprints/node_api_caching_docker.py` & `sbcli_dev-2.4.4/simplyblock_web/blueprints/node_api_caching_docker.py`

 * *Files identical despite different names*

## Comparing `sbcli_dev-2.4.3/simplyblock_web/blueprints/node_api_caching_ks.py` & `sbcli_dev-2.4.4/simplyblock_web/blueprints/node_api_caching_ks.py`

 * *Files identical despite different names*

## Comparing `sbcli_dev-2.4.3/simplyblock_web/blueprints/web_api_caching_node.py` & `sbcli_dev-2.4.4/simplyblock_web/blueprints/web_api_caching_node.py`

 * *Files identical despite different names*

## Comparing `sbcli_dev-2.4.3/simplyblock_web/blueprints/snode_ops.py` & `sbcli_dev-2.4.4/simplyblock_web/blueprints/snode_ops.py`

 * *Files identical despite different names*

## Comparing `sbcli_dev-2.4.3/simplyblock_web/blueprints/web_api_lvol.py` & `sbcli_dev-2.4.4/simplyblock_web/blueprints/web_api_lvol.py`

 * *Files identical despite different names*

## Comparing `sbcli_dev-2.4.3/simplyblock_web/blueprints/csi.py` & `sbcli_dev-2.4.4/simplyblock_web/blueprints/csi.py`

 * *Files identical despite different names*

## Comparing `sbcli_dev-2.4.3/simplyblock_web/blueprints/caching_node_ops.py` & `sbcli_dev-2.4.4/simplyblock_web/blueprints/caching_node_ops.py`

 * *Files identical despite different names*

## Comparing `sbcli_dev-2.4.3/simplyblock_web/blueprints/web_api_mgmt_node.py` & `sbcli_dev-2.4.4/simplyblock_web/blueprints/web_api_mgmt_node.py`

 * *Files identical despite different names*

## Comparing `sbcli_dev-2.4.3/simplyblock_web/blueprints/web_api_storage_node.py` & `sbcli_dev-2.4.4/simplyblock_web/blueprints/web_api_storage_node.py`

 * *Files identical despite different names*

## Comparing `sbcli_dev-2.4.3/simplyblock_web/blueprints/caching_node_ops_k8s.py` & `sbcli_dev-2.4.4/simplyblock_web/blueprints/caching_node_ops_k8s.py`

 * *Files identical despite different names*

## Comparing `sbcli_dev-2.4.3/simplyblock_web/blueprints/web_api_device.py` & `sbcli_dev-2.4.4/simplyblock_web/blueprints/web_api_device.py`

 * *Files identical despite different names*

## Comparing `sbcli_dev-2.4.3/simplyblock_web/blueprints/web_api_cluster.py` & `sbcli_dev-2.4.4/simplyblock_web/blueprints/web_api_cluster.py`

 * *Files identical despite different names*

## Comparing `sbcli_dev-2.4.3/simplyblock_web/blueprints/node_api_basic.py` & `sbcli_dev-2.4.4/simplyblock_web/blueprints/node_api_basic.py`

 * *Files identical despite different names*

## Comparing `sbcli_dev-2.4.3/simplyblock_web/blueprints/web_api_pool.py` & `sbcli_dev-2.4.4/simplyblock_web/blueprints/web_api_pool.py`

 * *Files identical despite different names*

