# Comparing `tmp/pyguiadapter-0.3.4.tar.gz` & `tmp/pyguiadapter-0.3.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyguiadapter-0.3.4.tar", max compression
+gzip compressed data, was "pyguiadapter-0.3.5.tar", max compression
```

## Comparing `pyguiadapter-0.3.4.tar` & `pyguiadapter-0.3.5.tar`

### file list

```diff
@@ -1,273 +1,273 @@
--rw-r--r--   0        0        0    35821 2024-04-14 16:11:23.455323 pyguiadapter-0.3.4/License
--rw-r--r--   0        0        0      108 2024-04-17 16:38:11.248187 pyguiadapter-0.3.4/pyguiadapter/__init__.py
--rw-r--r--   0        0        0      139 2024-04-17 15:57:53.099012 pyguiadapter-0.3.4/pyguiadapter/adapter/__init__.py
--rw-r--r--   0        0        0     9877 2024-04-29 11:00:31.764154 pyguiadapter-0.3.4/pyguiadapter/adapter/adapter.py
--rw-r--r--   0        0        0     5463 2024-04-29 10:52:58.130370 pyguiadapter-0.3.4/pyguiadapter/adapter/bundle.py
--rw-r--r--   0        0        0      198 2024-04-17 15:43:54.841916 pyguiadapter-0.3.4/pyguiadapter/adapter/constants.py
--rw-r--r--   0        0        0     1684 2024-04-17 15:48:37.357738 pyguiadapter-0.3.4/pyguiadapter/adapter/executor.py
--rw-r--r--   0        0        0     1593 2024-04-17 15:52:24.455478 pyguiadapter-0.3.4/pyguiadapter/commons.py
--rw-r--r--   0        0        0      199 2024-04-14 16:11:23.461322 pyguiadapter-0.3.4/pyguiadapter/exceptions.py
--rw-r--r--   0        0        0        0 2024-04-14 16:11:23.461322 pyguiadapter-0.3.4/pyguiadapter/interact/__init__.py
--rw-r--r--   0        0        0     5119 2024-04-17 16:06:29.919169 pyguiadapter-0.3.4/pyguiadapter/interact/ulogging.py
--rw-r--r--   0        0        0    12531 2024-04-14 16:11:23.461322 pyguiadapter-0.3.4/pyguiadapter/interact/upopup.py
--rw-r--r--   0        0        0     1074 2024-04-20 13:02:56.774164 pyguiadapter-0.3.4/pyguiadapter/interact/uprint.py
--rw-r--r--   0        0        0      753 2024-04-14 16:11:23.462322 pyguiadapter-0.3.4/pyguiadapter/res/icons/abnormal.svg
--rw-r--r--   0        0        0      563 2024-04-14 16:11:23.462322 pyguiadapter-0.3.4/pyguiadapter/res/icons/acoustic.svg
--rw-r--r--   0        0        0      437 2024-04-14 16:11:23.462322 pyguiadapter-0.3.4/pyguiadapter/res/icons/activity-source.svg
--rw-r--r--   0        0        0      721 2024-04-14 16:11:23.462322 pyguiadapter-0.3.4/pyguiadapter/res/icons/add-computer.svg
--rw-r--r--   0        0        0     1074 2024-04-14 16:11:23.463322 pyguiadapter-0.3.4/pyguiadapter/res/icons/add-picture.svg
--rw-r--r--   0        0        0      556 2024-04-14 16:11:23.463322 pyguiadapter-0.3.4/pyguiadapter/res/icons/add-print.svg
--rw-r--r--   0        0        0      611 2024-04-14 16:11:23.463322 pyguiadapter-0.3.4/pyguiadapter/res/icons/add-user.svg
--rw-r--r--   0        0        0      820 2024-04-14 16:11:23.463322 pyguiadapter-0.3.4/pyguiadapter/res/icons/add-web.svg
--rw-r--r--   0        0        0      444 2024-04-14 16:11:23.463322 pyguiadapter-0.3.4/pyguiadapter/res/icons/airplay.svg
--rw-r--r--   0        0        0      744 2024-04-14 16:11:23.463322 pyguiadapter-0.3.4/pyguiadapter/res/icons/api-app.svg
--rw-r--r--   0        0        0      915 2024-04-14 16:11:23.463322 pyguiadapter-0.3.4/pyguiadapter/res/icons/application-effect.svg
--rw-r--r--   0        0        0      513 2024-04-14 16:11:23.464322 pyguiadapter-0.3.4/pyguiadapter/res/icons/application-one.svg
--rw-r--r--   0        0        0      471 2024-04-14 16:11:23.464322 pyguiadapter-0.3.4/pyguiadapter/res/icons/application-two.svg
--rw-r--r--   0        0        0      444 2024-04-14 16:11:23.464322 pyguiadapter-0.3.4/pyguiadapter/res/icons/area-map.svg
--rw-r--r--   0        0        0     1704 2024-04-14 16:11:23.464322 pyguiadapter-0.3.4/pyguiadapter/res/icons/arithmetic-buttons.svg
--rw-r--r--   0        0        0      886 2024-04-14 16:11:23.464322 pyguiadapter-0.3.4/pyguiadapter/res/icons/arithmetic-one.svg
--rw-r--r--   0        0        0     1051 2024-04-14 16:11:23.464322 pyguiadapter-0.3.4/pyguiadapter/res/icons/arrow-keys.svg
--rw-r--r--   0        0        0      510 2024-04-14 16:11:23.464322 pyguiadapter-0.3.4/pyguiadapter/res/icons/audio-file.svg
--rw-r--r--   0        0        0      806 2024-04-14 16:11:23.464322 pyguiadapter-0.3.4/pyguiadapter/res/icons/audit.svg
--rw-r--r--   0        0        0      503 2024-04-14 16:11:23.465322 pyguiadapter-0.3.4/pyguiadapter/res/icons/average.svg
--rw-r--r--   0        0        0      871 2024-04-14 16:11:23.465322 pyguiadapter-0.3.4/pyguiadapter/res/icons/bitcoin.svg
--rw-r--r--   0        0        0      753 2024-04-14 16:11:23.465322 pyguiadapter-0.3.4/pyguiadapter/res/icons/blackboard.svg
--rw-r--r--   0        0        0      633 2024-04-14 16:11:23.465322 pyguiadapter-0.3.4/pyguiadapter/res/icons/blocks-and-arrows.svg
--rw-r--r--   0        0        0      261 2024-04-14 16:11:23.465322 pyguiadapter-0.3.4/pyguiadapter/res/icons/bluetooth.svg
--rw-r--r--   0        0        0      794 2024-04-14 16:11:23.466322 pyguiadapter-0.3.4/pyguiadapter/res/icons/bookmark-three.svg
--rw-r--r--   0        0        0      981 2024-04-14 16:11:23.466322 pyguiadapter-0.3.4/pyguiadapter/res/icons/broadcast.svg
--rw-r--r--   0        0        0      993 2024-04-14 16:11:23.466322 pyguiadapter-0.3.4/pyguiadapter/res/icons/browser.svg
--rw-r--r--   0        0        0     1399 2024-04-14 16:11:23.466322 pyguiadapter-0.3.4/pyguiadapter/res/icons/bug.svg
--rw-r--r--   0        0        0      978 2024-04-14 16:11:23.466322 pyguiadapter-0.3.4/pyguiadapter/res/icons/bytedance-mini-app.svg
--rw-r--r--   0        0        0      334 2024-04-14 16:11:23.466322 pyguiadapter-0.3.4/pyguiadapter/res/icons/card-two.svg
--rw-r--r--   0        0        0      643 2024-04-14 16:11:23.466322 pyguiadapter-0.3.4/pyguiadapter/res/icons/carousel-video.svg
--rw-r--r--   0        0        0      849 2024-04-14 16:11:23.466322 pyguiadapter-0.3.4/pyguiadapter/res/icons/carousel.svg
--rw-r--r--   0        0        0      685 2024-04-14 16:11:23.467323 pyguiadapter-0.3.4/pyguiadapter/res/icons/cast-screen.svg
--rw-r--r--   0        0        0      472 2024-04-14 16:11:23.467323 pyguiadapter-0.3.4/pyguiadapter/res/icons/category-management.svg
--rw-r--r--   0        0        0      443 2024-04-14 16:11:23.467323 pyguiadapter-0.3.4/pyguiadapter/res/icons/caution.svg
--rw-r--r--   0        0        0     1016 2024-04-14 16:11:23.467323 pyguiadapter-0.3.4/pyguiadapter/res/icons/certificate.svg
--rw-r--r--   0        0        0      634 2024-04-14 16:11:23.467323 pyguiadapter-0.3.4/pyguiadapter/res/icons/check-one.svg
--rw-r--r--   0        0        0      697 2024-04-14 16:11:23.467323 pyguiadapter-0.3.4/pyguiadapter/res/icons/checklist.svg
--rw-r--r--   0        0        0     1023 2024-04-14 16:11:23.467323 pyguiadapter-0.3.4/pyguiadapter/res/icons/chip.svg
--rw-r--r--   0        0        0      519 2024-04-14 16:11:23.467323 pyguiadapter-0.3.4/pyguiadapter/res/icons/classroom.svg
--rw-r--r--   0        0        0      478 2024-04-14 16:11:23.468322 pyguiadapter-0.3.4/pyguiadapter/res/icons/clipboard.svg
--rw-r--r--   0        0        0      576 2024-04-14 16:11:23.468322 pyguiadapter-0.3.4/pyguiadapter/res/icons/close-one.svg
--rw-r--r--   0        0        0     1211 2024-04-14 16:11:23.468322 pyguiadapter-0.3.4/pyguiadapter/res/icons/cloud-storage.svg
--rw-r--r--   0        0        0      536 2024-04-14 16:11:23.468322 pyguiadapter-0.3.4/pyguiadapter/res/icons/code-brackets.svg
--rw-r--r--   0        0        0      547 2024-04-14 16:11:23.468322 pyguiadapter-0.3.4/pyguiadapter/res/icons/code-download.svg
--rw-r--r--   0        0        0      639 2024-04-14 16:11:23.468322 pyguiadapter-0.3.4/pyguiadapter/res/icons/code-laptop.svg
--rw-r--r--   0        0        0      346 2024-04-14 16:11:23.468322 pyguiadapter-0.3.4/pyguiadapter/res/icons/code-one.svg
--rw-r--r--   0        0        0      441 2024-04-14 16:11:23.468322 pyguiadapter-0.3.4/pyguiadapter/res/icons/code.svg
--rw-r--r--   0        0        0      831 2024-04-14 16:11:23.469322 pyguiadapter-0.3.4/pyguiadapter/res/icons/collect-computer.svg
--rw-r--r--   0        0        0      732 2024-04-14 16:11:23.469322 pyguiadapter-0.3.4/pyguiadapter/res/icons/collect-laptop.svg
--rw-r--r--   0        0        0     1181 2024-04-14 16:11:23.469322 pyguiadapter-0.3.4/pyguiadapter/res/icons/collect-picture.svg
--rw-r--r--   0        0        0     1118 2024-04-14 16:11:23.469322 pyguiadapter-0.3.4/pyguiadapter/res/icons/color-card.svg
--rw-r--r--   0        0        0     1289 2024-04-14 16:11:23.469322 pyguiadapter-0.3.4/pyguiadapter/res/icons/command.svg
--rw-r--r--   0        0        0      371 2024-04-14 16:11:23.469322 pyguiadapter-0.3.4/pyguiadapter/res/icons/comment-one.svg
--rw-r--r--   0        0        0      581 2024-04-14 16:11:23.469322 pyguiadapter-0.3.4/pyguiadapter/res/icons/comment.svg
--rw-r--r--   0        0        0      553 2024-04-14 16:11:23.470322 pyguiadapter-0.3.4/pyguiadapter/res/icons/comments.svg
--rw-r--r--   0        0        0      628 2024-04-14 16:11:23.470322 pyguiadapter-0.3.4/pyguiadapter/res/icons/communication.svg
--rw-r--r--   0        0        0      753 2024-04-14 16:11:23.470322 pyguiadapter-0.3.4/pyguiadapter/res/icons/compass.svg
--rw-r--r--   0        0        0     1110 2024-04-14 16:11:23.470322 pyguiadapter-0.3.4/pyguiadapter/res/icons/compression.svg
--rw-r--r--   0        0        0      556 2024-04-14 16:11:23.470322 pyguiadapter-0.3.4/pyguiadapter/res/icons/computer.svg
--rw-r--r--   0        0        0      447 2024-04-14 16:11:23.470322 pyguiadapter-0.3.4/pyguiadapter/res/icons/cones.svg
--rw-r--r--   0        0        0     1850 2024-04-14 16:11:23.470322 pyguiadapter-0.3.4/pyguiadapter/res/icons/connect.svg
--rw-r--r--   0        0        0      620 2024-04-14 16:11:23.470322 pyguiadapter-0.3.4/pyguiadapter/res/icons/copy-one.svg
--rw-r--r--   0        0        0      524 2024-04-14 16:11:23.470322 pyguiadapter-0.3.4/pyguiadapter/res/icons/copyright.svg
--rw-r--r--   0        0        0     2644 2024-04-14 16:11:23.471322 pyguiadapter-0.3.4/pyguiadapter/res/icons/cpu.svg
--rw-r--r--   0        0        0      516 2024-04-14 16:11:23.471322 pyguiadapter-0.3.4/pyguiadapter/res/icons/cross-ring-two.svg
--rw-r--r--   0        0        0      895 2024-04-14 16:11:23.471322 pyguiadapter-0.3.4/pyguiadapter/res/icons/cube-four.svg
--rw-r--r--   0        0        0      369 2024-04-14 16:11:23.471322 pyguiadapter-0.3.4/pyguiadapter/res/icons/curve-adjustment.svg
--rw-r--r--   0        0        0     1177 2024-04-14 16:11:23.471322 pyguiadapter-0.3.4/pyguiadapter/res/icons/cuvette.svg
--rw-r--r--   0        0        0     1199 2024-04-14 16:11:23.472322 pyguiadapter-0.3.4/pyguiadapter/res/icons/dashboard-one.svg
--rw-r--r--   0        0        0     1332 2024-04-14 16:11:23.472322 pyguiadapter-0.3.4/pyguiadapter/res/icons/dashboard-two.svg
--rw-r--r--   0        0        0     1221 2024-04-14 16:11:23.472322 pyguiadapter-0.3.4/pyguiadapter/res/icons/data-all.svg
--rw-r--r--   0        0        0     1239 2024-04-14 16:11:23.472322 pyguiadapter-0.3.4/pyguiadapter/res/icons/data-display.svg
--rw-r--r--   0        0        0     1255 2024-04-14 16:11:23.472322 pyguiadapter-0.3.4/pyguiadapter/res/icons/data-lock.svg
--rw-r--r--   0        0        0      829 2024-04-14 16:11:23.472322 pyguiadapter-0.3.4/pyguiadapter/res/icons/data-screen.svg
--rw-r--r--   0        0        0      833 2024-04-14 16:11:23.472322 pyguiadapter-0.3.4/pyguiadapter/res/icons/data-server.svg
--rw-r--r--   0        0        0     1448 2024-04-14 16:11:23.472322 pyguiadapter-0.3.4/pyguiadapter/res/icons/data-switching.svg
--rw-r--r--   0        0        0     1209 2024-04-14 16:11:23.473322 pyguiadapter-0.3.4/pyguiadapter/res/icons/data-user.svg
--rw-r--r--   0        0        0      794 2024-04-14 16:11:23.473322 pyguiadapter-0.3.4/pyguiadapter/res/icons/data.svg
--rw-r--r--   0        0        0     1588 2024-04-14 16:11:23.473322 pyguiadapter-0.3.4/pyguiadapter/res/icons/database-alert.svg
--rw-r--r--   0        0        0     1606 2024-04-14 16:11:23.473322 pyguiadapter-0.3.4/pyguiadapter/res/icons/database-code.svg
--rw-r--r--   0        0        0     1596 2024-04-14 16:11:23.473322 pyguiadapter-0.3.4/pyguiadapter/res/icons/database-config.svg
--rw-r--r--   0        0        0     1513 2024-04-14 16:11:23.473322 pyguiadapter-0.3.4/pyguiadapter/res/icons/database-download.svg
--rw-r--r--   0        0        0     1516 2024-04-14 16:11:23.473322 pyguiadapter-0.3.4/pyguiadapter/res/icons/database-enter.svg
--rw-r--r--   0        0        0     1528 2024-04-14 16:11:23.473322 pyguiadapter-0.3.4/pyguiadapter/res/icons/database-fail.svg
--rw-r--r--   0        0        0     1513 2024-04-14 16:11:23.474322 pyguiadapter-0.3.4/pyguiadapter/res/icons/database-first.svg
--rw-r--r--   0        0        0     1492 2024-04-14 16:11:23.474322 pyguiadapter-0.3.4/pyguiadapter/res/icons/database-forbid.svg
--rw-r--r--   0        0        0     1738 2024-04-14 16:11:23.474322 pyguiadapter-0.3.4/pyguiadapter/res/icons/database-lock.svg
--rw-r--r--   0        0        0     1195 2024-04-14 16:11:23.474322 pyguiadapter-0.3.4/pyguiadapter/res/icons/database-network-point.svg
--rw-r--r--   0        0        0     1770 2024-04-14 16:11:23.474322 pyguiadapter-0.3.4/pyguiadapter/res/icons/database-network.svg
--rw-r--r--   0        0        0     1637 2024-04-14 16:11:23.474322 pyguiadapter-0.3.4/pyguiadapter/res/icons/database-point.svg
--rw-r--r--   0        0        0     1390 2024-04-14 16:11:23.474322 pyguiadapter-0.3.4/pyguiadapter/res/icons/database-position.svg
--rw-r--r--   0        0        0     1504 2024-04-14 16:11:23.475322 pyguiadapter-0.3.4/pyguiadapter/res/icons/database-power.svg
--rw-r--r--   0        0        0     1528 2024-04-14 16:11:23.475322 pyguiadapter-0.3.4/pyguiadapter/res/icons/database-proportion.svg
--rw-r--r--   0        0        0     1908 2024-04-14 16:11:23.475322 pyguiadapter-0.3.4/pyguiadapter/res/icons/database-search.svg
--rw-r--r--   0        0        0     1542 2024-04-14 16:11:23.475322 pyguiadapter-0.3.4/pyguiadapter/res/icons/database-setting.svg
--rw-r--r--   0        0        0     1504 2024-04-14 16:11:23.475322 pyguiadapter-0.3.4/pyguiadapter/res/icons/database-success.svg
--rw-r--r--   0        0        0     1638 2024-04-14 16:11:23.475322 pyguiadapter-0.3.4/pyguiadapter/res/icons/database-sync.svg
--rw-r--r--   0        0        0     1492 2024-04-14 16:11:23.475322 pyguiadapter-0.3.4/pyguiadapter/res/icons/database-time.svg
--rw-r--r--   0        0        0      762 2024-04-14 16:11:23.475322 pyguiadapter-0.3.4/pyguiadapter/res/icons/date-comes-back.svg
--rw-r--r--   0        0        0      470 2024-04-14 16:11:23.476322 pyguiadapter-0.3.4/pyguiadapter/res/icons/diamond-one.svg
--rw-r--r--   0        0        0      470 2024-04-14 16:11:23.476322 pyguiadapter-0.3.4/pyguiadapter/res/icons/diamond-three.svg
--rw-r--r--   0        0        0      466 2024-04-14 16:11:23.476322 pyguiadapter-0.3.4/pyguiadapter/res/icons/diamond-two.svg
--rw-r--r--   0        0        0      855 2024-04-14 16:11:23.476322 pyguiadapter-0.3.4/pyguiadapter/res/icons/disk-one.svg
--rw-r--r--   0        0        0      533 2024-04-14 16:11:23.476322 pyguiadapter-0.3.4/pyguiadapter/res/icons/disk-two.svg
--rw-r--r--   0        0        0      599 2024-04-14 16:11:23.476322 pyguiadapter-0.3.4/pyguiadapter/res/icons/disk.svg
--rw-r--r--   0        0        0      646 2024-04-14 16:11:23.476322 pyguiadapter-0.3.4/pyguiadapter/res/icons/document-folder.svg
--rw-r--r--   0        0        0      957 2024-04-14 16:11:23.476322 pyguiadapter-0.3.4/pyguiadapter/res/icons/download-one.svg
--rw-r--r--   0        0        0      649 2024-04-14 16:11:23.477322 pyguiadapter-0.3.4/pyguiadapter/res/icons/download-three.svg
--rw-r--r--   0        0        0      730 2024-04-14 16:11:23.477322 pyguiadapter-0.3.4/pyguiadapter/res/icons/download-two.svg
--rw-r--r--   0        0        0      827 2024-04-14 16:11:23.477322 pyguiadapter-0.3.4/pyguiadapter/res/icons/download-web.svg
--rw-r--r--   0        0        0      500 2024-04-14 16:11:23.477322 pyguiadapter-0.3.4/pyguiadapter/res/icons/electrocardiogram.svg
--rw-r--r--   0        0        0      568 2024-04-14 16:11:23.477322 pyguiadapter-0.3.4/pyguiadapter/res/icons/email-down.svg
--rw-r--r--   0        0        0      567 2024-04-14 16:11:23.477322 pyguiadapter-0.3.4/pyguiadapter/res/icons/email-push.svg
--rw-r--r--   0        0        0      634 2024-04-14 16:11:23.477322 pyguiadapter-0.3.4/pyguiadapter/res/icons/experiment-one.svg
--rw-r--r--   0        0        0      731 2024-04-14 16:11:23.477322 pyguiadapter-0.3.4/pyguiadapter/res/icons/experiment.svg
--rw-r--r--   0        0        0      680 2024-04-14 16:11:23.478322 pyguiadapter-0.3.4/pyguiadapter/res/icons/figma-component.svg
--rw-r--r--   0        0        0      652 2024-04-14 16:11:23.478322 pyguiadapter-0.3.4/pyguiadapter/res/icons/file-addition.svg
--rw-r--r--   0        0        0      664 2024-04-14 16:11:23.478322 pyguiadapter-0.3.4/pyguiadapter/res/icons/file-code.svg
--rw-r--r--   0        0        0      856 2024-04-14 16:11:23.478322 pyguiadapter-0.3.4/pyguiadapter/res/icons/file-conversion.svg
--rw-r--r--   0        0        0      772 2024-04-14 16:11:23.478322 pyguiadapter-0.3.4/pyguiadapter/res/icons/file-display.svg
--rw-r--r--   0        0        0     1316 2024-04-14 16:11:23.478322 pyguiadapter-0.3.4/pyguiadapter/res/icons/file-pdf-one.svg
--rw-r--r--   0        0        0     1381 2024-04-14 16:11:23.478322 pyguiadapter-0.3.4/pyguiadapter/res/icons/file-ppt.svg
--rw-r--r--   0        0        0      658 2024-04-14 16:11:23.478322 pyguiadapter-0.3.4/pyguiadapter/res/icons/file-protection.svg
--rw-r--r--   0        0        0      652 2024-04-14 16:11:23.479322 pyguiadapter-0.3.4/pyguiadapter/res/icons/file-text.svg
--rw-r--r--   0        0        0      468 2024-04-14 16:11:23.479322 pyguiadapter-0.3.4/pyguiadapter/res/icons/file-word.svg
--rw-r--r--   0        0        0      931 2024-04-14 16:11:23.479322 pyguiadapter-0.3.4/pyguiadapter/res/icons/film.svg
--rw-r--r--   0        0        0      734 2024-04-14 16:11:23.479322 pyguiadapter-0.3.4/pyguiadapter/res/icons/flask.svg
--rw-r--r--   0        0        0      455 2024-04-14 16:11:23.479322 pyguiadapter-0.3.4/pyguiadapter/res/icons/folder-open.svg
--rw-r--r--   0        0        0      851 2024-04-14 16:11:23.479322 pyguiadapter-0.3.4/pyguiadapter/res/icons/game-handle.svg
--rw-r--r--   0        0        0      989 2024-04-14 16:11:23.479322 pyguiadapter-0.3.4/pyguiadapter/res/icons/help.svg
--rw-r--r--   0        0        0      545 2024-04-14 16:11:23.480322 pyguiadapter-0.3.4/pyguiadapter/res/icons/hexagon-one.svg
--rw-r--r--   0        0        0      794 2024-04-14 16:11:23.480322 pyguiadapter-0.3.4/pyguiadapter/res/icons/id-card-h.svg
--rw-r--r--   0        0        0      935 2024-04-14 16:11:23.480322 pyguiadapter-0.3.4/pyguiadapter/res/icons/info.svg
--rw-r--r--   0        0        0      696 2024-04-14 16:11:23.480322 pyguiadapter-0.3.4/pyguiadapter/res/icons/install.svg
--rw-r--r--   0        0        0    11553 2024-04-14 16:11:23.462322 pyguiadapter-0.3.4/pyguiadapter/res/icons/LICENSE
--rw-r--r--   0        0        0      683 2024-04-14 16:11:23.480322 pyguiadapter-0.3.4/pyguiadapter/res/icons/many-to-many.svg
--rw-r--r--   0        0        0      602 2024-04-14 16:11:23.480322 pyguiadapter-0.3.4/pyguiadapter/res/icons/message-emoji.svg
--rw-r--r--   0        0        0      522 2024-04-14 16:11:23.481322 pyguiadapter-0.3.4/pyguiadapter/res/icons/message-one.svg
--rw-r--r--   0        0        0      763 2024-04-14 16:11:23.481322 pyguiadapter-0.3.4/pyguiadapter/res/icons/message-privacy.svg
--rw-r--r--   0        0        0      648 2024-04-14 16:11:23.481322 pyguiadapter-0.3.4/pyguiadapter/res/icons/message-search.svg
--rw-r--r--   0        0        0      679 2024-04-14 16:11:23.481322 pyguiadapter-0.3.4/pyguiadapter/res/icons/message-security.svg
--rw-r--r--   0        0        0      485 2024-04-14 16:11:23.481322 pyguiadapter-0.3.4/pyguiadapter/res/icons/message-sent.svg
--rw-r--r--   0        0        0      577 2024-04-14 16:11:23.481322 pyguiadapter-0.3.4/pyguiadapter/res/icons/message-success.svg
--rw-r--r--   0        0        0      550 2024-04-14 16:11:23.481322 pyguiadapter-0.3.4/pyguiadapter/res/icons/message-unread.svg
--rw-r--r--   0        0        0      738 2024-04-14 16:11:23.481322 pyguiadapter-0.3.4/pyguiadapter/res/icons/message.svg
--rw-r--r--   0        0        0      537 2024-04-14 16:11:23.482322 pyguiadapter-0.3.4/pyguiadapter/res/icons/mini-sd-card.svg
--rw-r--r--   0        0        0      521 2024-04-14 16:11:23.482322 pyguiadapter-0.3.4/pyguiadapter/res/icons/monitor.svg
--rw-r--r--   0        0        0     1053 2024-04-14 16:11:23.482322 pyguiadapter-0.3.4/pyguiadapter/res/icons/more-app.svg
--rw-r--r--   0        0        0      971 2024-04-14 16:11:23.482322 pyguiadapter-0.3.4/pyguiadapter/res/icons/movie-board.svg
--rw-r--r--   0        0        0     1213 2024-04-14 16:11:23.482322 pyguiadapter-0.3.4/pyguiadapter/res/icons/movie.svg
--rw-r--r--   0        0        0      995 2024-04-14 16:11:23.482322 pyguiadapter-0.3.4/pyguiadapter/res/icons/multi-function-knife.svg
--rw-r--r--   0        0        0      835 2024-04-14 16:11:23.482322 pyguiadapter-0.3.4/pyguiadapter/res/icons/notebook-one.svg
--rw-r--r--   0        0        0      626 2024-04-14 16:11:23.482322 pyguiadapter-0.3.4/pyguiadapter/res/icons/octagon.svg
--rw-r--r--   0        0        0      575 2024-04-14 16:11:23.483322 pyguiadapter-0.3.4/pyguiadapter/res/icons/online-meeting.svg
--rw-r--r--   0        0        0      227 2024-04-14 16:11:23.483322 pyguiadapter-0.3.4/pyguiadapter/res/icons/oval-one.svg
--rw-r--r--   0        0        0      537 2024-04-14 16:11:23.483322 pyguiadapter-0.3.4/pyguiadapter/res/icons/page-template.svg
--rw-r--r--   0        0        0      440 2024-04-14 16:11:23.483322 pyguiadapter-0.3.4/pyguiadapter/res/icons/page.svg
--rw-r--r--   0        0        0      412 2024-04-14 16:11:23.483322 pyguiadapter-0.3.4/pyguiadapter/res/icons/parallelogram.svg
--rw-r--r--   0        0        0      633 2024-04-14 16:11:23.483322 pyguiadapter-0.3.4/pyguiadapter/res/icons/pay-code.svg
--rw-r--r--   0        0        0      509 2024-04-14 16:11:23.483322 pyguiadapter-0.3.4/pyguiadapter/res/icons/pentagon-one.svg
--rw-r--r--   0        0        0      980 2024-04-14 16:11:23.483322 pyguiadapter-0.3.4/pyguiadapter/res/icons/people-plus-one.svg
--rw-r--r--   0        0        0     1040 2024-04-14 16:11:23.484322 pyguiadapter-0.3.4/pyguiadapter/res/icons/phone-incoming-one.svg
--rw-r--r--   0        0        0     1029 2024-04-14 16:11:23.484322 pyguiadapter-0.3.4/pyguiadapter/res/icons/phone-incoming.svg
--rw-r--r--   0        0        0     1083 2024-04-14 16:11:23.484322 pyguiadapter-0.3.4/pyguiadapter/res/icons/phone-missed.svg
--rw-r--r--   0        0        0     1015 2024-04-14 16:11:23.484322 pyguiadapter-0.3.4/pyguiadapter/res/icons/phone-outgoing-one.svg
--rw-r--r--   0        0        0     1008 2024-04-14 16:11:23.484322 pyguiadapter-0.3.4/pyguiadapter/res/icons/phone-outgoing.svg
--rw-r--r--   0        0        0      811 2024-04-14 16:11:23.484322 pyguiadapter-0.3.4/pyguiadapter/res/icons/phone-telephone.svg
--rw-r--r--   0        0        0      935 2024-04-14 16:11:23.484322 pyguiadapter-0.3.4/pyguiadapter/res/icons/phone-video-call.svg
--rw-r--r--   0        0        0      974 2024-04-14 16:11:23.484322 pyguiadapter-0.3.4/pyguiadapter/res/icons/platte.svg
--rw-r--r--   0        0        0      473 2024-04-14 16:11:23.485322 pyguiadapter-0.3.4/pyguiadapter/res/icons/play.svg
--rw-r--r--   0        0        0      434 2024-04-14 16:11:23.485322 pyguiadapter-0.3.4/pyguiadapter/res/icons/powerpoint.svg
--rw-r--r--   0        0        0      612 2024-04-14 16:11:23.485322 pyguiadapter-0.3.4/pyguiadapter/res/icons/ppt.svg
--rw-r--r--   0        0        0      427 2024-04-14 16:11:23.485322 pyguiadapter-0.3.4/pyguiadapter/res/icons/puzzle.svg
--rw-r--r--   0        0        0      364 2024-04-14 16:11:23.485322 pyguiadapter-0.3.4/pyguiadapter/res/icons/quadrilateral.svg
--rw-r--r--   0        0        0      783 2024-04-14 16:11:23.485322 pyguiadapter-0.3.4/pyguiadapter/res/icons/record-disc.svg
--rw-r--r--   0        0        0      880 2024-04-14 16:11:23.486322 pyguiadapter-0.3.4/pyguiadapter/res/icons/record.svg
--rw-r--r--   0        0        0      319 2024-04-14 16:11:23.486322 pyguiadapter-0.3.4/pyguiadapter/res/icons/rectangle-one.svg
--rw-r--r--   0        0        0      328 2024-04-14 16:11:23.486322 pyguiadapter-0.3.4/pyguiadapter/res/icons/rectangle-small.svg
--rw-r--r--   0        0        0      319 2024-04-14 16:11:23.486322 pyguiadapter-0.3.4/pyguiadapter/res/icons/rectangle.svg
--rw-r--r--   0        0        0      591 2024-04-14 16:11:23.486322 pyguiadapter-0.3.4/pyguiadapter/res/icons/rename.py
--rw-r--r--   0        0        0      425 2024-04-14 16:11:23.486322 pyguiadapter-0.3.4/pyguiadapter/res/icons/right-angle.svg
--rw-r--r--   0        0        0      217 2024-04-14 16:11:23.486322 pyguiadapter-0.3.4/pyguiadapter/res/icons/round.svg
--rw-r--r--   0        0        0      901 2024-04-14 16:11:23.487322 pyguiadapter-0.3.4/pyguiadapter/res/icons/rule-two.svg
--rw-r--r--   0        0        0      794 2024-04-14 16:11:23.487322 pyguiadapter-0.3.4/pyguiadapter/res/icons/ruler-one.svg
--rw-r--r--   0        0        0      926 2024-04-14 16:11:23.487322 pyguiadapter-0.3.4/pyguiadapter/res/icons/ruler.svg
--rw-r--r--   0        0        0      583 2024-04-14 16:11:23.487322 pyguiadapter-0.3.4/pyguiadapter/res/icons/sd-card.svg
--rw-r--r--   0        0        0     1259 2024-04-14 16:11:23.487322 pyguiadapter-0.3.4/pyguiadapter/res/icons/setting-computer.svg
--rw-r--r--   0        0        0     1148 2024-04-14 16:11:23.487322 pyguiadapter-0.3.4/pyguiadapter/res/icons/setting-laptop.svg
--rw-r--r--   0        0        0     1443 2024-04-14 16:11:23.487322 pyguiadapter-0.3.4/pyguiadapter/res/icons/setting-two.svg
--rw-r--r--   0        0        0      980 2024-04-14 16:11:23.487322 pyguiadapter-0.3.4/pyguiadapter/res/icons/share-one.svg
--rw-r--r--   0        0        0      328 2024-04-14 16:11:23.487322 pyguiadapter-0.3.4/pyguiadapter/res/icons/square-small.svg
--rw-r--r--   0        0        0      317 2024-04-14 16:11:23.488322 pyguiadapter-0.3.4/pyguiadapter/res/icons/square.svg
--rw-r--r--   0        0        0      954 2024-04-14 16:11:23.488322 pyguiadapter-0.3.4/pyguiadapter/res/icons/system.svg
--rw-r--r--   0        0        0      895 2024-04-14 16:11:23.488322 pyguiadapter-0.3.4/pyguiadapter/res/icons/table-file.svg
--rw-r--r--   0        0        0     1216 2024-04-14 16:11:23.488322 pyguiadapter-0.3.4/pyguiadapter/res/icons/tape.svg
--rw-r--r--   0        0        0      465 2024-04-14 16:11:23.488322 pyguiadapter-0.3.4/pyguiadapter/res/icons/terminal.svg
--rw-r--r--   0        0        0      751 2024-04-14 16:11:23.488322 pyguiadapter-0.3.4/pyguiadapter/res/icons/test-tube.svg
--rw-r--r--   0        0        0      724 2024-04-14 16:11:23.488322 pyguiadapter-0.3.4/pyguiadapter/res/icons/thermometer.svg
--rw-r--r--   0        0        0      425 2024-04-14 16:11:23.488322 pyguiadapter-0.3.4/pyguiadapter/res/icons/tips-one.svg
--rw-r--r--   0        0        0      510 2024-04-14 16:11:23.489322 pyguiadapter-0.3.4/pyguiadapter/res/icons/tool.svg
--rw-r--r--   0        0        0      587 2024-04-14 16:11:23.489322 pyguiadapter-0.3.4/pyguiadapter/res/icons/topic-discussion.svg
--rw-r--r--   0        0        0     1027 2024-04-14 16:11:23.489322 pyguiadapter-0.3.4/pyguiadapter/res/icons/topic.svg
--rw-r--r--   0        0        0      413 2024-04-14 16:11:23.489322 pyguiadapter-0.3.4/pyguiadapter/res/icons/trapezoid.svg
--rw-r--r--   0        0        0      831 2024-04-14 16:11:23.489322 pyguiadapter-0.3.4/pyguiadapter/res/icons/tree-list.svg
--rw-r--r--   0        0        0     1970 2024-04-14 16:11:23.489322 pyguiadapter-0.3.4/pyguiadapter/res/icons/triangle-ruler.svg
--rw-r--r--   0        0        0      468 2024-04-14 16:11:23.489322 pyguiadapter-0.3.4/pyguiadapter/res/icons/triangle.svg
--rw-r--r--   0        0        0      717 2024-04-14 16:11:23.489322 pyguiadapter-0.3.4/pyguiadapter/res/icons/vial.svg
--rw-r--r--   0        0        0     1823 2024-04-14 16:11:23.490322 pyguiadapter-0.3.4/pyguiadapter/res/icons/video.svg
--rw-r--r--   0        0        0      706 2024-04-14 16:11:23.490322 pyguiadapter-0.3.4/pyguiadapter/res/icons/view-grid-card.svg
--rw-r--r--   0        0        0      775 2024-04-14 16:11:23.490322 pyguiadapter-0.3.4/pyguiadapter/res/icons/view-grid-detail.svg
--rw-r--r--   0        0        0      887 2024-04-14 16:11:23.490322 pyguiadapter-0.3.4/pyguiadapter/res/icons/view-grid-list.svg
--rw-r--r--   0        0        0      642 2024-04-14 16:11:23.490322 pyguiadapter-0.3.4/pyguiadapter/res/icons/voice-input.svg
--rw-r--r--   0        0        0      903 2024-04-14 16:11:23.490322 pyguiadapter-0.3.4/pyguiadapter/res/icons/voice-message.svg
--rw-r--r--   0        0        0      685 2024-04-14 16:11:23.490322 pyguiadapter-0.3.4/pyguiadapter/res/icons/voice-one.svg
--rw-r--r--   0        0        0      508 2024-04-14 16:11:23.490322 pyguiadapter-0.3.4/pyguiadapter/res/icons/voice.svg
--rw-r--r--   0        0        0     1173 2024-04-14 16:11:23.490322 pyguiadapter-0.3.4/pyguiadapter/res/icons/weixin-mini-app.svg
--rw-r--r--   0        0        0      809 2024-04-14 16:11:23.491322 pyguiadapter-0.3.4/pyguiadapter/res/icons/wifi.svg
--rw-r--r--   0        0        0      976 2024-04-14 16:11:23.491322 pyguiadapter-0.3.4/pyguiadapter/res/icons/zip.svg
--rw-r--r--   0        0        0        0 2024-04-20 07:19:02.882935 pyguiadapter-0.3.4/pyguiadapter/tools/__init__.py
--rw-r--r--   0        0        0       99 2024-04-20 07:19:02.882935 pyguiadapter-0.3.4/pyguiadapter/tools/easyconfigs/__init__.py
--rw-r--r--   0        0        0      738 2024-04-20 07:19:02.882935 pyguiadapter-0.3.4/pyguiadapter/tools/easyconfigs/constants.py
--rw-r--r--   0        0        0      179 2024-04-20 07:19:02.883935 pyguiadapter-0.3.4/pyguiadapter/tools/easyconfigs/helper/__init__.py
--rw-r--r--   0        0        0     6540 2024-04-20 07:19:02.883935 pyguiadapter-0.3.4/pyguiadapter/tools/easyconfigs/helper/const_name_value.py
--rw-r--r--   0        0        0     3282 2024-04-20 07:19:02.883935 pyguiadapter-0.3.4/pyguiadapter/tools/easyconfigs/helper/imports.py
--rw-r--r--   0        0        0     3114 2024-04-20 07:19:02.883935 pyguiadapter-0.3.4/pyguiadapter/tools/easyconfigs/helper/parameter_constants.py
--rw-r--r--   0        0        0     2510 2024-04-20 07:19:02.884935 pyguiadapter-0.3.4/pyguiadapter/tools/easyconfigs/helper/parameter_widget_configs.py
--rw-r--r--   0        0        0     9041 2024-04-20 07:19:02.884935 pyguiadapter-0.3.4/pyguiadapter/tools/easyconfigs/impl.py
--rw-r--r--   0        0        0     1076 2024-04-20 07:19:02.884935 pyguiadapter-0.3.4/pyguiadapter/tools/easyconfigs/structures.py
--rw-r--r--   0        0        0      882 2024-04-20 07:19:02.884935 pyguiadapter-0.3.4/pyguiadapter/tools/easyconfigs/tpl/configs.tpl
--rw-r--r--   0        0        0      500 2024-04-20 07:19:02.884935 pyguiadapter-0.3.4/pyguiadapter/tools/easyconfigs/tpl/constants.tpl
--rw-r--r--   0        0        0      762 2024-04-20 07:19:02.885935 pyguiadapter-0.3.4/pyguiadapter/tools/easyconfigs/utils.py
--rw-r--r--   0        0        0      358 2024-04-17 16:40:54.565013 pyguiadapter-0.3.4/pyguiadapter/ui/__init__.py
--rw-r--r--   0        0        0     1513 2024-04-14 16:11:23.491322 pyguiadapter-0.3.4/pyguiadapter/ui/config.py
--rw-r--r--   0        0        0        0 2024-04-14 16:11:23.491322 pyguiadapter-0.3.4/pyguiadapter/ui/generated/__init__.py
--rw-r--r--   0        0        0     2792 2024-04-16 16:25:55.273398 pyguiadapter-0.3.4/pyguiadapter/ui/generated/ui_class_init_window.py
--rw-r--r--   0        0        0     7696 2024-04-16 16:25:55.346941 pyguiadapter-0.3.4/pyguiadapter/ui/generated/ui_execution_window.py
--rw-r--r--   0        0        0     3700 2024-04-16 16:25:55.416780 pyguiadapter-0.3.4/pyguiadapter/ui/generated/ui_selection_window.py
--rw-r--r--   0        0        0     1418 2024-04-17 16:04:29.140320 pyguiadapter-0.3.4/pyguiadapter/ui/menus.py
--rw-r--r--   0        0        0     1457 2024-04-14 16:11:23.492322 pyguiadapter-0.3.4/pyguiadapter/ui/styles.py
--rw-r--r--   0        0        0     3874 2024-04-17 16:07:29.237029 pyguiadapter-0.3.4/pyguiadapter/ui/utils.py
--rw-r--r--   0        0        0        0 2024-04-17 16:23:22.163246 pyguiadapter-0.3.4/pyguiadapter/ui/window/__init__.py
--rw-r--r--   0        0        0       78 2024-04-14 16:11:23.493322 pyguiadapter-0.3.4/pyguiadapter/ui/window/class_init/__init__.py
--rw-r--r--   0        0        0      260 2024-04-17 16:16:41.343493 pyguiadapter-0.3.4/pyguiadapter/ui/window/class_init/config.py
--rw-r--r--   0        0        0      160 2024-04-14 16:11:23.493322 pyguiadapter-0.3.4/pyguiadapter/ui/window/class_init/constants.py
--rw-r--r--   0        0        0     5367 2024-04-17 16:16:05.127955 pyguiadapter-0.3.4/pyguiadapter/ui/window/class_init/impl.py
--rw-r--r--   0        0        0       78 2024-04-14 16:11:23.493322 pyguiadapter-0.3.4/pyguiadapter/ui/window/func_execution/__init__.py
--rw-r--r--   0        0        0     5243 2024-04-17 16:10:52.573365 pyguiadapter-0.3.4/pyguiadapter/ui/window/func_execution/base.py
--rw-r--r--   0        0        0     2713 2024-04-17 16:17:12.915519 pyguiadapter-0.3.4/pyguiadapter/ui/window/func_execution/config.py
--rw-r--r--   0        0        0      674 2024-04-20 13:29:28.867557 pyguiadapter-0.3.4/pyguiadapter/ui/window/func_execution/constants.py
--rw-r--r--   0        0        0     4121 2024-04-14 16:11:23.494322 pyguiadapter-0.3.4/pyguiadapter/ui/window/func_execution/context.py
--rw-r--r--   0        0        0      288 2024-04-14 16:11:23.494322 pyguiadapter-0.3.4/pyguiadapter/ui/window/func_execution/exceptions.py
--rw-r--r--   0        0        0    18652 2024-04-29 10:58:08.523913 pyguiadapter-0.3.4/pyguiadapter/ui/window/func_execution/impl.py
--rw-r--r--   0        0        0       78 2024-04-14 16:11:23.494322 pyguiadapter-0.3.4/pyguiadapter/ui/window/func_selection/__init__.py
--rw-r--r--   0        0        0      830 2024-04-14 16:11:23.495322 pyguiadapter-0.3.4/pyguiadapter/ui/window/func_selection/config.py
--rw-r--r--   0        0        0      305 2024-04-14 16:11:23.495322 pyguiadapter-0.3.4/pyguiadapter/ui/window/func_selection/constants.py
--rw-r--r--   0        0        0     7509 2024-04-17 16:30:44.468256 pyguiadapter-0.3.4/pyguiadapter/ui/window/func_selection/impl.py
--rw-r--r--   0        0        0      702 2024-04-29 12:29:04.361757 pyguiadapter-0.3.4/pyproject.toml
--rw-r--r--   0        0        0     8722 2024-04-14 16:11:23.455323 pyguiadapter-0.3.4/README.md
--rw-r--r--   0        0        0     9251 1970-01-01 00:00:00.000000 pyguiadapter-0.3.4/PKG-INFO
+-rw-r--r--   0        0        0    35821 2024-04-14 16:11:23.455323 pyguiadapter-0.3.5/License
+-rw-r--r--   0        0        0      108 2024-04-17 16:38:11.248187 pyguiadapter-0.3.5/pyguiadapter/__init__.py
+-rw-r--r--   0        0        0      139 2024-04-17 15:57:53.099012 pyguiadapter-0.3.5/pyguiadapter/adapter/__init__.py
+-rw-r--r--   0        0        0    10113 2024-04-29 13:33:37.531700 pyguiadapter-0.3.5/pyguiadapter/adapter/adapter.py
+-rw-r--r--   0        0        0     5463 2024-04-29 10:52:58.130370 pyguiadapter-0.3.5/pyguiadapter/adapter/bundle.py
+-rw-r--r--   0        0        0      226 2024-04-29 13:33:04.775629 pyguiadapter-0.3.5/pyguiadapter/adapter/constants.py
+-rw-r--r--   0        0        0     1684 2024-04-17 15:48:37.357738 pyguiadapter-0.3.5/pyguiadapter/adapter/executor.py
+-rw-r--r--   0        0        0     1593 2024-04-17 15:52:24.455478 pyguiadapter-0.3.5/pyguiadapter/commons.py
+-rw-r--r--   0        0        0      199 2024-04-14 16:11:23.461322 pyguiadapter-0.3.5/pyguiadapter/exceptions.py
+-rw-r--r--   0        0        0        0 2024-04-14 16:11:23.461322 pyguiadapter-0.3.5/pyguiadapter/interact/__init__.py
+-rw-r--r--   0        0        0     5119 2024-04-17 16:06:29.919169 pyguiadapter-0.3.5/pyguiadapter/interact/ulogging.py
+-rw-r--r--   0        0        0    12531 2024-04-14 16:11:23.461322 pyguiadapter-0.3.5/pyguiadapter/interact/upopup.py
+-rw-r--r--   0        0        0     1074 2024-04-20 13:02:56.774164 pyguiadapter-0.3.5/pyguiadapter/interact/uprint.py
+-rw-r--r--   0        0        0      753 2024-04-14 16:11:23.462322 pyguiadapter-0.3.5/pyguiadapter/res/icons/abnormal.svg
+-rw-r--r--   0        0        0      563 2024-04-14 16:11:23.462322 pyguiadapter-0.3.5/pyguiadapter/res/icons/acoustic.svg
+-rw-r--r--   0        0        0      437 2024-04-14 16:11:23.462322 pyguiadapter-0.3.5/pyguiadapter/res/icons/activity-source.svg
+-rw-r--r--   0        0        0      721 2024-04-14 16:11:23.462322 pyguiadapter-0.3.5/pyguiadapter/res/icons/add-computer.svg
+-rw-r--r--   0        0        0     1074 2024-04-14 16:11:23.463322 pyguiadapter-0.3.5/pyguiadapter/res/icons/add-picture.svg
+-rw-r--r--   0        0        0      556 2024-04-14 16:11:23.463322 pyguiadapter-0.3.5/pyguiadapter/res/icons/add-print.svg
+-rw-r--r--   0        0        0      611 2024-04-14 16:11:23.463322 pyguiadapter-0.3.5/pyguiadapter/res/icons/add-user.svg
+-rw-r--r--   0        0        0      820 2024-04-14 16:11:23.463322 pyguiadapter-0.3.5/pyguiadapter/res/icons/add-web.svg
+-rw-r--r--   0        0        0      444 2024-04-14 16:11:23.463322 pyguiadapter-0.3.5/pyguiadapter/res/icons/airplay.svg
+-rw-r--r--   0        0        0      744 2024-04-14 16:11:23.463322 pyguiadapter-0.3.5/pyguiadapter/res/icons/api-app.svg
+-rw-r--r--   0        0        0      915 2024-04-14 16:11:23.463322 pyguiadapter-0.3.5/pyguiadapter/res/icons/application-effect.svg
+-rw-r--r--   0        0        0      513 2024-04-14 16:11:23.464322 pyguiadapter-0.3.5/pyguiadapter/res/icons/application-one.svg
+-rw-r--r--   0        0        0      471 2024-04-14 16:11:23.464322 pyguiadapter-0.3.5/pyguiadapter/res/icons/application-two.svg
+-rw-r--r--   0        0        0      444 2024-04-14 16:11:23.464322 pyguiadapter-0.3.5/pyguiadapter/res/icons/area-map.svg
+-rw-r--r--   0        0        0     1704 2024-04-14 16:11:23.464322 pyguiadapter-0.3.5/pyguiadapter/res/icons/arithmetic-buttons.svg
+-rw-r--r--   0        0        0      886 2024-04-14 16:11:23.464322 pyguiadapter-0.3.5/pyguiadapter/res/icons/arithmetic-one.svg
+-rw-r--r--   0        0        0     1051 2024-04-14 16:11:23.464322 pyguiadapter-0.3.5/pyguiadapter/res/icons/arrow-keys.svg
+-rw-r--r--   0        0        0      510 2024-04-14 16:11:23.464322 pyguiadapter-0.3.5/pyguiadapter/res/icons/audio-file.svg
+-rw-r--r--   0        0        0      806 2024-04-14 16:11:23.464322 pyguiadapter-0.3.5/pyguiadapter/res/icons/audit.svg
+-rw-r--r--   0        0        0      503 2024-04-14 16:11:23.465322 pyguiadapter-0.3.5/pyguiadapter/res/icons/average.svg
+-rw-r--r--   0        0        0      871 2024-04-14 16:11:23.465322 pyguiadapter-0.3.5/pyguiadapter/res/icons/bitcoin.svg
+-rw-r--r--   0        0        0      753 2024-04-14 16:11:23.465322 pyguiadapter-0.3.5/pyguiadapter/res/icons/blackboard.svg
+-rw-r--r--   0        0        0      633 2024-04-14 16:11:23.465322 pyguiadapter-0.3.5/pyguiadapter/res/icons/blocks-and-arrows.svg
+-rw-r--r--   0        0        0      261 2024-04-14 16:11:23.465322 pyguiadapter-0.3.5/pyguiadapter/res/icons/bluetooth.svg
+-rw-r--r--   0        0        0      794 2024-04-14 16:11:23.466322 pyguiadapter-0.3.5/pyguiadapter/res/icons/bookmark-three.svg
+-rw-r--r--   0        0        0      981 2024-04-14 16:11:23.466322 pyguiadapter-0.3.5/pyguiadapter/res/icons/broadcast.svg
+-rw-r--r--   0        0        0      993 2024-04-14 16:11:23.466322 pyguiadapter-0.3.5/pyguiadapter/res/icons/browser.svg
+-rw-r--r--   0        0        0     1399 2024-04-14 16:11:23.466322 pyguiadapter-0.3.5/pyguiadapter/res/icons/bug.svg
+-rw-r--r--   0        0        0      978 2024-04-14 16:11:23.466322 pyguiadapter-0.3.5/pyguiadapter/res/icons/bytedance-mini-app.svg
+-rw-r--r--   0        0        0      334 2024-04-14 16:11:23.466322 pyguiadapter-0.3.5/pyguiadapter/res/icons/card-two.svg
+-rw-r--r--   0        0        0      643 2024-04-14 16:11:23.466322 pyguiadapter-0.3.5/pyguiadapter/res/icons/carousel-video.svg
+-rw-r--r--   0        0        0      849 2024-04-14 16:11:23.466322 pyguiadapter-0.3.5/pyguiadapter/res/icons/carousel.svg
+-rw-r--r--   0        0        0      685 2024-04-14 16:11:23.467323 pyguiadapter-0.3.5/pyguiadapter/res/icons/cast-screen.svg
+-rw-r--r--   0        0        0      472 2024-04-14 16:11:23.467323 pyguiadapter-0.3.5/pyguiadapter/res/icons/category-management.svg
+-rw-r--r--   0        0        0      443 2024-04-14 16:11:23.467323 pyguiadapter-0.3.5/pyguiadapter/res/icons/caution.svg
+-rw-r--r--   0        0        0     1016 2024-04-14 16:11:23.467323 pyguiadapter-0.3.5/pyguiadapter/res/icons/certificate.svg
+-rw-r--r--   0        0        0      634 2024-04-14 16:11:23.467323 pyguiadapter-0.3.5/pyguiadapter/res/icons/check-one.svg
+-rw-r--r--   0        0        0      697 2024-04-14 16:11:23.467323 pyguiadapter-0.3.5/pyguiadapter/res/icons/checklist.svg
+-rw-r--r--   0        0        0     1023 2024-04-14 16:11:23.467323 pyguiadapter-0.3.5/pyguiadapter/res/icons/chip.svg
+-rw-r--r--   0        0        0      519 2024-04-14 16:11:23.467323 pyguiadapter-0.3.5/pyguiadapter/res/icons/classroom.svg
+-rw-r--r--   0        0        0      478 2024-04-14 16:11:23.468322 pyguiadapter-0.3.5/pyguiadapter/res/icons/clipboard.svg
+-rw-r--r--   0        0        0      576 2024-04-14 16:11:23.468322 pyguiadapter-0.3.5/pyguiadapter/res/icons/close-one.svg
+-rw-r--r--   0        0        0     1211 2024-04-14 16:11:23.468322 pyguiadapter-0.3.5/pyguiadapter/res/icons/cloud-storage.svg
+-rw-r--r--   0        0        0      536 2024-04-14 16:11:23.468322 pyguiadapter-0.3.5/pyguiadapter/res/icons/code-brackets.svg
+-rw-r--r--   0        0        0      547 2024-04-14 16:11:23.468322 pyguiadapter-0.3.5/pyguiadapter/res/icons/code-download.svg
+-rw-r--r--   0        0        0      639 2024-04-14 16:11:23.468322 pyguiadapter-0.3.5/pyguiadapter/res/icons/code-laptop.svg
+-rw-r--r--   0        0        0      346 2024-04-14 16:11:23.468322 pyguiadapter-0.3.5/pyguiadapter/res/icons/code-one.svg
+-rw-r--r--   0        0        0      441 2024-04-14 16:11:23.468322 pyguiadapter-0.3.5/pyguiadapter/res/icons/code.svg
+-rw-r--r--   0        0        0      831 2024-04-14 16:11:23.469322 pyguiadapter-0.3.5/pyguiadapter/res/icons/collect-computer.svg
+-rw-r--r--   0        0        0      732 2024-04-14 16:11:23.469322 pyguiadapter-0.3.5/pyguiadapter/res/icons/collect-laptop.svg
+-rw-r--r--   0        0        0     1181 2024-04-14 16:11:23.469322 pyguiadapter-0.3.5/pyguiadapter/res/icons/collect-picture.svg
+-rw-r--r--   0        0        0     1118 2024-04-14 16:11:23.469322 pyguiadapter-0.3.5/pyguiadapter/res/icons/color-card.svg
+-rw-r--r--   0        0        0     1289 2024-04-14 16:11:23.469322 pyguiadapter-0.3.5/pyguiadapter/res/icons/command.svg
+-rw-r--r--   0        0        0      371 2024-04-14 16:11:23.469322 pyguiadapter-0.3.5/pyguiadapter/res/icons/comment-one.svg
+-rw-r--r--   0        0        0      581 2024-04-14 16:11:23.469322 pyguiadapter-0.3.5/pyguiadapter/res/icons/comment.svg
+-rw-r--r--   0        0        0      553 2024-04-14 16:11:23.470322 pyguiadapter-0.3.5/pyguiadapter/res/icons/comments.svg
+-rw-r--r--   0        0        0      628 2024-04-14 16:11:23.470322 pyguiadapter-0.3.5/pyguiadapter/res/icons/communication.svg
+-rw-r--r--   0        0        0      753 2024-04-14 16:11:23.470322 pyguiadapter-0.3.5/pyguiadapter/res/icons/compass.svg
+-rw-r--r--   0        0        0     1110 2024-04-14 16:11:23.470322 pyguiadapter-0.3.5/pyguiadapter/res/icons/compression.svg
+-rw-r--r--   0        0        0      556 2024-04-14 16:11:23.470322 pyguiadapter-0.3.5/pyguiadapter/res/icons/computer.svg
+-rw-r--r--   0        0        0      447 2024-04-14 16:11:23.470322 pyguiadapter-0.3.5/pyguiadapter/res/icons/cones.svg
+-rw-r--r--   0        0        0     1850 2024-04-14 16:11:23.470322 pyguiadapter-0.3.5/pyguiadapter/res/icons/connect.svg
+-rw-r--r--   0        0        0      620 2024-04-14 16:11:23.470322 pyguiadapter-0.3.5/pyguiadapter/res/icons/copy-one.svg
+-rw-r--r--   0        0        0      524 2024-04-14 16:11:23.470322 pyguiadapter-0.3.5/pyguiadapter/res/icons/copyright.svg
+-rw-r--r--   0        0        0     2644 2024-04-14 16:11:23.471322 pyguiadapter-0.3.5/pyguiadapter/res/icons/cpu.svg
+-rw-r--r--   0        0        0      516 2024-04-14 16:11:23.471322 pyguiadapter-0.3.5/pyguiadapter/res/icons/cross-ring-two.svg
+-rw-r--r--   0        0        0      895 2024-04-14 16:11:23.471322 pyguiadapter-0.3.5/pyguiadapter/res/icons/cube-four.svg
+-rw-r--r--   0        0        0      369 2024-04-14 16:11:23.471322 pyguiadapter-0.3.5/pyguiadapter/res/icons/curve-adjustment.svg
+-rw-r--r--   0        0        0     1177 2024-04-14 16:11:23.471322 pyguiadapter-0.3.5/pyguiadapter/res/icons/cuvette.svg
+-rw-r--r--   0        0        0     1199 2024-04-14 16:11:23.472322 pyguiadapter-0.3.5/pyguiadapter/res/icons/dashboard-one.svg
+-rw-r--r--   0        0        0     1332 2024-04-14 16:11:23.472322 pyguiadapter-0.3.5/pyguiadapter/res/icons/dashboard-two.svg
+-rw-r--r--   0        0        0     1221 2024-04-14 16:11:23.472322 pyguiadapter-0.3.5/pyguiadapter/res/icons/data-all.svg
+-rw-r--r--   0        0        0     1239 2024-04-14 16:11:23.472322 pyguiadapter-0.3.5/pyguiadapter/res/icons/data-display.svg
+-rw-r--r--   0        0        0     1255 2024-04-14 16:11:23.472322 pyguiadapter-0.3.5/pyguiadapter/res/icons/data-lock.svg
+-rw-r--r--   0        0        0      829 2024-04-14 16:11:23.472322 pyguiadapter-0.3.5/pyguiadapter/res/icons/data-screen.svg
+-rw-r--r--   0        0        0      833 2024-04-14 16:11:23.472322 pyguiadapter-0.3.5/pyguiadapter/res/icons/data-server.svg
+-rw-r--r--   0        0        0     1448 2024-04-14 16:11:23.472322 pyguiadapter-0.3.5/pyguiadapter/res/icons/data-switching.svg
+-rw-r--r--   0        0        0     1209 2024-04-14 16:11:23.473322 pyguiadapter-0.3.5/pyguiadapter/res/icons/data-user.svg
+-rw-r--r--   0        0        0      794 2024-04-14 16:11:23.473322 pyguiadapter-0.3.5/pyguiadapter/res/icons/data.svg
+-rw-r--r--   0        0        0     1588 2024-04-14 16:11:23.473322 pyguiadapter-0.3.5/pyguiadapter/res/icons/database-alert.svg
+-rw-r--r--   0        0        0     1606 2024-04-14 16:11:23.473322 pyguiadapter-0.3.5/pyguiadapter/res/icons/database-code.svg
+-rw-r--r--   0        0        0     1596 2024-04-14 16:11:23.473322 pyguiadapter-0.3.5/pyguiadapter/res/icons/database-config.svg
+-rw-r--r--   0        0        0     1513 2024-04-14 16:11:23.473322 pyguiadapter-0.3.5/pyguiadapter/res/icons/database-download.svg
+-rw-r--r--   0        0        0     1516 2024-04-14 16:11:23.473322 pyguiadapter-0.3.5/pyguiadapter/res/icons/database-enter.svg
+-rw-r--r--   0        0        0     1528 2024-04-14 16:11:23.473322 pyguiadapter-0.3.5/pyguiadapter/res/icons/database-fail.svg
+-rw-r--r--   0        0        0     1513 2024-04-14 16:11:23.474322 pyguiadapter-0.3.5/pyguiadapter/res/icons/database-first.svg
+-rw-r--r--   0        0        0     1492 2024-04-14 16:11:23.474322 pyguiadapter-0.3.5/pyguiadapter/res/icons/database-forbid.svg
+-rw-r--r--   0        0        0     1738 2024-04-14 16:11:23.474322 pyguiadapter-0.3.5/pyguiadapter/res/icons/database-lock.svg
+-rw-r--r--   0        0        0     1195 2024-04-14 16:11:23.474322 pyguiadapter-0.3.5/pyguiadapter/res/icons/database-network-point.svg
+-rw-r--r--   0        0        0     1770 2024-04-14 16:11:23.474322 pyguiadapter-0.3.5/pyguiadapter/res/icons/database-network.svg
+-rw-r--r--   0        0        0     1637 2024-04-14 16:11:23.474322 pyguiadapter-0.3.5/pyguiadapter/res/icons/database-point.svg
+-rw-r--r--   0        0        0     1390 2024-04-14 16:11:23.474322 pyguiadapter-0.3.5/pyguiadapter/res/icons/database-position.svg
+-rw-r--r--   0        0        0     1504 2024-04-14 16:11:23.475322 pyguiadapter-0.3.5/pyguiadapter/res/icons/database-power.svg
+-rw-r--r--   0        0        0     1528 2024-04-14 16:11:23.475322 pyguiadapter-0.3.5/pyguiadapter/res/icons/database-proportion.svg
+-rw-r--r--   0        0        0     1908 2024-04-14 16:11:23.475322 pyguiadapter-0.3.5/pyguiadapter/res/icons/database-search.svg
+-rw-r--r--   0        0        0     1542 2024-04-14 16:11:23.475322 pyguiadapter-0.3.5/pyguiadapter/res/icons/database-setting.svg
+-rw-r--r--   0        0        0     1504 2024-04-14 16:11:23.475322 pyguiadapter-0.3.5/pyguiadapter/res/icons/database-success.svg
+-rw-r--r--   0        0        0     1638 2024-04-14 16:11:23.475322 pyguiadapter-0.3.5/pyguiadapter/res/icons/database-sync.svg
+-rw-r--r--   0        0        0     1492 2024-04-14 16:11:23.475322 pyguiadapter-0.3.5/pyguiadapter/res/icons/database-time.svg
+-rw-r--r--   0        0        0      762 2024-04-14 16:11:23.475322 pyguiadapter-0.3.5/pyguiadapter/res/icons/date-comes-back.svg
+-rw-r--r--   0        0        0      470 2024-04-14 16:11:23.476322 pyguiadapter-0.3.5/pyguiadapter/res/icons/diamond-one.svg
+-rw-r--r--   0        0        0      470 2024-04-14 16:11:23.476322 pyguiadapter-0.3.5/pyguiadapter/res/icons/diamond-three.svg
+-rw-r--r--   0        0        0      466 2024-04-14 16:11:23.476322 pyguiadapter-0.3.5/pyguiadapter/res/icons/diamond-two.svg
+-rw-r--r--   0        0        0      855 2024-04-14 16:11:23.476322 pyguiadapter-0.3.5/pyguiadapter/res/icons/disk-one.svg
+-rw-r--r--   0        0        0      533 2024-04-14 16:11:23.476322 pyguiadapter-0.3.5/pyguiadapter/res/icons/disk-two.svg
+-rw-r--r--   0        0        0      599 2024-04-14 16:11:23.476322 pyguiadapter-0.3.5/pyguiadapter/res/icons/disk.svg
+-rw-r--r--   0        0        0      646 2024-04-14 16:11:23.476322 pyguiadapter-0.3.5/pyguiadapter/res/icons/document-folder.svg
+-rw-r--r--   0        0        0      957 2024-04-14 16:11:23.476322 pyguiadapter-0.3.5/pyguiadapter/res/icons/download-one.svg
+-rw-r--r--   0        0        0      649 2024-04-14 16:11:23.477322 pyguiadapter-0.3.5/pyguiadapter/res/icons/download-three.svg
+-rw-r--r--   0        0        0      730 2024-04-14 16:11:23.477322 pyguiadapter-0.3.5/pyguiadapter/res/icons/download-two.svg
+-rw-r--r--   0        0        0      827 2024-04-14 16:11:23.477322 pyguiadapter-0.3.5/pyguiadapter/res/icons/download-web.svg
+-rw-r--r--   0        0        0      500 2024-04-14 16:11:23.477322 pyguiadapter-0.3.5/pyguiadapter/res/icons/electrocardiogram.svg
+-rw-r--r--   0        0        0      568 2024-04-14 16:11:23.477322 pyguiadapter-0.3.5/pyguiadapter/res/icons/email-down.svg
+-rw-r--r--   0        0        0      567 2024-04-14 16:11:23.477322 pyguiadapter-0.3.5/pyguiadapter/res/icons/email-push.svg
+-rw-r--r--   0        0        0      634 2024-04-14 16:11:23.477322 pyguiadapter-0.3.5/pyguiadapter/res/icons/experiment-one.svg
+-rw-r--r--   0        0        0      731 2024-04-14 16:11:23.477322 pyguiadapter-0.3.5/pyguiadapter/res/icons/experiment.svg
+-rw-r--r--   0        0        0      680 2024-04-14 16:11:23.478322 pyguiadapter-0.3.5/pyguiadapter/res/icons/figma-component.svg
+-rw-r--r--   0        0        0      652 2024-04-14 16:11:23.478322 pyguiadapter-0.3.5/pyguiadapter/res/icons/file-addition.svg
+-rw-r--r--   0        0        0      664 2024-04-14 16:11:23.478322 pyguiadapter-0.3.5/pyguiadapter/res/icons/file-code.svg
+-rw-r--r--   0        0        0      856 2024-04-14 16:11:23.478322 pyguiadapter-0.3.5/pyguiadapter/res/icons/file-conversion.svg
+-rw-r--r--   0        0        0      772 2024-04-14 16:11:23.478322 pyguiadapter-0.3.5/pyguiadapter/res/icons/file-display.svg
+-rw-r--r--   0        0        0     1316 2024-04-14 16:11:23.478322 pyguiadapter-0.3.5/pyguiadapter/res/icons/file-pdf-one.svg
+-rw-r--r--   0        0        0     1381 2024-04-14 16:11:23.478322 pyguiadapter-0.3.5/pyguiadapter/res/icons/file-ppt.svg
+-rw-r--r--   0        0        0      658 2024-04-14 16:11:23.478322 pyguiadapter-0.3.5/pyguiadapter/res/icons/file-protection.svg
+-rw-r--r--   0        0        0      652 2024-04-14 16:11:23.479322 pyguiadapter-0.3.5/pyguiadapter/res/icons/file-text.svg
+-rw-r--r--   0        0        0      468 2024-04-14 16:11:23.479322 pyguiadapter-0.3.5/pyguiadapter/res/icons/file-word.svg
+-rw-r--r--   0        0        0      931 2024-04-14 16:11:23.479322 pyguiadapter-0.3.5/pyguiadapter/res/icons/film.svg
+-rw-r--r--   0        0        0      734 2024-04-14 16:11:23.479322 pyguiadapter-0.3.5/pyguiadapter/res/icons/flask.svg
+-rw-r--r--   0        0        0      455 2024-04-14 16:11:23.479322 pyguiadapter-0.3.5/pyguiadapter/res/icons/folder-open.svg
+-rw-r--r--   0        0        0      851 2024-04-14 16:11:23.479322 pyguiadapter-0.3.5/pyguiadapter/res/icons/game-handle.svg
+-rw-r--r--   0        0        0      989 2024-04-14 16:11:23.479322 pyguiadapter-0.3.5/pyguiadapter/res/icons/help.svg
+-rw-r--r--   0        0        0      545 2024-04-14 16:11:23.480322 pyguiadapter-0.3.5/pyguiadapter/res/icons/hexagon-one.svg
+-rw-r--r--   0        0        0      794 2024-04-14 16:11:23.480322 pyguiadapter-0.3.5/pyguiadapter/res/icons/id-card-h.svg
+-rw-r--r--   0        0        0      935 2024-04-14 16:11:23.480322 pyguiadapter-0.3.5/pyguiadapter/res/icons/info.svg
+-rw-r--r--   0        0        0      696 2024-04-14 16:11:23.480322 pyguiadapter-0.3.5/pyguiadapter/res/icons/install.svg
+-rw-r--r--   0        0        0    11553 2024-04-14 16:11:23.462322 pyguiadapter-0.3.5/pyguiadapter/res/icons/LICENSE
+-rw-r--r--   0        0        0      683 2024-04-14 16:11:23.480322 pyguiadapter-0.3.5/pyguiadapter/res/icons/many-to-many.svg
+-rw-r--r--   0        0        0      602 2024-04-14 16:11:23.480322 pyguiadapter-0.3.5/pyguiadapter/res/icons/message-emoji.svg
+-rw-r--r--   0        0        0      522 2024-04-14 16:11:23.481322 pyguiadapter-0.3.5/pyguiadapter/res/icons/message-one.svg
+-rw-r--r--   0        0        0      763 2024-04-14 16:11:23.481322 pyguiadapter-0.3.5/pyguiadapter/res/icons/message-privacy.svg
+-rw-r--r--   0        0        0      648 2024-04-14 16:11:23.481322 pyguiadapter-0.3.5/pyguiadapter/res/icons/message-search.svg
+-rw-r--r--   0        0        0      679 2024-04-14 16:11:23.481322 pyguiadapter-0.3.5/pyguiadapter/res/icons/message-security.svg
+-rw-r--r--   0        0        0      485 2024-04-14 16:11:23.481322 pyguiadapter-0.3.5/pyguiadapter/res/icons/message-sent.svg
+-rw-r--r--   0        0        0      577 2024-04-14 16:11:23.481322 pyguiadapter-0.3.5/pyguiadapter/res/icons/message-success.svg
+-rw-r--r--   0        0        0      550 2024-04-14 16:11:23.481322 pyguiadapter-0.3.5/pyguiadapter/res/icons/message-unread.svg
+-rw-r--r--   0        0        0      738 2024-04-14 16:11:23.481322 pyguiadapter-0.3.5/pyguiadapter/res/icons/message.svg
+-rw-r--r--   0        0        0      537 2024-04-14 16:11:23.482322 pyguiadapter-0.3.5/pyguiadapter/res/icons/mini-sd-card.svg
+-rw-r--r--   0        0        0      521 2024-04-14 16:11:23.482322 pyguiadapter-0.3.5/pyguiadapter/res/icons/monitor.svg
+-rw-r--r--   0        0        0     1053 2024-04-14 16:11:23.482322 pyguiadapter-0.3.5/pyguiadapter/res/icons/more-app.svg
+-rw-r--r--   0        0        0      971 2024-04-14 16:11:23.482322 pyguiadapter-0.3.5/pyguiadapter/res/icons/movie-board.svg
+-rw-r--r--   0        0        0     1213 2024-04-14 16:11:23.482322 pyguiadapter-0.3.5/pyguiadapter/res/icons/movie.svg
+-rw-r--r--   0        0        0      995 2024-04-14 16:11:23.482322 pyguiadapter-0.3.5/pyguiadapter/res/icons/multi-function-knife.svg
+-rw-r--r--   0        0        0      835 2024-04-14 16:11:23.482322 pyguiadapter-0.3.5/pyguiadapter/res/icons/notebook-one.svg
+-rw-r--r--   0        0        0      626 2024-04-14 16:11:23.482322 pyguiadapter-0.3.5/pyguiadapter/res/icons/octagon.svg
+-rw-r--r--   0        0        0      575 2024-04-14 16:11:23.483322 pyguiadapter-0.3.5/pyguiadapter/res/icons/online-meeting.svg
+-rw-r--r--   0        0        0      227 2024-04-14 16:11:23.483322 pyguiadapter-0.3.5/pyguiadapter/res/icons/oval-one.svg
+-rw-r--r--   0        0        0      537 2024-04-14 16:11:23.483322 pyguiadapter-0.3.5/pyguiadapter/res/icons/page-template.svg
+-rw-r--r--   0        0        0      440 2024-04-14 16:11:23.483322 pyguiadapter-0.3.5/pyguiadapter/res/icons/page.svg
+-rw-r--r--   0        0        0      412 2024-04-14 16:11:23.483322 pyguiadapter-0.3.5/pyguiadapter/res/icons/parallelogram.svg
+-rw-r--r--   0        0        0      633 2024-04-14 16:11:23.483322 pyguiadapter-0.3.5/pyguiadapter/res/icons/pay-code.svg
+-rw-r--r--   0        0        0      509 2024-04-14 16:11:23.483322 pyguiadapter-0.3.5/pyguiadapter/res/icons/pentagon-one.svg
+-rw-r--r--   0        0        0      980 2024-04-14 16:11:23.483322 pyguiadapter-0.3.5/pyguiadapter/res/icons/people-plus-one.svg
+-rw-r--r--   0        0        0     1040 2024-04-14 16:11:23.484322 pyguiadapter-0.3.5/pyguiadapter/res/icons/phone-incoming-one.svg
+-rw-r--r--   0        0        0     1029 2024-04-14 16:11:23.484322 pyguiadapter-0.3.5/pyguiadapter/res/icons/phone-incoming.svg
+-rw-r--r--   0        0        0     1083 2024-04-14 16:11:23.484322 pyguiadapter-0.3.5/pyguiadapter/res/icons/phone-missed.svg
+-rw-r--r--   0        0        0     1015 2024-04-14 16:11:23.484322 pyguiadapter-0.3.5/pyguiadapter/res/icons/phone-outgoing-one.svg
+-rw-r--r--   0        0        0     1008 2024-04-14 16:11:23.484322 pyguiadapter-0.3.5/pyguiadapter/res/icons/phone-outgoing.svg
+-rw-r--r--   0        0        0      811 2024-04-14 16:11:23.484322 pyguiadapter-0.3.5/pyguiadapter/res/icons/phone-telephone.svg
+-rw-r--r--   0        0        0      935 2024-04-14 16:11:23.484322 pyguiadapter-0.3.5/pyguiadapter/res/icons/phone-video-call.svg
+-rw-r--r--   0        0        0      974 2024-04-14 16:11:23.484322 pyguiadapter-0.3.5/pyguiadapter/res/icons/platte.svg
+-rw-r--r--   0        0        0      473 2024-04-14 16:11:23.485322 pyguiadapter-0.3.5/pyguiadapter/res/icons/play.svg
+-rw-r--r--   0        0        0      434 2024-04-14 16:11:23.485322 pyguiadapter-0.3.5/pyguiadapter/res/icons/powerpoint.svg
+-rw-r--r--   0        0        0      612 2024-04-14 16:11:23.485322 pyguiadapter-0.3.5/pyguiadapter/res/icons/ppt.svg
+-rw-r--r--   0        0        0      427 2024-04-14 16:11:23.485322 pyguiadapter-0.3.5/pyguiadapter/res/icons/puzzle.svg
+-rw-r--r--   0        0        0      364 2024-04-14 16:11:23.485322 pyguiadapter-0.3.5/pyguiadapter/res/icons/quadrilateral.svg
+-rw-r--r--   0        0        0      783 2024-04-14 16:11:23.485322 pyguiadapter-0.3.5/pyguiadapter/res/icons/record-disc.svg
+-rw-r--r--   0        0        0      880 2024-04-14 16:11:23.486322 pyguiadapter-0.3.5/pyguiadapter/res/icons/record.svg
+-rw-r--r--   0        0        0      319 2024-04-14 16:11:23.486322 pyguiadapter-0.3.5/pyguiadapter/res/icons/rectangle-one.svg
+-rw-r--r--   0        0        0      328 2024-04-14 16:11:23.486322 pyguiadapter-0.3.5/pyguiadapter/res/icons/rectangle-small.svg
+-rw-r--r--   0        0        0      319 2024-04-14 16:11:23.486322 pyguiadapter-0.3.5/pyguiadapter/res/icons/rectangle.svg
+-rw-r--r--   0        0        0      591 2024-04-14 16:11:23.486322 pyguiadapter-0.3.5/pyguiadapter/res/icons/rename.py
+-rw-r--r--   0        0        0      425 2024-04-14 16:11:23.486322 pyguiadapter-0.3.5/pyguiadapter/res/icons/right-angle.svg
+-rw-r--r--   0        0        0      217 2024-04-14 16:11:23.486322 pyguiadapter-0.3.5/pyguiadapter/res/icons/round.svg
+-rw-r--r--   0        0        0      901 2024-04-14 16:11:23.487322 pyguiadapter-0.3.5/pyguiadapter/res/icons/rule-two.svg
+-rw-r--r--   0        0        0      794 2024-04-14 16:11:23.487322 pyguiadapter-0.3.5/pyguiadapter/res/icons/ruler-one.svg
+-rw-r--r--   0        0        0      926 2024-04-14 16:11:23.487322 pyguiadapter-0.3.5/pyguiadapter/res/icons/ruler.svg
+-rw-r--r--   0        0        0      583 2024-04-14 16:11:23.487322 pyguiadapter-0.3.5/pyguiadapter/res/icons/sd-card.svg
+-rw-r--r--   0        0        0     1259 2024-04-14 16:11:23.487322 pyguiadapter-0.3.5/pyguiadapter/res/icons/setting-computer.svg
+-rw-r--r--   0        0        0     1148 2024-04-14 16:11:23.487322 pyguiadapter-0.3.5/pyguiadapter/res/icons/setting-laptop.svg
+-rw-r--r--   0        0        0     1443 2024-04-14 16:11:23.487322 pyguiadapter-0.3.5/pyguiadapter/res/icons/setting-two.svg
+-rw-r--r--   0        0        0      980 2024-04-14 16:11:23.487322 pyguiadapter-0.3.5/pyguiadapter/res/icons/share-one.svg
+-rw-r--r--   0        0        0      328 2024-04-14 16:11:23.487322 pyguiadapter-0.3.5/pyguiadapter/res/icons/square-small.svg
+-rw-r--r--   0        0        0      317 2024-04-14 16:11:23.488322 pyguiadapter-0.3.5/pyguiadapter/res/icons/square.svg
+-rw-r--r--   0        0        0      954 2024-04-14 16:11:23.488322 pyguiadapter-0.3.5/pyguiadapter/res/icons/system.svg
+-rw-r--r--   0        0        0      895 2024-04-14 16:11:23.488322 pyguiadapter-0.3.5/pyguiadapter/res/icons/table-file.svg
+-rw-r--r--   0        0        0     1216 2024-04-14 16:11:23.488322 pyguiadapter-0.3.5/pyguiadapter/res/icons/tape.svg
+-rw-r--r--   0        0        0      465 2024-04-14 16:11:23.488322 pyguiadapter-0.3.5/pyguiadapter/res/icons/terminal.svg
+-rw-r--r--   0        0        0      751 2024-04-14 16:11:23.488322 pyguiadapter-0.3.5/pyguiadapter/res/icons/test-tube.svg
+-rw-r--r--   0        0        0      724 2024-04-14 16:11:23.488322 pyguiadapter-0.3.5/pyguiadapter/res/icons/thermometer.svg
+-rw-r--r--   0        0        0      425 2024-04-14 16:11:23.488322 pyguiadapter-0.3.5/pyguiadapter/res/icons/tips-one.svg
+-rw-r--r--   0        0        0      510 2024-04-14 16:11:23.489322 pyguiadapter-0.3.5/pyguiadapter/res/icons/tool.svg
+-rw-r--r--   0        0        0      587 2024-04-14 16:11:23.489322 pyguiadapter-0.3.5/pyguiadapter/res/icons/topic-discussion.svg
+-rw-r--r--   0        0        0     1027 2024-04-14 16:11:23.489322 pyguiadapter-0.3.5/pyguiadapter/res/icons/topic.svg
+-rw-r--r--   0        0        0      413 2024-04-14 16:11:23.489322 pyguiadapter-0.3.5/pyguiadapter/res/icons/trapezoid.svg
+-rw-r--r--   0        0        0      831 2024-04-14 16:11:23.489322 pyguiadapter-0.3.5/pyguiadapter/res/icons/tree-list.svg
+-rw-r--r--   0        0        0     1970 2024-04-14 16:11:23.489322 pyguiadapter-0.3.5/pyguiadapter/res/icons/triangle-ruler.svg
+-rw-r--r--   0        0        0      468 2024-04-14 16:11:23.489322 pyguiadapter-0.3.5/pyguiadapter/res/icons/triangle.svg
+-rw-r--r--   0        0        0      717 2024-04-14 16:11:23.489322 pyguiadapter-0.3.5/pyguiadapter/res/icons/vial.svg
+-rw-r--r--   0        0        0     1823 2024-04-14 16:11:23.490322 pyguiadapter-0.3.5/pyguiadapter/res/icons/video.svg
+-rw-r--r--   0        0        0      706 2024-04-14 16:11:23.490322 pyguiadapter-0.3.5/pyguiadapter/res/icons/view-grid-card.svg
+-rw-r--r--   0        0        0      775 2024-04-14 16:11:23.490322 pyguiadapter-0.3.5/pyguiadapter/res/icons/view-grid-detail.svg
+-rw-r--r--   0        0        0      887 2024-04-14 16:11:23.490322 pyguiadapter-0.3.5/pyguiadapter/res/icons/view-grid-list.svg
+-rw-r--r--   0        0        0      642 2024-04-14 16:11:23.490322 pyguiadapter-0.3.5/pyguiadapter/res/icons/voice-input.svg
+-rw-r--r--   0        0        0      903 2024-04-14 16:11:23.490322 pyguiadapter-0.3.5/pyguiadapter/res/icons/voice-message.svg
+-rw-r--r--   0        0        0      685 2024-04-14 16:11:23.490322 pyguiadapter-0.3.5/pyguiadapter/res/icons/voice-one.svg
+-rw-r--r--   0        0        0      508 2024-04-14 16:11:23.490322 pyguiadapter-0.3.5/pyguiadapter/res/icons/voice.svg
+-rw-r--r--   0        0        0     1173 2024-04-14 16:11:23.490322 pyguiadapter-0.3.5/pyguiadapter/res/icons/weixin-mini-app.svg
+-rw-r--r--   0        0        0      809 2024-04-14 16:11:23.491322 pyguiadapter-0.3.5/pyguiadapter/res/icons/wifi.svg
+-rw-r--r--   0        0        0      976 2024-04-14 16:11:23.491322 pyguiadapter-0.3.5/pyguiadapter/res/icons/zip.svg
+-rw-r--r--   0        0        0        0 2024-04-20 07:19:02.882935 pyguiadapter-0.3.5/pyguiadapter/tools/__init__.py
+-rw-r--r--   0        0        0       99 2024-04-20 07:19:02.882935 pyguiadapter-0.3.5/pyguiadapter/tools/easyconfigs/__init__.py
+-rw-r--r--   0        0        0      738 2024-04-20 07:19:02.882935 pyguiadapter-0.3.5/pyguiadapter/tools/easyconfigs/constants.py
+-rw-r--r--   0        0        0      179 2024-04-20 07:19:02.883935 pyguiadapter-0.3.5/pyguiadapter/tools/easyconfigs/helper/__init__.py
+-rw-r--r--   0        0        0     6540 2024-04-20 07:19:02.883935 pyguiadapter-0.3.5/pyguiadapter/tools/easyconfigs/helper/const_name_value.py
+-rw-r--r--   0        0        0     3282 2024-04-20 07:19:02.883935 pyguiadapter-0.3.5/pyguiadapter/tools/easyconfigs/helper/imports.py
+-rw-r--r--   0        0        0     3114 2024-04-20 07:19:02.883935 pyguiadapter-0.3.5/pyguiadapter/tools/easyconfigs/helper/parameter_constants.py
+-rw-r--r--   0        0        0     2510 2024-04-20 07:19:02.884935 pyguiadapter-0.3.5/pyguiadapter/tools/easyconfigs/helper/parameter_widget_configs.py
+-rw-r--r--   0        0        0     9041 2024-04-20 07:19:02.884935 pyguiadapter-0.3.5/pyguiadapter/tools/easyconfigs/impl.py
+-rw-r--r--   0        0        0     1076 2024-04-20 07:19:02.884935 pyguiadapter-0.3.5/pyguiadapter/tools/easyconfigs/structures.py
+-rw-r--r--   0        0        0      882 2024-04-20 07:19:02.884935 pyguiadapter-0.3.5/pyguiadapter/tools/easyconfigs/tpl/configs.tpl
+-rw-r--r--   0        0        0      500 2024-04-20 07:19:02.884935 pyguiadapter-0.3.5/pyguiadapter/tools/easyconfigs/tpl/constants.tpl
+-rw-r--r--   0        0        0      762 2024-04-20 07:19:02.885935 pyguiadapter-0.3.5/pyguiadapter/tools/easyconfigs/utils.py
+-rw-r--r--   0        0        0      358 2024-04-17 16:40:54.565013 pyguiadapter-0.3.5/pyguiadapter/ui/__init__.py
+-rw-r--r--   0        0        0     1513 2024-04-14 16:11:23.491322 pyguiadapter-0.3.5/pyguiadapter/ui/config.py
+-rw-r--r--   0        0        0        0 2024-04-14 16:11:23.491322 pyguiadapter-0.3.5/pyguiadapter/ui/generated/__init__.py
+-rw-r--r--   0        0        0     2792 2024-04-16 16:25:55.273398 pyguiadapter-0.3.5/pyguiadapter/ui/generated/ui_class_init_window.py
+-rw-r--r--   0        0        0     7696 2024-04-16 16:25:55.346941 pyguiadapter-0.3.5/pyguiadapter/ui/generated/ui_execution_window.py
+-rw-r--r--   0        0        0     3700 2024-04-16 16:25:55.416780 pyguiadapter-0.3.5/pyguiadapter/ui/generated/ui_selection_window.py
+-rw-r--r--   0        0        0     1418 2024-04-17 16:04:29.140320 pyguiadapter-0.3.5/pyguiadapter/ui/menus.py
+-rw-r--r--   0        0        0     1457 2024-04-14 16:11:23.492322 pyguiadapter-0.3.5/pyguiadapter/ui/styles.py
+-rw-r--r--   0        0        0     3874 2024-04-17 16:07:29.237029 pyguiadapter-0.3.5/pyguiadapter/ui/utils.py
+-rw-r--r--   0        0        0        0 2024-04-17 16:23:22.163246 pyguiadapter-0.3.5/pyguiadapter/ui/window/__init__.py
+-rw-r--r--   0        0        0       78 2024-04-14 16:11:23.493322 pyguiadapter-0.3.5/pyguiadapter/ui/window/class_init/__init__.py
+-rw-r--r--   0        0        0      260 2024-04-17 16:16:41.343493 pyguiadapter-0.3.5/pyguiadapter/ui/window/class_init/config.py
+-rw-r--r--   0        0        0      160 2024-04-14 16:11:23.493322 pyguiadapter-0.3.5/pyguiadapter/ui/window/class_init/constants.py
+-rw-r--r--   0        0        0     5367 2024-04-17 16:16:05.127955 pyguiadapter-0.3.5/pyguiadapter/ui/window/class_init/impl.py
+-rw-r--r--   0        0        0       78 2024-04-14 16:11:23.493322 pyguiadapter-0.3.5/pyguiadapter/ui/window/func_execution/__init__.py
+-rw-r--r--   0        0        0     5243 2024-04-17 16:10:52.573365 pyguiadapter-0.3.5/pyguiadapter/ui/window/func_execution/base.py
+-rw-r--r--   0        0        0     2713 2024-04-17 16:17:12.915519 pyguiadapter-0.3.5/pyguiadapter/ui/window/func_execution/config.py
+-rw-r--r--   0        0        0      674 2024-04-20 13:29:28.867557 pyguiadapter-0.3.5/pyguiadapter/ui/window/func_execution/constants.py
+-rw-r--r--   0        0        0     4121 2024-04-14 16:11:23.494322 pyguiadapter-0.3.5/pyguiadapter/ui/window/func_execution/context.py
+-rw-r--r--   0        0        0      288 2024-04-14 16:11:23.494322 pyguiadapter-0.3.5/pyguiadapter/ui/window/func_execution/exceptions.py
+-rw-r--r--   0        0        0    18652 2024-04-29 10:58:08.523913 pyguiadapter-0.3.5/pyguiadapter/ui/window/func_execution/impl.py
+-rw-r--r--   0        0        0       78 2024-04-14 16:11:23.494322 pyguiadapter-0.3.5/pyguiadapter/ui/window/func_selection/__init__.py
+-rw-r--r--   0        0        0      830 2024-04-14 16:11:23.495322 pyguiadapter-0.3.5/pyguiadapter/ui/window/func_selection/config.py
+-rw-r--r--   0        0        0      305 2024-04-14 16:11:23.495322 pyguiadapter-0.3.5/pyguiadapter/ui/window/func_selection/constants.py
+-rw-r--r--   0        0        0     7509 2024-04-17 16:30:44.468256 pyguiadapter-0.3.5/pyguiadapter/ui/window/func_selection/impl.py
+-rw-r--r--   0        0        0      702 2024-04-29 13:44:49.686046 pyguiadapter-0.3.5/pyproject.toml
+-rw-r--r--   0        0        0     8722 2024-04-14 16:11:23.455323 pyguiadapter-0.3.5/README.md
+-rw-r--r--   0        0        0     9251 1970-01-01 00:00:00.000000 pyguiadapter-0.3.5/PKG-INFO
```

### Comparing `pyguiadapter-0.3.4/License` & `pyguiadapter-0.3.5/License`

 * *Files identical despite different names*

### Comparing `pyguiadapter-0.3.4/pyguiadapter/adapter/adapter.py` & `pyguiadapter-0.3.5/pyguiadapter/adapter/adapter.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import contextlib
 import inspect
 import sys
 from typing import Type, Optional, List, Dict, Callable, Union
 
