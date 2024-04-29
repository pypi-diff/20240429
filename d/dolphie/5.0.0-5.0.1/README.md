# Comparing `tmp/dolphie-5.0.0.tar.gz` & `tmp/dolphie-5.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dolphie-5.0.0.tar", max compression
+gzip compressed data, was "dolphie-5.0.1.tar", max compression
```

## Comparing `dolphie-5.0.0.tar` & `dolphie-5.0.1.tar`

### file list

```diff
@@ -1,35 +1,35 @@
--rw-r--r--   0        0        0    35149 2022-09-02 19:06:44.751434 dolphie-5.0.0/LICENSE
--rw-r--r--   0        0        0    10612 2024-04-24 08:27:31.216200 dolphie-5.0.0/README.md
--rw-r--r--   0        0        0     7743 2024-04-24 08:27:31.216691 dolphie-5.0.0/dolphie/DataTypes.py
--rw-r--r--   0        0        0     8998 2024-04-24 08:27:31.216991 dolphie-5.0.0/dolphie/Dolphie.css
--rw-r--r--   0        0        0    21812 2024-04-24 08:27:31.217321 dolphie-5.0.0/dolphie/Modules/ArgumentParser.py
--rw-r--r--   0        0        0     6769 2024-04-24 08:27:31.217923 dolphie-5.0.0/dolphie/Modules/Functions.py
--rw-r--r--   0        0        0      975 2024-02-26 06:55:52.585216 dolphie-5.0.0/dolphie/Modules/ManualException.py
--rw-r--r--   0        0        0    38471 2024-04-24 08:27:31.218418 dolphie-5.0.0/dolphie/Modules/MetricManager.py
--rw-r--r--   0        0        0     8308 2024-04-24 08:27:31.218829 dolphie-5.0.0/dolphie/Modules/MySQL.py
--rw-r--r--   0        0        0    19600 2024-04-24 08:27:31.219258 dolphie-5.0.0/dolphie/Modules/Queries.py
--rw-r--r--   0        0        0    25493 2024-04-24 08:27:31.219824 dolphie-5.0.0/dolphie/Modules/TabManager.py
--rw-r--r--   0        0        0     9247 2024-04-24 08:27:31.220351 dolphie-5.0.0/dolphie/Panels/dashboard_panel.py
--rw-r--r--   0        0        0     1559 2024-02-26 06:55:52.588164 dolphie-5.0.0/dolphie/Panels/ddl_panel.py
--rw-r--r--   0        0        0     2893 2024-02-26 06:55:52.588611 dolphie-5.0.0/dolphie/Panels/innodb_trx_locks_panel.py
--rw-r--r--   0        0        0     7360 2024-04-24 08:27:31.220949 dolphie-5.0.0/dolphie/Panels/metadata_locks_panel.py
--rw-r--r--   0        0        0     9809 2024-04-24 08:27:31.221435 dolphie-5.0.0/dolphie/Panels/processlist_panel.py
--rw-r--r--   0        0        0     3925 2024-04-24 08:27:31.221888 dolphie-5.0.0/dolphie/Panels/proxysql_command_stats_panel.py
--rw-r--r--   0        0        0     5766 2024-04-24 08:27:31.222346 dolphie-5.0.0/dolphie/Panels/proxysql_dashboard_panel.py
--rw-r--r--   0        0        0     4949 2024-04-24 08:27:31.222954 dolphie-5.0.0/dolphie/Panels/proxysql_hostgroup_summary_panel.py
--rw-r--r--   0        0        0     4086 2024-04-24 08:27:31.223282 dolphie-5.0.0/dolphie/Panels/proxysql_mysql_query_rules_panel.py
--rw-r--r--   0        0        0     6839 2024-04-24 08:27:31.223666 dolphie-5.0.0/dolphie/Panels/proxysql_processlist_panel.py
--rw-r--r--   0        0        0    25774 2024-04-09 22:54:28.708150 dolphie-5.0.0/dolphie/Panels/replication_panel.py
--rw-r--r--   0        0        0     1050 2024-02-12 13:50:32.934971 dolphie-5.0.0/dolphie/Widgets/command_screen.py
--rw-r--r--   0        0        0     6319 2024-02-26 06:55:52.590441 dolphie-5.0.0/dolphie/Widgets/event_log_screen.py
--rw-r--r--   0        0        0     9392 2024-04-24 08:27:31.224044 dolphie-5.0.0/dolphie/Widgets/help.py
--rw-r--r--   0        0        0    13960 2024-03-15 01:09:17.039272 dolphie-5.0.0/dolphie/Widgets/host_setup.py
--rw-r--r--   0        0        0    12034 2024-04-24 08:27:31.224413 dolphie-5.0.0/dolphie/Widgets/modal.py
--rw-r--r--   0        0        0     3873 2024-04-24 08:27:31.224676 dolphie-5.0.0/dolphie/Widgets/proxysql_thread_screen.py
--rw-r--r--   0        0        0      563 2024-02-26 06:55:52.591220 dolphie-5.0.0/dolphie/Widgets/spinner.py
--rw-r--r--   0        0        0     5997 2024-04-24 08:27:31.225002 dolphie-5.0.0/dolphie/Widgets/thread_screen.py
--rw-r--r--   0        0        0     1125 2024-02-12 13:50:32.936036 dolphie-5.0.0/dolphie/Widgets/topbar.py
--rw-r--r--   0        0        0    13475 2024-04-24 08:27:31.225358 dolphie-5.0.0/dolphie/__init__.py
--rwxr-xr-x   0        0        0    79079 2024-04-24 08:27:31.225932 dolphie-5.0.0/dolphie/app.py
--rw-r--r--   0        0        0      679 2024-04-24 08:27:31.227560 dolphie-5.0.0/pyproject.toml
--rw-r--r--   0        0        0    11680 1970-01-01 00:00:00.000000 dolphie-5.0.0/PKG-INFO
+-rw-r--r--   0        0        0    35149 2022-09-02 19:06:44.751434 dolphie-5.0.1/LICENSE
+-rw-r--r--   0        0        0    10793 2024-04-26 06:15:38.607085 dolphie-5.0.1/README.md
+-rw-r--r--   0        0        0     7743 2024-04-24 08:27:31.216691 dolphie-5.0.1/dolphie/DataTypes.py
+-rw-r--r--   0        0        0     8998 2024-04-24 08:27:31.216991 dolphie-5.0.1/dolphie/Dolphie.css
+-rw-r--r--   0        0        0    21811 2024-04-26 06:15:38.607944 dolphie-5.0.1/dolphie/Modules/ArgumentParser.py
+-rw-r--r--   0        0        0     6769 2024-04-24 08:32:49.079123 dolphie-5.0.1/dolphie/Modules/Functions.py
+-rw-r--r--   0        0        0      975 2024-02-26 06:55:52.585216 dolphie-5.0.1/dolphie/Modules/ManualException.py
+-rw-r--r--   0        0        0    38471 2024-04-24 08:27:31.218418 dolphie-5.0.1/dolphie/Modules/MetricManager.py
+-rw-r--r--   0        0        0     8204 2024-04-29 08:16:25.745454 dolphie-5.0.1/dolphie/Modules/MySQL.py
+-rw-r--r--   0        0        0    18980 2024-04-29 08:07:57.617395 dolphie-5.0.1/dolphie/Modules/Queries.py
+-rw-r--r--   0        0        0    25493 2024-04-24 08:27:31.219824 dolphie-5.0.1/dolphie/Modules/TabManager.py
+-rw-r--r--   0        0        0     9429 2024-04-29 08:32:25.955658 dolphie-5.0.1/dolphie/Panels/dashboard_panel.py
+-rw-r--r--   0        0        0     1559 2024-02-26 06:55:52.588164 dolphie-5.0.1/dolphie/Panels/ddl_panel.py
+-rw-r--r--   0        0        0     2893 2024-02-26 06:55:52.588611 dolphie-5.0.1/dolphie/Panels/innodb_trx_locks_panel.py
+-rw-r--r--   0        0        0     7360 2024-04-24 08:27:31.220949 dolphie-5.0.1/dolphie/Panels/metadata_locks_panel.py
+-rw-r--r--   0        0        0     9917 2024-04-29 08:20:11.637840 dolphie-5.0.1/dolphie/Panels/processlist_panel.py
+-rw-r--r--   0        0        0     3925 2024-04-24 08:27:31.221888 dolphie-5.0.1/dolphie/Panels/proxysql_command_stats_panel.py
+-rw-r--r--   0        0        0     5766 2024-04-25 17:40:15.854128 dolphie-5.0.1/dolphie/Panels/proxysql_dashboard_panel.py
+-rw-r--r--   0        0        0     4949 2024-04-24 08:27:31.222954 dolphie-5.0.1/dolphie/Panels/proxysql_hostgroup_summary_panel.py
+-rw-r--r--   0        0        0     4086 2024-04-24 08:27:31.223282 dolphie-5.0.1/dolphie/Panels/proxysql_mysql_query_rules_panel.py
+-rw-r--r--   0        0        0     6839 2024-04-24 08:27:31.223666 dolphie-5.0.1/dolphie/Panels/proxysql_processlist_panel.py
+-rw-r--r--   0        0        0    26275 2024-04-29 09:08:12.751007 dolphie-5.0.1/dolphie/Panels/replication_panel.py
+-rw-r--r--   0        0        0     1050 2024-02-12 13:50:32.934971 dolphie-5.0.1/dolphie/Widgets/command_screen.py
+-rw-r--r--   0        0        0     6319 2024-02-26 06:55:52.590441 dolphie-5.0.1/dolphie/Widgets/event_log_screen.py
+-rw-r--r--   0        0        0     9388 2024-04-26 06:15:38.608277 dolphie-5.0.1/dolphie/Widgets/help.py
+-rw-r--r--   0        0        0    13960 2024-03-15 01:09:17.039272 dolphie-5.0.1/dolphie/Widgets/host_setup.py
+-rw-r--r--   0        0        0    12034 2024-04-24 08:27:31.224413 dolphie-5.0.1/dolphie/Widgets/modal.py
+-rw-r--r--   0        0        0     3873 2024-04-24 08:27:31.224676 dolphie-5.0.1/dolphie/Widgets/proxysql_thread_screen.py
+-rw-r--r--   0        0        0      563 2024-02-26 06:55:52.591220 dolphie-5.0.1/dolphie/Widgets/spinner.py
+-rw-r--r--   0        0        0     5997 2024-04-24 08:27:31.225002 dolphie-5.0.1/dolphie/Widgets/thread_screen.py
+-rw-r--r--   0        0        0     1125 2024-02-12 13:50:32.936036 dolphie-5.0.1/dolphie/Widgets/topbar.py
+-rw-r--r--   0        0        0    13455 2024-04-29 07:10:07.370077 dolphie-5.0.1/dolphie/__init__.py
+-rwxr-xr-x   0        0        0    79546 2024-04-29 08:40:21.156862 dolphie-5.0.1/dolphie/app.py
+-rw-r--r--   0        0        0      679 2024-04-29 08:58:05.522159 dolphie-5.0.1/pyproject.toml
+-rw-r--r--   0        0        0    11861 1970-01-01 00:00:00.000000 dolphie-5.0.1/PKG-INFO
```

### Comparing `dolphie-5.0.0/LICENSE` & `dolphie-5.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `dolphie-5.0.0/README.md` & `dolphie-5.0.1/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 # Dolphie
 <p align="center">
   <img src="https://user-images.githubusercontent.com/13244625/187600748-19d2ad15-42e8-4f9c-ada5-a153cdcf4070.png" width="120"><br>
-  Your single pane of glass for real-time analytics into MySQL & ProxySQL<br><br>
+  Your single pane of glass for real-time analytics into MySQL/MariaDB & ProxySQL<br><br>
   <img src="https://github.com/charles-001/dolphie/assets/13244625/88a41290-f52c-4b8e-97f8-3b7ef5096eae" width="30">
   <img src="https://github.com/charles-001/dolphie/assets/13244625/1d94502a-9abf-4436-a7d0-cb2b08c105c1" width="30">
   <img src="https://github.com/charles-001/dolphie/assets/13244625/9b1aadc8-cabb-4256-92f9-fe4d04451b83" width="30">
 </p>
 <p align="center">
   <a href="https://www.buymeacoffee.com/charlesthompson">
     <img src="https://www.buymeacoffee.com/assets/img/custom_images/orange_img.png" alt="Buy Me A Coffee">
@@ -71,23 +71,23 @@
 
 options:
   --help                show this help message and exit
   --host-setup          Start Dolphie by showing the Host Setup modal instead of automatically connecting
   -u , --user           Username
   -p , --password       Password
   -h , --host           Hostname/IP address
-  -P , --port           Port(Socket has precendence)
+  -P , --port           Port (Socket has precedence)
   -S , --socket         Socket file
   --config-file         Dolphie's config file to use. Options are read from these files in the given order: /etc/dolphie.cnf, ~/.dolphie.cnf
-  --mycnf-file          MySQL config file path to use. This should use [client] section [default: ~/.my.cnf]
+  --mycnf-file          MySQL/MariaDB config file path to use. This should use [client] section [default: ~/.my.cnf]
   -f , --host-cache-file
                         Resolve IPs to hostnames when your DNS is unable to. Each IP/hostname pair should be on its own line using format ip=hostname [default: ~/dolphie_host_cache]
   -q , --host-setup-file
                         Specify location of file that stores the available hosts to use in host setup modal [default: ~/dolphie_hosts]
-  -l , --login-path     Specify login path to use with mysql_config_editor's file ~/.mylogin.cnf for encrypted login credentials. Supercedes config file [default: client]
+  -l , --login-path     Specify login path to use with mysql_config_editor's file ~/.mylogin.cnf for encrypted login credentials. Supersedes config file [default: client]
   -r , --refresh_interval
                         How much time to wait in seconds between each refresh [default: 1]
   -H , --heartbeat-table
                         (MySQL only) If your hosts use pt-heartbeat, specify table in format db.table to use the timestamp it has for replication lag instead of Seconds_Behind_Master from SHOW REPLICA STATUS
   --ssl-mode            Desired security state of the connection to the host. Supports: REQUIRED/VERIFY_CA/VERIFY_IDENTITY [default: OFF]
   --ssl-ca              Path to the file that contains a CA (certificate authority)
   --ssl-cert            Path to the file that contains a certificate
@@ -97,15 +97,15 @@
   --pypi-repository     What PyPi repository to use when checking for a new version. If not specified, it will use Dolphie's PyPi repository
   --hostgroup           This is used for creating tabs and connecting to them for hosts you specify in Dolphie's config file under a hostgroup section. As an example, you'll have a section called [cluster1] then below it you will list each host on a new line in the format key=host (keys have no meaning). Hosts support optional port (default is whatever port parameter is) in the format host:port. You can also name the tabs by suffixing ~tab_name to the host (i.e. 1=host~tab_name)
   --show-trxs-only      (MySQL only) Start with only showing threads that have an active transaction
   --additional-columns  Start with additional columns in Processlist panel
   --debug-options       Display options that are set and what they're set by (command-line, dolphie config, etc) then exit
   -V, --version         Display version and exit
 
-MySQL my.cnf file supports these options under [client] section:
+MySQL/MariaDB my.cnf file supports these options under [client] section:
 	host
 	user
 	password
 	port
 	socket
 	ssl_mode REQUIRED/VERIFY_CA/VERIFY_IDENTITY
 	ssl_ca
@@ -146,23 +146,28 @@
 	(str) startup_panels
 	(str) graph_marker
 	(str) pypi_repository
 	(str) hostgroup
 	(bool) show_trxs_only
 	(bool) show_additional_query_columns
 ```
