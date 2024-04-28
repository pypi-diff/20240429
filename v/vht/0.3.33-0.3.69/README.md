# Comparing `tmp/vht-0.3.33.tar.gz` & `tmp/vht-0.3.69.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "vht-0.3.33.tar", last modified: Sat Mar 23 11:13:59 2024, max compression
+gzip compressed data, was "vht-0.3.69.tar", last modified: Sun Apr 28 23:48:37 2024, max compression
```

## Comparing `vht-0.3.33.tar` & `vht-0.3.69.tar`

### file list

```diff
@@ -1,134 +1,138 @@
-drwxrwxr-x   0 mal1ce    (1000) mal1ce    (1000)        0 2024-03-23 11:13:59.680609 vht-0.3.33/
--rw-r--r--   0 mal1ce    (1000) mal1ce    (1000)    35148 2022-12-31 13:17:54.000000 vht-0.3.33/LICENSE
--rw-r--r--   0 mal1ce    (1000) mal1ce    (1000)       49 2022-12-31 13:17:54.000000 vht-0.3.33/MANIFEST.in
--rw-r--r--   0 mal1ce    (1000) mal1ce    (1000)     1912 2024-03-23 11:13:59.680609 vht-0.3.33/PKG-INFO
--rw-r--r--   0 mal1ce    (1000) mal1ce    (1000)     1194 2023-08-11 00:51:13.000000 vht-0.3.33/README.md
-drwxrwxr-x   0 mal1ce    (1000) mal1ce    (1000)        0 2024-03-23 11:13:59.648611 vht-0.3.33/data/
-drwxrwxr-x   0 mal1ce    (1000) mal1ce    (1000)        0 2024-03-23 11:13:59.648611 vht-0.3.33/data/bank/
--rw-r--r--   0 mal1ce    (1000) mal1ce    (1000)     2430 2022-12-31 13:17:54.000000 vht-0.3.33/data/bank/10-gm1
--rw-r--r--   0 mal1ce    (1000) mal1ce    (1000)     4875 2022-12-31 13:17:54.000000 vht-0.3.33/data/bank/20-gm2
--rw-r--r--   0 mal1ce    (1000) mal1ce    (1000)      290 2022-12-31 13:17:54.000000 vht-0.3.33/data/com.github.rdybka.vht.desktop
-drwxrwxr-x   0 mal1ce    (1000) mal1ce    (1000)        0 2024-03-23 11:13:59.652611 vht-0.3.33/data/ctrl/
--rw-r--r--   0 mal1ce    (1000) mal1ce    (1000)      294 2022-12-31 13:17:54.000000 vht-0.3.33/data/ctrl/10-gm
--rw-r--r--   0 mal1ce    (1000) mal1ce    (1000)      166 2022-12-31 13:17:54.000000 vht-0.3.33/data/ctrl/20-zyn
--rw-r--r--   0 mal1ce    (1000) mal1ce    (1000)     4550 2022-12-31 13:17:54.000000 vht-0.3.33/data/mandy.png
--rw-r--r--   0 mal1ce    (1000) mal1ce    (1000)     1246 2022-12-31 13:17:54.000000 vht-0.3.33/data/menu.ui
--rw-r--r--   0 mal1ce    (1000) mal1ce    (1000)    11176 2022-12-31 13:17:54.000000 vht-0.3.33/data/vht.png
--rw-r--r--   0 mal1ce    (1000) mal1ce    (1000)     4458 2022-12-31 13:17:54.000000 vht-0.3.33/data/vht.svg
-drwxrwxr-x   0 mal1ce    (1000) mal1ce    (1000)        0 2024-03-23 11:13:59.652611 vht-0.3.33/doc/
--rw-rw-r--   0 mal1ce    (1000) mal1ce    (1000)     2361 2024-03-23 10:49:21.000000 vht-0.3.33/doc/vht.1.gz
--rw-r--r--   0 mal1ce    (1000) mal1ce    (1000)     4641 2023-09-11 08:35:38.000000 vht-0.3.33/doc/vht.1.md
-drwxrwxr-x   0 mal1ce    (1000) mal1ce    (1000)        0 2024-03-23 11:13:59.664610 vht-0.3.33/libvht/
--rw-r--r--   0 mal1ce    (1000) mal1ce    (1000)       75 2022-12-31 13:17:54.000000 vht-0.3.33/libvht/__init__.py
--rw-r--r--   0 mal1ce    (1000) mal1ce    (1000)     1538 2023-03-21 08:03:40.000000 vht-0.3.33/libvht/ctrlrow.c
--rw-r--r--   0 mal1ce    (1000) mal1ce    (1000)     1416 2022-12-31 13:17:54.000000 vht-0.3.33/libvht/ctrlrow.h
--rw-r--r--   0 mal1ce    (1000) mal1ce    (1000)     7095 2023-03-21 08:03:40.000000 vht-0.3.33/libvht/envelope.c
--rw-r--r--   0 mal1ce    (1000) mal1ce    (1000)     1612 2022-12-31 13:17:54.000000 vht-0.3.33/libvht/envelope.h
--rw-r--r--   0 mal1ce    (1000) mal1ce    (1000)     1960 2023-03-21 08:03:40.000000 vht-0.3.33/libvht/jack_process.c
--rw-r--r--   0 mal1ce    (1000) mal1ce    (1000)     1212 2022-12-31 13:17:54.000000 vht-0.3.33/libvht/jack_process.h
--rw-r--r--   0 mal1ce    (1000) mal1ce    (1000)    19730 2023-01-30 08:50:38.000000 vht-0.3.33/libvht/libcvht.h
--rw-r--r--   0 mal1ce    (1000) mal1ce    (1000)    31881 2024-03-23 11:03:40.000000 vht-0.3.33/libvht/libcvht.py
--rw-rw-r--   0 mal1ce    (1000) mal1ce    (1000)   477234 2024-03-23 11:03:40.000000 vht-0.3.33/libvht/libcvht_wrap.c
--rw-r--r--   0 mal1ce    (1000) mal1ce    (1000)     8287 2023-03-21 08:03:40.000000 vht-0.3.33/libvht/libvht.c
--rw-r--r--   0 mal1ce    (1000) mal1ce    (1000)    34606 2024-03-22 10:51:15.000000 vht-0.3.33/libvht/mandy.c
--rw-r--r--   0 mal1ce    (1000) mal1ce    (1000)     6088 2023-03-31 14:55:44.000000 vht-0.3.33/libvht/mandy.h
--rw-r--r--   0 mal1ce    (1000) mal1ce    (1000)     2354 2023-03-21 08:03:40.000000 vht-0.3.33/libvht/mandy_pix_scan.c
--rw-r--r--   0 mal1ce    (1000) mal1ce    (1000)     1001 2022-12-31 13:17:54.000000 vht-0.3.33/libvht/mandy_pix_scan.h
--rw-r--r--   0 mal1ce    (1000) mal1ce    (1000)     7405 2023-03-21 08:03:40.000000 vht-0.3.33/libvht/mandy_trk_disp.c
--rw-r--r--   0 mal1ce    (1000) mal1ce    (1000)      986 2022-12-31 13:17:54.000000 vht-0.3.33/libvht/mandy_trk_disp.h
--rw-r--r--   0 mal1ce    (1000) mal1ce    (1000)    16444 2023-03-21 08:03:40.000000 vht-0.3.33/libvht/midi_client.c
--rw-r--r--   0 mal1ce    (1000) mal1ce    (1000)     4381 2022-12-31 13:17:54.000000 vht-0.3.33/libvht/midi_client.h
--rw-r--r--   0 mal1ce    (1000) mal1ce    (1000)     3496 2023-03-21 08:03:40.000000 vht-0.3.33/libvht/midi_event.c
--rw-r--r--   0 mal1ce    (1000) mal1ce    (1000)     1540 2022-12-31 13:17:54.000000 vht-0.3.33/libvht/midi_event.h
--rw-r--r--   0 mal1ce    (1000) mal1ce    (1000)    15439 2023-03-21 08:03:40.000000 vht-0.3.33/libvht/module.c
--rw-r--r--   0 mal1ce    (1000) mal1ce    (1000)     3151 2022-12-31 13:17:54.000000 vht-0.3.33/libvht/module.h
--rw-r--r--   0 mal1ce    (1000) mal1ce    (1000)     3036 2023-03-21 08:03:40.000000 vht-0.3.33/libvht/row.c
--rw-r--r--   0 mal1ce    (1000) mal1ce    (1000)     1670 2022-12-31 13:17:54.000000 vht-0.3.33/libvht/row.h
--rw-rw-r--   0 mal1ce    (1000) mal1ce    (1000)    28781 2024-03-23 10:37:55.000000 vht-0.3.33/libvht/sequence.c
--rw-r--r--   0 mal1ce    (1000) mal1ce    (1000)     4464 2022-12-31 13:17:54.000000 vht-0.3.33/libvht/sequence.h
--rw-r--r--   0 mal1ce    (1000) mal1ce    (1000)    29202 2023-03-23 02:07:54.000000 vht-0.3.33/libvht/timeline.c
--rw-r--r--   0 mal1ce    (1000) mal1ce    (1000)     4538 2022-12-31 13:17:54.000000 vht-0.3.33/libvht/timeline.h
--rw-r--r--   0 mal1ce    (1000) mal1ce    (1000)    41059 2023-03-21 08:03:40.000000 vht-0.3.33/libvht/track.c
--rw-r--r--   0 mal1ce    (1000) mal1ce    (1000)     4153 2023-01-30 08:43:51.000000 vht-0.3.33/libvht/track.h
--rw-r--r--   0 mal1ce    (1000) mal1ce    (1000)     4675 2023-03-21 08:03:40.000000 vht-0.3.33/libvht/tracy.c
--rw-r--r--   0 mal1ce    (1000) mal1ce    (1000)     2370 2023-03-20 13:26:10.000000 vht-0.3.33/libvht/tracy.h
--rw-r--r--   0 mal1ce    (1000) mal1ce    (1000)     1882 2023-03-21 08:03:58.000000 vht-0.3.33/libvht/vhtcolumn.py
--rw-r--r--   0 mal1ce    (1000) mal1ce    (1000)     2639 2023-03-21 08:03:58.000000 vht-0.3.33/libvht/vhtctrl.py
--rw-r--r--   0 mal1ce    (1000) mal1ce    (1000)     2012 2023-03-21 08:03:58.000000 vht-0.3.33/libvht/vhtctrllist.py
--rw-r--r--   0 mal1ce    (1000) mal1ce    (1000)     3639 2023-03-21 08:03:58.000000 vht-0.3.33/libvht/vhtctrlrow.py
--rw-r--r--   0 mal1ce    (1000) mal1ce    (1000)     1973 2023-03-21 08:03:58.000000 vht-0.3.33/libvht/vhtextras.py
--rw-r--r--   0 mal1ce    (1000) mal1ce    (1000)     6566 2023-03-21 08:03:58.000000 vht-0.3.33/libvht/vhtmandy.py
--rw-r--r--   0 mal1ce    (1000) mal1ce    (1000)    21012 2023-03-21 08:03:58.000000 vht-0.3.33/libvht/vhtmodule.py
--rw-r--r--   0 mal1ce    (1000) mal1ce    (1000)     3283 2023-03-21 08:03:58.000000 vht-0.3.33/libvht/vhtport.py
--rw-r--r--   0 mal1ce    (1000) mal1ce    (1000)     2404 2023-03-21 08:03:58.000000 vht-0.3.33/libvht/vhtports.py
--rw-r--r--   0 mal1ce    (1000) mal1ce    (1000)     1922 2023-03-21 08:03:58.000000 vht-0.3.33/libvht/vhtquicklist.py
--rw-r--r--   0 mal1ce    (1000) mal1ce    (1000)     5623 2023-03-21 08:03:58.000000 vht-0.3.33/libvht/vhtrow.py
--rw-r--r--   0 mal1ce    (1000) mal1ce    (1000)    10811 2024-03-21 12:58:15.000000 vht-0.3.33/libvht/vhtsequence.py
--rw-r--r--   0 mal1ce    (1000) mal1ce    (1000)     3751 2023-03-21 08:03:58.000000 vht-0.3.33/libvht/vhttimeline.py
--rw-r--r--   0 mal1ce    (1000) mal1ce    (1000)     1887 2023-03-21 08:03:58.000000 vht-0.3.33/libvht/vhttimelinechange.py
--rw-r--r--   0 mal1ce    (1000) mal1ce    (1000)     2204 2023-03-21 08:03:58.000000 vht-0.3.33/libvht/vhttimelinechanges.py
--rw-r--r--   0 mal1ce    (1000) mal1ce    (1000)     1686 2023-03-21 08:03:58.000000 vht-0.3.33/libvht/vhttimelineloop.py
--rw-r--r--   0 mal1ce    (1000) mal1ce    (1000)     1913 2023-03-21 08:03:58.000000 vht-0.3.33/libvht/vhttimelineslices.py
--rw-r--r--   0 mal1ce    (1000) mal1ce    (1000)     5262 2023-03-21 08:03:58.000000 vht-0.3.33/libvht/vhttimelinestrip.py
--rw-r--r--   0 mal1ce    (1000) mal1ce    (1000)     3637 2023-03-21 08:03:58.000000 vht-0.3.33/libvht/vhttimelinestrips.py
--rw-r--r--   0 mal1ce    (1000) mal1ce    (1000)     1454 2023-03-21 08:03:58.000000 vht-0.3.33/libvht/vhttimelineticks.py
--rw-r--r--   0 mal1ce    (1000) mal1ce    (1000)     9143 2023-03-21 08:03:58.000000 vht-0.3.33/libvht/vhttrack.py
--rw-r--r--   0 mal1ce    (1000) mal1ce    (1000)     2270 2023-03-21 08:03:58.000000 vht-0.3.33/libvht/vhttracy.py
--rw-r--r--   0 mal1ce    (1000) mal1ce    (1000)     1693 2024-03-23 10:48:25.000000 vht-0.3.33/pyproject.toml
--rw-r--r--   0 mal1ce    (1000) mal1ce    (1000)      108 2024-03-23 11:13:59.680609 vht-0.3.33/setup.cfg
--rwxr--r--   0 mal1ce    (1000) mal1ce    (1000)     1796 2024-03-23 10:48:14.000000 vht-0.3.33/setup.py
-drwxrwxr-x   0 mal1ce    (1000) mal1ce    (1000)        0 2024-03-23 11:13:59.676609 vht-0.3.33/vht/
--rw-r--r--   0 mal1ce    (1000) mal1ce    (1000)      124 2022-12-31 13:17:54.000000 vht-0.3.33/vht/__init__.py
--rw-r--r--   0 mal1ce    (1000) mal1ce    (1000)     1088 2023-03-21 08:04:15.000000 vht-0.3.33/vht/autoexec.py
--rw-r--r--   0 mal1ce    (1000) mal1ce    (1000)     3531 2023-03-21 08:04:15.000000 vht-0.3.33/vht/bankcfg.py
--rw-r--r--   0 mal1ce    (1000) mal1ce    (1000)     1688 2023-03-21 08:04:15.000000 vht-0.3.33/vht/capturebutton.py
--rw-r--r--   0 mal1ce    (1000) mal1ce    (1000)    23674 2023-03-23 01:55:40.000000 vht-0.3.33/vht/configuration.py
--rw-r--r--   0 mal1ce    (1000) mal1ce    (1000)     5836 2023-03-21 08:04:15.000000 vht-0.3.33/vht/console.py
--rw-r--r--   0 mal1ce    (1000) mal1ce    (1000)    55124 2023-03-21 08:04:15.000000 vht-0.3.33/vht/controllereditor.py
--rw-r--r--   0 mal1ce    (1000) mal1ce    (1000)     6976 2023-03-21 08:04:15.000000 vht-0.3.33/vht/controllersview.py
--rw-r--r--   0 mal1ce    (1000) mal1ce    (1000)     5705 2023-03-21 08:04:15.000000 vht-0.3.33/vht/controllersviewrow.py
--rw-r--r--   0 mal1ce    (1000) mal1ce    (1000)     4560 2023-03-21 08:04:15.000000 vht-0.3.33/vht/controllerundobuffer.py
--rw-r--r--   0 mal1ce    (1000) mal1ce    (1000)     2909 2023-03-21 08:04:15.000000 vht-0.3.33/vht/ctrlcfg.py
--rw-r--r--   0 mal1ce    (1000) mal1ce    (1000)     1910 2023-03-21 08:04:15.000000 vht-0.3.33/vht/extras.py
--rw-r--r--   0 mal1ce    (1000) mal1ce    (1000)     1298 2023-03-21 08:04:15.000000 vht-0.3.33/vht/filerotator.py
--rwxr--r--   0 mal1ce    (1000) mal1ce    (1000)    11446 2024-03-22 12:13:50.000000 vht-0.3.33/vht/main.py
--rw-r--r--   0 mal1ce    (1000) mal1ce    (1000)    18385 2023-03-21 08:04:15.000000 vht-0.3.33/vht/mainwin.py
--rw-r--r--   0 mal1ce    (1000) mal1ce    (1000)    14192 2023-03-21 08:04:15.000000 vht-0.3.33/vht/mandymenu.py
--rw-r--r--   0 mal1ce    (1000) mal1ce    (1000)    18143 2024-03-22 11:55:36.000000 vht-0.3.33/vht/mandyview.py
--rw-r--r--   0 mal1ce    (1000) mal1ce    (1000)     2401 2023-03-21 08:04:15.000000 vht-0.3.33/vht/midimapview.py
--rw-r--r--   0 mal1ce    (1000) mal1ce    (1000)     4176 2023-03-21 08:04:15.000000 vht-0.3.33/vht/midimapviewrow.py
--rw-r--r--   0 mal1ce    (1000) mal1ce    (1000)     1299 2023-03-21 08:04:15.000000 vht-0.3.33/vht/notebooklabel.py
--rw-r--r--   0 mal1ce    (1000) mal1ce    (1000)     4721 2024-03-22 16:50:28.000000 vht-0.3.33/vht/poormanspiano.py
--rw-r--r--   0 mal1ce    (1000) mal1ce    (1000)     2677 2023-03-21 08:04:15.000000 vht-0.3.33/vht/portconfig.py
--rw-r--r--   0 mal1ce    (1000) mal1ce    (1000)     3547 2023-03-21 08:04:15.000000 vht-0.3.33/vht/portconfigpopover.py
--rw-r--r--   0 mal1ce    (1000) mal1ce    (1000)     7557 2023-03-21 08:04:15.000000 vht-0.3.33/vht/portconfigview.py
--rw-r--r--   0 mal1ce    (1000) mal1ce    (1000)    23430 2024-03-22 12:14:50.000000 vht-0.3.33/vht/preferenceswin.py
--rw-r--r--   0 mal1ce    (1000) mal1ce    (1000)     6623 2023-03-21 08:04:15.000000 vht-0.3.33/vht/probeditor.py
--rw-r--r--   0 mal1ce    (1000) mal1ce    (1000)     4996 2023-03-21 08:04:15.000000 vht-0.3.33/vht/propview.py
--rw-r--r--   0 mal1ce    (1000) mal1ce    (1000)     1035 2023-03-21 08:04:15.000000 vht-0.3.33/vht/pulsar.py
--rw-r--r--   0 mal1ce    (1000) mal1ce    (1000)     1100 2023-03-21 08:04:15.000000 vht-0.3.33/vht/randomcomposer.py
--rw-r--r--   0 mal1ce    (1000) mal1ce    (1000)     7264 2023-03-21 08:04:15.000000 vht-0.3.33/vht/renderer.py
--rw-r--r--   0 mal1ce    (1000) mal1ce    (1000)     9217 2023-03-21 08:04:15.000000 vht-0.3.33/vht/renderwin.py
--rw-r--r--   0 mal1ce    (1000) mal1ce    (1000)    15715 2023-03-21 08:04:15.000000 vht-0.3.33/vht/sequencelistview.py
--rw-r--r--   0 mal1ce    (1000) mal1ce    (1000)     7775 2023-03-21 12:19:50.000000 vht-0.3.33/vht/sequencelistviewpopover.py
--rw-r--r--   0 mal1ce    (1000) mal1ce    (1000)    11262 2023-03-21 08:04:15.000000 vht-0.3.33/vht/sequencepropviewpopover.py
--rw-r--r--   0 mal1ce    (1000) mal1ce    (1000)    12223 2023-03-21 12:19:50.000000 vht-0.3.33/vht/sequencetriggersview.py
--rw-r--r--   0 mal1ce    (1000) mal1ce    (1000)    37154 2024-03-22 14:06:25.000000 vht-0.3.33/vht/sequenceview.py
--rw-r--r--   0 mal1ce    (1000) mal1ce    (1000)     6678 2023-03-21 08:04:15.000000 vht-0.3.33/vht/shortcutmayhem.py
--rw-r--r--   0 mal1ce    (1000) mal1ce    (1000)    20316 2024-03-22 16:23:30.000000 vht-0.3.33/vht/sidetrackview.py
--rw-r--r--   0 mal1ce    (1000) mal1ce    (1000)    19524 2023-09-09 20:22:06.000000 vht-0.3.33/vht/statusbar.py
--rw-r--r--   0 mal1ce    (1000) mal1ce    (1000)     2879 2023-03-21 08:04:15.000000 vht-0.3.33/vht/thumbmanager.py
--rw-r--r--   0 mal1ce    (1000) mal1ce    (1000)    51601 2023-03-21 08:04:15.000000 vht-0.3.33/vht/timelineview.py
--rw-r--r--   0 mal1ce    (1000) mal1ce    (1000)     6308 2023-03-21 08:04:15.000000 vht-0.3.33/vht/timeshifteditor.py
--rw-r--r--   0 mal1ce    (1000) mal1ce    (1000)    22027 2023-03-21 08:04:15.000000 vht-0.3.33/vht/trackpropview.py
--rw-r--r--   0 mal1ce    (1000) mal1ce    (1000)    31965 2023-03-21 08:04:15.000000 vht-0.3.33/vht/trackpropviewpopover.py
--rw-r--r--   0 mal1ce    (1000) mal1ce    (1000)     3229 2023-03-21 08:04:15.000000 vht-0.3.33/vht/trackundobuffer.py
--rw-r--r--   0 mal1ce    (1000) mal1ce    (1000)    96092 2024-03-22 15:55:48.000000 vht-0.3.33/vht/trackview.py
--rw-r--r--   0 mal1ce    (1000) mal1ce    (1000)     9212 2023-03-21 08:04:15.000000 vht-0.3.33/vht/trackviewpointer.py
--rw-r--r--   0 mal1ce    (1000) mal1ce    (1000)     8127 2023-03-21 08:04:15.000000 vht-0.3.33/vht/velocityeditor.py
-drwxrwxr-x   0 mal1ce    (1000) mal1ce    (1000)        0 2024-03-23 11:13:59.680609 vht-0.3.33/vht.egg-info/
--rw-r--r--   0 mal1ce    (1000) mal1ce    (1000)     1912 2024-03-23 11:13:59.000000 vht-0.3.33/vht.egg-info/PKG-INFO
--rw-rw-r--   0 mal1ce    (1000) mal1ce    (1000)     2458 2024-03-23 11:13:59.000000 vht-0.3.33/vht.egg-info/SOURCES.txt
--rw-rw-r--   0 mal1ce    (1000) mal1ce    (1000)        1 2024-03-23 11:13:59.000000 vht-0.3.33/vht.egg-info/dependency_links.txt
--rw-rw-r--   0 mal1ce    (1000) mal1ce    (1000)       37 2024-03-23 11:13:59.000000 vht-0.3.33/vht.egg-info/entry_points.txt
--rw-rw-r--   0 mal1ce    (1000) mal1ce    (1000)       27 2024-03-23 11:13:59.000000 vht-0.3.33/vht.egg-info/top_level.txt
+drwxrwxr-x   0 mal1ce    (1000) mal1ce    (1000)        0 2024-04-28 23:48:37.426646 vht-0.3.69/
+-rw-r--r--   0 mal1ce    (1000) mal1ce    (1000)    35148 2022-12-31 13:17:54.000000 vht-0.3.69/LICENSE
+-rw-r--r--   0 mal1ce    (1000) mal1ce    (1000)       49 2022-12-31 13:17:54.000000 vht-0.3.69/MANIFEST.in
+-rw-r--r--   0 mal1ce    (1000) mal1ce    (1000)     1912 2024-04-28 23:48:37.426646 vht-0.3.69/PKG-INFO
+-rw-r--r--   0 mal1ce    (1000) mal1ce    (1000)     1194 2023-08-11 00:51:13.000000 vht-0.3.69/README.md
+drwxrwxr-x   0 mal1ce    (1000) mal1ce    (1000)        0 2024-04-28 23:48:37.402646 vht-0.3.69/data/
+drwxrwxr-x   0 mal1ce    (1000) mal1ce    (1000)        0 2024-04-28 23:48:37.402646 vht-0.3.69/data/bank/
+-rw-r--r--   0 mal1ce    (1000) mal1ce    (1000)     2430 2022-12-31 13:17:54.000000 vht-0.3.69/data/bank/10-gm1
+-rw-r--r--   0 mal1ce    (1000) mal1ce    (1000)     4875 2022-12-31 13:17:54.000000 vht-0.3.69/data/bank/20-gm2
+-rw-r--r--   0 mal1ce    (1000) mal1ce    (1000)      290 2022-12-31 13:17:54.000000 vht-0.3.69/data/com.github.rdybka.vht.desktop
+drwxrwxr-x   0 mal1ce    (1000) mal1ce    (1000)        0 2024-04-28 23:48:37.402646 vht-0.3.69/data/ctrl/
+-rw-r--r--   0 mal1ce    (1000) mal1ce    (1000)      294 2022-12-31 13:17:54.000000 vht-0.3.69/data/ctrl/10-gm
+-rw-r--r--   0 mal1ce    (1000) mal1ce    (1000)      166 2022-12-31 13:17:54.000000 vht-0.3.69/data/ctrl/20-zyn
+-rw-r--r--   0 mal1ce    (1000) mal1ce    (1000)     4550 2022-12-31 13:17:54.000000 vht-0.3.69/data/mandy.png
+-rw-r--r--   0 mal1ce    (1000) mal1ce    (1000)     1246 2022-12-31 13:17:54.000000 vht-0.3.69/data/menu.ui
+-rw-r--r--   0 mal1ce    (1000) mal1ce    (1000)    11176 2022-12-31 13:17:54.000000 vht-0.3.69/data/vht.png
+-rw-r--r--   0 mal1ce    (1000) mal1ce    (1000)     4458 2022-12-31 13:17:54.000000 vht-0.3.69/data/vht.svg
+drwxrwxr-x   0 mal1ce    (1000) mal1ce    (1000)        0 2024-04-28 23:48:37.402646 vht-0.3.69/doc/
+-rw-rw-r--   0 mal1ce    (1000) mal1ce    (1000)     2364 2024-04-28 23:29:39.000000 vht-0.3.69/doc/vht.1.gz
+-rw-r--r--   0 mal1ce    (1000) mal1ce    (1000)     4643 2024-04-28 23:29:30.000000 vht-0.3.69/doc/vht.1.md
+drwxrwxr-x   0 mal1ce    (1000) mal1ce    (1000)        0 2024-04-28 23:48:37.414646 vht-0.3.69/libvht/
+-rw-r--r--   0 mal1ce    (1000) mal1ce    (1000)       75 2022-12-31 13:17:54.000000 vht-0.3.69/libvht/__init__.py
+-rw-r--r--   0 mal1ce    (1000) mal1ce    (1000)     1538 2023-03-21 08:03:40.000000 vht-0.3.69/libvht/ctrlrow.c
+-rw-r--r--   0 mal1ce    (1000) mal1ce    (1000)     1416 2022-12-31 13:17:54.000000 vht-0.3.69/libvht/ctrlrow.h
+-rw-r--r--   0 mal1ce    (1000) mal1ce    (1000)     7095 2023-03-21 08:03:40.000000 vht-0.3.69/libvht/envelope.c
+-rw-r--r--   0 mal1ce    (1000) mal1ce    (1000)     1612 2022-12-31 13:17:54.000000 vht-0.3.69/libvht/envelope.h
+-rw-rw-r--   0 mal1ce    (1000) mal1ce    (1000)     1961 2024-04-20 19:24:40.000000 vht-0.3.69/libvht/jack_process.c
+-rw-r--r--   0 mal1ce    (1000) mal1ce    (1000)     1212 2022-12-31 13:17:54.000000 vht-0.3.69/libvht/jack_process.h
+-rw-r--r--   0 mal1ce    (1000) mal1ce    (1000)    19982 2024-04-28 12:26:17.000000 vht-0.3.69/libvht/libcvht.h
+-rw-r--r--   0 mal1ce    (1000) mal1ce    (1000)    32223 2024-04-28 23:29:38.000000 vht-0.3.69/libvht/libcvht.py
+-rw-rw-r--   0 mal1ce    (1000) mal1ce    (1000)   481702 2024-04-28 23:29:38.000000 vht-0.3.69/libvht/libcvht_wrap.c
+-rw-r--r--   0 mal1ce    (1000) mal1ce    (1000)     8287 2023-03-21 08:03:40.000000 vht-0.3.69/libvht/libvht.c
+-rw-r--r--   0 mal1ce    (1000) mal1ce    (1000)    34608 2024-04-08 16:06:43.000000 vht-0.3.69/libvht/mandy.c
+-rw-r--r--   0 mal1ce    (1000) mal1ce    (1000)     6088 2023-03-31 14:55:44.000000 vht-0.3.69/libvht/mandy.h
+-rw-r--r--   0 mal1ce    (1000) mal1ce    (1000)     2354 2023-03-21 08:03:40.000000 vht-0.3.69/libvht/mandy_pix_scan.c
+-rw-r--r--   0 mal1ce    (1000) mal1ce    (1000)     1001 2022-12-31 13:17:54.000000 vht-0.3.69/libvht/mandy_pix_scan.h
+-rw-r--r--   0 mal1ce    (1000) mal1ce    (1000)     7405 2023-03-21 08:03:40.000000 vht-0.3.69/libvht/mandy_trk_disp.c
+-rw-r--r--   0 mal1ce    (1000) mal1ce    (1000)      986 2022-12-31 13:17:54.000000 vht-0.3.69/libvht/mandy_trk_disp.h
+-rw-rw-r--   0 mal1ce    (1000) mal1ce    (1000)    17029 2024-04-20 19:24:40.000000 vht-0.3.69/libvht/midi_client.c
+-rw-r--r--   0 mal1ce    (1000) mal1ce    (1000)     4512 2024-04-14 23:40:36.000000 vht-0.3.69/libvht/midi_client.h
+-rw-r--r--   0 mal1ce    (1000) mal1ce    (1000)     3496 2023-03-21 08:03:40.000000 vht-0.3.69/libvht/midi_event.c
+-rw-r--r--   0 mal1ce    (1000) mal1ce    (1000)     1540 2022-12-31 13:17:54.000000 vht-0.3.69/libvht/midi_event.h
+-rw-rw-r--   0 mal1ce    (1000) mal1ce    (1000)    16010 2024-04-22 08:56:08.000000 vht-0.3.69/libvht/module.c
+-rw-r--r--   0 mal1ce    (1000) mal1ce    (1000)     3256 2024-04-22 08:54:58.000000 vht-0.3.69/libvht/module.h
+-rw-r--r--   0 mal1ce    (1000) mal1ce    (1000)     3036 2023-03-21 08:03:40.000000 vht-0.3.69/libvht/row.c
+-rw-r--r--   0 mal1ce    (1000) mal1ce    (1000)     1670 2022-12-31 13:17:54.000000 vht-0.3.69/libvht/row.h
+-rw-rw-r--   0 mal1ce    (1000) mal1ce    (1000)    28979 2024-04-28 13:47:56.000000 vht-0.3.69/libvht/sequence.c
+-rw-rw-r--   0 mal1ce    (1000) mal1ce    (1000)     4502 2024-04-28 12:25:10.000000 vht-0.3.69/libvht/sequence.h
+-rw-rw-r--   0 mal1ce    (1000) mal1ce    (1000)     6457 2024-04-22 10:40:58.000000 vht-0.3.69/libvht/smf.c
+-rw-rw-r--   0 mal1ce    (1000) mal1ce    (1000)     1680 2024-04-22 08:52:28.000000 vht-0.3.69/libvht/smf.h
+-rw-rw-r--   0 mal1ce    (1000) mal1ce    (1000)     2912 2024-04-20 23:47:04.000000 vht-0.3.69/libvht/stolen.c
+-rw-r--r--   0 mal1ce    (1000) mal1ce    (1000)    29202 2023-03-23 02:07:54.000000 vht-0.3.69/libvht/timeline.c
+-rw-r--r--   0 mal1ce    (1000) mal1ce    (1000)     4538 2022-12-31 13:17:54.000000 vht-0.3.69/libvht/timeline.h
+-rw-r--r--   0 mal1ce    (1000) mal1ce    (1000)    41059 2023-03-21 08:03:40.000000 vht-0.3.69/libvht/track.c
+-rw-r--r--   0 mal1ce    (1000) mal1ce    (1000)     4153 2023-01-30 08:43:51.000000 vht-0.3.69/libvht/track.h
+-rw-r--r--   0 mal1ce    (1000) mal1ce    (1000)     4675 2024-04-08 11:52:27.000000 vht-0.3.69/libvht/tracy.c
+-rw-r--r--   0 mal1ce    (1000) mal1ce    (1000)     2370 2024-04-08 11:52:18.000000 vht-0.3.69/libvht/tracy.h
+-rw-r--r--   0 mal1ce    (1000) mal1ce    (1000)     1882 2023-03-21 08:03:58.000000 vht-0.3.69/libvht/vhtcolumn.py
+-rw-r--r--   0 mal1ce    (1000) mal1ce    (1000)     2639 2023-03-21 08:03:58.000000 vht-0.3.69/libvht/vhtctrl.py
+-rw-r--r--   0 mal1ce    (1000) mal1ce    (1000)     2012 2023-03-21 08:03:58.000000 vht-0.3.69/libvht/vhtctrllist.py
+-rw-r--r--   0 mal1ce    (1000) mal1ce    (1000)     3639 2023-03-21 08:03:58.000000 vht-0.3.69/libvht/vhtctrlrow.py
+-rw-r--r--   0 mal1ce    (1000) mal1ce    (1000)     1973 2023-03-21 08:03:58.000000 vht-0.3.69/libvht/vhtextras.py
+-rw-r--r--   0 mal1ce    (1000) mal1ce    (1000)     6566 2023-03-21 08:03:58.000000 vht-0.3.69/libvht/vhtmandy.py
+-rw-r--r--   0 mal1ce    (1000) mal1ce    (1000)    21144 2024-04-22 09:54:53.000000 vht-0.3.69/libvht/vhtmodule.py
+-rw-r--r--   0 mal1ce    (1000) mal1ce    (1000)     3432 2024-04-14 19:43:50.000000 vht-0.3.69/libvht/vhtport.py
+-rw-r--r--   0 mal1ce    (1000) mal1ce    (1000)     2404 2024-04-09 00:56:37.000000 vht-0.3.69/libvht/vhtports.py
+-rw-r--r--   0 mal1ce    (1000) mal1ce    (1000)     1922 2023-03-21 08:03:58.000000 vht-0.3.69/libvht/vhtquicklist.py
+-rw-r--r--   0 mal1ce    (1000) mal1ce    (1000)     5623 2023-03-21 08:03:58.000000 vht-0.3.69/libvht/vhtrow.py
+-rw-r--r--   0 mal1ce    (1000) mal1ce    (1000)    10975 2024-04-28 12:27:13.000000 vht-0.3.69/libvht/vhtsequence.py
+-rw-r--r--   0 mal1ce    (1000) mal1ce    (1000)     3751 2023-03-21 08:03:58.000000 vht-0.3.69/libvht/vhttimeline.py
+-rw-r--r--   0 mal1ce    (1000) mal1ce    (1000)     1887 2023-03-21 08:03:58.000000 vht-0.3.69/libvht/vhttimelinechange.py
+-rw-r--r--   0 mal1ce    (1000) mal1ce    (1000)     2204 2023-03-21 08:03:58.000000 vht-0.3.69/libvht/vhttimelinechanges.py
+-rw-r--r--   0 mal1ce    (1000) mal1ce    (1000)     1686 2023-03-21 08:03:58.000000 vht-0.3.69/libvht/vhttimelineloop.py
+-rw-r--r--   0 mal1ce    (1000) mal1ce    (1000)     1913 2023-03-21 08:03:58.000000 vht-0.3.69/libvht/vhttimelineslices.py
+-rw-r--r--   0 mal1ce    (1000) mal1ce    (1000)     5262 2023-03-21 08:03:58.000000 vht-0.3.69/libvht/vhttimelinestrip.py
+-rw-r--r--   0 mal1ce    (1000) mal1ce    (1000)     3637 2023-03-21 08:03:58.000000 vht-0.3.69/libvht/vhttimelinestrips.py
+-rw-r--r--   0 mal1ce    (1000) mal1ce    (1000)     1454 2023-03-21 08:03:58.000000 vht-0.3.69/libvht/vhttimelineticks.py
+-rw-r--r--   0 mal1ce    (1000) mal1ce    (1000)     9143 2023-03-21 08:03:58.000000 vht-0.3.69/libvht/vhttrack.py
+-rw-r--r--   0 mal1ce    (1000) mal1ce    (1000)     2270 2023-03-21 08:03:58.000000 vht-0.3.69/libvht/vhttracy.py
+-rw-r--r--   0 mal1ce    (1000) mal1ce    (1000)     1791 2024-04-28 23:44:34.000000 vht-0.3.69/pyproject.toml
+-rw-r--r--   0 mal1ce    (1000) mal1ce    (1000)       70 2024-04-28 23:48:37.426646 vht-0.3.69/setup.cfg
+-rwxr--r--   0 mal1ce    (1000) mal1ce    (1000)     1837 2024-04-28 23:32:00.000000 vht-0.3.69/setup.py
+drwxrwxr-x   0 mal1ce    (1000) mal1ce    (1000)        0 2024-04-28 23:48:37.422646 vht-0.3.69/vht/
+-rw-r--r--   0 mal1ce    (1000) mal1ce    (1000)      124 2022-12-31 13:17:54.000000 vht-0.3.69/vht/__init__.py
+-rw-r--r--   0 mal1ce    (1000) mal1ce    (1000)     1088 2023-03-21 08:04:15.000000 vht-0.3.69/vht/autoexec.py
+-rw-r--r--   0 mal1ce    (1000) mal1ce    (1000)     3531 2023-03-21 08:04:15.000000 vht-0.3.69/vht/bankcfg.py
+-rw-r--r--   0 mal1ce    (1000) mal1ce    (1000)     1688 2024-04-26 02:28:28.000000 vht-0.3.69/vht/capturebutton.py
+-rw-rw-r--   0 mal1ce    (1000) mal1ce    (1000)     3834 2024-04-28 13:24:55.000000 vht-0.3.69/vht/codedaemon.py
+-rw-r--r--   0 mal1ce    (1000) mal1ce    (1000)    24274 2024-04-22 09:13:03.000000 vht-0.3.69/vht/configuration.py
+-rw-r--r--   0 mal1ce    (1000) mal1ce    (1000)     5836 2023-03-21 08:04:15.000000 vht-0.3.69/vht/console.py
+-rw-r--r--   0 mal1ce    (1000) mal1ce    (1000)    55124 2023-03-21 08:04:15.000000 vht-0.3.69/vht/controllereditor.py
+-rw-r--r--   0 mal1ce    (1000) mal1ce    (1000)     6976 2023-03-21 08:04:15.000000 vht-0.3.69/vht/controllersview.py
+-rw-r--r--   0 mal1ce    (1000) mal1ce    (1000)     5705 2023-03-21 08:04:15.000000 vht-0.3.69/vht/controllersviewrow.py
+-rw-r--r--   0 mal1ce    (1000) mal1ce    (1000)     4560 2023-03-21 08:04:15.000000 vht-0.3.69/vht/controllerundobuffer.py
+-rw-r--r--   0 mal1ce    (1000) mal1ce    (1000)     2909 2023-03-21 08:04:15.000000 vht-0.3.69/vht/ctrlcfg.py
+-rw-r--r--   0 mal1ce    (1000) mal1ce    (1000)     1910 2023-03-21 08:04:15.000000 vht-0.3.69/vht/extras.py
+-rw-r--r--   0 mal1ce    (1000) mal1ce    (1000)     1298 2023-03-21 08:04:15.000000 vht-0.3.69/vht/filerotator.py
+-rwxr--r--   0 mal1ce    (1000) mal1ce    (1000)    11500 2024-04-27 16:39:10.000000 vht-0.3.69/vht/main.py
+-rw-r--r--   0 mal1ce    (1000) mal1ce    (1000)    18460 2024-04-28 12:22:47.000000 vht-0.3.69/vht/mainwin.py
+-rw-r--r--   0 mal1ce    (1000) mal1ce    (1000)    14192 2023-03-21 08:04:15.000000 vht-0.3.69/vht/mandymenu.py
+-rw-r--r--   0 mal1ce    (1000) mal1ce    (1000)    18144 2024-04-08 12:16:06.000000 vht-0.3.69/vht/mandyview.py
+-rw-r--r--   0 mal1ce    (1000) mal1ce    (1000)     2401 2023-03-21 08:04:15.000000 vht-0.3.69/vht/midimapview.py
+-rw-r--r--   0 mal1ce    (1000) mal1ce    (1000)     4176 2023-03-21 08:04:15.000000 vht-0.3.69/vht/midimapviewrow.py
+-rw-r--r--   0 mal1ce    (1000) mal1ce    (1000)     1299 2023-03-21 08:04:15.000000 vht-0.3.69/vht/notebooklabel.py
+-rw-r--r--   0 mal1ce    (1000) mal1ce    (1000)     4721 2024-03-22 16:50:28.000000 vht-0.3.69/vht/poormanspiano.py
+-rw-r--r--   0 mal1ce    (1000) mal1ce    (1000)     2677 2024-04-14 21:33:38.000000 vht-0.3.69/vht/portconfig.py
+-rw-r--r--   0 mal1ce    (1000) mal1ce    (1000)     3547 2023-03-21 08:04:15.000000 vht-0.3.69/vht/portconfigpopover.py
+-rw-r--r--   0 mal1ce    (1000) mal1ce    (1000)     7615 2024-04-14 19:32:45.000000 vht-0.3.69/vht/portconfigview.py
+-rw-r--r--   0 mal1ce    (1000) mal1ce    (1000)    24666 2024-04-22 09:57:34.000000 vht-0.3.69/vht/preferenceswin.py
+-rw-r--r--   0 mal1ce    (1000) mal1ce    (1000)     6623 2023-03-21 08:04:15.000000 vht-0.3.69/vht/probeditor.py
+-rw-r--r--   0 mal1ce    (1000) mal1ce    (1000)     4996 2023-03-21 08:04:15.000000 vht-0.3.69/vht/propview.py
+-rw-r--r--   0 mal1ce    (1000) mal1ce    (1000)     1035 2023-03-21 08:04:15.000000 vht-0.3.69/vht/pulsar.py
+-rw-r--r--   0 mal1ce    (1000) mal1ce    (1000)     1100 2023-03-21 08:04:15.000000 vht-0.3.69/vht/randomcomposer.py
+-rw-r--r--   0 mal1ce    (1000) mal1ce    (1000)     8290 2024-04-22 09:54:53.000000 vht-0.3.69/vht/renderer.py
+-rw-r--r--   0 mal1ce    (1000) mal1ce    (1000)     9639 2024-04-21 16:33:45.000000 vht-0.3.69/vht/renderwin.py
+-rw-r--r--   0 mal1ce    (1000) mal1ce    (1000)    15715 2023-03-21 08:04:15.000000 vht-0.3.69/vht/sequencelistview.py
+-rw-r--r--   0 mal1ce    (1000) mal1ce    (1000)    13092 2024-04-28 12:53:09.000000 vht-0.3.69/vht/sequencelistviewpopover.py
+-rw-r--r--   0 mal1ce    (1000) mal1ce    (1000)    11262 2023-03-21 08:04:15.000000 vht-0.3.69/vht/sequencepropviewpopover.py
+-rw-r--r--   0 mal1ce    (1000) mal1ce    (1000)    12223 2023-03-21 12:19:50.000000 vht-0.3.69/vht/sequencetriggersview.py
+-rw-r--r--   0 mal1ce    (1000) mal1ce    (1000)    37321 2024-04-28 00:39:42.000000 vht-0.3.69/vht/sequenceview.py
+-rw-r--r--   0 mal1ce    (1000) mal1ce    (1000)     6678 2023-03-21 08:04:15.000000 vht-0.3.69/vht/shortcutmayhem.py
+-rw-r--r--   0 mal1ce    (1000) mal1ce    (1000)    20316 2024-03-22 16:23:30.000000 vht-0.3.69/vht/sidetrackview.py
+-rw-r--r--   0 mal1ce    (1000) mal1ce    (1000)    19524 2023-09-09 20:22:06.000000 vht-0.3.69/vht/statusbar.py
+-rw-r--r--   0 mal1ce    (1000) mal1ce    (1000)     2879 2023-03-21 08:04:15.000000 vht-0.3.69/vht/thumbmanager.py
+-rw-r--r--   0 mal1ce    (1000) mal1ce    (1000)    51601 2023-03-21 08:04:15.000000 vht-0.3.69/vht/timelineview.py
+-rw-r--r--   0 mal1ce    (1000) mal1ce    (1000)     6308 2023-03-21 08:04:15.000000 vht-0.3.69/vht/timeshifteditor.py
+-rw-r--r--   0 mal1ce    (1000) mal1ce    (1000)    22027 2023-03-21 08:04:15.000000 vht-0.3.69/vht/trackpropview.py
+-rw-r--r--   0 mal1ce    (1000) mal1ce    (1000)    31965 2024-04-08 23:20:41.000000 vht-0.3.69/vht/trackpropviewpopover.py
+-rw-r--r--   0 mal1ce    (1000) mal1ce    (1000)     3229 2023-03-21 08:04:15.000000 vht-0.3.69/vht/trackundobuffer.py
+-rw-r--r--   0 mal1ce    (1000) mal1ce    (1000)    96092 2024-03-22 15:55:48.000000 vht-0.3.69/vht/trackview.py
+-rw-r--r--   0 mal1ce    (1000) mal1ce    (1000)     9212 2023-03-21 08:04:15.000000 vht-0.3.69/vht/trackviewpointer.py
+-rw-r--r--   0 mal1ce    (1000) mal1ce    (1000)     8127 2023-03-21 08:04:15.000000 vht-0.3.69/vht/velocityeditor.py
+drwxrwxr-x   0 mal1ce    (1000) mal1ce    (1000)        0 2024-04-28 23:48:37.426646 vht-0.3.69/vht.egg-info/
+-rw-r--r--   0 mal1ce    (1000) mal1ce    (1000)     1912 2024-04-28 23:48:37.000000 vht-0.3.69/vht.egg-info/PKG-INFO
+-rw-rw-r--   0 mal1ce    (1000) mal1ce    (1000)     2518 2024-04-28 23:48:37.000000 vht-0.3.69/vht.egg-info/SOURCES.txt
+-rw-rw-r--   0 mal1ce    (1000) mal1ce    (1000)        1 2024-04-28 23:48:37.000000 vht-0.3.69/vht.egg-info/dependency_links.txt
+-rw-rw-r--   0 mal1ce    (1000) mal1ce    (1000)       37 2024-04-28 23:48:37.000000 vht-0.3.69/vht.egg-info/entry_points.txt
+-rw-rw-r--   0 mal1ce    (1000) mal1ce    (1000)       27 2024-04-28 23:48:37.000000 vht-0.3.69/vht.egg-info/top_level.txt
```

### Comparing `vht-0.3.33/LICENSE` & `vht-0.3.69/LICENSE`

 * *Files identical despite different names*

### Comparing `vht-0.3.33/PKG-INFO` & `vht-0.3.69/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vht
-Version: 0.3.33
+Version: 0.3.69
 Summary: vahatraker - a live MIDI sequencer for JACK
 Home-page: https://github.com/rdybka/vht
 Author: Remigiusz Dybka
 Author-email: remigiusz.dybka@gmail.com
 License: GPLv3+
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: X11 Applications :: GTK
```

### Comparing `vht-0.3.33/README.md` & `vht-0.3.69/README.md`

 * *Files identical despite different names*

### Comparing `vht-0.3.33/data/bank/10-gm1` & `vht-0.3.69/data/bank/10-gm1`

 * *Files identical despite different names*

### Comparing `vht-0.3.33/data/bank/20-gm2` & `vht-0.3.69/data/bank/20-gm2`

 * *Files identical despite different names*

### Comparing `vht-0.3.33/data/mandy.png` & `vht-0.3.69/data/mandy.png`

 * *Files identical despite different names*

### Comparing `vht-0.3.33/data/menu.ui` & `vht-0.3.69/data/menu.ui`

 * *Files identical despite different names*

### Comparing `vht-0.3.33/data/vht.png` & `vht-0.3.69/data/vht.png`

 * *Files identical despite different names*

### Comparing `vht-0.3.33/data/vht.svg` & `vht-0.3.69/data/vht.svg`

 * *Files identical despite different names*

### Comparing `vht-0.3.33/doc/vht.1.md` & `vht-0.3.69/doc/vht.1.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
-% VHT(1) vht 0.3.32
+% VHT(1) vht 0.3.69
 % Remigiusz Dybka