-from PyQt6.QtWidgets import QApplication, QMessageBox
+from PyQt6.QtWidgets import QApplication, QMessageBox, QStyleFactory
 from function2widgets import CommonParameterWidgetArgs
 
 
 from pyguiadapter.commons import T, DocumentFormat
 from pyguiadapter.exceptions import (
     AlreadyExistsError,
     NotExistError,
@@ -21,14 +21,15 @@
 
 from .bundle import FunctionBundle
 from .constants import (
     ALWAYS_SHOW_SELECTION_WINDOW,
     AS_IS,
     _KEY_WIDGET_ARGS,
     CANCEL_EVENT_PARAM_NAME,
+    DEFAULT_APP_STYLE,
 )
 
 
 class GUIAdapter:
     def __init__(
         self,
         argv: List[str] = None,
@@ -43,14 +44,15 @@
         callback_selection_window_created: Optional[
             Callable[[SelectionWindow], None]
         ] = None,
         callback_execution_window_created: Optional[
             Callable[[ExecutionWindow], None]
         ] = None,
         always_show_selection_window: bool = ALWAYS_SHOW_SELECTION_WINDOW,
+        app_style: Optional[str] = DEFAULT_APP_STYLE,
     ):
         if argv is None:
             argv = sys.argv
 
         self._argv = argv
         self._config_class_init_window = (
             config_class_init_window or ClassInitWindowConfig()
@@ -63,14 +65,16 @@
         )
 
         self._callback_app_started = callback_app_started
         self._callback_execution_window_created = callback_execution_window_created
         self._callback_class_init_window_created = callback_class_init_window_created
         self._callback_selection_window_created = callback_selection_window_created
 
+        self._app_style = app_style
+
         self.always_show_selection_window = always_show_selection_window
 
         self._func_bundles = {}
         self._application: Optional[QApplication] = None
 
         self._selection_window: Optional[SelectionWindow] = None
         self._execution_window: Optional[ExecutionWindow] = None
@@ -171,14 +175,16 @@
     @property
     def execution_window_config(self) -> ExecutionWindowConfig:
         return self._config_execution_window
 
     def _start_application(self):
         if self._application is not None:
             return
+        if self._app_style:
+            QApplication.setStyle(QStyleFactory.create(self._app_style))
         self._application = QApplication(self._argv)
         if self._callback_app_started is not None:
             self._callback_app_started(self._application)
 
     def _execute_application(self):
         if self._application is None:
             raise AppNotStartedError("application not started")
```

### Comparing `pyguiadapter-0.3.4/pyguiadapter/adapter/bundle.py` & `pyguiadapter-0.3.5/pyguiadapter/adapter/bundle.py`

 * *Files identical despite different names*

### Comparing `pyguiadapter-0.3.4/pyguiadapter/adapter/executor.py` & `pyguiadapter-0.3.5/pyguiadapter/adapter/executor.py`

 * *Files identical despite different names*

### Comparing `pyguiadapter-0.3.4/pyguiadapter/commons.py` & `pyguiadapter-0.3.5/pyguiadapter/commons.py`

 * *Files identical despite different names*

### Comparing `pyguiadapter-0.3.4/pyguiadapter/interact/ulogging.py` & `pyguiadapter-0.3.5/pyguiadapter/interact/ulogging.py`

 * *Files identical despite different names*

### Comparing `pyguiadapter-0.3.4/pyguiadapter/interact/upopup.py` & `pyguiadapter-0.3.5/pyguiadapter/interact/upopup.py`

 * *Files identical despite different names*

### Comparing `pyguiadapter-0.3.4/pyguiadapter/interact/uprint.py` & `pyguiadapter-0.3.5/pyguiadapter/interact/uprint.py`

 * *Files identical despite different names*

### Comparing `pyguiadapter-0.3.4/pyguiadapter/res/icons/abnormal.svg` & `pyguiadapter-0.3.5/pyguiadapter/res/icons/abnormal.svg`

 * *Files identical despite different names*

### Comparing `pyguiadapter-0.3.4/pyguiadapter/res/icons/acoustic.svg` & `pyguiadapter-0.3.5/pyguiadapter/res/icons/acoustic.svg`

 * *Files identical despite different names*

### Comparing `pyguiadapter-0.3.4/pyguiadapter/res/icons/add-computer.svg` & `pyguiadapter-0.3.5/pyguiadapter/res/icons/add-computer.svg`

 * *Files identical despite different names*

### Comparing `pyguiadapter-0.3.4/pyguiadapter/res/icons/add-picture.svg` & `pyguiadapter-0.3.5/pyguiadapter/res/icons/add-picture.svg`

 * *Files identical despite different names*

### Comparing `pyguiadapter-0.3.4/pyguiadapter/res/icons/add-print.svg` & `pyguiadapter-0.3.5/pyguiadapter/res/icons/add-print.svg`

 * *Files identical despite different names*

### Comparing `pyguiadapter-0.3.4/pyguiadapter/res/icons/add-user.svg` & `pyguiadapter-0.3.5/pyguiadapter/res/icons/add-user.svg`

 * *Files identical despite different names*

### Comparing `pyguiadapter-0.3.4/pyguiadapter/res/icons/add-web.svg` & `pyguiadapter-0.3.5/pyguiadapter/res/icons/add-web.svg`

 * *Files identical despite different names*

### Comparing `pyguiadapter-0.3.4/pyguiadapter/res/icons/api-app.svg` & `pyguiadapter-0.3.5/pyguiadapter/res/icons/api-app.svg`

 * *Files identical despite different names*

### Comparing `pyguiadapter-0.3.4/pyguiadapter/res/icons/application-effect.svg` & `pyguiadapter-0.3.5/pyguiadapter/res/icons/application-effect.svg`

 * *Files identical despite different names*

### Comparing `pyguiadapter-0.3.4/pyguiadapter/res/icons/application-one.svg` & `pyguiadapter-0.3.5/pyguiadapter/res/icons/application-one.svg`

 * *Files identical despite different names*

### Comparing `pyguiadapter-0.3.4/pyguiadapter/res/icons/arithmetic-buttons.svg` & `pyguiadapter-0.3.5/pyguiadapter/res/icons/arithmetic-buttons.svg`

 * *Files identical despite different names*

### Comparing `pyguiadapter-0.3.4/pyguiadapter/res/icons/arithmetic-one.svg` & `pyguiadapter-0.3.5/pyguiadapter/res/icons/arithmetic-one.svg`

 * *Files identical despite different names*

### Comparing `pyguiadapter-0.3.4/pyguiadapter/res/icons/arrow-keys.svg` & `pyguiadapter-0.3.5/pyguiadapter/res/icons/arrow-keys.svg`

 * *Files identical despite different names*

### Comparing `pyguiadapter-0.3.4/pyguiadapter/res/icons/audit.svg` & `pyguiadapter-0.3.5/pyguiadapter/res/icons/audit.svg`

 * *Files identical despite different names*

### Comparing `pyguiadapter-0.3.4/pyguiadapter/res/icons/bitcoin.svg` & `pyguiadapter-0.3.5/pyguiadapter/res/icons/bitcoin.svg`

 * *Files identical despite different names*

### Comparing `pyguiadapter-0.3.4/pyguiadapter/res/icons/blackboard.svg` & `pyguiadapter-0.3.5/pyguiadapter/res/icons/blackboard.svg`

 * *Files identical despite different names*

### Comparing `pyguiadapter-0.3.4/pyguiadapter/res/icons/blocks-and-arrows.svg` & `pyguiadapter-0.3.5/pyguiadapter/res/icons/blocks-and-arrows.svg`

 * *Files identical despite different names*

### Comparing `pyguiadapter-0.3.4/pyguiadapter/res/icons/bookmark-three.svg` & `pyguiadapter-0.3.5/pyguiadapter/res/icons/bookmark-three.svg`

 * *Files identical despite different names*

### Comparing `pyguiadapter-0.3.4/pyguiadapter/res/icons/broadcast.svg` & `pyguiadapter-0.3.5/pyguiadapter/res/icons/broadcast.svg`

 * *Files identical despite different names*

### Comparing `pyguiadapter-0.3.4/pyguiadapter/res/icons/browser.svg` & `pyguiadapter-0.3.5/pyguiadapter/res/icons/browser.svg`

 * *Files identical despite different names*

### Comparing `pyguiadapter-0.3.4/pyguiadapter/res/icons/bug.svg` & `pyguiadapter-0.3.5/pyguiadapter/res/icons/bug.svg`

 * *Files identical despite different names*

### Comparing `pyguiadapter-0.3.4/pyguiadapter/res/icons/bytedance-mini-app.svg` & `pyguiadapter-0.3.5/pyguiadapter/res/icons/bytedance-mini-app.svg`

 * *Files identical despite different names*

### Comparing `pyguiadapter-0.3.4/pyguiadapter/res/icons/carousel-video.svg` & `pyguiadapter-0.3.5/pyguiadapter/res/icons/carousel-video.svg`

 * *Files identical despite different names*

### Comparing `pyguiadapter-0.3.4/pyguiadapter/res/icons/carousel.svg` & `pyguiadapter-0.3.5/pyguiadapter/res/icons/carousel.svg`

 * *Files identical despite different names*

### Comparing `pyguiadapter-0.3.4/pyguiadapter/res/icons/cast-screen.svg` & `pyguiadapter-0.3.5/pyguiadapter/res/icons/cast-screen.svg`

 * *Files identical despite different names*

### Comparing `pyguiadapter-0.3.4/pyguiadapter/res/icons/certificate.svg` & `pyguiadapter-0.3.5/pyguiadapter/res/icons/certificate.svg`

 * *Files identical despite different names*

### Comparing `pyguiadapter-0.3.4/pyguiadapter/res/icons/check-one.svg` & `pyguiadapter-0.3.5/pyguiadapter/res/icons/check-one.svg`

 * *Files identical despite different names*

### Comparing `pyguiadapter-0.3.4/pyguiadapter/res/icons/checklist.svg` & `pyguiadapter-0.3.5/pyguiadapter/res/icons/checklist.svg`

 * *Files identical despite different names*

### Comparing `pyguiadapter-0.3.4/pyguiadapter/res/icons/chip.svg` & `pyguiadapter-0.3.5/pyguiadapter/res/icons/chip.svg`

 * *Files identical despite different names*

### Comparing `pyguiadapter-0.3.4/pyguiadapter/res/icons/classroom.svg` & `pyguiadapter-0.3.5/pyguiadapter/res/icons/classroom.svg`

 * *Files identical despite different names*

### Comparing `pyguiadapter-0.3.4/pyguiadapter/res/icons/close-one.svg` & `pyguiadapter-0.3.5/pyguiadapter/res/icons/close-one.svg`

 * *Files identical despite different names*

### Comparing `pyguiadapter-0.3.4/pyguiadapter/res/icons/cloud-storage.svg` & `pyguiadapter-0.3.5/pyguiadapter/res/icons/cloud-storage.svg`

 * *Files identical despite different names*

### Comparing `pyguiadapter-0.3.4/pyguiadapter/res/icons/code-brackets.svg` & `pyguiadapter-0.3.5/pyguiadapter/res/icons/code-brackets.svg`

 * *Files identical despite different names*

### Comparing `pyguiadapter-0.3.4/pyguiadapter/res/icons/code-download.svg` & `pyguiadapter-0.3.5/pyguiadapter/res/icons/code-download.svg`

 * *Files identical despite different names*

### Comparing `pyguiadapter-0.3.4/pyguiadapter/res/icons/code-laptop.svg` & `pyguiadapter-0.3.5/pyguiadapter/res/icons/code-laptop.svg`

 * *Files identical despite different names*

### Comparing `pyguiadapter-0.3.4/pyguiadapter/res/icons/collect-computer.svg` & `pyguiadapter-0.3.5/pyguiadapter/res/icons/collect-computer.svg`

 * *Files identical despite different names*

### Comparing `pyguiadapter-0.3.4/pyguiadapter/res/icons/collect-laptop.svg` & `pyguiadapter-0.3.5/pyguiadapter/res/icons/collect-laptop.svg`

 * *Files identical despite different names*

### Comparing `pyguiadapter-0.3.4/pyguiadapter/res/icons/collect-picture.svg` & `pyguiadapter-0.3.5/pyguiadapter/res/icons/collect-picture.svg`

 * *Files identical despite different names*

### Comparing `pyguiadapter-0.3.4/pyguiadapter/res/icons/color-card.svg` & `pyguiadapter-0.3.5/pyguiadapter/res/icons/color-card.svg`

 * *Files identical despite different names*

### Comparing `pyguiadapter-0.3.4/pyguiadapter/res/icons/command.svg` & `pyguiadapter-0.3.5/pyguiadapter/res/icons/command.svg`

 * *Files identical despite different names*

### Comparing `pyguiadapter-0.3.4/pyguiadapter/res/icons/comment.svg` & `pyguiadapter-0.3.5/pyguiadapter/res/icons/comment.svg`

 * *Files identical despite different names*

### Comparing `pyguiadapter-0.3.4/pyguiadapter/res/icons/comments.svg` & `pyguiadapter-0.3.5/pyguiadapter/res/icons/comments.svg`

 * *Files identical despite different names*

### Comparing `pyguiadapter-0.3.4/pyguiadapter/res/icons/communication.svg` & `pyguiadapter-0.3.5/pyguiadapter/res/icons/communication.svg`

 * *Files identical despite different names*

### Comparing `pyguiadapter-0.3.4/pyguiadapter/res/icons/compass.svg` & `pyguiadapter-0.3.5/pyguiadapter/res/icons/compass.svg`

 * *Files identical despite different names*

### Comparing `pyguiadapter-0.3.4/pyguiadapter/res/icons/compression.svg` & `pyguiadapter-0.3.5/pyguiadapter/res/icons/compression.svg`

 * *Files identical despite different names*

### Comparing `pyguiadapter-0.3.4/pyguiadapter/res/icons/computer.svg` & `pyguiadapter-0.3.5/pyguiadapter/res/icons/computer.svg`

 * *Files identical despite different names*

### Comparing `pyguiadapter-0.3.4/pyguiadapter/res/icons/connect.svg` & `pyguiadapter-0.3.5/pyguiadapter/res/icons/connect.svg`

 * *Files identical despite different names*

### Comparing `pyguiadapter-0.3.4/pyguiadapter/res/icons/copy-one.svg` & `pyguiadapter-0.3.5/pyguiadapter/res/icons/copy-one.svg`

 * *Files identical despite different names*

### Comparing `pyguiadapter-0.3.4/pyguiadapter/res/icons/copyright.svg` & `pyguiadapter-0.3.5/pyguiadapter/res/icons/copyright.svg`

 * *Files identical despite different names*

### Comparing `pyguiadapter-0.3.4/pyguiadapter/res/icons/cpu.svg` & `pyguiadapter-0.3.5/pyguiadapter/res/icons/cpu.svg`

 * *Files identical despite different names*

### Comparing `pyguiadapter-0.3.4/pyguiadapter/res/icons/cross-ring-two.svg` & `pyguiadapter-0.3.5/pyguiadapter/res/icons/cross-ring-two.svg`

 * *Files identical despite different names*

### Comparing `pyguiadapter-0.3.4/pyguiadapter/res/icons/cube-four.svg` & `pyguiadapter-0.3.5/pyguiadapter/res/icons/cube-four.svg`

 * *Files identical despite different names*

### Comparing `pyguiadapter-0.3.4/pyguiadapter/res/icons/cuvette.svg` & `pyguiadapter-0.3.5/pyguiadapter/res/icons/cuvette.svg`

 * *Files identical despite different names*

### Comparing `pyguiadapter-0.3.4/pyguiadapter/res/icons/dashboard-one.svg` & `pyguiadapter-0.3.5/pyguiadapter/res/icons/dashboard-one.svg`

 * *Files identical despite different names*

### Comparing `pyguiadapter-0.3.4/pyguiadapter/res/icons/dashboard-two.svg` & `pyguiadapter-0.3.5/pyguiadapter/res/icons/dashboard-two.svg`

 * *Files identical despite different names*

### Comparing `pyguiadapter-0.3.4/pyguiadapter/res/icons/data-all.svg` & `pyguiadapter-0.3.5/pyguiadapter/res/icons/data-all.svg`

 * *Files identical despite different names*

### Comparing `pyguiadapter-0.3.4/pyguiadapter/res/icons/data-display.svg` & `pyguiadapter-0.3.5/pyguiadapter/res/icons/data-display.svg`

 * *Files identical despite different names*

### Comparing `pyguiadapter-0.3.4/pyguiadapter/res/icons/data-lock.svg` & `pyguiadapter-0.3.5/pyguiadapter/res/icons/data-lock.svg`

 * *Files identical despite different names*

### Comparing `pyguiadapter-0.3.4/pyguiadapter/res/icons/data-screen.svg` & `pyguiadapter-0.3.5/pyguiadapter/res/icons/data-screen.svg`

 * *Files identical despite different names*

### Comparing `pyguiadapter-0.3.4/pyguiadapter/res/icons/data-server.svg` & `pyguiadapter-0.3.5/pyguiadapter/res/icons/data-server.svg`

 * *Files identical despite different names*

### Comparing `pyguiadapter-0.3.4/pyguiadapter/res/icons/data-switching.svg` & `pyguiadapter-0.3.5/pyguiadapter/res/icons/data-switching.svg`

 * *Files identical despite different names*

### Comparing `pyguiadapter-0.3.4/pyguiadapter/res/icons/data-user.svg` & `pyguiadapter-0.3.5/pyguiadapter/res/icons/data-user.svg`

 * *Files identical despite different names*

### Comparing `pyguiadapter-0.3.4/pyguiadapter/res/icons/data.svg` & `pyguiadapter-0.3.5/pyguiadapter/res/icons/data.svg`

 * *Files identical despite different names*

### Comparing `pyguiadapter-0.3.4/pyguiadapter/res/icons/database-alert.svg` & `pyguiadapter-0.3.5/pyguiadapter/res/icons/database-alert.svg`

 * *Files identical despite different names*

### Comparing `pyguiadapter-0.3.4/pyguiadapter/res/icons/database-code.svg` & `pyguiadapter-0.3.5/pyguiadapter/res/icons/database-code.svg`

 * *Files identical despite different names*

### Comparing `pyguiadapter-0.3.4/pyguiadapter/res/icons/database-config.svg` & `pyguiadapter-0.3.5/pyguiadapter/res/icons/database-config.svg`

 * *Files identical despite different names*

### Comparing `pyguiadapter-0.3.4/pyguiadapter/res/icons/database-download.svg` & `pyguiadapter-0.3.5/pyguiadapter/res/icons/database-download.svg`

 * *Files identical despite different names*

### Comparing `pyguiadapter-0.3.4/pyguiadapter/res/icons/database-enter.svg` & `pyguiadapter-0.3.5/pyguiadapter/res/icons/database-enter.svg`

 * *Files identical despite different names*

### Comparing `pyguiadapter-0.3.4/pyguiadapter/res/icons/database-fail.svg` & `pyguiadapter-0.3.5/pyguiadapter/res/icons/database-fail.svg`

 * *Files identical despite different names*

### Comparing `pyguiadapter-0.3.4/pyguiadapter/res/icons/database-first.svg` & `pyguiadapter-0.3.5/pyguiadapter/res/icons/database-first.svg`

 * *Files identical despite different names*

### Comparing `pyguiadapter-0.3.4/pyguiadapter/res/icons/database-forbid.svg` & `pyguiadapter-0.3.5/pyguiadapter/res/icons/database-forbid.svg`

 * *Files identical despite different names*

### Comparing `pyguiadapter-0.3.4/pyguiadapter/res/icons/database-lock.svg` & `pyguiadapter-0.3.5/pyguiadapter/res/icons/database-lock.svg`

 * *Files identical despite different names*

### Comparing `pyguiadapter-0.3.4/pyguiadapter/res/icons/database-network-point.svg` & `pyguiadapter-0.3.5/pyguiadapter/res/icons/database-network-point.svg`

 * *Files identical despite different names*

### Comparing `pyguiadapter-0.3.4/pyguiadapter/res/icons/database-network.svg` & `pyguiadapter-0.3.5/pyguiadapter/res/icons/database-network.svg`

 * *Files identical despite different names*

### Comparing `pyguiadapter-0.3.4/pyguiadapter/res/icons/database-point.svg` & `pyguiadapter-0.3.5/pyguiadapter/res/icons/database-point.svg`

 * *Files identical despite different names*

### Comparing `pyguiadapter-0.3.4/pyguiadapter/res/icons/database-position.svg` & `pyguiadapter-0.3.5/pyguiadapter/res/icons/database-position.svg`

 * *Files identical despite different names*

### Comparing `pyguiadapter-0.3.4/pyguiadapter/res/icons/database-power.svg` & `pyguiadapter-0.3.5/pyguiadapter/res/icons/database-power.svg`

 * *Files identical despite different names*

### Comparing `pyguiadapter-0.3.4/pyguiadapter/res/icons/database-proportion.svg` & `pyguiadapter-0.3.5/pyguiadapter/res/icons/database-proportion.svg`

 * *Files identical despite different names*

### Comparing `pyguiadapter-0.3.4/pyguiadapter/res/icons/database-search.svg` & `pyguiadapter-0.3.5/pyguiadapter/res/icons/database-search.svg`

 * *Files identical despite different names*

### Comparing `pyguiadapter-0.3.4/pyguiadapter/res/icons/database-setting.svg` & `pyguiadapter-0.3.5/pyguiadapter/res/icons/database-setting.svg`

 * *Files identical despite different names*

### Comparing `pyguiadapter-0.3.4/pyguiadapter/res/icons/database-success.svg` & `pyguiadapter-0.3.5/pyguiadapter/res/icons/database-success.svg`

 * *Files identical despite different names*

### Comparing `pyguiadapter-0.3.4/pyguiadapter/res/icons/database-sync.svg` & `pyguiadapter-0.3.5/pyguiadapter/res/icons/database-sync.svg`

 * *Files identical despite different names*

### Comparing `pyguiadapter-0.3.4/pyguiadapter/res/icons/database-time.svg` & `pyguiadapter-0.3.5/pyguiadapter/res/icons/database-time.svg`

 * *Files identical despite different names*

### Comparing `pyguiadapter-0.3.4/pyguiadapter/res/icons/date-comes-back.svg` & `pyguiadapter-0.3.5/pyguiadapter/res/icons/date-comes-back.svg`

 * *Files identical despite different names*

### Comparing `pyguiadapter-0.3.4/pyguiadapter/res/icons/disk-one.svg` & `pyguiadapter-0.3.5/pyguiadapter/res/icons/disk-one.svg`

 * *Files identical despite different names*

### Comparing `pyguiadapter-0.3.4/pyguiadapter/res/icons/disk-two.svg` & `pyguiadapter-0.3.5/pyguiadapter/res/icons/disk-two.svg`

 * *Files identical despite different names*

### Comparing `pyguiadapter-0.3.4/pyguiadapter/res/icons/disk.svg` & `pyguiadapter-0.3.5/pyguiadapter/res/icons/disk.svg`

 * *Files identical despite different names*

### Comparing `pyguiadapter-0.3.4/pyguiadapter/res/icons/document-folder.svg` & `pyguiadapter-0.3.5/pyguiadapter/res/icons/document-folder.svg`

 * *Files identical despite different names*

### Comparing `pyguiadapter-0.3.4/pyguiadapter/res/icons/download-one.svg` & `pyguiadapter-0.3.5/pyguiadapter/res/icons/download-one.svg`

 * *Files identical despite different names*

### Comparing `pyguiadapter-0.3.4/pyguiadapter/res/icons/download-three.svg` & `pyguiadapter-0.3.5/pyguiadapter/res/icons/download-three.svg`

 * *Files identical despite different names*

### Comparing `pyguiadapter-0.3.4/pyguiadapter/res/icons/download-two.svg` & `pyguiadapter-0.3.5/pyguiadapter/res/icons/download-two.svg`

 * *Files identical despite different names*

### Comparing `pyguiadapter-0.3.4/pyguiadapter/res/icons/download-web.svg` & `pyguiadapter-0.3.5/pyguiadapter/res/icons/download-web.svg`

 * *Files identical despite different names*

### Comparing `pyguiadapter-0.3.4/pyguiadapter/res/icons/email-down.svg` & `pyguiadapter-0.3.5/pyguiadapter/res/icons/email-down.svg`

 * *Files identical despite different names*

### Comparing `pyguiadapter-0.3.4/pyguiadapter/res/icons/email-push.svg` & `pyguiadapter-0.3.5/pyguiadapter/res/icons/email-push.svg`

 * *Files identical despite different names*

### Comparing `pyguiadapter-0.3.4/pyguiadapter/res/icons/experiment-one.svg` & `pyguiadapter-0.3.5/pyguiadapter/res/icons/experiment-one.svg`

 * *Files identical despite different names*

### Comparing `pyguiadapter-0.3.4/pyguiadapter/res/icons/experiment.svg` & `pyguiadapter-0.3.5/pyguiadapter/res/icons/experiment.svg`

 * *Files identical despite different names*

### Comparing `pyguiadapter-0.3.4/pyguiadapter/res/icons/figma-component.svg` & `pyguiadapter-0.3.5/pyguiadapter/res/icons/figma-component.svg`

 * *Files identical despite different names*

### Comparing `pyguiadapter-0.3.4/pyguiadapter/res/icons/file-addition.svg` & `pyguiadapter-0.3.5/pyguiadapter/res/icons/file-addition.svg`

 * *Files identical despite different names*

### Comparing `pyguiadapter-0.3.4/pyguiadapter/res/icons/file-code.svg` & `pyguiadapter-0.3.5/pyguiadapter/res/icons/file-code.svg`

 * *Files identical despite different names*

### Comparing `pyguiadapter-0.3.4/pyguiadapter/res/icons/file-conversion.svg` & `pyguiadapter-0.3.5/pyguiadapter/res/icons/file-conversion.svg`

 * *Files identical despite different names*

### Comparing `pyguiadapter-0.3.4/pyguiadapter/res/icons/file-display.svg` & `pyguiadapter-0.3.5/pyguiadapter/res/icons/file-display.svg`

 * *Files identical despite different names*

### Comparing `pyguiadapter-0.3.4/pyguiadapter/res/icons/file-pdf-one.svg` & `pyguiadapter-0.3.5/pyguiadapter/res/icons/file-pdf-one.svg`

 * *Files identical despite different names*

### Comparing `pyguiadapter-0.3.4/pyguiadapter/res/icons/file-ppt.svg` & `pyguiadapter-0.3.5/pyguiadapter/res/icons/file-ppt.svg`

 * *Files identical despite different names*

### Comparing `pyguiadapter-0.3.4/pyguiadapter/res/icons/file-protection.svg` & `pyguiadapter-0.3.5/pyguiadapter/res/icons/file-protection.svg`

 * *Files identical despite different names*

### Comparing `pyguiadapter-0.3.4/pyguiadapter/res/icons/file-text.svg` & `pyguiadapter-0.3.5/pyguiadapter/res/icons/file-text.svg`

 * *Files identical despite different names*

### Comparing `pyguiadapter-0.3.4/pyguiadapter/res/icons/film.svg` & `pyguiadapter-0.3.5/pyguiadapter/res/icons/film.svg`

 * *Files identical despite different names*

### Comparing `pyguiadapter-0.3.4/pyguiadapter/res/icons/flask.svg` & `pyguiadapter-0.3.5/pyguiadapter/res/icons/flask.svg`

 * *Files identical despite different names*

### Comparing `pyguiadapter-0.3.4/pyguiadapter/res/icons/game-handle.svg` & `pyguiadapter-0.3.5/pyguiadapter/res/icons/game-handle.svg`

 * *Files identical despite different names*

### Comparing `pyguiadapter-0.3.4/pyguiadapter/res/icons/help.svg` & `pyguiadapter-0.3.5/pyguiadapter/res/icons/help.svg`

 * *Files identical despite different names*

### Comparing `pyguiadapter-0.3.4/pyguiadapter/res/icons/hexagon-one.svg` & `pyguiadapter-0.3.5/pyguiadapter/res/icons/hexagon-one.svg`

 * *Files identical despite different names*

### Comparing `pyguiadapter-0.3.4/pyguiadapter/res/icons/id-card-h.svg` & `pyguiadapter-0.3.5/pyguiadapter/res/icons/id-card-h.svg`

 * *Files identical despite different names*

### Comparing `pyguiadapter-0.3.4/pyguiadapter/res/icons/info.svg` & `pyguiadapter-0.3.5/pyguiadapter/res/icons/info.svg`

 * *Files identical despite different names*

### Comparing `pyguiadapter-0.3.4/pyguiadapter/res/icons/install.svg` & `pyguiadapter-0.3.5/pyguiadapter/res/icons/install.svg`

 * *Files identical despite different names*

### Comparing `pyguiadapter-0.3.4/pyguiadapter/res/icons/LICENSE` & `pyguiadapter-0.3.5/pyguiadapter/res/icons/LICENSE`

 * *Files identical despite different names*

### Comparing `pyguiadapter-0.3.4/pyguiadapter/res/icons/many-to-many.svg` & `pyguiadapter-0.3.5/pyguiadapter/res/icons/many-to-many.svg`

 * *Files identical despite different names*

### Comparing `pyguiadapter-0.3.4/pyguiadapter/res/icons/message-emoji.svg` & `pyguiadapter-0.3.5/pyguiadapter/res/icons/message-emoji.svg`

 * *Files identical despite different names*

### Comparing `pyguiadapter-0.3.4/pyguiadapter/res/icons/message-one.svg` & `pyguiadapter-0.3.5/pyguiadapter/res/icons/message-one.svg`

 * *Files identical despite different names*

### Comparing `pyguiadapter-0.3.4/pyguiadapter/res/icons/message-privacy.svg` & `pyguiadapter-0.3.5/pyguiadapter/res/icons/message-privacy.svg`

 * *Files identical despite different names*

### Comparing `pyguiadapter-0.3.4/pyguiadapter/res/icons/message-search.svg` & `pyguiadapter-0.3.5/pyguiadapter/res/icons/message-search.svg`

 * *Files identical despite different names*

### Comparing `pyguiadapter-0.3.4/pyguiadapter/res/icons/message-security.svg` & `pyguiadapter-0.3.5/pyguiadapter/res/icons/message-security.svg`

 * *Files identical despite different names*

### Comparing `pyguiadapter-0.3.4/pyguiadapter/res/icons/message-success.svg` & `pyguiadapter-0.3.5/pyguiadapter/res/icons/message-success.svg`

 * *Files identical despite different names*

### Comparing `pyguiadapter-0.3.4/pyguiadapter/res/icons/message-unread.svg` & `pyguiadapter-0.3.5/pyguiadapter/res/icons/message-unread.svg`

 * *Files identical despite different names*

### Comparing `pyguiadapter-0.3.4/pyguiadapter/res/icons/message.svg` & `pyguiadapter-0.3.5/pyguiadapter/res/icons/message.svg`

 * *Files identical despite different names*

### Comparing `pyguiadapter-0.3.4/pyguiadapter/res/icons/mini-sd-card.svg` & `pyguiadapter-0.3.5/pyguiadapter/res/icons/mini-sd-card.svg`

 * *Files identical despite different names*

### Comparing `pyguiadapter-0.3.4/pyguiadapter/res/icons/monitor.svg` & `pyguiadapter-0.3.5/pyguiadapter/res/icons/monitor.svg`

 * *Files identical despite different names*

### Comparing `pyguiadapter-0.3.4/pyguiadapter/res/icons/more-app.svg` & `pyguiadapter-0.3.5/pyguiadapter/res/icons/more-app.svg`

 * *Files identical despite different names*

### Comparing `pyguiadapter-0.3.4/pyguiadapter/res/icons/movie-board.svg` & `pyguiadapter-0.3.5/pyguiadapter/res/icons/movie-board.svg`

 * *Files identical despite different names*

### Comparing `pyguiadapter-0.3.4/pyguiadapter/res/icons/movie.svg` & `pyguiadapter-0.3.5/pyguiadapter/res/icons/movie.svg`

 * *Files identical despite different names*

### Comparing `pyguiadapter-0.3.4/pyguiadapter/res/icons/multi-function-knife.svg` & `pyguiadapter-0.3.5/pyguiadapter/res/icons/multi-function-knife.svg`

 * *Files identical despite different names*

### Comparing `pyguiadapter-0.3.4/pyguiadapter/res/icons/notebook-one.svg` & `pyguiadapter-0.3.5/pyguiadapter/res/icons/notebook-one.svg`

 * *Files identical despite different names*

### Comparing `pyguiadapter-0.3.4/pyguiadapter/res/icons/octagon.svg` & `pyguiadapter-0.3.5/pyguiadapter/res/icons/octagon.svg`

 * *Files identical despite different names*

### Comparing `pyguiadapter-0.3.4/pyguiadapter/res/icons/online-meeting.svg` & `pyguiadapter-0.3.5/pyguiadapter/res/icons/online-meeting.svg`

 * *Files identical despite different names*

### Comparing `pyguiadapter-0.3.4/pyguiadapter/res/icons/page-template.svg` & `pyguiadapter-0.3.5/pyguiadapter/res/icons/page-template.svg`

 * *Files identical despite different names*

### Comparing `pyguiadapter-0.3.4/pyguiadapter/res/icons/pay-code.svg` & `pyguiadapter-0.3.5/pyguiadapter/res/icons/pay-code.svg`

 * *Files identical despite different names*

### Comparing `pyguiadapter-0.3.4/pyguiadapter/res/icons/people-plus-one.svg` & `pyguiadapter-0.3.5/pyguiadapter/res/icons/people-plus-one.svg`

 * *Files identical despite different names*

### Comparing `pyguiadapter-0.3.4/pyguiadapter/res/icons/phone-incoming-one.svg` & `pyguiadapter-0.3.5/pyguiadapter/res/icons/phone-incoming-one.svg`

 * *Files identical despite different names*

### Comparing `pyguiadapter-0.3.4/pyguiadapter/res/icons/phone-incoming.svg` & `pyguiadapter-0.3.5/pyguiadapter/res/icons/phone-incoming.svg`

 * *Files identical despite different names*

### Comparing `pyguiadapter-0.3.4/pyguiadapter/res/icons/phone-missed.svg` & `pyguiadapter-0.3.5/pyguiadapter/res/icons/phone-missed.svg`

 * *Files identical despite different names*

### Comparing `pyguiadapter-0.3.4/pyguiadapter/res/icons/phone-outgoing-one.svg` & `pyguiadapter-0.3.5/pyguiadapter/res/icons/phone-outgoing-one.svg`

 * *Files identical despite different names*

### Comparing `pyguiadapter-0.3.4/pyguiadapter/res/icons/phone-outgoing.svg` & `pyguiadapter-0.3.5/pyguiadapter/res/icons/phone-outgoing.svg`

 * *Files identical despite different names*

### Comparing `pyguiadapter-0.3.4/pyguiadapter/res/icons/phone-telephone.svg` & `pyguiadapter-0.3.5/pyguiadapter/res/icons/phone-telephone.svg`

 * *Files identical despite different names*

### Comparing `pyguiadapter-0.3.4/pyguiadapter/res/icons/phone-video-call.svg` & `pyguiadapter-0.3.5/pyguiadapter/res/icons/phone-video-call.svg`

 * *Files identical despite different names*

### Comparing `pyguiadapter-0.3.4/pyguiadapter/res/icons/platte.svg` & `pyguiadapter-0.3.5/pyguiadapter/res/icons/platte.svg`

 * *Files identical despite different names*

### Comparing `pyguiadapter-0.3.4/pyguiadapter/res/icons/ppt.svg` & `pyguiadapter-0.3.5/pyguiadapter/res/icons/ppt.svg`

 * *Files identical despite different names*

### Comparing `pyguiadapter-0.3.4/pyguiadapter/res/icons/record-disc.svg` & `pyguiadapter-0.3.5/pyguiadapter/res/icons/record-disc.svg`

 * *Files identical despite different names*

### Comparing `pyguiadapter-0.3.4/pyguiadapter/res/icons/record.svg` & `pyguiadapter-0.3.5/pyguiadapter/res/icons/record.svg`

 * *Files identical despite different names*

### Comparing `pyguiadapter-0.3.4/pyguiadapter/res/icons/rename.py` & `pyguiadapter-0.3.5/pyguiadapter/res/icons/rename.py`

 * *Files identical despite different names*

### Comparing `pyguiadapter-0.3.4/pyguiadapter/res/icons/rule-two.svg` & `pyguiadapter-0.3.5/pyguiadapter/res/icons/rule-two.svg`

 * *Files identical despite different names*

### Comparing `pyguiadapter-0.3.4/pyguiadapter/res/icons/ruler-one.svg` & `pyguiadapter-0.3.5/pyguiadapter/res/icons/ruler-one.svg`

 * *Files identical despite different names*

### Comparing `pyguiadapter-0.3.4/pyguiadapter/res/icons/ruler.svg` & `pyguiadapter-0.3.5/pyguiadapter/res/icons/ruler.svg`

 * *Files identical despite different names*

### Comparing `pyguiadapter-0.3.4/pyguiadapter/res/icons/sd-card.svg` & `pyguiadapter-0.3.5/pyguiadapter/res/icons/sd-card.svg`

 * *Files identical despite different names*

### Comparing `pyguiadapter-0.3.4/pyguiadapter/res/icons/setting-computer.svg` & `pyguiadapter-0.3.5/pyguiadapter/res/icons/setting-computer.svg`

 * *Files identical despite different names*

### Comparing `pyguiadapter-0.3.4/pyguiadapter/res/icons/setting-laptop.svg` & `pyguiadapter-0.3.5/pyguiadapter/res/icons/setting-laptop.svg`

 * *Files identical despite different names*

### Comparing `pyguiadapter-0.3.4/pyguiadapter/res/icons/setting-two.svg` & `pyguiadapter-0.3.5/pyguiadapter/res/icons/setting-two.svg`

 * *Files identical despite different names*

### Comparing `pyguiadapter-0.3.4/pyguiadapter/res/icons/share-one.svg` & `pyguiadapter-0.3.5/pyguiadapter/res/icons/share-one.svg`

 * *Files identical despite different names*

### Comparing `pyguiadapter-0.3.4/pyguiadapter/res/icons/system.svg` & `pyguiadapter-0.3.5/pyguiadapter/res/icons/system.svg`

 * *Files identical despite different names*

### Comparing `pyguiadapter-0.3.4/pyguiadapter/res/icons/table-file.svg` & `pyguiadapter-0.3.5/pyguiadapter/res/icons/table-file.svg`

 * *Files identical despite different names*

### Comparing `pyguiadapter-0.3.4/pyguiadapter/res/icons/tape.svg` & `pyguiadapter-0.3.5/pyguiadapter/res/icons/tape.svg`

 * *Files identical despite different names*

### Comparing `pyguiadapter-0.3.4/pyguiadapter/res/icons/test-tube.svg` & `pyguiadapter-0.3.5/pyguiadapter/res/icons/test-tube.svg`

 * *Files identical despite different names*

### Comparing `pyguiadapter-0.3.4/pyguiadapter/res/icons/thermometer.svg` & `pyguiadapter-0.3.5/pyguiadapter/res/icons/thermometer.svg`

 * *Files identical despite different names*

### Comparing `pyguiadapter-0.3.4/pyguiadapter/res/icons/topic-discussion.svg` & `pyguiadapter-0.3.5/pyguiadapter/res/icons/topic-discussion.svg`

 * *Files identical despite different names*

### Comparing `pyguiadapter-0.3.4/pyguiadapter/res/icons/topic.svg` & `pyguiadapter-0.3.5/pyguiadapter/res/icons/topic.svg`

 * *Files identical despite different names*

### Comparing `pyguiadapter-0.3.4/pyguiadapter/res/icons/tree-list.svg` & `pyguiadapter-0.3.5/pyguiadapter/res/icons/tree-list.svg`

 * *Files identical despite different names*

### Comparing `pyguiadapter-0.3.4/pyguiadapter/res/icons/triangle-ruler.svg` & `pyguiadapter-0.3.5/pyguiadapter/res/icons/triangle-ruler.svg`

 * *Files identical despite different names*

### Comparing `pyguiadapter-0.3.4/pyguiadapter/res/icons/vial.svg` & `pyguiadapter-0.3.5/pyguiadapter/res/icons/vial.svg`

 * *Files identical despite different names*

### Comparing `pyguiadapter-0.3.4/pyguiadapter/res/icons/video.svg` & `pyguiadapter-0.3.5/pyguiadapter/res/icons/video.svg`

 * *Files identical despite different names*

### Comparing `pyguiadapter-0.3.4/pyguiadapter/res/icons/view-grid-card.svg` & `pyguiadapter-0.3.5/pyguiadapter/res/icons/view-grid-card.svg`

 * *Files identical despite different names*

### Comparing `pyguiadapter-0.3.4/pyguiadapter/res/icons/view-grid-detail.svg` & `pyguiadapter-0.3.5/pyguiadapter/res/icons/view-grid-detail.svg`

 * *Files identical despite different names*

### Comparing `pyguiadapter-0.3.4/pyguiadapter/res/icons/view-grid-list.svg` & `pyguiadapter-0.3.5/pyguiadapter/res/icons/view-grid-list.svg`

 * *Files identical despite different names*

### Comparing `pyguiadapter-0.3.4/pyguiadapter/res/icons/voice-input.svg` & `pyguiadapter-0.3.5/pyguiadapter/res/icons/voice-input.svg`

 * *Files identical despite different names*

### Comparing `pyguiadapter-0.3.4/pyguiadapter/res/icons/voice-message.svg` & `pyguiadapter-0.3.5/pyguiadapter/res/icons/voice-message.svg`

 * *Files identical despite different names*

### Comparing `pyguiadapter-0.3.4/pyguiadapter/res/icons/voice-one.svg` & `pyguiadapter-0.3.5/pyguiadapter/res/icons/voice-one.svg`

 * *Files identical despite different names*

### Comparing `pyguiadapter-0.3.4/pyguiadapter/res/icons/weixin-mini-app.svg` & `pyguiadapter-0.3.5/pyguiadapter/res/icons/weixin-mini-app.svg`

 * *Files identical despite different names*

### Comparing `pyguiadapter-0.3.4/pyguiadapter/res/icons/wifi.svg` & `pyguiadapter-0.3.5/pyguiadapter/res/icons/wifi.svg`

 * *Files identical despite different names*

### Comparing `pyguiadapter-0.3.4/pyguiadapter/res/icons/zip.svg` & `pyguiadapter-0.3.5/pyguiadapter/res/icons/zip.svg`

 * *Files identical despite different names*

### Comparing `pyguiadapter-0.3.4/pyguiadapter/tools/easyconfigs/constants.py` & `pyguiadapter-0.3.5/pyguiadapter/tools/easyconfigs/constants.py`

 * *Files identical despite different names*

### Comparing `pyguiadapter-0.3.4/pyguiadapter/tools/easyconfigs/helper/const_name_value.py` & `pyguiadapter-0.3.5/pyguiadapter/tools/easyconfigs/helper/const_name_value.py`

 * *Files identical despite different names*

### Comparing `pyguiadapter-0.3.4/pyguiadapter/tools/easyconfigs/helper/imports.py` & `pyguiadapter-0.3.5/pyguiadapter/tools/easyconfigs/helper/imports.py`

 * *Files identical despite different names*

### Comparing `pyguiadapter-0.3.4/pyguiadapter/tools/easyconfigs/helper/parameter_constants.py` & `pyguiadapter-0.3.5/pyguiadapter/tools/easyconfigs/helper/parameter_constants.py`

 * *Files identical despite different names*

### Comparing `pyguiadapter-0.3.4/pyguiadapter/tools/easyconfigs/helper/parameter_widget_configs.py` & `pyguiadapter-0.3.5/pyguiadapter/tools/easyconfigs/helper/parameter_widget_configs.py`

 * *Files identical despite different names*

### Comparing `pyguiadapter-0.3.4/pyguiadapter/tools/easyconfigs/impl.py` & `pyguiadapter-0.3.5/pyguiadapter/tools/easyconfigs/impl.py`

 * *Files identical despite different names*

### Comparing `pyguiadapter-0.3.4/pyguiadapter/tools/easyconfigs/structures.py` & `pyguiadapter-0.3.5/pyguiadapter/tools/easyconfigs/structures.py`

 * *Files identical despite different names*

### Comparing `pyguiadapter-0.3.4/pyguiadapter/tools/easyconfigs/tpl/configs.tpl` & `pyguiadapter-0.3.5/pyguiadapter/tools/easyconfigs/tpl/configs.tpl`

 * *Files identical despite different names*

### Comparing `pyguiadapter-0.3.4/pyguiadapter/tools/easyconfigs/utils.py` & `pyguiadapter-0.3.5/pyguiadapter/tools/easyconfigs/utils.py`

 * *Files identical despite different names*

### Comparing `pyguiadapter-0.3.4/pyguiadapter/ui/config.py` & `pyguiadapter-0.3.5/pyguiadapter/ui/config.py`

 * *Files identical despite different names*

### Comparing `pyguiadapter-0.3.4/pyguiadapter/ui/generated/ui_class_init_window.py` & `pyguiadapter-0.3.5/pyguiadapter/ui/generated/ui_class_init_window.py`

 * *Files identical despite different names*

### Comparing `pyguiadapter-0.3.4/pyguiadapter/ui/generated/ui_execution_window.py` & `pyguiadapter-0.3.5/pyguiadapter/ui/generated/ui_execution_window.py`

 * *Files identical despite different names*

### Comparing `pyguiadapter-0.3.4/pyguiadapter/ui/generated/ui_selection_window.py` & `pyguiadapter-0.3.5/pyguiadapter/ui/generated/ui_selection_window.py`

 * *Files identical despite different names*

### Comparing `pyguiadapter-0.3.4/pyguiadapter/ui/menus.py` & `pyguiadapter-0.3.5/pyguiadapter/ui/menus.py`

 * *Files identical despite different names*

### Comparing `pyguiadapter-0.3.4/pyguiadapter/ui/styles.py` & `pyguiadapter-0.3.5/pyguiadapter/ui/styles.py`

 * *Files identical despite different names*

### Comparing `pyguiadapter-0.3.4/pyguiadapter/ui/utils.py` & `pyguiadapter-0.3.5/pyguiadapter/ui/utils.py`

 * *Files identical despite different names*

### Comparing `pyguiadapter-0.3.4/pyguiadapter/ui/window/class_init/impl.py` & `pyguiadapter-0.3.5/pyguiadapter/ui/window/class_init/impl.py`

 * *Files identical despite different names*

### Comparing `pyguiadapter-0.3.4/pyguiadapter/ui/window/func_execution/base.py` & `pyguiadapter-0.3.5/pyguiadapter/ui/window/func_execution/base.py`

 * *Files identical despite different names*

### Comparing `pyguiadapter-0.3.4/pyguiadapter/ui/window/func_execution/config.py` & `pyguiadapter-0.3.5/pyguiadapter/ui/window/func_execution/config.py`

 * *Files identical despite different names*

### Comparing `pyguiadapter-0.3.4/pyguiadapter/ui/window/func_execution/constants.py` & `pyguiadapter-0.3.5/pyguiadapter/ui/window/func_execution/constants.py`

 * *Files identical despite different names*

### Comparing `pyguiadapter-0.3.4/pyguiadapter/ui/window/func_execution/context.py` & `pyguiadapter-0.3.5/pyguiadapter/ui/window/func_execution/context.py`

 * *Files identical despite different names*

### Comparing `pyguiadapter-0.3.4/pyguiadapter/ui/window/func_execution/impl.py` & `pyguiadapter-0.3.5/pyguiadapter/ui/window/func_execution/impl.py`

 * *Files identical despite different names*

### Comparing `pyguiadapter-0.3.4/pyguiadapter/ui/window/func_selection/config.py` & `pyguiadapter-0.3.5/pyguiadapter/ui/window/func_selection/config.py`

 * *Files identical despite different names*

### Comparing `pyguiadapter-0.3.4/pyguiadapter/ui/window/func_selection/impl.py` & `pyguiadapter-0.3.5/pyguiadapter/ui/window/func_selection/impl.py`

 * *Files identical despite different names*

### Comparing `pyguiadapter-0.3.4/pyproject.toml` & `pyguiadapter-0.3.5/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "pyguiadapter"
-version = "0.3.4"
+version = "0.3.5"
 description = "turn (almost) any python functions into a gui in a few lines of code"
 authors = ["zimolab <zimolab@aliyun.com>"]
 readme = "README.md"
 homepage = "https://github.com/zimolab/PyGUIAdapter"
 repository = "https://github.com/zimolab/PyGUIAdapter"
 documentation = "https://github.com/zimolab/PyGUIAdapter"
```

### Comparing `pyguiadapter-0.3.4/README.md` & `pyguiadapter-0.3.5/README.md`

 * *Files identical despite different names*

### Comparing `pyguiadapter-0.3.4/PKG-INFO` & `pyguiadapter-0.3.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyguiadapter
-Version: 0.3.4
+Version: 0.3.5
 Summary: turn (almost) any python functions into a gui in a few lines of code
 Home-page: https://github.com/zimolab/PyGUIAdapter
 Author: zimolab
 Author-email: zimolab@aliyun.com
 Requires-Python: >=3.8,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
```