+## Supported ProxySQL versions
+- ProxySQL 2.6+ (could work on previous versions but not tested)
+
+Note: Use `admin` user instead of `stats` user so you can use all features
+
+## Supported MariaDB versions
+- MariaDB 5.5/10.0/11.0+
+- RDS MariaDB
 
 ## Supported MySQL versions
 - MySQL/Percona Server 5.6/5.7/8.0+
-- RDS & Aurora + Azure
-
-## Supported ProxySQL versions
-- ProxySQL 2.6+ (could work on previous versions but not tested)
+- RDS MySQL & Aurora + Azure
 
-## Grants required
+## MySQL Grants required
 #### Least privilege
 1. PROCESS (only if you switch to using processlist via `P` command)
 2. SELECT to `performance_schema` + `pt-heartbeat table` (if used)
 3. REPLICATION CLIENT/REPLICATION SLAVE
 4. BACKUP_ADMIN (MySQL 8 only)
 
 #### Recommended
```

#### html2text {}

```diff
@@ -1,11 +1,11 @@
 # Dolphie
  [https://user-images.githubusercontent.com/13244625/187600748-19d2ad15-42e8-
                           4f9c-ada5-a153cdcf4070.png]
-    Your single pane of glass for real-time analytics into MySQL & ProxySQL
+Your single pane of glass for real-time analytics into MySQL/MariaDB & ProxySQL
 
   [https://github.com/charles-001/dolphie/assets/13244625/88a41290-f52c-4b8e-
   97f8-3b7ef5096eae][https://github.com/charles-001/dolphie/assets/13244625/
  1d94502a-9abf-4436-a7d0-cb2b08c105c1][https://github.com/charles-001/dolphie/
              assets/13244625/9b1aadc8-cabb-4256-92f9-fe4d04451b83]
                                _[_B_u_y_ _M_e_ _A_ _C_o_f_f_e_e_]
 ![Untitled](https://github.com/charles-001/dolphie/assets/13244625/d1292ddc-
@@ -27,25 +27,25 @@
 dolphie:latest $ docker run -dit --name dolphie ghcr.io/charles-001/dolphie:
 latest $ docker exec -it dolphie dolphie -h host.docker.internal -u root --ask-
 pass ``` ## Usage ``` positional arguments: uri Use a URI string for
 credentials (mysql/proxysql) - format: mysql://user:password@host:port (port is
 optional with default 3306, or 6032 for ProxySQL) options: --help show this
 help message and exit --host-setup Start Dolphie by showing the Host Setup
 modal instead of automatically connecting -u , --user Username -p , --password
-Password -h , --host Hostname/IP address -P , --port Port(Socket has
-precendence) -S , --socket Socket file --config-file Dolphie's config file to
+Password -h , --host Hostname/IP address -P , --port Port (Socket has
+precedence) -S , --socket Socket file --config-file Dolphie's config file to
 use. Options are read from these files in the given order: /etc/dolphie.cnf,
-~/.dolphie.cnf --mycnf-file MySQL config file path to use. This should use
-[client] section [default: ~/.my.cnf] -f , --host-cache-file Resolve IPs to
+~/.dolphie.cnf --mycnf-file MySQL/MariaDB config file path to use. This should
+use [client] section [default: ~/.my.cnf] -f , --host-cache-file Resolve IPs to
 hostnames when your DNS is unable to. Each IP/hostname pair should be on its
 own line using format ip=hostname [default: ~/dolphie_host_cache] -q , --host-
 setup-file Specify location of file that stores the available hosts to use in
 host setup modal [default: ~/dolphie_hosts] -l , --login-path Specify login
 path to use with mysql_config_editor's file ~/.mylogin.cnf for encrypted login
-credentials. Supercedes config file [default: client] -r , --refresh_interval
+credentials. Supersedes config file [default: client] -r , --refresh_interval
 How much time to wait in seconds between each refresh [default: 1] -H , --
 heartbeat-table (MySQL only) If your hosts use pt-heartbeat, specify table in
 format db.table to use the timestamp it has for replication lag instead of
 Seconds_Behind_Master from SHOW REPLICA STATUS --ssl-mode Desired security
 state of the connection to the host. Supports: REQUIRED/VERIFY_CA/
 VERIFY_IDENTITY [default: OFF] --ssl-ca Path to the file that contains a CA
 (certificate authority) --ssl-cert Path to the file that contains a certificate
@@ -61,61 +61,64 @@
 called [cluster1] then below it you will list each host on a new line in the
 format key=host (keys have no meaning). Hosts support optional port (default is
 whatever port parameter is) in the format host:port. You can also name the tabs
 by suffixing ~tab_name to the host (i.e. 1=host~tab_name) --show-trxs-only
 (MySQL only) Start with only showing threads that have an active transaction --
 additional-columns Start with additional columns in Processlist panel --debug-
 options Display options that are set and what they're set by (command-line,