-% May 2023
+% April 2024
 
 # NAME
 **vht** - a minimalistic MIDI sequencer for JACK/GNOME
 
 # SYNOPSIS
 **vht** [file]
```

### Comparing `vht-0.3.33/libvht/ctrlrow.c` & `vht-0.3.69/libvht/ctrlrow.c`

 * *Files identical despite different names*

### Comparing `vht-0.3.33/libvht/ctrlrow.h` & `vht-0.3.69/libvht/ctrlrow.h`

 * *Files identical despite different names*

### Comparing `vht-0.3.33/libvht/envelope.c` & `vht-0.3.69/libvht/envelope.c`

 * *Files identical despite different names*

### Comparing `vht-0.3.33/libvht/envelope.h` & `vht-0.3.69/libvht/envelope.h`

 * *Files identical despite different names*

### Comparing `vht-0.3.33/libvht/jack_process.c` & `vht-0.3.69/libvht/jack_process.c`

 * *Files 2% similar despite different names*

```diff
@@ -28,18 +28,19 @@
 	float period_usecs;
 
 	midi_client *clt = (midi_client *)arg;
 	module *mod = (module *)clt->mod_ref;
 
 	jack_get_cycle_times(clt->jack_client, &curr_frames, &curr_usecs, &next_usecs, &period_usecs);
 	midi_synch_output_ports(clt);
