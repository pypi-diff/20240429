# Comparing `tmp/towalink_tlm-0.2.0.tar.gz` & `tmp/towalink_tlm-0.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "towalink_tlm-0.2.0.tar", last modified: Sun Jun 11 07:58:12 2023, max compression
+gzip compressed data, was "towalink_tlm-0.3.1.tar", last modified: Mon Apr 29 07:29:14 2024, max compression
```

## Comparing `towalink_tlm-0.2.0.tar` & `towalink_tlm-0.3.1.tar`

### file list

```diff
@@ -1,94 +1,94 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-11 07:58:12.559374 towalink_tlm-0.2.0/
--rwxrw-r--   0 root         (0) root         (0)    34523 2020-08-22 10:31:22.000000 towalink_tlm-0.2.0/LICENSE
--rwxrw-r--   0 root         (0) root         (0)       92 2020-08-22 10:32:22.000000 towalink_tlm-0.2.0/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     1526 2023-06-11 07:58:12.587373 towalink_tlm-0.2.0/PKG-INFO
--rwxrw-r--   0 root         (0) root         (0)      496 2023-06-03 20:36:23.000000 towalink_tlm-0.2.0/README.md
--rwxrw-r--   0 root         (0) root         (0)       97 2023-06-11 07:58:12.639373 towalink_tlm-0.2.0/setup.cfg
--rwxrw-r--   0 root         (0) root         (0)     1885 2023-06-03 20:36:23.000000 towalink_tlm-0.2.0/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-11 07:58:04.359489 towalink_tlm-0.2.0/src/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-11 07:58:06.675456 towalink_tlm-0.2.0/src/tlm/
--rwxrw-r--   0 root         (0) root         (0)    13045 2023-06-03 20:36:23.000000 towalink_tlm-0.2.0/src/tlm/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-11 07:58:06.799455 towalink_tlm-0.2.0/src/tlm/ansible/
--rwxrw-r--   0 root         (0) root         (0)      312 2023-05-21 17:49:12.000000 towalink_tlm-0.2.0/src/tlm/ansible/node.yml
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-11 07:58:04.139492 towalink_tlm-0.2.0/src/tlm/ansible/roles/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-11 07:58:03.811496 towalink_tlm-0.2.0/src/tlm/ansible/roles/bird/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-11 07:58:03.783497 towalink_tlm-0.2.0/src/tlm/ansible/roles/bird/files/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-11 07:58:07.267448 towalink_tlm-0.2.0/src/tlm/ansible/roles/bird/files/etc_apt_preferencesd/
--rwxrw-r--   0 root         (0) root         (0)      232 2020-09-08 12:46:36.000000 towalink_tlm-0.2.0/src/tlm/ansible/roles/bird/files/etc_apt_preferencesd/debian-testing
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-11 07:58:07.403446 towalink_tlm-0.2.0/src/tlm/ansible/roles/bird/tasks/
--rwxrw-r--   0 root         (0) root         (0)     2727 2022-07-06 20:50:24.000000 towalink_tlm-0.2.0/src/tlm/ansible/roles/bird/tasks/main.yml
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-11 07:58:03.699498 towalink_tlm-0.2.0/src/tlm/ansible/roles/bird-lg-proxy/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-11 07:58:03.675498 towalink_tlm-0.2.0/src/tlm/ansible/roles/bird-lg-proxy/files/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-11 07:58:06.907453 towalink_tlm-0.2.0/src/tlm/ansible/roles/bird-lg-proxy/files/etc_initd/
--rwxrw-r--   0 root         (0) root         (0)      265 2023-06-11 07:52:39.000000 towalink_tlm-0.2.0/src/tlm/ansible/roles/bird-lg-proxy/files/etc_initd/towalink_bird-lg-proxy
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-11 07:58:07.019451 towalink_tlm-0.2.0/src/tlm/ansible/roles/bird-lg-proxy/files/etc_systemd_system/
--rwxrw-r--   0 root         (0) root         (0)      395 2023-06-11 07:53:03.000000 towalink_tlm-0.2.0/src/tlm/ansible/roles/bird-lg-proxy/files/etc_systemd_system/towalink_bird-lg-proxy.service
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-11 07:58:07.127450 towalink_tlm-0.2.0/src/tlm/ansible/roles/bird-lg-proxy/tasks/
--rwxrw-r--   0 root         (0) root         (0)     1262 2021-09-19 16:04:20.000000 towalink_tlm-0.2.0/src/tlm/ansible/roles/bird-lg-proxy/tasks/main.yml
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-11 07:58:03.919495 towalink_tlm-0.2.0/src/tlm/ansible/roles/nodeconfig/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-11 07:58:03.891495 towalink_tlm-0.2.0/src/tlm/ansible/roles/nodeconfig/files/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-11 07:58:07.543444 towalink_tlm-0.2.0/src/tlm/ansible/roles/nodeconfig/files/opt_towalink_scripts/
--rwxrw-r--   0 root         (0) root         (0)      297 2020-09-07 15:14:20.000000 towalink_tlm-0.2.0/src/tlm/ansible/roles/nodeconfig/files/opt_towalink_scripts/rsync-nodecfg.sh
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-11 07:58:07.727442 towalink_tlm-0.2.0/src/tlm/ansible/roles/nodeconfig/tasks/
--rwxrw-r--   0 root         (0) root         (0)     2336 2020-11-23 09:46:52.000000 towalink_tlm-0.2.0/src/tlm/ansible/roles/nodeconfig/tasks/main.yml
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-11 07:58:04.111492 towalink_tlm-0.2.0/src/tlm/ansible/roles/startup/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-11 07:58:04.055493 towalink_tlm-0.2.0/src/tlm/ansible/roles/startup/files/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-11 07:58:08.003438 towalink_tlm-0.2.0/src/tlm/ansible/roles/startup/files/etc_initd/
--rwxrw-r--   0 root         (0) root         (0)      216 2020-09-10 18:23:39.000000 towalink_tlm-0.2.0/src/tlm/ansible/roles/startup/files/etc_initd/towalink_startup
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-11 07:58:08.135436 towalink_tlm-0.2.0/src/tlm/ansible/roles/startup/files/etc_systemd_system/
--rwxrw-r--   0 root         (0) root         (0)      330 2020-09-11 10:10:47.000000 towalink_tlm-0.2.0/src/tlm/ansible/roles/startup/files/etc_systemd_system/towalink_startup.service
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-11 07:58:08.299434 towalink_tlm-0.2.0/src/tlm/ansible/roles/startup/files/opt_towalink_startup/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-11 07:58:08.427432 towalink_tlm-0.2.0/src/tlm/ansible/roles/startup/files/opt_towalink_startup/scripts/
--rwxrw-r--   0 root         (0) root         (0)      317 2020-06-21 21:01:14.000000 towalink_tlm-0.2.0/src/tlm/ansible/roles/startup/files/opt_towalink_startup/scripts/wireguard
--rwxrw-r--   0 root         (0) root         (0)      250 2020-06-21 20:25:57.000000 towalink_tlm-0.2.0/src/tlm/ansible/roles/startup/files/opt_towalink_startup/towalink.sh
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-11 07:58:08.583430 towalink_tlm-0.2.0/src/tlm/ansible/roles/startup/tasks/
--rwxrw-r--   0 root         (0) root         (0)     1115 2020-09-08 10:25:54.000000 towalink_tlm-0.2.0/src/tlm/ansible/roles/startup/tasks/main.yml
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-11 07:58:04.223491 towalink_tlm-0.2.0/src/tlm/ansible/roles/system/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-11 07:58:04.195491 towalink_tlm-0.2.0/src/tlm/ansible/roles/system/files/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-11 07:58:08.735427 towalink_tlm-0.2.0/src/tlm/ansible/roles/system/files/unused_etc_sysctld/
--rwxrw-r--   0 root         (0) root         (0)      309 2020-09-10 17:23:27.000000 towalink_tlm-0.2.0/src/tlm/ansible/roles/system/files/unused_etc_sysctld/towalink.conf
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-11 07:58:08.887425 towalink_tlm-0.2.0/src/tlm/ansible/roles/system/tasks/
--rwxrw-r--   0 root         (0) root         (0)      589 2020-09-11 14:09:00.000000 towalink_tlm-0.2.0/src/tlm/ansible/roles/system/tasks/main.yml
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-11 07:58:09.219421 towalink_tlm-0.2.0/src/tlm/ansible/vars/
--rwxrw-r--   0 root         (0) root         (0)      137 2020-10-03 21:23:15.000000 towalink_tlm-0.2.0/src/tlm/ansible/vars/external_vars.yml
--rwxrw-r--   0 root         (0) root         (0)     4639 2021-06-16 18:55:44.000000 towalink_tlm-0.2.0/src/tlm/ansiblecaller.py
--rwxrw-r--   0 root         (0) root         (0)     1430 2020-06-02 19:29:15.000000 towalink_tlm-0.2.0/src/tlm/configfilecopier.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-11 07:58:10.383404 towalink_tlm-0.2.0/src/tlm/configmanager/
--rwxrw-r--   0 root         (0) root         (0)        0 2020-06-15 18:25:35.000000 towalink_tlm-0.2.0/src/tlm/configmanager/__init__.py
--rwxrw-r--   0 root         (0) root         (0)     8002 2020-11-23 20:47:19.000000 towalink_tlm-0.2.0/src/tlm/configmanager/configmanager.py
--rwxrw-r--   0 root         (0) root         (0)     3738 2020-09-18 20:20:25.000000 towalink_tlm-0.2.0/src/tlm/configmanager/generatedconfig.py
--rwxrw-r--   0 root         (0) root         (0)     1688 2020-07-25 19:44:05.000000 towalink_tlm-0.2.0/src/tlm/configmanager/nodeconfig.py
--rwxrw-r--   0 root         (0) root         (0)     1503 2020-07-25 19:45:52.000000 towalink_tlm-0.2.0/src/tlm/configmanager/siteconfig.py
--rwxrw-r--   0 root         (0) root         (0)     6433 2020-09-17 19:42:31.000000 towalink_tlm-0.2.0/src/tlm/configmanager/tomlconfig.py
--rwxrw-r--   0 root         (0) root         (0)     4205 2021-05-27 20:26:40.000000 towalink_tlm-0.2.0/src/tlm/configmanager/tomlconfighierarchy.py
--rwxrw-r--   0 root         (0) root         (0)     2408 2023-06-03 20:36:25.000000 towalink_tlm-0.2.0/src/tlm/configmanager/wireguard.py
--rwxrw-r--   0 root         (0) root         (0)     5778 2020-07-12 20:32:32.000000 towalink_tlm-0.2.0/src/tlm/configmanager/yamlconfig.py
--rwxrw-r--   0 root         (0) root         (0)    18466 2023-06-09 15:59:39.000000 towalink_tlm-0.2.0/src/tlm/configorchestrator.py
--rwxrw-r--   0 root         (0) root         (0)     1330 2020-06-24 20:38:54.000000 towalink_tlm-0.2.0/src/tlm/directorycomparer.py
--rwxrw-r--   0 root         (0) root         (0)      891 2020-06-25 20:50:01.000000 towalink_tlm-0.2.0/src/tlm/exceptionlogger.py
--rwxrw-r--   0 root         (0) root         (0)     5170 2020-09-06 18:30:57.000000 towalink_tlm-0.2.0/src/tlm/exechelper.py
--rwxrw-r--   0 root         (0) root         (0)     2492 2021-06-16 19:49:03.000000 towalink_tlm-0.2.0/src/tlm/filesync.py
--rwxrw-r--   0 root         (0) root         (0)     3533 2023-06-09 16:27:34.000000 towalink_tlm-0.2.0/src/tlm/gitcaller.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-11 07:58:10.719400 towalink_tlm-0.2.0/src/tlm/healthcheck/
--rwxrw-r--   0 root         (0) root         (0)        0 2023-06-03 20:36:25.000000 towalink_tlm-0.2.0/src/tlm/healthcheck/__init__.py
--rwxrw-r--   0 root         (0) root         (0)     1489 2023-06-03 20:36:25.000000 towalink_tlm-0.2.0/src/tlm/healthcheck/cmdexec.py
--rwxrw-r--   0 root         (0) root         (0)      831 2023-06-03 20:36:25.000000 towalink_tlm-0.2.0/src/tlm/healthcheck/ping.py
--rwxrw-r--   0 root         (0) root         (0)     3347 2020-07-12 20:29:48.000000 towalink_tlm-0.2.0/src/tlm/jinjatransformer.py
--rwxrw-r--   0 root         (0) root         (0)     3082 2023-06-09 15:57:54.000000 towalink_tlm-0.2.0/src/tlm/management_interface.py
--rwxrw-r--   0 root         (0) root         (0)    18840 2023-06-09 15:59:51.000000 towalink_tlm-0.2.0/src/tlm/nodeattacher.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-11 07:58:11.747385 towalink_tlm-0.2.0/src/tlm/skeleton/
--rwxrw-r--   0 root         (0) root         (0)      160 2020-09-12 09:56:45.000000 towalink_tlm-0.2.0/src/tlm/skeleton/LICENSE
--rwxrw-r--   0 root         (0) root         (0)     2811 2023-06-03 20:36:24.000000 towalink_tlm-0.2.0/src/tlm/skeleton/bird.conf.jinja
--rwxrw-r--   0 root         (0) root         (0)      322 2023-06-03 20:36:24.000000 towalink_tlm-0.2.0/src/tlm/skeleton/bird_neighbors.conf.jinja
--rwxrw-r--   0 root         (0) root         (0)       46 2020-09-11 15:09:58.000000 towalink_tlm-0.2.0/src/tlm/skeleton/bird_site-template.conf.jinja
--rwxrw-r--   0 root         (0) root         (0)     1644 2020-09-27 20:09:05.000000 towalink_tlm-0.2.0/src/tlm/skeleton/config.toml
--rwxrw-r--   0 root         (0) root         (0)      330 2020-09-11 18:12:23.000000 towalink_tlm-0.2.0/src/tlm/skeleton/startup_loopback.jinja
--rwxrw-r--   0 root         (0) root         (0)      545 2020-09-11 15:09:40.000000 towalink_tlm-0.2.0/src/tlm/skeleton/tlwg.conf.jinja
--rwxrw-r--   0 root         (0) root         (0)    14437 2023-06-03 20:49:12.000000 towalink_tlm-0.2.0/src/tlm/towalinkmanager.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-11 07:58:12.451375 towalink_tlm-0.2.0/src/towalink_tlm.egg-info/
--rwxrw-r--   0 root         (0) root         (0)     1526 2023-06-11 07:58:03.000000 towalink_tlm-0.2.0/src/towalink_tlm.egg-info/PKG-INFO
--rwxrw-r--   0 root         (0) root         (0)     2264 2023-06-11 07:58:03.000000 towalink_tlm-0.2.0/src/towalink_tlm.egg-info/SOURCES.txt
--rwxrw-r--   0 root         (0) root         (0)        1 2023-06-11 07:58:03.000000 towalink_tlm-0.2.0/src/towalink_tlm.egg-info/dependency_links.txt
--rwxrw-r--   0 root         (0) root         (0)       33 2023-06-11 07:58:03.000000 towalink_tlm-0.2.0/src/towalink_tlm.egg-info/entry_points.txt
--rwxrw-r--   0 root         (0) root         (0)       72 2023-06-11 07:58:03.000000 towalink_tlm-0.2.0/src/towalink_tlm.egg-info/requires.txt
--rwxrw-r--   0 root         (0) root         (0)        4 2023-06-11 07:58:03.000000 towalink_tlm-0.2.0/src/towalink_tlm.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-29 07:29:13.987734 towalink_tlm-0.3.1/
+-rwxrw-r--   0 root         (0) root         (0)    34523 2020-08-22 10:31:22.000000 towalink_tlm-0.3.1/LICENSE
+-rwxrw-r--   0 root         (0) root         (0)       92 2020-08-22 10:32:22.000000 towalink_tlm-0.3.1/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     1703 2024-04-29 07:29:13.987734 towalink_tlm-0.3.1/PKG-INFO
+-rwxrw-r--   0 root         (0) root         (0)      496 2023-06-03 20:36:23.000000 towalink_tlm-0.3.1/README.md
+-rwxrw-r--   0 root         (0) root         (0)       97 2024-04-29 07:29:13.991734 towalink_tlm-0.3.1/setup.cfg
+-rwxrw-r--   0 root         (0) root         (0)     1895 2024-04-25 18:32:46.000000 towalink_tlm-0.3.1/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-29 07:29:13.763737 towalink_tlm-0.3.1/src/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-29 07:29:13.827736 towalink_tlm-0.3.1/src/tlm/
+-rwxrw-r--   0 root         (0) root         (0)    13045 2023-06-03 20:36:23.000000 towalink_tlm-0.3.1/src/tlm/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-29 07:29:13.831736 towalink_tlm-0.3.1/src/tlm/ansible/
+-rwxrw-r--   0 root         (0) root         (0)      312 2023-05-21 17:49:12.000000 towalink_tlm-0.3.1/src/tlm/ansible/node.yml
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-29 07:29:13.755737 towalink_tlm-0.3.1/src/tlm/ansible/roles/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-29 07:29:13.739737 towalink_tlm-0.3.1/src/tlm/ansible/roles/bird/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-29 07:29:13.739737 towalink_tlm-0.3.1/src/tlm/ansible/roles/bird/files/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-29 07:29:13.847736 towalink_tlm-0.3.1/src/tlm/ansible/roles/bird/files/etc_apt_preferencesd/
+-rwxrw-r--   0 root         (0) root         (0)      232 2020-09-08 12:46:36.000000 towalink_tlm-0.3.1/src/tlm/ansible/roles/bird/files/etc_apt_preferencesd/debian-testing
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-29 07:29:13.851736 towalink_tlm-0.3.1/src/tlm/ansible/roles/bird/tasks/
+-rwxrw-r--   0 root         (0) root         (0)     2727 2022-07-06 20:50:24.000000 towalink_tlm-0.3.1/src/tlm/ansible/roles/bird/tasks/main.yml
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-29 07:29:13.735737 towalink_tlm-0.3.1/src/tlm/ansible/roles/bird-lg-proxy/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-29 07:29:13.735737 towalink_tlm-0.3.1/src/tlm/ansible/roles/bird-lg-proxy/files/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-29 07:29:13.835736 towalink_tlm-0.3.1/src/tlm/ansible/roles/bird-lg-proxy/files/etc_initd/
+-rwxrw-r--   0 root         (0) root         (0)      265 2023-06-11 07:52:39.000000 towalink_tlm-0.3.1/src/tlm/ansible/roles/bird-lg-proxy/files/etc_initd/towalink_bird-lg-proxy
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-29 07:29:13.839736 towalink_tlm-0.3.1/src/tlm/ansible/roles/bird-lg-proxy/files/etc_systemd_system/
+-rwxrw-r--   0 root         (0) root         (0)      395 2023-06-11 07:53:03.000000 towalink_tlm-0.3.1/src/tlm/ansible/roles/bird-lg-proxy/files/etc_systemd_system/towalink_bird-lg-proxy.service
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-29 07:29:13.843736 towalink_tlm-0.3.1/src/tlm/ansible/roles/bird-lg-proxy/tasks/
+-rwxrw-r--   0 root         (0) root         (0)     1262 2021-09-19 16:04:20.000000 towalink_tlm-0.3.1/src/tlm/ansible/roles/bird-lg-proxy/tasks/main.yml
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-29 07:29:13.747737 towalink_tlm-0.3.1/src/tlm/ansible/roles/nodeconfig/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-29 07:29:13.743737 towalink_tlm-0.3.1/src/tlm/ansible/roles/nodeconfig/files/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-29 07:29:13.855736 towalink_tlm-0.3.1/src/tlm/ansible/roles/nodeconfig/files/opt_towalink_scripts/
+-rwxrw-r--   0 root         (0) root         (0)      297 2020-09-07 15:14:20.000000 towalink_tlm-0.3.1/src/tlm/ansible/roles/nodeconfig/files/opt_towalink_scripts/rsync-nodecfg.sh
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-29 07:29:13.859736 towalink_tlm-0.3.1/src/tlm/ansible/roles/nodeconfig/tasks/
+-rwxrw-r--   0 root         (0) root         (0)     2336 2020-11-23 09:46:52.000000 towalink_tlm-0.3.1/src/tlm/ansible/roles/nodeconfig/tasks/main.yml
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-29 07:29:13.755737 towalink_tlm-0.3.1/src/tlm/ansible/roles/startup/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-29 07:29:13.751737 towalink_tlm-0.3.1/src/tlm/ansible/roles/startup/files/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-29 07:29:13.867736 towalink_tlm-0.3.1/src/tlm/ansible/roles/startup/files/etc_initd/
+-rwxrw-r--   0 root         (0) root         (0)      231 2023-11-19 11:13:30.000000 towalink_tlm-0.3.1/src/tlm/ansible/roles/startup/files/etc_initd/towalink_startup
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-29 07:29:13.871736 towalink_tlm-0.3.1/src/tlm/ansible/roles/startup/files/etc_systemd_system/
+-rwxrw-r--   0 root         (0) root         (0)      330 2020-09-11 10:10:47.000000 towalink_tlm-0.3.1/src/tlm/ansible/roles/startup/files/etc_systemd_system/towalink_startup.service
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-29 07:29:13.875736 towalink_tlm-0.3.1/src/tlm/ansible/roles/startup/files/opt_towalink_startup/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-29 07:29:13.879736 towalink_tlm-0.3.1/src/tlm/ansible/roles/startup/files/opt_towalink_startup/scripts/
+-rwxrw-r--   0 root         (0) root         (0)      317 2020-06-21 21:01:14.000000 towalink_tlm-0.3.1/src/tlm/ansible/roles/startup/files/opt_towalink_startup/scripts/wireguard
+-rwxrw-r--   0 root         (0) root         (0)      250 2020-06-21 20:25:57.000000 towalink_tlm-0.3.1/src/tlm/ansible/roles/startup/files/opt_towalink_startup/towalink.sh
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-29 07:29:13.883735 towalink_tlm-0.3.1/src/tlm/ansible/roles/startup/tasks/
+-rwxrw-r--   0 root         (0) root         (0)     1115 2020-09-08 10:25:54.000000 towalink_tlm-0.3.1/src/tlm/ansible/roles/startup/tasks/main.yml
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-29 07:29:13.759737 towalink_tlm-0.3.1/src/tlm/ansible/roles/system/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-29 07:29:13.759737 towalink_tlm-0.3.1/src/tlm/ansible/roles/system/files/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-29 07:29:13.887735 towalink_tlm-0.3.1/src/tlm/ansible/roles/system/files/unused_etc_sysctld/
+-rwxrw-r--   0 root         (0) root         (0)      309 2020-09-10 17:23:27.000000 towalink_tlm-0.3.1/src/tlm/ansible/roles/system/files/unused_etc_sysctld/towalink.conf
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-29 07:29:13.891735 towalink_tlm-0.3.1/src/tlm/ansible/roles/system/tasks/
+-rwxrw-r--   0 root         (0) root         (0)      589 2020-09-11 14:09:00.000000 towalink_tlm-0.3.1/src/tlm/ansible/roles/system/tasks/main.yml
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-29 07:29:13.895735 towalink_tlm-0.3.1/src/tlm/ansible/vars/
+-rwxrw-r--   0 root         (0) root         (0)      137 2020-10-03 21:23:15.000000 towalink_tlm-0.3.1/src/tlm/ansible/vars/external_vars.yml
+-rwxrw-r--   0 root         (0) root         (0)     4639 2021-06-16 18:55:44.000000 towalink_tlm-0.3.1/src/tlm/ansiblecaller.py
+-rwxrw-r--   0 root         (0) root         (0)     1430 2020-06-02 19:29:15.000000 towalink_tlm-0.3.1/src/tlm/configfilecopier.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-29 07:29:13.927735 towalink_tlm-0.3.1/src/tlm/configmanager/
+-rwxrw-r--   0 root         (0) root         (0)        0 2020-06-15 18:25:35.000000 towalink_tlm-0.3.1/src/tlm/configmanager/__init__.py
+-rwxrw-r--   0 root         (0) root         (0)     8372 2024-04-25 19:51:28.000000 towalink_tlm-0.3.1/src/tlm/configmanager/configmanager.py
+-rwxrw-r--   0 root         (0) root         (0)     3943 2024-04-23 20:25:29.000000 towalink_tlm-0.3.1/src/tlm/configmanager/generatedconfig.py
+-rwxrw-r--   0 root         (0) root         (0)     1688 2020-07-25 19:44:05.000000 towalink_tlm-0.3.1/src/tlm/configmanager/nodeconfig.py
+-rwxrw-r--   0 root         (0) root         (0)     1503 2020-07-25 19:45:52.000000 towalink_tlm-0.3.1/src/tlm/configmanager/siteconfig.py
+-rwxrw-r--   0 root         (0) root         (0)     6433 2020-09-17 19:42:31.000000 towalink_tlm-0.3.1/src/tlm/configmanager/tomlconfig.py
+-rwxrw-r--   0 root         (0) root         (0)     4205 2021-05-27 20:26:40.000000 towalink_tlm-0.3.1/src/tlm/configmanager/tomlconfighierarchy.py
+-rwxrw-r--   0 root         (0) root         (0)     2408 2024-04-23 19:52:45.000000 towalink_tlm-0.3.1/src/tlm/configmanager/wireguard.py
+-rwxrw-r--   0 root         (0) root         (0)     5778 2020-07-12 20:32:32.000000 towalink_tlm-0.3.1/src/tlm/configmanager/yamlconfig.py
+-rwxrw-r--   0 root         (0) root         (0)    18758 2024-04-26 20:04:14.000000 towalink_tlm-0.3.1/src/tlm/configorchestrator.py
+-rwxrw-r--   0 root         (0) root         (0)     1330 2020-06-24 20:38:54.000000 towalink_tlm-0.3.1/src/tlm/directorycomparer.py
+-rwxrw-r--   0 root         (0) root         (0)      891 2020-06-25 20:50:01.000000 towalink_tlm-0.3.1/src/tlm/exceptionlogger.py
+-rwxrw-r--   0 root         (0) root         (0)     5170 2020-09-06 18:30:57.000000 towalink_tlm-0.3.1/src/tlm/exechelper.py
+-rwxrw-r--   0 root         (0) root         (0)     2556 2024-04-26 20:02:14.000000 towalink_tlm-0.3.1/src/tlm/filesync.py
+-rwxrw-r--   0 root         (0) root         (0)     3533 2023-06-09 16:27:34.000000 towalink_tlm-0.3.1/src/tlm/gitcaller.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-29 07:29:13.935735 towalink_tlm-0.3.1/src/tlm/healthcheck/
+-rwxrw-r--   0 root         (0) root         (0)        0 2023-06-03 20:36:25.000000 towalink_tlm-0.3.1/src/tlm/healthcheck/__init__.py
+-rwxrw-r--   0 root         (0) root         (0)     1489 2023-06-03 20:36:25.000000 towalink_tlm-0.3.1/src/tlm/healthcheck/cmdexec.py
+-rwxrw-r--   0 root         (0) root         (0)      831 2023-06-03 20:36:25.000000 towalink_tlm-0.3.1/src/tlm/healthcheck/ping.py
+-rwxrw-r--   0 root         (0) root         (0)     3347 2020-07-12 20:29:48.000000 towalink_tlm-0.3.1/src/tlm/jinjatransformer.py
+-rwxrw-r--   0 root         (0) root         (0)     3082 2023-06-09 15:57:54.000000 towalink_tlm-0.3.1/src/tlm/management_interface.py
+-rwxrw-r--   0 root         (0) root         (0)    18840 2023-06-09 15:59:51.000000 towalink_tlm-0.3.1/src/tlm/nodeattacher.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-29 07:29:13.963734 towalink_tlm-0.3.1/src/tlm/skeleton/
+-rwxrw-r--   0 root         (0) root         (0)      160 2020-09-12 09:56:45.000000 towalink_tlm-0.3.1/src/tlm/skeleton/LICENSE
+-rwxrw-r--   0 root         (0) root         (0)     2811 2023-06-03 20:36:24.000000 towalink_tlm-0.3.1/src/tlm/skeleton/bird.conf.jinja
+-rwxrw-r--   0 root         (0) root         (0)      322 2023-06-03 20:36:24.000000 towalink_tlm-0.3.1/src/tlm/skeleton/bird_neighbors.conf.jinja
+-rwxrw-r--   0 root         (0) root         (0)       46 2020-09-11 15:09:58.000000 towalink_tlm-0.3.1/src/tlm/skeleton/bird_site-template.conf.jinja
+-rwxrw-r--   0 root         (0) root         (0)     1644 2020-09-27 20:09:05.000000 towalink_tlm-0.3.1/src/tlm/skeleton/config.toml
+-rwxrw-r--   0 root         (0) root         (0)      330 2020-09-11 18:12:23.000000 towalink_tlm-0.3.1/src/tlm/skeleton/startup_loopback.jinja
+-rwxrw-r--   0 root         (0) root         (0)      603 2024-04-23 20:31:58.000000 towalink_tlm-0.3.1/src/tlm/skeleton/tlwg.conf.jinja
+-rwxrw-r--   0 root         (0) root         (0)    14437 2023-06-03 20:49:12.000000 towalink_tlm-0.3.1/src/tlm/towalinkmanager.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-29 07:29:13.983734 towalink_tlm-0.3.1/src/towalink_tlm.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     1703 2024-04-29 07:29:13.000000 towalink_tlm-0.3.1/src/towalink_tlm.egg-info/PKG-INFO
+-rwxrw-r--   0 root         (0) root         (0)     2264 2024-04-29 07:29:13.000000 towalink_tlm-0.3.1/src/towalink_tlm.egg-info/SOURCES.txt
+-rwxrw-r--   0 root         (0) root         (0)        1 2024-04-29 07:29:13.000000 towalink_tlm-0.3.1/src/towalink_tlm.egg-info/dependency_links.txt
+-rwxrw-r--   0 root         (0) root         (0)       33 2024-04-29 07:29:13.000000 towalink_tlm-0.3.1/src/towalink_tlm.egg-info/entry_points.txt
+-rwxrw-r--   0 root         (0) root         (0)       72 2024-04-29 07:29:13.000000 towalink_tlm-0.3.1/src/towalink_tlm.egg-info/requires.txt
+-rwxrw-r--   0 root         (0) root         (0)        4 2024-04-29 07:29:13.000000 towalink_tlm-0.3.1/src/towalink_tlm.egg-info/top_level.txt
```

### Comparing `towalink_tlm-0.2.0/LICENSE` & `towalink_tlm-0.3.1/LICENSE`

 * *Files identical despite different names*

### Comparing `towalink_tlm-0.2.0/PKG-INFO` & `towalink_tlm-0.3.1/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: towalink_tlm
-Version: 0.2.0
+Version: 0.3.1
 Summary: command line tool for configuring and managing a Towalink installation
 Home-page: https://www.towalink.net
 Author: The Towalink Project
 Author-email: pypi.tlm@towalink.net
 Project-URL: Project homepage, https://www.towalink.net
 Project-URL: Repository, https://www.github.com/towalink/tlm
 Project-URL: Documentation, https://towalink.readthedocs.io