-dolphie config, etc) then exit -V, --version Display version and exit MySQL
-my.cnf file supports these options under [client] section: host user password
-port socket ssl_mode REQUIRED/VERIFY_CA/VERIFY_IDENTITY ssl_ca ssl_cert ssl_key
-Login path file supports these options: host user password port socket
-Environment variables support these options: DOLPHIE_USER DOLPHIE_PASSWORD
-DOLPHIE_HOST DOLPHIE_PORT DOLPHIE_SOCKET Dolphie's config supports these
-options under [dolphie] section: (bool) host_setup (str) user (str) password
-(str) host (int) port (str) socket (str) ssl_mode (str) ssl_ca (str) ssl_cert
-(str) ssl_key (str) mycnf_file (str) login_path (str) host_cache_file (str)
-host_setup_file (int) refresh_interval (str) heartbeat_table (str)
-startup_panels (str) graph_marker (str) pypi_repository (str) hostgroup (bool)
-show_trxs_only (bool) show_additional_query_columns ``` ## Supported MySQL
-versions - MySQL/Percona Server 5.6/5.7/8.0+ - RDS & Aurora + Azure ##
-Supported ProxySQL versions - ProxySQL 2.6+ (could work on previous versions
-but not tested) ## Grants required #### Least privilege 1. PROCESS (only if you
-switch to using processlist via `P` command) 2. SELECT to `performance_schema`
-+ `pt-heartbeat table` (if used) 3. REPLICATION CLIENT/REPLICATION SLAVE 4.
-BACKUP_ADMIN (MySQL 8 only) #### Recommended 1. PROCESS (only if you switch to
-using processlist via `P` command) 2. Global SELECT access (good for explaining
-queries, listing all databases, etc) 4. REPLICATION CLIENT/REPLICATION SLAVE 5.
-SUPER (required if you want to kill queries) 6. BACKUP_ADMIN (MySQL 8 only) ##
-Features - Tabs docked at the top to seamlessly switch between connected hosts
-- Hostgroups to make it easy for connecting to multiple hosts at once - Dolphie
-uses panels to present groups of data. They can all be turned on/off to have a
-view of your database server that you prefer - Graphs for many metrics that can
-give you great insight into how your database is performing - Sparkline to show
-queries per second in a live view - 2 options for finding replica lag in this
-order of precedence: - `pt-heartbeat table` (specified by `--heartbeat-table`)
-- `SHOW SLAVE STATUS` - Keeps a history of the servers you connect to that
-provides autocompletion for hostnames in the Host Setup modal - Host cache
-file. This provides users a way to specify hostnames for IPs when their
-network's DNS can't resolve them. An example use case for this is when you
-connect to your work's VPN and DNS isn't available to resolve IPs. In my
-opinion, it's a lot easier to look at hostnames than IPs! - Supports encrypted
-login credentials via `mysql_config_editor` - Automatic conversion of large
-numbers & bytes to human-readable - Notifies when new version is available -
-Many commands at your fingertips with autocompletion for their input ##
-Hostgroups Hostgroups are a way to easily connect to multiple hosts at once. To
-set this up, you will create a section in Dolphie's config file with the name
-you want the hostgroup to be and list each host on a new line in the format
-`key=host` (keys have no meaning). Hosts support optional port (default is
-whatever `port` parameter is) in the format `host:port`. You can also name the
-tabs by suffixing `~tab_name` to the host. Once ready, you will use the
-parameter `hostgroup` or `Host Setup` modal to see it in action! Note: Colors
-can be used in the tab name by using the format `[color]text[/color]` (i.e. `
-[red]production[/red]`). You can also use emojis supported by Rich (can see
-them by running `python -m rich.emoji`) by using the format `:emoji:` (i.e. `:
-ghost:`). Rich supports the normal emoji shortcodes. Example: ```ini [cluster1]
-1=host1 2=host2:3307 3=host3:3308~[red]production[/red] :ghost: ``` ## Things
-to note Order of precedence for methods that pass options to Dolphie: 1.
-Command-line 2. Environment variables 3. Dolphie's config (set by `--config-
-file`) 4. ~/.mylogin.cnf (`mysql_config_editor`) 5. ~/.my.cnf (set by `--mycnf-
-file`) ## Feedback I welcome all questions, bug reports, and requests. If you
-enjoy Dolphie, please let me know! I'd love to hear from you :smiley:
+dolphie config, etc) then exit -V, --version Display version and exit MySQL/
+MariaDB my.cnf file supports these options under [client] section: host user
+password port socket ssl_mode REQUIRED/VERIFY_CA/VERIFY_IDENTITY ssl_ca
+ssl_cert ssl_key Login path file supports these options: host user password
+port socket Environment variables support these options: DOLPHIE_USER
+DOLPHIE_PASSWORD DOLPHIE_HOST DOLPHIE_PORT DOLPHIE_SOCKET Dolphie's config
+supports these options under [dolphie] section: (bool) host_setup (str) user
+(str) password (str) host (int) port (str) socket (str) ssl_mode (str) ssl_ca
+(str) ssl_cert (str) ssl_key (str) mycnf_file (str) login_path (str)
+host_cache_file (str) host_setup_file (int) refresh_interval (str)
+heartbeat_table (str) startup_panels (str) graph_marker (str) pypi_repository
+(str) hostgroup (bool) show_trxs_only (bool) show_additional_query_columns ```
+## Supported ProxySQL versions - ProxySQL 2.6+ (could work on previous versions
+but not tested) Note: Use `admin` user instead of `stats` user so you can use
+all features ## Supported MariaDB versions - MariaDB 5.5/10.0/11.0+ - RDS
+MariaDB ## Supported MySQL versions - MySQL/Percona Server 5.6/5.7/8.0+ - RDS
+MySQL & Aurora + Azure ## MySQL Grants required #### Least privilege 1. PROCESS
+(only if you switch to using processlist via `P` command) 2. SELECT to
+`performance_schema` + `pt-heartbeat table` (if used) 3. REPLICATION CLIENT/
+REPLICATION SLAVE 4. BACKUP_ADMIN (MySQL 8 only) #### Recommended 1. PROCESS
+(only if you switch to using processlist via `P` command) 2. Global SELECT
+access (good for explaining queries, listing all databases, etc) 4. REPLICATION
+CLIENT/REPLICATION SLAVE 5. SUPER (required if you want to kill queries) 6.
+BACKUP_ADMIN (MySQL 8 only) ## Features - Tabs docked at the top to seamlessly
+switch between connected hosts - Hostgroups to make it easy for connecting to
+multiple hosts at once - Dolphie uses panels to present groups of data. They
+can all be turned on/off to have a view of your database server that you prefer
+- Graphs for many metrics that can give you great insight into how your
+database is performing - Sparkline to show queries per second in a live view -
+2 options for finding replica lag in this order of precedence: - `pt-heartbeat
+table` (specified by `--heartbeat-table`) - `SHOW SLAVE STATUS` - Keeps a
+history of the servers you connect to that provides autocompletion for
+hostnames in the Host Setup modal - Host cache file. This provides users a way
+to specify hostnames for IPs when their network's DNS can't resolve them. An
+example use case for this is when you connect to your work's VPN and DNS isn't
+available to resolve IPs. In my opinion, it's a lot easier to look at hostnames
+than IPs! - Supports encrypted login credentials via `mysql_config_editor` -
+Automatic conversion of large numbers & bytes to human-readable - Notifies when
+new version is available - Many commands at your fingertips with autocompletion
+for their input ## Hostgroups Hostgroups are a way to easily connect to
+multiple hosts at once. To set this up, you will create a section in Dolphie's
+config file with the name you want the hostgroup to be and list each host on a
+new line in the format `key=host` (keys have no meaning). Hosts support
+optional port (default is whatever `port` parameter is) in the format `host:
+port`. You can also name the tabs by suffixing `~tab_name` to the host. Once
+ready, you will use the parameter `hostgroup` or `Host Setup` modal to see it
+in action! Note: Colors can be used in the tab name by using the format `
+[color]text[/color]` (i.e. `[red]production[/red]`). You can also use emojis
+supported by Rich (can see them by running `python -m rich.emoji`) by using the
+format `:emoji:` (i.e. `:ghost:`). Rich supports the normal emoji shortcodes.
+Example: ```ini [cluster1] 1=host1 2=host2:3307 3=host3:3308~[red]production[/
+red] :ghost: ``` ## Things to note Order of precedence for methods that pass
+options to Dolphie: 1. Command-line 2. Environment variables 3. Dolphie's
+config (set by `--config-file`) 4. ~/.mylogin.cnf (`mysql_config_editor`) 5.
+~/.my.cnf (set by `--mycnf-file`) ## Feedback I welcome all questions, bug
+reports, and requests. If you enjoy Dolphie, please let me know! I'd love to
+hear from you :smiley:
```

### Comparing `dolphie-5.0.0/dolphie/DataTypes.py` & `dolphie-5.0.1/dolphie/DataTypes.py`

 * *Files identical despite different names*

### Comparing `dolphie-5.0.0/dolphie/Dolphie.css` & `dolphie-5.0.1/dolphie/Dolphie.css`

 * *Files identical despite different names*

### Comparing `dolphie-5.0.0/dolphie/Modules/ArgumentParser.py` & `dolphie-5.0.1/dolphie/Modules/ArgumentParser.py`

 * *Files 0% similar despite different names*

```diff
@@ -151,15 +151,15 @@
             metavar="",
         )
         self.parser.add_argument(
             "-P",
             "--port",
             dest="port",
             type=int,
-            help="Port (socket has precendence)",
+            help="Port (socket has precedence)",
             metavar="",
         )
         self.parser.add_argument(
             "-S",
             "--socket",
             dest="socket",
             type=str,
```

### Comparing `dolphie-5.0.0/dolphie/Modules/Functions.py` & `dolphie-5.0.1/dolphie/Modules/Functions.py`

 * *Files identical despite different names*

### Comparing `dolphie-5.0.0/dolphie/Modules/ManualException.py` & `dolphie-5.0.1/dolphie/Modules/ManualException.py`

 * *Files identical despite different names*

### Comparing `dolphie-5.0.0/dolphie/Modules/MetricManager.py` & `dolphie-5.0.1/dolphie/Modules/MetricManager.py`

 * *Files identical despite different names*

### Comparing `dolphie-5.0.0/dolphie/Modules/MySQL.py` & `dolphie-5.0.1/dolphie/Modules/MySQL.py`

 * *Files 2% similar despite different names*

```diff
@@ -31,15 +31,14 @@
         self.socket = socket
         self.port = port
         self.ssl = ssl
         self.save_connection_id = save_connection_id
 
         self.max_reconnect_attempts: int = 3
         self.running_query: bool = False
-        self.using_ssl: str = None
         self.source: ConnectionSource = None
 
         if auto_connect:
             self.connect()
 
     def connect(self):
         try:
@@ -64,21 +63,18 @@
             except Exception:
                 self.source = ConnectionSource.mysql
 
             # Get connection ID for processlist filtering
             if self.save_connection_id:
                 self.connection_id = self.connection.thread_id()
 
-            # Determine if SSL is being used
-            self.using_ssl = (
-                "ON"
-                if self.source == ConnectionSource.mysql
-                and self.fetch_value_from_field("SHOW STATUS LIKE 'Ssl_cipher'", "Value")
-                else "OFF"
-            )
+            # We don't want any SQL modes to be set to avoid unexpected behavior between MySQL & MariaDB
+            if self.source == ConnectionSource.mysql:
+                self.execute("SET SESSION sql_mode=''")
+
         except pymysql.Error as e:
             if len(e.args) == 1:
                 raise ManualException(e.args[0])
             else:
                 raise ManualException(e.args[1])
         except FileNotFoundError:  # Catch SSL file path errors
             raise ManualException("SSL certificate file path isn't valid!")
```

### Comparing `dolphie-5.0.0/dolphie/Modules/Queries.py` & `dolphie-5.0.1/dolphie/Modules/Queries.py`

 * *Files 9% similar despite different names*

```diff
@@ -240,30 +240,22 @@
             information_schema.PROCESSLIST
         WHERE
             Command Like 'Binlog Dump%'
     """
     ps_user_statisitics: str = """
         SELECT
             u.user AS user,
-            ANY_VALUE(total_connections) AS total_connections,
-            ANY_VALUE(current_connections) AS current_connections,
+            total_connections AS total_connections,
+            current_connections AS current_connections,
             CONVERT(SUM(sum_rows_affected), UNSIGNED) AS rows_affected,
             CONVERT(SUM(sum_rows_sent), UNSIGNED) AS rows_sent,
             CONVERT(SUM(sum_rows_examined), UNSIGNED) AS rows_examined,
             CONVERT(SUM(sum_created_tmp_disk_tables), UNSIGNED) AS created_tmp_disk_tables,
             CONVERT(SUM(sum_created_tmp_tables), UNSIGNED) AS created_tmp_tables,
-            ANY_VALUE(plugin) AS plugin,
-            ANY_VALUE(CASE
-                WHEN (password_lifetime IS NULL OR password_lifetime = 0) AND @@default_password_lifetime = 0 THEN "N/A"
-                ELSE CONCAT(
-                    CAST(IFNULL(password_lifetime, @@default_password_lifetime) as signed) +
-                    CAST(DATEDIFF(password_last_changed, NOW()) as signed),
-                    " days"
-                )
-            END) AS password_expires_in
+            plugin AS plugin
         FROM
             performance_schema.users u
             JOIN performance_schema.events_statements_summary_by_user_by_event_name ess ON u.user = ess.user
             JOIN mysql.user mysql_user ON mysql_user.user = u.user
         WHERE
             current_connections != 0
         GROUP BY
@@ -304,47 +296,47 @@
             t.processlist_id = $1
         ORDER BY
             ATTR_NAME
     """
     ddls: str = """
         SELECT
             t.processlist_id,
-            ANY_VALUE(stmt.sql_text) AS sql_text,
-            ANY_VALUE(stage.event_name) AS state,
-            ANY_VALUE(CONCAT(ROUND(100 * stage.work_completed / stage.work_estimated, 2), "%")) AS percentage_completed,
-            ANY_VALUE(stmt.timer_wait) AS started_ago,
-            ANY_VALUE(CONVERT(stmt.timer_wait / ROUND(100 * stage.work_completed / stage.work_estimated, 2) * 100,
-                UNSIGNED)) AS estimated_full_time,
-            ANY_VALUE(CONVERT((stmt.timer_wait / ROUND(100 * stage.work_completed / stage.work_estimated, 2) * 100)
-                - stmt.timer_wait, UNSIGNED)) AS estimated_remaining_time,
+            stmt.sql_text AS sql_text,
+            stage.event_name AS state,
+            CONCAT(ROUND(100 * stage.work_completed / stage.work_estimated, 2), "%") AS percentage_completed,
+            stmt.timer_wait AS started_ago,
+            CONVERT(stmt.timer_wait / ROUND(100 * stage.work_completed / stage.work_estimated, 2) * 100,
+                UNSIGNED) AS estimated_full_time,
+            CONVERT((stmt.timer_wait / ROUND(100 * stage.work_completed / stage.work_estimated, 2) * 100)
+                - stmt.timer_wait, UNSIGNED) AS estimated_remaining_time,
             CONVERT(SUM(`mt`.`CURRENT_NUMBER_OF_BYTES_USED`), UNSIGNED) AS memory
         FROM
             `performance_schema`.`events_statements_current` stmt JOIN
             `performance_schema`.`events_stages_current` stage ON stage.nesting_event_id = stmt.event_id JOIN
             `performance_schema`.`memory_summary_by_thread_by_event_name` `mt` ON `mt`.thread_id = stmt.thread_id JOIN
             `performance_schema`.`threads` t ON t.thread_id = stmt.thread_id
         WHERE
             stage.event_name LIKE 'stage/innodb/alter%'
         GROUP BY
             t.processlist_id
     """
     metadata_locks: str = """
         SELECT
-            ANY_VALUE(OBJECT_INSTANCE_BEGIN) AS id,
+            OBJECT_INSTANCE_BEGIN AS id,
             OBJECT_TYPE,
-            ANY_VALUE(OBJECT_SCHEMA) AS OBJECT_SCHEMA,
+            OBJECT_SCHEMA AS OBJECT_SCHEMA,
             GROUP_CONCAT(OBJECT_NAME ORDER BY OBJECT_NAME) AS OBJECT_NAME,
             LOCK_TYPE,
             LOCK_STATUS,
-            ANY_VALUE(SOURCE) AS CODE_SOURCE,
-            ANY_VALUE(NAME) AS THREAD_SOURCE,
-            ANY_VALUE(PROCESSLIST_ID) AS PROCESSLIST_ID,
-            ANY_VALUE(PROCESSLIST_USER) AS PROCESSLIST_USER,
-            ANY_VALUE(PROCESSLIST_TIME) AS PROCESSLIST_TIME,
-            ANY_VALUE(PROCESSLIST_INFO) AS PROCESSLIST_INFO
+            SOURCE AS CODE_SOURCE,
+            NAME AS THREAD_SOURCE,
+            PROCESSLIST_ID AS PROCESSLIST_ID,
+            PROCESSLIST_USER AS PROCESSLIST_USER,
+            PROCESSLIST_TIME AS PROCESSLIST_TIME,
+            PROCESSLIST_INFO AS PROCESSLIST_INFO
         FROM
             `performance_schema`.`metadata_locks` mlb JOIN
             `performance_schema`.`threads` t ON mlb.OWNER_THREAD_ID = t.THREAD_ID
         WHERE
             NOT (
                 OBJECT_TYPE = 'TABLE' AND
                 LOCK_STATUS = 'GRANTED' AND
```

### Comparing `dolphie-5.0.0/dolphie/Modules/TabManager.py` & `dolphie-5.0.1/dolphie/Modules/TabManager.py`

 * *Files identical despite different names*

### Comparing `dolphie-5.0.0/dolphie/Panels/dashboard_panel.py` & `dolphie-5.0.1/dolphie/Panels/dashboard_panel.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 from datetime import datetime, timedelta
 
 from dolphie.Modules.Functions import format_bytes, format_number
 from dolphie.Modules.MetricManager import MetricData
+from dolphie.Modules.MySQL import ConnectionSource
 from dolphie.Modules.TabManager import Tab
 from dolphie.Panels import replication_panel
 from rich.style import Style
 from rich.table import Table
 
 
 def create_panel(tab: Tab) -> Table:
@@ -29,29 +30,32 @@
     elif dolphie.innodb_cluster:
         host_type = "InnoDB Cluster"
     elif dolphie.group_replication:
         host_type = "Group Replication"
     elif dolphie.galera_cluster:
         host_type = "Galera Cluster"
     else:
-        host_type = "MySQL"
+        if dolphie.connection_source_alt == ConnectionSource.mariadb:
+            host_type = "MariaDB"
+        else:
+            host_type = "MySQL"
 
     runtime = str(datetime.now() - dolphie.dolphie_start_time).split(".")[0]
 
     replicas = 0
     if dolphie.replica_manager.available_replicas:
         replicas = len(dolphie.replica_manager.available_replicas)
 
     table_information.add_column()
     table_information.add_column(min_width=25, max_width=27)
     table_information.add_row("[label]Version", f"{dolphie.host_distro} {dolphie.host_version}")
     table_information.add_row(
         "[label]", "%s (%s)" % (global_variables["version_compile_os"], global_variables["version_compile_machine"])
     )
-    table_information.add_row("[label]Type", f"{host_type} [label]SSL[/label] {dolphie.main_db_connection.using_ssl}")
+    table_information.add_row("[label]Type", host_type)
     table_information.add_row("[label]Uptime", str(timedelta(seconds=global_status["Uptime"])))
     table_information.add_row("[label]Runtime", f"{runtime} [dark_gray]({dolphie.refresh_latency}s)")
     table_information.add_row("[label]Replicas", "%s" % replicas)
     table_information.add_row(
         "[label]Threads",
         "[label]con[/label] %s[highlight]/[/highlight][label]run[/label]"
         " %s[highlight]/[/highlight][label]cac[/label] %s"
@@ -103,20 +107,17 @@
         innodb_efficiency = f"[{color_code}]{efficiency:.2f}%"
 
     # Add data to our table
     table_innodb.add_row("[label]Read Hit", innodb_efficiency)
     table_innodb.add_row("[label]Chkpt Age", dolphie.metric_manager.get_metric_checkpoint_age(format=True))
     table_innodb.add_row("[label]AHI Hit", dolphie.metric_manager.get_metric_adaptive_hash_index())
 
-    bp_instances = global_variables.get("innodb_buffer_pool_instances", "N/A")
-    if bp_instances != "N/A":
-        plural = "s" if bp_instances > 1 else ""
-        table_innodb.add_row("[label]BP Instance" + plural, format_number(bp_instances))
-    else:
-        table_innodb.add_row("[label]BP Instance", bp_instances)
+    bp_instances = global_variables.get("innodb_buffer_pool_instances", 1)
+    plural = "s" if bp_instances > 1 else ""
+    table_innodb.add_row(f"[label]BP Instance{plural}", format_number(bp_instances))
 
     table_innodb.add_row("[label]BP Size", format_bytes(global_variables["innodb_buffer_pool_size"]))
     table_innodb.add_row(
         "[label]BP Available",
         format_bytes(
             dolphie.global_variables["innodb_buffer_pool_size"] - dolphie.global_status["Innodb_buffer_pool_bytes_data"]
         ),
@@ -170,26 +171,28 @@
         binlog_row_image = None
         if binlog_format == "ROW":
             binlog_row_image = global_variables.get("binlog_row_image", "N/A")
             table_primary.add_row("[label]Format", "{} ({})".format(binlog_format, binlog_row_image))
         else:
             table_primary.add_row("[label]Format", binlog_format, binlog_row_image)
 
-        gtid_mode = global_variables.get("gtid_mode", "N/A")
-        table_primary.add_row("[label]GTID", gtid_mode)
+        if dolphie.connection_source_alt == ConnectionSource.mariadb:
+            table_primary.add_row("[label]Encrypt", global_variables.get("encrypt_binlog", "N/A"))
+        else:
+            table_primary.add_row("[label]GTID", global_variables.get("gtid_mode", "N/A"))
 
-        binlog_compression = global_variables.get("binlog_transaction_compression", "N/A")
-        # binlog_compression_percentage = ""
-        # if binlog_compression == "ON":
-        #     if dolphie.binlog_transaction_compression_percentage:
-        #         binlog_compression_percentage = f" ({dolphie.binlog_transaction_compression_percentage}% gain)"
-        #     else:
-        #         binlog_compression_percentage = " (N/A gain)"
+            binlog_compression = global_variables.get("binlog_transaction_compression", "N/A")
+            # binlog_compression_percentage = ""
+            # if binlog_compression == "ON":
+            #     if dolphie.binlog_transaction_compression_percentage:
+            #         binlog_compression_percentage = f" ({dolphie.binlog_transaction_compression_percentage}% gain)"
+            #     else:
+            #         binlog_compression_percentage = " (N/A gain)"
 
-        table_primary.add_row("[label]Compression", binlog_compression)
+            table_primary.add_row("[label]Compression", binlog_compression)
 
         # Save some global_variables to be used in next refresh
         if dolphie.binlog_status:
             dolphie.previous_binlog_position = dolphie.binlog_status["Position"]
 
     tab.dashboard_section_3.update(table_primary)
```

### Comparing `dolphie-5.0.0/dolphie/Panels/ddl_panel.py` & `dolphie-5.0.1/dolphie/Panels/ddl_panel.py`

 * *Files identical despite different names*

### Comparing `dolphie-5.0.0/dolphie/Panels/innodb_trx_locks_panel.py` & `dolphie-5.0.1/dolphie/Panels/innodb_trx_locks_panel.py`

 * *Files identical despite different names*

### Comparing `dolphie-5.0.0/dolphie/Panels/metadata_locks_panel.py` & `dolphie-5.0.1/dolphie/Panels/metadata_locks_panel.py`

 * *Files identical despite different names*

### Comparing `dolphie-5.0.0/dolphie/Panels/processlist_panel.py` & `dolphie-5.0.1/dolphie/Panels/processlist_panel.py`

 * *Files 2% similar despite different names*

```diff
@@ -9,24 +9,31 @@
 
 
 def create_panel(tab: Tab) -> DataTable:
     dolphie = tab.dolphie
 
     if not dolphie.performance_schema_enabled and dolphie.use_performance_schema:
         dolphie.app.notify(
-            "Performance Schema is not enabled on this host, using Information Schema instead for processlist"
+            "Performance Schema is not enabled on this host, using Information Schema instead for Processlist"
         )
         dolphie.use_performance_schema = False
 
     columns = [
         {"name": "Process ID", "field": "id", "width": None, "format_number": False},
-        {"name": "Protocol", "field": "protocol", "width": 8, "format_number": False},
-        {"name": "Username", "field": "user", "width": 20, "format_number": False},
     ]
 
+    if dolphie.use_performance_schema:
+        columns.extend([{"name": "Protocol", "field": "protocol", "width": 8, "format_number": False}])
+
+    columns.extend(
+        [
+            {"name": "Username", "field": "user", "width": 20, "format_number": False},
+        ]
+    )
+
     if dolphie.show_additional_query_columns:
         columns.extend(
             [
                 {"name": "Hostname/IP", "field": "host", "width": 16, "format_number": False},
                 {"name": "Database", "field": "db", "width": 13, "format_number": False},
             ]
         )
```

### Comparing `dolphie-5.0.0/dolphie/Panels/proxysql_command_stats_panel.py` & `dolphie-5.0.1/dolphie/Panels/proxysql_command_stats_panel.py`

 * *Files identical despite different names*

### Comparing `dolphie-5.0.0/dolphie/Panels/proxysql_dashboard_panel.py` & `dolphie-5.0.1/dolphie/Panels/proxysql_dashboard_panel.py`

 * *Files identical despite different names*

### Comparing `dolphie-5.0.0/dolphie/Panels/proxysql_hostgroup_summary_panel.py` & `dolphie-5.0.1/dolphie/Panels/proxysql_hostgroup_summary_panel.py`

 * *Files identical despite different names*

### Comparing `dolphie-5.0.0/dolphie/Panels/proxysql_mysql_query_rules_panel.py` & `dolphie-5.0.1/dolphie/Panels/proxysql_mysql_query_rules_panel.py`

 * *Files identical despite different names*

### Comparing `dolphie-5.0.0/dolphie/Panels/proxysql_processlist_panel.py` & `dolphie-5.0.1/dolphie/Panels/proxysql_processlist_panel.py`

 * *Files identical despite different names*

### Comparing `dolphie-5.0.0/dolphie/Panels/replication_panel.py` & `dolphie-5.0.1/dolphie/Panels/replication_panel.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 import re
 
-from dolphie.DataTypes import Replica
+from dolphie.DataTypes import ConnectionSource, Replica
 from dolphie.Modules.Functions import format_number, format_time
 from dolphie.Modules.ManualException import ManualException
 from dolphie.Modules.MySQL import Database
 from dolphie.Modules.Queries import MySQLQueries
 from dolphie.Modules.TabManager import Tab
 from rich import box
 from rich.align import Align
@@ -120,27 +120,14 @@
     def create_replication_panel():
         if not dolphie.replication_status:
             tab.replication_container.display = False
             return None
 
         tab.replication_container.display = True
 
-        replication_variables = ""
-        available_replication_variables = {
-            "binlog_transaction_dependency_tracking": "dependency_tracking",
-            "slave_parallel_type": "parallel_type",
-            "slave_parallel_workers": "parallel_workers",
-            "slave_preserve_commit_order": "preserve_commit_order",
-        }
-
-        for setting_variable, setting_display_name in available_replication_variables.items():
-            value = dolphie.global_variables.get(setting_variable, "N/A")
-            replication_variables += f"[b light_blue]{setting_display_name}[/b light_blue] {value}  "
-        replication_variables = replication_variables.strip()
-
         if dolphie.replication_applier_status:
             table_thread_applier_status = Table(box=None, header_style="#c5c7d2")
             table_thread_applier_status.add_column("Worker", justify="center")
             table_thread_applier_status.add_column("Usage", min_width=6)
             table_thread_applier_status.add_column("Apply Time")
             table_thread_applier_status.add_column("Last Applied Transaction")
 
@@ -164,15 +151,38 @@
                 )
 
             tab.replication_thread_applier.update(table_thread_applier_status)
             tab.replication_thread_applier_container.display = True
         else:
             tab.replication_thread_applier_container.display = False
 
+        if tab.dolphie.connection_source_alt == ConnectionSource.mariadb:
+            available_replication_variables = {
+                "gtid_domain_id": "gtid_domain_id",
+                "slave_parallel_mode": "parallel_mode",
+                "slave_parallel_workers": "parallel_workers",
+                "slave_parallel_threads": "parallel_threads",
+                "slave_domain_parallel_threads": "domain_parallel_threads",
+            }
+        else:
+            available_replication_variables = {
+                "binlog_transaction_dependency_tracking": "dependency_tracking",
+                "slave_parallel_type": "parallel_type",
+                "slave_parallel_workers": "parallel_workers",
+                "slave_preserve_commit_order": "preserve_commit_order",
+            }
+
+        replication_variables = ""
+        for setting_variable, setting_display_name in available_replication_variables.items():
+            value = dolphie.global_variables.get(setting_variable, "N/A")
+            replication_variables += f"[b light_blue]{setting_display_name}[/b light_blue] {value}  "
+        replication_variables = replication_variables.strip()
+
         tab.replication_variables.update(replication_variables)
+
         tab.replication_status.update(create_replication_table(tab))
 
     create_replication_panel()
     create_cluster_panel()
     create_group_replication_panel()
```

### Comparing `dolphie-5.0.0/dolphie/Widgets/command_screen.py` & `dolphie-5.0.1/dolphie/Widgets/command_screen.py`

 * *Files identical despite different names*

### Comparing `dolphie-5.0.0/dolphie/Widgets/event_log_screen.py` & `dolphie-5.0.1/dolphie/Widgets/event_log_screen.py`

 * *Files identical despite different names*

### Comparing `dolphie-5.0.0/dolphie/Widgets/help.py` & `dolphie-5.0.1/dolphie/Widgets/help.py`

 * *Files 0% similar despite different names*

```diff
@@ -55,27 +55,27 @@
             "=": "Rename the current tab",
             "a": "Toggle additional processlist columns",
             "c": "Clear all filters set",
             "d": "Display all databases",
             "D": "Disconnect from the tab's host",
             "e": "Display error log from Performance Schema",
             "f": "Filter processlist by a supported option",
-            "i": "Toggle displaying idle processs",
+            "i": "Toggle displaying idle process",
             "k": "Kill a process by its ID",
             "K": "Kill a process by a supported option",
             "l": "Display the most recent deadlock",
             "o": "Display output from SHOW ENGINE INNODB STATUS",
             "m": "Display memory usage",
             "p": "Pause refreshing of panels",
             "P": "Switch between using Information Schema/Performance Schema for processlist panel",
             "q": "Quit",
             "r": "Set the refresh interval",
             "R": "Reset all metrics",
             "t": "Display details of a process along with an EXPLAIN of its query",
-            "T": "Transaction view - toggle displaying processs that only have an active transaction",
+            "T": "Transaction view - toggle displaying process that only have an active transaction",
             "s": "Toggle sorting for Age in descending/ascending order",
             "u": "List active connected users and their statistics",
             "v": "Variable wildcard search sourced from SHOW GLOBAL VARIABLES",
             "z": "Display all entries in the host cache",
             "space": "Force a manual refresh of all panels except replicas",
             "ctrl+a": "Switch to the previous tab",
             "ctrl+d": "Switch to the next tab",
@@ -106,15 +106,15 @@
                 "The percentage of how many lookups there are from Adapative Hash Index\ncompared to it not"
                 " being used"
             ),
             "Cache Hit": "The percentage of how many binary log lookups are from cache instead of from disk",
             "History List": "History list length (number of un-purged row changes in InnoDB's undo logs)",
             "QPS": "Queries per second from Com_queries in SHOW GLOBAL STATUS",
             "Latency": "How much time it takes to receive data from the host for each refresh interval",
-            "processs": "Con = Connected, Run = Running, Cac = Cached from SHOW GLOBAL STATUS",
+            "process": "Con = Connected, Run = Running, Cac = Cached from SHOW GLOBAL STATUS",
             "Speed": "How many seconds were taken off of replication lag from the last refresh interval",
             "Tickets": "Relates to innodb_concurrency_tickets variable",
             "R-Lock/Mod": "Relates to how many rows are locked/modified for the process's transaction",
             "GR": "Group Replication",
         }
 
         table_terminology = Table(
@@ -144,15 +144,15 @@
             "-": "Remove the current tab",
             "=": "Rename the current tab",
             "a": "Toggle additional processlist/query rule columns",
             "c": "Clear all filters set",
             "D": "Disconnect from the tab's host",
             "e": "Display errors reported by backend servers during query execution",
             "f": "Filter processlist by a supported option",
-            "i": "Toggle displaying idle processs",
+            "i": "Toggle displaying idle process",
             "k": "Kill a process by its ID",
             "K": "Kill a process by a supported option",
             "m": "Display memory usage",
             "p": "Pause refreshing of panels",
             "q": "Quit",
             "r": "Set the refresh interval",
             "R": "Reset all metrics",
```

### Comparing `dolphie-5.0.0/dolphie/Widgets/host_setup.py` & `dolphie-5.0.1/dolphie/Widgets/host_setup.py`

 * *Files identical despite different names*

### Comparing `dolphie-5.0.0/dolphie/Widgets/modal.py` & `dolphie-5.0.1/dolphie/Widgets/modal.py`

 * *Files identical despite different names*

### Comparing `dolphie-5.0.0/dolphie/Widgets/proxysql_thread_screen.py` & `dolphie-5.0.1/dolphie/Widgets/proxysql_thread_screen.py`

 * *Files identical despite different names*

### Comparing `dolphie-5.0.0/dolphie/Widgets/spinner.py` & `dolphie-5.0.1/dolphie/Widgets/spinner.py`

 * *Files identical despite different names*

### Comparing `dolphie-5.0.0/dolphie/Widgets/thread_screen.py` & `dolphie-5.0.1/dolphie/Widgets/thread_screen.py`

 * *Files identical despite different names*

### Comparing `dolphie-5.0.0/dolphie/Widgets/topbar.py` & `dolphie-5.0.1/dolphie/Widgets/topbar.py`

 * *Files identical despite different names*

### Comparing `dolphie-5.0.0/dolphie/__init__.py` & `dolphie-5.0.1/dolphie/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -175,27 +175,27 @@
         # Get proper host version and fork
         if "percona xtradb cluster" in version_comment:
             self.host_distro = "Percona XtraDB Cluster"
         elif "percona server" in version_comment:
             self.host_distro = "Percona Server"
         elif "mariadb cluster" in version_comment:
             self.host_distro = "MariaDB Cluster"
-            self.connection_source_alt == ConnectionSource.mariadb
+            self.connection_source_alt = ConnectionSource.mariadb
         elif "mariadb" in version_comment or "mariadb" in version:
             self.host_distro = "MariaDB"
-            self.connection_source_alt == ConnectionSource.mariadb
+            self.connection_source_alt = ConnectionSource.mariadb
         elif aurora_version:
             self.host_distro = "Amazon Aurora"
-            self.connection_source_alt == ConnectionSource.aws_rds
+            self.connection_source_alt = ConnectionSource.aws_rds
         elif "rdsdb" in basedir:
             self.host_distro = "Amazon RDS"
-            self.connection_source_alt == ConnectionSource.aws_rds
+            self.connection_source_alt = ConnectionSource.aws_rds
         elif global_variables.get("aad_auth_only"):
             self.host_distro = "Azure MySQL"
-            self.connection_source_alt == ConnectionSource.azure_mysql
+            self.connection_source_alt = ConnectionSource.azure_mysql
         else:
             self.host_distro = "MySQL"
 
         # For RDS and Azure, we will use the host specified to connect with since hostname isn't related to the endpoint
         if self.connection_source_alt == ConnectionSource.aws_rds:
             self.host_with_port = f"{self.host.split('.rds.amazonaws.com')[0]}:{self.port}"
         elif self.connection_source_alt == ConnectionSource.azure_mysql:
@@ -208,16 +208,15 @@
         if self.connection_source_alt == ConnectionSource.mariadb and major_version >= 10:
             self.server_uuid = global_variables.get("server_id")
 
         if global_variables.get("performance_schema") == "ON":
             self.performance_schema_enabled = True
 
         # Check to see if the host is in a Galera cluster
-        galera_matches = any(key.startswith("wsrep_") for key in global_variables.keys())
-        if galera_matches:
+        if global_variables.get("wsrep_on") == "ON" or global_variables.get("wsrep_cluster_address"):
             self.galera_cluster = True
 
         # Check to get information on what cluster type it is
         if self.is_mysql_version_at_least("8.1"):
             query = MySQLQueries.determine_cluster_type_81
         else:
             query = MySQLQueries.determine_cluster_type_8
```

### Comparing `dolphie-5.0.0/dolphie/app.py` & `dolphie-5.0.1/dolphie/app.py`

 * *Files 0% similar despite different names*

```diff
@@ -387,25 +387,29 @@
 
         # Add the total queries to the global status
         dolphie.global_status["Queries"] = total_queries_count
 
         dolphie.main_db_connection.execute(ProxySQLQueries.connection_pool_data)
         data = dolphie.main_db_connection.fetchone()
         dolphie.global_status["proxysql_backend_host_average_latency"] = int(data.get("avg_latency", 0))
-        dolphie.global_status["proxysql_multiplex_efficiency_ratio"] = round(
-            100
-            - (
-                (
-                    int(data.get("connection_pool_connections", 0))
-                    / dolphie.global_status.get("Client_Connections_connected", 0)
-                )
-                * 100
-            ),
-            2,
-        )
+
+        if dolphie.global_status.get("Client_Connections_connected", 0):  # Don't divide by 0
+            dolphie.global_status["proxysql_multiplex_efficiency_ratio"] = round(
+                100
+                - (
+                    (
+                        int(data.get("connection_pool_connections", 0))
+                        / dolphie.global_status.get("Client_Connections_connected", 0)
+                    )
+                    * 100
+                ),
+                2,
+            )
+        else:
+            dolphie.global_status["proxysql_multiplex_efficiency_ratio"] = 100
 
         if dolphie.panels.proxysql_hostgroup_summary.visible:
             dolphie.main_db_connection.execute(ProxySQLQueries.hostgroup_summary)
             dolphie.proxysql_hostgroup_summary = dolphie.main_db_connection.fetchall()
 
         if dolphie.panels.processlist.visible:
             dolphie.processlist_threads = proxysql_processlist_panel.fetch_data(tab)
@@ -812,41 +816,42 @@
             )
 
             dolphie.secondary_db_connection.execute(query)
             row = dolphie.secondary_db_connection.fetchone()
             if row and row.get("enabled") == "NO":
                 self.notify(
                     "Metadata Locks panel requires Performance Schema to have"
-                    " [highlight]wait/lock/metadata/sql/mdl[/highlight] enabled"
+                    " [highlight]wait/lock/metadata/sql/mdl[/highlight] enabled in setup_instruments table"
                 )
                 return
 
             self.toggle_panel(dolphie.panels.metadata_locks.name)
             self.tab_manager.active_tab.metadata_locks_datatable.clear()
             tab.metadata_locks_title.update("Metadata Locks ([highlight]0[/highlight])")
         elif key == "6":
             if dolphie.connection_source == ConnectionSource.proxysql:
                 self.toggle_panel(dolphie.panels.proxysql_command_stats.name)
-                return
-
-            if not dolphie.is_mysql_version_at_least("5.7") or not dolphie.performance_schema_enabled:
-                self.notify("DDL panel requires MySQL 5.7+ with Performance Schema enabled")
-                return
-
-            query = "SELECT enabled FROM performance_schema.setup_instruments WHERE name LIKE 'stage/innodb/alter%';"
-            dolphie.secondary_db_connection.execute(query)
-            data = dolphie.secondary_db_connection.fetchall()
-            for row in data:
-                if row.get("enabled") == "NO":
-                    self.notify("DDL panel requires Performance Schema to have 'stage/innodb/alter%' enabled")
+            else:
+                if not dolphie.is_mysql_version_at_least("5.7") or not dolphie.performance_schema_enabled:
+                    self.notify("DDL panel requires MySQL 5.7+ with Performance Schema enabled")
                     return
 
-            self.toggle_panel(dolphie.panels.ddl.name)
-            self.tab_manager.active_tab.ddl_datatable.clear()
-            tab.ddl_title.update("DDL ([highlight]0[/highlight])")
+                query = (
+                    "SELECT enabled FROM performance_schema.setup_instruments WHERE name LIKE 'stage/innodb/alter%';"
+                )
+                dolphie.secondary_db_connection.execute(query)
+                data = dolphie.secondary_db_connection.fetchall()
+                for row in data:
+                    if row.get("enabled") == "NO":
+                        self.notify("DDL panel requires Performance Schema to have 'stage/innodb/alter%' enabled")
+                        return
+
+                self.toggle_panel(dolphie.panels.ddl.name)
+                self.tab_manager.active_tab.ddl_datatable.clear()
+                tab.ddl_title.update("DDL ([highlight]0[/highlight])")
         elif key == "grave_accent":
             self.tab_manager.setup_host_tab(tab)
         elif key == "space":
             if tab.worker.state != WorkerState.RUNNING:
                 tab.worker_timer.stop()
                 self.run_worker_main(tab.id)
         elif key == "plus":
@@ -907,29 +912,30 @@
 
             self.run_command_in_worker(key=key, dolphie=dolphie)
 
         elif key == "D":
             await self.tab_manager.disconnect_tab(tab)
 
         elif key == "e":
-            if dolphie.connection_source == ConnectionSource.proxysql:
+            if dolphie.connection_source_alt == ConnectionSource.mariadb:
+                self.notify(f"Command [highlight]{key}[/highlight] is only available for MySQL connections")
+            elif dolphie.connection_source == ConnectionSource.proxysql:
                 self.run_command_in_worker(key=key, dolphie=dolphie)
-                return
-
-            if dolphie.is_mysql_version_at_least("8.0") and dolphie.performance_schema_enabled:
-                self.app.push_screen(
-                    EventLog(
-                        dolphie.connection_status,
-                        dolphie.app_version,
-                        dolphie.host_with_port,
-                        dolphie.secondary_db_connection,
-                    )
-                )
             else:
-                self.notify("Error log command requires MySQL 8+ with Performance Schema enabled")
+                if dolphie.is_mysql_version_at_least("8.0") and dolphie.performance_schema_enabled:
+                    self.app.push_screen(
+                        EventLog(
+                            dolphie.connection_status,
+                            dolphie.app_version,
+                            dolphie.host_with_port,
+                            dolphie.secondary_db_connection,
+                        )
+                    )
+                else:
+                    self.notify("Error log command requires MySQL 8+ with Performance Schema enabled")
 
         elif key == "f":
 
             def command_get_input(filter_data):
                 filter_name, filter_value = filter_data[0], filter_data[1]
                 filters_mapping = {
                     "User": "user_filter",
@@ -1671,15 +1677,14 @@
                         "Total": {"field": "total_connections", "format_number": True},
                         "Rows Read": {"field": "rows_examined", "format_number": True},
                         "Rows Sent": {"field": "rows_sent", "format_number": True},
                         "Rows Updated": {"field": "rows_affected", "format_number": True},
                         "Tmp Tables": {"field": "created_tmp_tables", "format_number": True},
                         "Tmp Disk Tables": {"field": "created_tmp_disk_tables", "format_number": True},
                         "Plugin": {"field": "plugin", "format_number": False},
-                        "Password Expire": {"field": "password_expires_in", "format_number": False},
                     }
 
                     table = Table(
                         header_style="b",
                         box=box.SIMPLE_HEAVY,
                         show_edge=False,
                         style="table_border",
```

### Comparing `dolphie-5.0.0/pyproject.toml` & `dolphie-5.0.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "dolphie"
-version = "5.0.0"
+version = "5.0.1"
 license = "GPL-3.0-or-later"
 description = "Your single pane of glass for real-time analytics into MySQL & ProxySQL"
 authors = ["Charles Thompson <01charles.t@gmail.com>"]
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.8"
```

### Comparing `dolphie-5.0.0/PKG-INFO` & `dolphie-5.0.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dolphie
-Version: 5.0.0
+Version: 5.0.1
 Summary: Your single pane of glass for real-time analytics into MySQL & ProxySQL
 License: GPL-3.0-or-later
 Author: Charles Thompson
 Author-email: 01charles.t@gmail.com
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
 Classifier: Programming Language :: Python :: 3
@@ -23,15 +23,15 @@
 Requires-Dist: textual-autocomplete (>=2.1.0b0,<3.0.0)
 Requires-Dist: textual[syntax] (>=0.57.1,<0.58.0)
 Description-Content-Type: text/markdown
 
 # Dolphie
 <p align="center">
   <img src="https://user-images.githubusercontent.com/13244625/187600748-19d2ad15-42e8-4f9c-ada5-a153cdcf4070.png" width="120"><br>
-  Your single pane of glass for real-time analytics into MySQL & ProxySQL<br><br>
+  Your single pane of glass for real-time analytics into MySQL/MariaDB & ProxySQL<br><br>
   <img src="https://github.com/charles-001/dolphie/assets/13244625/88a41290-f52c-4b8e-97f8-3b7ef5096eae" width="30">
   <img src="https://github.com/charles-001/dolphie/assets/13244625/1d94502a-9abf-4436-a7d0-cb2b08c105c1" width="30">
   <img src="https://github.com/charles-001/dolphie/assets/13244625/9b1aadc8-cabb-4256-92f9-fe4d04451b83" width="30">
 </p>
 <p align="center">
   <a href="https://www.buymeacoffee.com/charlesthompson">
     <img src="https://www.buymeacoffee.com/assets/img/custom_images/orange_img.png" alt="Buy Me A Coffee">
@@ -97,23 +97,23 @@
 
 options:
   --help                show this help message and exit
   --host-setup          Start Dolphie by showing the Host Setup modal instead of automatically connecting
   -u , --user           Username
   -p , --password       Password
   -h , --host           Hostname/IP address
-  -P , --port           Port(Socket has precendence)
+  -P , --port           Port (Socket has precedence)
   -S , --socket         Socket file
   --config-file         Dolphie's config file to use. Options are read from these files in the given order: /etc/dolphie.cnf, ~/.dolphie.cnf
-  --mycnf-file          MySQL config file path to use. This should use [client] section [default: ~/.my.cnf]
+  --mycnf-file          MySQL/MariaDB config file path to use. This should use [client] section [default: ~/.my.cnf]
   -f , --host-cache-file
                         Resolve IPs to hostnames when your DNS is unable to. Each IP/hostname pair should be on its own line using format ip=hostname [default: ~/dolphie_host_cache]
   -q , --host-setup-file
                         Specify location of file that stores the available hosts to use in host setup modal [default: ~/dolphie_hosts]
-  -l , --login-path     Specify login path to use with mysql_config_editor's file ~/.mylogin.cnf for encrypted login credentials. Supercedes config file [default: client]
+  -l , --login-path     Specify login path to use with mysql_config_editor's file ~/.mylogin.cnf for encrypted login credentials. Supersedes config file [default: client]
   -r , --refresh_interval
                         How much time to wait in seconds between each refresh [default: 1]
   -H , --heartbeat-table
                         (MySQL only) If your hosts use pt-heartbeat, specify table in format db.table to use the timestamp it has for replication lag instead of Seconds_Behind_Master from SHOW REPLICA STATUS
   --ssl-mode            Desired security state of the connection to the host. Supports: REQUIRED/VERIFY_CA/VERIFY_IDENTITY [default: OFF]
   --ssl-ca              Path to the file that contains a CA (certificate authority)
   --ssl-cert            Path to the file that contains a certificate
@@ -123,15 +123,15 @@
   --pypi-repository     What PyPi repository to use when checking for a new version. If not specified, it will use Dolphie's PyPi repository
   --hostgroup           This is used for creating tabs and connecting to them for hosts you specify in Dolphie's config file under a hostgroup section. As an example, you'll have a section called [cluster1] then below it you will list each host on a new line in the format key=host (keys have no meaning). Hosts support optional port (default is whatever port parameter is) in the format host:port. You can also name the tabs by suffixing ~tab_name to the host (i.e. 1=host~tab_name)
   --show-trxs-only      (MySQL only) Start with only showing threads that have an active transaction
   --additional-columns  Start with additional columns in Processlist panel
   --debug-options       Display options that are set and what they're set by (command-line, dolphie config, etc) then exit
   -V, --version         Display version and exit
 
-MySQL my.cnf file supports these options under [client] section:
+MySQL/MariaDB my.cnf file supports these options under [client] section:
 	host
 	user
 	password
 	port
 	socket
 	ssl_mode REQUIRED/VERIFY_CA/VERIFY_IDENTITY
 	ssl_ca
@@ -172,23 +172,28 @@
 	(str) startup_panels
 	(str) graph_marker
 	(str) pypi_repository
 	(str) hostgroup
 	(bool) show_trxs_only
 	(bool) show_additional_query_columns
 ```
+## Supported ProxySQL versions
+- ProxySQL 2.6+ (could work on previous versions but not tested)
+
+Note: Use `admin` user instead of `stats` user so you can use all features
+
+## Supported MariaDB versions
+- MariaDB 5.5/10.0/11.0+
+- RDS MariaDB
 
 ## Supported MySQL versions
 - MySQL/Percona Server 5.6/5.7/8.0+
-- RDS & Aurora + Azure
-
-## Supported ProxySQL versions
-- ProxySQL 2.6+ (could work on previous versions but not tested)
+- RDS MySQL & Aurora + Azure
 
-## Grants required
+## MySQL Grants required
 #### Least privilege
 1. PROCESS (only if you switch to using processlist via `P` command)
 2. SELECT to `performance_schema` + `pt-heartbeat table` (if used)
 3. REPLICATION CLIENT/REPLICATION SLAVE
 4. BACKUP_ADMIN (MySQL 8 only)
 
 #### Recommended
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: dolphie Version: 5.0.0 Summary: Your single pane of
+Metadata-Version: 2.1 Name: dolphie Version: 5.0.1 Summary: Your single pane of
 glass for real-time analytics into MySQL & ProxySQL License: GPL-3.0-or-later
 Author: Charles Thompson Author-email: 01charles.t@gmail.com Requires-Python:
 >=3.8,<4.0 Classifier: License :: OSI Approved :: GNU General Public License v3
 or later (GPLv3+) Classifier: Programming Language :: Python :: 3 Classifier:
 Programming Language :: Python :: 3.8 Classifier: Programming Language ::
 Python :: 3.9 Classifier: Programming Language :: Python :: 3.10 Classifier:
 Programming Language :: Python :: 3.11 Requires-Dist: charset-normalizer
@@ -10,15 +10,15 @@
 packaging (>=24.0,<25.0) Requires-Dist: plotext (>=5.2.8,<6.0.0) Requires-Dist:
 pymysql (>=1.1.0,<2.0.0) Requires-Dist: requests (>=2.31.0,<3.0.0) Requires-
 Dist: rich (>=13.7.1,<14.0.0) Requires-Dist: sqlparse (>=0.4.4,<0.5.0)
 Requires-Dist: textual-autocomplete (>=2.1.0b0,<3.0.0) Requires-Dist: textual
 [syntax] (>=0.57.1,<0.58.0) Description-Content-Type: text/markdown # Dolphie
  [https://user-images.githubusercontent.com/13244625/187600748-19d2ad15-42e8-
                           4f9c-ada5-a153cdcf4070.png]
-    Your single pane of glass for real-time analytics into MySQL & ProxySQL
+Your single pane of glass for real-time analytics into MySQL/MariaDB & ProxySQL
 
   [https://github.com/charles-001/dolphie/assets/13244625/88a41290-f52c-4b8e-
   97f8-3b7ef5096eae][https://github.com/charles-001/dolphie/assets/13244625/
  1d94502a-9abf-4436-a7d0-cb2b08c105c1][https://github.com/charles-001/dolphie/
              assets/13244625/9b1aadc8-cabb-4256-92f9-fe4d04451b83]
                                _[_B_u_y_ _M_e_ _A_ _C_o_f_f_e_e_]
 ![Untitled](https://github.com/charles-001/dolphie/assets/13244625/d1292ddc-
@@ -40,25 +40,25 @@
 dolphie:latest $ docker run -dit --name dolphie ghcr.io/charles-001/dolphie:
 latest $ docker exec -it dolphie dolphie -h host.docker.internal -u root --ask-
 pass ``` ## Usage ``` positional arguments: uri Use a URI string for
 credentials (mysql/proxysql) - format: mysql://user:password@host:port (port is
 optional with default 3306, or 6032 for ProxySQL) options: --help show this
 help message and exit --host-setup Start Dolphie by showing the Host Setup
 modal instead of automatically connecting -u , --user Username -p , --password
-Password -h , --host Hostname/IP address -P , --port Port(Socket has
-precendence) -S , --socket Socket file --config-file Dolphie's config file to
+Password -h , --host Hostname/IP address -P , --port Port (Socket has
+precedence) -S , --socket Socket file --config-file Dolphie's config file to
 use. Options are read from these files in the given order: /etc/dolphie.cnf,
-~/.dolphie.cnf --mycnf-file MySQL config file path to use. This should use
-[client] section [default: ~/.my.cnf] -f , --host-cache-file Resolve IPs to
+~/.dolphie.cnf --mycnf-file MySQL/MariaDB config file path to use. This should
+use [client] section [default: ~/.my.cnf] -f , --host-cache-file Resolve IPs to
 hostnames when your DNS is unable to. Each IP/hostname pair should be on its
 own line using format ip=hostname [default: ~/dolphie_host_cache] -q , --host-
 setup-file Specify location of file that stores the available hosts to use in
 host setup modal [default: ~/dolphie_hosts] -l , --login-path Specify login
 path to use with mysql_config_editor's file ~/.mylogin.cnf for encrypted login
-credentials. Supercedes config file [default: client] -r , --refresh_interval
+credentials. Supersedes config file [default: client] -r , --refresh_interval
 How much time to wait in seconds between each refresh [default: 1] -H , --
 heartbeat-table (MySQL only) If your hosts use pt-heartbeat, specify table in
 format db.table to use the timestamp it has for replication lag instead of
 Seconds_Behind_Master from SHOW REPLICA STATUS --ssl-mode Desired security
 state of the connection to the host. Supports: REQUIRED/VERIFY_CA/
 VERIFY_IDENTITY [default: OFF] --ssl-ca Path to the file that contains a CA
 (certificate authority) --ssl-cert Path to the file that contains a certificate
@@ -74,61 +74,64 @@
 called [cluster1] then below it you will list each host on a new line in the
 format key=host (keys have no meaning). Hosts support optional port (default is
 whatever port parameter is) in the format host:port. You can also name the tabs
 by suffixing ~tab_name to the host (i.e. 1=host~tab_name) --show-trxs-only
 (MySQL only) Start with only showing threads that have an active transaction --
 additional-columns Start with additional columns in Processlist panel --debug-
 options Display options that are set and what they're set by (command-line,
-dolphie config, etc) then exit -V, --version Display version and exit MySQL
-my.cnf file supports these options under [client] section: host user password
-port socket ssl_mode REQUIRED/VERIFY_CA/VERIFY_IDENTITY ssl_ca ssl_cert ssl_key
-Login path file supports these options: host user password port socket
-Environment variables support these options: DOLPHIE_USER DOLPHIE_PASSWORD
-DOLPHIE_HOST DOLPHIE_PORT DOLPHIE_SOCKET Dolphie's config supports these
-options under [dolphie] section: (bool) host_setup (str) user (str) password
-(str) host (int) port (str) socket (str) ssl_mode (str) ssl_ca (str) ssl_cert
-(str) ssl_key (str) mycnf_file (str) login_path (str) host_cache_file (str)
-host_setup_file (int) refresh_interval (str) heartbeat_table (str)
-startup_panels (str) graph_marker (str) pypi_repository (str) hostgroup (bool)
-show_trxs_only (bool) show_additional_query_columns ``` ## Supported MySQL
-versions - MySQL/Percona Server 5.6/5.7/8.0+ - RDS & Aurora + Azure ##
-Supported ProxySQL versions - ProxySQL 2.6+ (could work on previous versions
-but not tested) ## Grants required #### Least privilege 1. PROCESS (only if you
-switch to using processlist via `P` command) 2. SELECT to `performance_schema`
-+ `pt-heartbeat table` (if used) 3. REPLICATION CLIENT/REPLICATION SLAVE 4.
-BACKUP_ADMIN (MySQL 8 only) #### Recommended 1. PROCESS (only if you switch to
-using processlist via `P` command) 2. Global SELECT access (good for explaining
-queries, listing all databases, etc) 4. REPLICATION CLIENT/REPLICATION SLAVE 5.
-SUPER (required if you want to kill queries) 6. BACKUP_ADMIN (MySQL 8 only) ##
-Features - Tabs docked at the top to seamlessly switch between connected hosts
-- Hostgroups to make it easy for connecting to multiple hosts at once - Dolphie
-uses panels to present groups of data. They can all be turned on/off to have a
-view of your database server that you prefer - Graphs for many metrics that can
-give you great insight into how your database is performing - Sparkline to show
-queries per second in a live view - 2 options for finding replica lag in this
-order of precedence: - `pt-heartbeat table` (specified by `--heartbeat-table`)
-- `SHOW SLAVE STATUS` - Keeps a history of the servers you connect to that
-provides autocompletion for hostnames in the Host Setup modal - Host cache
-file. This provides users a way to specify hostnames for IPs when their
-network's DNS can't resolve them. An example use case for this is when you
-connect to your work's VPN and DNS isn't available to resolve IPs. In my
-opinion, it's a lot easier to look at hostnames than IPs! - Supports encrypted
-login credentials via `mysql_config_editor` - Automatic conversion of large
-numbers & bytes to human-readable - Notifies when new version is available -
-Many commands at your fingertips with autocompletion for their input ##
-Hostgroups Hostgroups are a way to easily connect to multiple hosts at once. To
-set this up, you will create a section in Dolphie's config file with the name
-you want the hostgroup to be and list each host on a new line in the format
-`key=host` (keys have no meaning). Hosts support optional port (default is
-whatever `port` parameter is) in the format `host:port`. You can also name the
-tabs by suffixing `~tab_name` to the host. Once ready, you will use the
-parameter `hostgroup` or `Host Setup` modal to see it in action! Note: Colors
-can be used in the tab name by using the format `[color]text[/color]` (i.e. `
-[red]production[/red]`). You can also use emojis supported by Rich (can see
-them by running `python -m rich.emoji`) by using the format `:emoji:` (i.e. `:
-ghost:`). Rich supports the normal emoji shortcodes. Example: ```ini [cluster1]
-1=host1 2=host2:3307 3=host3:3308~[red]production[/red] :ghost: ``` ## Things
-to note Order of precedence for methods that pass options to Dolphie: 1.
-Command-line 2. Environment variables 3. Dolphie's config (set by `--config-
-file`) 4. ~/.mylogin.cnf (`mysql_config_editor`) 5. ~/.my.cnf (set by `--mycnf-
-file`) ## Feedback I welcome all questions, bug reports, and requests. If you
-enjoy Dolphie, please let me know! I'd love to hear from you :smiley:
+dolphie config, etc) then exit -V, --version Display version and exit MySQL/
+MariaDB my.cnf file supports these options under [client] section: host user
+password port socket ssl_mode REQUIRED/VERIFY_CA/VERIFY_IDENTITY ssl_ca
+ssl_cert ssl_key Login path file supports these options: host user password
+port socket Environment variables support these options: DOLPHIE_USER
+DOLPHIE_PASSWORD DOLPHIE_HOST DOLPHIE_PORT DOLPHIE_SOCKET Dolphie's config
+supports these options under [dolphie] section: (bool) host_setup (str) user
+(str) password (str) host (int) port (str) socket (str) ssl_mode (str) ssl_ca
+(str) ssl_cert (str) ssl_key (str) mycnf_file (str) login_path (str)
+host_cache_file (str) host_setup_file (int) refresh_interval (str)
+heartbeat_table (str) startup_panels (str) graph_marker (str) pypi_repository
+(str) hostgroup (bool) show_trxs_only (bool) show_additional_query_columns ```
+## Supported ProxySQL versions - ProxySQL 2.6+ (could work on previous versions
+but not tested) Note: Use `admin` user instead of `stats` user so you can use
+all features ## Supported MariaDB versions - MariaDB 5.5/10.0/11.0+ - RDS
+MariaDB ## Supported MySQL versions - MySQL/Percona Server 5.6/5.7/8.0+ - RDS
+MySQL & Aurora + Azure ## MySQL Grants required #### Least privilege 1. PROCESS
+(only if you switch to using processlist via `P` command) 2. SELECT to
+`performance_schema` + `pt-heartbeat table` (if used) 3. REPLICATION CLIENT/
+REPLICATION SLAVE 4. BACKUP_ADMIN (MySQL 8 only) #### Recommended 1. PROCESS
+(only if you switch to using processlist via `P` command) 2. Global SELECT
+access (good for explaining queries, listing all databases, etc) 4. REPLICATION
+CLIENT/REPLICATION SLAVE 5. SUPER (required if you want to kill queries) 6.
+BACKUP_ADMIN (MySQL 8 only) ## Features - Tabs docked at the top to seamlessly
+switch between connected hosts - Hostgroups to make it easy for connecting to
+multiple hosts at once - Dolphie uses panels to present groups of data. They
+can all be turned on/off to have a view of your database server that you prefer
+- Graphs for many metrics that can give you great insight into how your
+database is performing - Sparkline to show queries per second in a live view -
+2 options for finding replica lag in this order of precedence: - `pt-heartbeat
+table` (specified by `--heartbeat-table`) - `SHOW SLAVE STATUS` - Keeps a
+history of the servers you connect to that provides autocompletion for
+hostnames in the Host Setup modal - Host cache file. This provides users a way
+to specify hostnames for IPs when their network's DNS can't resolve them. An
+example use case for this is when you connect to your work's VPN and DNS isn't
+available to resolve IPs. In my opinion, it's a lot easier to look at hostnames
+than IPs! - Supports encrypted login credentials via `mysql_config_editor` -
+Automatic conversion of large numbers & bytes to human-readable - Notifies when
+new version is available - Many commands at your fingertips with autocompletion
+for their input ## Hostgroups Hostgroups are a way to easily connect to
+multiple hosts at once. To set this up, you will create a section in Dolphie's
+config file with the name you want the hostgroup to be and list each host on a
+new line in the format `key=host` (keys have no meaning). Hosts support
+optional port (default is whatever `port` parameter is) in the format `host:
+port`. You can also name the tabs by suffixing `~tab_name` to the host. Once
+ready, you will use the parameter `hostgroup` or `Host Setup` modal to see it
+in action! Note: Colors can be used in the tab name by using the format `
+[color]text[/color]` (i.e. `[red]production[/red]`). You can also use emojis
+supported by Rich (can see them by running `python -m rich.emoji`) by using the
+format `:emoji:` (i.e. `:ghost:`). Rich supports the normal emoji shortcodes.
+Example: ```ini [cluster1] 1=host1 2=host2:3307 3=host3:3308~[red]production[/
+red] :ghost: ``` ## Things to note Order of precedence for methods that pass
+options to Dolphie: 1. Command-line 2. Environment variables 3. Dolphie's
+config (set by `--config-file`) 4. ~/.mylogin.cnf (`mysql_config_editor`) 5.
+~/.my.cnf (set by `--mycnf-file`) ## Feedback I welcome all questions, bug
+reports, and requests. If you enjoy Dolphie, please let me know! I'd love to
+hear from you :smiley:
```