+
 	module_advance(mod, curr_frames);
 	clt->jack_last_frame = jack_last_frame_time(clt->jack_client);
-
 	midi_buffer_flush(clt);
+
 	return 0;
 }
 
 int jack_sample_rate_changed(jack_nframes_t srate, void *arg) {
 	((midi_client *)arg)->jack_sample_rate = srate;
 	return 0;
 }
```

### Comparing `vht-0.3.33/libvht/jack_process.h` & `vht-0.3.69/libvht/jack_process.h`

 * *Files identical despite different names*

### Comparing `vht-0.3.33/libvht/libcvht.h` & `vht-0.3.69/libvht/libcvht.h`

 * *Files 1% similar despite different names*

```diff
@@ -70,15 +70,15 @@
 extern void module_set_pnq_hack(module *mod, int ph);
 extern int module_get_pnq_hack(module *mod);
 extern void module_set_inception(module *mod, int i);
 extern int module_get_inception(module *mod);
 
 extern void module_set_should_save(module *mod, int ss);
 extern int module_get_should_save(module *mod);
-
+extern int module_dump_midi(module *mod, const char *phname, int tc, int tpf);
 extern int module_get_nseq(module *mod);
 extern sequence *module_get_seq(module *mod, int);
 extern void module_add_sequence(module *mod, sequence *seq);
 extern void module_del_sequence(module *mod, int s);
 extern void module_swap_sequence(module *mod, int s1, int s2);
 extern sequence *module_sequence_replace(module *mod, int s, sequence *seq);
 extern sequence *module_get_curr_seq(module *mod);