@@ -17,14 +17,21 @@
 Classifier: Intended Audience :: System Administrators
 Classifier: Intended Audience :: Information Technology
 Classifier: Intended Audience :: Telecommunications Industry
 Classifier: Topic :: System :: Networking
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
+Requires-Dist: python-configuration
+Requires-Dist: jinja2
+Requires-Dist: pyyaml
+Requires-Dist: toml
+Requires-Dist: tomlkit
+Requires-Dist: ansible
+Requires-Dist: wgconfig>=1.0.1
 
 # tlm - Towalink Manager
 
 Tool for configuring and managing a Towalink installation.
 
 ---
```

#### html2text {}

```diff
@@ -1,20 +1,22 @@
-Metadata-Version: 2.1 Name: towalink_tlm Version: 0.2.0 Summary: command line
+Metadata-Version: 2.1 Name: towalink_tlm Version: 0.3.1 Summary: command line
 tool for configuring and managing a Towalink installation Home-page: https://
 www.towalink.net Author: The Towalink Project Author-email:
 pypi.tlm@towalink.net Project-URL: Project homepage, https://www.towalink.net
 Project-URL: Repository, https://www.github.com/towalink/tlm Project-URL:
 Documentation, https://towalink.readthedocs.io Keywords: Towalink VPN SD-WAN
 WireGuard Classifier: Programming Language :: Python Classifier: Programming
 Language :: Python :: 3 Classifier: License :: OSI Approved :: GNU Affero
 General Public License v3 or later (AGPLv3+) Classifier: Operating System ::
 POSIX :: Linux Classifier: Development Status :: 4 - Beta Classifier: Intended
 Audience :: System Administrators Classifier: Intended Audience :: Information
 Technology Classifier: Intended Audience :: Telecommunications Industry
 Classifier: Topic :: System :: Networking Requires-Python: >=3.6 Description-