@@ -103,22 +103,25 @@
 
 extern void queue_midi_note_on(midi_client *clt, sequence *seq, int port, int chn, int note, int velocity);
 extern void queue_midi_note_off(midi_client *clt, sequence *seq, int port, int chn, int note);
 extern void queue_midi_ctrl(midi_client *clt, sequence *seq, track *trk, int val, int ctrl);
 extern void midi_refresh_port_names(midi_client *clt);
 extern int midi_nport_names(midi_client *clt);
 extern char *midi_get_port_name(midi_client *clt, int prt);
+extern char *midi_get_port_pname(midi_client *clt, jack_port_t *prtref);
+
 extern jack_port_t *midi_get_port_ref(midi_client *clt, char *name);
 extern char *midi_get_port_type(jack_port_t *prtref);
 extern int midi_get_port_mine(midi_client *clt, jack_port_t *prtref);
 extern int midi_get_port_input(jack_port_t *prtref);
 extern int midi_get_port_output(jack_port_t *prtref);
 extern int midi_get_port_physical(jack_port_t *prtref);
 
 extern const char **midi_get_port_connections(midi_client *clt, jack_port_t *prtref);
+extern PyObject *midi_get_props(midi_client *clt);
 extern void midi_free_charpp(char **cpp);
 extern int charpp_nitems(char **cpp);
 extern char *charpp_item(char **cpp, int itm);
 extern void midi_port_connect(midi_client *clt, const char *prtref, const char *prtref2);
 extern void midi_port_disconnect(midi_client *clt, const char *prtref, const char *prtref2);
 extern int midi_port_names_changed(midi_client *clt);
 extern int midi_port_is_open(midi_client *clt, int prt);
@@ -148,15 +151,14 @@
 extern void sequence_set_trg_playmode(sequence *seq, int v);
 extern void sequence_set_trg_quantise(sequence *seq, int v);
 extern int sequence_get_trg_playmode(sequence *seq);
 extern int sequence_get_trg_quantise(sequence *seq);
 extern int module_get_max_trg_grp();
 extern int sequence_get_trg_grp(sequence *seq, int g);
 extern void sequence_set_trg_grp(sequence *seq, int g, int grp);
-
 extern void sequence_set_trig(sequence *seq, int t, int tp, int ch, int nt);
 extern char *sequence_get_trig(sequence *seq, int t);
 extern void sequence_trigger_mute(sequence *seq, int nframes);
 extern void sequence_trigger_mute_forward(sequence *seq, int nframes);
 extern void sequence_trigger_mute_back(sequence *seq, int nframes);
 extern void sequence_trigger_cue(sequence *seq, int nframes);
 extern void sequence_trigger_cue_forward(sequence *seq, int nframes);
@@ -185,14 +187,16 @@
 extern int sequence_get_loop_active(sequence *seq);
 extern void sequence_set_loop_active(sequence *seq, int v);
 extern int sequence_get_loop_start(sequence *seq);
 extern void sequence_set_loop_start(sequence *seq, int s);
 extern int sequence_get_loop_end(sequence *seq);
 extern void sequence_set_loop_end(sequence *seq, int e);
 
+extern int sequence_get_next_row(sequence *seq);
+
 // track
 extern row *track_get_row_ptr(track *, int c, int r);
 extern ctrlrow *track_get_ctrlrow_ptr(track *, int c, int r);
 extern int track_get_index(track *trk);
 extern int track_get_length(track *trk);
 extern int track_get_ncols(track *trk);
 extern int track_get_port(track *trk);
```

### Comparing `vht-0.3.33/libvht/libcvht.py` & `vht-0.3.69/libvht/libcvht.py`

 * *Files 0% similar despite different names*

```diff
@@ -214,14 +214,17 @@
 
 def module_set_should_save(mod, ss):
     return _libcvht.module_set_should_save(mod, ss)
 
 def module_get_should_save(mod):
     return _libcvht.module_get_should_save(mod)
 
+def module_dump_midi(mod, phname, tc, tpf):
+    return _libcvht.module_dump_midi(mod, phname, tc, tpf)
+
 def module_get_nseq(mod):
     return _libcvht.module_get_nseq(mod)
 
 def module_get_seq(mod, arg2):
     return _libcvht.module_get_seq(mod, arg2)
 
 def module_add_sequence(mod, seq):
@@ -301,14 +304,17 @@
 
 def midi_nport_names(clt):
     return _libcvht.midi_nport_names(clt)
 
 def midi_get_port_name(clt, prt):
     return _libcvht.midi_get_port_name(clt, prt)
 
+def midi_get_port_pname(clt, prtref):
+    return _libcvht.midi_get_port_pname(clt, prtref)
+
 def midi_get_port_ref(clt, name):
     return _libcvht.midi_get_port_ref(clt, name)
 
 def midi_get_port_type(prtref):
     return _libcvht.midi_get_port_type(prtref)
 
 def midi_get_port_mine(clt, prtref):
@@ -322,14 +328,17 @@
 
 def midi_get_port_physical(prtref):
     return _libcvht.midi_get_port_physical(prtref)
 
 def midi_get_port_connections(clt, prtref):
     return _libcvht.midi_get_port_connections(clt, prtref)
 
+def midi_get_props(clt):
+    return _libcvht.midi_get_props(clt)
+
 def midi_free_charpp(cpp):
     return _libcvht.midi_free_charpp(cpp)
 
 def charpp_nitems(cpp):
     return _libcvht.charpp_nitems(cpp)
 
 def charpp_item(cpp, itm):
@@ -523,14 +532,17 @@
 
 def sequence_get_loop_end(seq):
     return _libcvht.sequence_get_loop_end(seq)
 
 def sequence_set_loop_end(seq, e):
     return _libcvht.sequence_set_loop_end(seq, e)
 
+def sequence_get_next_row(seq):
+    return _libcvht.sequence_get_next_row(seq)
+
 def track_get_row_ptr(arg1, c, r):
     return _libcvht.track_get_row_ptr(arg1, c, r)
 
 def track_get_ctrlrow_ptr(arg1, c, r):
     return _libcvht.track_get_ctrlrow_ptr(arg1, c, r)
 
 def track_get_index(trk):
```

### Comparing `vht-0.3.33/libvht/libcvht_wrap.c` & `vht-0.3.69/libvht/libcvht_wrap.c`

 * *Files 0% similar despite different names*

```diff
@@ -4472,14 +4472,63 @@
   resultobj = SWIG_From_int((int)(result));
   return resultobj;
 fail:
   return NULL;
 }
 
 
+SWIGINTERN PyObject *_wrap_module_dump_midi(PyObject *SWIGUNUSEDPARM(self), PyObject *args) {
+  PyObject *resultobj = 0;
+  module *arg1 = (module *) 0 ;
+  char *arg2 = (char *) 0 ;
+  int arg3 ;
+  int arg4 ;
+  void *argp1 = 0 ;
+  int res1 = 0 ;
+  int res2 ;
+  char *buf2 = 0 ;
+  int alloc2 = 0 ;
+  int val3 ;
+  int ecode3 = 0 ;
+  int val4 ;
+  int ecode4 = 0 ;
+  PyObject *swig_obj[4] ;
+  int result;
+  
+  if (!SWIG_Python_UnpackTuple(args, "module_dump_midi", 4, 4, swig_obj)) SWIG_fail;
+  res1 = SWIG_ConvertPtr(swig_obj[0], &argp1,SWIGTYPE_p_module, 0 |  0 );
+  if (!SWIG_IsOK(res1)) {
+    SWIG_exception_fail(SWIG_ArgError(res1), "in method '" "module_dump_midi" "', argument " "1"" of type '" "module *""'"); 
+  }
+  arg1 = (module *)(argp1);
+  res2 = SWIG_AsCharPtrAndSize(swig_obj[1], &buf2, NULL, &alloc2);
+  if (!SWIG_IsOK(res2)) {
+    SWIG_exception_fail(SWIG_ArgError(res2), "in method '" "module_dump_midi" "', argument " "2"" of type '" "char const *""'");
+  }
+  arg2 = (char *)(buf2);
+  ecode3 = SWIG_AsVal_int(swig_obj[2], &val3);
+  if (!SWIG_IsOK(ecode3)) {
+    SWIG_exception_fail(SWIG_ArgError(ecode3), "in method '" "module_dump_midi" "', argument " "3"" of type '" "int""'");
+  } 
+  arg3 = (int)(val3);
+  ecode4 = SWIG_AsVal_int(swig_obj[3], &val4);
+  if (!SWIG_IsOK(ecode4)) {
+    SWIG_exception_fail(SWIG_ArgError(ecode4), "in method '" "module_dump_midi" "', argument " "4"" of type '" "int""'");
+  } 
+  arg4 = (int)(val4);
+  result = (int)module_dump_midi(arg1,(char const *)arg2,arg3,arg4);
+  resultobj = SWIG_From_int((int)(result));
+  if (alloc2 == SWIG_NEWOBJ) free((char*)buf2);
+  return resultobj;
+fail:
+  if (alloc2 == SWIG_NEWOBJ) free((char*)buf2);
+  return NULL;
+}
+
+
 SWIGINTERN PyObject *_wrap_module_get_nseq(PyObject *SWIGUNUSEDPARM(self), PyObject *args) {
   PyObject *resultobj = 0;
   module *arg1 = (module *) 0 ;
   void *argp1 = 0 ;
   int res1 = 0 ;
   PyObject *swig_obj[1] ;
   int result;
@@ -5379,14 +5428,44 @@
   resultobj = SWIG_FromCharPtr((const char *)result);
   return resultobj;
 fail:
   return NULL;
 }
 
 
+SWIGINTERN PyObject *_wrap_midi_get_port_pname(PyObject *SWIGUNUSEDPARM(self), PyObject *args) {
+  PyObject *resultobj = 0;
+  midi_client *arg1 = (midi_client *) 0 ;
+  jack_port_t *arg2 = (jack_port_t *) 0 ;
+  void *argp1 = 0 ;
+  int res1 = 0 ;
+  void *argp2 = 0 ;
+  int res2 = 0 ;
+  PyObject *swig_obj[2] ;
+  char *result = 0 ;
+  
+  if (!SWIG_Python_UnpackTuple(args, "midi_get_port_pname", 2, 2, swig_obj)) SWIG_fail;
+  res1 = SWIG_ConvertPtr(swig_obj[0], &argp1,SWIGTYPE_p_midi_client, 0 |  0 );
+  if (!SWIG_IsOK(res1)) {
+    SWIG_exception_fail(SWIG_ArgError(res1), "in method '" "midi_get_port_pname" "', argument " "1"" of type '" "midi_client *""'"); 
+  }
+  arg1 = (midi_client *)(argp1);
+  res2 = SWIG_ConvertPtr(swig_obj[1], &argp2,SWIGTYPE_p_jack_port_t, 0 |  0 );
+  if (!SWIG_IsOK(res2)) {
+    SWIG_exception_fail(SWIG_ArgError(res2), "in method '" "midi_get_port_pname" "', argument " "2"" of type '" "jack_port_t *""'"); 
+  }
+  arg2 = (jack_port_t *)(argp2);
+  result = (char *)midi_get_port_pname(arg1,arg2);
+  resultobj = SWIG_FromCharPtr((const char *)result);
+  return resultobj;
+fail:
+  return NULL;
+}
+
+
 SWIGINTERN PyObject *_wrap_midi_get_port_ref(PyObject *SWIGUNUSEDPARM(self), PyObject *args) {
   PyObject *resultobj = 0;
   midi_client *arg1 = (midi_client *) 0 ;
   char *arg2 = (char *) 0 ;
   void *argp1 = 0 ;
   int res1 = 0 ;
   int res2 ;
@@ -5564,14 +5643,37 @@
   resultobj = SWIG_NewPointerObj(SWIG_as_voidptr(result), SWIGTYPE_p_p_char, 0 |  0 );
   return resultobj;
 fail:
   return NULL;
 }
 
 
+SWIGINTERN PyObject *_wrap_midi_get_props(PyObject *SWIGUNUSEDPARM(self), PyObject *args) {
+  PyObject *resultobj = 0;
+  midi_client *arg1 = (midi_client *) 0 ;
+  void *argp1 = 0 ;
+  int res1 = 0 ;
+  PyObject *swig_obj[1] ;
+  PyObject *result = 0 ;
+  
+  if (!args) SWIG_fail;
+  swig_obj[0] = args;
+  res1 = SWIG_ConvertPtr(swig_obj[0], &argp1,SWIGTYPE_p_midi_client, 0 |  0 );
+  if (!SWIG_IsOK(res1)) {
+    SWIG_exception_fail(SWIG_ArgError(res1), "in method '" "midi_get_props" "', argument " "1"" of type '" "midi_client *""'"); 
+  }
+  arg1 = (midi_client *)(argp1);
+  result = (PyObject *)midi_get_props(arg1);
+  resultobj = result;
+  return resultobj;
+fail:
+  return NULL;
+}
+
+
 SWIGINTERN PyObject *_wrap_midi_free_charpp(PyObject *SWIGUNUSEDPARM(self), PyObject *args) {
   PyObject *resultobj = 0;
   char **arg1 = (char **) 0 ;
   void *argp1 = 0 ;
   int res1 = 0 ;
   PyObject *swig_obj[1] ;
   
@@ -7410,14 +7512,37 @@
   resultobj = SWIG_Py_Void();
   return resultobj;
 fail:
   return NULL;
 }
 
 
+SWIGINTERN PyObject *_wrap_sequence_get_next_row(PyObject *SWIGUNUSEDPARM(self), PyObject *args) {
+  PyObject *resultobj = 0;
+  sequence *arg1 = (sequence *) 0 ;
+  void *argp1 = 0 ;
+  int res1 = 0 ;
+  PyObject *swig_obj[1] ;
+  int result;
+  
+  if (!args) SWIG_fail;
+  swig_obj[0] = args;
+  res1 = SWIG_ConvertPtr(swig_obj[0], &argp1,SWIGTYPE_p_sequence, 0 |  0 );
+  if (!SWIG_IsOK(res1)) {
+    SWIG_exception_fail(SWIG_ArgError(res1), "in method '" "sequence_get_next_row" "', argument " "1"" of type '" "sequence *""'"); 
+  }
+  arg1 = (sequence *)(argp1);
+  result = (int)sequence_get_next_row(arg1);
+  resultobj = SWIG_From_int((int)(result));
+  return resultobj;
+fail:
+  return NULL;
+}
+
+
 SWIGINTERN PyObject *_wrap_track_get_row_ptr(PyObject *SWIGUNUSEDPARM(self), PyObject *args) {
   PyObject *resultobj = 0;
   track *arg1 = (track *) 0 ;
   int arg2 ;
   int arg3 ;
   void *argp1 = 0 ;
   int res1 = 0 ;
@@ -13560,14 +13685,15 @@
 	 { "module_get_transport", _wrap_module_get_transport, METH_O, NULL},
 	 { "module_set_pnq_hack", _wrap_module_set_pnq_hack, METH_VARARGS, NULL},
 	 { "module_get_pnq_hack", _wrap_module_get_pnq_hack, METH_O, NULL},
 	 { "module_set_inception", _wrap_module_set_inception, METH_VARARGS, NULL},
 	 { "module_get_inception", _wrap_module_get_inception, METH_O, NULL},
 	 { "module_set_should_save", _wrap_module_set_should_save, METH_VARARGS, NULL},
 	 { "module_get_should_save", _wrap_module_get_should_save, METH_O, NULL},
+	 { "module_dump_midi", _wrap_module_dump_midi, METH_VARARGS, NULL},
 	 { "module_get_nseq", _wrap_module_get_nseq, METH_O, NULL},
 	 { "module_get_seq", _wrap_module_get_seq, METH_VARARGS, NULL},
 	 { "module_add_sequence", _wrap_module_add_sequence, METH_VARARGS, NULL},
 	 { "module_del_sequence", _wrap_module_del_sequence, METH_VARARGS, NULL},
 	 { "module_swap_sequence", _wrap_module_swap_sequence, METH_VARARGS, NULL},
 	 { "module_sequence_replace", _wrap_module_sequence_replace, METH_VARARGS, NULL},
 	 { "module_get_curr_seq", _wrap_module_get_curr_seq, METH_O, NULL},
@@ -13589,21 +13715,23 @@
 	 { "midi_ignore_buffer_add", _wrap_midi_ignore_buffer_add, METH_VARARGS, NULL},
 	 { "queue_midi_note_on", _wrap_queue_midi_note_on, METH_VARARGS, NULL},
 	 { "queue_midi_note_off", _wrap_queue_midi_note_off, METH_VARARGS, NULL},
 	 { "queue_midi_ctrl", _wrap_queue_midi_ctrl, METH_VARARGS, NULL},
 	 { "midi_refresh_port_names", _wrap_midi_refresh_port_names, METH_O, NULL},
 	 { "midi_nport_names", _wrap_midi_nport_names, METH_O, NULL},
 	 { "midi_get_port_name", _wrap_midi_get_port_name, METH_VARARGS, NULL},
+	 { "midi_get_port_pname", _wrap_midi_get_port_pname, METH_VARARGS, NULL},
 	 { "midi_get_port_ref", _wrap_midi_get_port_ref, METH_VARARGS, NULL},
 	 { "midi_get_port_type", _wrap_midi_get_port_type, METH_O, NULL},
 	 { "midi_get_port_mine", _wrap_midi_get_port_mine, METH_VARARGS, NULL},
 	 { "midi_get_port_input", _wrap_midi_get_port_input, METH_O, NULL},
 	 { "midi_get_port_output", _wrap_midi_get_port_output, METH_O, NULL},
 	 { "midi_get_port_physical", _wrap_midi_get_port_physical, METH_O, NULL},
 	 { "midi_get_port_connections", _wrap_midi_get_port_connections, METH_VARARGS, NULL},
+	 { "midi_get_props", _wrap_midi_get_props, METH_O, NULL},
 	 { "midi_free_charpp", _wrap_midi_free_charpp, METH_O, NULL},
 	 { "charpp_nitems", _wrap_charpp_nitems, METH_O, NULL},
 	 { "charpp_item", _wrap_charpp_item, METH_VARARGS, NULL},
 	 { "midi_port_connect", _wrap_midi_port_connect, METH_VARARGS, NULL},
 	 { "midi_port_disconnect", _wrap_midi_port_disconnect, METH_VARARGS, NULL},
 	 { "midi_port_names_changed", _wrap_midi_port_names_changed, METH_O, NULL},
 	 { "midi_port_is_open", _wrap_midi_port_is_open, METH_VARARGS, NULL},
@@ -13663,14 +13791,15 @@
 	 { "sequence_rotate", _wrap_sequence_rotate, METH_VARARGS, NULL},
 	 { "sequence_get_loop_active", _wrap_sequence_get_loop_active, METH_O, NULL},
 	 { "sequence_set_loop_active", _wrap_sequence_set_loop_active, METH_VARARGS, NULL},
 	 { "sequence_get_loop_start", _wrap_sequence_get_loop_start, METH_O, NULL},
 	 { "sequence_set_loop_start", _wrap_sequence_set_loop_start, METH_VARARGS, NULL},
 	 { "sequence_get_loop_end", _wrap_sequence_get_loop_end, METH_O, NULL},
 	 { "sequence_set_loop_end", _wrap_sequence_set_loop_end, METH_VARARGS, NULL},
+	 { "sequence_get_next_row", _wrap_sequence_get_next_row, METH_O, NULL},
 	 { "track_get_row_ptr", _wrap_track_get_row_ptr, METH_VARARGS, NULL},
 	 { "track_get_ctrlrow_ptr", _wrap_track_get_ctrlrow_ptr, METH_VARARGS, NULL},
 	 { "track_get_index", _wrap_track_get_index, METH_O, NULL},
 	 { "track_get_length", _wrap_track_get_length, METH_O, NULL},
 	 { "track_get_ncols", _wrap_track_get_ncols, METH_O, NULL},
 	 { "track_get_port", _wrap_track_get_port, METH_O, NULL},
 	 { "track_get_channel", _wrap_track_get_channel, METH_O, NULL},
```

### Comparing `vht-0.3.33/libvht/libvht.c` & `vht-0.3.69/libvht/libvht.c`

 * *Files identical despite different names*

### Comparing `vht-0.3.33/libvht/mandy.c` & `vht-0.3.69/libvht/mandy.c`

 * *Files 0% similar despite different names*

```diff
@@ -527,15 +527,15 @@
 		tracy_excl_out(trc);
 	}
 	mandy_gen_info(mand);
 }
 
 // this runs in gui thread
 void mandy_animate(mandy *mand) {
-	double sm = 2;
+	double sm = 1.5;
 
 	long double dx = mand->dx;
 	long double dy = mand->dy;
 	long double drot = mand->drot;
 	long double dzoom = mand->dzoom;
 
 	/*for (unsigned int tr = 0; tr < mand->ntracies; tr++) {
```

### Comparing `vht-0.3.33/libvht/mandy.h` & `vht-0.3.69/libvht/mandy.h`

 * *Files identical despite different names*

### Comparing `vht-0.3.33/libvht/mandy_pix_scan.c` & `vht-0.3.69/libvht/mandy_pix_scan.c`

 * *Files identical despite different names*

### Comparing `vht-0.3.33/libvht/mandy_pix_scan.h` & `vht-0.3.69/libvht/mandy_pix_scan.h`

 * *Files identical despite different names*

### Comparing `vht-0.3.33/libvht/mandy_trk_disp.c` & `vht-0.3.69/libvht/mandy_trk_disp.c`

 * *Files identical despite different names*

### Comparing `vht-0.3.33/libvht/mandy_trk_disp.h` & `vht-0.3.69/libvht/mandy_trk_disp.h`

 * *Files identical despite different names*

### Comparing `vht-0.3.33/libvht/midi_client.c` & `vht-0.3.69/libvht/midi_client.c`

 * *Files 2% similar despite different names*

```diff
@@ -15,14 +15,16 @@
  * You should have received a copy of the GNU General Public License
  * along with this program.  If not, see <http://www.gnu.org/licenses/>.
  */
 
 #include <stdio.h>
 #include <stdlib.h>
 #include <jack/midiport.h>
+#include <jack/metadata.h>
+#include <jack/uuid.h>
 #include <errno.h>
 #include "jack_process.h"
 #include "module.h"
 #include "midi_event.h"
 #include "midi_client.h"
 
 midi_client *midi_client_new(void *mod) {
@@ -304,14 +306,17 @@
 			} else {
 				jack_midi_event_write(outp, clt->midi_buffer[port][i].time, buff, l);
 				last = &clt->midi_buffer[port][i];
 			}
 		}
 
 		module *mod = (module *) clt->mod_ref;
+		if (mod->midi_file) {
+			smf_client_flush(mod->midi_file, port, clt->midi_buffer[port][i]);
+		}
 
 		if (clt->dump_notes && !dbl) {
 			char desc[256];
 			midi_describe_event(clt->midi_buffer[port][i], desc, 256);
 			printf("%02d:%02d:%03d >> pt: %02d, %s\n", mod->min, mod->sec, mod->ms, port, desc);
 		}
 
@@ -544,14 +549,34 @@
 		return NULL;
 	}
 
 	strcpy(buff, clt->ports[prt]);
 	return buff;
 }
 
+char *midi_get_port_pname(midi_client *clt, jack_port_t *prtref) {
+	static char buff[1023];
+
+	jack_uuid_t uuid = jack_port_uuid(prtref);
+	char *val = 0;
+	char *type = 0;
+	if (0 == jack_get_property(uuid, JACK_METADATA_PRETTY_NAME, &val, &type)) {
+		strcpy(buff, val);
+	} else {
+		buff[0] = 0;
+	}
+
+	if (val)
+		jack_free(val);
+	if (type)
+		jack_free(type);
+
+	return buff;
+}
+
 jack_port_t *midi_get_port_ref(midi_client *clt, char *name) {
 	return jack_port_by_name(clt->jack_client, name);
 }
 
 char *midi_get_port_type(jack_port_t *prtref) {
 	static char buff[1023];
 	const char *t = jack_port_type(prtref);
@@ -584,14 +609,20 @@
 }
 
 void midi_free_charpp(char **cpp) {
 	if (cpp)
 		jack_free(cpp);
 }
 