-Content-Type: text/markdown License-File: LICENSE # tlm - Towalink Manager Tool
-for configuring and managing a Towalink installation. --- ## Documentation The
-documentation of the Towalink project can be found at https://
-towalink.readthedocs.io --- ## License [![License](http://img.shields.io/:
-license-agpl3-blue.svg?style=flat-square)](https://opensource.org/licenses/
-AGPL-3.0) - **[AGPL3 license](https://opensource.org/licenses/AGPL-3.0)** -
-Copyright 2020-2023 Â© _D_i_r_k_ _H_e_n_r_i_c_i.
+Content-Type: text/markdown License-File: LICENSE Requires-Dist: python-
+configuration Requires-Dist: jinja2 Requires-Dist: pyyaml Requires-Dist: toml
+Requires-Dist: tomlkit Requires-Dist: ansible Requires-Dist: wgconfig>=1.0.1 #
+tlm - Towalink Manager Tool for configuring and managing a Towalink
+installation. --- ## Documentation The documentation of the Towalink project
+can be found at https://towalink.readthedocs.io --- ## License [![License]
+(http://img.shields.io/:license-agpl3-blue.svg?style=flat-square)](https://
+opensource.org/licenses/AGPL-3.0) - **[AGPL3 license](https://opensource.org/
+licenses/AGPL-3.0)** - Copyright 2020-2023 Â© _D_i_r_k_ _H_e_n_r_i_c_i.
```

### Comparing `towalink_tlm-0.2.0/setup.py` & `towalink_tlm-0.3.1/setup.py`

 * *Files 9% similar despite different names*

```diff
@@ -3,31 +3,31 @@
 
 
 with open('README.md', 'r') as f:
     long_description = f.read()
 
 setup_kwargs = {
     'name': 'towalink_tlm',
-    'version': '0.2.0',
+    'version': '0.3.1',
     'author': 'The Towalink Project',
     'author_email': 'pypi.tlm@towalink.net',
     'description': 'command line tool for configuring and managing a Towalink installation',
     'long_description': long_description,
     'long_description_content_type': 'text/markdown',
     'url': 'https://www.towalink.net',
-    'packages': setuptools.find_packages('src'),
+    'packages': setuptools.find_namespace_packages('src'),
     'package_dir': {'': 'src'},
     'include_package_data': True,
     'install_requires': ['python-configuration',
                          'jinja2',
                          'pyyaml',
                          'toml',
                          'tomlkit',
                          'ansible',
-                         'wgconfig>=0.1.4'
+                         'wgconfig>=1.0.1'
                         ],
     'entry_points': '''
         [console_scripts]
         tlm=tlm:main
     ''',
     'classifiers': [
         'Programming Language :: Python',
```

### Comparing `towalink_tlm-0.2.0/src/tlm/__init__.py` & `towalink_tlm-0.3.1/src/tlm/__init__.py`

 * *Files identical despite different names*

### Comparing `towalink_tlm-0.2.0/src/tlm/ansible/roles/bird/tasks/main.yml` & `towalink_tlm-0.3.1/src/tlm/ansible/roles/bird/tasks/main.yml`

 * *Files identical despite different names*

### Comparing `towalink_tlm-0.2.0/src/tlm/ansible/roles/bird-lg-proxy/tasks/main.yml` & `towalink_tlm-0.3.1/src/tlm/ansible/roles/bird-lg-proxy/tasks/main.yml`

 * *Files identical despite different names*

### Comparing `towalink_tlm-0.2.0/src/tlm/ansible/roles/nodeconfig/tasks/main.yml` & `towalink_tlm-0.3.1/src/tlm/ansible/roles/nodeconfig/tasks/main.yml`

 * *Files identical despite different names*

### Comparing `towalink_tlm-0.2.0/src/tlm/ansible/roles/startup/tasks/main.yml` & `towalink_tlm-0.3.1/src/tlm/ansible/roles/startup/tasks/main.yml`

 * *Files identical despite different names*

### Comparing `towalink_tlm-0.2.0/src/tlm/ansible/roles/system/tasks/main.yml` & `towalink_tlm-0.3.1/src/tlm/ansible/roles/system/tasks/main.yml`

 * *Files identical despite different names*

### Comparing `towalink_tlm-0.2.0/src/tlm/ansiblecaller.py` & `towalink_tlm-0.3.1/src/tlm/ansiblecaller.py`

 * *Files identical despite different names*

### Comparing `towalink_tlm-0.2.0/src/tlm/configfilecopier.py` & `towalink_tlm-0.3.1/src/tlm/configfilecopier.py`

 * *Files identical despite different names*

### Comparing `towalink_tlm-0.2.0/src/tlm/configmanager/configmanager.py` & `towalink_tlm-0.3.1/src/tlm/configmanager/configmanager.py`

 * *Files 4% similar despite different names*

```diff
@@ -16,14 +16,15 @@
 
 
 logger = logging.getLogger(__name__)
 ATTR_NODE_ID = 'node_id'
 NODE_DIR_PREFIX = 'node_'
 SITE_DIR_PREFIX = 'site_'
 CONFNAME = 'config.toml' # name of the config file
+WG_MTU_DEFAULT = 1420
 
 
 class ConfigManager():
     """Class for managing the complete config directory hierarchy"""
     generated_dir = 'generated' # directory    
 
     def __init__(self, confdir='/etc/towalink'):
@@ -74,18 +75,23 @@
     def update_generated_config(self):
         """Make sure that the automatically generated config is current"""
         neighbors = collections.defaultdict(list)
         for node1_key, node2_key in itertools.combinations(self.nodes.keys(), 2):
             node1 = self.nodes[node1_key]
             node2 = self.nodes[node2_key]
             active = len(node1.groups.intersection(node2.groups)) > 0
+            node1_wgmtu = node1.complete_cfg.get('wg_mtu', WG_MTU_DEFAULT)
+            node2_wgmtu = node2.complete_cfg.get('wg_mtu', WG_MTU_DEFAULT)
+            wg_mtu = min(node1_wgmtu, node2_wgmtu)  # set link MTU to smallest common denominator of both Nodes
+            if wg_mtu == WG_MTU_DEFAULT:
+                wg_mtu = None
             if active:
                 neighbors[node1_key].append(node2_key)
                 neighbors[node2_key].append(node1_key)
-            self.generated.set_linkdata(node1_key, node2_key, active=active)
+            self.generated.set_linkdata(node1_key, node2_key, active=active, wg_mtu=wg_mtu)
         self.generated.set_neighbors(neighbors)
         self.generated.save_config()    
         
     def get_nodes(self):
         """Returns a dictionary of nodes (id-><flat data>)"""
         nodes = { node_key: node.complete_cfg for node_key, node in self.nodes.items() }
         return nodes
```

### Comparing `towalink_tlm-0.2.0/src/tlm/configmanager/generatedconfig.py` & `towalink_tlm-0.3.1/src/tlm/configmanager/generatedconfig.py`

 * *Files 4% similar despite different names*

```diff
@@ -21,43 +21,43 @@
 
     def __init__(self, path):
         """Object initialization"""
         filename = os.path.join(path, self.confname)
         super().__init__(filename)
         if os.path.isfile(filename):
             self.load_config()
-        self.wireguard = wireguard.Wireguard()
+        self.wireguard = wireguard.WireGuard()
 
     def save_config(self):
         """Saves the current configuration to file"""
         dirname = os.path.dirname(self._filename)
         if self._is_changed and not os.path.exists(dirname):
             os.makedirs(dirname)
         super().save_config()
 
     def generate_wireguard_keypair(self):
-        """Returns a Wireguard key pair"""
+        """Returns a WireGuard key pair"""
         wg_private, wg_public = self.wireguard.generate_keypair()
         if wg_public is None:
-            raise ValueError('Generating Wireguard key pair failed. Is Wireguard installed and in the search path?')
+            raise ValueError('Generating WireGuard key pair failed. Is WireGuard installed and in the search path?')
         return wg_private, wg_public
 
     def generate_wireguard_psk(self):
         """Returns a Wireguard pre-shared key"""
         wg_preshared = self.wireguard.generate_presharedkey()
         if wg_preshared is None:
-            raise ValueError('Generating Wireguard pre-shared key failed. Is Wireguard installed and in the search path?')
+            raise ValueError('Generating WireGuard pre-shared key failed. Is WireGuard installed and in the search path?')
         return wg_preshared
 
     def set_neighbors(self, neighbors):
         """Represent the current neighbor relations"""
         for node_key, neighborlist in neighbors.items():
             self.set_item(f'neighbors.{node_key}', neighborlist)
 
-    def set_linkdata(self, node1_key, node2_key, active):
+    def set_linkdata(self, node1_key, node2_key, active, wg_mtu):
         """Ensures that all data of a link is present as needed"""
         if node1_key > node2_key: # make sure that the first identifier is the smaller one
             node2_key, node1_key = node1_key, node2_key
         linkname = f'{node1_key}-{node2_key}'
         self.set_item(f'links.{linkname}.active', active)
         self.set_item(f'links.{linkname}.wg_active', active)
         if active and (self.get_item(f'links.{linkname}.wg_private_{node1_key}') is None):
@@ -69,13 +69,15 @@
             self.set_item(f'links.{linkname}.wg_private_{node2_key}', wg_private)
             self.set_item(f'links.{linkname}.wg_public_{node2_key}', wg_public)
         if active and (self.get_item(f'links.{linkname}.wg_preshared') is None):
             wg_preshared = self.generate_wireguard_psk()
             self.set_item(f'links.{linkname}.wg_preshared', wg_preshared)
         if active and (self.get_item(f'links.{linkname}.bgp_password') is None):
             bgp_password = ''.join(secrets.choice(string.ascii_uppercase + string.ascii_lowercase + string.digits) for _ in range(16))
-            self.set_item(f'links.{linkname}.bgp_password', bgp_password)            
+            self.set_item(f'links.{linkname}.bgp_password', bgp_password)
+        if active or (self.get_item(f'links.{linkname}.wg_mtu') is not None):  # set initially only when active but update existing value always
+            self.set_item(f'links.{linkname}.wg_mtu', wg_mtu)
 
 
 if __name__ == '__main__':
     logging.basicConfig(format='%(asctime)s %(levelname)s %(module)s: %(message)s', level=logging.INFO)  # use %(name)s instead of %(module) to include hierarchy information, see 
     sc = GeneratedConfig()
```

### Comparing `towalink_tlm-0.2.0/src/tlm/configmanager/nodeconfig.py` & `towalink_tlm-0.3.1/src/tlm/configmanager/nodeconfig.py`

 * *Files identical despite different names*

### Comparing `towalink_tlm-0.2.0/src/tlm/configmanager/siteconfig.py` & `towalink_tlm-0.3.1/src/tlm/configmanager/siteconfig.py`

 * *Files identical despite different names*

### Comparing `towalink_tlm-0.2.0/src/tlm/configmanager/tomlconfig.py` & `towalink_tlm-0.3.1/src/tlm/configmanager/tomlconfig.py`

 * *Files identical despite different names*

### Comparing `towalink_tlm-0.2.0/src/tlm/configmanager/tomlconfighierarchy.py` & `towalink_tlm-0.3.1/src/tlm/configmanager/tomlconfighierarchy.py`

 * *Files identical despite different names*

### Comparing `towalink_tlm-0.2.0/src/tlm/configmanager/wireguard.py` & `towalink_tlm-0.3.1/src/tlm/configmanager/wireguard.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 # -*- coding: utf-8 -*-
 
-"""Class for executing Wireguard commands"""
+"""Class for executing WireGuard commands"""
 
 import logging
 import shlex
 import subprocess
 
 
 logger = logging.getLogger(__name__);
 
 
-class Wireguard(object):
-    """Class for executing Wireguard commands"""
+class WireGuard(object):
+    """Class for executing WireGuard commands"""
     
     def execute(self, command, input=None, suppressoutput=False, suppresserrors=False):
         """Execute a command"""
         args = shlex.split(command)
         stdin = None if input is None else subprocess.PIPE
         input = None if input is None else input.encode('utf-8')
         nsp = subprocess.Popen(args, stdin=stdin, stdout=subprocess.PIPE, stderr=subprocess.PIPE)
@@ -27,43 +27,43 @@
         out = out.decode('utf8')
         if not suppressoutput and (len(out) > 0):
             print(out)
         nsp.wait()
         return out, err, nsp.returncode
         
     def generate_privatekey(self):
-        """Generates a Wireguard private key"""
+        """Generates a WireGuard private key"""
         out, err, returncode = self.execute('wg genkey', suppressoutput=True)
         if (returncode != 0) or (len(err) > 0):
             return None
         out = out.strip() # remove trailing newline
         return out
         
     def get_publickey(self, wg_private):
-        """Gets the public key belonging to the given Wireguard private key"""
+        """Gets the public key belonging to the given WireGuard private key"""
         if wg_private is None:
             return None
         out, err, returncode = self.execute('wg pubkey', input=wg_private, suppressoutput=True)
         if (returncode != 0) or (len(err) > 0):
             return None
         out = out.strip() # remove trailing newline
         return out
 
     def generate_keypair(self):
-        """Generates a Wireguard key pair (returns tuple of private key and public key)"""
+        """Generates a WireGuard key pair (returns tuple of private key and public key)"""
         wg_private = self.generate_privatekey()
         wg_public = self.get_publickey(wg_private)
         return wg_private, wg_public
 
     def generate_presharedkey(self):
-        """Generates a Wireguard preshared key"""
+        """Generates a WireGuard preshared key"""
         out, err, returncode = self.execute('wg genpsk', suppressoutput=True)
         if (returncode != 0) or (len(err) > 0):
             return None
         out = out.strip() # remove trailing newline
         return out
 
 
 if __name__ == '__main__':
-    wg = Wireguard()
+    wg = WireGuard()
     print(wg.generate_keypair())
     print(wg.generate_presharedkey())
```

### Comparing `towalink_tlm-0.2.0/src/tlm/configmanager/yamlconfig.py` & `towalink_tlm-0.3.1/src/tlm/configmanager/yamlconfig.py`

 * *Files identical despite different names*

### Comparing `towalink_tlm-0.2.0/src/tlm/configorchestrator.py` & `towalink_tlm-0.3.1/src/tlm/configorchestrator.py`

 * *Files 2% similar despite different names*

```diff
@@ -146,14 +146,16 @@
                     peer.remove(str(node_id))
                     peer = peer[0]
                     peerdata = self.cm.nodes.get(int(peer))
                     # Wireguard attributes
                     wg_ifname = f'tlwg_{peer}'
                     cfg_effective.set_item(f'wg_links.{peer}.wg_ifname', wg_ifname)
                     cfg_effective.set_item(f'wg_links.{peer}.wg_listenport', wg_listenport_base + int(peer))
+                    if data.get('wg_mtu') is not None:
+                        cfg_effective.set_item(f'wg_links.{peer}.wg_mtu', data.get('wg_mtu'))
                     #Removed IPv4 addresses since it is added by other means (i.e. post-up directive)
                     #wg_addresses = [ self.get_ipaddress_byoffset(internode_transfernet_ipv4, offset=node_id, keep_prefixlen=True),
                     #                 self.get_ipaddress_byoffset(internode_transfernet_ipv6, offset=node_id, keep_prefixlen=True) ]
                     wg_addresses = [ self.get_ipaddress_byoffset(internode_transfernet_ipv6, offset=node_id, keep_prefixlen=True) ]
                     cfg_effective.set_item(f'wg_links.{peer}.wg_addresses', wg_addresses)
                     cfg_effective.set_item(f'wg_links.{peer}.wg_address_ipv4', self.get_ipaddress_byoffset(internode_transfernet_ipv4, offset=node_id, keep_prefixlen=False))
                     cfg_effective.set_item(f'wg_links.{peer}.wg_address_ipv6', self.get_ipaddress_byoffset(internode_transfernet_ipv6, offset=node_id, keep_prefixlen=False))
@@ -255,22 +257,23 @@
             if self.process_new_configversion(node_id, dryrun = dryrun):
                 changed[node_id] = node
         return self.cm.nodes, changed
 
     def mirror_node_configs(self, nodes):
         """Mirrors the config files of the given nodes to the respective devices"""
         for node_id in nodes:
-            node = self.cm.nodes.get(node_id)            
+            node = self.cm.nodes.get(node_id)
+            node_fullname = node.complete_cfg.get('node_fullname')
             mgmt_address = node.get('attach_mgmt_address')
             if mgmt_address is None:
                 logger.warning(f'Node [{node_id}] does not seem to have been attached; attach_mgmt_address is missing; skipping')
                 continue            
             logger.debug(f'Mirroring config files for node [{node_id}] with management address [{mgmt_address}]')
             fs = filesync.FileSync(sourcepath=self.get_node_dir(node_id), destpath=NODE_CONFIG_PATH)
-            fs.mirror_node_configs(mgmt_address)
+            fs.mirror_node_configs(node_fullname, mgmt_address)
 
     def activate_nodeconfigs(self, nodes, version='latest'):
         """Activates the requested config version on the given node devices"""
         # Validate version parameter
         if version is None:
             raise ValueError('Version must not be None')
         version = str(version).lower()
@@ -281,15 +284,16 @@
                 version = version[1:]
             if version in ['latest', 'current']:
                 version = None
         if (version is not None) and (not version.isnumeric()):
             raise ValueError('Version is malformed')
         # Iterate through nodes
         for node_id in nodes:
-            node = self.cm.nodes.get(node_id)            
+            node = self.cm.nodes.get(node_id)   
+            node_fullname = node.complete_cfg.get('node_fullname')
             mgmt_address = node.get('attach_mgmt_address')
             if mgmt_address is None:
                 logger.warning(f'Node [{node_id}] does not seem to have been attached; attach_mgmt_address is missing; skipping')
                 continue            
             # Create symlink to active configuration
             nodedir = self.get_node_dir(node_id)
             latest, _ = self.get_latest_configdir(nodedir)
@@ -305,15 +309,15 @@
                 continue
             with contextlib.suppress(FileNotFoundError):
                 os.unlink(os.path.join(nodedir, 'active'))
             os.symlink(versiondir, os.path.join(nodedir, 'active'))
             # Mirroring changes to node
             logger.info(f'Activating config for node [{node_id}]')
             fs = filesync.FileSync(sourcepath=self.get_node_dir(node_id), destpath=NODE_CONFIG_PATH)
-            fs.mirror_node_active(mgmt_address)
+            fs.mirror_node_active(node_fullname, mgmt_address)
 
 
 if __name__ == '__main__':
     logging.basicConfig(format='%(asctime)s %(levelname)s %(module)s: %(message)s', level=logging.DEBUG)  # use %(name)s instead of %(module) to include hierarchy information, see 
     co = ConfigOrchestrator('/etc/towalink/')
     import exceptionlogger
     exceptionlogger.call(co.update_all, reraise_exceptions=True)
```

### Comparing `towalink_tlm-0.2.0/src/tlm/directorycomparer.py` & `towalink_tlm-0.3.1/src/tlm/directorycomparer.py`

 * *Files identical despite different names*

### Comparing `towalink_tlm-0.2.0/src/tlm/exceptionlogger.py` & `towalink_tlm-0.3.1/src/tlm/exceptionlogger.py`

 * *Files identical despite different names*

### Comparing `towalink_tlm-0.2.0/src/tlm/exechelper.py` & `towalink_tlm-0.3.1/src/tlm/exechelper.py`

 * *Files identical despite different names*

### Comparing `towalink_tlm-0.2.0/src/tlm/filesync.py` & `towalink_tlm-0.3.1/src/tlm/filesync.py`

 * *Files 13% similar despite different names*

```diff
@@ -44,22 +44,22 @@
         if rsync_path is not None:
             opts.append(f'--rsync-path={rsync_path}')
         opts.append(src)
         opts.append(dst)
         opts = ' '.join(opts)
         return self.execute(opts)
  
-    def mirror_node_configs(self, hostname):
+    def mirror_node_configs(self, node_fullname, hostname):
         """Mirror a Node's config files to the Node"""
-        logger.info(f'Mirroring configs to {hostname}')
+        logger.info(f'Mirroring configs to {node_fullname}({hostname})')
         src = self.sourcepath + '/'
         dst = '[' + hostname + ']:' + self.destpath
         excludes = ['tmp', 'new', 'active']
         #rsync -a --exclude=new --exclude=tmp --exclude=active /etc/towalink/effective/node_12/ [fe80::c%tlwg_mgmt]:/etc/towalink/configs
         return self.exec_rsync(src=src, dst=dst, options=['-a', '-q', '-e', '"ssh -o ConnectTimeout=2"'], excludes=excludes)
 
-    def mirror_node_active(self, hostname):
+    def mirror_node_active(self, node_fullname, hostname):
         """Mirror a Node's active config version to the Node"""
-        logger.info(f'Mirroring active config to {hostname}')
+        logger.info(f'Mirroring active config to {node_fullname}({hostname})')
         src = os.path.join(self.sourcepath, 'active')
         dst = '[' + hostname + ']:' + self.destpath
         return self.exec_rsync(src=src, dst=dst, options=['-a', '-q', '-e', '"ssh -o ConnectTimeout=2"'], rsync_path=RSYNC_PATH_SPECIAL)
```

### Comparing `towalink_tlm-0.2.0/src/tlm/gitcaller.py` & `towalink_tlm-0.3.1/src/tlm/gitcaller.py`

 * *Files identical despite different names*

### Comparing `towalink_tlm-0.2.0/src/tlm/healthcheck/cmdexec.py` & `towalink_tlm-0.3.1/src/tlm/healthcheck/cmdexec.py`

 * *Files identical despite different names*

### Comparing `towalink_tlm-0.2.0/src/tlm/healthcheck/ping.py` & `towalink_tlm-0.3.1/src/tlm/healthcheck/ping.py`

 * *Files identical despite different names*

### Comparing `towalink_tlm-0.2.0/src/tlm/jinjatransformer.py` & `towalink_tlm-0.3.1/src/tlm/jinjatransformer.py`

 * *Files identical despite different names*

### Comparing `towalink_tlm-0.2.0/src/tlm/management_interface.py` & `towalink_tlm-0.3.1/src/tlm/management_interface.py`

 * *Files identical despite different names*

### Comparing `towalink_tlm-0.2.0/src/tlm/nodeattacher.py` & `towalink_tlm-0.3.1/src/tlm/nodeattacher.py`

 * *Files identical despite different names*

### Comparing `towalink_tlm-0.2.0/src/tlm/skeleton/bird.conf.jinja` & `towalink_tlm-0.3.1/src/tlm/skeleton/bird.conf.jinja`

 * *Files identical despite different names*

### Comparing `towalink_tlm-0.2.0/src/tlm/skeleton/config.toml` & `towalink_tlm-0.3.1/src/tlm/skeleton/config.toml`

 * *Files identical despite different names*

### Comparing `towalink_tlm-0.2.0/src/tlm/skeleton/tlwg.conf.jinja` & `towalink_tlm-0.3.1/src/tlm/skeleton/tlwg.conf.jinja`

 * *Files 11% similar despite different names*

```diff
@@ -1,14 +1,17 @@
 [Interface]
 ListenPort = {{wg_listenport}}
 PrivateKey = {{wg_private}}
 Address = {{wg_addresses|join(', ')}}
 {%- if wg_peer_address_ipv4 is defined %}
 Postup = ip addr add {{wg_address_ipv4}} peer {{wg_peer_address_ipv4}} dev {{wg_ifname}}
 {%- endif %}
+{%- if wg_mtu is defined %}
+Mtu = {{wg_mtu}}
+{%- endif %}
 Table = off
 
 [Peer]
 Endpoint = {{wg_peer_endpoint}}
 PublicKey = {{wg_peer_public}}
 {%- if wg_peer_preshared is defined and wg_peer_preshared|length %}
 PresharedKey = {{wg_peer_preshared}}
```

### Comparing `towalink_tlm-0.2.0/src/tlm/towalinkmanager.py` & `towalink_tlm-0.3.1/src/tlm/towalinkmanager.py`

 * *Files identical despite different names*

### Comparing `towalink_tlm-0.2.0/src/towalink_tlm.egg-info/PKG-INFO` & `towalink_tlm-0.3.1/src/towalink_tlm.egg-info/PKG-INFO`

 * *Files 26% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: towalink-tlm
-Version: 0.2.0
+Version: 0.3.1
 Summary: command line tool for configuring and managing a Towalink installation
 Home-page: https://www.towalink.net
 Author: The Towalink Project
 Author-email: pypi.tlm@towalink.net
 Project-URL: Project homepage, https://www.towalink.net
 Project-URL: Repository, https://www.github.com/towalink/tlm
 Project-URL: Documentation, https://towalink.readthedocs.io
@@ -17,14 +17,21 @@
 Classifier: Intended Audience :: System Administrators
 Classifier: Intended Audience :: Information Technology
 Classifier: Intended Audience :: Telecommunications Industry
 Classifier: Topic :: System :: Networking
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
+Requires-Dist: python-configuration
+Requires-Dist: jinja2
+Requires-Dist: pyyaml
+Requires-Dist: toml
+Requires-Dist: tomlkit
+Requires-Dist: ansible
+Requires-Dist: wgconfig>=1.0.1
 
 # tlm - Towalink Manager
 
 Tool for configuring and managing a Towalink installation.
 
 ---
```

#### html2text {}

```diff
@@ -1,20 +1,22 @@
-Metadata-Version: 2.1 Name: towalink-tlm Version: 0.2.0 Summary: command line
+Metadata-Version: 2.1 Name: towalink-tlm Version: 0.3.1 Summary: command line
 tool for configuring and managing a Towalink installation Home-page: https://
 www.towalink.net Author: The Towalink Project Author-email:
 pypi.tlm@towalink.net Project-URL: Project homepage, https://www.towalink.net
 Project-URL: Repository, https://www.github.com/towalink/tlm Project-URL:
 Documentation, https://towalink.readthedocs.io Keywords: Towalink VPN SD-WAN
 WireGuard Classifier: Programming Language :: Python Classifier: Programming
 Language :: Python :: 3 Classifier: License :: OSI Approved :: GNU Affero
 General Public License v3 or later (AGPLv3+) Classifier: Operating System ::
 POSIX :: Linux Classifier: Development Status :: 4 - Beta Classifier: Intended
 Audience :: System Administrators Classifier: Intended Audience :: Information
 Technology Classifier: Intended Audience :: Telecommunications Industry
 Classifier: Topic :: System :: Networking Requires-Python: >=3.6 Description-
-Content-Type: text/markdown License-File: LICENSE # tlm - Towalink Manager Tool
-for configuring and managing a Towalink installation. --- ## Documentation The
-documentation of the Towalink project can be found at https://
-towalink.readthedocs.io --- ## License [![License](http://img.shields.io/:
-license-agpl3-blue.svg?style=flat-square)](https://opensource.org/licenses/
-AGPL-3.0) - **[AGPL3 license](https://opensource.org/licenses/AGPL-3.0)** -
-Copyright 2020-2023 Â© _D_i_r_k_ _H_e_n_r_i_c_i.
+Content-Type: text/markdown License-File: LICENSE Requires-Dist: python-
+configuration Requires-Dist: jinja2 Requires-Dist: pyyaml Requires-Dist: toml
+Requires-Dist: tomlkit Requires-Dist: ansible Requires-Dist: wgconfig>=1.0.1 #
+tlm - Towalink Manager Tool for configuring and managing a Towalink
+installation. --- ## Documentation The documentation of the Towalink project
+can be found at https://towalink.readthedocs.io --- ## License [![License]
+(http://img.shields.io/:license-agpl3-blue.svg?style=flat-square)](https://
+opensource.org/licenses/AGPL-3.0) - **[AGPL3 license](https://opensource.org/
+licenses/AGPL-3.0)** - Copyright 2020-2023 Â© _D_i_r_k_ _H_e_n_r_i_c_i.
```

### Comparing `towalink_tlm-0.2.0/src/towalink_tlm.egg-info/SOURCES.txt` & `towalink_tlm-0.3.1/src/towalink_tlm.egg-info/SOURCES.txt`

 * *Files identical despite different names*