+PyObject *midi_get_props(midi_client *clt) {
+
+
+	return NULL;
+}
+
 void midi_port_connect(midi_client *clt, const char *prtref, const char *prtref2) {
 	int stat = jack_connect(clt->jack_client, prtref, prtref2);
 	if (stat == EEXIST)
 		stat = 0;
 }
 
 void midi_port_disconnect(midi_client *clt, const char *prtref, const char *prtref2) {
```

### Comparing `vht-0.3.33/libvht/midi_client.h` & `vht-0.3.69/libvht/midi_client.h`

 * *Files 1% similar despite different names*

```diff
@@ -24,14 +24,15 @@
 #define MIDI_CLIENT_PORT_NAME "out_%02d"
 #define MIDI_EVT_BUFFER_LENGTH 1023
 
 #include <pthread.h>
 #include <jack/jack.h>
 #include "sequence.h"
 #include "midi_event.h"
+#include <Python.h>
 
 /* should be easy enough to refactor this into some kind of driver architecture
 - have fun! */
 
 typedef struct midi_client_t {
 	void *mod_ref;
 	int default_midi_port;
@@ -92,21 +93,24 @@
 
 void midi_send_transp(midi_client *clt, int play, long frames);
 
 void midi_refresh_port_names(midi_client *clt);
 int midi_port_names_changed(midi_client *clt);
 int midi_nport_names(midi_client *clt);
 char *midi_get_port_name(midi_client *clt, int prt);
+
 jack_port_t *midi_get_port_ref(midi_client *clt, char *name);
 char *midi_get_port_type(jack_port_t *prtref);
+char *midi_get_port_pname(midi_client *clt, jack_port_t *prtref);
 int midi_get_port_mine(midi_client *clt, jack_port_t *prtref);
 int midi_get_port_input(jack_port_t *prtref);
 int midi_get_port_output(jack_port_t *prtref);
 int midi_get_port_physical(jack_port_t *prtref);
 const char **midi_get_port_connections(midi_client *clt, jack_port_t *prtref);
+PyObject *midi_get_props(midi_client *clt);
 void midi_free_charpp(char **cpp);
 void midi_port_connect(midi_client *clt, const char *prtref, const char *prtref2);
 void midi_port_disconnect(midi_client *clt, const char *prtref, const char *prtref2);
 
 // those are for outputs
 int midi_port_is_open(midi_client *clt, int prt);
 void midi_close_port(midi_client *clt, int prt);
```

### Comparing `vht-0.3.33/libvht/midi_event.c` & `vht-0.3.69/libvht/midi_event.c`

 * *Files identical despite different names*

### Comparing `vht-0.3.33/libvht/midi_event.h` & `vht-0.3.69/libvht/midi_event.h`

 * *Files identical despite different names*

### Comparing `vht-0.3.33/libvht/module.c` & `vht-0.3.69/libvht/module.c`

 * *Files 2% similar despite different names*

```diff
@@ -20,14 +20,15 @@
 #include <stdio.h>
 #include <math.h>
 #include <pthread.h>
 #include "module.h"
 #include "midi_client.h"
 #include "track.h"
 #include "midi_event.h"
+#include "smf.h"
 
 struct rec_update_t rec_update[MIDI_EVT_BUFFER_LENGTH];
 int cur_rec_update;
 
 int lastsec;
 
 void module_excl_in(module *mod) {
@@ -214,14 +215,17 @@
 			timeline_advance(mod->tline, per, mod->clt->jack_buffer_size);
 		}
 
 		for (int s = 0; s < mod->nseq; s++) {
 			sequence_handle_triggers_post_adv(mod->seq[s], period * mod->seq[s]->rpb * (mod->bpm / 60.0), mod->clt->jack_buffer_size);
 		}
 
+		if (mod->midi_file)
+			smf_set_pos(mod->midi_file, curr_frames);
+
 		mod->song_pos += period;
 
 		// fix mode switching
 		if (mod->switch_req && mod->nseq) {
 			//printf("delaying: %f\n", mod->switch_delay);
 
 			if (mod->play_mode == 0) {
@@ -291,25 +295,27 @@
 int module_get_should_save(module *mod) {
 	return mod->should_save;
 }
 
 void module_play(module *mod, int play) {
 	module_excl_in(mod);
 	int prev_state = mod->playing;
+
 	mod->playing = play;
 
 	if (mod->render_mode > 0 && mod->playing && !prev_state) {
 		mod->playing = -2; // this will skip first callback from jack
 		midi_set_freewheel(mod->clt, 1);
 	}
 
 	module_excl_out(mod);
 
-	if (play == 0)
+	if (play == 0) {
 		module_mute(mod);
+	}
 
 	if (mod->transp && !mod->render_mode) {
 		midi_send_transp(mod->clt, play, -1);
 	}
 }
 
 module *module_new() {
@@ -325,14 +331,15 @@
 	mod->mute = 0;
 	mod->ctrlpr = DEFAULT_CTRLPR;
 	mod->cur_rec_update = 0;
 	mod->seq = malloc(sizeof(sequence *));
 	mod->transp = 0;
 	pthread_mutex_init(&mod->excl, NULL);
 	mod->clt = midi_client_new(mod);
+	mod->midi_file = smf_new(mod);
 	mod->tline = timeline_new(mod->clt);
 	mod->play_mode = 0;
 	mod->switch_delay = 0.0;
 	mod->switch_req = 0;
 	mod->render_mode = 0;
 	mod->render_lead_out = 0;
 	mod->panic = 0;
@@ -348,23 +355,41 @@
 	return mod;
 }
 
 void module_mute(module *mod) {
 	mod->mute = 1;
 }
 
+int module_dump_midi(module *mod, const char *phname, int tc, int tpf) {
+	mod->midi_file->tc = tc;
+	mod->midi_file->ticks = tpf;
+	return smf_dump(mod->midi_file, phname);
+}
+
 void module_reset(module *mod) {
 	mod->zero_time = 0;
 	mod->song_pos = 0;
 	mod->min = mod->sec = mod->ms = 0;
+
 	for (int s = 0; s < mod->nseq; s++) {
 		mod->seq[s]->pos = 0;
-		//mod->seq[s]->lost = 1;
 		for (int t = 0; t < mod->seq[s]->ntrk; t++) {
 			track_kill_notes(mod->seq[s]->trk[t]);
+		}
+	}
+
+	midi_buff_excl_in(mod->clt);
+	midi_buffer_clear(mod->clt);
+	smf_clear(mod->midi_file);
+	smf_set_pos(mod->midi_file, 0);
+	midi_buff_excl_out(mod->clt);
+
+	for (int s = 0; s < mod->nseq; s++) {
+		mod->seq[s]->pos = 0;
+		for (int t = 0; t < mod->seq[s]->ntrk; t++) {
 			track_reset(mod->seq[s]->trk[t]);
 		}
 	}
 
 	timeline_reset(mod->tline);
 	if (mod->transp)
 		midi_send_transp(mod->clt, mod->playing, 0);
@@ -403,14 +428,16 @@
 }
 
 void module_free(module *mod) {
 	for (int s = 0; s < mod->nseq; s++)
 		for (int t = 0; t < mod->seq[s]->ntrk; t++)
 			track_kill_notes(mod->seq[s]->trk[t]);
 
+	smf_free(mod->midi_file);
+
 	sleep(.420);
 
 	midi_stop(mod->clt);
 	for (int s = 0; s < mod->nseq; s++)
 		sequence_free(mod->seq[s]);
 
 	free(mod->seq);
```

### Comparing `vht-0.3.33/libvht/module.h` & `vht-0.3.69/libvht/module.h`

 * *Files 3% similar despite different names*

```diff
@@ -23,14 +23,15 @@
 #include <jack/jack.h>
 #include <jack/midiport.h>
 #include <pthread.h>
 #include "midi_event.h"
 #include "midi_client.h"
 #include "sequence.h"
 #include "timeline.h"
+#include "smf.h"
 
 #define DEFAULT_CTRLPR 16
 
 typedef struct module_t {
 	int playing;
 	int recording;
 
@@ -47,14 +48,15 @@
 	int nseq;
 	sequence *curr_seq;
 	int mute;
 
 	int cur_rec_update;
 	pthread_mutex_t excl;
 	midi_client *clt;
+	smf *midi_file;
 	int play_mode; // 0 - seq_loop, 1 - timeline
 	int panic;
 	double switch_delay;
 	int switch_req;
 	int transp;
 	int render_mode;
 	jack_nframes_t end_time;
@@ -68,15 +70,15 @@
 void module_play(module *mod, int);
 void module_free(module *mod);
 void module_handle_inception(track *trk, midi_event evt);
 void module_advance(module *mod, jack_nframes_t curr_frames);
 void module_mute(module *mod);
 void module_reset(module *mod);
 void module_dump_notes(module *mod, int n);
-
+int module_dump_midi(module *mod, const char *phname, int tc, int tpf);
 void module_excl_in(module *mod);
 void module_excl_out(module *mod);
 
 void module_synch_transp(module *mod, int play, jack_nframes_t frames);
 void module_send_transp(module *mod, int play, jack_nframes_t frames);
 
 void module_add_sequence(module *mod, sequence *seq);
```

### Comparing `vht-0.3.33/libvht/row.c` & `vht-0.3.69/libvht/row.c`

 * *Files identical despite different names*

### Comparing `vht-0.3.33/libvht/row.h` & `vht-0.3.69/libvht/row.h`

 * *Files identical despite different names*

### Comparing `vht-0.3.33/libvht/sequence.c` & `vht-0.3.69/libvht/sequence.c`

 * *Files 1% similar despite different names*

```diff
@@ -61,14 +61,16 @@
 
 	seq->trg_grp[0] = 0;
 	seq->trg_grp[1] = 0;
 
 	seq->trg_playmode = 0;
 	seq->trg_quantise = 1;
 	seq->mod_excl = NULL;
+
+	seq->next_row = -1;
 	seq->clt = NULL;
 	seq->playing = 0;
 	seq->lost = 1;
 	seq->thumb_dirty = 1;
 	seq->thumb_repr = NULL;
 	seq->thumb_last_ring = 0;
 	seq->thumb_length = 0;
@@ -764,15 +766,15 @@
 		if (seq->trg_quantise == 0) { // play now!
 			seq->playing = 1;
 			seq->trg_status[TRIGGER_PLAY] = TRIGGER_STATUS_IDLE;
 			if (seq->trg_playmode == PLAY_TRIGGER_ONESHOT)
 				seq->trg_status[TRIGGER_PLAY] = TRIGGER_STATUS_KILLLATE;
 
 			seq->pos = 0;
-
+			seq->next_row = 0;
 			for (int t = 0; t < seq->ntrk; t++) {
 				track_reset(seq->trk[t]);
 			}
 
 			sequence_advance(seq, pp, nf);
 		}
 	}
@@ -791,15 +793,15 @@
 
 // this will be called on row boundaries
 void sequence_handle_triggers_adv(sequence *seq, int r) {
 	if (seq->trg_status[TRIGGER_CUE] == TRIGGER_STATUS_RUN) {
 		if (r == 0) {
 			seq->playing =! seq->playing;
 			seq->trg_status[TRIGGER_CUE] = TRIGGER_STATUS_IDLE;
-
+			seq->next_row = 0;
 			if (!seq->playing) {
 				for (int t = 0; t < seq->ntrk; t++)
 					track_kill_notes(seq->trk[t]);
 			}
 
 			seq->lost = 1;
 		}
@@ -807,15 +809,15 @@
 
 	if (seq->trg_status[TRIGGER_PLAY] == TRIGGER_STATUS_SYNC && seq->trg_quantise) {
 		seq->trg_times[TRIGGER_PLAY]--;
 
 		if (seq->trg_times[TRIGGER_PLAY] == 0) {
 			seq->playing = 1;
 			seq->pos = 0;
-
+			seq->next_row = 0;
 			for (int t = 0; t < seq->ntrk; t++) {
 				track_reset(seq->trk[t]);
 			}
 
 
 			seq->trg_status[TRIGGER_PLAY] = TRIGGER_STATUS_IDLE;
 			if (seq->trg_playmode == PLAY_TRIGGER_ONESHOT)
@@ -865,14 +867,17 @@
 
 		if (np > .999999)
 			rr++;
 
 		while (rr >= seq->length)
 			rr -= seq->length;
 
+		// let waiter pass
+		seq->next_row = rr;
+
 		for (int t = 0; t < seq->ntrk; t++) {
 			if (seq->trk[t]->mand->active) {
 				int qnt = seq->trk[t]->mand->tracies[0]->qnt;
 				if (qnt > 0 && r % qnt == 0)
 					for (int c = 0; c < seq->trk[t]->ncols; c++) {
 						int v = seq->trk[t]->mand_qnt[c];
 						if (v > -232323 && v < 0) {
@@ -1289,7 +1294,11 @@
 		do {
 			trigger *tr = &seq->triggers[t];
 			sequence_set_trig(seq, t, tr->type, tr->channel, tr->note);
 			t+=3;
 		} while (t < 5);
 	}
 }
+
+int sequence_get_next_row(sequence *seq) {
+	return seq->next_row;
+}
```

### Comparing `vht-0.3.33/libvht/sequence.h` & `vht-0.3.69/libvht/sequence.h`

 * *Files 2% similar despite different names*

```diff
@@ -15,14 +15,15 @@
  * You should have received a copy of the GNU General Public License
  * along with this program.  If not, see <http://www.gnu.org/licenses/>.
  */
 
 #ifndef __SEQUENCE_H__
 #define __SEQUENCE_H__
 #include <pthread.h>
+#include <semaphore.h>
 #include "midi_event.h"
 #include "track.h"
 
 
 #define SEQUENCE_MAX_LENGTH	512
 
 #define PLAY_TRIGGER_ONOFF		0
@@ -67,14 +68,15 @@
 	trigger triggers[N_TRIGGERS];
 	int trg_times[N_TRIGGERS];
 	int trg_status[N_TRIGGERS];
 	int trg_grp[2]; // trigger group
 	int trg_playmode;
 	int trg_quantise;
 	pthread_mutex_t *mod_excl;
+	int next_row;
 	void *clt;
 	char *extras;
 	int playing;
 	int lost;
 	int thumb_dirty;
 	int *thumb_repr;
 	int thumb_last_ring;
```

### Comparing `vht-0.3.33/libvht/timeline.c` & `vht-0.3.69/libvht/timeline.c`

 * *Files identical despite different names*

### Comparing `vht-0.3.33/libvht/timeline.h` & `vht-0.3.69/libvht/timeline.h`

 * *Files identical despite different names*

### Comparing `vht-0.3.33/libvht/track.c` & `vht-0.3.69/libvht/track.c`

 * *Files identical despite different names*

### Comparing `vht-0.3.33/libvht/track.h` & `vht-0.3.69/libvht/track.h`

 * *Files identical despite different names*

### Comparing `vht-0.3.33/libvht/tracy.c` & `vht-0.3.69/libvht/tracy.c`

 * *Files identical despite different names*

### Comparing `vht-0.3.33/libvht/tracy.h` & `vht-0.3.69/libvht/tracy.h`

 * *Files 2% similar despite different names*

```diff
@@ -17,15 +17,15 @@
  */
 
 #ifndef __TRACY_H__
 #define __TRACY_H__
 
 #include <Python.h>
 
-#define TRACY_MAX_TAIL	64
+#define TRACY_MAX_TAIL	32
 #define TRACY_MAX_SPEED	127
 
 typedef struct tracy_tail_coord {
 	long double x, y, r;
 	float dx, dy, dr;
 } tail_xy;
```

### Comparing `vht-0.3.33/libvht/vhtcolumn.py` & `vht-0.3.69/libvht/vhtcolumn.py`

 * *Files identical despite different names*

### Comparing `vht-0.3.33/libvht/vhtctrl.py` & `vht-0.3.69/libvht/vhtctrl.py`

 * *Files identical despite different names*

### Comparing `vht-0.3.33/libvht/vhtctrllist.py` & `vht-0.3.69/libvht/vhtctrllist.py`

 * *Files identical despite different names*

### Comparing `vht-0.3.33/libvht/vhtctrlrow.py` & `vht-0.3.69/libvht/vhtctrlrow.py`

 * *Files identical despite different names*

### Comparing `vht-0.3.33/libvht/vhtextras.py` & `vht-0.3.69/libvht/vhtextras.py`

 * *Files identical despite different names*

### Comparing `vht-0.3.33/libvht/vhtmandy.py` & `vht-0.3.69/libvht/vhtmandy.py`

 * *Files identical despite different names*

### Comparing `vht-0.3.33/libvht/vhtmodule.py` & `vht-0.3.69/libvht/vhtmodule.py`

 * *Files 1% similar despite different names*

```diff
@@ -569,14 +569,17 @@
                         cb(s.seq.index, t.index)
 
             self.play = jm["playing"]
 
         self.should_save = False
         return True
 
+    def dump_midi(self, filename, tc=0, ticks=100):
+        return libcvht.module_dump_midi(self._mod_handle, filename, tc, ticks)
+
     def unpack_seq(self, seq, matrix=False, append=False):
         sq = None
         par = -1
 
         if matrix:
             s = self.add_sequence()
             s.parent = par
```

### Comparing `vht-0.3.33/libvht/vhtport.py` & `vht-0.3.69/libvht/vhtport.py`

 * *Files 2% similar despite different names*

```diff
@@ -108,10 +108,15 @@
 
         return self._cons
 
     @property
     def name(self):
         return self._name
 
+    @property
+    def pname(self):
+        pn = libcvht.midi_get_port_pname(self._clt_handle, self._prtref)
+        return pn if pn else self._name
+
     def __str__(self):
         self.update_strrep()
         return self._strrep
```

### Comparing `vht-0.3.33/libvht/vhtports.py` & `vht-0.3.69/libvht/vhtports.py`

 * *Files identical despite different names*

### Comparing `vht-0.3.33/libvht/vhtquicklist.py` & `vht-0.3.69/libvht/vhtquicklist.py`

 * *Files identical despite different names*

### Comparing `vht-0.3.33/libvht/vhtrow.py` & `vht-0.3.69/libvht/vhtrow.py`

 * *Files identical despite different names*

### Comparing `vht-0.3.33/libvht/vhtsequence.py` & `vht-0.3.69/libvht/vhtsequence.py`

 * *Files 2% similar despite different names*

```diff
@@ -48,14 +48,17 @@
         h1 = int(self._seq_handle)
         h2 = int(other._seq_handle)
         if h1 == h2:
             return True
 
         return False
 
+    def __hash__(self):
+        return int(self._seq_handle)
+
     def __getitem__(self, itm):
         if itm >= self.__len__():
             return None
 
         if itm < 0:
             if not len(self) >= -itm:
                 raise IndexError()
@@ -342,14 +345,18 @@
 
     def trigger_play_on(self):
         libcvht.sequence_trigger_play_on(self._seq_handle, -1)
 
     def trigger_play_off(self):
         libcvht.sequence_trigger_play_off(self._seq_handle, -1)
 
+    @property
+    def next_row(self):
+        return libcvht.sequence_get_next_row(self._seq_handle)
+
     def __str__(self):
         ret = ""
         for itm in self:
             ret = ret + itm.__str__()
             ret = ret + "\n"
 
         return ret
```

### Comparing `vht-0.3.33/libvht/vhttimeline.py` & `vht-0.3.69/libvht/vhttimeline.py`

 * *Files identical despite different names*

### Comparing `vht-0.3.33/libvht/vhttimelinechange.py` & `vht-0.3.69/libvht/vhttimelinechange.py`

 * *Files identical despite different names*

### Comparing `vht-0.3.33/libvht/vhttimelinechanges.py` & `vht-0.3.69/libvht/vhttimelinechanges.py`

 * *Files identical despite different names*

### Comparing `vht-0.3.33/libvht/vhttimelineloop.py` & `vht-0.3.69/libvht/vhttimelineloop.py`

 * *Files identical despite different names*

### Comparing `vht-0.3.33/libvht/vhttimelineslices.py` & `vht-0.3.69/libvht/vhttimelineslices.py`

 * *Files identical despite different names*

### Comparing `vht-0.3.33/libvht/vhttimelinestrip.py` & `vht-0.3.69/libvht/vhttimelinestrip.py`

 * *Files identical despite different names*

### Comparing `vht-0.3.33/libvht/vhttimelinestrips.py` & `vht-0.3.69/libvht/vhttimelinestrips.py`

 * *Files identical despite different names*

### Comparing `vht-0.3.33/libvht/vhttimelineticks.py` & `vht-0.3.69/libvht/vhttimelineticks.py`

 * *Files identical despite different names*

### Comparing `vht-0.3.33/libvht/vhttrack.py` & `vht-0.3.69/libvht/vhttrack.py`

 * *Files identical despite different names*

### Comparing `vht-0.3.33/libvht/vhttracy.py` & `vht-0.3.69/libvht/vhttracy.py`

 * *Files identical despite different names*

### Comparing `vht-0.3.33/pyproject.toml` & `vht-0.3.69/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 [build-system]
-requires = ["setuptools", "wheel"]
+build-backend = 'setuptools.build_meta'
+requires = ["setuptools>=61.0"]
 
 [metadata]
 name = "vht"
-version = "0.3.33"
+version = "0.3.69"
 description = "vahatraker - a live MIDI sequencer for JACK"
 author = "Remigiusz Dybka"
 author_email = "remigiusz.dybka@gmail.com"
-license = "GPLv3+"
 url = "https://github.com/rdybka/vht"
 long_description = "file: README.md"
 long_description_content_type = "text/markdown"
 classifiers = [
     "Development Status :: 5 - Production/Stable",
     "Environment :: X11 Applications :: GTK",
     "Intended Audience :: End Users/Desktop",
@@ -25,14 +25,17 @@
 [options]
 packages = ["vht", "libvht"]
 install_requires = []
 
 [options.entry_points]
 vht = "vht.main:run"
 
+[options.build-dependencies]
+vht = ["jack"]
+
 [options.package_data]
 vht = ["data/*", "data/ctrl/*", "data/bank/*"]
 
 [options.data_files]
 "share/vht" = ["data/mandy.png", "data/vht.svg", "data/vht.png", "data/menu.ui"]
 "share/vht/ctrl" = ["data/ctrl/10-gm", "data/ctrl/20-zyn"]
 "share/vht/bank" = ["data/bank/10-gm1", "data/bank/20-gm2"]
@@ -43,14 +46,16 @@
 [options.extensions]
 "libvht/_libcvht" = ["libvht/libvht.c", 
 "libvht/libcvht_wrap.c",
 "libvht/midi_client.c",
 "libvht/jack_process.c",
 "libvht/midi_event.c",
 "libvht/module.c",
+"libvht/smf.c",
+"libvht/stolen.c",
 "libvht/row.c",
 "libvht/ctrlrow.c",
 "libvht/sequence.c",
 "libvht/track.c",
 "libvht/envelope.c",
 "libvht/timeline.c",
 "libvht/mandy.c",
```

### Comparing `vht-0.3.33/setup.py` & `vht-0.3.69/setup.py`

 * *Files 7% similar despite different names*

```diff
@@ -2,28 +2,30 @@
 
 from setuptools import setup, Extension
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setup(name = "vht",
-	version = "0.3.33",
+	version = "0.3.69",
 	description = "vahatraker - a live MIDI sequencer for JACK",
 	long_description=long_description,
 	long_description_content_type="text/markdown",
 	author = "Remigiusz Dybka",
 	author_email = "remigiusz.dybka@gmail.com",
 	url = "https://github.com/rdybka/vht",
 	license = 'GPLv3+',
 	ext_modules = [Extension("libvht/_libcvht", ["libvht/libvht.c",
 			"libvht/libcvht_wrap.c",
 			"libvht/midi_client.c",
 			"libvht/jack_process.c",
 			"libvht/midi_event.c",
 			"libvht/module.c",
+			"libvht/smf.c",
+			"libvht/stolen.c",
 			"libvht/row.c",
 			"libvht/ctrlrow.c",
 			"libvht/sequence.c",
 			"libvht/track.c",
 			"libvht/envelope.c",
 			"libvht/timeline.c",
 			"libvht/mandy.c",
```

### Comparing `vht-0.3.33/vht/autoexec.py` & `vht-0.3.69/vht/autoexec.py`

 * *Files identical despite different names*

### Comparing `vht-0.3.33/vht/bankcfg.py` & `vht-0.3.69/vht/bankcfg.py`

 * *Files identical despite different names*

### Comparing `vht-0.3.33/vht/capturebutton.py` & `vht-0.3.69/vht/capturebutton.py`

 * *Files identical despite different names*

### Comparing `vht-0.3.33/vht/configuration.py` & `vht-0.3.69/vht/configuration.py`

 * *Files 5% similar despite different names*

```diff
@@ -136,14 +136,17 @@
         self.timeline_delete_time = 0.25
         self.timeline_hint_time = 0.25
 
         self.render_mode = 2
         self.render_meter = 0
         self.render_secs = 5
         self.render_format = "flac"
+        self.render_midi = True
+        self.render_timecode = 0
+        self.render_ticks = 120
         self.render_folder = str(Path.home())
 
         self.key = {
             # sequenceview		shift, ctrl, alt
             "quit": cfgkey("q", False, True, False),
             "toggle_timeline": cfgkey("Tab", False, True, False),
             "toggle_console": cfgkey("grave", False, False, False),
@@ -336,14 +339,17 @@
 
         cfg["render"] = {
             "render_mode": str(self.render_mode),
             "render_secs": str(self.render_secs),
             "render_meter": str(self.render_meter),
             "render_format": self.render_format,
             "render_folder": self.render_folder,
+            "render_midi": self.render_midi,
+            "render_timecode": str(self.render_timecode),
+            "render_ticks": str(self.render_ticks),
         }
 
         cfg["other"] = {
             "new_tracks_left": self.new_tracks_left,
             "new_seqs_with_tracks": self.new_seqs_with_tracks,
             "port_popup": self.port_popup,
             "pnq_hack": self.pnq_hack,
@@ -403,15 +409,18 @@
                 mmp[mi] = str(mn) if mn else ""
 
         rnd = self.cfg_parser["render"]
         rnd["render_mode"] = str(self.render_mode)
         rnd["render_secs"] = str(self.render_secs)
         rnd["render_meter"] = str(self.render_meter)
         rnd["render_format"] = self.render_format
+        rnd["render_midi"] = str(self.render_midi)
         rnd["render_folder"] = self.render_folder
+        rnd["render_timecode"] = str(self.render_timecode)
+        rnd["render_ticks"] = str(self.render_ticks)
 
         oth = self.cfg_parser["other"]
         oth["new_tracks_left"] = str(self.new_tracks_left)
         oth["new_seqs_with_tracks"] = str(self.new_seqs_with_tracks)
         oth["port_popup"] = str(self.port_popup)
         oth["pnq_hack"] = str(self.pnq_hack)
         oth["inception"] = str(self.inception)
@@ -513,14 +522,17 @@
 
             rnd = self.cfg_parser["render"]
 
             self.render_mode = rnd.getint("render_mode")
             self.render_secs = rnd.getint("render_secs")
             self.render_meter = rnd.getint("render_meter")
             self.render_format = rnd["render_format"]
+            self.render_midi = rnd.getboolean("render_midi")
+            self.render_timecode = rnd.getint("render_timecode")
+            self.render_ticks = rnd.getint("render_ticks")
             self.render_folder = rnd["render_folder"]
 
             oth = self.cfg_parser["other"]
             self.new_tracks_left = oth.getboolean("new_tracks_left")
             self.new_seqs_with_tracks = oth.getboolean("new_seqs_with_tracks")
             self.port_popup = oth.getboolean("port_popup")
             self.pnq_hack = oth.getboolean("pnq_hack")
```

### Comparing `vht-0.3.33/vht/console.py` & `vht-0.3.69/vht/console.py`

 * *Files identical despite different names*

### Comparing `vht-0.3.33/vht/controllereditor.py` & `vht-0.3.69/vht/controllereditor.py`

 * *Files identical despite different names*

### Comparing `vht-0.3.33/vht/controllersview.py` & `vht-0.3.69/vht/controllersview.py`

 * *Files identical despite different names*

### Comparing `vht-0.3.33/vht/controllersviewrow.py` & `vht-0.3.69/vht/controllersviewrow.py`

 * *Files identical despite different names*

### Comparing `vht-0.3.33/vht/controllerundobuffer.py` & `vht-0.3.69/vht/controllerundobuffer.py`

 * *Files identical despite different names*

### Comparing `vht-0.3.33/vht/ctrlcfg.py` & `vht-0.3.69/vht/ctrlcfg.py`

 * *Files identical despite different names*

### Comparing `vht-0.3.33/vht/extras.py` & `vht-0.3.69/vht/extras.py`

 * *Files identical despite different names*

### Comparing `vht-0.3.33/vht/filerotator.py` & `vht-0.3.69/vht/filerotator.py`

 * *Files identical despite different names*

### Comparing `vht-0.3.33/vht/main.py` & `vht-0.3.69/vht/main.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 #!/usr/bin/env python3
 
 # vahatraker - a live MIDI sequencer for JACK
 #
-# Copyright (C) 2023 Remigiusz Dybka - remigiusz.dybka@gmail.com
+# Copyright (C) 2024 Remigiusz Dybka - remigiusz.dybka@gmail.com
 #
 # This program is free software: you can redistribute it and/or modify
 # it under the terms of the GNU General Public License as published by
 # the Free Software Foundation, either version 3 of the License, or
 # (at your option) any later version.
 #
 # This program is distributed in the hope that it will be useful,
@@ -33,14 +33,15 @@
 import time
 import pkg_resources
 
 from vht.mainwin import MainWin
 from vht.shortcutmayhem import ShortcutMayhem
 from vht.preferenceswin import PreferencesWin
 from vht.renderwin import RenderWin
+from vht.codedaemon import CodeDaemon
 from vht.portconfig import refresh_connections
 from vht import mod, cfg, ctrlcfg, autoexec, bankcfg, randomcomposer
 import vht.extras
 import vht.filerotator
 
 
 class VHTApp(Gtk.Application):
@@ -198,15 +199,15 @@
     def on_append(self, action, param):
         self.load(True)
 
     def on_about_dialog(self, action, param):
         ab = Gtk.AboutDialog(self.main_win)
         ab.set_license_type(Gtk.License.GPL_3_0)
         ab.set_copyright(
-            "Copyright (C) 2023 Remigiusz Dybka\nremigiusz.dybka@gmail.com\n@schtixfnord"
+            "Copyright (C) 2024 Remigiusz Dybka\nremigiusz.dybka@gmail.com"
         )
         pkg = pkg_resources.require("vht")[0]
         ab.set_version(pkg.version)
         ab.set_program_name("vahatraker")
         ab.set_comments("a live MIDI sequencer for JACK")
         ab.set_logo(
             GdkPixbuf.Pixbuf.new_from_file_at_size(
@@ -326,15 +327,15 @@
     for val in cfg.midi_in.values():
         if val:
             midig.append(val)
 
     vht.extras.register(mod)
     mod.set_midi_record_ignore(midig)
     randomcomposer.muzakize()
-
+    mod.cdaemon = CodeDaemon()
     # fix data path
     paths2try = []
 
     paths2try.append(os.path.normpath(os.path.join(pkg.module_path, "data")))
     paths2try.append(os.path.normpath(os.path.join(pkg.module_path, "share/vht")))
 
     p = pkg.module_path
```

### Comparing `vht-0.3.33/vht/mainwin.py` & `vht-0.3.69/vht/mainwin.py`

 * *Files 2% similar despite different names*

```diff
@@ -242,14 +242,15 @@
 
         rt = dialog.run()
         dialog.destroy()
         if rt == Gtk.ResponseType.CANCEL:
             return True
 
     def tick(self, wdg, param):
+        mod.cdaemon.tick()
         self.time_display.set_markup(
             """<span font_desc="Roboto bold" font_family="monospace" size="x-large">%s</span>"""
             % mod.time
         )
         if self.transport_switch.props.state != mod.transport:
             self.transport_switch.props.state = mod.transport
 
@@ -521,14 +522,15 @@
             for trk in mod[seq_id]:
                 if int(trk) in self.sequence_view.trk_cache:
                     del self.sequence_view.trk_cache[int(trk)]
 
                 if int(trk) in self.sequence_view.prop_view.trk_prop_cache:
                     del self.sequence_view.prop_view.trk_prop_cache[int(trk)]
 
+            mod.cdaemon.remove_seq(mod[seq_id])
             mod.del_sequence(seq_id)
             self.sequence_view.switch(nxt)
             mod.timeline.update()
             mod.thumbmanager.clear()
             return True
         elif type(seq_id) is tuple:
             curr = mod.curr_seq
```

### Comparing `vht-0.3.33/vht/mandymenu.py` & `vht-0.3.69/vht/mandymenu.py`

 * *Files identical despite different names*

### Comparing `vht-0.3.33/vht/mandyview.py` & `vht-0.3.69/vht/mandyview.py`

 * *Files 0% similar despite different names*

```diff
@@ -201,15 +201,16 @@
                 if trcid == 0 and not self.trc_pos:
                     self.trc_pos = (d["x"], d["y"])
 
                 tail = trc.tail
                 tl = len(tail)
 
                 tw = max(8, 8 * 0.5 / d["zoom"])
-                sm = 3
+                sm = 2
+
                 np = (
                     self.trc_pos[0] + (d["x"] - self.trc_pos[0]) / sm,
                     self.trc_pos[1] + (d["y"] - self.trc_pos[1]) / sm,
                 )
 
                 if math.isfinite(np[0]) and math.isfinite(np[1]):
                     self.trc_pos = np
@@ -540,15 +541,15 @@
 
         return False
 
     def tick(self, wdg, param):
         nt = time.time_ns()
 
         t = (nt - self.last_t) / 1000000
-        if t > 40:
+        if t > 15:
             self.redraw()
             self.last_t = nt
 
         return True
 
     def on_enter(self, wdg, prm):
         self.entered = True
```

### Comparing `vht-0.3.33/vht/midimapview.py` & `vht-0.3.69/vht/midimapview.py`

 * *Files identical despite different names*

### Comparing `vht-0.3.33/vht/midimapviewrow.py` & `vht-0.3.69/vht/midimapviewrow.py`

 * *Files identical despite different names*

### Comparing `vht-0.3.33/vht/notebooklabel.py` & `vht-0.3.69/vht/notebooklabel.py`

 * *Files identical despite different names*

### Comparing `vht-0.3.33/vht/poormanspiano.py` & `vht-0.3.69/vht/poormanspiano.py`

 * *Files identical despite different names*

### Comparing `vht-0.3.33/vht/portconfig.py` & `vht-0.3.69/vht/portconfig.py`

 * *Files identical despite different names*

### Comparing `vht-0.3.33/vht/portconfigpopover.py` & `vht-0.3.69/vht/portconfigpopover.py`

 * *Files identical despite different names*

### Comparing `vht-0.3.33/vht/portconfigview.py` & `vht-0.3.69/vht/portconfigview.py`

 * *Files 2% similar despite different names*

```diff
@@ -47,17 +47,17 @@
         self.head_row.pack_start(Gtk.Label(self.lab1), False, False, 0)
         self.head_row.pack_end(Gtk.Label(self.lab2), False, False, 0)
 
         self.insert(self.head_row, 0)
         wdg = self.get_children()[0]
         wdg.set_sensitive(False)
 
-    def add(self, prtname, state):
+    def add(self, prtname, pretty, state):
         rw = Gtk.Box()
-        rw.pack_start(Gtk.Label(prtname), False, False, 0)
+        rw.pack_start(Gtk.Label(pretty if pretty else prtname), False, False, 0)
         statewdg = Gtk.CheckButton()
         statewdg.set_active(state)
         statewdg.connect("toggled", self.tgl_meta, prtname)
         rw.pack_end(statewdg, False, False, 0)
         self.insert(rw, -1)
 
     def tgl_meta(self, widget, prtname):
@@ -131,19 +131,19 @@
         for prt in mod.ports:
             if prt.mine and prt.input:
                 inp = prt
 
         for prt in mod.ports:
             if prt.type == "midi" and not prt.mine:
                 if prt.output:
-                    self.bl_in.add(*[prt.name, inp in prt.connections])
+                    self.bl_in.add(*[prt.name, prt.pname, inp in prt.connections])
 
         for p in mod.extras["portconfig"]["in"]:
             if not p in mod.ports:
-                self.bl_unv_in.add(p, 1)
+                self.bl_unv_in.add(p, p, 1)
 
         # outputs
         inp = None
         outp = None
 
         for prt in mod.ports:
             if prt.mine and prt.output:
@@ -153,19 +153,19 @@
         for prt in mod.ports:
             if prt.type == "midi" and not prt.mine:
                 if prt.input:
                     conn = False
                     if inp and inp in prt.connections:
                         conn = True
 
-                    self.bl_out.add(prt.name, conn)
+                    self.bl_out.add(prt.name, prt.pname, conn)
 
         for p in mod.extras["portconfig"]["out"][act_out]:
             if not p in mod.ports:
-                self.bl_unv_out.add(p, 1)
+                self.bl_unv_out.add(p, p, 1)
 
         self.show_all()
 
         if len(self.bl_unv_out) > 1:
             self.bl_unv_out.show()
         else:
             self.bl_unv_out.hide()
```

### Comparing `vht-0.3.33/vht/preferenceswin.py` & `vht-0.3.69/vht/preferenceswin.py`

 * *Files 4% similar despite different names*

```diff
@@ -242,24 +242,26 @@
         grid.set_margin_right(mrg)
 
         fr, gr = self.create_frame("Default input", mrg)
         cmb = Gtk.ComboBoxText()
         cmb.set_hexpand(True)
         cmb.append_text("none")
         pp = []
+        pretty = {}
         for prt in self.mod.ports:
             if prt.type == "midi" and not prt.mine and prt.output:
                 pp.append(prt.name)
+                pretty[prt.name] = prt.pname
 
         dinp = self.cfg.midi_default_input
         if dinp and dinp not in pp:
             pp.append(dinp)
 
         for prt in pp:
-            cmb.append_text(prt)
+            cmb.append(prt, pretty[prt] if prt in pretty else prt)
 
         dinp = self.cfg.midi_default_input
         if dinp and dinp in pp:
             cmb.set_active(pp.index(dinp) + 1)
         else:
             cmb.set_active(0)
 
@@ -269,24 +271,26 @@
 
         fr, gr = self.create_frame("Default output", mrg)
         cmb = Gtk.ComboBoxText()
         cmb.set_hexpand(True)
         cmb.append_text("none")
 
         pp = []
+        pretty = {}
         for prt in self.mod.ports:
             if prt.type == "midi" and not prt.mine and prt.input:
                 pp.append(prt.name)
+                pretty[prt.name] = prt.pname
 
         doutp = self.cfg.midi_default_output
         if doutp and doutp not in pp:
             pp.append(doutp)
 
         for prt in pp:
-            cmb.append_text(prt)
+            cmb.append(prt, pretty[prt] if prt in pretty else prt)
 
         doutp = self.cfg.midi_default_output
         if doutp and doutp in pp:
             cmb.set_active(pp.index(doutp) + 1)
         else:
             cmb.set_active(0)
 
@@ -370,46 +374,72 @@
         )
         bx.pack_start(self.qc_2_ctrl_ent, False, False, 0)
         bx.pack_end(self.qc_2_def_slider, True, True, 0)
         gr.attach(bx, 0, 2, 1, 1)
 
         grid.attach(fr, 0, 2, 1, 1)
 
+        fr, gr = self.create_frame("Midi export SMPTE", mrg)
+
+        cmb = Gtk.ComboBoxText()
+        cmb.append_text("30fps")
+        cmb.append_text("25fps")
+
+        cmb.set_active(self.cfg.render_timecode)
+        cmb.connect("changed", self.on_combo_rendertc_changed)
+
+        tick_slider = self.create_slider(0, self.cfg.render_ticks, 40, 120, 4)
+
+        tick_slider.add_mark(40, Gtk.PositionType.TOP)
+        tick_slider.add_mark(80, Gtk.PositionType.TOP)
+        tick_slider.add_mark(100, Gtk.PositionType.TOP)
+        tick_slider.add_mark(120, Gtk.PositionType.TOP)
+
+        bx = Gtk.Box()
+        bx.set_hexpand(True)
+        bx.pack_start(cmb, False, False, 0)
+        bx.pack_end(Gtk.Label.new("ticks/frame"), False, False, 0)
+
+        bx.pack_end(tick_slider, True, True, 0)
+
+        gr.attach(bx, 0, 0, 1, 1)
+        grid.attach(fr, 0, 3, 1, 1)
+
         fr, gr = self.create_frame("White piano keys", mrg)
         self.piano_white_keys_ent = self.create_entry(self.cfg.piano_white_keys, 14)
         rsbutt = self.create_reset_butt(2)
         bx = Gtk.Box()
         bx.set_hexpand(True)
         bx.pack_start(self.piano_white_keys_ent, False, False, 0)
         bx.pack_end(rsbutt, False, False, 0)
 
         gr.attach(bx, 0, 0, 1, 1)
-        grid.attach(fr, 0, 3, 1, 1)
+        grid.attach(fr, 0, 4, 1, 1)
 
         fr, gr = self.create_frame("Black piano keys", mrg)
         self.piano_black_keys_ent = self.create_entry(self.cfg.piano_black_keys, 10)
         rsbutt = self.create_reset_butt(1)
         bx = Gtk.Box()
         bx.set_hexpand(True)
         bx.pack_start(self.piano_black_keys_ent, False, False, 0)
         bx.pack_end(rsbutt, False, False, 0)
 
         gr.attach(bx, 0, 0, 1, 1)
-        grid.attach(fr, 0, 4, 1, 1)
+        grid.attach(fr, 0, 5, 1, 1)
 
         fr, gr = self.create_frame("Velocity keys", mrg)
         self.velocity_keys_ent = self.create_entry(self.cfg.velocity_keys, 7)
         rsbutt = self.create_reset_butt(0)
         bx = Gtk.Box()
         bx.set_hexpand(True)
         bx.pack_start(self.velocity_keys_ent, False, False, 0)
         bx.pack_end(rsbutt, False, False, 0)
 
         gr.attach(bx, 0, 0, 1, 1)
-        grid.attach(fr, 0, 5, 1, 1)
+        grid.attach(fr, 0, 6, 1, 1)
 
         return grid
 
     def create_box4(self):
         grid = Gtk.Grid()
         mrg = 5
         grid.set_margin_top(mrg)
@@ -614,37 +644,43 @@
         if data == 1:
             self.cfg.quick_control_1_def = int(val)
         if data == 2:
             self.cfg.quick_control_2_def = int(val)
         if data == 3:
             self.parent.set_opacity(self.cfg.window_opacity)
             self.cfg.window_opacity = val
+        if data == 4:
+            self.cfg.render_ticks = int(val)
 
     def on_combo_midi_input_changed(self, wdg):
-        self.cfg.midi_default_input = wdg.get_active_text() if wdg.get_active() else ""
+        self.cfg.midi_default_input = wdg.get_active_id() if wdg.get_active() else ""
         pc = self.mod.extras["portconfig"]
         if self.cfg.midi_default_input and self.cfg.midi_default_input not in pc["in"]:
             pc["in"].append(self.cfg.midi_default_input)
 
         refresh_connections(self.mod, self.cfg)
         if self.parent._status_bar.portpopover.pooped:
             self.parent._status_bar.portpopover.refresh()
 
     def on_combo_midi_output_changed(self, wdg):
-        self.cfg.midi_default_output = wdg.get_active_text() if wdg.get_active() else ""
+        self.cfg.midi_default_output = wdg.get_active_id() if wdg.get_active() else ""
         pc = self.mod.extras["portconfig"]
         if (
             self.cfg.midi_default_output
             and self.cfg.midi_default_output not in pc["out"][0]
         ):
             pc["out"][0].append(self.cfg.midi_default_output)
         refresh_connections(self.mod, self.cfg)
         if self.parent._status_bar.portpopover.pooped:
             self.parent._status_bar.portpopover.refresh()
 
+    def on_combo_rendertc_changed(self, wdg):
+        v = wdg.get_active()
+        self.cfg.render_timecode = v
+
     def on_combo_mouseover_changed(self, wdg):
         v = wdg.get_active()
         n = 0
         t = 0
 
         if v == 1:
             t = True
```

### Comparing `vht-0.3.33/vht/probeditor.py` & `vht-0.3.69/vht/probeditor.py`

 * *Files identical despite different names*

### Comparing `vht-0.3.33/vht/propview.py` & `vht-0.3.69/vht/propview.py`

 * *Files identical despite different names*

### Comparing `vht-0.3.33/vht/pulsar.py` & `vht-0.3.69/vht/pulsar.py`

 * *Files identical despite different names*

### Comparing `vht-0.3.33/vht/randomcomposer.py` & `vht-0.3.69/vht/randomcomposer.py`

 * *Files identical despite different names*

### Comparing `vht-0.3.33/vht/renderer.py` & `vht-0.3.69/vht/renderer.py`

 * *Files 12% similar despite different names*

```diff
@@ -29,14 +29,15 @@
 
         self._avail = True
         self._pre_delay_start = 0
         self._finished = False
         self._queue = []
         self._seqs = []
         self._orig_pm = None
+        self._midi_file = None
 
         try:
             prc = subprocess.Popen(
                 ["jack_capture", "--version"],
                 stdin=subprocess.PIPE,
                 stdout=subprocess.PIPE,
                 stderr=subprocess.PIPE,
@@ -62,17 +63,20 @@
             return True
 
         if self.mod.render_mode == 23 and self.mod.play == 0:
             self.mod.freewheel_off()
 
             if self.mod.play_mode == 1:
                 self.mod.play_mode = self._orig_pm
-
             if self._proc:
                 stdout, stderr = self._proc.communicate(input="\n", timeout=5)
+                if self._midi_file:
+                    self.mod.dump_midi(
+                        self._midi_file, self.cfg.render_timecode, self.cfg.render_ticks
+                    )
                 self._proc = None
             if self._queue:
                 self.start_queue()
             else:
                 self._finished = True
                 self.mod.mainwin.timeline_view.follow = False
                 if self._proc:
@@ -102,14 +106,19 @@
 
     def start_live(self, folder, filename, fmt, meter):
         opts = ["jack_capture"]
         opts.append("-f")
         opts.append(fmt)
         opts.append("-fp")
         opts.append(os.path.join(folder, filename + "_"))
+        if self.cfg.render_midi:
+            self._midi_file = os.path.join(folder, filename + ".mid")
+        else:
+            self._midi_file = None
+
         meters = ["none", "vu", "ppm", "dpm", "jf", "sco"]
         if meter > 0:
             opts.append("-mb")
             opts.append("-mt")
             opts.append(meters[meter])
 
         self._orig_pm = self.mod.play_mode
@@ -130,14 +139,18 @@
         opts = ["jack_capture"]
         opts.append("-jf")
         # opts.append("--daemon")
         opts.append("-f")
         opts.append(fmt)
         opts.append("-fp")
         opts.append(os.path.join(folder, filename + "_"))
+        if self.cfg.render_midi:
+            self._midi_file = os.path.join(folder, filename + ".mid")
+        else:
+            self._midi_file = None
 
         self.mod.render_mode = 3
         self._orig_pm = self.mod.play_mode
 
         self._proc = subprocess.Popen(
             opts,
             stdin=subprocess.PIPE,
@@ -160,17 +173,20 @@
         opts = ["jack_capture"]
         opts.append("-jf")
         # opts.append("--daemon")
         opts.append("-f")
         opts.append(fmt)
         opts.append("-fp")
         opts.append(os.path.join(folder, filename + ("_seq%02d" % seqid) + "_"))
+        if self.cfg.render_midi:
+            self._midi_file = os.path.join(folder, filename + ("_seq%02d.mid" % seqid))
 
         self.mod.play = 0
         self.mod.reset()
+        self.mod.reset()  # in case some old note-offs hang
         for s in self.mod:
             s.playing = False
 
         self.mod.play_mode = 0
         self.mod.render_mode = 1
         self._orig_pm = self.mod.play_mode
         self.mod.set_lead_out(lead_out)
@@ -212,14 +228,18 @@
         opts = ["jack_capture"]
         opts.append("-jf")
         # opts.append("--daemon")
         opts.append("-f")
         opts.append(fmt)
         opts.append("-fp")
         opts.append(os.path.join(folder, filename + "_"))
+        if self.cfg.render_midi:
+            self._midi_file = os.path.join(folder, filename + ".mid")
+        else:
+            self._midi_file = None
 
         self.mod.play = 0
         self.mod.reset()
         self._seqs = []
         for s in self.mod:
             if s.playing:
                 self._seqs.append(s.index)
@@ -250,8 +270,12 @@
         self.mod.mainwin.timeline_view.follow = False
 
         if self._proc:
             stdout, stderr = self._proc.communicate(input="\n", timeout=5)
             self._proc = None
             self._queue = []
             self._finished = True
+            if self._midi_file:
+                self.mod.dump_midi(
+                    self._midi_file, self.cfg.render_timecode, self.cfg.render_ticks
+                )
             self.mod.render_mode = 0
```

### Comparing `vht-0.3.33/vht/renderwin.py` & `vht-0.3.69/vht/renderwin.py`

 * *Files 2% similar despite different names*

```diff
@@ -80,58 +80,68 @@
         if cfg.render_format in self.formats:
             self.format_cmb.set_active(self.formats.index(cfg.render_format))
         else:
             self.format_cmb.set_active(0)
 
         self.grid.attach(self.format_cmb, 1, 1, 2, 1)
 
+        self.midi_sw = Gtk.Switch()
+        self.midi_sw.set_active(cfg.render_midi)
+        self.midi_sw.connect("state-set", self.on_midi_switch)
+
+        lab = Gtk.Label.new("midi:")
+        bx = Gtk.Box()
+        bx.pack_start(lab, False, False, 0)
+        bx.pack_end(self.midi_sw, False, False, 0)
+        self.grid.attach(bx, 2, 2, 1, 1)
+
         lab = Gtk.Label.new("dest:")
         lab.set_xalign(labx)
-        self.grid.attach(lab, 0, 2, 1, 1)
+        self.grid.attach(lab, 0, 3, 1, 1)
 
         self.butt_fc = Gtk.FileChooserButton.new(
             "select output folder", Gtk.FileChooserAction.SELECT_FOLDER
         )
         self.butt_fc.connect("file-set", self.on_folder_set)
         self.butt_fc.set_current_folder(cfg.render_folder)
-        self.grid.attach(self.butt_fc, 1, 2, 2, 1)
+        self.grid.attach(self.butt_fc, 1, 3, 2, 1)
 
         lab = Gtk.Label.new("silence:")
         lab.set_xalign(labx)
-        self.grid.attach(lab, 0, 3, 1, 1)
+        self.grid.attach(lab, 0, 4, 1, 1)
 
         box = Gtk.Box()
         self.secs_adj = Gtk.Adjustment(0, 0, 123, 1.0, 1.0)
         self.secs_button = Gtk.SpinButton()
         self.secs_button.set_adjustment(self.secs_adj)
         self.secs_adj.set_value(cfg.render_secs)
         self.secs_adj.connect("value-changed", self.on_secs_changed)
-        self.grid.attach(self.secs_button, 1, 3, 2, 1)
+        self.grid.attach(self.secs_button, 1, 4, 2, 1)
 
         lab = Gtk.Label.new("meter:")
         lab.set_xalign(labx)
-        self.grid.attach(lab, 0, 4, 1, 1)
+        self.grid.attach(lab, 0, 5, 1, 1)
 
         self.meter_cmb = Gtk.ComboBoxText()
         self.meters = ["none", "vu", "ppm", "dpm", "jf", "sco"]
         for f in self.meters:
             self.meter_cmb.append_text(f)
 
         self.meter_cmb.set_active(cfg.render_meter)
         self.meter_cmb.connect("changed", self.on_meter_cmb_changed)
 
-        self.grid.attach(self.meter_cmb, 1, 4, 2, 1)
+        self.grid.attach(self.meter_cmb, 1, 5, 2, 1)
 
         self.rbutt = Gtk.Button()
         self.rbutt.set_label("Start!")
         self.rbutt.connect("clicked", self.on_go_clicked)
-        self.grid.attach(self.rbutt, 2, 6, 1, 1)
+        self.grid.attach(self.rbutt, 2, 7, 1, 1)
 
         self.progress = Gtk.ProgressBar()
-        self.grid.attach(self.progress, 0, 5, 3, 1)
+        self.grid.attach(self.progress, 0, 6, 3, 1)
 
         self.mode_cmb.set_active(cfg.render_mode)
 
         if not mod.renderer.available:
             self.rbutt.set_sensitive(False)
             self.rbutt.set_label("jack_capture not found")
 
@@ -149,14 +159,17 @@
 
     def on_folder_set(self, wdg):
         self.cfg.render_folder = wdg.get_filename()
 
     def on_meter_cmb_changed(self, wdg):
         self.cfg.render_meter = wdg.get_active()
 
+    def on_midi_switch(self, wdg, prm):
+        self.cfg.render_midi = prm
+
     def on_mode_cmb_changed(self, wdg):
         self.cfg.render_mode = wdg.get_active()
         if self.cfg.render_mode == 2:
             self.secs_button.set_sensitive(False)
             self.meter_cmb.set_sensitive(True)
         else:
             self.secs_button.set_sensitive(True)
```

### Comparing `vht-0.3.33/vht/sequencelistview.py` & `vht-0.3.69/vht/sequencelistview.py`

 * *Files identical despite different names*

### Comparing `vht-0.3.33/vht/sequencepropviewpopover.py` & `vht-0.3.69/vht/sequencepropviewpopover.py`

 * *Files identical despite different names*

### Comparing `vht-0.3.33/vht/sequencetriggersview.py` & `vht-0.3.69/vht/sequencetriggersview.py`

 * *Files identical despite different names*

### Comparing `vht-0.3.33/vht/sequenceview.py` & `vht-0.3.69/vht/sequenceview.py`

 * *Files 2% similar despite different names*

```diff
@@ -16,14 +16,15 @@
 # along with this program.  If not, see <http://www.gnu.org/licenses/>.
 
 from vht.trackpropview import TrackPropView
 from vht.portconfig import *
 from vht.propview import PropView
 from vht.trackview import TrackView
 from vht.sidetrackview import SideTrackView
+from vht.codedaemon import CodeDaemon
 from vht import *
 import cairo
 import gi
 import copy
 
 gi.require_version("Gtk", "3.0")
 from gi.repository import Gdk, Gtk, Gio, GObject
@@ -840,14 +841,16 @@
 
         self._side_box.remove(self._side_box.get_children()[0])
 
     def load(self, filename, append=False):
         close_connections(mod)
         TrackView.leave_all()
 
+        del mod.cdaemon
+        mod.clear_popups()
         self.clear()
         for i in self.trk_cache:
             self.trk_cache[i].destroy()
 
         for i in self.prop_view.trk_prop_cache:
             self.prop_view.trk_prop_cache[i].destroy()
 
@@ -883,26 +886,28 @@
             mod.timeline_view.fix_extras()
             mod.seqlist.configure()
             mod.seqlist.redraw()
 
             mod.mainwin.seq_mode_butt_ignore_signal = True
             mod.mainwin.seq_mode_butt.set_active(not mod.play_mode)
             mod.mainwin.seq_mode_butt_ignore_signal = False
+            mod.cdaemon = CodeDaemon()
             return True
         else:
             mod.new()
             randomcomposer.muzakize()
             self.seq = mod[0]
             self.build()
             mod.timeline_view.fix_extras()
             mod.seqlist.configure()
             mod.seqlist.redraw()
             mod.mainwin.seq_mode_butt_ignore_signal = True
             mod.mainwin.seq_mode_butt.set_active(not mod.play_mode)
             mod.mainwin.seq_mode_butt_ignore_signal = False
+            mod.cdaemon = CodeDaemon()
             return False
 
     def switch(self, new_seq):
         mod.clear_popups()
         if mod.active_track:
             if mod.active_track.edit:
                 self.active_tracks[self.seq.index] = mod.active_track
```

### Comparing `vht-0.3.33/vht/shortcutmayhem.py` & `vht-0.3.69/vht/shortcutmayhem.py`

 * *Files identical despite different names*

### Comparing `vht-0.3.33/vht/sidetrackview.py` & `vht-0.3.69/vht/sidetrackview.py`

 * *Files identical despite different names*

### Comparing `vht-0.3.33/vht/statusbar.py` & `vht-0.3.69/vht/statusbar.py`

 * *Files identical despite different names*

### Comparing `vht-0.3.33/vht/thumbmanager.py` & `vht-0.3.69/vht/thumbmanager.py`

 * *Files identical despite different names*

### Comparing `vht-0.3.33/vht/timelineview.py` & `vht-0.3.69/vht/timelineview.py`

 * *Files identical despite different names*

### Comparing `vht-0.3.33/vht/timeshifteditor.py` & `vht-0.3.69/vht/timeshifteditor.py`

 * *Files identical despite different names*

### Comparing `vht-0.3.33/vht/trackpropview.py` & `vht-0.3.69/vht/trackpropview.py`

 * *Files identical despite different names*

### Comparing `vht-0.3.33/vht/trackpropviewpopover.py` & `vht-0.3.69/vht/trackpropviewpopover.py`

 * *Files identical despite different names*

### Comparing `vht-0.3.33/vht/trackundobuffer.py` & `vht-0.3.69/vht/trackundobuffer.py`

 * *Files identical despite different names*

### Comparing `vht-0.3.33/vht/trackview.py` & `vht-0.3.69/vht/trackview.py`

 * *Files identical despite different names*

### Comparing `vht-0.3.33/vht/trackviewpointer.py` & `vht-0.3.69/vht/trackviewpointer.py`

 * *Files identical despite different names*

### Comparing `vht-0.3.33/vht/velocityeditor.py` & `vht-0.3.69/vht/velocityeditor.py`

 * *Files identical despite different names*

### Comparing `vht-0.3.33/vht.egg-info/PKG-INFO` & `vht-0.3.69/vht.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vht
-Version: 0.3.33
+Version: 0.3.69
 Summary: vahatraker - a live MIDI sequencer for JACK
 Home-page: https://github.com/rdybka/vht
 Author: Remigiusz Dybka
 Author-email: remigiusz.dybka@gmail.com
 License: GPLv3+
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: X11 Applications :: GTK
```

### Comparing `vht-0.3.33/vht.egg-info/SOURCES.txt` & `vht-0.3.69/vht.egg-info/SOURCES.txt`

 * *Files 5% similar despite different names*

```diff
@@ -38,14 +38,17 @@
 libvht/midi_event.h
 libvht/module.c
 libvht/module.h
 libvht/row.c
 libvht/row.h
 libvht/sequence.c
 libvht/sequence.h
+libvht/smf.c
+libvht/smf.h
+libvht/stolen.c
 libvht/timeline.c
 libvht/timeline.h
 libvht/track.c
 libvht/track.h
 libvht/tracy.c
 libvht/tracy.h
 libvht/vhtcolumn.py
@@ -70,14 +73,15 @@
 libvht/vhttimelineticks.py
 libvht/vhttrack.py
 libvht/vhttracy.py
 vht/__init__.py
 vht/autoexec.py
 vht/bankcfg.py
 vht/capturebutton.py
+vht/codedaemon.py
 vht/configuration.py
 vht/console.py
 vht/controllereditor.py
 vht/controllersview.py
 vht/controllersviewrow.py
 vht/controllerundobuffer.py
 vht/ctrlcfg.py
```

